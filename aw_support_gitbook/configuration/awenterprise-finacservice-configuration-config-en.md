---
title: "EN-CONFIG-AW_Enterprise_FinAc_Service"
source: "EN-CONFIG-AW_Enterprise_FinAc_Service.pdf"
tags: ["A+W Enterprise", "FinAc Service", "Configuration", "Intrastat", "XML Export", "ERP", "Database", "Software for Glass", "eGecko", "SAP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides configuration instructions for the A+W Enterprise FinAc Service, a module for providing financial and accounting (FinAc) data to third-party systems. It covers installation, configuration using the FinAc Service Config Tool, logging, and the structure of control tables. The document also details specific functions like exporting documents, master data, and handling open items."
long_description: "This is a comprehensive internal guide for the A+W Enterprise FinAc Service. The document details the setup, configuration, and operation of this service, which acts as a bridge to export financial and accounting data from the A+W Enterprise system to external systems like eGecko, SAP, and proAlpha. It begins with a version history and an overview of the service's architecture. The guide provides step-by-step installation instructions, including manual steps for older versions and specific setups for Intrastat export. The core of the document focuses on configuration, covering the FinAc Service Config Tool, environment variables, and setting up automatic service restarts. It explains the logging mechanisms (service log, database log) for troubleshooting. Detailed descriptions of the key control tables, `fibutransfer` and `intrastat`, are provided, including field definitions and status codes to help diagnose processing errors. The document outlines the logic for various functions, such as exporting invoices, master data, stock transactions, and processing payment plans. A significant portion is dedicated to the Intrastat export functionality for Germany, Austria, and Slovakia, with specific data mapping tables for each country's requirements. Finally, it includes extensive troubleshooting sections for common issues like processing failures, database connection problems, and rounding errors."
---

# A+W Enterprise FinAc Service
**-INTERNAL-**
A+W - Software for Glass

---
## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2012-11-26 | SVH | Initial version | 1.0 |
| 2013-01-09 | MP | Addition of transfer logic | 1.1 |
| 2021-12-16 | SVH | Documentation Intrastat export Germany | |
| 2022-05-24 | SVH | Documentation Intrastat export Austria | |
| 2022-06-14 | SVH | Documentation performance, lock logic, SQL explain | |
| 2022-06-21 | SVH | Special treatment Product number -9999 | |
| 2022-06-29 | SVH | [AW-108450] - Correction "regionCode" | |
| 2022-07-14 | SVH | Docu "Automatic rebooting" | |
| 2022-10-04 | SVH | [AW-86600] - E-Mail dispatch | |
| 2022-11-10 | SVH | [AW-124033] – Updating of the open Items | |
| 2022-11-24 | SVH | Note about payment plan (partial/final invoice) | |
| 2023-03-23 | SVH | Additions/changes to cleanup logic | |
| 2024-01-26 | SVH | [AW-158197] + [AW-170082] - Intrastat-Export Slovakia | |
| 2024-04-25 | SVH | [AW-180534] – Description of currency determination | |
| 2024-07-08 | SVH | [AW-198935] – FinAc transfer of stock movements - Troubleshooting | |
| 2024-08-21 | SVH | [AW-198536] - Tax amount on the final invoice | |

## 1. General

The FinAc service is a module for providing FinAc data for third-party systems. Initial development was done with AWDesk #266591.

With [AW-84955], the functionality of the service was expanded. It can now also generate Intrastat data for the German Federal Statistics Office. There is a special chapter in this document about this functionality.

### 1.1. Availability/Versions

The FinAc service is available in Version 6.

Implemented are up to this point:
- XML interface to eGecko in different versions
- XML interface to SAP
- ASCII interface to proAlpha
- Intrastat export

**Version overview**

| Name | Comment |
| :--- | :--- |
| FinAc Service 5.5 | deprecated, installation no longer recommended |
| FinAc Service 6 | Current version of the FinAc service |

### 1.2. Documentation

All documents that are required as information source for the start-up of the FinAc service are provided on the A+W Sharepoint. They can be made available to the customer by Support/Planning.

- Installation instructions for the AWE FinAc service
- Configuration instructions for the AWE FinAc service (this document)
- Individual AWE FinAc interface documentation for the customer

### 1.3. Diagram

*A diagram shows the data flow for the A+W Enterprise FinAc Service. Data originates from ALCIB databases (DB 1 and DB 2), writing "fibutransfer" records. The "FIBU Service" fetches this transfer and booking data, retrieves its configuration, and then controls the process of generating XML files. These XML files are written to a local file system. A separate "Übertragungsprozess" (transfer process) picks up these XML files, sends them to a third-party system like "eGecko", and reports the status back to the FIBU Service.*

## 2. Installation

The procedure for the installation of the FinAc service is described in the installation document.

### 2.1. Installation

#### 2.1.1. General

For an installation with ALCIB versions 2011 and 2009, the following points listed must be executed manually.

**Create table fibutransfer/fibutransferok**

The following scripts must be executed:
- `...\install\xsql\12\1\1\120101001_fibutransfer.sql`
- `...\install\xsql\12\1\1\120101002_fibutransferok.sql`

**Creation of the number range fibutransid**

The following script must be executed:
- `...\install\xsql\12\1\1\120101003_nr_kreise.upd`
After that, the nr_server must be restarted

#### 2.1.2. Intrastat export

In Version AWE 6, it can be necessary to execute these points manually if the environment and the database version are not up-to-date.

**Create table intrastat/intrastatok**

- `..\alcib\14\0\de\install\xsql\13\0\4\130004168_intrastat.sql`
- `..\alcib\14\0\de\install\xsql\13\0\4\130004171_intrastatok.sql`
- `..\alcib\14\0\de\install\xsql\13\0\4\130004173_intrastat.sql`
- `..\alcib\14\0\de\install\xsql\13\0\4\130004174_intrastatok.sql`

**Make scripts available**

In the CMD directory, the scripts `intrastatinitexport` and `intrastatrecover` must be available.

## 3. Configuration

### 3.1. FinAc Service Config Tool

The configuration dialogs of the config tool are described in the installation document.

**Cleanup Time**
The default cleanup time is 40 days. The maximum configurable cleanup time is 1000 days (that is, nearly three years).

**Document Export Settings - Use Site Folders**
On the "Document Export Settings" dialog, by activating the "Use Site Folders" checkbox, it can be achieved that the files generated are written automatically to a site-specific subdirectory of "Export Root Path". The subdirectory corresponds to the configured "AWE site".

#### 3.1.1. Site-specific configuration

The FinAc transfer can be configured site-specifically. Every AWE site, especially every subsite in a multisite environment can be assigned a FinAc site.

*The user interface screenshots show the "Database Settings" and "Subsite Settings" dialogs within the A+W Enterprise 6 FinAc Service Configuration tool. The Database Settings allow mapping an AWESite to a FinAcSite, FinAcInterface, and specific database server. The Subsite Settings allow mapping a combination of AweMainSite and AweSubsite to a specific FinAcSite.*

### 3.2. FinAc service – automatic restart after abort due to error

Via the Windows "Services" dialog, the automatic restart of the FinAc service can be configured after an abort due to error.

For this, mark the FinAc service in "Services", then right-click to call up the context menu and select "Properties". Change to the "Recovery" tab there.

*The screenshot of the A+W Enterprise 6 FinAc Service Properties (Local Computer) shows the "Recovery" tab. It is configured to "Restart the Service" for the first, second, and subsequent failures, with a restart occurring after 1 minute.*

### 3.3. AWE environment variables

| Name | Description |
| :--- | :--- |
| **FIBU_FIBUTRANSFER_BOOKING** | The env variable must be activated. If the switch is active, a FinAc booking record is added to the fibutransfer table.<br>1 = booking of fibutransfer, 0 = no booking of fibutransfer<br>2 = test mode: booking of fibutransfer parallel to the previous FinAc booking logic<br>Activation of the variables only has effects if the logic was activated for the active FIBU_ART or the active USER_ID. |
| **FIBU_ART** | The env variable must be activated. Specification of the FinAc art. |
| **FIBU_RABATT** | The env variable must be activated so that non-redistributed discounts are not transferred to the FinAc. |
| **MODUL_WAEHRUNG** | The env variable must be activated. Activates the multi-currency capability (value contains the local currency). |
| **FIBU_WAEHRUNG** | The env variable currently has no influence on the processing in the FinAc service. |
| **EURO_XWAEHR** | Variable specifies the currency number of the EURO in the table xwaehr. The env variable currently has no influence on the processing in the FinAc service. |
| **FIBU_TRIANGULATION** | For amount calculation, switches for foreign currency between kauf.kurs (previous) and triangulation (future). If the variable is not set, triangulation is used. To switch off the triangulation, the variable must be set to "OFF." Setting to "OFF" does nothing!! |
| **WAEHRUNG_KURS** | If this environment variable is active, then the conversion rate of a foreign currency under MASTER DATA=>KEYS=>SYSTEM KEY=>CURRENCY is interpreted as units of own currency for ONE unit of foreign currency. With a variable that is not set (default), the conversion rate is interpreted as units of the foreign currency for ONE unit of the own currency. The variable must be activated before starting an operation and must be retained. |
| **KUPLUS_ACTIVE_FIELDS** | The variable is evaluated when updating the open items. |
| **LIMITS_MANDANTENTRENNUNG**| Limit check for the table limits. The variable is evaluated when updating the open items. |
| **WL_AWE_TO_FINAC** | The env variable is required for the export of stock transactions from the A+W Enterprise stock. WL_AWE_TO_FINAC generally has to be activated with "ON" so that the A+W Enterprise stock booker fills the transfer table wltofinac. |

## 4. Logging

### 4.1. ftest

For searches that affect the filling of the interface table fibutransfer, a ftest can be switched on.

### 4.2. FinAc service log

Via the config tool of the FinAc service, the log file and the log level are specified.

For searches that affect the generation of the interface files, the log level must first be configured appropriately. After that, the affected process will be presented to the FinAc service again for processing. The log created this way can then be evaluated.

The central trace categories are "AWEFinAcService" and "AWEBasis".

In normal operation, the trace level "Error" or "Info" should be set for "AWEFinAcService". For "AWEBasis" in any case the trace level "Error" should be set since otherwise the log file quickly becomes very large.

For the search, for "AWEFinAcService", the trace level is changed to "Debug". "AWEBasis", by contrast, does not essentially have to be set to the trace level "Debug"; this only in individual cases.

*The screenshot of the Protocol Configuration dialog shows settings for Trace Level and Log Level for categories AWEBasis (Error/Info) and AWEFinAcService (Debug/Info).*

### 4.3. Database log

In the database configuration, it is possible to activate the database log with the "SQL Explain" checkbox. The activation then exists for the corresponding database as long as the A+W Enterprise FinAc Service is running or as long as it is restarted without configuration change.

The database log should only be used briefly for research/analysis purposes and after that deactivated immediately, for the logs can quickly get very large and thus cause storage space problems on the DB server.

## 5. Control table fibutransfer

The table fibutransfer is the control table for the FinAc booking.
Successfully processed records are transferred with appropriate configuration to the back-up table fibutransferok.

| No. | Field | Data Type | Content/example |
| :--- | :--- | :--- | :--- |
| 1 | fibutransid | integer | Unique booking code from own number range (fibutransid). See chapter "IDs in the table fibutransfer". |
| 2 | status | smallint | See chapter "Status values in the table fibutransfer". |
| 3 | hausnr | smallint | AWE site number. |
| 4 | btyp | smallint | Booking type:<br>1 = master data<br>2 = transaction data<br>3 = open items ("open amounts")<br>4 = open orders ("ongoing orders")<br>5 = Stock transactions<br>6 = Intrastat declaration<br>7 = Update limits/kuplus |
| 5 | auftrnr | integer | Key data for document bookings (invoice, credit, collective invoice). |
| 6 | procedure | smallint | |
| 7 | subnr | smallint | |
| 8 | mpnr | integer | Key data for MP bookings (customer/debtors, suppliers/creditors). |
| 9 | kuliflag | smallint | |
| 10 | izeit | datetime | Time stamp of the insert in the booking table. |
| 11 | uzeit | datetime | Time stamp of the last update of the service. |
| 12 | serviceid | char(40) | Unique ID of the service that processes this record. The ID must be emptied if a record is reset by hand to status 0 or -1. |
| 13 | versuche | smallint | Number of transfer attempts. Is incremented if the service sets either the status "processed successfully" or an error status. |
| 14 | xmldatei | char(80) | Name of the xml file in which the debtor booking or the SP invoice booking is located. |
| 15 | xmldatei2 | char(80) | Name of the xml file in which an automatically generated additional document (e.g. automatic SP invoice booking) is located. (only filled in special cases!) |
| 16 | sfill1 | smallint | Short field for future purposes. Filled with the value "1" for incoming goods cancellation bookings. |
| 17 | sfill2 | smallint | Short field for future purposes. |
| 18 | lfill1 | integer | Long field for future purposes. Filled with kauf.aufnr when booking incoming goods. |
| 19 | lfill2 | integer | Long field for future purposes. |
| 20 | cfill1 | char(20) | Char field for future purposes. |

## 6. Status values in the table fibutransfer

This section describes the status values used in the table fibutransfer. These are especially error codes that help identify and solve errors that have occurred.

### 6.1. Status -1 – 99: progress status

| No | Status | Description |
| :--- | :--- | :--- |
| -1 | StartImmediatly / Urgent | New booking record that should be processed immediately. Caution: booking records that wait with status "0" receive, when the configured processing time has been reached, briefly the status "-1" before they change to the status "1" (progress). |
| 0 | Waiting | New booking record. |
| 1 | Progress | Booking record in process. |
| 2 | TransferFileReady | Transfer file was created successfully. |
| 11 | FileReadyAvoidTransfer | Transfer file was created successfully, no transfer planned. |
| 90 | RequestDismissedGoodsReceivedStorno-NonStornoPair | Customer-specific [AW-71301] |
| 91 | RequestDismissedInternalVoucher | Customer-specific [AW-62883] |
| 92 | RequestDismissedPayType | Customer-specific (AWDesk #459504) |
| 93 | RequestWaitingForKaufStillZero | Customer-specific (AWDesk #458356) |
| 94 | RequestDismissedCustIndivOutOf-NumberRange | Customer-specific (AWDesk #441441) |
| 95 | RequestDismissedNullAmount | No processing due to zero quantity (AWDesk #379226). |
| 96 | RequestIgnoredNotImplemented | No processing (functionality not implemented). |
| 97 | RequestDismissed | Keine Abarbeitung (No processing) |
| 98 | Duplicatelgnored | No processing because record duplicate. |
| 99 | Success | Booking record was processed successfully. |

### 6.2. Status 100 – 149: general error or incorrect configuration

| No | Error | Description |
| :--- | :--- | :--- |
| 100 | Error | Error that cannot be identified precisely. |

### 6.3. Status 150 – 199: incorrect fibutransfer data
*(No specific errors listed in this range)*

### 6.4. Status 200 – 249: error during the creation of the XML files

| No | Error | Description |
| :--- | :--- | :--- |
| 201 | DataError | General data error. The AWE data could not be transformed into xml format. Search in the log for a more precise description of the error. |
| 202 | XhausDataError | Data error in the table xhaus. No xhaus record for a site or a customer could be found. Search in the log for a more precise description of the error. |

### 6.5. Status 250 – 299: error in the transfer

| No | Error | Description |
| :--- | :--- | :--- |
| 250 | TransferError | General error in the transfer logic. Origin unknown. More information in the log. |
| 251 | TransferTypeUnknown | The Transfer Type switch has an unknown value. |
| 252 | ExportPathIsNullOrEmpty | The switch ExportPath is not set. |
| 253 | ExportPathDoesNotExist | The directory that was stored in the switch ExportPath does not exist. |
| 254 | TransferBasePathIsNullOrEmpty | The switch TransferBasePath is not set. |
| 255 | TransferBasePathDoesNotExist | The directory that was stored in the switch TransferBasePath does not exist. |
| 256 | FtpServerNamelsNullOrEmpty | The switch FTPServerName is not set. |
| 257 | FtpUserIsNullOrEmpty | The switch FTPUser is not set. |
| 258 | FtpPasswordIsNullOrEmpty | The switch FTPPassword is not set. |
| 259 | MaxFtpAttempsIsNotValid | The switch MaxFtpAttempts has an unknown value. |
| 260 | XMLServiceFlagIsNotValid | The switch XMLServiceFlag has an unknown value. |
| 261 | FilenamelsNullOrEmpty | Within the file list transferred, there is a record with an empty file name. |
| 262 | ExportFileDoesNotExist | The file to be transferred does not exist in the ExportPath directory. |
| 263 | ExportFileCouldNotBeDeleted | The file cannot be deleted. |
| 264 | DestinationPathCouldNotBeDetermined | No target path could be determined. This means that the name of the export file does not correspond to the valid format. |
| 265 | DestinationPathDoesNotExist | The target path determined does not exist and could also not be created. |
| 266 | ExportFileCouldNotBeTransfered | The file could not be transferred. Under some circumstances, write permissions may be lacking. |
| 267 | FtpConnectionCouldNotBeEstablished | The connection to the FTP server could not be established. |
| 268 | ErrorConflictXmlFiles | Two files are stored in the fibutransfer record and there were different errors for both transfers. More information in the log. |
| 271 | ErrorCreatingExportFile | The file could not be written. If a network path is accessed, the path must be specified in UNC notation in the config tool. No network drive letter may be used in the path specification. Additional possible cause: error in the XML format. |

### 6.6. Status 300 – 399: error in special logic

| No. | Error | Description |
| :--- | :--- | :--- |
| 321 | SomeFilesCouldNotBeProcessed | Error during import of "open items." One or several file(s) could not be imported or processed. |

## 7. IDs in the table fibutransfer

The field `fibutransfer.fibutransid` is filled via the number range "fibutransid" if the FinAc transfer is started from A+W Enterprise.

There are special cases in which the FinAc service itself generates a fibutransfer record in order to process it subsequently. In these cases, the ID is negative. It is not determined from a number range, but rather repeated each time when the FinAc service writes the record type to fibutransfer. The fibutransid arises in that "-1000" is subtracted from the value of the booking type.

For example, for "Intrastat": -1000 – 6 = -1006.

The listing of these special cases is in this table.

| fibutransid | Name | Description |
| :--- | :--- | :--- |
| -1003 | Orders in Work | Export of the open/running orders. Customer-specific configuration. |
| -1004 | Unpaid Invoices | Import of the unpaid invoices. Customer-specific configuration. |
| -1005 | Stock transactions | Export of stock transactions. Customer-specific configuration. |
| -1006 | Intrastat | Export of Intrastat data. Special configuration. |
| -1007 | Update limits/kuplus | Updating of the open items (balances). |

Negative IDs can also arise if booking requirements are inserted via scripts.

## 8. Processing of the FinAc transfer data

The transfer data stored in the table fibutransfer is processed cyclically or at the configured point in time by the FinAc service.

First, the transaction transfer data (invoices/credits) for all configured sites is processed, then the master transfer data (debtors/creditors) of all sites is processed.

### 8.1. Rush FinAc transfer data

In the individual programs, the script "update_urgent_fibutransfer" is created as individual program.

The execution of the script means that all fibutransfer records of the current DB with the status 0 are updated to status -1.

The records with status -1 are processed with the next polling of the DB. Records with status 0 are kept until the specified processing time.

During the processing of the rush transfer data, first the master transfer data (debtors/creditors) for all configured sites is processed, then the transaction transfer data (invoices/credits) of all sites is processed.

**Attention**: Here the processing sequence is the reverse of the general sequence at the specified processing time. This difference in the processing sequence exists for historical reasons and has no deeper meaning.

## 9. Generation of the local XML files

Depending on the configuration in the config tool, the XML files generated are stored locally or there is a direct transfer to the company network or to an FTP server.

It can also be configured in the config tool whether or not the local files should be deleted after the transfer.

The storage location of the local files is specified in "export root path." If the "Use site folders" checkbox is checked, the files are written separately by AWE sites in subdirectories of "export root path."

The standard structure of the XML files is defined as follows:

- **Debtor files**
  `DE_XX_YY_<Zeitstempel>.xml`
- **FinAc document files**
  `FB_XX_YY_<Zeitstempel>.xml`
- **Core document files**
  `KB_XX_YY_<Zeitstempel>.xml`

(XX = FinAc site, YY = AWE site)

However, it is also possible to define customer-specific file names. In this case, it has to be clarified whether the transfer logic has to be adjusted accordingly.

See also section 10 "Transfer of the XML Files."

Depending on the configuration, the directory structure is:
`ExportRootPath` or `ExportRootPath\YY`
(YY = AWE site)

## 10. Transfer of the XML files

Depending on the transfer type switch, a transfer of the XML files on the company network or to an FTP server can be configured.

The logic behind this behaves the same way in both cases.

All files to be transferred will be expected in the configured export directory. This will be checked in the first step.

For each file, it is then determined using the file name to which FinAc client it belongs and whether it is a master data or document file.

The structure of the XML files was defined as follows for the implementation of the transfer logic:

- **Debtor files**
  `DE_XX_YY_<Timestamp>.xml`
- **FinAc document files**
  `FB_XX_YY_<Timestamp>.xml`
- **Core document files**
  `KB_XX_YY_<Timestamp>.xml`

(XX = FinAc site, YY = ALCIB site)

Which produces the following specified directory structure:

- **Master data**
  `TransferBasePath\XX\sd`
- **Transaction data**
  `TransferBasePath\XX\fb`

(XX = FinAc site)

**CAUTION**: On customer request, the names of the XML files can also be different. In this case, it has to be clarified whether or not the customer wants to use transfer logic. If the transfer logic should be used, under some circumstances, customer-specific adjustments to the logic have to be made so that the files can be transferred to the desired transfer directories.

It is now checked whether the target directory exists. If the path does not yet exist, it is created anew. This assumes that either the service user in the case of transfer on the network and the FTP user in case of the FTP transfer has sufficient write rights for this action!

Then the file is transferred. If everything has worked without error thus far, the XML file is deleted in the original export directory unless something else was configured.

An individual transfer status was determined for each file. It is now reported back to the transfer table.

In the case of the FTP transfer, there is a special feature. With the configuration switch max. attempts, you can set how often it should be attempted to upload a file to the FTP server if there is an error during transfer, e.g. because the FTP server is temporarily unavailable.

**Note**:
After saving the files in the transfer directory, the further processing of the files is the customer's responsibility.
In particular, if files are moved and/or renamed, it can no longer be traced whether the content of the files has also been manipulated.

## 11. Functions

### 11.1. Export of documents (SA/PU invoices/credit notes)

The export of invoices and credit notes is handled by the basic functionality of the FinAc service. However, each export logic is implemented customer-specifically depending on the target system. In addition, the FinAc service offers other export and import interfaces, which can also be made available customer-specifically. They are described here in further chapters.

#### 11.1.1. Document line items

Only valid (active) document line items are exported. Cancelled items (kpos.aendkz = 2) are ignored.
See PF [AW-108418].

### 11.2. Export of master data (customers/suppliers)

#### 11.2.1. Digression: Generation of the transfer records from the AWE Backend

**Multisiteconfiguration - internal site separation**

The FinAc transfer with multisite configuration must be implemented customer-specifically. Previously for some customers (USER_IDs), there is already a multisite master data transfer.

If the env variable `FIBU_MANDANTENTRENNUNG` is activated, the internal sites are taken into account during FinAc transfer. The variable influences both the transfer of payables and the transfer of vendors.

The activation of the variables causes that for a payable/vendor to be transferred, for each configured site of a system with internal site separation, a transfer record with the corresponding site number is provided in the table fibutransfer. The configured sites are determined from table xhaus.

The `MP_SITE_EXACT` variable overrides this logic. If `MP_SITE_EXACT` is active, for each market partner transferred, it is checked whether for a configured site there is also an entry in the table mpmdzu. Only if this entry exists is the corresponding transfer record written.

For customers, the described logic can be overridden again by the variable `LIMITS_MANDANTENTRENNUNG` (see AWDesk #388239). If `LIMITS_MANDANTENTRENNUNG` is active, only transfer records for sites are written for which an entry in the table limits is found.

### 11.3. Updating of the open items (balances)

#### 11.3.1. Functions

AWDesk #349767, [AW-77698], [AW-124033]

After the transfer of transaction data (invoices/credits), there is a check whether the open items must be updated. They are updated in the table kuplus depending on the env variables `KUPLUS_ACTIVE_FIELDS`.

If the env variable `LIMITS_MANDANTENTRENNUNG` is active with the value "ON," the table limits are updated; otherwise the table kuplus.

If `KUPLUS_ACTIVE_FIELDS` contains the entry "op_brutto," "op_brutto" is used in kuplus and limits for the updating instead of "op".

- **Table kuplus**
  The amounts in `kuplus.fibu_op`, `kuplus.op` and `kuplus.op_brutto` are updated.
- **Table limits**
  The amounts in `limits.fibu_op`, `limits.op` and `limits.op_brutto` are updated.

**Adjustment with [AW-124033] – refinement of the logic**

It can be that at the time of the update of the open items, there are still records with SA transaction data (SA invoices/SA credits) in the table fibutransfer. These can be either waiting records or records that encountered an error. Crucial is that no XML file is stored yet in the fibutransfer record (entry in fibutransfer.xmldatei field, see also [AW-138111]).

In this case, the following logic runs in the FinAc service: The debtor and open amount will be determined for these records previously not transferred to the FinAc. If the env variable `KUPLUS_ACTIVE_FIELDS` contains the entry "op_brutto," the open amount is determined from rechfuss.gesbrutto; otherwise from rechfuss.nettototal.

- **kuplus Table**
  The amount in `kuplus.fibu_op` is increased by `kuplus.op` or `kuplus.op_brutto` and `kuplus.op` or `kuplus.op_brutto` is then set to "0".
- **limits table**
  The amount in `limits.fibu_op` is increased by `limits.op` or `limits.op_brutto` and `limits.op` or `limits.op_brutto` is then set to "0".

After the amount in the table field "fibu_op" was incremented by "op"/"op_brutto," and "op"/"op_brutto" has been set to "0", the amount in "fibu_op" is then reduced by the total of the open amounts for each debtor, the amount in the table field "op_brutto" or "op" is increased by the total of the open amounts.

The updated amounts are written back to kuplus/limits.

**Please note:**
Thanks to the logic of updating open items by the FinAc service, the value in `kuplus.fibu_op`/`limits.fibu_op` can deviate from the value that is imported initially via the file `salden.dat` by the `trm_ctrl`. This effect occurs if at night first the import (`salden.dat`/`trm_ctrl`) and then the FinAc transfer of the FinAc service is started.
See also PF [AW-124033].

#### 11.3.2. Troubleshooting

1.  **A customer's open items appear not to be correct.**
    -> Check whether there are still records for the customer/debtor in the table `fibutransfer`.
    See also PF [AW-138111].
2.  **The update of the balances should be triggered manually.**
    Manual insert into the table `fibutransfer`:
    `insert into fibutransfer (fibutransid, status, hausnr, btyp, auftrnr, vorgang, subnr, mpnr, kuliflag, izeit, uzeit, serviceid, versuche, xmldatei, xmldatei2, sfill1, sfill2, lfill1, lfill2, cfill1) values (-1007, -1, <hausnr>, 7, 0, 0, 0, 0, 0, CURRENT YEAR TO SECOND, '', '', 0, '', '', 0, 0, 0, 0, 0)`
3.  **Error "Concurrency violation"**
    Error message: "Concurrency violation: The UpdateCommand has affected x of the expected y data records."
    Check whether other processes that access the limits/kuplus tables are still running at the time of the error message, e.g. import (`salden.dat`/`trm_ctrl`).
    If necessary, change the start time of the process(es) so that they do not interfere with each other.
    See also PF [AW-227292].

### 11.4. Import of the open items ("open amounts") from the FinAc (AWDesk #379226)

The import of the open items from the FinAc is realized customer-specifically.

This means that in the FinAc Service, there is no logic for the import of the `salden.dat`. The import of the `salden.dat` is still done via the DFÜ/`trm_ctrl`. For additional information, please see the EDI configuration instructions.

To see whether there is already a customer-specific logic for import of the open items in the FinAc Service, consult the customer-specific interface description.

#### 11.4.1. Import directory

The import processes files that are in a configured work directory.

The root directory is stored in the config tool. Below the root directory, all company numbers are created as folders, which are specified on the "Database settings" dialog in the "AWESite" file and for which an import should be executed.

Below each company number directory, the directories:
- `work`
- `archive`
- `problem`
must be created.

**Example:**
The directory structure for an AWESite '140' would be `<Import Root Path>\140\` containing `work`, `archive`, and `problem` subfolders.

The FinAc service must have read rights to all directories, as well as the right to rename and copy files.
All files to be imported must be stored in the directory `<Import Root Path>\<AWESite>\work`.

#### 11.4.2. Import logic

On the start of the import, all files stored in the work directory will be processed. Error-free imported files will be stored with prefix "archived_<Timestamp>" in the "archive" folder.

If an error occurs during the processing of a file, the entire file is discarded and stored in the "problem" folder with the prefix "problem_<Timestamp>".

During the import of the open items, the field `fibu_op` in the table limits (or kuplus) is updated.

If the current site is a master or submaster (`xhaus.dbart=1` or `xhaus.dbart=2`), `limits.fibu_op kundengenau` is updated, otherwise `kuplus.fibu_op`.

If the env variable `LIMIT_ZENTRALE_DB` is not active and the current site is a master or submaster (`xhaus.dbart=1` or `xhaus.dbart=2`), then both fields `limits.fibu_op` and `kuplus.fibu_op` are updated.

#### 11.4.3. Environment variables

`LIMIT_ZENTRALE_DB`

#### 11.4.4. Starting the import outside of the configured times

In the individual programs, the script "insert_open_amounts_fibutransfer" must be created as an individual program with parameter "hausnumber".

The execution of the script causes a trigger record for the import of the open items for the current company number to be written to `fibutransfer`.

With the next polling of the DB, the import is executed.

### 11.5. Export of ongoing orders from AWE (AWDesk #379226)

The export of ongoing orders from AWE is realized customer-specifically. To see whether the logic is already available, consult the customer-specific interface description.

### 11.6. Export of stock transactions

It is possible to export stock transactions from the A+W Enterprise stock in combination with the stock booker and the FinAc service.

#### 11.6.1. Configuration

**Env variables**
So that the stock booker provides the stock transaction data in the table `wltofinac`, the env variable `WL_AWE_TO_FINAC` generally has to be activated with "ON."

**Master data**
In the article field configuration (`artcomfld`), the configurable field "FinAc Transfer" has to be created as numeric data type.

In the AWE article master data, the article has to be identified for which a booking to the FinAc should be made; the identification is made through the entry of a "1" in the configurable field "FinAc Transfer."

Using this identification logic, articles kept in the AWE stock for which a FinAc transfer is required can be distinguished from those that should not be transferred to the FinAc.

**Config tool**
Configuration of the start time of the file generation and of the transfer directory.

#### 11.6.2. Functions

**Transfer tables**
With the updating of the AWE environment to the status "Quality Release 05/19" (31.05.2019), the required transfer tables `wltofinac` and `wltofinacok` are available.

**Table wltofinac**
The stock booker writes stock removals and receipt in the table; these should be transferred to the FinAc service (evaluation of `wlh.b_status`). See also the overview of the stock booker status values below. Here, there is no evaluation of the configurable field "FinAc Transfer" for the booking record. Booking articles that are not identified for FinAc transfer are sorted out later by the FinAc service.

| Field | Type | Description |
| :--- | :--- | :--- |
| artnr | integer | AWE article number |
| bitnr | smallint | AWE variant number |
| b_preis | decimal(16) | Booking price (current average price) |
| b_status | smallint | AWE booking status |
| b_zeit_awe | datetime year to second | AWE booking time |
| b_zeit_finac | datetime year to second | Booking time of FinAc service |
| lnr | integer | Stock number. |
| hausnr | smallint | Site Number |
| error | integer | Processing flag/error flag. On insert by the stock booker, the error flag is on the value "0". For the records in this table, there is no urgent logic like in the table `fibutransfer`. The error value is not taken over into the table `wltofinacok`. Records in `wltofinacok` count as processed without errors. Possible error values are documented under a special title. |

**Error values in the table wltofinac (field wltofinac.fehler)**

| Error number | Description |
| :--- | :--- |
| 0 | Ready for processing |
| -2 | In processing by the FinAc service. In some error cases, the records with this error value get "stuck". |
| 99 | Successfully processed by the FinAc service. This error value is generally not visible since records with this value are shifted into the table wltofinacok. |
| 102 | The record is not transferred to the FinAc. This error value is generally not visible since records with this value are deleted by the FinAc service. |
| 201 | Error not further specified. |
| 202 | Missing account. |
| 203 | Missing counter account. |
| 204 | Missing cost center. |

**Table wltofinacok**
The FinAc service writes all successfully processed booking records to the table; furthermore, also the booking records cumulated via the article number that are written to the transfer file.
The cumulated records can be recognized because the field `b_zeit_awe` has no current time stamp, but rather the default value "Minimum Date" (0001-01-01 00:00:00).

| Field | Type | Description |
| :--- | :--- | :--- |
| artnr | integer | AWE article number |
| bitnr | smallint | AWE variant number |
| b_preis | decimal(16) | Booking price (current average price) |
| b_status | smallint | AWE booking status |
| b_zeit_awe | datetime year to second | AWE booking time |
| b_zeit_finac | datetime year to second | Booking time of FinAc service |
| lnr | integer | Stock number |
| hausnr | smallint | Site Number |
| konto | integer | Account |
| kstelle | integer | Cost Center |
| counter | integer | counter account |

**Description of the flow**
If the environment variable `WL_AWE_TO_FINAC` is active, the stock booker checks with each booking processed using its status value (receipt, removal) whether it comes into question for a transfer to the FinAc. If this is the case, an appropriate booking record is written to the table `wltofinac`. All AWE stock bookings are written to the table `wltofinac` except manual AWE receipts and receipts due to inventory differences (note: the booking of an inventory difference always contains the time stamp of the start of the inventory). Stock removals are transferred with a negative leading sign. See also the overview of the stock booker status values below.

The price written to `wltofinac.b_preis` is rounded to 6 places after the decimal point (AWDesk #457773).

The booking records from `wltofinac` are processed once a day by the FinAc service. Start time of the file generation and transfer directory can be configured in the config tool of the FinAc service.

The transfer file is generated according to the customer-specific requirement.

Only stock bookings for articles are written to the transfer file that are specially marked in the master data (stock-kept articles). The identification is done via a private field (table `artprvfld`) with the field designation (`artprvfld.fldbez`) "FinAc Transfer"; the value of the field (`artprvfld.longval`) has to be assigned the value "1" so that the article is transferred to the FinAc.

Records that could be written successfully to the transfer file are transferred to `wltofinacok` and deleted in `wltofinac`. Booking records for articles that should not be transferred to the FinAc are also deleted from `wltofinac`, however they are not transferred to `wltofinacok`.

If for some reason records remain in `wltofinac`, these are considered again during the next transfer.

The records in `wltofinacok` are deleted according to the configured "clean-up time" in the config tool.

**Note about inventory evaluation**
The transfer of the inventory evaluation (booking status 25) was implemented with AWDesk #461899. The difference amounts that arise from an inventory evaluation are incorporated into the total formation.

**Overview of the stock booker status values (wlh.b_status) for which an entry is made in the table wltofinac**
For all status values not listed in the table, no entry is written to the table wltofinac.

| Status | Designation |
| :--- | :--- |
| 11 | Stock receipt |
| 12 | Stock removal |
| 21 | Inventory receipt |
| 22 | Inventory removal |
| 25 | Stock evaluation (#461899) |
| 26 | Inventory variant delete |
| 28 | Inventory variant and log delete |
| 29 | Stock receipt external - [AW-232628] |
| 30 | Stock removal external |
| 32 | Variant delete |
| 34 | Variant and log delete |
| 36 | Variant log delete |
| 42 | Article delete |
| 44 | Article and log delete |
| 46 | Article log delete |
| 52 | Purchase shelf removal |
| 54 | PMS shelf removal |
| 62 | Purchase removal |
| 64 | PMS removal |
| 66 | Purchase box removal |
| 68 | PMS removal external |
| 71 | Box receipt |
| 72 | Box removal |
| 81 | Inventory box receipt |
| 82 | Inventory box removal |
| 111 | Shelf receipt |
| 112 | Shelf removal |
| 115 | Inventory shelf receipt |
| 116 | Inventory shelf removal |
| 124 | Delivery note removal - [AW-68577] |
| 351 | Stack receipt |
| 352 | Stack removal |
| 361 | Inventory stack receipt |
| 362 | Inventory stack removal |
| 364 | Stack stock inventory |
| 403 | Completion report receipt |
| 404 | Completion report removal |
| 415 | Packed message receipt |

#### 11.6.3. Troubleshooting – an already-generated transfer file has gone lost

If a transfer file gets lost without having transferred the data to the FinAc, it can be necessary to unload records from a particular time interval from the table `wltofinacok` and to insert them again into the table `wltofinac` in order to process them again.

**Caution**:
It must be noted that no cumulative entries are present in the table `wltofinacok`. The cumulated records can be recognized because the field `b_zeit_awe` has no current time stamp, but rather the default value "Minimum Date" (0001-01-01 00:00:00).
The cumulated records may not be transferred into the table `wltofinac`. They are generated again with another process. If they are present in the table `wltofinac`, they cause an exception in the FinAc service during processing. The exception that is generated is unfortunately misleading, so that you won't recognize the cause of the problem right away.

The following statement can be used to unload the data from `wltofinacok`:
`unload to wltofinac select artnr, bitnr, b_preis, b_status, b_zeit_awe, b_zeit_finac, lnr, hausnr, 999 from wltofinacok where b_zeit_finac >= DATE('...') and b_zeit_awe != DATE('01.01.0001')`

In the statement, a "999" is attached to the unloaded records so that the records are loaded into the table `wltofinac` with a defined error value (`wltofinac.fehler`).

After unloading, the unloaded records PLUS the cumulated records with the corresponding statement in `wltofinacok` should be deleted.

If the records are inserted into the table `wltofinac`, in the FinAc service Config Tool, the processing time must be set to the desired time and the records inserted must be updated from `fehler=999` to `fehler=0`.
After the successful generation of the file, the processing time in the FinAc service Config Tool must be reset to the original value.

See PF [AW-198935].

### 11.7. Standard logic for determination of the currency used in the FinAc document data

The following logic for determination of the currency in the transfer data is used by default.
If there is a customer-specific deviation in the logic, it is described separately in the customer-specific documentation of the interface.

In the invoice/credit, it is stored in the field `kauf._waehrprs` with which currency the calculation should be done:
- `0` = National currency
- `1` = Foreign currency

If calculation should be done in foreign currency (`kauf._waehrprs` = 1), the currency is used from the field `kauf.waehrung`.

If calculation should be done in national currency (`kauf._waehrprs` = 0), there is a check whether the env variable `MODUL_WAEHRUNG` is active with a value > 0.

If `MODUL_WAEHRUNG` is active with a value > 0, the currency is used that is assigned to the stored currency number (`xwaehr.wnr`).

If `MODUL_WAEHRUNG` is not active or is <= 0, the currency with the currency number (`xwaehr.wnr`) "1" is used.

Essentially there is also a possibility to specify the currency in the FinAc transfer via the env variable `FIBU_WAEHRUNG`.
However, the evaluation of `FIBU_WAEHRUNG` is currently not implemented in the FinAc Service.

### 11.8. Sending an e-mail in case of error

If errors occur during export of the FINAC data, a corresponding info e-mail is sent insofar as the e-mail configuration has been done.

**Site numbers over placeholders**
The e-mail configuration is done via the Config tool of the FinAc service. If it is necessary to design the recipient e-mail address site-specifically, the placeholder "$SITE$" can be stored as recipient. The placeholder is replaced with the current site number when sending. Here, a leading "0" is used for single-digit site numbers.

**Caution**: In the sender address, there is no replacement of the placeholder.

Precisely one e-mail is sent per site, processing type (e.g. master data, documents, etc.) and processing cycle.

Errors in the processing of documents are reported independently of the time stamp (`fibutransfer.izeit`) of the processing record (`fibutransfer` record) via e-mail, as long as the record is present in the table `fibutransfer`.
Errors in the processing of master data and all other processings are only reported for 2 days. As soon as the error record has a time stamp (`fibutransfer.izeit`) that is longer than 2 days in the past, the error is no longer reported via e-mail.

The e-mail is in English. At the moment, there is no other language choice available.
See PF [AW-86600].

### 11.9. Cleanup - data cleansing

The cleanup time span (in days) can be configured in the Config tool. If the cleanup time is not configured, the value "40 days" will be used as the default.

**Back-up table fibutransferok**
If in the Config Tool the transfer of processed records to the back-up table `fibutransferok` is configured, the back-up records there are deleted when the configured "cleanup time" is reached.

The time stamp in `fibutransferok.uzeit` is used as reference for the "cleanup time". This is the time at which the record was processed by the FinAc service.
**Caution**: the logic has been changed; previously, "izeit" was used.
**Caution**: If a record initially remains for a long time with an error code in the table `fibutransfer`, then the source of the error is eliminated and the record processed successfully, the "old" time stamp in the "izeit" field can mean that the record is deleted immediately from the table `fibutransferok` at the next cleanup.

**Back-up table wltofinacok**
Records in the back-up table `wltofinacok` are deleted when the configured "cleanup time" is reached.
The time stamp in `wltofinacok.b_zeit_finac` is used as reference for the "cleanup time". This is the time at which the record was processed successfully by the FinAc service.

## 12. Customer-specific interfaces

The documentation for customer-specific interfaces is available in the separate documents.

## 13. Working with payment plan (partial/final invoice)

Since 2022, customers have been indicating increasingly that they will want to work with payment plans in A+W Enterprise in the future.

If the payment plan logic is put into operation, in the course of this, the FinAc transfer for partial and final invoices must also be tested.

It cannot be ruled out that the use of payment plans requires adjustments in the logic of the FinAc transfer. It's not possible to make a blanket statement about this. The situation has to be checked individually for each customer.

See also [AW-122198], [AW-128055], [AW-117351]

**Note**
A deposit invoice is identified with `kauf.eingang = 12`.
A final invoice is marked with `kauf.eingang = 13`.

Deposit invoices and final invoice that belong together have the same order reference in `kauf.referenz`.

In the final invoices, the partial payments made are stored as discount records. The article number of the partial payment article is stored in a partial payment record. A partial payment article is defined by the `article.atyp 995`.

If a customer is working with a payment plan but no non-redistributed discounts are transferred to the FinAc (FIBU_RABATT "OFF" or not set), a special logic in the FinAc service ensures that the partial payment discounts are considered in the final calculation.

### 13.1. Treatment of tax amounts in the final invoice

If the net amount (`kauf.nettototal`) of a final invoice is very small (cent range), a VAT amount of "0.00" can result from this.

Since the VAT amount is used as basis for the distribution of the VAT across the FinAc items, a zero amount is not permissible.

In this case, the VAT record of the final invoice (`kauf.kukz` -> `xmwst.satz`) is used in order to recalculate the VAT amount without restriction of the places after the decimal point and for the redistribution to the FinAc items.

See PF [AW-198536].

## 14. Troubleshooting

### 14.1. Manual manipulation of fibutransfer

**Present record with error status again for processing (update)**

- **Immediate processing**
  If for searching purposes, a record in the table `fibutransfer` that has encountered an error should be presented to the FinAc service again for immediate processing, the status must be updated to -1; furthermore, the `serviceid` must be emptied ('').
  The records with status -1 are processed with the next polling of the DB.
- **Processing for the configured time**
  If a record in the table `fibutransfer` should be presented to the FinAc service again for processing, `fibutransfer.status = 0` and `fibutransfer.serviceid = ''` (empty) must be set.

**Send successfully processed record back again for processing (unload/load)**

**Attention**: Caution is in order! It must be ensured that there will not be doubled data in the transfer files due to renewed processings.

Records that should be re-presented must unload from the table `fibutransferok` and then be loaded into the table `fibutransfer`.

After this, there must be an update:
`fibutransfer.status = -1/0`
`fibutransfer.serviceid = ""`
`fibutransfer.xmldatei = ""`

**Generate record manually (insert)**
With suitable insert statements, processes for processing can be presented to the FinAc service manually. Such a manipulation if it is absolutely required should never be done by the customer, but always by A+W Support.

When generating records for incoming goods booking, special caution is required. Here, for the insert in addition to the standard fields, the fields `lfill1` (`kauf.aufnr`) and for incoming goods cancellations `sfill1` (cancellation flag 1) have to be filled.

**Memory holes**
FinAc service takes up ever more memory with time.
If this problem occurs, please contact development.
It is probably in connection with #277739.

### 14.2. No or incorrect processing

FinAc service is running, however it did not process any records from the table `fibutransfer`.
Please check whether several database connections with the same AWE site number are stored in the Config Tool. Such a configuration results in the error described. The doubled site number must be removed.

Since AWDesk #447648, the storage of an already-existing AWE site number has been prevented. Here it plays no role whether the existing database connection is activated or deactivated.

**Handling of documents (invoices/credits) for which the FinAc transfer fails**
It can happen that the FinAc service cannot perform a document transfer to the FinAc due to a data error. The document record then remains with error status (generally status 201) in the transfer table `fibutransfer`. The document (invoice/credit) counts as already booked in AWE at this point in time and it can no longer be changed.

The state must be resolved so that the data is consistent in AWE and FinAc.
There are several approaches for this. Which one is used depends on the cause of the error:

1.  **Correction of the error in the AWE master data and resetting of the error status in the transfer table fibutransfer**
    If the error is triggered in the FinAc transfer due to missing or flawed master data, it is sufficient to correct this and then reset the transfer record in the table `fibutransfer` so that the transfer is started once again.
2.  **Manual resetting of a document (invoice/credit) in AWE for the correction of amounts and other invoice data and renewed transfer to the FinAc service**
    If an affected invoice/credit was not yet transferred to the customer, the invoice correction can be treated as an internal error. The A+W Enterprise Service can be contacted. The service employees are in a position to reset the status of the invoice/credit so that the data can be corrected and the document transfer to the FinAc can be started again.
3.  **Manual entry of the document in the FinAc**
    If an affected invoice/credit was already transferred to the customer and the correction affects the invoice amount, the invoice/credit can no longer be corrected after the fact in AWE. The document has to be entered manually in the FinAc.

See also AWDesk #451277

### 14.3. DB connection problems

**Error handling in case of DB connection problems (AWDesk #410539)**
It is now ensured in Version 6 of the FinAc service that in case of connection problems for a configured DB, all other DBs not affected will be worked through. For this purpose, the problematic DB connection is removed temporarily from the list of DBs to be worked through. After expiry of the next polling interval, it is checked again for the problematic DB whether a connection is possible again. With this logic, the service is not sensitive to temporary DB problems. In case of incorrectly configured/non-accessible databases, the faulty connection will generate an error entry in the log in each polling cycle and thus inflate it. It is therefore recommended that you delete or deactivate non-functional DB configurations in the config tool.

### 14.4. Temporary database problems/network problems/Informix error

See chapter "FinAc Service - automatic restart after abort due to error".

### 14.5. Interruption of the service without error message in the log

Check in the Event Viewer whether there are indications about the cause of the interruption.
Under some circumstances, the virus scanner can be responsible for this.

### 14.6. Error in rounding correction

Message in FinAc service log:
`FibuBeleg.CheckMakeRoundingCorrectionItems(): Net: final amount <...>, rounded accounting items sum <...>, diff ... => rounding correction failed - not enough accounting items to correct.`

**Possible cause:**
There is a not redistributed discount/surcharge, but the env variable `FIBU_RABATT` is not active.
See PF [AW-222523].

## 15. Statistics - Intrastat export

Currently (as of June 2022), the function of the Intrastat message for **Germany** and **Austria** is made available via the AWE FinAc Service. The report files are generated by the FinAc Service in the specified format and written to a configurable directory. The transfer of the report data to the statistics authority is the customer's obligation.

**Intrastat message Germany**
The functionality of the Intrastat message - message about trade with partners in other European countries to the Stat.BA of companies headquartered in Germany - was implemented with [AW-84955] + [AW-98004] and made available via the AWE FinAc service.
xml transfer files in the Intrastat format (INSTAT/SML version 6.3.1) are generated.
The message data is provided by A+W Enterprise in the table `intrastat` and processed by the AWE FinAc service. The export files are made available in a configurable directory.
All information about the legal specifications of the Intrastat message are on the Internet page of the German Federal Statistics Office. In particular, also in the document `https://www-idev.destatis.de/idev/doc/intra/doc/Intrahandel_Leitfaden.pdf`

**Intrastat message Austria**
The functionality of the Intrastat message - message about trade with partners in other European countries to the STATISTIK AUSTRIA of companies headquartered in Austria - was implemented with [AW-103173].
Transfer files in the character code "iso-8859-1" are generated.

### 15.1. Documentation

The general description of the Intrastat interface in A+W Enterprise up to the booking of the table `intrastat`, including master data configuration and operation, is found in the separate configuration instructions for A+W Enterprise "A+W Enterprise Intrastat XML Connector" on Sharepoint.
Customer-specific features of the Intrastat interface are described in a separate chapter in the respective documentation of the customer's FinAc interface documentation.

**General information**
Corrections to statistical authorities, e.g. credits, essentially have to be created manually since the correction messages have to be marked as a clear copy of the original message. Furthermore, the various exception rules cannot be mapped by the system.

### 15.2. Installation

#### 15.2.1. DB scripts

For the Intrastat functionality, the table `intrastat` was expanded and the table `intrastatok` recreated.
Therefore, the following DB scripts must be executed:
- `srvalcib\develop\alcib\14\0\de\install\xsql\13\0\4\130004168_intrastat.sql`
- `srvalcib\develop\alcib\14\0\de\install\xsql\13\0\4\130004171_intrastatok.sql`
- `srvalcib\develop\alcib\14\0\de\install\xsql\13\0\4\130004173_intrastat.sql`
- `srvalcib\develop\alcib\14\0\de\install\xsql\13\0\4\130004174_intrastatok.sql`

### 15.3. Configuration

#### 15.3.1. AWE environment variables

| Name | Description | Note |
| :--- | :--- | :--- |
| `INTRASTAT_RECEIVER` | Market partner number of the Intrastat message recipient. In Germany, the message recipient is the German Federal Statistics Office; in other EU countries, the corresponding official office. Site-specific entry possible. | Only Intrastat message Germany and Slovakia. |
| `INTRASTAT_MATNR` | Material number (= interchange agreement ID). The material number (a five-digit alphanumeric character string) in Germany is assigned by the Federal Statistics Office; in other EU countries by the corresponding official office. It identifies the approval of the message in xml format for the sender. Site-specific entry possible. | Only Intrastat message Germany and Slovakia. For the Intrastat message Austria, a freely selectable file name prefix can be stored for the generated message file. If no value is stored, the prefix "INTRA" is used. |
| `INTRASTAT_SENDER_ID` | Identifier (ID number) of the Intrastat sender/reporter. The structure of this number is specified by the StBA in Germany; in other EU countries by the corresponding official office. For detailed information about the structure, see chapter "Special data transfer", keyword "Identifier". Site-specific entry possible. | Only Intrastat message Germany and Slovakia. |

#### 15.3.2. A+W Enterprise Master Data

Master data for message recipients is only relevant for Intrastat message Germany and Slovakia.

**Intrastat message recipient Germany (German Federal Statistics Office)**
In Germany, the Intrastat message recipient is the German Federal Statistics Office; in other EU countries, the corresponding official office.
This recipient is stored with name and address in the market partner master data as MP type "Other" (`kuliflag=2`).
The market partner number is entered in the env variables `INTRASTAT_RECEIVER`.

#### 15.3.3. FinAc Service Config Tool

All dialogs of the Config tool are described in the installation instructions.
In this chapter, they will only be discussed in excerpt in order to point out special features.

**Common Settings**
FinAc interface and Intrastat interface can be configured on this dialog independently of one another.
Customer can use the Intrastat interface without operating a FinAc interface via the FinAc Service.
The general configuration of the FinAc and Intrastat interface version is stored in the "common settings". This setting can be adjusted/overwritten again site-specifically in the "site settings".
Which setting should be selected for the Intrastat interface is described in the respective chapter "Intrastat functionality <country>".
With **Lock Limit (records)**, the number of records can be specified from which an exclusive lock is placed on the table `intrastat` during processing. For a precise description of the lock logic, see the separate chapter.

**Intrastat export settings**

| Description | Field type | Description |
| :--- | :--- | :--- |
| Export Intrastat | Checkbox | General activation of the intrastat export |
| Use Site Folders | Checkbox | Activation of the storage in site-specific subfolders |
| Export Root Path | Path | Root path for the generated files |
| Clean-up Time | Number of days | The "Clean up Time" must be specified so that the records from `intrastatok` are retained long enough so that any required additional message to the German Federal Statistics Office can be sent. |

**Site Properties**

| Description | Field type | Description |
| :--- | :--- | :--- |
| Active Connection | Checkbox | Activation of the site connection |
| AWE Site | Numeric | AWE site number |
| Intrastat export | Checkbox | Site-specific activation of the Intrastat export |
| Test | Checkbox | Site-specific activation of the test mode for the Intrastat export. In test mode, successfully processed data records of the table `intrastat` are marked with the special status "98". They are not pushed into the table `intrastatok`. To process them again, they must be updated by hand to status "0". |
| Intrastat interface version | Combo box | Site-specific configuration of the Intrastat interface version. |
| SQL Explain | Checkbox | DB-specific activation of the DB log, e.g. for the analysis of performance problems. |

**Subsite Properties**

| Description | Field type | Description |
| :--- | :--- | :--- |
| Active Subsite | Checkbox | Activation of the subsite connection |
| AWE Main Site | Numeric | AWE main site number |
| AWE Subsite | Numeric | AWE subsite number |
| FinAc Site | Numeric | FinAc subsite number |
| Overwrite Main | Checkbox | Activation of the subsite-specific Intrastat configuration. |
| Intrastat export | Checkbox | Subsite-specific activation of the Intrastat export |
| Test | Checkbox | Subsite-specific activation of the test mode for the Intrastat export. In test mode, successfully processed data records of the table `intrastat` are marked with the special status "98". They are not pushed into the table `intrastatok`. To process them again, they must be updated by hand to status "0". |
| Intrastat interface version | Combo box | Subsite-specific configuration of the Intrastat interface version. |

**Remarks**:
A file transfer via FTP is currently not implemented.

#### 15.3.4. Scripts

Scripts are made available in the cmd directory with the help of which the user can change the status of data records in the table `intrastat` and start the export of Intrastat data. Starting the export is done regardless of the daily or monthly starting point configured in the Config tool of the FinAc service.
A script call must be created in the individual programs.
An AWE FinAc service must be installed and configured so that the export can be done.

**Warning**: If a script parameter of the type "date" is transferred, the date must absolutely be specified in the format "dd.mm.yyyy".

**Script "intrastatinitexport"**
The script starts the immediate Intrastat export in that the records in the table `intrastat` to be exported are marked with the status "-1".
**Attention**: Data records that are in the table `intrastat` with the status "1" or "98" are not updated by the script. They must be updated manually in order to process them again.
The script can be called in different modes, that is, with different parameters.

| Mode | Parameter | Description |
| :--- | :--- | :--- |
| 1 | `[hausnr] -si [auftrnr]` | Intrastat export for a defined SA invoice number. `si` = "sales invoice", `[auftrnr]` -> `intrastat.auftrnr` |
| 2 | `[hausnr] -pi [auftrnr]` | Intrastat export for a defined PU invoice number. `pi` = "purchase invoice", `[auftrnr]` -> `intrastat.auftrnr` |
| 3 | `[hausnr] -d1 [datum]` | Intrastat export for a defined invoice date. `[datum]` -> `intrastat.melddat` |
| 4 | `[hausnr] -d2 [datum1] [datum2]` | Intrastat export for a defined invoice period. `[datum1]` -> from `intrastat.melddat`, `[datum2]` -> to `intrastat.melddat` |

**Script "intrastatrecover"**
The script obtains the data for a defined period from the table `intrastatok` back into the table `intrastat`. The data records obtained remain in `intrastatok` and then have the special status "299". In the table `intrastat`, they have the status "0". To export the records directly, the script "intrastatinitexport" must also be called.

| Parameter | Description |
| :--- | :--- |
| `[hausnr] [datum1] [datum2]` | Retrieval of the data from `intrastatok`. Export for a defined invoice period. `[datum1]` -> from `intrastatok.melddat`, `[datum2]` -> to `intrastatok.melddat` |

**Attention**: There are particular scenarios in which executing the script "intrastatrecover" causes problems. If for a reporting period, there are already records with status 99 in `intrastatok` and after that the records are generated in `intrastat` again for this reporting period via the rebooker and the intrastat report is executed, there are doubled records in the table `intrastat` if the script "intrastatrecover" is executed. To prevent the problem, before the run of the rebooker or the generation of the intrastat report, the existing records with status 99 for the reporting period in question must be removed (deleted) from `intrastatok`.

### 15.4. Transfer table intrastat

The table `intrastat` is the transfer table for the Intrastat export. Only invoice items that are listed in this table are taken over into the export file.
Successfully processed records are transferred to the back-up table `intrastatok`.

| Field name | Data Type | Description | From DB field | Comment |
| :--- | :--- | :--- | :--- | :--- |
| melddat | date | Message date | kauf.edat | Attention: Items of an order must belong to the same reference period (period/month)! See notes. |
| auftrnr | integer | SA/PU invoice number | kauf.auftrnr | |
| lfdpos | smallint | Item number | kpos.lfdpos | |
| land | char(10) | COUNTRY | kauf._oadrnr/kauf._ladrnr -> adr.kfzcode -> xland.intracode | StBA key (corresponds to ISO Alpha 2 code). For dispatch: Country of destination, generally customer's country. Caution: For receipt: Dispatching country, generally supplier's country. |
| region | smallint | Reg. No | xhaus.kunr -> mp.region | StBA keys. For dispatch: sender's region. For receipt: goods recipient's region -> generally region of the site. |
| geschart | smallint | Type of business | kauf._reklamart -> xxrart.intrageschart | StBA key. If no key is stored, a default value is used: kauf.nettototal > 0 => Default 11 (= final purchase/sale), kauf.nettototal = 0 => Default 12 (= trial shipment). |
| verkehr | smallint | Mode of transport | xversand.intraverkehr | StBA key. If no key is stored, the default value 3 (= road transport) is entered. |
| warennr | integer | Product number | kpos.artnr -> artikel.intrastat | |
| ursprl | char(10) | Country of origin | kauf._oadrnr/kauf._ladrnr -> adr.kfzcode -> xland.intracode | StBA key (corresponds to ISO Alpha 2 code). Country of manufacture. |
| process | integer | Statistical process | Hard-coded in source code. 10000 = dispatch, 43000 = receipt. |
| gewicht | decimal(8) | Item weight | kpos.gewicht | in kg |
| me | smallint | Measurement | kpos.artnr -> artikel.intrastat/intrawar.warennr -> intrawar.me | AWE measurement |
| phymestk | decimal(10,2) | | kpos.phymestk * kpos.berechnet | |
| betrag | money(10,2) | | kpos.erloes | In company currency |
| statwert | money(10,2) | Revenue + transport surcharge (%) from xversand.intrsatz or intratransp.intrasatz if TRANSPORTZU_LIEF is active | kauf.versandart -> xversand.intrasatz | In company currency |
| haus | smallint | Site | kauf.hausnr | |
| aufnr | integer | Internal order number | kauf.aufnr / kpos.aufnr | |
| subnr | smallint | Sub number | kauf.subnr | For partial invoices |
| private1 | integer | Firma/Company | kauf.company | |
| private2 | integer | | kaufprvfld.longval2, setid = 5 | |
| private3 | integer | | kaufprvfld.longval3, setid = 5 | |
| private4 | integer | | kaufprvfld.longval4, setid = 5 | |
| status | smallint | Status | | NEW: Processing status of the data record. Possible values are found in a separate list in this document. |
| izeit | datetime | | | Insert time stamp |
| uzeit | datetime | | | Update time stamp |
| serviceid | char(40) | | | NEW: ID of the FinAc service that processes the record. |
| versuche | smallint | | | Number of processing attempts |
| itemnum | smallint | Item number (within a declaration) in the XML file | | NEW: Field for saving the "itemNumber" under which the data record is found in the xml file (in combination with "declarationld") |
| xmldatei | char(100) | File | | File name of the xml file in which the data record was written. For sorted-out records due to the Great Britain special logic, the note "Non-EU". |
| declarationid| smallint | Declaration number in the XML file | | Field for saving the "declarationld" under which the data record is found in the xml file (in combination with "itemNumber") |

### 15.5. Status values in the table intrastat

#### 15.5.1. Status -2 - 99: progress status

| No. | Status | Description |
| :--- | :--- | :--- |
| -999 | Marked internally | Status that is used by AWE support in order to exclude records from processing manually. |
| -2 | OnHold | The data record is waiting. It was set to this status because in other records of the same reference period or for the same invoice (depending on customer configuration) errors were found that prevent the export. It can only be exported when all incorrect data records have been corrected. |
| -1 | StartImmediatly / Urgent | Data record is ready for immediate processing. |
| 0 | Waiting | Data record is ready for processing at the specified time -> see configuration in the Config tool of the FinAc service. |
| 1 | InProcess | Data record is being processed by FinAc service now. |
| 98 | Success (Test) | Data record processed successfully in test mode. The record will NOT be pushed into the table intrstatok. |
| 99 | Success | Data record processed successfully. |

#### 15.5.2. Status 100 – 199: incorrect intrastat data

| No. | Status | Description |
| :--- | :--- | :--- |
| 101 | UnspecificError | Unspecific error. |
| 111 | ProductNumberMissing | Product number missing (intrastat.warennr). |
| 112 | VatNumberMissing | VAT number missing (kauf._steuernr) of the goods recipient for goods dispatch. |
| 113 | OriginCountryMissing | Country of origin missing (intrastat.ursprl) of the goods for goods receipt. |

#### 15.5.3. Status 200 – 299: miscellaneous

| No. | Status | Description |
| :--- | :--- | :--- |
| 271 | ErrorCreatingExportFile | The file could not be written. If a network path is accessed, the path must be specified in UNC notation in the config tool. No network drive letter may be used in the path specification. Additional possible cause: error in the XML format. In this case, the log file provides additional notes about the cause of the error. |
| 299 | Recovered | Attention: This status only occurs in the table `intrastatok`. It indicates that the data record from the back-up table was copied back into the transfer table `intrastat`. Copying is done by a script. Records copied back are retained in `intrastatok` nonetheless and are marked with this status. |

### 15.6. intrastatok back-up table

All successfully processed records from the table `intrastat` are backed up in the table `intrastatok`. The structure is very similar to the table `intrastat`. The field "versuche" is missing.

The backed up data can be important if the German Federal Statistics Office demands another Intrastat message for a reference period already reported. In this case, the records backed up must be unloaded with a qualified unload from the table `intrastatok` and re-loaded into the table `intrastat`.

For this functionality, a script (`intrastatrecover`) is made available by A+W, which can be called up via the individual programs.

### 15.7. General functions

#### 15.7.1. Export file path/directory

The export file path is determined according to the configuration in the Config tool of the FinAc Service. The "Export Root Path" is stored there and it is specified whether site-specific subdirectories should be created ("Use Site Folders"). Below the path determined this way, a subdirectory for the year is created by default.

Example for a possible export directory (Root Path/Site/Year):
`"C:\IntrastatExport\05\2022"`

The export directory is generated automatically by the FinAc service if it doesn't already exist.

#### 15.7.2. Treatment of non-redistributed discounts

In the standard logic, the non-redistributed discounts are distributed percentage-wise according to the item amounts (`intrastat.betrag`) across the items to be exported and added to or subtracted from the invoice amount in the export file.

#### 15.7.3. Handling of Intrastat items with special product numbers

**Product number -9999**
Items that are in the table `intrastat` with the product number -9999 are not written to the export file and are thus not reported to the statistics authority.
The product numbers can, for articles that should not be reported to the statistics authority, be stored in the article master data (`artikel.intrastat`).
See also [AW-111829].

#### 15.7.4. Error handling

Incorrect data records in the table `intrastat` are marked with a status >= 100.

A data record in the table `intrastat` always refers to exactly one invoice item (`intrastat.subnr = 0`) or partial invoice item (`intrastat.subnr > 0`). Intrastat data records for an invoice/partial invoice are always exported completely or not at all. If an error occurs in a data record for an invoice/partial invoice, all items from this invoice/partial invoice are excluded from the export until the error is corrected.

In order to avoid the generation of an unnecessary number of files (multiple reports) of a sender for one and the same time period, in the standard logic, only one file is generated if all intrastat data records in this batch are error-free. As soon as an error occurs in a data record of an invoice, the export file is not generated.

All error-free invoices wait for the next run after the error is eliminated. The waiting records are marked with the status "-2". For the next run, all records to be booked must be updated to the status "0" or "-1".

On customer request, the logic can be adjusted so that in a run an export file is generated for all invoices with error-free data records and only the data records remain for which incorrect invoice items were found.

#### 15.7.5. Data check

The error status values described in the chapter "intrastat table" indicate which data checks the FinAc service undertakes. Here's an overview table.

| Description | Status | Comment |
| :--- | :--- | :--- |
| Missing product code | 111 | Product code is mandatory. |
| Missing VAT number | 112 | The trade partner's VAT number must be specified for export of goods starting in January 2022. |
| Missing country of origin | 113 | The country of origin must be specified for export of goods starting in January 2022. |

**Treatment of Intrastat data records with zero amount**
Data records with zero amounts are skipped and thus not written to the report file.

**Special logic for trade partners in Northern Ireland and Great Britain except for Northern Ireland**
Despite Brexit, Northern Ireland will be treated like an EU member state with regard to trade statistics. However, in the current AWE data structure, Great Britain (including Northern Ireland) is assigned only precisely one data record for specification of the country ID (`xxland.kfz`, `xxland.intracode`).

With an entered Intrastat country code (`xxland.intracode`), the trade partner is marked for the Intrastat message. Here, there can also be no distinction between the rest of Great Britain and Northern Ireland. Invoice items for trade partners in Great Britain and Northern Ireland land equally in the transfer table `intrastat`. For this reason, the intrastat data records are not checked by the FinAc service after the fact.

The Stat.BA has declared the special country code "XI" for Northern Ireland. The country code for Great Britain is "GB". For both country codes, the FinAc service checks whether the delivery address (in case of non-existent delivery address the market partner address) is in Northern Ireland. The check is done using the postal code. All postal codes in Northern Ireland begin with the letter combination "BT". Deliveries from and to Northern Ireland are taken over into the Intrastat message. All other deliveries from and to Great Britain (except for Northern Ireland) are sorted out and transferred into the archive table `intrastatok`.

The sorting is also done if in the pass no xml file is generated due to other data errors. Sorted out intrastat records with trade partners in Great Britain (except for Northern Ireland) will be removed from the table `intrastat` and written to the table `intrastatok`. For these data records, the note "Non-EU" is stored in the field "xmldatei".

**Different Intrastat versions in the multisite system**
In multisite systems, it is possible that the main site is assigned to another country than the subsite(s) and that a different, non country-specific Intrastat booking/version is configured with the Config tool of the AWE FinAc service.
In this case, the Intrastat key of your own country (main site) must be stored in the country keys. (see also the configuration instruction "A+W Enterprise Intrastat XML Connector") In this case, bookings (table `intrastat`) within your own country are detected and sorted out after the fact before the Intrastat file is generated.
See also PF [AW-158197].

#### 15.7.6. Cleanup - data cleansing

The cleanup time (in days) can be configured in the Config tool. If the cleanup time is not configured, the value "100 days" will be used as the default.

**Table intrastatok**
The back-up records in the table `intrastatok` are deleted if the configured "cleanup time" is reached.
As reference for the "Cleanup time", the time stamp in `intrastatok.uzeit` is used. This is the time at which the record was written to the table `intrastatok`.

#### 15.7.7. Sending e-mails

If errors occur when exporting the Intrastat data, the information about the errors found will be sent in an info e-mail.

The e-mail configuration is done via the Config tool of the FinAc service. If it is necessary to design the recipient e-mail address site-specifically, the placeholder "$SITE$" can be stored as recipient. The placeholder is replaced with the current site number when sending. Here, a leading "0" is used for single-digit site numbers.

Per site and export period, precisely one e-mail will be sent.
The e-mail is in English. At the moment, there is no other language choice available.

**E-mail in case of non-existent export data**
If at the time configured or triggered via script of the Intrastat export there is no export data (table `intrastat`), an info e-mail is sent that says that there was no export data at the time of processing.
The e-mail specifies the time of processing and the client affected.

**Note**:
Information with regard to the export time (period) cannot be specified in the e-mail. The export period arises from the export data in the table `intrastat`. If there is no export data present, the information about the time period is also missing.
Available with AWE FinAc Service - build 13.4.11225.
See PF [AW-216782].

#### 15.7.8. Lock logic (exclusive lock intrastat)

**Caution**: This logic cannot be configured (as of 06/14/2022). The logic may only be activatable if adjustments were made to the AWE Backend that prevent the booking of an invoice if during the generation of the data records required for an invoice in the table `intrastat` the access (insert) to this table is not possible. Currently, an error during insert is ignored and the invoice is booked nevertheless.
See PF [AW-113125].

> *The following description is not yet valid (as of 06/14/2022).*
> In the Config tool of the FinAc Service, the possibility is provided to select the database precisely whether during processing of the Intrastat message the table `intrastat` should be locked exclusively. If the exclusive lock is activated, the program logic also evaluates the "lock limit," that is, the lower limit of data records in the table `intrastat`. This value can also be configured in the Config tool. Only if the number of records in the table `intrastat` is over the limit is the table `intrastat` actually exclusively locked.
> The possibility of the exclusive lock was provided since an analysis showed that there are customer systems with which data record quantities in the 5-digit range (> 10,000) are created each month in the table `intrastat`. The exclusive lock unburdens the database with regard to locks and logs.

#### 15.7.9. Notes

**Message date - intrastat.melddat**
Since intrastat records are not just generated automatically, but can also be changed manually or entered anew, attention must be paid that all items of an invoice have the same message date (or at least the same reference period (=period/month)).
The FinAc service cannot currently handle invoices whose items belong to different reference periods. In this case, the message date of the first selected item forms the basis for the reference period for all following items of an invoice.

### 15.8. Intrastat Germany function

The initial implementation was done with ticket [AW-84955].
The generation of the document is implemented as "self-reporter" (`partyType="PSI"`).
An xml file is generated. For the description of the xml structure, see the next section "Data Mapping."

#### 15.8.1. Configuration

In order to use the default Intrastat interface Germany, the Intrastat interface "Intrastat_6.3.1_DE_001" must be selected in the Config tool.

#### 15.8.2. Data mapping

The data mapping is based on the interface description of the German Federal Statistics Office (`https://www-idev.destatis.de/idev/doc/intra/hilfe6_2_1.html`) in combination with the key directory (SVZ) of the German Federal Statistics Office (`https://www-idev.destatis.de/idev/doc/intra/hilfe6_3.html`).

The xml version Intrastat 6.3.1 is used.
Validity start January 2022.

**XML prologue:**
`<?xml version="1.0" encoding="ISO-8859-1"?>`
Only character set ISO-8859-1 is allowed.

| Intrastat xml element | Data type / Flag | Description | AWE DB field | Comment |
| :--- | :--- | :--- | :--- | :--- |
| `<INSTAT>` | M | 1. Root element | | |
| `<Envelope>` | M | 2. Root element | | |
| `envelopeId` | string / ? | Message ID | Material number from `INTRASTAT_MATNR` | `matnr` + `-` + `refbzr` + `-` + `datum` + `-` + `uhrzeit`. See "special data determination" |
| `<DateTime>` | | | | |
| `date` | string / ? | Date of the document generation | | yyyy-mm-dd |
| `time` | string / ? | time | | hh:mm:ss |
| `</DateTime>` | | | | |
| `<Party partyType="CC" partyRole="receiver">` | M | Participants: Recipient | env variable `INTRASTAT_RECEIVER` -> mp.mpnr | See "special data determination". The only possible recipient is the German Federal Statistics Office with identifier "00". |
| `partyId` | string / M | Identifier | fix „00" | |
| `partyName` | string / M | | mp.name | |
| `<Address>` | M | Address | | |
| `streetName` | string / M | Street | mp.str | |
| `streetNumber` | string / ? | Site Number | mp.str (number) | |
| `postalCode` | string / M | ZIP code | mp.plz | |
| `cityName` | string / M | City | mp.ort | |
| `countryName` | string / M | Country | mp.land | |
| `</Address>` | | | | |
| `</Party>` | | | | |
| `<Party partyType="PSI" partyRole="sender">` | M | Participants: Sender | Client -> xhaus.kunr -> mp.mpnr | See "special data determination" |
| `partyId` | string / M | Identifier | `INTRASTAT_SENDER_ID` | See "special data determination" |
| `partyName` | string / M | | mp.name | |
| `interchangeAgreementId` | string / M | MUST only for sender | Material number from `INTRASTAT_MATNR` | |
| `<Address>` | M | Address | | |
| `streetName` | string / M | Street | mp.str | |
| `streetNumber` | string / ? | Site Number | mp.str (number) | |
| `postalCode` | string / M | ZIP code | mp.plz | |
| `cityName` | string / M | City | mp.ort | |
| `countryName` | string / M | COUNTRY | mp.name | |
| `</Address>` | | | | |
| `</Party>` | | | | |
| `softwareUsed` | string / ? | Application with which the document was generated | fix: "A+W Enterprise 6 FinAc Service" | Entry generated by the program |
| `<Declaration>` | M | Message with as many items as desired, which describe transactions with individual product codes. | | One declaration per period (month) and transport direction (receipt/dispatch). Attention: The reference period is also in the `envelopeId` (bzr), therefore always only one declaration per transport direction in an envelope or a file! |
| `declarationId` | string / ? | Message ID | Sequential number beginning with 1 | |
| `<DateTime>` | | Timestamp | | |
| `date` | string / ? | Date of the declaration generation | | yyyy-mm-dd |
| `time` | string / ? | Time of the declaration generation | | hh:mm:ss |
| `</DateTime>` | | | | |
| `referencePeriod` | string / M | Reference period; year and month in which the internal goods traffic took place. | Month and year from `intrastat.melddat` | yyyy-mm |
| `PSIId` | string / M | Identifier of the reporter. | `INTRASTAT_SENDER_ID` | See "special data determination" |
| `<Function>` | M | Function of the message | | |
| `functionCode` | string / M | Function key. For the German intra-trade statistics, only the specification of the capital letter "O" is provided. | fix „O" | |
| `</Function>` | | | | |
| `flowCode` | string / M | Transport direction. Receipt= A, Dispatch= D | | Derived from `intrastat.verfahre`n: 10000 = dispatch => D, 43000 = receipt => A |
| `<Item>` | ? | Individual item | | Per combination product code + invoice number |
| `itemNumber` | string / M | Document no. Sequential document number beginning with 1. | | |
| `<CN8>` | M | Product information | | |
| `CN8Code` | string / M | 8-digit product code from the product index for the external trade statistics `https://www.destatis.de/warenverzeichnis` | `intrastat.warennr` | |
| `SUCode` | string / ? | Unit of the sub quantity. InSU specified quantities (currently not analyzed) | `intrastat.me` -> `xme.kurzbez` | |
| `</CN8>` | | | | |
| `MSConsDestCode` | string (SVZ) / M | Destination/dispatch country | `intrastat.land` | For dispatch: Country of destination, generally customer's country. Caution: For receipt: Dispatching country, generally supplier's country. According to SVZ (corresponds to ISO Alpha 2 code) |
| `countryOfOriginCode` | string (SVZ) / M | Country of origin | `intrastat.ursprl` | Country of manufacture. According to SVZ (corresponds to ISO Alpha 2 code) |
| `netMass` | string / ? | Own weight in full kg. Specification not required if special dimension unit must be specified. | `intrastat.gewicht` | Value will be rounded commercially. If '0', it is set to '1' to avoid error. [AW-105142] |
| `quantityInSU` | string / ? | Quantity in the special dimension unit. | `intrastat.phymestk` | Value will be rounded commercially. If '0', it is set to '1' to avoid error. [AW-105142] |
| `invoicedAmount` | decimal / ? | Invoice amount in full euros. | `intrastat.betrag` | Type of the business according to SVZ. Value will be rounded commercially. If '0', it results, it is set to '1' to avoid error. [AW-105142] |
| `statisticalValue` | decimal / ? | Statistical value, to be specified if a specified value threshold is exceeded. | | See "special data determination" |
| `invoiceNumber` | string / M | Invoice number | `intrastat.auftrnr` | |
| `partnerId` | string / M | VAT identification number of the goods recipient | `kauf._steuernr` | Only mandatory for goods dispatch. Transfer from `mp.steuernr`. |
| `<natureOfTransaction>` | M | Type of business | | |
| `natureOfTransactionACode` | string (SVZ) / M | Type of business, key number 1st digit | 1st digit of `intrastat.geschart` | according to SVZ |
| `natureOfTransactionBCode` | string (SVZ) / M | Type of business, key number 2nd digit | 2nd digit of `intrastat.geschart` | according to SVZ |
| `</natureOfTransaction>`| | | | |
| `modeOfTransportCode` | string (SVZ) / M | Mode of transport | `intrastat.verkehr` | according to SVZ |
| `regionCode` | string / M | Region of origin / Destination region | `intrastat.region`. If `intrastat.region` = 0, `mp.region` (sender region from master data) [AW-108450] | according to SVZ |
| `</Item>` | | | | |
| `</Declaration>` | | | | |
| `numberOfDeclarations` | string / ? | Number of messages in envelope | | |
| `</Envelope>` | | | | |
| `</INSTAT>` | | | | |

#### 15.8.3. Export file name

One file per period (month) is generated. Both goods shipments and goods receipts are included in this file.
The name of the xml export file corresponds to the "envelopeld" with file extension ".xml".
The name of the export file is specified by Stat.BA. According to information from Stat.VA from 01/27/2022, it is urgently recommended that you not change the file name.

> "When uploading the files via IDEV, there is no checking of the specified file name. It is anticipated that in the middle of the coming year, the upload process will change (you will be informed in due time). Which checks are made then is not yet certain. Therefore, we would like to recommend that you specify the file name as intended."

#### 15.8.4. Special data determination

**Participant "recipient" (`<Party partyType="CC" partyRole="receiver">`)**
The Intrastat message recipient is the German Federal Statistics Office. The address data of the message recipient is determined from the market partner (type "other"), which is stored in the env variable `INTRASTAT_RECEIVER`.

**Participant "Sender" (`<Party partyType="PSI" partyRole="sender">`)**
The Intrastat message sender is the site for which the file generation is configured.
The `partyType="PSI"` indicates that this is a self-reporter.
The message sender's address is drawn from the MP master data. The market partner number is determined from the table `xhaus`. For the current site, the stored `xhaus.kunr` will be selected.

**Identifier (PSIId, partyId)**
The identification of the sender (`partyType` = PSI or TD) is done using a 16-digit identifier (ID number), which is composed of the key of the federal state of the Ministry of Finance (Bu/FA), the 10 or 11-digit VAT number (UstVA), a "0" for 10-digit VAT number and the 3-digit distinguishing number.
The identifier is stored in the environment variable `INTRASTAT_SENDER_ID`. The stored value should be checked precisely again by the customer with initial configuration of the Intrastat message:
- in total 16 digits
- Start with 2-digit key of the federal state of the responsible Ministry of Finance (Bu/Fa according to key index)
- Then 10 or 11-digit VAT number (UstVA), a leading "0" for 10-digit VAT number so that the VAT number always has 11 digits
- Then 3-digit distinguishing number (will be assigned by the Ministry of Finance), if none present, then three "0s"
All information about this is made available by the Stat.VA: `https://www-idev.destatis.de/idev/doc/intra/doc/Intrahandel_Leitfaden.pdf`

**Statistical value `<statisticalValue>`**
Excerpt from `https://www-idev.destatis.de/idev/doc/intra/doc/Intrahandel_Leitfaden.pdf`
> **Feld Statistischer Wert**
> Dieses Feld muss grundsätzlich nicht ausgefüllt werden, wenn es sich bei der Warentransaktion um einen Verkauf (Schlüssel 11 und 12 in Feld Art des Geschäfts) oder ein Kommissions-, Konsignations- oder Lagergeschäft (Schlüssel 31 und 32 in Feld Art des Geschäfts) handelt und der Gesamtwert der entsprechenden Versendungen im Vorjahr 45 Mill. Euro nicht überstiegen hat.

In the standard logic (status as of 03/11/2022), NO statistical value is written to the Intrastat message file. If a deviating logic is required, it must be programmed customer-specifically.
See also PF [AW-105440].

#### 15.8.5. Data check

The error status values described in the chapter "intrastat table" indicate which data checks the FinAc service undertakes. Here's an overview table.

| Description | Status | Element in the export file | Comment |
| :--- | :--- | :--- | :--- |
| Missing product code | 111 | CN8Code | Product code is mandatory. |
| Missing VAT number | 112 | partnerId | The trade partner's VAT number must be specified for export of goods starting in January 2022. |
| Missing country of origin | 113 | countryOfOriginCode | The country of origin must be specified for export of goods starting in January 2022. |

About the changes starting in 2022, see also:
`https://www-idev.destatis.de/idev/doc/intra/doc/Leitfaden_Aend_AHStat_2022.pdf`

**Treatment of Intrastat data records with zero amount**
Items with zero amounts are not accepted by Stat.BA. Data records with zero amounts are skipped and thus not written to the report file.

#### 15.8.6. Notes

**Multiple reports for one and the same reference period**
The Stat.BA has specified on request on 01/27/2022 that several Intrastat messages in the form of several files can be updated for a reference period.
A configuration with a daily generation is then conceivable, with which approx. 30 small files will be uploaded at the end of the month instead of one large file.

### 15.9. Intrastat Austria function

The initial implementation was done with ticket [AW-103173].
A flat/text file in the character code "iso-8859-1" is generated. The file has the extension "asc".
For the data record description, see the next section "Data Mapping."
The dollar sign `$` is used as field separator within a data record.
Only the comma `,` is permitted as decimal separator.

**Caution**: Since the article designation (`artikel.artbez1`) is transferred in the data record, no dollar sign may be included in this designation.

#### 15.9.1. Configuration

In order to use the default Intrastat interface Austria, the Intrastat interface "Intrastat_2022_AT_001" must be selected in the Config tool.

#### 15.9.2. Data mapping

The data mapping is based on the interface description of Statistik Austria. The documentation can be found on Statistik's website: `https://www.statistik.at/web_de/frageboegen/unternehmen/aussenhandel_intrastat/index.html`.
Validity start January 2022.

| No. | Field name | Data Type | Field length | AWE DB field | Comment |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | KN8 code | String | 8 | `intrastat.warennr` | Product number |
| 2 | Product description | String | 2048 | `intrastat.lfdpos` -> `kpos.artnr` -> `artikel.artbez1` | The transfer of the description is optional. By default, the field is filled by the FinAc Service. The field length is limited to 20 characters, however. |
| 3 | Destination country (export) / Dispatch country (import) | String | 2 | `intrastat.land` | Caution: During import, the sending country is here! |
| 4 | Country of origin | String | 2 | `intrastat.ursprl` | "Country of manufacture" (import and export) |
| 5 | Type of business | String | 2 | `intrastat.geschart` | |
| 6 | Intrinsic weight | Num | 14 | `intrastat.gewicht` | 10 places before the decimal point (maximum), 3 places after the decimal point (precisely). Decimal separator: comma. |
| 7 | Special measurement | Num | 14 | `intrastat.phymestk` | The value can be "0"; it is then transmitted as "0.000". 10 places before decimal, 3 places after. |
| 8 | Invoice amount | Num | 13 | `intrastat.betrag` | 10 places before decimal, 2 places after. |
| 9 | Statistical value | Num | 13 | - | The same value as invoice amount. See "special data determination". 10 places before decimal, 2 places after. |
| 10 | Recipient UID | String | 14 | `kauf._steuernr` | Only for dispatch/export. May not be filled for import. |

#### 15.9.3. Export file name

Two files per period (month) are generated. One file contains the goods shipments, the other file contains the goods receipts for a period.

The file name is generated analogous to the logic for the Intrastat message in Germany. As prefix, the character string "INTRA" is used by default. Through activation and assignment of the env variable `INTRASTAT_MATNR`, the prefix can be changed at customer request.

After that comes the specification of the period in the format `[yyyymm]`.
Then comes the abbreviation "S" or "P": S = Sales (goods shipments), P = Purchase (goods receipts).
After that comes the time stamp in the format `[yyyymmdd-hhMM]`.
The final part is the file extension ".asc". The file is written in the character code "iso-8859-1".

Example:
`INTRA-202110-P-20220523-1022.asc`
`INTRA-202110-S-20220523-1022.asc`

#### 15.9.4. Special data determination

**Statistical value**
Different specifications apply in Austria than in Germany.
According to notes in the documentation from Statistik Austria:
> **Hinweis**: Wirtschaftsbeteiligte, deren Jahresumsatz je Warenstromrichtung die Grenze von 12 Millionen Euro nicht überschreitet, können den Statistischen Wert gleich dem Rechnungsbetrag setzen (nur für die Geschäftsart 1 gültig, bei den übrigen Geschäftsarten ist ein gesonderter **Statistischer Wert** zu ermitteln).

It must be clarified customer-specifically whether another logic must be implemented.

#### 15.9.5. Error handling

The general error handling applies. In addition, it must be noted that for a reference period (period/month), either always both files (for shipments and receipts) must be written or none. That is, if there is an error within the goods shipments, the goods receipts will also not be generated and vice-versa.

#### 15.9.6. Sending e-mails

In the subject line of the info or error e-mail that is sent upon generation of the Intrastat message for Austria, the abbreviation "S" (Sales) or "P" (Purchase) is output. It indicates whether the info/error mail refers to goods shipments (S) or goods receipts (P).

In the info mail, there is an overview of the invoice amounts reported sent to Intrastat. Since Statistik Austria requires the invoice amounts with decimal places, the amounts with places after the decimal are also specified in the e-mail.

### 15.10. Intrastat Slovakia functionality

The implementation was done with ticket [AW-158197].
Slovakia uses a format according to "instat62.xsd". This is a modified form of the instat format that is also used in Germany.
For additional information about format and expression, please see: `https://intrastat.financnasprava.sk/en/index.php?page=xml`

#### 15.10.1. Configuration

In order to use the default Intrastat interface Slovakia, the Intrastat interface "Intrastat_6.2_SK_001" must be selected.

#### 15.10.2. Data mapping

The data mapping is based on the information that is made available by the Slovakian financial authorities under `https://intrastat.financnasprava.sk/en/index.php?page=xml`.

**XML prologue:**
`<?xml version="1.0" encoding="ISO-8859-2"?>`
Character set: ISO-8859-2

*The following table is an extensive data mapping for the Slovakian Intrastat XML format. It is largely similar to the German format, with some fields noted as being stored directly in the source code rather than pulled from AWE DB fields.*

| Intrastat xml element | Data type / Flag | Description | AWE DB field | Comment |
| :--- | :--- | :--- | :--- | :--- |
| `<INSTAT>` | M | 1. Root element | | |
| `<Envelope>` | M | 2. Root element | | |
| `envelopeId` | string / ? | Message ID | Material number from `INTRASTAT_MATNR` | `matnr` + `-` + `refbzr` + `-` + `datum` + `-` + `uhrzeit`. See "special data determination" |
| ... | ... | ... | ... | ... |
| `totalNumberLines` | string / ? | Number of „Items“ | | |
| `totalNumberDetailedLines` | string / ? | Like „totalNumberLines“ | | |
| ... | ... | ... | ... | ... |
| `MSConsDestCode` | string (SVZ) / M | Destination/dispatch country | `intrastat.land` | For dispatch: Country of destination. For receipt: Dispatching country. |
| ... | ... | ... | ... | ... |

*(Note: The full table for Slovakia is very similar to the German one, with minor variations in comments and source fields. Key differences include the character set and some fields being hard-coded.)*

#### 15.10.3. Export file name

See corresponding subchapter in the chapter "Intrastat Germany functionality".

#### 15.10.4. Special data determination

**Participant "PSI" (`<Party partyType="PSI" partyRole="sender">`)**
The Intrastat message sender is the site for which the file generation is configured.
The message sender's address is drawn from the MP master data. The market partner number is determined from the table `xhaus`. For the current site, the stored `xhaus.kunr` will be selected.

#### 15.10.5. Data check

See corresponding subchapter in the chapter "Intrastat Germany functionality".

#### 15.10.6. Notes

See corresponding subchapter in the chapter "Intrastat Germany functionality".

### 15.11. Troubleshooting

**Cannot lock table (awserv.intrastat) in requested mode.**
This error message can occur when executing the scripts `intrastatinitexport` and `intrastatrecover` if a user of A+W Enterprise is on the intrastat booking dialog at the time the script is executed. When the user has closed the dialog, the script can be executed.

### 15.12. Intrastat booking dialog in AWE

The booking dialog for the Intrastat booking records can be reached via the menu System > Statistics Data > Intrastat > Bookings.
For a detailed description of the booking dialog, see the configuration document "A+W Enterprise Intrastat XML Connector" in Sharepoint.

### 15.13. Performance

The larger the data quantity in the table `intrastat` is, the longer the processing with the FinAc Service takes. The last tests (status as of 06/09/2022) have shown that for approx. 10,000 intrastat records, a processing time of approx. 22-25 minutes is normal.
Most time is required for the updating of the data records in the table `intrastat` (2 x 5 minutes) and the selecting of the article data (10-12 minutes).

### 15.14. Additional information for planning and service

Additional important information for planning and service is found in the "Intrastat export" section in the document "AWE FinAc Info Intern.docx" in the interfaces area in Sharepoint.

### 15.15. Termination

**Konfigurationstabelle mp_intrastat (no longer in use!)**
The table `mp_intrastat` contained additional data about the message sender:
- Federal state (StBA key) of the responsible Ministry of Finance
- VAT number of the message sender
- Distinguishing number (addition) for separately reported companies within an organization, assigned by the StBA

The combination of these three values is transferred in the Intrastat xml file as "Identifier" of the sender.
The identifier (sender ID) is now stored completely in the env variable `INTRASTAT_SENDER_ID`.
Therefore the table `mp_intrastat` for which there was no maintenance dialog, is no longer required.
