---
title: "EN-CONFIG-AW_Enterprise_B2B_Service_ERP_WS"
source: "EN-CONFIG-AW_Enterprise_B2B_Service_ERP_WS.pdf"
tags: ["A+W Enterprise", "B2B Service", "ERP Webservice", "DORMA", "openTRANS", "Configuration", "Technical Documentation", "API", "Software for Glass"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This internal document provides configuration details for the A+W Enterprise B2B Service, focusing on its integration with the ERP Webservice. It covers setup for DORMA purchase orders, openTRANS document transfers (invoices and delivery notes), and general troubleshooting for the webservice."
long_description: "This is an internal technical configuration guide for the A+W Enterprise B2B Service, a component that facilitates Business-to-Business communication between the A+W Enterprise (AWE) system and external partners via an ERP Webservice. The document outlines the historical development and functionality of the service. Initially, it was designed to handle DORMA purchase orders using the openTRANS 1.0 format. It later expanded to support generic invoice and delivery note transfers using the more current openTRANS 2.1 standard, including the ability to generate and store these documents as XML files. The guide provides detailed configuration instructions for specific use cases. For DORMA purchase orders, it covers database updates, CommonBase settings (and its subsequent deprecation), licensing notes, and comprehensive troubleshooting for connection problems, remote certificate errors, and specific error messages from the Dorma system. For openTRANS document transfers, it explains the logic for triggering invoice and delivery note generation, the necessary environment variables, data mapping for XML output, and special considerations for internal charging scenarios (like for SGG/Caleoglas). The document also includes technical details on table configurations (mpdfuectrl, ottransfer), API URLs, and general troubleshooting steps for the ERP Webservice, such as resolving URL format exceptions and log file issues."
---

# A+W Configuration
# A+W Enterprise B2B Service feat. ERP Webservice

- -INTERNAL-

A+W - Software for Glass

---
## Change history
| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2019-02-05 | Original version | Transfer from Dokuware document | 1.0 |
| 2022-05-03 | SVH | ISO country code in address element `<COUNTRY>` - PF [AW-106274] | |
| 2022-11-16 | SVH | Dorma server certificate | |
| 2022-12-07 | SVH | Dorma Service unavailable | |
| 2022-12-19 | SVH | [AW-130251] - new Dorma Webservice URL | |
| 2023-01-06 | SVH | Note about A+W license for Dorma purchase orders | |
| 2023-01-18 | SVH | Transfer documentation of the internal calculation from this document to the special document | |

## Content

1.  **General information**
    1.1. General remark about document transfer/export
    1.2. B2B Service and the CommonBase
    1.3. B2B Service and the Informix-Client
2.  **DORMA purchase orders**
    2.1. General Information
    2.2. Additional documentation
    2.3. Installation and configuration
        2.3.1. Expansion of the CommonBase (AWDesk case #207909)
        2.3.2. Note about the A+W license
        2.3.3. DB update
        2.3.4. Table mpdfuectrl
    2.4. External customer number in the DORMA purchase order (AWDesk case #251625 + case #254109)
    2.5. No takeover of quantity units
    2.6. Sending e-mails
        2.6.1. Configuration (status as of 01/19/2019)
        2.6.2. Version 3.5 (2009)
        2.6.3. Perils
    2.7. Ottransfer
    2.8. Dorma webservice
        2.8.1. Dorma Webservice URL
        2.8.2. No connection to the Dorma webservice
        2.8.3. The underlying connection was closed: no protected channel for capital SSL/TLS could be established
        2.8.4. "Unable to connect to the remote server"
        2.8.5. Problems with the remote certificate
        2.8.6. Service Unavailable
    2.9. Sending e-mail/storing the purchase order confirmation (AWDesk #280451)
    2.10. Troubleshooting / error messages
        2.10.1. DORMA Order Response wit error
        2.10.2. DORMA Order Response with error V0004
        2.10.3. DORMA Order Response with error V9999
        2.10.4. DORMA purchase order cannot be generated
3.  **Document export/transfer**
    3.1. openTRANS document transfer
        3.1.1. Documentation
        3.1.2. Entry in table ottransfer (AWDesk #350373)
        3.1.3. Check
        3.1.4. Output and storage of XML documents in openTRANS Version 2.1 (Version 1.0 is not supported)
    3.2. Internal charging (special version of the openTRANS document transfer for SGG/Caleoglas)
    3.3. Automatic warehouse in / delivery note generation for direct delivery (AWDesk #334475)
        3.3.1. env variables
        3.3.2. Input tables
        3.3.3. Trigger record in aufint
        3.3.4. Restrictions
        3.3.5. Additional documentation/troubleshooting
    3.4. Troubleshooting
        3.4.1. Assignment of the webservice user for the "customer" webservice
        3.4.2. No access to database possible (from ERP webservice)
        3.4.3. B2B service does not write log to the desired log depth
        3.4.4. B2B service/ERP webservice crash with internal charging
4.  **General data mapping**
    4.1. openTRANS address element `<COUNTRY>`
5.  **Troubleshooting (general)**
    5.1. ERP Webservice URL: UriFormatException
    5.2. ERP webservice does not write a log
    5.3. ERP webservice does not write log to the desired log depth
    5.4. ERP webservice (import) cannot be addressed

## 1. General information

Previously, the basic functionality of the B2B service was to make available AWE data in the openTRANS format and to transfer it. There is a logic for the creation and transfer of DORMA POs and a document export that creates and transfers invoice and delivery note documents.

### 1.1. General remark about document transfer/export

The logic of the B2B service is very unclear overall, which is due to the history.

First in AWE there was the DORMA purchase order transfer, which uses the openTRANS format, and the special logic of the internal charging for SGG (invoice transfer). Both logics use the openTRANS format 1.0.

At the time when the internal charging was implemented, there was not yet a need to generate an openTRANS xml as file. The format was used by internal charging as an object that was generated by a webservice and then transferred via webservice to another site and processed further there (-> filling of the eingang* tables). In the process, the non-redistributed discounts are transferred as invoice items with "user-defined extensions." These structures do not correspond to the openTRANS standard.

Later on, a delivery note transfer (internal charging does an invoice transfer) according to the same principle was added. When the delivery note transfer was implemented, the current openTRANS format was already Version 2.1, which is why the delivery note transfer was implemented with the format 2.1.

In turn later on, xml documents were needed after all, and as quickly as possible, which is why these documents were wrested from the existing logic. The logic of internal charging could not yet process collective invoices, therefore with this logic, no xml document for a collective invoice can be created.

In 2017, we began to expand the B2B service in Version 6 so that it can generate openTRANS invoices and delivery notes in the openTRANS 2.1 format without restrictions. For this functionality, only the B2B service is needed (NO ERP webservice!), therefore, the version of an installed ERP webservice is irrelevant here. Discounts that are not redistributed are written to regular discount structures with this logic; these comply with the openTRANS standard.

In this new logic, collective invoices also work.

A tabular overview of the various functions is in the "other" configuration document for the B2B where the functions are described that do not need any ERP web service.

In order to do its work, the B2B service 6 needs the current table structure of table ottransfer. If the logic should be installed with an AWE backend with Version < 6, then attention must be paid that the table ottransfer is brought up to date using scripts.

In the AWE backend versions < 6, the trigger records in ottransfer are NOT written by the program for this logic; they have to be generated via customizing.

The description of the new B2B functionality without ERP Webservice is in the document EN-CONFIG A+W Enterprise B2B Service.docx

Documentation of the openTRANS standard (versions 1.0 and 2.1) is available on the Internet site www.opentrans.de. Furthermore, it is stored internally at A+W under `\\jupiter\Doku_DocuWare\Interfaces\openTrans`.

### 1.2. B2B Service and the CommonBase

Unfortunately, the CommonBase was only removed with ALCIB Version 2011 (4.5), B2B Service 3.6. This means that for an installation with an ALCIB 2009 (4.4), the CommonBase is still required.

> **CAUTION**
> If you have configured database access in the CommonBase and then you click around more, it can happen that the password is not saved correctly. In this case, it is necessary to re-configure it.

### 1.3. B2B Service and the Informix-Client

See also case 268201.
The B2B service does not run with all client SDK versions.
- Client-SDK 3.50 TC3 works!
- (Client-SDK 3.50 TC5 does NOT work!)
- Whether Client-SDK 3.50 TC4 works is not known.

## 2. DORMA purchase orders

### 2.1. General Information

See also AWDesk 90727, under this case there is also a description (release notes).
DORMA purchase orders are purchase orders for DORMA articles for DORMA from AWE. The prerequisite for this is that the articles to be ordered were previously transmitted to AWE via the DORMA master data import (BMECAT) by DORMA.
The entry of the interface data into the table ottransfer is done via REP/rep/dormaueb.rep

### 2.2. Additional documentation

- `\\jupiter\DOKU_DocuWare\AWEnterprise\B2B_DORMA`
- `\\jupiter\Doku DocuWare\AWEnterprise\B2B_DORMA\User Manuals\D-AWE-HB-AWB2B.pdf`

### 2.3. Installation and configuration

#### 2.3.1. Expansion of the CommonBase (AWDesk case #207909)

From Version 3.67 on, the B2B service (and thus also the DORMA interface) is operated without the CommonBase.
All settings that were previously made in the CommonBase are now made directly in ALCIB.
The order interface without CommonBase works with version ALCIB 2011 (4.5) or higher.

#### 2.3.2. Note about the A+W license

Previously an A+W license was required for the Dorma interface. In the current version, this is no longer the case.

#### 2.3.3. DB update

In order to be able to perform the configuration, the tables aldfuetyp and aldfuectrl must be up-to-date.
See document `\\jupiter\Doku DocuWare\ALCIB-PMS\INSTALLATION-UPDATE\Installation Configuration\aldfuetyp aldfuectrl.docx`

#### 2.3.4. Table mpdfuectrl

On the dialog System > Data Transfer > Transaction Transfer > Configuration, all settings are stored that were previously stored in the CommonBase.
For the DORMA order interface, partner type "Supplier" and market partner "" must be selected (caution: market partner generally, that is "0," the DORMA supplier, may not be entered here!).

In the field "Type of the EDI", the EDI type is specified:
- Type 109 Dorma interface

| aldfuectrl ID | Data Type | Designation |
| :--- | :--- | :--- |
| 6 | alphanum. | Dorma Webservice URL |
| 9 | alphanum. | Dorma Webservice User <br> The user is apparently always a numeric value followed by a string, connected with an underscore. Example: "12345_test" <br> The numeric value must, as it seems always be at the start of the user name. <br> See also PF [AW-87836]. |
| 10 | alphanum. | Dorma Webservice Password |
| 11 | alphanum. | ERP server name (unix), same entry as in the AWE env variable `AWC_ALCIB_SERVER_NAME` |
| 12 | alphanum. | ERP server socket port (unix), same entry as in AWE env variable `AWC_PORT_CONTROL_SERVER` |

### 2.4. External customer number in the DORMA purchase order (AWDesk case #251625 + case #254109)

**Up to and including ALCIB 2008**

Up to ALCIB Version 2008 (ErpWebservice 2.0, B2B service 2.0), the customer number transferred in the purchase order to DORMA was determined as follows:
- A purchase order in ALCIB always has a site assignment (kauf.hausnr).
- For the site of the purchase order, the associated customer number (xhaus.kunr) is searched for in xhaus.
- Then for the customer number from xhaus from mp, the associated external customer number (mp.extkundnr) is determined.

This external customer number is transferred to DORMA.

If no external customer number is stored, an exception is logged in the B2B service log, which unfortunately is not very meaningful:

```
12-04-2012 11:40:19 error, Albwir.Edi.OpenTrans:
OpenTransDORMAOrder.GenerateDocument():System.Web.Services.Protocols.SoapException:
The request could not be processed by the server. ---> System. FormatException: The input
character string has the incorrect format.
for System.Number.StringToNumber(String str, NumberStyles options, NumberBuffer& number,
NumberFormatInfo info, Boolean parseDecimal)
for System.Number.ParseInt32(String s, NumberStyles style, NumberFormatInfo info)
for
Albwir.Erp.WebService.OpenTrans.AlcibOpenTransDORMAOrderAdapter.ExportOpenTransDORM
AOrder(Int32 documentNo, ORDER& orderData, ExportInfo& exportInfo)
for Albwir.Erp.WebService.ErpDataService.OpenTransExportDORMAOrder(Int32 documentNo,
ORDER& orderData, ExportInfo& exportInfo)
--- End of the internal exception stack monitoring ---
```

**From and including ALCIB 2009 on**

From ALCIB Version 2998 (ErpWebservice 3.5, B2B service 3.5), the customer number transferred to DORMA is determined in two stages:
- First, there is a search for the external customer number in the master data of the DORMA supplier
- If an external customer number is entered there, this customer number is transferred to DORMA
- If for DORMA suppliers no external customer number is stored, there is a search according to the "old" logic (see above) for an external customer number.

If no external customer number can be determined, this is logged clearly in the ErpWebservice log and an exception is thrown, which in turn is logged in the B2B service log.

### 2.5. No takeover of quantity units

See case 253061.
The quantity unit (mussken.gv1) is not taken over during the master data import. The mussken records then have to be adjusted after the fact (by hand).

### 2.6. Sending e-mails

#### 2.6.1. Configuration (status as of 01/19/2019)

Currently it is the case that the e-mail configuration is obtained from mpdfuectrl, for the "type of EDI" 110 (that is, "general").
The recipient is replaced after the fact by the contact e-mail address from the Dorma purchase order, so that in the end, the e-mail does not go to the configured recipient from mptfuctrl, but only to the CC recipients stored there.
See also AWDesk #427847.

#### 2.6.2. Version 3.5 (2009)

A notification e-mail will be sent to the author (euser) of the purchase order. If no e-mail address is stored for the author, the e-mail is sent to the address that is stored in the CommonBase.

#### 2.6.3. Perils

It can be that the sending of an e-mail from the B2B service is blocked by the SMTP server or the virus scanner or the firewall.
For example, if the McAfee on ws-mader-visa believes that the B2B service is a tool for sending mass e-mails (worm), because the application has no window. An e-mail can only be sent if the checking for mass e-mail worms in McAfee is switched off.

### 2.7. Ottransfer

DORMA purchase order records are written to ottransfer via REP/rep/dormaueb.rep.
Starting with Version 2009 (4.5), the table ottransfer includes the column subno, otherwise there is a SOAP format exception.

### 2.8. Dorma webservice

#### 2.8.1. Dorma Webservice URL

(Status as of 12/19/2022)

The Dorma Webservice URL (Production) is: https://shop.dorma-glas.com/soapdorma/receive/dormakaba/prod
The old URL is no longer valid.

The new DORMA Webservice address can no longer be called up in the browser for testing. Dorma's new security concept includes suppressing the call via the browser.

As TLS version for the encryption, currently TLS 1.2 (and higher) are permitted.

The new test Webservice URL is:
https://shop.dorma-glas.com/soapdorma/receive/dormakaba/dev

See PF [AW-130251].

Calling the URL with `?wsdl` at the end causes the URL called up to return an xml document with the description of the functionality of the Webservice:
- **Produktive WebService:** https://shop.dorma-glas.com/soapdorma/receive/dormakaba/prod?wsdl
- **Test Webservice:** https://shop.dorma-glas.com/soapdorma/receive/dormakaba/dev?wsdl

(status as of 01/15/2019)

The link for the webservice (production) is: `https://shop.dorma-glas.com/wp/ws_d.php?webservice-glas`

A list of the available business processes can also be determined using the URL: `https://shop.dormaglas.com/dorma_shops/webservice/dev/webservice_dorma.php?webservice=glas`.

The link for the test webservice is: `https://shop.dorma-glas.com/wp/ws_d.php?webservice-glas`

In the older Dorma documentation "Documentation of Webservice WDI.pdf," some of the specifications of the URLs are imprecise. The URL includes an `&wsdl` at the end. This specification causes the URL called up to deliver an XML document with the description of the functionality of the webservice.

If a webservice function should be called directly, the URL must be used without `&wsdl`.
See also AWDesk #427847.

#### 2.8.2. No connection to the Dorma webservice

If there is no access to the remote webservice, this can be because of the user or the password. However, it can also be that the routing is not in order at the customer. That is, the customer has to test whether he can connect to the webservice when he enters the URL into the browser on his computer.

#### 2.8.3. The underlying connection was closed: no protected channel for capital SSL/TLS could be established

See also #336813
Possible solution approaches:
- New certificate must be installed (then restart IIS)
- Reboot the computer

#### 2.8.4. "Unable to connect to the remote server"

Via the browser, it is possible to call up the Dorma webservice without a problem, but the B2B service cannot establish a connection. The extended exception message reads:
> "A connection attempt failed because the connected party did not properly respond after a period of time, or established connection failed because connected host has failed to respond `<IP address>:<Port>`"

Possible solution: the firewall is blocking the routing to the Dorma webservice.
If the local firewall is not active on the system in question, but instead there is a firewall system via proxy server/router, the person responsible (for the customer's) IT has to view the log files in order to identify the blockage. A firewall rule has to be set up, which permits the addressing of the Dorma webservice by the B2B service.
See also PF-Ticket [AW-68568].

#### 2.8.5. Problems with the remote certificate

For years, the HTTPS communications protocol has been used to call up the Dorma webservice. HTTPS guarantees security in communication by encrypting the contents and authenticating the webserver and website.

The Dorma webserver authenticates itself using a server certificate on the client (here, the AWE B2B service).
A server certificate is issued by an official certification office. It has a limited validity period.

When the following error message (B2B service protocol) occurs when calling up the Dorma webservice:

> The underlying connection was terminated: No position of trust could be issued for the protected SSL/TLS channel.
> The remote certificate is invalid according to the validation procedure.

This indicates that the server certificate provided by Dorma is flawed or expired.
This problem cannot be solved on the client page (in this case, B2B service).
The affected customer (or, under some circumstances, also A+W Support) must ask at Dormy why there are certificate problems and whether the certificate is expired and must be reissued.
As a transitional solution, it is also possible to inquire at Dorma whether an addressing of the Dorma webservice via an insecure connection (HTTP instead of HTTPS) is possible temporarily until the problem has been solved on the Dorma side.
See also PF [AW-125913].

#### 2.8.6. Service Unavailable

If the Dorma Webshop cannot be reached via the browser ("Service unavailable" message), the problem is actually with the Dorma Webshop and not the B2B service. As a result, it is necessary to contact Dorma customer service.

> **Service Unavailable**
> The server is temporarily unable to service your request due to maintenance downtime or capacity problems. Please try again later.

See also PF [AW-130251].

### 2.9. Sending e-mail/storing the purchase order confirmation (AWDesk #280451)

When configuring DORMA purchase orders in ALCIB / AWE without CommonBase (i.e., after ALCIB Version 2011) you also configure how to e-mail DORMA order confirmations (send report) in the ERP system. If the configuration doesn't exist or is incomplete you cannot send an e-mail. Instead, the log file of the B2B Service shows the TEMP path (plus file name) where you can find the order confirmations in HTML format.

To determine the TEMP path, (starting with Version AWE 6), the following Windows environment variables (Caution! These are the variable settings for the B2B service user!) must be checked:
- TMP
- TEMP
- USERPROFILE

The first variable assigned is used. If none is set, the Windows path will be used.

The configuration of e-mail sending is done using the entries in the table mpdfuectrl. The entries are made via the dialogue: System > File Transfer > Transaction Transfer > Configuration.

That the configuration can be done on the dialog, in versions before AWE 5.2 and in ALCIB 2011, table entries in the tables aldfuetyp and aldfuectrl must be maintained.
See document `\\jupiter\Doku DocuWare\ALCIB-PMS\INSTALLATION-UPDATE\Installation Configuration\aldfuetyp aldfuectrl.docx`

Furthermore, the alcib binfile must be up-to-date (see Case 280451)!

All entries for the e-mail sending must be made for the market partner type "supplier" with market partner number 0. As "Type of the EDI", the number 110 (type "General") must be entered. For this EDI, the control types with the capital IDs 28 to 36, as needed, must be configured.
Control types that are optional (e.g. authentication) do not have to be configured as long as they are not needed.

| aldfuectrl ID | Data Type | Designation |
| :--- | :--- | :--- |
| 28 | alphanum. | E-mail server <br> Probably corresponds to the entry in the env variables SMTP_MAIL_SERVER. |
| 29 | num. | E-mail port <br> Does not have to be specified. |
| 30 | alphanum. | E-mail sender |
| 31 | alphanum. | E-mail recipient |
| 32 | alphanum. | E-Mail CC (optional) |
| 33 | Checkbox | Use Authentication (optional) |
| 34 | Checkbox | Enable SSL |
| 35 | alphanum. | E-Mail User (Account) (optional) |
| 36 | alphanum. | E-mail password (optional) |

Please note that the current version of the B2B service must be installed (see case 280451).

### 2.10. Troubleshooting / error messages

#### 2.10.1. DORMA Order Response with error

Dorma sends various error messages.
- V0001
- V0003
- V0004
- V0005
- V0006
- V1382
- V9999

Some of these errors will be listed below with special explanations.
The error messages that are not explained in detail here are found in the following document: `\\jupiter\Doku DocuWare\AWEnterprise\B2B_DORMA\User Manuals\D-AWE-HB-AWB2B.pdf`
Under some circumstances, AWDesk #90272, activity #450125 may also help.

#### 2.10.2. DORMA Order Response with error V0004

Dorma could not import the P.O. The problem has to be handled by Dorma. Please contact Dorma to clarify the situation.
Possible cause: an article ordered was taken out of the program by Dorma (AWDesk #458103, PF [AW-34468])
See also #349178,338518

#### 2.10.3. DORMA Order Response with error V9999

"Response without supplier order id from Dorma"

This could be because of missing supplier article number and designation, color numbers of the purchase order items.
- -> Check purchase order items
- -> Perhaps you will also find a hint about the problem in the capital ERP webservice
See also AWDesk #434943, #277594

#### 2.10.4. DORMA purchase order cannot be generated

> GetPurchaseOrderData() Exception: the index was outside the array range.
> OpenTransDORMAOrder.GenerateDocument(): the request could not be processed by the server.
> ---> The index was outside the array range.

There are purchase order items without poszu records (-> color)
See also AWDesk # 421963

## 3. Document export/transfer

### 3.1. openTRANS document transfer

#### 3.1.1. Documentation

- **See:** `\\jupiter\DOKU DocuWare\ALCIB-PMS\!General\Release Documents\2011\ReleaseNotes\DE-ALCIB-2011-ERN-IN-Dokumentenübertragung-openTrans.docx`
- **Description of the XML file:** `\\jupiter\DOKU_DocuWare\ALCIB-PMS\ENTERPRISE-MODULE\ERPWebservice\openTrans-Alcib-DB-Doku.xls`

#### 3.1.2. Entry in table ottransfer (AWDesk #350373)

The logic for entry in the table ottransfer was reworked with AWDesk #350373. (Logic available starting with version 5.3)

An entry in the table ottransfer occurs with invoice or delivery note generation (more precisely: on approval) if the following preconditions are fulfilled:

**A) Invoice approval**
- a. for the customer of the invoice, the flag "Invoice transfer" (mp.rechdfuekz) is activated in the market partner master data AND the customer is an external customer (no entry for the customer number in xhaus), in this case the entry type of the reference order is not important
- b. for the customer of the invoice, the flag "Invoice transfer" (mp.rechdfuekz) is activated in the market partner master data AND the customer is an internal customer (entry for the customer number in xhaus) AND kauf.eingang of the reference order is "4", this means the order was transferred via EDI

The same prerequisites as for invoices apply for credits. If the prerequisites are fulfilled as described, credits are also transferred.

**B) Release delivery note**
- a. for the customer of the delivery note, the flag "Delivery note transfer" (mp.liefdfuekz) is activated in the market partner master data AND the customer is an external customer (no entry for the customer number in xhaus), in this case the entry type of the reference order is not important
- b. for the customer of the delivery note, the flag "Delivery note transfer" (mp.liefdfuekz) is activated in the market partner master data AND the customer is an internal customer (entry for the customer number in xhaus) AND kauf.eingang of the reference order is "4", this means the order was transferred via EDI

**General note about the determination of the reference order**

The reference order CANNOT be determined via a reference chain that is as long as you want. Valid is a one-time referencing of an invoice to a credit note or a credit note to an invoice. After that, the reference must be directly to the order or delivery note.
See PF [AW-84943].

**env variables**

For the invoice/credit generation (also with the logic for internal charging), the following env variables must be activated:
- invoices: `OPENTRANS_XMLINVOICE = ON` (-> AWDesk #350373)
- credits: `OPENTRANS_XMLCREDITNOTE = ON` (-> AWDesk #350378)

#### 3.1.3. Check

**Environment variables**
- `AUTO_EK_KONTROLLE` must be deactivated
- `AUTO_EK_TRANS_VERS` must be deactivated

**Table mpdfuectrl**

URL of the target webservice must be stored in mpdfuectrl of the sending site for the customer (customer specifically! Generally does not work!), (Recipient, kuliflag=0) of the openTRANS document transfer with dfuetyp 105, under id 6.

| ID | Name | Description |
| :-- | :--- | :--- |
| 6 | URL | In the form: `http://<Rechnername>/Albwir.Erp.Webservice.<Version>/ErpData.asmx` |
| 7 | Database Name | Name of the recipient DB (DB server is determined from xhaus) |
| 8 | DB_LOCALE | DB_LOCALE of the recipient (CLIENT_LOCALE is determined from xhaus) |

**Caution:** user and password for the DB access to the receiving sites are taken over from the config tool of the B2B service. That is, they have to be the same on the sending and receiving system.

**Table xhaus**

DB-Server (xhaus.informixserver), CLIENT_LOCALE (xhaus.clientlocale) and customer number (xhaus.kunr) will be determined for the target site (xhaus.haus) from the table xhaus.

#### 3.1.4. Output and storage of XML documents in openTRANS Version 2.1 (Version 1.0 is not supported)

Starting with version 5.5, it is possible to save invoices and delivery notes as XML documents.
If for the Open Trans processing no webservice URL is stored for the target sites, the output file is generated automatically.

**Configuration of the file path (#315897)**

See also the installation instructions for version 5.5.
In the config tool, under "File Export Path", the desired route path can be specified, under which the exported openTRANS XML files should be saved. `C:\\Temp` is entered as default.
The internal logic completes the directory `<site number>` and `<customer number>` in the path specified here.
The exported file is saved under the following name:
`openTRANS_<document type>_<site number>_<customer number>_<document number>.xml`

If the document generated is a partial document (kauf.subnr > 0), the subnr is also noted in the filename:
`openTRANS_<transaction type>_<site number>_<customer number>_<case number>_<transaction subnumber>.xml`

**Example:**
The file export path `D:\openTRANS` is entered in the Config tool.
The created openTRANS invoice file of invoice 776655 for customer 1234 in site 10 is saved in:
`D:\openTRANS\10\1234\openTRANS_INVOICE_10_1234_776655.xml`

If errors occur during creation of export file, the records remains in table ottransfer with an error flag. The A+W Enterprise B2B Service currently uses no log protocol.
If for some reason the file generation for a transaction is started again even though a file has already been generated, the existing file is overwritten by the newly-generated one.

**User Defined Extensions**

The user-defined extensions implemented within the internal charging logic are not written when an XML file is generated.

**Data Mapping openTRANS Invoice**

Initiated by case #345700, the following elements are also filled:

| | Designation | AWE DB field | openTRANS Element | Comment |
| :--- | :--- | :--- | :--- | :--- |
| 1 | Customer item number | kposex.exarttxt | `<INVOICE_ITEM_LIST>`<br>`<INVOICE ITEM>`<br>`<PRODUCT_ID>`<br>`<BUYER_PID>` | Prerequisite: env variable `DFUE_KUARTBEZ_TO_KPOSEX` is active. <br> Customer item number and name are taken over from kposex.exarttxt |
| 2 | VAT per item | kpos.npospreis,<br>kauf.mwstkz | `<INVOICE_ITEM_LIST>`<br>`<INVOICE_ITEM>`<br>`<PRODUCT_PRICE_FIX>`<br>`<TAX_DETAILS_FIX>`<br>`<TAX_AMOUNT>` | Is calculated using the relevant VAT record (kauf.mwstkz) and the net item price (kpos.npospreis). Prerequisite: there is only one valid VAT record for the entire order.<br> **CAUTION:** the item VAT amounts are not compared to the total VAT of the order(kauf.mwstbetrag), which means that there may be differences here if the invoice does not include redistributed discounts. |
| 3 | Customer item | kpos.kuposnr | `<INVOICE_ITEM_LIST>`<br>`<INVOICE_ITEM>`<br>`<CUSTOMER_ORDER_REFERENCE>`<br>`<LINE_ITEM_ID>` | |
| 4 | Reference | kpos.kommnr,<br>komm.kommtext | `<INVOICE_ITEM_LIST>`<br>`<INVOICE_ITEM>`<br>`<REMARKS>`<br>`(type="general")` | The text is determined using the commission number. |
| 5 | Customer order number | kauf.exaufnr | `<INVOICE_ITEM_LIST>`<br>`<INVOICE_ITEM>`<br>`<CUSTOMER_ORDER_REFERENCE>`<br>`<ORDER_ID>` | |
| 6 | Subsidiary number | | `<INVOICE_HEADER>`<br>`<INVOICE_INFO>`<br>`<REMARKS type="header">` | In the REMARKS, a header text is transferred that includes the subsidiary number. A fixed marketing text (for example, "FIL") is specified, so that the subsidiary number can be filtered out by the recipient. The marking text can be specified with a set phrase. <br> (This adjustment has to be made by the customer together with the planner!) |

**Note about VAT per item (#345700):**
Currently, the VAT amount is specified on the XML invoice for each item. At customer request, this is a calculated value from net item price * VAT record, which in total sometimes does not match the total VAT amount. This circumstance is known to the customer, see also case #345700.

### 3.2. Internal charging (special version of the openTRANS document transfer for SGG/Caleoglas)

- **Documentation:** `\\hausi\AWDCaseDoc\127\127053\Wareneingangskontrolle.doc`
- **Documentation in Sharepoint:** `https://awsoftwaregmbh.sharepoint.com/:w:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/DE-A+W%20Enterprise%20Cust%20Auto%20Goods%20Receipt.docx?d=w10900c1fb5f645278125dda31105c10f&csf=1&web=1&e=eQMeMy`

> **Warning:**
> The B2B service can either be operated in the configuration "internal charging" (`AUTO_EK_KONTROLLE` active, openTRANS Version 1.0) or in the standard (automatic GR, xml export, openTRANS Version 2.1). The mixture is not possible.

### 3.3. Automatic warehouse in / delivery note generation for direct delivery (AWDesk #334475)

With the Version AWE B2B Service 5.5 (12.5), the automatic warehouse in and delivery note generation is implemented for direct delivery.
If the automatic purchase order transfer is configured for two companies and:
- in the production company for the order of the purchase order the delivery note transfer (mp.liefdfuekz) is active and
- the order is for a third-party deal,

if after the delivery note transfer by the B2B service in the commercial company the automatic warehouse in and delivery note generation is initiated.
This happens in that the transfer table eingangekkopf the transferred header record is marked with autokz=1, furthermore for the purchase order associated with the delivery note, a record with the still ID -42 (ERZEUGE_WE) is placed in front of the intauf.
The logic is not implemented bracketed via an env variable but is implemented as standard logic.

#### 3.3.1. env variables

`WARENEINGANG_EXTERN`
The variable must be active ("ON"). If the variable is deactivated, no partial delivery notes can be generated.

#### 3.3.2. Input tables

The same input tables are used as for the internal charging.

**Input table eingangekkopf**
The table eingangekkopf is expanded in Version 6.0 (13.0) to include two fields "autokz" and "status." If the logic for the automatic WI in the Version 5.5 (12.5) should be put into operation, the corresponding database script for eingangekkopf must be executed after the fact.

#### 3.3.3. Trigger record in aufint

The trigger record that is placed in front of the intauf regardless of the actual number of items in the purchase order, always has the item quantity "1" (aufint.posanz); thus these records with still ID -42 are always processed by the same intauf.

#### 3.3.4. Restrictions

**Invoice transfer**
The logic is only available for delivery note transfer. Analogously, it would be conceivable that for invoice transfer and automatic purchase price invoice generation would take place. The trigger record before the intauf would then still bear the still ID -43 (ERZEUGE_EKRECH). This logic is currently NOT implemented.

**Special logic "Internal invoicing"**
The special logic (env variables) is still available.
With active "internal charging", however, the invoice and delivery note transfer may not be activated simultaneously for a market partner in the production site, since in this case, there can be conflicts during the GR booking at the distributor.

#### 3.3.5. Additional documentation/troubleshooting

For information about the eingangek* tables or troubleshooting, see the documentation of the internal calculation.

### 3.4. Troubleshooting

#### 3.4.1. Assignment of the webservice user for the "customer" webservice

See case 256084.
The user and the password for the customer webservice is currently taken over from the config file of the B2B service in order to simplify things - taken over because in all installations, you work with the ERP webservice. If in the future a customer webservice should really be addressed, switches must be added to mpdfuectrl.

#### 3.4.2. No access to database possible (from ERP webservice)

Error message:
```
ERROR [HYOOO] [Informix.NET provider][Informix] Unable to load locale categories.
...
```
The entries in xhaus.clientlocale and xhaus.informixserver must be checked. The `CLIENT_LOCALE` must match the set `CLIENT_LOCALE` on the sites in question.
See also #328013.

#### 3.4.3. B2B service does not write log to the desired log depth

Restart B2B service.

#### 3.4.4. B2B service/ERP webservice crash with internal charging

Was the order was changed at the target site so that the item references are no longer right?
See also AWDesk #355311, #323921.

## 4. General data mapping

### 4.1. openTRANS address element `<COUNTRY>`

According to the openTRANS interface description, the openTRANS element `<COUNTRY>` should contain the name of the country in the address details.
Historically conditioned, however, the element is filled with the country abbreviation from A+W Enterprise.
Now the logic has been expanded so that instead of as previously the country code, the assigned ISO country code from xxland.iso is written to the element. If in the table xxland no ISO country code is stored, the country code is still written to the element.

**Remarks:**
With the designation "ISO country code," the two-letter (Alpha-2) code according to ISO 3166-1 is meant.
The current structure of the table xxland only permits the entry of the two-letter code. The three-letter (Alpha-3) code cannot be used.
See PF [AW-106274].

## 5. Troubleshooting (general)

### 5.1. ERP Webservice URL: UriFormatException

System.UriFormatException: Invalid URI: The hostname could not be parsed.
Check whether the URI contains only slashes. Backslashes are not allowed.

### 5.2. ERP webservice does not write a log

Check whether the ERP webservice is running under the correct user, who has enough rights.
See also AWDesk 324151.

### 5.3. ERP webservice does not write log to the desired log depth

Under some circumstances, IIS must be restarted so that the new log settings are recognized.
Careful, other processes also access the webservice methods. IIS restart only possible at a non-critical point in time!

### 5.4. ERP webservice (import) cannot be addressed

URL in mpdfuectrl must end on "ErpData.asmx".
URL and DB settings must be stored customer-specifically in mpdfuectrl.
