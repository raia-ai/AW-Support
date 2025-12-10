---
title: "EN-CONFIG-AW_Enterprise_B2B_Service"
source: "EN-CONFIG-AW_Enterprise_B2B_Service.pdf"
tags: ["A+W Enterprise", "B2B Service", "Configuration", "openTRANS", "XRechnung", "E-invoicing", "Software", "Glass Industry", "EDI", "XML"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides configuration instructions for the A+W Enterprise B2B Service. It details the setup for various functionalities, including openTRANS document exports, A+W EDI exports, and E-invoicing with XRechnung. The guide covers installation steps, logging, control table management, and data mapping for different business documents."
long_description: "This is a comprehensive configuration manual for the A+W Enterprise B2B Service, a software solution for the glass industry. The document focuses on the 'new' functionality that operates without the A+W ERP Webservice. It is intended for internal use by technical personnel responsible for setting up and maintaining the B2B service.\n\nThe manual is structured to guide the user through the entire configuration process. It begins with general information, distinguishing between old and new functionalities and providing an overview of features such as DORMA PO transfer, internal charging, and various document exports (order confirmation, invoice, delivery note). It then covers installation procedures for different back-end versions, B2B service setup, and the configuration tool.\n\nKey sections are dedicated to specific export formats. Chapter 6 provides an in-depth guide to 'openTRANS export', including installation, configuration of master data and EDI settings, triggering document generation, and detailed data mapping for order confirmations, invoices, and dispatch notifications. Chapter 7 briefly covers the 'PO export / A+W EDI export'. A major section, Chapter 8, is dedicated to 'E-invoicing – XRechnung', the German standard for electronic invoices. This section outlines requirements, version details, validation, installation steps, configuration of environment variables, master data, and specific functions. It also includes extensive data mapping and descriptions of specific data fields (BT-10, BT-49, etc.). The document concludes with sections on error handling, cleanup logic, and a detailed troubleshooting guide for common issues."
---
# A+W Enterprise B2B Service
**Configuration Instructions**

-INTERNAL-

A+W - Software for Glass

---
## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2019-02-05 | Original version | Transfer from Dokuware document | 1.0 |
| 2020-05-07 | SVH | Addition A+W EDI Export (AWDesk #422752) | |
| 2022-02-14 | SVH | openTRANS export credit notes (PF [AW-87535]) | |
| 2022-05-03 | SVH | ISO country code in address element <COUNTRY> - PF [AW-106274] | |
| 2023-08-18 | SVH | Triggering the document generation | |
| 2023-08-22 | SVH | Log "docexport<MMdd>" | |
| 2023-09-01 | SVH | [AW-155564] – Clean-up logic | |
| 2023-09-08 | SVH | [AW-157266] – Configuration mpdfuectrl | |
| 2023-09-20 | SVH | [AW-157970] – DBNull-Values | |
| 2024-10-10 | SVH | [AW-111997] - E-Invoicing - XRechnung | |
| 2024-12-06 | SVH | [AW-111997] - E-Invoicing - XRechnung | |
| 2025-01-13 | SVH | [AW-213600] - Troubleshooting | |
| 2025-01-17 | SVH | [AW-217006] - Reworking of the entire document | |
| 2025-02-06 | SVH | [AW-111997] - E-Invoicing – XRechnung - Validation, Texts | |
| 2025-02-11 | SVH | [AW-214065] - Error handling | |
| 2025-03-28 | SVH | [AW-111997] - elnvoicing – Texts | |
| 2025-04-24 | SVH | [AW-111997] - E-invoicing - eMail-addresses | |
| 2025-05-23 | SVH | [AW-111997] - E-Invoicing - Tax code and Payment type code | |
| 2025-07-02 | SVH | [AW-111997] - E-invoicing – eMail addresses – SP rpgeteinvemailaddress | |

## Content
1.  **General Information**
2.  **Installation**
    *   2.1. Operation with ALCIB 2008 back-end
        *   2.1.1. SQL scripts
    *   2.2. Operation starting with Version 6
        *   2.2.1. Tabelle ottransfer
    *   2.3. B2B Service Setup
3.  **Configuration of B2B Service config tool**
    *   3.1. Config-Tool
    *   3.2. B2B service - automatic restart after abort due to error
4.  **Logging**
    *   4.1. B2B Service log
    *   4.2. Ftest
    *   4.3. Log docexport<MMdd>
5.  **Control table ottransfer**
    *   5.1. Interface-dependent details in ottransfer
    *   5.2. Status in ottransfer.steuerflag
        *   5.2.1. Processing status
        *   5.2.2. Error status
    *   5.3. Archive table ottransferok
6.  **openTRANS export**
    *   6.1. General information
    *   6.2. Installation - operation starting with Version 6
        *   6.2.1. AWE Backend
        *   6.2.2. Table aldfuectrl
        *   6.2.3. fx_texte
        *   6.2.4. Table errmsg
    *   6.3. Customizing
        *   6.3.1. vorgangs_sql - Interpane (AWDesk #402176)
    *   6.4. Configuration
        *   6.4.1. Environment variables
        *   6.4.2. MP master
        *   6.4.3. EDI configuration (mpdfuectrl)
        *   6.4.4. openTRANS Invoice (invoice)
    *   6.5. Triggering the document generation
    *   6.6. openTRANS format
    *   6.7. Output file
        *   6.7.1. Order confirmation
        *   6.7.2. Invoice / credit note
        *   6.7.3. Delivery note
    *   6.8. General data mapping
        *   6.8.1. openTRANS address element <COUNTRY>
    *   6.9. Standard export
        *   6.9.1. General Information
        *   6.9.2. Specific data determination
        *   6.9.3. Determination of the customer item ID (LINE_ITEM_ID of the reference order item) (#402154, #403065, #422771, #431998)
        *   6.9.4. Order confirmation
        *   6.9.5. Dispatch notification based on the order data analogous to pre-delivery note
        *   6.9.6. Invoice / credit note
    *   6.10. Hornbach export
7.  **PO export / A+W EDI export**
8.  **E-invoicing – XRechnung**
    *   8.1. General Information
        *   8.1.1. Definition
        *   8.1.2. CIUS
        *   8.1.3. Additional information
    *   8.2. Requirements
    *   8.3. Electronic invoice and PDF invoice (report)
    *   8.4. XRechnung version
    *   8.5. ZUGFeRD version
    *   8.6. Manual validation of the XRechnung
    *   8.7. Installation A+W Enterprise
        *   8.7.1. Binfile/environment
        *   8.7.2. al tables
        *   8.7.3. Error messages
        *   8.7.4. Report texts
    *   8.8. Installation B2B service
    *   8.9. Configuration - B2B Service config tool
    *   8.10. Configuration - environment variables
        *   8.10.1. MODUL_EINVOICING
        *   8.10.2. EINVOICE_NO_REFDAT
        *   8.10.3. NO_EINVOICE_FOR_INTERN_CR_NOTE
        *   8.10.4. RABATTLOGIK_2005
        *   8.10.5. REP_FAKTURA
        *   8.10.6. SKONTO_SPECIAL
        *   8.10.7. EINV_FORMART_RECH
        *   8.10.8. EINV FORMART GUTS
        *   8.10.9. XWAEHR_ISOCODE_FIELD
    *   8.11. Configuration - SPs
        *   8.11.1. rpgeteinvemailaddress
        *   8.11.2. cu_get_e_invoice_name
    *   8.12. Configuration – MP-specific (mpdfuectrl)
    *   8.13. Configuration of the master data
        *   8.13.1. Seller/Supplier
        *   8.13.2. Buyer/Recipient
        *   8.13.3. Buyer/Recipient - e-mail addresses
        *   8.13.4. Document types - document type of the e-invoice
        *   8.13.5. Company items
        *   8.13.6. Countries ISO code
        *   8.13.7. Currency ISO code
        *   8.13.8. Tax code
        *   8.13.9. Method of payment code
        *   8.13.10. Contact Person
        *   8.13.11. Employee
        *   8.13.12. Bank details
        *   8.13.13. Configurable Texts
    *   8.14. Functions
        *   8.14.1. General
        *   8.14.2. Invoice handling
        *   8.14.3. Language
        *   8.14.4. File generation and file name
        *   8.14.5. Determination of e-mail addresses
        *   8.14.6. Text
        *   8.14.7. Surcharges and discounts
        *   8.14.8. Invoice amounts in foreign currency
        *   8.14.9. Credit notes
        *   8.14.10. Deposit invoice / final invoice
        *   8.14.11. Validation of the e-invoice
        *   8.14.12. Error handling
        *   8.14.13. Cleanup logic
        *   8.14.14. Restrictions
    *   8.15. Data mapping
        *   8.15.1. UBL
        *   8.15.2. CII
    *   8.16. Specific data description
        *   8.16.1. Legal seller
        *   8.16.2. Buyer reference / route ID (BT-10)
        *   8.16.3. Buyer electronic address (BT-49)
        *   8.16.4. Seller electronic address (BT-34)
        *   8.16.5. Seller additional legal information (BT-33)
        *   8.16.6. Payment terms (BT-20)
        *   8.16.7. Legal information about the seller (BT-33)
        *   8.16.8. Address addition of the customer (BT-163)
        *   8.16.1. Texts on header level (BT-22)
        *   8.16.2. Texts on item level (BT-127)
        *   8.16.3. Legal company name
        *   8.16.4. Delivery address
        *   8.16.5. Telephone number of the supplier contact
        *   8.16.6. Item dimensions (BT-160/BT-161)
    *   8.17. E-mail addresses in the e-invoice
    *   8.18. Manual generation of e-invoices
        *   8.18.1. CMD script „xrechnungexport"
    *   8.19. Sending the E-invoice via e-mail
        *   8.19.1. Data security
    *   8.20. Archiving the e-invoice
    *   8.21. Creation and archiving of the XRechnung via ZUGFeRD PDF file.
    *   8.22. Troubleshooting
        *   8.22.1. Sending the e-invoice - PDF is sent, but not configured
        *   8.22.2. E-invoice (file) is missing when sending
9.  **E-mail notification in case of error (AWDesk #407285)**
10. **Cleanup logic**
11. **Troubleshooting**
    *   11.1. There is no entry in the table ottransfer
    *   11.2. "object reference not set"-Exception in GetAnsprData()
    *   11.3. Error "no lapool data" or quantities missing in the dispatch notification document
    *   11.4. Error during select on lapool (only Version ALCIB 2008 (4.2))
    *   11.5. Exception due to DBNull value
    *   11.6. openTRANS Invoice – empty document
    *   11.7. Temporary database problems/network problems/Informix error
    *   11.8. Interruption of the B2B service without error message in the log
    *   11.9. B2B Service aborts due to error, but does not restart

## 1. General Information
The logic of the B2B service can be subdivided into "old" functionality, which uses the methods of the A+W ERP Webservice; that is, which also always requires the installation of the ERP Webservice, and "new" functionality, which makes do without the ERP Webservice.

The document describes the "new" functionality (without ERP Webservice), which was initially developed with AWDesk #392089.

The "old" functionality (with ERP Webservice call) is described in the separate document EN-CONFIG-A+W Enterprise B2B Service ERP WS.docx.

**Overview of functions**

| Functions | open TRANS format | ERP WS required | Note |
| :--- | :--- | :--- | :--- |
| DORMA PO transfer | 1.0 | yes | The object generated in the openTRANS format 1.0 is transferred directly to the DORMA web service.<br>There is no xml file. |
| Internal charging<br>(Invoice transfer) | 1.0 | yes | Special logic for SGG.<br>The object generated in the openTRANS format 1.0 is transferred directly to the A+W ERP web service.<br>Use of user-defined extensions that do not correspond to the openTRANS standard.<br>There is no xml file. |
| Delivery note transfer | 2.1 | yes | Logic analogous to the "internal invoicing".<br>The object generated in the openTRANS format 2.1 is transferred directly to the A+W ERP web service.<br>There is no xml file. |
| Export invoice (outdated)<br>Generation of an xml document. | 1.0 | yes | Conceived as a quickly available transitional solution.<br>No collective invoices possible.<br>Should be terminated. |
| Export delivery note (outdated)<br>Generation of an xml document. | 2.1 | yes | Conceived as a quickly available transitional solution.<br>Should be terminated. |
| Export order confirmation<br>Generation of an xml document. | 2.1 | No | No electronic signature. |
| Export invoice<br>Generation of an xml document. | 2.1 | NO | No electronic signature. |
| Export delivery note<br>Generation of an xml document. | 2.1 | NO | No electronic signature. |
| Export PO | - | NO | Flat file, format A+W internal |
| Export XRechnung | - | NO | xml format (UBL)<br>No electronic signature. |

## 2. Installation

### 2.1. Operation with ALCIB 2008 back-end

#### 2.1.1. SQL scripts
The following SQL scripts must be executed in order to make the table ottransfer compatible with the B2B Service 6/ERP Webservice 6:
`...\install\xsql\4\4\0\ottransfer01.sql`
`...\install\xsql\4\5\0\ottransfer01.sql`
`...\install\xsql\13\0\0\130000085_ottransfer.sql`
`...\install\xsql\13\0\4\130004003_ottransfer.sql`

### 2.2. Operation starting with Version 6

#### 2.2.1. Tabelle ottransfer
The status of the table ottransfer must be checked. If there are fields missing, the appropriate SQL scripts (see "operation with ALCIB 2008 back end") must be executed.

### 2.3. B2B Service Setup
For start-up, the B2B Service 6 must be installed. Installing the ERP Webservice is not necessary.

## 3. Configuration of B2B Service config tool

### 3.1. Config-Tool
In the Config Tool of the B2B Service, each export type must be activated individually and the database connection entered.
The e-mail sending can (and should) also be configured in case of error.
The operation of the config tool is described precisely in the installation instructions.

### 3.2. B2B service – automatic restart after abort due to error
Via the Windows "Services" dialog, the automatic restart of the B2B service can be configured after an abort due to error.
For this, mark the B2B service in "Services", then right-click to call up the context menu and select "Properties". Change to the "Recovery" tab there.

**Recovery Settings:**
- **First failure:** Restart the Service
- **Second failure:** Restart the Service
- **Subsequent failures:** Restart the Service
- **Reset fail count after:** 0 days
- **Restart service after:** 1 minutes

## 4. Logging

### 4.1. B2B Service log
The logging can be configured via the config tool of the B2B service.

### 4.2. Ftest
If the ftest is active in A+W Enterprise, the checking of the configuration of the document export and the insert into the table ottransfer is logged in detail there.

### 4.3. Log docexport<MMdd>
The log "docexport<MMdd>" is written in the site-specific PROTOPFAD.
Here it is possible to trace at which point the entry of an export record (file generation) to the table ottransfer from the A+W Enterprise was initiated.

## 5. Control table ottransfer
The table ottransfer is the control table of the document export.
Successfully processed records are transferred to the table ottransferok and deleted from ottransfer. Incorrect records remain in ottransfer with steuerflag > 600.

| No. | Field | Data type | Description | Comment |
| :--- | :--- | :--- | :--- | :--- |
| 1 | auftrnr | integer | | |
| 2 | vorgang | smallint | | |
| 3 | schnittstelle | char(6) | Interface type | "OTDOC" – openTRANS document export<br>"EDIEXP" – PO export, AWE standard interface<br>"E-INV" - [AW-111997] - E-invoicing |
| 4 | steuerflag | smallint | | 0 = wait for processing<br>1 = in processing<br>301 = wait for lock<br>> 600 = error, see error status chapter |
| 5 | filltime | datetime | | |
| 6 | Ifdnr | smallint | | |
| 7 | serviceid | smallint | | |
| 8 | subnr | smallint | | |
| 9 | hausnr | smallint | | |
| 10 | routenr | smallint | | |
| 11 | Itplan | date | | |
| 12 | uzeit | datetime | Update time | |
| 13 | doctype | smallint | Document type | The entry depends on the interface used. See details in section "Interface-dependent details in ottransfer". |
| 14 | subtype | smallint | Customer-specific document subtype | The entry depends on the interface used. See details in section "Interface-dependent details in ottransfer". |
| 15 | comment | char(20) | Comment | The comment contains an indication from which AWE program logic the ottransfer record was generated. If an ottransfer record contains an error status, the previous comment is replaced by the description of the current error. |

### 5.1. Interface-dependent details in ottransfer
The entries in the fields `ottransfer.doctype` (document type) and `ottransfer.subtype` (document subtype) depend on the interface used (field ottransfer.schnittstelle).
Both details must be stored via the EDI configuration of the market partner or globally for all market partners (table mpdfuectrl).

> **Caution:**
> During export of openTRANS documents, attention must be paid that the "old logic" is switched off. That is, for a market partner for which an openTRANS invoice/credit should be exported, the flag "Invoice transfer" (mp.rechdfuekz) must be deactivated in the master.
> If the logic "internal calculation" is not required, the environment variables OPENTRANS_XMLINVOICE and OPENTRANS_XMLCREDITNOTE should be deactivated.

Here is the overview table of the possible combinations.

| Export type | Interface (ottransfer.interface) | Document types (ottransfer.doctype) | Document subtypes (ottransfer.subtype) |
| :--- | :--- | :--- | :--- |
| openTRANS | "OTDOC" | 1 = Order confirmation<br>2 = dispatch notification based on the order data analogous to pre-delivery note<br>3 = dispatch notice (not yet implemented)<br>4 = invoice<br>5 = credit note | 1 = standard-export<br>2 = Hornbach export (AWDesk #407285, #437427)<br><br>**Caution:** The subtype is configured once, globally for all stored document types. |
| PO export | "EDIEXP" | 1 = Default | 1 = Default |
| XRechnung | "E-INV" | 1= XRechnung | 1 = Default |

### 5.2. Status in ottransfer.steuerflag

#### 5.2.1. Processing status
Via the `ottransfer.steuerflag` field, the processing status of a document can be determined.

| Status (steuerflag) | Description |
| :--- | :--- |
| -999 | The record was not recognized |
| -998 | The record is ignored |
| 0 | Wait for processing |
| 1 | Being processed |
| 301 | Wait due to block |
| 302 | Wait due to kauf.still < 0 |
| 998 | Cancellation not transferred |
| 999 | Successfully processed |

#### 5.2.2. Error status
Incorrect records remain in ottransfer with steuerflag > 600. There is a list of the possible error numbers in the following table.

| Error number (steuerflag) | Description |
| :--- | :--- |
| 601 | General unspecified error |
| 602 | Unknown processing type (combination ottransfer.doctype/subtype) |
| 603 | Missing lapool data |
| 604 | Error in reprocessing (e.g. DB updates after file generation) |
| 605 | Error when lifting the number lock |
| 606 | Error when saving file |
| 607 | Error when deleting the record from the table ottransfer |
| 608 | Interface not implemented |
| 620 | kauf record could not be found |
| 701 | Missing NDU (number of the dispatch unit) |
| 721 | elnvoicing - data error |
| 722 | E-invoice - validation error |

### 5.3. Archive table ottransferok
Successfully processed records are transferred to the table ottransferok.

## 6. openTRANS export
Export of openTRANS documents in the xml format.

### 6.1. General information
openTRANS 2.1 is an open standard for support of electronic data exchange for business transactions between trading companies. By using the module, trade partners can make business documents available automatically in a standardized format. Documentation of the openTRANS 2.1 standard is available on the Internet site www.opentrans.de. Furthermore, it is stored internally at A+W under `\\jupiter\Doku_DocuWare\Interfaces\openTrans`.

The exported documents are NOT signed electronically.

An import of openTRANS xml documents is not implemented (status as of 07/24/2019). Currently, an import is only done within the internal charging logic and delivery note transfer by SGG. The import here is done via a project that is transferred directly to the ERP webservice. The project includes user-defined extensions that are not included in the openTRANS standard.

### 6.2. Installation - operation starting with Version 6
See also the general chapter "Operation with Version 6" further above.

#### 6.2.1. AWE Backend
With AWDesk #417278, the logic is made available, which with appropriate configuration (mpdfuectrl) for printing of the order confirmation, the pre-delivery note and the invoice, the appropriate openTRANS document is created.
As long as this logic does not exist in the back end, the generation of the openTRANS documents must be initiated with customizing (insert in ottransfer).

#### 6.2.2. Table aldfuectrl
With AWDesk #417278, the preparations were made for making the document export configurable for a specific customer when printing order confirmation/dispatch notification/invoice.
The following records in aldfuectrl are required for this:
`INSERT INTO aldfuectrl (id, errno, labeltxt, idtyp) VALUES (42, 22639, 'invoice', 1);`
`INSERT INTO aldfuectrl (id, errno, labeltxt, idtyp) VALUES (43, 37065, 'order response', 1);`
`INSERT INTO aldfuectrl (id, errno, labeltxt, idtyp) VALUES (44, 37383, 'dispatch notification – order data', 1);`
`INSERT INTO aldfuectrl (id, errno, labeltxt, idtyp) VALUES (45, 37384, 'document subtype', 2);`

#### 6.2.3. fx_texte
With AWDesk #417278, the preparations were made for making the document export configurable for a specific customer when printing order confirmation/dispatch notification/invoice.
For this, current fx_texte are required, which contain the entries for numbers 37383, 37384.

#### 6.2.4. Table errmsg
With AWDesk #407285, the e-mail sending in case of error was implemented.
For language-dependent messages in the e-mails, the message numbers 37395 to 37410 must exist in the table errmsg.

### 6.3. Customizing

#### 6.3.1. vorgangs_sql - Interpane (AWDesk #402176)
Customizing the vorgangs_sql: for customers for whom the openTRANS files are written, for orders that are generated via EDI, the information in kposex.exarttxt is abbreviated to the information relevant for the customer.

### 6.4. Configuration

#### 6.4.1. Environment variables
> **Caution:** Attention must be paid that the env variables OPENTRANS_XMLINVOICE and OPENTRANS_XMLCREDITNOTE must be deactivated if the logic for generation of openTRANS documents should be put into operation.

#### 6.4.2. MP master
If the openTRANS export should be configured for a customer, it must be checked in the MP master data that the flags "Delivery note transfer" (mp.liefdfuekz) and "Invoice transfer" (mp.rechdfuekz) are deactivated.
**Note:**
The flags "Delivery note transfer" and "Invoice transfer" (updated label: "Invoice transfer internal") are used for the logic for internal calculation. The logic is described in the configuration document "Enterprise B2B Service ERP WS".

#### 6.4.3. EDI configuration (mpdfuectrl)
See also AWDesk #417278.
The document export is configured in the menu element System > Data Transfer > Document Transfer > Configuration or via the MP master data dialog. The settings are saved in the table mpdfuectrl.
Configuration of the openTRANS export must be done customer-specifically.
General (market partner-spanning) entries are possible, but will be ignored during the program-side evaluation so that they have no control effect.

**Document types**
Each document type is activated individually.
For this, for the customer or in general, an entry is generated with the "EDI type" 105 (document export) and the control type specified (ID):
- Order confirmation (ID 43)
- Dispatch notification (ID 44)
- Invoice (ID 42)
- Credit (ID 64)

The corresponding checkbox is activated.
Furthermore, the document subtype (ID 45) must be created once. This applies for all documents. See next paragraph.

**Document subtype (ID 45)**
The customer-specific version is defined by an entry with "EDI type" 105 (document export) and control type 45 (document subtype).
Caution: The one entry is valid for all activated documents.
A number corresponding to a valid subtype is stored here as a value. The valid subtypes can be found in the table in chapter "control table ottransfer".
If no special requirement is known, the "Standard" is entered (generally "1").

> **Warning:**
> - The subtype must be stored explicitly. If the setting is missing or no value > 0 is stored, the document export will not be executed.

#### 6.4.4. openTRANS Invoice (invoice)
The simultaneous activation of openTRANS invoice export and XRechnung export for a customer is not forbidden by A+W Enterprise (status as of 01/17/2025).
However, the simultaneous sending of different invoice formats for one and the same invoice to a customer should absolutely be avoided.
Please check during configuration of the openTRANS invoice that no sending of XRechnung is active.

### 6.5. Triggering the document generation
The description of the control table ottransfer includes an overview of all document types that can be exported.
The export is initiated via a record in the table ottransfer.
The corresponding data record is generally generated from A+W Enterprise. (A customer-specific logic via script or vorgangs_sql is also conceivable, but should be avoided if possible.)

**Initiation of document generation**

| Document type | Program position | Comment |
| :--- | :--- | :--- |
| Dispatch notification based on the order data | Printing of preliminary delivery note | In dispatch |
| Order confirmation | Printing/e-mailing of the order confirmation | Sales > Forms |
| Invoice | Printing/e-mailing of the invoice | Sales > Forms |
| Credit note | Printing/e-mailing of the credit note | Sales > Forms |

The document generation is configured as described in the "Configuration" chapter, via the market partner settings in the table mpdfuectrl.

> **Attention:** If a printer configuration is accidentally used for the form printing where the printing is not permitted, there is no export of the document.
> In ftest, the missing print permission can be discerned from the following entry:
> "
> ... IsAusgabeFuerDruckerErlaubt() drupfad: 'nooutputprinter'...
> IsAusgabeFuerDruckerErlaubt() returns 0 ..."

### 6.6. openTRANS format
The documents are generated as xml documents in the openTRANS 2.1 format.
The complete format description can be found here:
`\\jupiter\Doku_DocuWare\Interfaces\openTrans`

### 6.7. Output file
The root directory for saving the output files is configured in the config tool of the B2B service.
The files are stored from there in the subdirectory structure `<Hausnr>\<Kunr>`.
The file name of the output file is composed as follows:

#### 6.7.1. Order confirmation
`<Dateityp>_<Hausnr>_<Kundennr>_<Auftragsnr>`
**Example:** Root directory C:\Temp, file type ORDERRESPONSE, Site no 12, Cuno 123, Ordno 445667
**Output file:** `c:\Temp\12\123\openTRANS_ORDERRESPONSE_12_123_445667.xml`

#### 6.7.2. Invoice / credit note
The export of credit notes was implemented with PF [AW-87535].

`<File type>_<Site no>_<Customer no>_<Invoice no>`

**Example invoice:** Root directory C:\Temp, file type INVOICE, Site no 12, Cuno 123, Ordno 445667
**Output file:** `c:\Temp\12\123\openTRANS_INVOICE_12_123_445667.xml`

**Example credit note:** Root directory C:\Temp, file type CREDITNOTE, Site no 12, Cuno 123, Ordno 445668
**Output file:** `c:\Temp\12\123\openTRANS_CREDITNOTE_12_123_445668.xml`

**Partial invoice**
`<File type>_<Site no>_<Customer no>_<Invoice no>_<Subno>`
**Example:** Root directory C:\Temp, file type INVOICE, Site no 12, Cuno 123, Ordno 445667, Subno 1
**Output file:** `c:\Temp\12\123\openTRANS_INVOICE_12_123_445667_1.xml`

#### 6.7.3. Delivery note
`<File type>_<Site no>_<Customer no>_<Orderno>_<Route>_<Planned delivery date>`
**Example:** Root directory C:\Temp, file type ORDERRESPONSE, site no 12, cuno 123, ordno 445667, Route 60, DDplan 06.06.2018
**Output file:** `c:\Temp\12\123\openTRANS_DISPATCHNOTIFICATION_12_123_445667_60_06062018.xml`

### 6.8. General data mapping

#### 6.8.1. openTRANS address element <COUNTRY>
According to the openTRANS interface description, the openTRANS element `<COUNTRY>` should contain the name of the country in the address details.
Historically conditioned, however, the element is filled with the country abbreviation from A+W Enterprise.
Now the logic has been expanded so that instead of as previously the country code, the assigned ISO country code from xxland.iso is written to the element. If in the table xxland no ISO country code is stored, the country code is still written to the element.

**Remarks:**
With the designation "ISO country code," the two-letter (Alpha-2) code according to ISO 3166-1 is meant.
The current structure of the table xxland only permits the entry of the two-letter code. The three-letter (Alpha-3) code cannot be used.
See PF [AW-106274].

### 6.9. Standard export

#### 6.9.1. General Information
The standard export was developed with AWDesk #392089 in cooperation with Cantor (as recipient of the exported files). The standard export is therefore sometimes called "Cantor export."

#### 6.9.2. Specific data determination
**Determination of the external order number**
The external order number is transmitted via the EDI import to AWE. However, it is not listed in the content of the EDI file, but rather is included in the file name of the EDI file. The file name of the EDI file is saved in AWE in kauf.exbez1. The external order number is also written to kauf.exaufnr during import. In kauf.exaufnr-string, it is expected in the first position, separated from all other values by empty spaces.
Example: „155764 7060 HORNBACH“

Additions with AWDesk #403065:
If no external number exists, the abbreviation "NA" (not available) is written in the corresponding element instead.

**Determination of the external site number**
The site number of the external site is transferred during EDI import into the file in record K1, field 11. According to docu "alfak_edi_deu.doc", it was previously not evaluated in AWE.

#### 6.9.3. Determination of the customer item ID (LINE_ITEM_ID of the reference order item) (#402154, #403065, #422771, #431998)
The customer item ID will be transferred in the following elements of the openTRANS-xml structures:
1.  **DISPATCHNOTIFICATION:**
    `<DISPATCHNOTIFICATION_ITEM>.<ORDER_REFERENCE>.<LINE_ITEM_ID>`
    `<DISPATCHNOTIFICATION_ITEM>.<CUSTOMER_ORDER_REFERENCE>.<LINE_ITEM_ID>`
2.  **INVOICE:**
    `<INVOICE_ITEM>.<ORDER_REFERENCE>.<LINE_ITEM_ID>`
    `<INVOICE_ITEM>.<CUSTOMER_ORDER_REFERENCE>.<LINE_ITEM_ID>`
3.  **ORDERRESPONSE:**
    `<ORDERRESPONSE_ITEM>.<LINE_ITEM_ID>`

Via the menu item System > Data Transmission > Process Transmission > Configuration, the customer-specific mode with which the customer item ID is to be determined can be stored for the EDI type 105 with ID 46 (customer item mode).
The default mode is mode 0. This is the standard logic described above. If a mode has not been explicitly configured via System > Data Transmission > Transfer Document> Configuration, the default mode 0 is used.
Similarly, via the menu element System > Data Transfer > Process Transmission > Configuration, a mode that deviates from default mode 0 can be stored for all customers. (AWDesk #431998).

Prerequisite for the configuration is that the table aldfuectrl contains a data set for ID=46.
If the record does not exist, it can be created with the following sql statement:
`INSERT INTO aldfuectrl (id, errno, labeltxt, idtyp) VALUES (46, 37525, 'customer item mode', 2)`

**Standard logic - MODE 0**
The customer item ID is configured in the standard logic as follows:
`kpos.lfdpos` (in order to guarantee unambiguousness) plus slash plus `kpos.kuposnr`
Example for kpos.lfdpos 2, kpos.kuposnr "ABC123": `LINE_ITEM_ID = 2/ABC123`
If no external item ID exists, that is, the field kpos.kuposnr is empty, then instead of the ID, the string "NA" (abbreviation for "not available") is written.
Example for kpos.lfdpos 3: `LINE_ITEM_ID = 3/NA`

**Customer individual logic MODE 1 – Determination of customer item ID from the item text (AWDesk #422771)**
For each item the item text (kpos.arttxtnr -> auftxt.txtnr) is selected which has no tuple assignment (auftxt.tnr = 0) and in which the text "reference:" exists. The first numeric integer value after the text "reference:" is used as the customer item number.
The item texts are processed in ascending order in the sequence numbers (auftxt.seqnr). The first record with auftxt.tnr=0 and the text "reference:" in auftxt.txt is used to determine the customer item number. If there are several records with the text "reference:", the sentence with the smallest sequence number and tuple number 0 wins.
If no text "reference:" is found in the item texts, the customer item number is filled with the value "NA" (not available).

**Customer individual logic MODE 2 – External AWE item number (kpos.lfdpos) as customer item ID (AWDesk #431998)**
The customer item ID (LINE_ITEM_ID) is assigned the external AWE item number from kpos.Idfpos.

**Overview of MODES customer item ID**

| MODE | Description | Functions | Configuration |
| :--- | :--- | :--- | :--- |
| **0** | **Standard** <br> Configuration only necessary if this mode is desired for individual customers and a deviating mode was configured for all customers | `kpos.lfdpos` (in order to guarantee unambiguousness) plus slash plus `kpos.kuposnr` | System > Data transfer > Document transfer > Configuration<br>EDI type 105, control type 46<br>Value 0 |
| **1** | **Customer item ID from the item text** <br> (AWDesk #422771) | Text „reference: <ID>" in item text (`kpos.arttxtnr` -> `auftxt.txtnr`) | System > Data transfer > Document transfer > Configuration<br>EDI type 105, control type 46<br>Value 1 |
| **2** | **External AWE item number** <br> (AWDesk #431998) | `kpos.lfdpos` | System > Data transfer > Document transfer > Configuration<br>EDI type 105, control type 46<br>Value 2 |

#### 6.9.4. Order confirmation
Only quantities, articles and dates are confirmed. The product structure and changes to the BOM are not exported.

**Data Mapping**

| openTRANS xml element | Data type | Mandatory field | Description | AWE DB field | Comment |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **<ORDERRESPONSE_HEADER>** | | | | | |
| **<ORDERRESPONSE_INFO>** | | | | | |
| ORDER_ID | string | Y | | `kauf.exaufnr` | See chapter "Determination of the external order number" |
| SUPPLIER_ORDER_ID | string | | | `kauf.auftrnr` | |
| ORDERRESPONSE_DATE | string | Y | Format `yyyy-MM-ddT00:00:00` | - | Date of the generation of this document |
| ORDER_DATE | string | | Format `yyyy-MM-ddT00:00:00` | `kauf.edat` | ? |
| **<DELIVERY_DATE>** | | | | | |
| DELIVERY_START_DATE | string | | Format `yyyy-MM-ddT00:00:00` | `kauf.ltplan` | |
| DELIVERY_END_DATE | string | | Format `yyyy-MM-ddT00:00:00` | `kauf.ltplan` | |
| **</DELIVERY_DATE>** | | | | | |
| **<PARTY> (supplier)** | | Y | | | |
| PARTY_ID | string | | | `kauf.hausnr` -> `xhaus.linr` | |
| **<ADDRESS>** | | | | `xhaus.linr` -> `mp` | |
| NAME | string | | | `mp.name` | |
| NAME2 | string | | | `mp.vname` | |
| NAME3 | string | | | `mp.branche` | |
| STREET | string | | | `mp.str` | |
| ZIP | string | | | `mp.plz` | |
| CITY | string | | | `mp.ort` | |
| COUNTRY | string | | | `xxland.iso` determined using `mp.kfzcode` | [AW-106274] See "General data mapping" section |
| VAT_ID | string | | presently not filled | `mp.steuernr` | VAT ID |
| PHONE | string | | | `mp.telefon` | |
| FAX | string | | | `mp.faxnr` | |
| EMAIL | string | | | `mp.email` | |
| URL | string | | | `mp.website` | |
| **</ADDRESS>** | | | | | |
| **</PARTY> (supplier)** | | | | | |
| **<PARTY> (customer)** | | Y | | | |
| PARTY_ID | string | | | `kauf.kunr` | |
| **<ADDRESS>** | | | | | |
| NAME | string | | | `kauf.orgname` | |
| NAME2 | string | | | `kauf.orgvorname` | |
| NAME3 | string | | | `kauf.orgbranche` | |
| STREET | string | | | `kauf.orgstr` | |
| ZIP | string | | | `kauf.orgplz` | |
| BOXNO | string | | | `kauf.orgpostfach` | |
| ZIPBOX | string | | | `kauf.orgpfplz` | |
| CITY | string | | | `kauf.orgort` | |
| COUNTRY | string | | | `xxland.iso` determined using `kauf.orgkfzcode` | [AW-106274] See "General data mapping" section |
| PHONE | string | | | `kauf.orgtel` | |
| FAX | string | | | `kauf.faxnr` | |
| EMAIL | string | | | `kauf.email` | |
| URL | string | | | `kauf.website` | |
| **</ADDRESS>** | | | | | |
| **</PARTY> (customer)** | | | | | |
| **<PARTY> (delivery)** | | N | | | Data from adr access via `kauf.ladrnr` -> `adr.adrnr`. If `kauf.ladrnr` = 0, then fill with `kauf.l*`, but only if `kauf.lname` is not empty |
| PARTY_ID | string | | | `kauf.hausnr` -> `xhaus.linr` | |
| **<ADDRESS>** | | | | | |
| NAME | string | | | `adr.adrname` ... `kauf.lname` | |
| NAME2 | string | | | `adr.adrvname` ... `kauf.lvorname` | |
| NAME3 | string | | | `adr.branche` ... `kauf.lbranche` | |
| STREET | string | | | `adr.str` ... `kauf.lstr` | |
| ZIP | string | | | `adr.plz` ... `kauf.lplz` | |
| CITY | string | | | `adr.ort` ... `kauf.lort` | |
| COUNTRY | string | | | `xxland.iso` determined using `adr.kfzcode` or `kauf.lkfzcode` | [AW-106274] See "General data mapping" section |
| PHONE | string | | | `adr.telefon` | |
| FAX | string | | | `adr.fax` | |
| EMAIL | string | | | `adr.email` | |
| **</ADDRESS>** | | | | | |
| **</PARTY> (delivery)** | | | | | |
| **<ORDER_PARTIES_REFERENCE>** | | | | | |
| BUYER_IDREF | string | | | `kauf.kunr` | |
| SUPPLIER_IDREF | string | | | `kauf.hausnr` -> `xhaus.linr` | |
| **<SHIPMENT_PARTIES_REFERENCE>** | | Y | | | |
| DELIVERY_IDREF | string | | | 0 | See chapter "Determination of the external site number" |
| **</SHIPMENT_PARTIES_REFERENCE>** | | | | | |
| **</ORDER_PARTIES_REFERENCE>** | | | | | |
| **</ORDERRESPONSE_INFO>** | | | | | |
| **</ORDERRESPONSE_HEADER>** | | | | | |
| **<ORDERRESPONSE_ITEM_LIST>** | | | | | |
| **<ORDERRESPONSE_ITEM> (multiple)** | | | | | |
| LINE_ITEM_ID | string | Y | `<lfdpos>/<kuposnr>` Beispiel: `2/ABC123` | `kpos.lfdpos` `kpos.kuposnr` | For a detailed description, see chapter "Determination of the customer item ID". |
| **<PRODUCT_ID>** | | Y | | | |
| SUPPLIER_PID | string | | | `kpos.artnr` | |
| DESCRIPTION_SHORT | string | | | `kpos.artbez1` | |
| BUYER_PID | string | | | `kposex.exarttxt` | |
| **</PRODUCT_ID>** | | | | | |
| QUANTITY | decimal | Y | | `kpos.menge` | |
| ORDER_UNIT | dtPUNIT | | always "C62" (piece) | - | always "piece" |
| PRICE_LINE_AMOUNT | decimal | Y | | `kpos.npospreis` | |
| **<PRODUCT_PRICE_FIX>** | | | | | |
| PRICE_AMOUNT | decimal | | | `kpos.nstpreis` | |
| **<TAX_DETAILS_FIX>** | | | | | |
| TAX_AMOUNT | decimal | | | - | `invoiced FinAcFunct.GetItemVatAmount()` ??? |
| TAX | decimal | | | `kauf.mwstkz` / 100 | |
| **</TAX_DETAILS_FIX>** | | | | | |
| PRICE_QUANTITY | decimal | | always 1 (because of Order_UNIT "piece") | | |
| REMARK | string | | | `kpos.kommnr` -> `komm.kommtxt` | |
| **</PRODUCT_PRICE_FIX>** | | | | | |
| **</ORDERRESPONSE_ITEM> (multiple)** | | | | | |
| **</ORDERRESPONSE_ITEM_LIST>** | | | | | |
| **<ORDERRESPONSE_SUMMARY>** | | | | | |
| TOTAL_ITEM_NUM | string | | | - | Number of kpos records |
| TOTAL_AMOUNT | decimal | | | `kauf.gesbrutto` | |
| **<ALLOW_OR_CHARGES_FIX>** | | | | | |
| **<ALLOW_OR_CHARGE> (multiple)** | | | | | |
| ALLOW_OR_CHARGE_SEQUENCE | string | | | `kaufrab.seqnr` | |
| ALLOW_OR_CHARGE_TYPE | string | | surcharge/allowance | `kaufrab.satzart` | `kaufrab.satzart` = 0 => allowance <br> `kaufrab.satzart` = 1 => surcharge |
| ALLOW_OR_CHARGE_NAME | string | | | `kaufrab.txt` | |
| ALLOW_OR_CHARGE_DESCR | string | | | `kaufrab.aufnr`/`kaufrab.methode` | |
| **<ALLOW_OR_CHARGE_VALUE>** | | | | | |
| **<AOC_MONETARY_AMOUNT>** | float | | | `kaufrab.betrag` | |
| **</ALLOW_OR_CHARGE_VALUE>** | | | | | |
| **</ALLOW_OR_CHARGE>** | | | | | |
| **<ALLOW_OR_CHARGES_TOTAL_AMOUNT>** | float | | | | Sum of all kaufrab amounts |
| **</ALLOW_OR_CHARGES_FIX>** | | | | | |
| **</ORDERRESPONSE_SUMMARY>** | | | | | |

**ORDERRESPONSE_ITEM.LINE_ITEM_ID (#402154 + #403065)**
Since the order confirmation contains no element CUSTOMER_ORDER_REFERENCE, the information about the customer item ID must be accommodated in the element LINE_ITEM_ID.
For a detailed description, see chapter "Determination of the customer item ID".

#### 6.9.5. Dispatch notification based on the order data analogous to pre-delivery note

**Data Mapping**

| openTRANS xml element | Data type | Mandatory field | Description | AWE DB field | Comment |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **<DISPATCHNOTIFICATION_HEADER>** | | | | | |
| **<CONTROL_INFO>** | | | | | |
| GENERATOR_INFO | string | | File-generating program | | AWE B2B Service |
| GENERATION_DATE | string | | Date of file generation Format `yyyy-MM-ddT00:00:00` | | |
| **</CONTROL_INFO>** | | | | | |
| **<DISPATCHNOTIFICATION_INFO>** | | | | | |
| DISPATCHNOTIFICATION_ID | string | Y | | `kauf.auftrnr` - `lapool.routenr` | Combination of order number and route, separated by a hyphen |
| DISPATCHNOTIFICATION_DATE | string | Y | Format `yyyy-MM-ddT00:00:00` | | Date of the generation of this document |
| **<DELIVERY_DATE>** | | | | | |
| DELIVERY_START_DATE | string | | Format `yyyy-MM-ddT00:00:00` | `lapool.ltplan` | |
| DELIVERY_END_DATE | string | | Format `yyyy-MM-ddT00:00:00` | `lapool.ltplan` | |
| **</DELIVERY_DATE>** | | | | | |
| **<PARTY> (supplier)** | | Y | | | |
| PARTY_ID | string | | | `kauf.hausnr` -> `xhaus.linr` | |
| **<ADDRESS>** | | | | `xhaus.linr` -> `mp` | |
| NAME | string | | | `mp.name` | |
| NAME2 | string | | | `mp.vname` | |
| NAME3 | string | | | `mp.branche` | |
| STREET | string | | | `mp.str` | |
| ZIP | string | | | `mp.plz` | |
| CITY | string | | | `mp.ort` | |
| COUNTRY | string | | | `xxland.iso` determined using `mp.kfzcode` | [AW-106274] See "General data mapping" section |
| PHONE | string | | | `mp.telefon` | |
| FAX | string | | | `mp.faxnr` | |
| EMAIL | string | | | `mp.email` | |
| URL | string | | | `mp.website` | |
| **</ADDRESS>** | | | | | |
| **</PARTY> (supplier)** | | | | | |
| **<PARTY> (customer)** | | Y | | | |
| PARTY_ID | string | | | `kauf.kunr` | |
| **<ADDRESS>** | | | | | |
| NAME | string | | | `kauf.orgname` | |
| NAME2 | string | | | `kauf.orgvorname` | |
| NAME3 | string | | | `kauf.orgbranche` | |
| STREET | string | | | `kauf.orgstr` | |
| ZIP | string | | | `kauf.orgplz` | |
| BOXNO | string | | | `kauf.orgpostfach` | |
| ZIPBOX | string | | | `kauf.orgpfplz` | |
| CITY | string | | | `kauf.orgort` | |
| COUNTRY | string | | | `xxland.iso` determined using `kauf.orgkfzcode` | [AW-106274] See "General data mapping" section |
| PHONE | string | | | `kauf.orgtel` | |
| FAX | string | | | `kauf.faxnr` | |
| EMAIL | string | | | `kauf.email` | |
| URL | string | | | `kauf.website` | |
| **</ADDRESS>** | | | | | |
| **</PARTY> (customer)** | | | | | |
| **<PARTY> (delivery)** | | N | | | Data from adr access via `kauf.ladrnr` -> `adr.adrnr`. If `kauf.ladrnr` = 0, then fill with `kauf.l*`, but only if `kauf.lname` is not empty |
| PARTY_ID | string | | | `kauf.hausnr` -> `xhaus.linr` | |
| **<ADDRESS>** | | | | | |
| NAME | string | | | `adr.adrname` ... `kauf.lname` | |
| NAME2 | string | | | `adr.adrvname` ... `kauf.lvorname` | |
| NAME3 | string | | | `adr.branche` ... `kauf.lbranche` | |
| STREET | string | | | `adr.str` ... `kauf.lstr` | |
| ZIP | string | | | `adr.plz` ... `kauf.lplz` | |
| CITY | string | | | `adr.ort` ... `kauf.lort` | |
| COUNTRY | string | | | `xxland.iso` determined using `adr.kfzcode` or `kauf.lkfzcode` | [AW-106274] See "General data mapping" section |
| PHONE | string | | | `adr.telefon` | |
| FAX | string | | | `adr.fax` | |
| EMAIL | string | | | `adr.email` | |
| **</ADDRESS>** | | | | | |
| **</PARTY> (delivery)** | | | | | |
| BUYER_IDREF | string | | | `kauf.kunr` | |
| SUPPLIER_IDREF | string | | | `kauf.hausnr` -> `xhaus.linr` | |
| **<SHIPMENT_PARTIES_REFERENCE>** | | Y | | | |
| DELIVERY_IDREF | string | | | 0 | See chapter "Determination of the external site number" |
| **</SHIPMENT_PARTIES_REFERENCE>** | | | | | |
| **</DISPATCHNOTIFICATION_INFO>** | | | | | |
| **</DISPATCHNOTIFICATION_HEADER>** | | | | | |
| **<DISPATCHNOTIFICATION_ITEM_LIST>** | | | | | |
| **<DISPATCHNOTIFICATION_ITEM> (multiple)** | | | | | |
| LINE_ITEM_ID | string | Y | | `kpos.lfdpos` | |
| **<PRODUCT_ID>** | | Y | | | |
| SUPPLIER_PID | string | | | `kpos.artnr` | |
| DESCRIPTION_SHORT | string | | | `kpos.artbez1` | |
| BUYER_PID | string | | | `kposex.exarttxt` | |
| **</PRODUCT_ID>** | | | | | |
| QUANTITY | decimal | Y | | `lapool.iststk` | The packed quantity (`lapool.iststk`) is always taken over into the field „QUANTITY“. AWDesk #407233 <br> `lapool.iststk`: Verpackt-Stückzahl <br> `lapool.sollstk`: Soll-Stück (geplant) |
| ORDER_UNIT | dtPUNIT | | always "C62" (piece) | - | always "piece" |
| **<DELIVERY_REFERENCE>** | | | | | |
| **<DELIVERY_DATE>** | | | | | |
| DELIVERY_START_DATE | string | | Format `yyyy-MM-ddT00:00:00` | `lapool.ltplan` | |
| DELIVERY_END_DATE | string | | Format `yyyy-MM-ddT00:00:00` | `lapool.ltplan` | |
| **</DELIVERY_DATE>** | | | | | |
| **</DELIVERY_REFERENCE>** | | | | | |
| **<ORDER_REFERENCE>** | | Y | | | |
| ORDER_ID | string | Y | Reference order: `kauf.exaufnr` | See chapter "Determination of the external order number" |
| LINE_ITEM_ID | string | Y | `<lfdpos>/<kuposnr>` Example: `2/ABC123` | Reference order item: `kpos.lfdpos` `kpos.kuposnr` | For a detailed description, see chapter "Determination of the customer item ID". |
| ORDER_DATE | string | | | `kauf.edat` | |
| **</ORDER_REFERENCE>** | | | | | |
| **<SUPPLIER_ORDER_REFERENCE>** | | | | | |
| SUPPLIER_ORDER_ID | string | | | `kauf.auftrnr` | |
| SUPPLIER_ORDER_ITEM_ID | string | | | `kpos.lfdpos` | |
| **</SUPPLIER_ORDER_REFERENCE>** | | | | | |
| **<CUSTOMER_ORDER_REFERENCE>** | | | | | |
| ORDER_ID | string | | | Reference order: `kauf.exaufnr` | See chapter "Determination of the external order number" |
| LINE_ITEM_ID | string | | `<lfdpos>/<kuposnr>` Example: `2/ABC123` | Reference order item: `kpos.lfdpos` `kpos.kuposnr` | For a detailed description, see chapter "Determination of the customer item ID". |
| ORDER_DATE | string | | | `kauf.edat` | |
| **</CUSTOMER_ORDER_REFERENCE>** | | | | | |
| **<SHIPMENT_PARTIES_REFERENCE>** | | | | | |
| DELIVERY_IDREF | string | | | 0 | See chapter "Determination of the external site number" |
| **</SHIPMENT_PARTIES_REFERENCE>** | | | | | |
| REMARK | string | | | `kpos.kommnr` -> `komm.kommtxt` | |
| **</DISPATCHNOTIFICATION_ITEM> (multiple)** | | | | | |
| **</DISPATCHNOTIFICATION_ITEM_LIST>** | | | | | |
| **<DISPATCHNOTIFICATION_SUMMARY>** | | | | | |
| TOTAL_ITEM_NUM | string | | | - | Number of kpos records |
| **</DISPATCHNOTIFICATION_SUMMARY>** | | | | | |

**Dispatch notification items**
Dispatch notification items with quantity 0 will be listed in the xml document nevertheless.

**ORDER_REFERENCE.LINE_ITEM_ID (#403065)**
In the dispatch notification, the element ORDER_REFERENCE must absolutely be written according to the openTRANS specification.
For a detailed description, see chapter "Determination of the customer item ID".

#### 6.9.6. Invoice / credit note

**Credit notes**
Credit notes were implemented with PF [AW-87535]. For credit notes we use the same openTRANS document as for invoices. The distinction is made by the `<INVOICE_TYPE>` element.
In the header of the file ("REMARKS") header and footer texts assigned to the credit note are exported.

**Collective invoices**
Collective invoices can be exported in the same element structure as invoices. In the header, it is noted in the field INVOICE_COVERAGE whether this is a collective invoice.

**Data Mapping**

| openTRANS xml element | Data type | Mandatory field | Description | AWE DB field | Comment |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **<INVOICE_HEADER>** | | | | | |
| **<CONTROL_INFO>** | | | | | |
| GENERATOR_INFO | string | | File-generating program | | AWE B2B Service |
| GENERATION_DATE | string | | Date of file generation Format `yyyy-MM-ddT00:00:00` | | |
| **</CONTROL_INFO>** | | | | | |
| **<INVOICE_INFO>** | | | | | |
| INVOICE_TYPE | enum | Y | `kauf.vorgang` =7 => invoice<br>`kauf.vorgang` =9 => credit_memo | based on `kauf.vorgang` | Gutschrift -> PF [AW-87535] |
| INVOICE_COVERAGE | enum | | single (individual invoice)<br>collective (collective invoice) | | |
| INVOICE_ID | string | Y | | `kauf.auftrnr` | |
| INVOICE_DATE | string | Y | Format `yyyy-MM-ddT00:00:00` | `kauf.edat` | |
| **<DELIVERY_DATE>** | | | | | |
| DELIVERY_START_DATE | string | | Format `yyyy-MM-ddT00:00:00` | `kauf.ltplan`/`kauf.ltideal` | If ltplan is not assigned, ltideal is used |
| DELIVERY_END_DATE | string | | Format `yyyy-MM-ddT00:00:00` | `kauf.ltplan`/`kauf.ltideal` | If ltplan is not assigned, ltideal is used |
| **</DELIVERY_DATE>** | | | | | |
| **<PARTY> (supplier)** | | Y | | | |
| PARTY_ID | string | | | `kauf.hausnr` -> `xhaus.linr` | |
| **<ADDRESS>** | | | | `xhaus.linr` -> `mp` | |
| NAME | string | | | `mp.name` | |
| NAME2 | string | | | `mp.vname` | |
| NAME3 | string | | | `mp.branche` | |
| STREET | string | | | `mp.str` | |
| ZIP | string | | | `mp.plz` | |
| CITY | string | | | `mp.ort` | |
| COUNTRY | string | | | `xxland.iso` determined using `mp.kfzcode` | [AW-106274] See "General data mapping" section |
| VAT_ID | string | | presently not filled | `mp.steuernr` | VAT ID |
| PHONE | string | | | `mp.telefon` | |
| FAX | string | | | `mp.faxnr` | |
| EMAIL | string | | | `mp.email` | |
| URL | string | | | `mp.website` | |
| **<CONTACT_DETAILS>** | | | | | |
| CONTACT_NAME | string | | | `kauf.eusr`-> `mitarb.maname` | |
| FIRST_NAME | string | | | `kauf.eusr`-> `mitarb.mavname` | |
| **<EMAILS>** | | | | | |
| EMAIL | string | | | `kauf.eusr`-> `mitarb.email` | |
| **</EMAILS>** | | | | | |
| **</CONTACT_DETAILS>** | | | | | |
| **</ADDRESS>** | | | | | |
| **</PARTY> (supplier)** | | | | | |
| **<PARTY> (customer)** | | Y | | | |
| PARTY_ID | string | | | `kauf.kunr` | |
| **<ADDRESS>** | | | | | |
| NAME | string | | | `kauf.orgname` | |
| NAME2 | string | | | `kauf.orgvorname` | |
| NAME3 | string | | | `kauf.orgbranche` | |
| STREET | string | | | `kauf.orgstr` | |
| ZIP | string | | | `kauf.orgplz` | |
| BOXNO | string | | | `kauf.orgpostfach` | |
| ZIPBOX | string | | | `kauf.orgpfplz` | |
| CITY | string | | | `kauf.orgort` | |
| COUNTRY | string | | | `xxland.iso` determined using `kauf.orgkfzcode` | [AW-106274] See "General data mapping" section |
| NET_VALUE | string | | presently not filled | `kauf.steuernr` | VAT ID |
| PHONE | string | | | `kauf.orgtel` | |
| FAX | string | | | `kauf.faxnr` | |
| EMAIL | string | | | `kauf.email` | |
| URL | string | | | `kauf.website` | |
| **</ADDRESS>** | | | | | |
| **</PARTY> (customer)** | | | | | |
| **<PARTY> (delivery)** | | N | | | Data from adr access via `kauf.ladrnr` -> `adr.adrnr`. If `kauf.ladrnr` = 0, then fill with `kauf.l*`, but only if `kauf.lname` is not empty |
| PARTY_ID | string | | | `kauf.hausnr` -> `xhaus.linr` | |
| **<ADDRESS>** | | | | | |
| NAME | string | | | `adr.adrname` ... `kauf.lname` | |
| NAME2 | string | | | `adr.adrvname` ... `kauf.lvorname` | |
| NAME3 | string | | | `adr.branche` ... `kauf.lbranche` | |
| STREET | string | | | `adr.str` ... `kauf.lstr` | |
| ZIP | string | | | `adr.plz` ... `kauf.lplz` | |
| CITY | string | | | `adr.ort` ... `kauf.lort` | |
| COUNTRY | string | | | `xxland.iso` determined using `adr.kfzcode` or `kauf.lkfzcode` | [AW-106274] See "General data mapping" section |
| PHONE | string | | | `adr.telefon` | |
| FAX | string | | | `adr.fax` | |
| EMAIL | string | | | `adr.email` | |
| **</ADDRESS>** | | | | | |
| **</PARTY> (delivery)** | | | | | |
| CURRENCY | dtCURRENCY | | Currency | | if `kauf.wehrprs` = 1 -> `kauf.waehrung` -> `xwaehr.kurzbez`<br> if `kauf.waehrprs` = 0 -> MODUL_WAEHRUNG -> `xwaehr.kurzbez` -> Conversion to IG code; default: EUR |
| REMARKS1 (multiple) | | | | `auftxt.txt` | Header and footer texts (auftxt.drupos 1+ 2) invoices: auftxt.formular=4; Credit notes: auftxr.formular=5 |
| **<PAYMENT>** | | | Only for invoices, not for credit notes. | | |
| **<ACCOUNT>** | | | | | |
| HOLDER | string | | | empty | |
| BANK_ACCOUNT | string | | | empty | |
| **</ACCOUNT>** | | | | | |
| **<PAYMENT_TERMS>** | | | | | |
| **<TIME_FOR_PAYMENT> (multiple)** | | | | | |
| DAYS | short | | | `rechfuss.sktage1`/`rechfuss.sktage2`/`rechfuss.sktage3` | |
| DISCOUNT_FACTOR | float | | | `rechfuss.skvh1` bzw. `rechfuss.skvh2` bzw. `rechfuss.skvh3` / 100 | |
| **</TIME_FOR_PAYMENT>** | | | | | |
| **</PAYMENT_TERMS>** | | | | | |
| **</PAYMENT>** | | | | | |
| **</INVOICE_INFO>** | | | | | |
| **<ORDER_HISTORY>** | | | | | |
| ORDER_ID | string | Y | Customer order number of the reference order (remains empty for collective invoices) | Reference order: `kauf.exaufnr` | See chapter "Determination of the external order number" |
| SUPPLIER_ORDER_ID | string | | Supplier order number of the reference order (remains empty for collective invoices) | Reference order: `kauf.auftrnr` | |
| ORDER_DATE | string | | Format `yyyy-MM-ddT00:00:00` (remains empty for collective invoices) | Reference order: `kauf.edat` | |
| DELIVERYNOTE_ID | string | | ID of reference delivery note (remains empty for collective invoices) | Reference delivery note: `kauf.auftrnr`/`kauf.subnr` | |
| DELIVERYNOTE_DATE | string | | Format `yyyy-MM-ddT00:00:00` (remains empty for collective invoices) | Reference delivery note: `kauf.edat` | |
| **</ORDER_HISTORY>** | | | | | |
| **</INVOICE_HEADER>** | | | | | |
| **<INVOICE_ITEM_LIST>** | | | | | |
| **<INVOICE_ITEM> (multiple)** | | | | | |
| **<PRODUCT_ID>** | | Y | | | |
| SUPPLIER_PID | string | | | `kpos.artnr` | |
| DESCRIPTION_SHORT | string | | | `kpos.artbez1` | |
| BUYER_PID | string | | | `kposex.exarttxt` | |
| **</PRODUCT_ID>** | | | | | |
| LINE_ITEM_ID | string | | Serial numbering of the items | | |
| QUANTITY | decimal | | | `kpos.berechnet` | |
| ORDER_UNIT | dtPUNIT | | always "C62" (piece) | - | always "piece" |
| PRICE_LINE_AMOUNT | decimal | Y | | `kpos.npospreis` | |
| **<PRODUCT_PRICE_FIX>** | | | | | |
| PRICE_AMOUNT | decimal | | | `kpos.nstpreis` | |
| **<TAX_DETAILS_FIX>** | | | | | |
| TAX_AMOUNT | decimal | | | - | `invoiced FinAcFunct.GetItemVatAmount()` ??? |
| TAX | decimal | | | `kauf.mwstkz` / 100 | |
| **</TAX_DETAILS_FIX>** | | | | | |
| PRICE_QUANTITY | decimal | | always 1 (because of Order_UNIT "piece") | | |
| REMARK | string | | | `kpos.kommnr` -> `komm.kommtxt` | |
| **</PRODUCT_PRICE_FIX>** | | | | | |
| **<ORDER_REFERENCE>** | | | | | |
| ORDER_ID | string | Y | | Reference order: `kauf.exaufnr` | See chapter "Determination of the external order number" |
| LINE_ITEM_ID | string | Y | `<lfdpos>/<kuposnr>` Example: `2/ABC123` | Reference order item: `kpos.lfdpos` `kpos.kuposnr` | For a detailed description, see chapter "Determination of the customer item ID". |
| ORDER_DATE | string | | | Reference order: `kauf.edat` | |
| **</ORDER_REFERENCE>** | | | | | |
| **<SUPPLIER_ORDER_REFERENCE>** | | | | | |
| SUPPLIER_ORDER_ID | string | | | Reference order: `kauf.auftrnr` | |
| SUPPLIER_ORDER_ITEM_ID | string | | | Reference order item: `kpos.lfdpos` | |
| **</SUPPLIER_ORDER_REFERENCE>** | | | | | |
| **<CUSTOMER_ORDER_REFERENCE>** | | | | | |
| ORDER_ID | string | | | Reference order: `kauf.exaufnr` | See chapter "Determination of the external order number" |
| LINE_ITEM_ID | string | | `<lfdpos>/<kuposnr>` Example: `2/ABC123` | Reference order item: `kpos.lfdpos` `kpos.kuposnr` | For a detailed description, see chapter "Determination of the customer item ID". |
| ORDER_DATE | string | | | Reference order: `kauf.edat` | |
| **</CUSTOMER_ORDER_REFERENCE>** | | | | | |
| **<DELIVERY_REFERENCE>** | | | | | |
| DELIVERYNOTE_ID | string | | ID of reference delivery note | Reference delivery note: `kauf.auftrnr`/`kauf.subnr` | |
| LINE_ITEM_ID | string | | | Reference deliver note item: `kpos.lfdpos` | |
| **</DELIVERY_REFERENCE>** | | | | | |
| REMARKS1 | string | | | `komm.kommtxt` | |
| **</INVOICE_ITEM>** | | | | | |
| **</INVOICE_ITEM_LIST>** | | | | | |
| **<INVOICE_SUMMARY>** | | | | | |
| TOTAL_ITEM_NUM | string | | | - | Number of kpos records |
| TOTAL_AMOUNT | decimal | | | `rechfuss.gesbrutto` | |
| NET_VALUE_GOODS | decimal | | | `rechfuss.nettototal` | |
| **<TAX_DETAILS_FIX>** | | | | | |
| TAX_AMOUNT | decimal | | | `rechfuss.mwstbetrag` | |
| TAX | decimal | | | `rechfuss.mwstkz` / 100 | |
| **</TAX_DETAILS_FIX>** | | | | | |
| **<ALLOW_OR_CHARGES_FIX>** | | | | | |
| **<ALLOW_OR_CHARGE> (multiple)** | | | | | |
| ALLOW_OR_CHARGE_SEQUENCE | string | | | `kaufrab.seqnr` | |
| ALLOW_OR_CHARGE_TYPE | string | | surcharge/allowance | `kaufrab.satzart` | `kaufrab.satzart` = 0 => allowance<br>`kaufrab.satzart` = 1 => surcharge |
| ALLOW_OR_CHARGE_NAME | string | | | `kaufrab.txt` | |
| ALLOW_OR_CHARGE_DESCR | string | | | `kaufrab.aufnr`/`kaufrab.methode` | |
| **<ALLOW_OR_CHARGE_VALUE>** | | | | | |
| **<AOC_MONETARY_AMOUNT>** | float | | | `kaufrab.betrag` | |
| **</ALLOW_OR_CHARGE_VALUE>** | | | | | |
| **</ALLOW_OR_CHARGE>** | | | | | |
| **<ALLOW_OR_CHARGES_TOTAL_AMOUNT>** | float | | | | Sum of all kaufrab amounts |
| **</ALLOW_OR_CHARGES_FIX>** | | | | | |
| **</INVOICE_SUMMARY>** | | | | | |

**Invoice items**
Invoice items with quantity 0 will NOT be listed in the xml document.

**ORDER_REFERENCE.LINE_ITEM_ID (#403065)**
In the invoice, the element ORDER_REFERENCE must not absolutely be written according to the openTRANS specification.
If there is an external order reference, it is written.
For a detailed description, see chapter "Determination of the customer item ID".

### 6.10. Hornbach export
The Hornbach export was developed with AWDesk #407285.
This interface is a user end customer-specific version of the openTRANS interface.
There is a precise description on the Sharepoint in the document:
[https://awsoftwaregmbh.sharepoint.com/:w:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/DE-A+W%20Enterprise%20B2BService%20Hornbach%20Vegla.docx?d=w81bbd82249014459a962b22d39d2870d&csf=1&web=1&e=WELSCa](https://awsoftwaregmbh.sharepoint.com/:w:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/DE-A+W%20Enterprise%20B2BService%20Hornbach%20Vegla.docx?d=w81bbd82249014459a962b22d39d2870d&csf=1&web=1&e=WELSCa)

## 7. PO export / A+W EDI export
With AWDesk #422752, the logic for exporting POs in the A+W EDI standard format was implemented. The logic requires no ERP Webservice.
The installation instructions and explanation of the config tool settings are made available in the installation document for the B2B service.
The entire description of the A+W EDI Export interface and the configuration instructions are in the configuration document for "A+W Enterprise EDI."

## 8. E-invoicing – XRechnung
Implemented with PF [AW-111997].

> **CAUTION:**
> The topic "XRechnung" is complex. Various requirements must be fulfilled for the activation of XRechnung. Checking the requirements must be done customer-specifically or client-specifically by AWE planning. It may be necessary for planning and service to make adjustments.
> Therefore, please heed the "Requirements" chapter.
> Generation of the XRechnung format (as of 08/29/2024) is still in the pilot phase. Therefore, it is not yet safe to assume that the customer will receive a completely implemented product.

### 8.1. General Information
The XRechnung is a specified format for electronic invoices in Germany, which implements the EU-wide standard for electronic invoice exchange. It was developed as part of the EU directive 2014/55/EU, which encourages the digitalization and standardization of invoicing within public administration.

An XRechnung is based on XML structures and includes standardized data fields to ease the exchange of invoice information. Public authorities in Germany are obliged to accept invoices in electronic form since November 27, 2020 and they may only accept e-invoices that correspond to this standard.

Generating electronic invoices means generating an invoice format that can be read in automatically (mechanically).
The EU agreed upon a standard in 2017, which is specified in the standard EN 16931 (CEN/TC 434 EN 16931).In the same year, the "ordinance concerning electronic invoicing in Federal publish purchasing" was published in the Federal Law Gazette.
In Germany, due to this ordnance, "XRechnung" is used as electronic invoice format. XRechnung fulfills the EU standard.
Initially introduced only for B2G business transactions in Germany, XRechnung is increasingly being used for domestic B2B and B2C business transactions.

The A+W Enterprise B2B Service offers the opportunity to generate customer-specific electronic invoices in the XRechnung format.
The prerequisite is that XRechnung has been configured as invoice format for customers in the A+W Enterprise market partner master data. See Chapter "Configuration of the master data."

#### 8.1.1. Definition
From https://www.e-rechnung-bund.de/erp-hersteller:
The "XRechnung" standard, consisting of different components, is developed and operated by the coordination office for IT standards (KoSIT). This includes the specification of "XRechnung" itself, which is composed of the semantic data model and the technical implementation of the business rules. The business rules determine the logical dependencies of the invoice contents and are an essential component for the implementation of the specification. For this reason, it is recommended that you familiarize yourself with the precise legal rules.
In addition to the "XRechnung" specification, other components are provided, which support the technical implementation of the standard and can be used for the transmission of invoices:
- The validator configuration as open source reference implementation for checking of an XML document for conformity with XRechnung
- The test suite with test cases (sample invoices and reference messages)
- The development resource for support of the visualization of XRechnung

#### 8.1.2. CIUS
The standard XRechnung represents a national design of the European standard EN 16931, a so-called core invoice usage specification (CIUS). The national design of the directive in the other EU member states specifies this with local specifications within the framework specified by the standards.

#### 8.1.3. Additional information
A short overview of the functionality is in the performance description "A+W Enterprise Order Invoice to XML".

The detailed data mapping is described in the Excel sheet:
[https://awsoftwaregmbh.sharepoint.com/:x:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/XRechnung_UBL_AWE_DataMapping.xlsx?d=wf72f02fd93e643a89874003b1618aff3&csf=1&web=1&e=6pBqSv](https://awsoftwaregmbh.sharepoint.com/:x:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/XRechnung_UBL_AWE_DataMapping.xlsx?d=wf72f02fd93e643a89874003b1618aff3&csf=1&web=1&e=6pBqSv)

Detailed information about the principle of the electronic invoice are found on the Sharepoint at:
[https://awsoftwaregmbh.sharepoint.com/:b:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/Rechnungen_XRechnung_ZUGFeRD_Konzept.pdf?csf=1&web=1&e=Da27hz](https://awsoftwaregmbh.sharepoint.com/:b:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/Rechnungen_XRechnung_ZUGFeRD_Konzept.pdf?csf=1&web=1&e=Da27hz)

Additional notes are also in the associated functional description "A+W Enterprise Order Invoices to XML".

### 8.2. Requirements
The chapter includes, in the form of a checklist, a rough overview of the requirements that must be checked so that XRechnung can be activated in the customer system.
All points on the checklist are explained in other places in this or other configuration documents.

- The new discount logic must be active. (RABATTLOGIK_2005 = ON)
- Invoice report/invoice form:
  - No old rep reports may be used, but only CrystalReports reports. Are there calculations on the form?
  - If so, why?
  - Do the calculations have to be included in XRechnung?
  - Should XRechnung plus PDF invoice be sent (match!)?
- Check the currencies used in the system
  - See "Currency ISO code" chapter.
- Archiving:
  - How should the XRechnung archiving be done?
  - Is there already an archiving concept?
  - Can the existing archiving process be retained?
- XRechnung-Viewer:
  - Is it possible to "view" generated XRechnungen?
  - There are tools for displaying the xml format. For example, the eRechnung viewer "Ultramarinviewer".
  - A+W only points out that "Ultramarinviewer" can be used. This is not an A+W recommendation.
- Validation of the XRechnung:
  - The recipient of the XRechnung generally uses a validation tool to check the validity of the electronic invoice.
  - Many validation tools are available online and can be used without restriction.
  - Does the customer user a validation tool? If so, which one?

### 8.3. Electronic invoice and PDF invoice (report)
An invoice counts as electronic invoice if it is machine-readable, that is, if it can be read in automatically and processed by a computer program.
In Germany, among other things, XRechnung is used as electronic invoice format.
In AWE, previously PDF invoices were generated and sent. The configuration in the market partner master data allows that the customer PDF invoice and an electronic invoice are activated for a customer.
The customary PDF invoice is not linked to the electronic invoice in any way.

**Please note:**
If an electronic invoice is sent to the customer and also a PDF invoice, then the electronic invoice is the valid and determining one.
A PDF sent in addition is not relevant. Attention must be paid that both invoices are the same and do not contain amounts that deviate from one another due to separate calculations in the report.
The customary PDF invoice is not to be confused with an invoice in the ZUGFeRD format. The invoice in the ZUGFeRD format is a PDF/A-3, in which the electronic invoice is embedded.
With the ZUGFeRD format, it is specified that the PDF/A-3 must contain precisely the invoice information that also exists in the embedded electronic invoice. No information may be omitted and none may be added. Here too, the embedded electronic invoice is the valid one.

### 8.4. XRechnung version
The XRechnung standard is implemented in Version 3.0 (more precisely, 3.0.2)
The schema used is "UBL Invoice 2.3".

### 8.5. ZUGFeRD version
ZUGFeRD was previously implemented in Version 2.3.2.
Starting on 05/15/2025, ZUGFeRD Version 2.3.3 is implemented.
As a basis, the complete version invoice CII D22B is used:

**ZUGFeRD Profile Levels (Data on Document Level vs. Data on Item Level)**
- **Vollständige INVOICE CII D22B** (Complete)
  - **Profil EXTENDED**
    - **Profil EXTENDED-B2B-FR**
      - **Profil EXTENDED-CTC-FR**
        - **Profil EN16931**
          - **Profil BASIC WL (Factur-X)**
          - **Profil BASIC (Factur-X)**
          - **MINIMUM**

To generate ZUGFeRD format, the entry "ZUGFeRD" must be selected in the recipient's MP master data on the "Invoice" dialog in the "Dispatch type" field.

### 8.6. Manual validation of the XRechnung
There are many online validation tools available.
The validation tools that were used in the course of development to check generated XRechnungen are listed below:
- https://www.epoconsulting.com/erechnung-sap/xrechnung-validator
- https://ecosio.com/de/peppol-und-xml-dokumente-online-validieren/
  (Here it is not only necessary to upload the file, but also to select the correct xml document: UBL Invoice 2.3)

### 8.7. Installation A+W Enterprise

#### 8.7.1. Binfile/environment
- Binfiles and environment must be at least QR[2410] or newer.
- Ideal prerequisite is QR[2503].
- For QR[2410] 2 sql scripts must be executed, which are first executed automatically with QR[2503]:
  - `130004273_printparamok.sql`
  - `130004268_printparam.sql`

#### 8.7.2. al tables
- The table `aldfuetyp_tab` must include all current entries.
- The table `aldfuectrl_tab` must include all current entries.
- For language-dependent messages in the e-mails and names in the MP-specific configuration (mpdfuectrl), the tables `alerrmsg/errmsg`, `messages` and `fx_texte` must be up to date.

#### 8.7.3. Error messages
For language-dependent names in the xml file, the following message numbers must exist in the table errmsg:
- 38529 - General discount
- 38530 - General surcharge
If the entries do not exist, an English default text is used.

#### 8.7.4. Report texts
The report texts (`cr_repstrings` table) must be up-to-date.
The report texts are made available by A+W and during installation/update of the environment, taken over by the customer into the table `alrepstrings` inserted and after `cr_repstrings`.
The automatic takeover after `cr_repstrings` is only possible if in the language master data (Master data > Keys > System > Languages) the AWE language is maintained correctly.
In the A+W development environment, `alrepstrings` is a view that is filled from `pantrans`. When packing the environment, `alrepstrings` is unloaded.
On the customer system, `alrepstrings` is a table that is filled with the unloaded records during installation/update.
In `alrepstrings`, the `sprkz` (as in `pantrans`) corresponds to the AWE language from `alerrmsg` Nr.17 (beginning with deutsch=0).
In `cr_repstrings`, the `sprkz` corresponds to the text language from `xsprzu.sprkz`.

> **Caution:**
> During update of the environment, all report texts are taken over anew from the table `alrepstrings` after `cr_repstrings`. If at the customer one or several of these texts specified by A+W were changed via the maintenance screen, such customer changes are lost during the update.

The report texts made available by A+W can be recognized by the activated A+W flag (`cr_repstrings.awflag`) and on the type designators with the prefix "cr_".
All report texts that were generated specially for XRechnung bear the prefix "cr_xr_".
Note: On the customer system, the `awflag` can be changed for an entry (type).
Menu Master Data > Keys > System > Report Texts.
The following entries must be present for "Type".

| Type | A+W Text German | Comment |
| :--- | :--- | :--- |
| 1 cr_postbox | P.O. box | |
| 2 cr_custit | Reference | |
| 3 cr_width | Width | |
| 4 cr_height | Height | |
| 5 cr_xr_dims | Sizes | Added specially for XRechnung. |
| 6 cr_cav | AIR | |
| 7 cr_thickness | Thickness | |
| 8 cr_xr_shape | Shape number | Added specially for XRechnung. |
| 9 cr_xr_ceo | Management | Added specially for XRechnung. |
| 10 cr_xr_cosb | Headquarters of the Supervisory Board | Added specially for XRechnung. |
| 11 contract | Project | The project number (kauf.objnr) is transferred in a note element on the header level. The report text "contract" will be used as label. This "type" is an exception since it does not begin with "cr_". |

### 8.8. Installation B2B service
To use the XRechnung functionality, the current version of the A+W Enterprise B2B Service must be installed. See also the separate installation instructions.

### 8.9. Configuration - B2B Service config tool
The generation of electronic invoices by the B2B service is activated with the "E-Invoice Export" checkbox in the "Common Settings" section of the configuration tool.

On the "E-invoice export settings" dialog, the basic path for storage of the files generated is configured via the "Export Root Path" field.

The export path must absolutely be configured if:
- The env variable `EINVOICE_NO_REFDAT` is active (that is, that the generated xml file is NOT saved as file attachment)
- The generation of the e-invoice is initiated manually (for example, using a script)

However, it is recommended that you store the path in every case regardless of the configuration of `EINVOICE_NO_REFDAT` since in case of error the file generated if necessary will be stored in this path for research purposes.
The B2B service must be able to reach the directory and have write access rights to it.

**Note:**
For the automatic generation of the XRechnung, the file is stored as A+W Enterprise file attachment in a subdirectory for which the folder is defined in the environment variable `DATEI_REF_PFAD`.
See special section "XRechnung document as file attachment".

### 8.10. Configuration - environment variables

#### 8.10.1. MODUL_EINVOICING
The electronic invoice export functionality is released with a module variable `MODUL_EINVOICING`.

#### 8.10.2. EINVOICE_NO_REFDAT
Deactivates the storage of the e-invoices/credits as document attachment in the table `kaufref`.

#### 8.10.3. NO_EINVOICE_FOR_INTERN_CR_NOTE
If the variable is active, it is possible to define in each credit directly in the header under "Credit type" (`kauf._rechart`) whether this is an external or internal credit.
If the env variable is not active, the "Credit type" label exists and the toggle values "external/internal" (0|1) do not.
Internal credits (`kauf._rechart` = 1) are NOT exported as e-invoice.

#### 8.10.4. RABATTLOGIK_2005
The new discount logic must be active.
`RABATTLOGIK_2005 = ON`.

#### 8.10.5. REP_FAKTURA
Invoice and credit note form types for "electronic invoices" (e-invoicing) must be entered in the environment variable `REP_FAKTURA`.

#### 8.10.6. SKONTO_SPECIAL
With the variables, the alternative procedure for cash discount records in the customer master and in the order is activated. Cash discounts can then be created language-specifically. The table `xxskonto` is filled (instead of previously `xskonto`).

#### 8.10.7. EINV_FORMART_RECH
In the variables, the form type (`xemail.formart`) for electronic invoices (e.g., XRechnung) is stored. The form type stored here is required if in the e-mail addresses a special e-mail address for electronic invoices should be configured.

#### 8.10.8. EINV_FORMART_GUTS
In the variables, the form type (`xemail.formart`) for electronic credit notes (e.g., XRechnung) is stored.
The form type stored here is required if in the e-mail addresses a special e-mail address for electronic credit notes should be configured.

#### 8.10.9. XWAEHR_ISOCODE_FIELD
With the variable, it is specified in which field of the key table "Currency" (`xwaehr`) the currency code is stored according to the international standard "ISO 4217 alpha-3".
The ISO currency code is required for the generation of the electronic invoice (XRechnung).
1. ISO code in the "Abbreivation" field (`xwaehr.kurzbez`)
2. ISO code or numeric value of the ISO code in the "FinAc Key" field (`xwaehr.fibuschl`)
3. Numeric value of the ISO code in the "Nr" field (`xwaehr.wnr`)

If the variable is not active or contains an undefined value, during the generation of the electronic invoice, the ISO code in the "Abbreviation" field (`xwaehr.kurzbez`) is expected.

### 8.11. Configuration – SPs

#### 8.11.1. rpgeteinvemailaddress
With the SP, the e-mail addresses of the e-invoice are determined.
The script for the SP can be found under:
`...\alcib\14\0\de\install\xsql\sp\rp`

#### 8.11.2. cu_get_e_invoice_name
The name of the e-invoice file is generated with the SP.
This is a customizing SP. There is no default version of the SP that is provided by A+W.

### 8.12. Configuration – MP-specific (mpdfuectrl)
[SVH 26.06.2025 – Chapter currently being edited]

If no MP-specific configuration exists, the e-invoice will be generated in the format of an XRechnung, type UBL.
If no MP-specific configuration exists and if the dispatch type "ZUGFeRD" is configured in the MP master data, the e-invoice will be generated in the format of an XRechnung, type CII.

The configuration is done for the EDI type "120" (e-invoice).
Possible configuration settings:
- ID 69 (validation)
- ID 70 (XML format)
The configuration must be done MP-specifically. An MP-spanning configuration is not evaluated.

### 8.13. Configuration of the master data

#### 8.13.1. Seller/Supplier
The configuration of the seller master data described here is obligatory.
The seller is defined via the supplier in the table `xhaus` (field `xhaus.linr`). If necessary, it can be configured client-specifically. If no internal EDI should be executed with this supplier, the supplier can also be written negatively to `xhaus.linr`.

> **Caution:**
> If for the sellers/suppliers a FinAc debtor with deviating market partner number is stored, the entire master data configuration described for the FinAc debtor must be made.

The following details must be stored for the suppliers/creditors in the MP master data:

**"Address" dialog**
- **E-Mail address (mp.email)**
  This e-mail address will be taken over into the e-invoice as default address.
  However, the entry is overridden by the e-mail configuration that is stored for the buyer. The sender address specified in the buyer master data (`xemail.emailabs`) takes precedence.

**"Identification" dialog**
- VAT ID No.
- Trade register

**"Invoice" dialog**
- "E-invoice" must be actived with the checkbox.

#### 8.13.2. Buyer/Recipient
The configuration of the buyer master data described here is obligatory.

> **Caution:** If for ordercustomers a FinAc debtor with deviating market partner number is stored, the entire master data configuration described for the FinAc debtor must be made.

So that automatic invoice generation + booking and manual invoice generation + booking behave the same way with regard to the debtor, the `alcib` binfile must have at least the version 13.04.18690.

> **Caution:**
> The simultaneous activation of openTRANS invoice export and e-invoice export for a customer is not forbidden by A+W Enterprise (status as of 01/17/2025).
> However, the simultaneous sending of different invoice formats for one and the same invoice to a customer should absolutely be avoided.
> Please check during configuration of e-invoice that no sending of openTRANS invoice is active.

Customers (FinAc debtors) that should receive an e-invoice require particular details in the MP master data and have to be identified explicitly there.
For an e-invoice customer, the following details must be stored in the MP master data:

**"Identification" dialog**
- VAT ID No.

**"Invoice" dialog**
- Activating the "e-invoice" checkbox
- To generate ZUGFeRD format, the entry "ZUGFeRD" must be selected in the "Dispatch type" field.
- Route ID (mandatory, see separate section about this)

#### 8.13.3. Buyer/Recipient - e-mail addresses
The configuration of the e-mail addresses in the master data is obligatory.
In the XRechnung, the e-mail address of the invoice recipient is mandatory. The recipient e-mail address must be stored via the contact data > E-mail addresses (table `xemail`).
Menu "Master Data > Market Partner > F4 > Contact Data > E-mail Addresses".
The XRechnung contains the sender e-mail address of the seller and the recipient e-mail address of the buyer.
With an entry in the e-mail addresses, the recipient e-mail address and the override of the master data entry for the sender e-mail address can be specified.
The sender e-mail address does not absolutely have to be stored in `xemail`. If it does not exist in `xemail`, it is drawn from the seller's master data (`mp.email`).

For this, a data record for a special form type, one each for invoices and credit notes, can be created.
For invoices, the desired form type is stored in the environment variable `EINV_FORMART_RECH`. For credit notes, the desired form type is stored in the environment variable `EINV_FORMART_GUTS`.
Alternatively, a general data record for the form type "0" can be stored.
The fields "Employee" and "Department" are populated with the value "0".

The logic for determining the e-mail addresses is described precisely again in the section "Determining the valid record from the market partner e-mail addresses".

#### 8.13.4. Document types - document type of the e-invoice
The configuration of the document type of the e-invoice is obligatory.
Menu "Master Data > Keys > System > Document Types".
The document type "E-invoice" must be created for the e-invoice. For this document type, the document type (`xdokutype.dokutyp`) "E-invoice" must be selected.
For the document type "E-invoice", the "VF" checkbox (=takeover into the document) must be activated. Only if this entry is present can the B2B service save the XRechnung correctly as document attachment.
For the document type "E-invoice", the "type of output" (`xdokutype.ausgabeart`) must be set to "via e-mail" if the XRechnung should be sent via the Print Service.
Furthermore, this document type must then be assigned a form and a recipient. This happens on the "System > Print Management > Forms > Document Type Allocation" menu
For a further description of sending the XRechnung, see the configuration instructions for the "Enterprise Print Service".

#### 8.13.5. Company items
The configuration of company items is optional.
If in the XRechnung the management and the headquarters of the supervisory board are specified, the corresponding company items must be present.
For this, two items must be defined via the menu "Master Data > Keys > Item > Position" on the "Items" dialog:
1.  **Management:**
    An item for which the value "Manager" is selected in the "Leading Position" field.
2.  **Chair of the supervisory board:**
    An item for which the value "Chair of the supervisory board" is selected in the "Leading position" field.

Language-specific names for the company items can be stored.
Then the manager and supervisory board are assigned via Contact Person (see separate section).

#### 8.13.6. Countries ISO code
For Germany and the country of the buyer's invoice address, the 2-digit country ISO code according to ISO 3166-1 must be stored.
Menu "Master Data > Keys > Market Partner > Countries", field "ISO".

#### 8.13.7. Currency ISO code
The currency used in the XRechnung depends on the currency that is stored for the invoice recipient and in the invoice and the associated selection field "Print in".
The generation of the XRechnung can either be done in own currency or foreign currency.
If "Foreign currency" is selected, you must be sure that in the currency key (Master Data > Keys > System <> Currency), the ISO code in the format "ISO 4217 alpha-3" is specified for the currency used.
Since the currency table does not have an explicit field for the ISO code, it is specified via the setting in the env variable `XWAEHR_ISOCODE_FIELD` in which field of the currency table the ISO code is found; see the description of the env variable.
If the env variable `XWAEHR_ISOCODE_FIELD` is not active or contains an undefined value, during the generation of the electronic invoice, the ISO code in the "Abbreviation" field (`xwaehr.kurzbez`) is expected.
In the XRechnung, currently the following currency ISO codes are considered.

| ISO code | Numeric value | Currency | Country |
| :--- | :--- | :--- | :--- |
| AUD | 36 | Dollar | Australia |
| CHF | 756 | Franks | Switzerland |
| CNY | 156 | Yuan | China |
| EUR | 978 | Euro | ECU countries |
| GBP | 826 | Pound | Great Britain |
| HKD | 344 | Dollar | Hong Kong |
| INR | 356 | Rupee | India |
| JPY | 392 | Yen | Japan |
| KRW | 410 | Won | South Korea |
| PLN | 985 | Zloty | Poland |
| RUB | 643 | Ruble | Russia |
| SGD | 702 | Dollar | Singapore |
| TWD | 901 | Dollar | Taiwan |
| USD | 840 | Dollar | USA |

If in the customer system a currency is used that is not listed in the table, please inform the A+W Enterprise development department.

#### 8.13.8. Tax code
The configuration of the tax code is optional. However, it is explicitly recommended.
QR[2503] is required for this functionality.
Menu Master Data > Keys > System > Taxes > Tax Rates

Based on the code list UNTDID.5305 ([https://www.xrepository.de/details/urn:xoev-de:kosit:codeliste:untdid.5305_1](https://www.xrepository.de/details/urn:xoev-de:kosit:codeliste:untdid.5305_1)), in the tax records in the field "E-invoice", the tax code is stored that should be transferred in the e-invoice.
If no tax code is stored in the "E-invoice" field, the default code "S" will be used.
If no tax code is stored in the "E-invoice" field and the invoice does not contain a tax record > 0, the code "Z" will be used.

**Overview of the most important tax codes**

| Alphanum. Code | Name EN | Bezeichung DE |
| :--- | :--- | :--- |
| S | Standard rate | Standardsteuersatz |
| Z | Zero rated goods | steuerfreie Waren |
| E | Exempt from tax | steuerbefreit |
| AE | VAT Reverse Charge | Umkehr der Steuerschuldnerschaft |
| K | VAT exempt for EEA intra-community supply of goods and services | Mehrwertsteuerbefreiung für innergemeinschaftliche Lieferungen von Waren und Dienstleistungen im EWR |
| G | Free export item, tax not charged | Kostenlose Ausfuhrsendung, ohne Steuer |
| O | Services outside scope of tax | nicht steuerpflichtige Dienstleitungen |
| L | Canary Islands general indirect tax | Allgemeine indirekte Steuer der Kanarischen Inseln |
| M | Tax for production, services and importation in Ceuta and Melilla | Steuer auf Produktion, Dienstleistungen und Importe in Ceuta und Melilla |

#### 8.13.9. Method of payment code
The configuration of the method of payment code is optional. However, it is explicitly recommended.
QR[2503] is required for this functionality.
Master data > Keys > System > Payment method

Based on the code list UNTDID.4461 ([https://www.xrepository.de/details/urn:xoev-de:xrechnung:codeliste:untdid.4461_3#version](https://www.xrepository.de/details/urn:xoev-de:xrechnung:codeliste:untdid.4461_3#version)) in the payment method in the "E-invoice" field, the payment method code is stored that should be transferred in the e-invoice.
If no payment method code is stored in the "E-invoice" field, the code "58" ("SEPA credit transfer") is used.

#### 8.13.10. Contact Person
The configuration of contact partners is optional.
Menu "Master Data > Market Partner > F4 > Contact Data > Contact person".

**Seller/Supplier**
If in the XRechnung the management and the headquarters of the supervisory board should be specified, the contact person for management and the chair of the supervisory board must be created in the seller master data.
1.  A contact person must be created for each person who is part of the management. By selecting the "Item", the contact person is marked as management. Using the "List sequence" field, you can specify in which order the managers are specified on the XRechnung.
2.  Headquarters of the supervisory board
    Only one contact person may be identified via the "Item" field as chair of the supervisory board.

**Buyer/Recipient**
If the XRechnung should include a buyer contact, there must be a contact person for the buyer.
In the invoice, the buyer contact is stored on the "Properties" dialog, "Employee assignment" grouping, field "Ordered by" (`kauf.buser`).
A new contact person can be created directly during document entry, field "Ordered by".

#### 8.13.11. Employee
The configuration of an employee as seller contact is optional.
If in the XRechnung a special seller contact should be specified, an appropriate employee must be created in the master data from whom the contact data is drawn.
The seller contact is stored in the invoice on the dialog "Properties, "Employee assignment" grouping, "User" field (`kauf.abvertr`).
If no contact is stored in the "User" field, the contact data:
- Name
- Phone number
- E-mail address
from the seller's master data is used.

> **Caution:** A seller contact is only taken over in the XRechnung if the contact data is complete. This means that there must be a name, phone number, and e-mail address.

#### 8.13.12. Bank details
The configuration of bank details is optional.
If in the E-invoice one or several bank details should be specified, the bank details must be stored appropriately in the seller master data.
Attention must be paid that in the seller's master data on the "Invoice" dialog, the "E-invoice" is activated. Only then can a prioritization be entered for the stored bank details.
Menu "Master Data > Market Partner > F4 > Contact Data > Bank Details".
- The "IBAN" field must be filled
- In the "E-invoice" field, the value "XRechnung" must be selected
- In the priority field, the sequence can be specified in which the bank details are listed on the E-invoice

The bank details are listed according to the priority entered (1,2,3, etc.) in the XRechnung.
If bank details are marked for XRechnung (value "XRechnung" in the "E-invoice" field), but no priority is specified, these bank details are taken over into the XRechnung; they are added to the list at the end after the bank details with priority.
If there are several sets of bank details with "XRechnung" marking but without priority, they are listed in the XRechnung after the bank details with priority. The sequence is random here.

#### 8.13.13. Configurable Texts
The creation of configurable texts is optional.

**Header and footer texts**
Customer-specific header/footer texts can be specified, which are then taken over into the XRechnung.
Example of header texts:
"Glass structure from outside to inside."
or
"Delivery of the goods was made according to our general terms of sale and delivery."

Menu "Master Data > Text Management > Configurable Texts".
The condition for a configurable header/footer text is specified via a stored procedure (SP). You must pay attention that the SP name only includes lower-case letters. The name of the function has to commence with "cu_".
Every text can be stored language-specifically. If your system is multilingual, the environment variable `KONFIGTEXTE_MEHRSPRACHIG` must be set.
For multi-line texts, you must pay attention that the line ends with a complete word. Word separation should absolutely be avoided.

An example for an SP, which generates header/footer texts for XRechnung, is saved under:
`.../install/xsql/cust/st/cu_getmprechexport.sql`.
The SP "`cu_getmprechexport.sql`" checks whether a document of the invoice export is configured for the customer.
In the "Value" field, the expected return value of the SP is stored.
The sequence of the texts is specified via the "Nr" field in the configurable texts.

**Remarks:**
The details about the SP are stored in the table `auftxtzu`.
The stored text is not saved in a file, but under a defined text number for a defined file name (`auftxtzu.datei` = `xtxtnr.datei` -> `xtxtnr.txtnr` = `stammtxt.txtnr`) in the table `stammtxt`.
For each text, the form types (`auftxtzu.formvec`) can be determined for which the text is valid.

> **Caution:**
> Under some circumstances, the environment variables RECH_MIT_KONFIGTXT and GUTS_MIT_KONFIGTXT must be set. See the configuration instructions for "Enterprise".

### 8.14. Functions

#### 8.14.1. General
The B2B Service generates an electronic invoice in the XRechnung format. This is an xml document.
The generation is triggered on invoice booking (if the invoice could be booked successfully). During invoice booking, a transfer record is written to the table `ottransfer`, which is then processed by the B2B Service. For details on the transfer record, see section "Control table ottransfer".

**Transfer record in table ottransfer**
The transfer record in the table `ottransfer` is generated by A+W Enterprise.
For this, the MP-specific configuration of the XML format of the e-invoice (`mpdfuectrl`, ID 70) is evaluated.
If for the XML format a value > 0 is stored, this value will be taken over as "doctype" in the ottransfer record.
If no value is stored or if the value is "0", the "doctype" in the ottransfer record is assigned the default value "1".
The "Configuration -- MP-specific" chapter describes what the values mean.

#### 8.14.2. Invoice handling
Both a document-related invoice and a manual invoice without reference to an XRechnung can be generated.
If the invoice recipient complains about the XRechnung and correction is required, the normal AWE process takes over here. The invoice is canceled. A credit and a new invoice are created.

#### 8.14.3. Language
In which language the text of the XRechnung is output is determined by the language of the invoice (`kauf.sprkz`).

#### 8.14.4. File generation and file name

**Specification of the file name (SP cu_get_e_invoice_name")**
The file name of the XRechnung can be specified customer-specifically via the stored procedure "`cu_get_e_invoice_name`". The use of the SP is optional.
If the SP does not exist, a default name is used that is specified by the program.
With use of the SP, you must pay attention that the generated file name does not contain any blank spaces.
The SP has the following parameters: `cu_get_e_invoice_name(kauf.auftrnr, kauf.vorgang, kauf.subnr, kauf.hausnr, kauf.kunr)`.
The file name returned from the SP may be a maximum of 255 characters long.
The file name returned from the SP must have the file extension ".xml".

If the SP "`cu_get_e_invoice_name`" does not exist and the XRechnung is generated as attachment (document attachment), a default name is used, which is specified by the AWE backend.
For invoices, the default name is `"E_INV_<auftrnr>_<subnr>_<vorgang>.xml"`.
For credit notes, the default name is `"E_CRN_<auftrnr>_<subnr>_<vorgang>.xml"`.

If the SP "`cu_get_e_invoice_name`" does not exist and the XRechnung is not generated as attachment (document attachment), a default name is used, which is specified by the AWE B2B Service.
The default name has the following structure: `"e_inv_<kunr>_<auftrnr>_<timestamp>.xml"`
"e_inv" stands here as abbreviation for "electronic invoice".

**Note about the ZUGFeRD format:**
When using the ZUGFeRD format, the same rules apply for the file embedded in the PDF the same rules apply for the file name as for the XRechnung format.

**E-invoice document as attachment (document attachment)**
The generated e-invoice is saved by default as attachment (document attachment) of the AWE invoice.
The O/L field indicates whether this is an original document or a link.
For e-invoices, an "R" for reserved is displayed if the B2B Service has not yet generated the XML document for the e-invoice or could not generate it.

If a storage as attachment (document attachment) is not desired, the logic can be suppressed by activating the environment variable `EINVOICE_NO_REFDAT`.
The file path for saving as attachment (document attachment) is defined by the environment variable `DATEI_REF_PFAD` (can be configured client-specifically) and the invoice number.
The complete path is: `<DATEI_REF_PFAD>\<Mandantennummer>\<Rechnungsnummer>\0`
The "0" stands for a file attachment (document attachment) that is not assigned to an individual item, but rather to the invoice generally.

**Write protection of the XML file**
The generated xml file is write-protected.
That is, the "write-protected" attribute is active in the file properties. When copying within the file system, the write protection is retained.
In particular, write protection is also retained during archiving (storage of a copy of the xml file in the archive) if the archive is in the same file system.
If the xml file is sent via e-mail as an attachment, the write protection remains active if the attachment is opened directly (without saving).
As soon as the xml file is saved by the e-mail recipient, the file loses the write protection from the source system.

**XRechnung document as independent file (no attachment/document attachment)**
If the environment variable `EINVOICE_NO_REFDAT` is active or for another reason the file name of the file to be generated is not found in the database (`kaufref.datei`) by the B2B service at the time or processing, the generated file is saved according to the configuration (path) in the config tool of the B2B service.
Then, no attachment (document attachment) is generated for the invoice.
The file name (`kaufref.datei`) could be missing, for example, if a manual generation of the e-invoice is executed (manual insert into the table `ottransfer`).

**File handling and file name with new generation of the file**
If an e-invoice file is repeated for an invoice, the old files are retained in the file path.
If the name of the new file matches the name of the old file, the current time stamp is added to the name of the old file and the extension "old" is added.

#### 8.14.5. Determination of e-mail addresses

**Determination of the valid record from the market partner e-mail addresses**
The e-mail address of seller and buyer are transferred into the XRechnung. (Element "EndpointID").
The e-mail address for sender and recipient is drawn from the e-mail master data of the invoice recipient (table `xemail`).

**SP "rpgeteinvemailaddress"**
To guarantee that the e-mail addresses determined by the B2B Service match the sender and recipient e-mail address that will be used later during form dispatch in A+W Enterprise, the SP "rpgeteinvemailaddress" is provided. The SP is called for determination of the e-mail addresses both in the AWE B2B Service as well as in the AWE form dispatch.
**Declaration:**
`rpgeteinvemailaddress(p_auftrnr int, p_vorgang smallint)
returning char(80) as email, char(80) as emailabs, char(80) as cc, char(80) as bcc;`

If necessary, the SP can be adapted individually by the customer. In the version delivered by A+W, the SP includes the "xemail logic" described below for determination of the e-mail addresses.
If the SP does not exist, the "xemail logic" described below is also used to determine the e-mail addresses in the B2B Service.
In the form dispatch, the default logic is used. Here there can be differences between the sender stored in the e-invoice and recipient e-mail address and the e-mail address used in the form dispatch.

**xemail logic**
The record relevant for this from the e-mail addresses of the invoice recipient (`kauf.kunr` -> `xemail.mpnr`) is determined in that the e-mail addresses (table `xemail`) are searched for with employee = 0 (`xemail.manr`) and department = 0 (`xemail.abtnr`) according to a data record for the special form type.
For an invoice, the form type that is stored in the env variable `EINV_FORMART_RECH` counts.
For a credit note, the form type that is stored in the env variable `EINV_FORMART_GUTS` counts.
If a record is found with these search criteria, it is valid.
For the e-invoice, the record is only valid if employee `manr`= 0 AND department `abtnr` = 0. Records with entered employee or department will not be considered.
If no record was found for the defined form type, it is checked whether a record for the form type "0" exists. The same check logic is run through as described above.
In a multisite system, the site number is also considered. First a valid data record for the current company is searched for. If there is none, there is a search for a general record with site number "0".

> **Caution:** If in the xemail record found, a sender address (`xemail.emailabs`) is stored, this is used. If no sender address is stored, the e-mail address master data of the legal seller is used.

#### 8.14.6. Text
The texts are taken over into the e-invoice in the language of the invoice (`kauf.sprkz`).
The general/item-spanning texts are stored in BT-22.
The item and article-specific texts are stored in BT-127.
Master data texts that are not available in the language of the invoice are written in the default language (English) into the e-invoice.
The form vector is evaluated for all texts.
Note: The document texts are already available in the correct language (language of the invoice) in the table `auftxt`.

**Tabular display of all texts that are taken over into the e-invoice**

| Processing name | Table reference | Comment |
| :--- | :--- | :--- |
| Header texts and footer texts (manual, automatic and configured) | `kauf.auftxt=auftxt.txt` -> `auftxt.txt` | Document-related text<br>`auftxt.drupos=1` (header text)<br>`auftxt.drupos=2` (footer text)<br>`auftxt.generiert=0` (manual)<br>`auftxt.generiert=1` (automatic)<br>`auftxt.generiert=3` (configured) |
| Item header texts (manual, automatic and configured) | `kpos.poskotxtnr=auftxt.txtnr` -> `auftxt.txt` | Item-related text<br>`auftxt.drupos=3` (before item)<br>`auftxt.drupos=4` (after item)<br>`auftxt.generiert=0` (manual)<br>`auftxt.generiert=1` (automatic)<br>`auftxt.generiert=3` (configured) |
| Item article/item processing texts | `kpos.arttxtnr=auftxt.txtnr` -> `auftxt.txt` | Article-related text<br>`auftxt.drupos=3` (before item)<br>`auftxt.drupos=4` (after item)<br>`auftxt.generiert=-1` (automatic, tuple-related)<br>`auftxt.generiert=-2` (configured, tuple-related) |
| Current texts | `akttxt.verfalldat` > "Current date" | Header and footer texts (`akttxt.drupos` 0 / 1)<br>Client-spanning and client-specific texts (`akttxt.hausnr` 0 / `kauf.hausnr`). |
| Group texts | `kauf.kunr=grpzu.kulinr` -> `grpzu.grpnr=grptxt.grpnr` -> `grptxt.datei/pfad` = `xtxtnr.datei/pfad` -> `xtxtnr.txtnr` = `stammtxt.txtnr` -> `stammtxt.stammtxt` | Header and footer texts (`grptxt.drupos` 0 / 1)<br>Client-spanning and client-specific texts (`akttxt.hausnr` 0 / `kauf.hausnr`). |
| Project texts | `kauf.objnr=objtxtzu.objnr` -> `objtxtzu.datei/pfad` = `xtxtnr.datei/pfad` -> `xtxtnr.txtnr` = `stammtxt.txtnr` -> `stammtxt.stammtxt` | Header and footer texts (`objtxtzu.drupos` 0 / 1)<br>Customer-spanning and customer-specific texts (`objtxtzu.kunr` 0 / `kauf.kunr`). |
| Market partner texts | `kauf.kunr=txtzu.kulinr` -> `txtzu.datei/pfad` = `xtxtnr.datei/pfad` -> `xtxtnr.txtnr` = `stammtxt.txtnr` -> `stammtxt.stammtxt` | Header and footer texts (`txtzu.drupos` 0 / 1) |
| Product group texts | `kpos.wagrp=wargrptxt.wgrnr` -> `wargrptxt.datei/pfad` = `xtxtnr.datei/pfad` -> `xtxtnr.txtnr` = `stammtxt.txtnr` -> `stammtxt.stammtxt` | Client-spanning and client-specific texts (`wargrptxt.hausnr` 0 / `kauf.hausnr`). |
| Article texts (master data) | `kpos.artnr = artxtzu.artnr` -> `artxtzu.datei/pfad` = `xtxtnr.datei/pfad` -> `xtxtnr.txtnr` = `stammtxt.txtnr` -> `stammtxt.stammtxt` | |
| Customer-specific article texts | `kpos.artnr = artxtzu.artnr` & `kauf.kunr=artxtzu.kunr` -> `artxtzu.datei/pfad` = `xtxtnr.datei/pfad` -> `xtxtnr.txtnr` = `stammtxt.txtnr` -> `stammtxt.stammtxt` | |
| Project-specific article texts | `kpos.artnr = artxtzu.artnr` & `kauf.objnr =artxtzu.objnr` -> `artxtzu.datei/pfad` = `xtxtnr.datei/pfad` -> `xtxtnr.txtnr` = `stammtxt.txtnr` -> `stammtxt.stammtxt` | |

**Sequence of the general/item-spanning invoice texts in the e-invoice**
Within the text type, the sequence is specified by the sequential number (`<tab>.lfdnr`).

| No. | Processing name |
| :--- | :--- |
| 1 | Manual document header texts |
| 2 | Automatic header texts |
| 3 | Configured document header texts |
| 4 | Manual document footer texts |
| 5 | Automatic document footer texts |
| 6 | Configured document footer texts |
| 7 | Customer-specific project header texts |
| 8 | Customer-specific project footer texts |
| 9 | Customer-spanning project header texts |
| 10 | Customer-spanning project footer texts |
| 11 | Customer header texts |
| 12 | Customer footer texts |
| 13 | Client-specific group header texts |
| 14 | Client-specific group footer texts |
| 15 | Client-spanning group header texts |
| 16 | Client-spanning group footer texts |
| 17 | Client-specific current header texts |
| 18 | Client-specific current footer texts |
| 19 | Client-spanning current header texts |
| 20 | Client-spanning current footer texts |

**Sequence of the item-specific invoice texts in the e-invoice**
Within the text type, the sequence is specified by the sequential number (`<tab>.lfdnr`).

| No. | Processing name |
| :--- | :--- |
| 1 | Article texts, before item, automatic, header tuple |
| 2 | Article texts, before item, configured, header tuple |
| 3 | Article texts, before item, manual |
| 4 | Article texts, before item, automatic |
| 5 | Article texts, before item, configured |
| 6 | Article texts, before item, automatic, tuple-specific, but not header tuple |
| 7 | Article texts, before item, configured, tuple-specific, but not header tuple |
| 8 | Article texts, after item, automatic, header tuple |
| 9 | Article texts, after item, configured, header tuple |
| 10 | Article texts, after item, manual |
| 11 | Article texts, after item, automatic |
| 12 | Article texts, after item, configured |
| 13 | Article texts, after item, automatic, tuple-specific, but not header tuple |
| 14 | Article texts, after item, configured, tuple-specific, but not header tuple |
| 15 | Item header texts |
| 16 | Article master data texts, project-specific |
| 17 | Article master data texts, customer-specific |
| 18 | Article master data texts, general |
| 19 | Product group texts |

#### 8.14.7. Surcharges and discounts
To be able to handle surcharges/discounts, the new discount logic must be active (`RABATTLOGIK_2005` = ON).
All surcharges/discounts are identified in the XRechnung as order surcharges/discounts.
There are no surcharges/discounts on the item level, completely regardless of whether the surcharges/discounts in A+W Enterprise are created as redistributed or non-redistributed surcharges/discounts.

**General reductions and surcharges**
General reductions and surcharges, such as due to zero invoice, for example, due to minimum order value or manually-entered amounts, are saved in the table fields `kauf.gesrab` and `kauf._sonderrab`. These amounts also cause a surcharge/reduction in the e-invoice.
These general surcharges/reductions are described in the "Enterprise" configuration instructions.

#### 8.14.8. Invoice amounts in foreign currency
To determine the currency of the XRechnung, the print option (field: "Print in") of the AWE invoice is evaluated. The options available for selection in the invoice and in the customer master data are from the time when the Euro was introduced as currency. The print options are:
- 0: kalkulierte Währung (calculated currency)
- 1: Fremdwährung im Fuß (foreign currency in footer)
- 2: Fremdwährung in Pos. und Fuß (foreign currency in item and footer)
- 3: kalk. Währung+Euro im Fuß (calc. currency + Euro in footer)
- 4: kalk. Währung+Euro in Pos. und Fuß (calc. currency + Euro in item and footer)
- 5: Fremdwährung+Euro im Fuß (foreign currency + Euro in footer)
- 6: Fremdwährung+Euro in Pos. und Fuß (foreign currency + Euro in item and footer)

The XRechnung can contain precisely one currency. This is either the calculated currency (= own currency) or the foreign currency.
- For option 0, 3, 4, the XRechnung is created in calculated currency (= own currency).
- For option 1, 2, 5, 6, the XRechnung is created in foreign currency.

For calculation in own currency and printout in foreign currency, a currency conversion within the B2B service is required. With conversion with the conversion rate stored in the invoice (`kauf._kurs`), there can be rounding differences.

Rounding difference > 1 currency unit are not tolerated. The XRechnung will not be generated. An e-mail will be sent, which informs about the error. The transfer record remains with an error status in the table `ottransfer`.
Rounding difference <= 1 currency unit are balanced out.
The correction is made according to the following hierarchy:
- First in the last general surcharge (if present)
- then in the last general discount (if present)
- then in the last item

If a rounding correction across surcharges/discounts or items is not possible, an "AllowanceCharge" element (discount/surcharge element) is generated in the last item with the rounding difference amount.

#### 8.14.9. Credit notes
The generating and sending of e-credits is possible with use of the QR[2503].
Credit notes are currently (as of 04/16/2025) exported as negative invoices.
The amounts in the invoice contain a negative leading sign.
Excepted from this are the net prices of the item basic quantity; its amount remains positive. Instead, the item quantities are transferred as negative values.

#### 8.14.10. Deposit invoice / final invoice

**Deposit invoice**
In the deposit invoice, the deposit amount is indicated in an invoice item.

**Final invoice**
In the final invoice, the deposit amounts are indicated from the associated deposit invoices as discount items.

**Note about data in A+W Enterprise**
- A deposit invoice is identified with `kauf.eingang` = 12.
- A final invoice is marked with `kauf.eingang` = 13.
- Deposit invoices and final invoice that belong together have the same order reference in `kauf.referenz`.
- In the final invoices, the partial payments made are stored as discount records. The article number of the partial payment article is stored in a partial payment record.
- A partial payment article is defined by the `article.atyp` 995.

#### 8.14.11. Validation of the e-invoice
Before the e-invoice counts as "successfully created", the B2B Service conducts a validation of the file created.
Checked here are:
- The use of the correct syntax schema
- Adherence to the rules for the standard EN 16931
- In the case of XRechnung and ZUGFeRD: Adherence to the XRechnung rules

**Possible validation errors and how to eliminate them**

| Rule | Error description | Troubleshooting |
| :--- | :--- | :--- |
| BR-DE-1 | An invoice (INVOICE) must include details about "PAYMENT INSTRUCTIONS" (BG-16). | In the master data for the supplier/seller (invoice sender, `xhaus.linr`) or the creditor, valid bank details must be stored. |
| BR-DE-16 | If in an invoice the tax codes S, Z, E, AE, K, G, L or M are used, at least one of the elements "Seller VAT identifier" (BT-31), "Seller tax registration identifier" (BT-32) or "SELLER TAX REPRESENTATIVE PARTY" (BG-11) must be transmitted. | In the master data for the supplier/seller, the VAT number must be stored. |
| PEPPOL-EN16931-R020 | Seller electronic address MUST be provided | In the master data for the supplier/seller or the creditor, an e-mail address must be stored. |
| PEPPOL-EN16931-R010 | Buyer electronic address MUST be provided | In the master data of the recipient/buyer, an e-mail address must be stored. |

#### 8.14.12. Error handling
If during generation or validation of the e-invoice there is an error, a corresponding info e-mail is sent.
If during validation of the e-invoice an error occurs, the generated xml file is also saved for research purposes.
The storage is done in the path that is stored in the Config Tool of the B2B Service as export path. Therefore, it is important that this path also be configured if the export works with file attachments.
The B2B service must be able to reach the directory and have write access rights to it.
The name of the xml error file contains a time stamp and the extention "failure".
Path and name of the xml error file are specified in the info e-mail.

**Special case: invoices with kauf.still < 0**
Invoices/credits count as complete and unlocked if the still code is populated with the value "0". Kauf.still Werte < "0" indicate that an invoice/credit is still being processed by background processes.
The B2B Service checks whether an invoice is still locked with the still code. Invoices/credits with `kauf.still` < "0" will be placed back in the table ottransfer with the control flag "302". After expiry of the next polling interval, the still code will be checked again. If the kauf record has the correct still code ("0"), the invoice/credit will be processed.

#### 8.14.13. Cleanup logic
Saved research files (see "Error handling" chapter) will be deleted according to the clean-up logic when the configured clean-up time has been reached.
See also general chapter "Clean-up logic".

#### 8.14.14. Restrictions
- The XRechnung does not include a signature.
- No advertising may be placed in the XRechnung.
- There is no end-to-end encryption of the electronic invoice when sending via e-mail.
- Current status
  - This is (as of 07/16/2024) the first version of the XRechnung export made available by A+W Enterprise. There has not yet been a pilot phase, which is why the release of the version is being done with reservations. The official release will only be made after a successful pilot. The following functions are not yet included in this version, but are planned for the following version:
    - Export of collective invoices
  - The following function is not included and is also not planned:
    - Export of file attachments (e.g., declaration of performance, production sketches, etc.)

### 8.15. Data mapping
For the description of the data mapping, there are special Excel documents.

#### 8.15.1. UBL
Description of the UBL elements from:
[https://docs.peppol.eu/poacc/billing/3.0/2023-Q4/syntax/ubl-invoice](https://docs.peppol.eu/poacc/billing/3.0/2023-Q4/syntax/ubl-invoice).

Description "business term" of:
[https://xeinkauf.de/xrechnung/versionen-und-bundles/](https://xeinkauf.de/xrechnung/versionen-und-bundles/)
-> Bundle XRechnung 3.0.2

Data-Mapping Excel-Sheet:
[https://awsoftwaregmbh.sharepoint.com/:x:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/XRechnung_UBL_AWE_DataMapping.xlsx?d=wf72f02fd93e643a89874003b1618aff3&csf=1&web=1&e=BS2leO](https://awsoftwaregmbh.sharepoint.com/:x:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/XRechnung_UBL_AWE_DataMapping.xlsx?d=wf72f02fd93e643a89874003b1618aff3&csf=1&web=1&e=BS2leO)

There is a single version-spanning data mapping description. The description refers to the highest implemented version of the xml format (currently Version UBL 2.3). If xml elements do not exist in older versions or are not filled, the data mapping includes a corresponding note.

#### 8.15.2. CII
[SVH 05.02.2025 - being edited]
Description of the CII elements and "business term" of:
[https://www.ferd-net.de/publikationen-produkte/publikationen/detailseite/zugferd-232-deutsch](https://www.ferd-net.de/publikationen-produkte/publikationen/detailseite/zugferd-232-deutsch)

### 8.16. Specific data description

#### 8.16.1. Legal seller
In the XRechnung, details about the seller must be stored, which identify him as the legal bearer or legal person.
These details must be stored in A+W Enterprise in the market partner master data. The supplier (`xhaus.linr`) stored as market partner in the table xhaus for this site is used.
The supplier can be defined precisely to the sub-site here.
For the supplier, a different FinAc creditor (`mp.stddebnr`) can be defined.
It is possible that the market partner number stored in the `xhaus.linr` has a negative value. This is legitimate. The negative value indicates that no internal EDI is configured for this supplier.
For this processing in the B2B service, the market partner number is most crucial. The leading sign does not matter.

**FinAc creditor**
If in the market partner master data of the legal buyer (xhaus-Lieferanten) a different FinAc creditor (`mp.stddebnr`) is defined, then -- instead of the supplier's details -- the creditor's details will be used in the e-invoice.

**Basic additions to the table xhaus:**
In A+W Enterprise, a site installation with regard to other sites and external business partners can occur depending on the business process either as buyer/recipient or seller/supplier. For this reason, each site is assigned a customer market partner number (`xhaus.kunr`) and a supplier market part number (`xhaus.linr`) via the table `xhaus`. (see "EN-CONFIG-A+W Enterprise EDI")
In business processes in which the site appears as customer (buyer/recipient), the customer master data is used (`xhaus.kunr`).
In business processes in which the site appears as seller/supplier, the supplier master data is used (`xhaus.linr`).
In the business process of invoice creation, the site is the seller/supplier, therefore the supplier (`xhaus.linr`) stored in `xhaus` is decisive for determining the master data.
The customer data (buyer/recipient) is not determined via the table `xhaus`, but always via the customer number of the invoice.

#### 8.16.2. Buyer reference / route ID (BT-10)
General designation: "buyer reference".
The term "route ID" is only used in Germany.
To be able to address an electronic invoice through the invoicer or recipient, the invoice recipient must be identified uniquely and addressable.
The route ID enables an electronic addressing and forwarding of the e-invoice to the central invoice receipt platform of the German Federal government to the connected ERP or release systems of the authorities and facilities of the German Federal administration.
The route ID is specified in the standard XRechnung in the "Käuferreferenz" field (BT-10) and must be transmitted as a mandatory detail on every e-invoice.
(From https://www.e-rechnung-bund.de/faq/leitweg-id/.)

If the invoice recipient does not have a route ID because it is not an authority, the field is filled with the A+W Enterprise customer number.
If the field would remain empty, there would be an error in validating the document.

**Structure of the route ID:**
The route ID (Leitweg-ID) consists of three parts:
- **Grobadressierung (Coarse addressing):** Up to 12 digits.
- **Feinadressierung (Fine addressing):** Max 30 digits (optional).
- **Prüfziffer (Check digit):** 2 digits.

Example: `04 0 11 000 - 1234512345 - 06`
(From https://www.xoev.de/sixcms/media.php/13/Leitweg-ID-Formatspezifikation-v2-0-2.pdf)

The assignment of the route IDs is also regulated by federal state and countries:
- For public customers connected to state authorities and on the federal level, the central finance department of the federal government (ZFB) is responsible.
- The issuing offices for country authorities can be looked up here: [https://www.e-rechnung-bund.de/e-rechnung/umsetzung-der-e-rechnung-in-den-bundeslaendern](https://www.e-rechnung-bund.de/e-rechnung/umsetzung-der-e-rechnung-in-den-bundeslaendern)

#### 8.16.3. Buyer electronic address (BT-49)
"buyer electronic address" ("EndpointID" of the buyer) specifies the electronic address of the buyer to which the invoice is sent. The entry is mandatory.
The recipient e-mail address is taken over from the buyer's master data.
There must be a valid e-mail address record for the invoice recipient (see section "Determination of the valid record from the market partner e-mail addresses") and the recipient e-mail address (`xemail.email`) must be stored there.

#### 8.16.4. Seller electronic address (BT-34)
"seller electronic address" ("EndpointID" of the seller) specifies the seller's electronic address to which the response of the response level to an invoice can be sent. The entry is mandatory.
The sender e-mail address is taken over from the legal seller (Client number -> `xhaus.linr` -> `mpemail`).
If, however, there is a valid e-mail address record for the invoice recipient (see paragraph "Determination of the valid record from the market partner e-mail addresses") and if a sender e-mail address (`xemail.emailabs`) is stored in this record, then this sender e-mail address takes precedence over the master data of the legal seller.

#### 8.16.5. Seller additional legal information (BT-33)
Information about the management and the chair of the supervisory board is stored in this field.
In AWE, the designations of the items used at the company are stored in Master Data > Keys > Item.
To identify the manager and the chair of the supervisory board, in the "leading position" field, it is possible to select the appropriate toggle value.
In the next step, it is possible to create the management and chair of the supervisory board as "Contact Person" for the legal seller (that is the market partner who is stored in the table `xhaus` under the respective site number as supplier (`xhaus.linr`)).
The identification as "Manager" is done by entering the position defined as "Manager" in "Position".
The management can consist of several people. In this case, the "List sequence" field specifies the order in which the people are named on the e-invoice.
The identification as "Supervisory board chair" is done by entering the position defined as "Chair of the supervisory board" in "Position".
There is always only one chair of the supervisory board. Multiple designations are not possible.

#### 8.16.6. Payment terms (BT-20)
A text description of the payment terms that apply for the payment amount due (including description of possible cash discount conditions). This information element can include several lines and several specifications of payment terms and both unstructured and structured text. The unstructured text may not contain a `#`.
If information about the granting of cash discounts is specified, it will be displayed as follows: To be specified in the first segment is "SKONTO", in the second "TAGE=n", in the third "PROZENT=n". Percentages must be specified without leading sign and separated from places after the decimal point by a dot. If the amount to be calculated is not based on "Amount due for payment" (BT-115) but is only part of the invoice amount due, the basic value for calculation of cash discount must be specified as fourth segment "BASICBETRAG=n" according to the semantic data types amount.
Each entry begins with a `#`, the segments are separated with a `#`, and a line concludes with a `#`. At the end of a complete cash discount specification, there must be an XML-compliant line break.
Examples with three segments per line:
`#SKONTO#TAGE=14#PROZENT=2.25#`
`#SKONTO#TAGE=28#PROZENT=1.00#`

Examples with four segments per line (the granting of cash discount refers only to a partial amount of the invoice (e.g., material) and the basic value for calculation of the cash discount must also be specified):
`#SKONTO#TAGE=14#PROZENT=2.25#BASISBETRAG=357.93#`
`#SKONTO#TAGE=28#PROZENT=1.00#BASISBETRAG=357.93#`

All details for granting cash discounts must be made in capital letters. Additional whitespace (empty space, tabs or line breaks) is not permissible. Other characters or texts than in the examples above are not permissible.

#### 8.16.7. Legal information about the seller (BT-33)
Here, details about the management and the headquarters of the supervisory board are supplied.
The names are specified via the people marked in "Company position".
At the start is a text that designates the position.
In the highest priority, the designation is used that is stored in the company positions (master data). If no text is found there, corresponding report texts are used:

| Type | A+W Text German |
| :--- | :--- |
| cr_xr_ceo | Management |
| cr_xr_cosb | Headquarters of the Supervisory Board |

#### 8.16.8. Address addition of the customer (BT-163)
The following report text is used for the address addition:

| Type | A+W Text German |
| :--- | :--- |
| cr_postbox | P.O. box |

#### 8.16.1. Texts on header level (BT-22)
See "Configurable texts" and "Texts" chapters.

#### 8.16.2. Texts on item level (BT-127)
For the labels on item level, the following report texts are used:

| Type | A+W Text German |
| :--- | :--- |
| cr_custit | Reference |
| cr_xr_shape | Shape number |

For a detailed description, see "Report texts" chapter.

#### 8.16.3. Legal company name
To enter the legal company name of a market partner, the field "Company name" is available in the market partner master data on the "Identification" dialog.
If the field is filled, the content is used to specify the name of the sender and recipient of the XRechnung.
If it is not filled, "First name" and "Last name" from the market partner master data are used.
See PF [AW-172502].

#### 8.16.4. Delivery address
The delivery address is only filled if it deviates from the invoice address.
Compared are the following details of the address:
- "Attn."
- "Addition"
- "Street"
- "PCd, POB"
- "POB City"
- "PCd, City"
- "Country"

If at least one of the details in the invoice and delivery address is different, the entire delivery address is filled into the XRechnung.

#### 8.16.5. Telephone number of the supplier contact
An employee's extension can be stored in the employee master data (`mitarb.durchw`). Here, it is not necessary to supply the complete telephone number.
To be able to transfer the complete telephone number in the XRechnung document, the basic telephone number must be stored in the master data of the legal seller (`mp.telefon`).
A stored telephone number must correspond to the guidelines of DIN 5008 so that it is interpreted correctly by the program.
See also https://de.wikipedia.org/wiki/Rufnummer

> In Deutschland ist die DIN 5008 maßgeblich, nationale Rufnummern werden folgendermaßen dargestellt:
> **Schreibweise:** `030 12345-67`
> **DIN 5008:** Funktionale Gliederung mit Leerzeichen. Durchwahl mit Bindestrich.

If in the employee master data only the extension is specified, the complete telephone number of the employee is determined in that the basic telephone number from the legal seller is selected and the extension attached with "-" (hyphen).

**Example 1**
Telephone number of the legal seller: 0123 456789
Employee extension: 77
=> Complete employee telephone number: 0123 456789-77

**Example 2**
Telephone number of the legal seller: 0123 456789-224
Employee extension: 77
=> Complete employee telephone number: 0123 456789-77

**Example 3**
Telephone number of the legal seller: 0123 456789-224
Employee extension: 0456 123456-77
=> Complete employee telephone number: 0456 123456-77

**Example 4**
Telephone number of the legal seller: 0123 456789-224
Employee extension: 0456 123456
=> Complete employee telephone number: 0456 123456

**Example 5**
Telephone number of the legal seller: 0123 456789-224
Employee extension: 2233
=> Complete employee telephone number: 0123 456789-2233

**Example 6**
Telephone number of the legal seller: 0123 456789-224
Employee extension: 22 33
=> Complete employee telephone number: 22 33

#### 8.16.6. Item dimensions (BT-160/BT-161)
The following item dimensions are taken over as "properties" of the item in the XRechnung.

| Name | AWE DB field |
| :--- | :--- |
| Width | `kpos.laenge` |
| Height | `kpos.breite` |
| AIR1 | `kpos.szr` |
| AIR2 | `kposp.szr2` |
| Thickness | `ktechw.dicke` |

For the names, the following report texts are used:

| Type | A+W Text German |
| :--- | :--- |
| cr_width | Breite |
| cr_height | Höhe |
| cr_cav | SZR |
| cr_thickness | Dicke |

### 8.17. E-mail addresses in the e-invoice
The generation and sending of e-invoices in A+W Enterprise is done in two different processes, which are uncoupled from one another.
The generation of the e-invoice (creation of the xml file) will be done by the AWE B2B Service.
Sending the e-invoice will be done in A+W Enterprise via the "Sales > Forms > E-mail/fax" menu and then handled by the AWE Print Service.

**Generation of the e-invoice**
The XRechnung is the special format of the e-invoice in Germany.
In the XRechnung, the sender e-mail address and the recipient e-mail address are stored as "EndpointID".
- The "EndpointID" of the seller ("seller electronic address") is in element BT-34.
- The "Endpoint ID" of the buyer ("buyer electronic address") is in element BT-49.

For both of these elements, it is described in the configuration instructions for the B2B Service how the corresponding data is determined.
The "EndpointID" of the seller ("seller electronic address") is taken over from the legal seller (Client number-> `xhaus.linr` -> `mp.email`).
If, however, there is a valid e-mail address record for the invoice recipient (see paragraph "Determination of the valid record from the market partner e-mail addresses") and if a sender e-mail address (`xemail.emailabs`) is stored in this record, then this sender e-mail address takes precedence over the master data of the legal seller.

The "EndpointID" of the buyer ("buyer electronic address") is also taken over from the buyer's master data.
There must be a valid e-mail address record for the invoice recipient (see section "Determination of the valid record from the market partner e-mail addresses") and the recipient e-mail address (`xemail.email`) must be stored there.

**Sending the e-invoice**
If via the "Sales > Forms > E-mail/fax" menu the sending of an e-invoice is triggered, here the entries for the "EndpointID" in XRechnung (file) are not known. The sender e-mail address and recipient e-mail address here are currently determined via a generally applicable, multi-stage logic.
In this logic, for the sender e-mail address the legal seller (Client number -> `xhaus.linr`) is currently NOT considered.
The consequence of this is that the correct sender e-mail address can only be ensured in that an e-mail address record is created for the buyer in the master data that is valid for the form, and there the desired sender e-mail address is entered under "E-mail from".
As of 04/24/2025, an update will be made available soon in which the logic is adjusted when triggering the e-mail dispatch. In the future, it will call the SP "`rpgeteinvemailaddress`" in order to determine the e-mail addresses. With this SP, it is ensured that the same e-mail logic is used in the B2B Service and in the form dispatch.

### 8.18. Manual generation of e-invoices
Due to a manual insert into the table ottranser or an update of the error flag, an invoice can be presented to the B2B Service to create the e-invoice.
The manual insert/update should only be done by A+W Enterprise Support.
A detailed description of how to execute the insert/update is in the "Enterprise System" configuration guide.

#### 8.18.1. CMD script „xrechnungexport“
> **Caution: This logic should no longer be used!**
> The logic served test purposes in the initial stage of the implementation, when the generation of the e-invoice could not yet be configured in A+W Enterprise.
> To generate an XRechnung for an AWE invoice/credit manually, the cmd script "xrechnungexport" was stored as an individual program.
> This script should no longer be used since it can cause flawed program behavior.

### 8.19. Sending the E-invoice via e-mail
For dispatch of the XRechnung, no special authorization is required. Users that are generally authorized to dispatch invoices can also send XRechnung.
A detailed documentation of the dispatch of XRechnung is in "EN-CONFIG-A+W Enterprise Print Service".

#### 8.19.1. Data security
In the A+W Enterprise Print Service, it is possible to activate SSL encryption for e-mail sending. See also the installation instructions for the Print Service.
The customer is responsible for the required SSL certificate(s).
There is no end-to-end encryption of the electronic invoice when sending via e-mail.

### 8.20. Archiving the e-invoice
A detailed documentation of the archiving of XRechnung is in "EN-CONFIG-A+W Enterprise Print Service".
Note: Even after the archiving, the e-invoice document (xml file) remains as a file attachment in the data attachment directory (`DATEI_REF_PFAD`).

### 8.21. Creation and archiving of the XRechnung via ZUGFeRD PDF file.
A detailed documentation of the creation and archiving of XRechnung in a ZUGFeRD PDF file is in "EN-CONFIG-A+W Enterprise Print Service".

### 8.22. Troubleshooting

#### 8.22.1. Sending the e-invoice - PDF is sent, but not configured
Check whether at least QR[2410] is active.
Furthermore, 2 sql scripts must be executed, which are first executed automatically with QR[2503].
`130004273_printparamok.sql`
`130004268_printparam.sql`

#### 8.22.2. E-invoice (file) is missing when sending
The generation of the e-invoice (file) will be done by the AWE B2B Service in an asynchronous process during invoice booking.
It can happen that the user triggers the sending of the e-invoice although the e-invoice (file) was not yet generated or there was an error during the generation/validation.
When triggering sending in the form dispatch, there is no check whether the e-invoice file exists. Therefore, there is also no warning message if the file is missing. Only the print service encounters an error when printing.
The user can make sure before triggering dispatch of the e-invoice that the file exists by checking the status of the file attachment in "Document type assignment".
For e-invoices, in the "O/L" field, an "R" for reserved is displayed if the B2B Service has not yet generated the XML document for the e-invoice or could not generate it.

## 9. E-mail notification in case of error (AWDesk #407285)
With Version 6.4.1792, the functionality for sending an e-mail is provided. An info e-mail is sent if the export of a document fails.
The e-mail includes the affected process number as well as a description of the error that has occurred.
The e-mail recipient is configured using the config tool (see installation description).
> **Attention:**
> In the B2B Service, currently NO placeholder for site numbers ("$SITES$") can be specified in the e-mail addresses. This logic existed previously only in the FinAc Service.

## 10. Cleanup logic
The logic for cleansing/clean-up of the tables `ottransfer` and `ottransferok` was expanded.
With the Config tool, it is possible to store the number of days for which the records with error status in the transfer table `ottransfer` or successfully processed records in the archive table `ottransferok` should be kept. If the period has elapsed, the records are deleted.
The default retention time for successfully processed records in the table `ottransferok` is 100 days. The value from `ottransferok.uzeit` is used as reference time.
The default retention time for faulty records in the table `ottransfer` is 200 days. The value from `ottransfer.filltime` is used as reference time.
A configuration of "0" days is possible in the Config tool, but it is intercepted by the program. In this case, the records are deleted after 365 days.
It is not recommended that you set the retention time for faulty records to a value < 30 (days). The records may be required for any error research or should under some circumstances be reset and be presented again for processing.
See PF [AW-155564].

## 11. Troubleshooting

### 11.1. There is no entry in the table ottransfer
- Check whether the `alcib` binfile is current.
- Check configuration in `mpdfuectrl`.
- Check whether the printer configuration permits the printing -> see chapter "Triggering the document generation."

### 11.2. "object reference not set"-Exception in GetAnsprData()
Supplier of the current site from `xhaus` is not stored in the mp master data.
See AWDesk #406571.

### 11.3. Error "no lapool data" or quantities missing in the dispatch notification document
- Check whether the trigger record in `ottransfer` includes the correct data in `ltplan` and `routenr`.
- Check version of the B2B service. With AWDesk #437472, the logic was changed so that the dispatch notification document can also be generated if there is already a delivery note; that is, `lapool` records with `subnr` > 0 are also found.

### 11.4. Error during select on lapool (only Version ALCIB 2008 (4.2))
The DB field `lapool.private_long1` has to be added to the table `lapool` by hand.

### 11.5. Exception due to DBNull value
DBNull values in the market partner/address data cause exceptions.
The following DB fields may not contain any DBNull values:

**Table mp**
- vname
- branche
- str
- plz
- ort
- kfzcode
- telefon
- faxnr
- email
- website

**Table adr**
- adrvname
- branche
- str
- plz
- ort
- kfzcode
- telefon
- faxnr
- email

See also PF [AW-157970].
For the first name, the source code was adjusted, DBNull values are tolerated there, but should nevertheless be eliminated if possible.

### 11.6. openTRANS Invoice – empty document
If the env variables `OPENTRANS_CMLINVOICE` and `OPENTRANS_XMLCREDITNOTE` are active, the openTRANS files are generated with the "old logic" (via the ERP Webservice). This "old logic" is no longer under maintenance and must be replaced by the "new logic" (described in this document).
In particular, for a market partner for which an openTRANS invoice/credit should be exported, the flag "Invoice transfer" (`mp.rechdfuekz`) must be deactivated in the master.
If the "internal calculation" logic is not required, the env variables `OPENTRANS_XMLINVOICE` and `OPENTRANS_XMLCREDITNOTE` should be deactivated.
See PF [AW-213600].

### 11.7. Temporary database problems/network problems/Informix error
If database/network/Informix errors occur that are so severe that they cause an automatic ending of the B2B service, you can try to stabilize the service by configuring an automatic restart of the B2B service.
See chapter "B2B – automatic restart after abort due to error".
See also PF [AW-210525] + [AW-214065].

### 11.8. Interruption of the B2B service without error message in the log
Check in the Event Viewer whether there are indications about the cause of the interruption.
Under some circumstances, the virus scanner can be responsible for this.

### 11.9. B2B Service aborts due to error, but does not restart
The B2B Service can only conduct an automatic restart if the service is configured appropriately in the manager. See chapter "B2B – automatic restart after abort due to error".
If the restart does not happen despite correct configuration, the "Event display" must be checked. Are there notes there why the restart was prevented?
With correct configuration of the restart, the following (similar) message is in the "Event display":
> **Event 7031, Service Control Manager**
> The A+W Enterprise 6 B2B service terminated unexpectedly. It has done this 1 time(s). The following corrective action will be taken in 60000 milliseconds: Restart the service.
