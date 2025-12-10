---
title: "EN-CONFIG-AW_Business-12"
source: "EN-CONFIG-AW_Business-12.pdf"
tags: ["A+W Business", "ALFAK", "ERP Configuration", "Financial Accounting Interface", "Database Replication", "SQL Server Migration", "CAM Credit Management", "Workflow Automation", "UDF"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical configuration manual for A+W Business (ALFAK) software. It provides detailed instructions on managing production status, automating workflows, configuring interfaces to various financial accounting systems (Brilliant, Datev, Varial, eGecko), setting up credit management with CAM, and managing database replication and migration from SQL Base to SQL Server."
long_description: "This is a comprehensive guide for system administrators and technical consultants configuring the A+W Business (ALFAK) ERP system. The document is divided into major sections covering production management, financial interfaces, and database administration. The production management section details the meaning of status codes in the `BW_LOCK_KAPA` table and explains how to use various user-defined functions (UDFs) to automate status changes and workflow tasks. The financial accounting interface section provides in-depth instructions for setting up data transfers to systems like Brilliant, Datev, Varial, eGecko, and the CAM credit management system, including required settings, formula definitions, and data mapping. The final section focuses on database management, offering a step-by-step guide to setting up and managing data replication between a central headquarters and subsidiary sites, as well as a detailed procedure for migrating databases from SQL Base to Microsoft SQL Server. The document includes numerous screenshots, tables, code examples, and function definitions to facilitate configuration."
---

---
## 11.18. Managing the production status in table BW_LOCK_ΚΑΡΑ

The table BW_LOCK_KAPA contains the field STATUS. It depicts the order status with regard to production. The field can show the following entries:

**Tab. 50: Managing the production status in table BW_LOCK_KAPA**

| Value | Meaning | Action |
| :---- | :--- | :--- |
| 0 | New order entered, or structural changes | Order entry |
| 1 | Transfer to production/planning completed | Transfer to ALCIM/ALCIM Capacity Planning |
| 2 | Order imported in ALCIM Capacity Planning | Manual via workflow* |
| 5 | Planning or report error in ALCIM Capacity Planning | Manual via workflow* |
| 10 | Order ready for production release in ALCIM | Manual via workflow* |
| 11 | Production release sent to ALCIM | Manual via workflow* |
| 12 | Released for production in ALCIM | Workflow Release for Production in ALCIM |

> \*) To change the status manually in table BW_LOCK_KAPA, the function udf_UpdateKapaStatus can be used in a formula.

## 11.19. Structural order changes

Changes of the shipping or production date, all structural changes of an item (e.g. width or height, supply type,..), and all changes of the BOM (shape, processing steps, ...) result in the setting of the order status in the corresponding BW_LOCK_KAPA record to 0 so that it can be transferred again to ALCIM Capacity Planning.

Price changes do not result in an update of the production state in BW_LOCK_KAPA.

## 11.20. Availability on stock

Together with the report from ALCIM Capacity Planning, availability of the articles on stock will be checked.
In case of a shortage of stock, a task will be entered for the user.

The user can double-click on the task to go directly to the order and check the stock availability.

## 11.21. Automatic transfer to statistics, archives, or document deletion

Automatic transfer (to statistics, archives, document deletion) and the archiving of the system log book via VisualBasic script/batch file (auto_eoday.vbs, auto_eoday.bat) are no longer supported; this has been replaced by two work-flow tasks in ALFAK Interface Service (AIS).

### Start-up of the work-flow tasks:
- Update ALFAK Interface Service 2009
- Update the COM objects abcreceive44.exe and abcprocess44.exe
- Update abcstamm.exe
- Update the message file germes.txt (or the appropriate message file)

All of the above elements have to date from 27.11.2009 or later.

### Automatic transfer to statistics and archives:

Define a formula for automatic transfer in formula management
- Example formula: Database DEMO44 or ALF (formula number 9008)
- Example formula: local ALFAK installation in sub-directory Formula (file Workflow_AutomaticTransfer_EndOfDay.txt).
- The example formula will perform the transfer for all document types. By deleting the corresponding lines, the formula can be restricted to certain document types (e.g. only quotations).
- Define the work-flow task by allocating the new formula in Customizing management, tab 3 Work-flow Tasks.
- Define the AIS settings in Customizing management, tab 4 Automatic process execution. Enter a fixed time (e.g. 20:00 for 20:00 h) as an interval/time, and set the execution to "1-fixed time". With these settings, AIS will execute this task daily at 20:00 h.
- Restart AIS
- Reports from the transfer are no longer recorded in text files but are shown on the service monitor
- For a further client (in the same or a different database) add a second section to the AIS configuration. For a second client in the same database, please make sure to limit the ALFAK user to the second client.
  - Increase the setting „BatchUsers“ to „2":
    ```xml
    <add key="BatchUsers" value="2" />
    ```
  - Insert and configure the block „Setting2" for second client analogous to „Setting1":
    ```xml
    <add key="Setting2/DatabaseName" value="demo44" />
    <add key="Setting2/DatabaseType" value="2" />
    <add key="Setting2/DatabaseServer" value="" />
    <add key="Setting2/ALFAKUser" value="sysadm2" />
    <add key="Setting2/ALFAKPassword" value="c3lzYWRt" />
    <add key="Setting2/InstanceName" value="sysadm2" />
    <add key="Setting2/IniFile" value="C:\ProgramData\A+W\ALFAK 2009\abcstart.ini" />
    ```

### Archiving and deletion of the system logbook:
For customers who do not do automatic transfers but still want to archive and delete the system logbook:
- Example formula: Database DEMO44 or ALF (formula number 9009)
- Example formula: local ALFAK installation in sub-directory Formula (file Workflow_ArchiveSystemLogbook.txt).
- Set up like the automatic transfer described above

### Separate deletion of statistics, order info, commission statistics, stock logbook, time management, rack history, EDI back-up files, credit limit snapshots, and history orders:
The deletion of the above-mentioned data is done after the storage days specified in the company master data during the automatic statistic and archive transfer. However, the functionality is also available separately and can be started in an individual workflow task with the function "udf_ClearStatistics." An example is available in the formula "Workflow_ClearStatistics.txt."

## 11.22. Constants and functions used

### 11.22.1. Constants

#### 1. Task/date types
| Constant | Description |
| :--- | :--- |
| TASK_Standard | Standard date |
| TASK_OrderEntry | Date for calling the order entry |
| TASK_AWCapacity | Date as per capacity planning |
| TASK_DokumentsToPrint | Task type printout |
| TASK_DokumentsToFax | Task type fax |
| TASK_DokumentsToMail | Task type email |

#### 2. Document types
| Constant | Description |
| :--- | :--- |
| nMODE_ANGEBOT | Quotation |
| nMODE_AUFTRAG | Order |
| nMODE_GUTSCHRIFT | Credit note |
| nMODE_BESTELLUNG | Purchase orders |
| nMODE_BESTELLANFRAGE | Enquiry |

#### 3. Report types to ALFAK service monitor
| Constant | Description |
| :--- | :--- |
| EV_ERROR | Error report |
| EV_HINT | Note |
| EV_WARNING | Warning |
| EV_RESULT | Result |

#### 4. Production status (saved in BW_LOCK_КАРА)
| Constant | Description |
| :--- | :--- |
| KAPA_NEW_ENTRY | Document entered/changed |
| KAPA_TRANSFERRED | Document transferred to ALCIM |
| KAPA_IMPORTED | Document imported in to ALCIM |
| KAPA_IMPORT_ERROR | Document import caused an error |
| KAPA_READY_FOR_RELEASE | Document ready for production release |
| KAPA_RELEASE_SEND | Production release dispatched |
| KAPA_RELEASE_FOR_PRODUCTION | Document released for production |

### 11.22.2. Functions

#### 1. Adding a task/date

**`udf_addTaskForUser (Task text, Task type, Document Number, Document Type, Employee, Number manager name, Task time)`**

The function enters a date/task in the transferred ALFAK user's task list.

**Return:**
TRUE if the date could be entered or did already exist; otherwise FALSE

**Important:** The task/date will be created only if there had been no task/date existing for the transferred combination of user, task type, and reference.

If `DATETIME_Null` is transferred as expiry time in parameter "Task time", the expiry time will be set to the present date + 1 day.

Reference of the task/date (parameter „Reference") may be the name of a number manager for example. If the parameter „Reference" is left blank, the document number will be entered in the reference field of the task/date.

**Order entry only:**
If the task type is `TASK_DocumentToPrint`, `TASK_DocumentToFax` or `TASK_DocumentToMail` and a number manager has been transferred as a reference, a double-click on the date/task will call the print program and the number manager.

If the task type is `TASK_AWCapacity` and a document has been transferred as a reference or document number, double-clicking on the date/task will open order entry on this document and the transferred document type.

**Examples for task times:**
- two hours ahead: `SalDateCurrent() + (1/24)*2` (1/24 is 1 hour)
- one day ahead: `SalDateCurrent() + 1`

The user's task list only shows tasks/dates that do not lie in the past.

**Parameter:**
- **Task text**: Text of the task/date for the user
- **Task type**: Task/date type (see constants TASK_XXX)
- **Document number**: Number of a document
- **Document type**: Document type (see constants nMODE_XXX)
- **Employee**: Name of an ALFAK user
- **Reference**: Reference info (e.g. name of the number manager)
- **Task time**: Expiry of the date/task

**Example:**
The user Administrator is allocated a task/date informing him that there are orders to be printed. The date expires in two hours' time. A double-click on the date opens the print program and the number manager, Print'.
```
udf_addTaskForUser('Orders to be printed', TASK_DokumentsToPrint, 0, nMODE_AUFTRAG, 'Administrator', 'Print', SalDateCurrent() + (1/24)*2)
```
The user Administrator receives a task/date informing him that he should check the delivery date of order 1000. The date expires in a day's time. A double-click on the date opens the order entry on order 1000.
```
udf_addTaskForUser('Please check delivery date', TASK_AWCapacity, 1000, nMODE_AUFTRAG, 'Administrator', '', SalDateCurrent() + 1)
```

#### 2. Event to ALFAK service monitor
**`udf_EventToServiceMonitor(Event type, Event message)`**
This function sends a message to the service monitor which appears on the service monitor's message list.

**Parameter:**
- **Event type**: Event type (see constants)
- **Event message**: Event text

**Example:**
```
udf_EventToServiceMonitor(EV_HINT, 'Document 1000 ready for OC')
```

#### 3. Adding a document to a number manager
**`udf_AddDocumentToNumberManager(Number manager name, Employee, Document number, Document type)`**
The document will not be transferred to a number manager. The number manager will be created if it does not exist already for the transferred user.

**Parameter:**
- **Number manager name**: Number manager name
- **Employee**: Name of an ALFAK user
- **Document number**: Number of a document
- **Document type**: Document type (see constants)

**Example:**
```
udf_AddDocumentToNumberManager('PRINT', 'Administrator', 1000, nMODE_AUFTRAG)
```

#### 4. Updating the task list in a program
**`udf_UpdateTasks(Program name)`**
This function updates the list of dates in a program.

**Parameter:**
- **Program name**: Name eines Programms

**Example:**
```
udf_UpdateTasks('abcauftr.exe')
```

#### 5. Check for purchased elements
**`udf_CheckForPurchaseParts(Document status, Status point purchase parts, Status point no purchase parts)`**
This function checks all orders of the transferred status for purchase elements and changes the status to 'purchase elements included' or 'no purchase elements'. The new status is defined by the transferred status points.

**Parameter:**
- **Document status**: Status of the orders to be checked
- **Status point purchase parts**: Status point for included purchase elements. The order will get the allocated status if it contains purchase elements.
- **Status point no purch. parts**: Status point for 'no purchase elements'. The order will get the allocated status if it does NOT contain purchase elements.

**Example:**
```
udf_CheckForPurchaseParts(21, 1029, 35)
```

#### 6. Status increase
**`udf_StatusUpdate(Document number, Status point new)`**
This function raises the order status to the status of the transferred status point. The status will NOT be lowered.

**Parameter:**
- **Document number**: Order number
- **Status point new**: Status point for status increase

**Example:**
```
udf_StatusUpdate(1000, 35)
```

#### 7. ALCIM transfer to production
**`udf_TransferToProduction(Document number, Document type)`**
This function executes a production transfer to ALCIM for the transferred document.

**Parameter:**
- **Document number**: Order number
- **Document type**: Document type (see constants)

**Example:**
```
udf_TransferToProduction(1000, nMODE_AUFTRAG)
```

#### 8. Production transfer to ALCIM Capacity Planning
**`udf_TransferToCapacityPlanning(Document number, Document type)`**
This function executes a production transfer to ALCIM Capacity Planning for the transferred document.

**Parameter:**
- **Document number**: Order number
- **Document type**: Document type (see constants)

**Example:**
```
udf_TransferToProduction(1000, nMODE_AUFTRAG)
```

#### 9. Production release
**`udf_ReleaseForProduction(Document number, Status point new)`**
This function performs for the transferred document a production release in ALCIM via PPS webservice and raises the status in ALFAK to the status of the transferred status point.

**Parameter:**
- **Document number**: Order number
- **Status point new**: Status point for status increase

**Example:**
```
udf_ReleaseForProduction(1000, 40)
```

#### 10. Update of production status in BW_LOCK_KAPA
**`udf_UpdateKapaStatus (Document number, Document type, Kapa status)`**
This function sets the status (production status in BW_LOCK_KAPA) for the transferred document.

**Parameter:**
- **Document number**: Document number
- **Document type**: Document type (see constants)
- **Kapa status**: Production status (see constants)

**Example:**
```
udf_UpdateKapaStatus(1000, nMODE_AUFTRAG, KAPA_NEW_ENTRY)
```

#### 11. Reducing the order status after scheduling error in ALCIM Capacity Planning
**`udf_StatusUpdateAfterPlanningError (Document number, Status point new)`**
This function reduces the status of the transferred order to the user status of the transferred status point if the current order status is lower/equals status 39 „Scheduling error“. This function should be used to select all orders of status 39 then reduce their status.

**Parameter:**
- **Document number**: Document number
- **Status point new**: Status point the user status of which this order shall get

**Example:**
```
udf_StatusUpdateAfterPlanningError (1000, 2)
```

#### 12. Checking and reading the status allocation
**`udf_ReadStatusPoint (nStatusPoint, Receive nStatus, Receive nMindeststatus, Receive nSperrstatus)`**
Reads the status allocation for the status point. If the status allocation can be read, the receive parameters nStatus, nMinStatus and nSperrStatus will get the values allocated to this status point.

**Parameter:**
- **nStatusPoint**: Status point to be read
- **nStatus**: Allocated status
- **nMindestStatus**: Minimum status of the status allocation
- **nSperrStatus**: Lock status of status allocation

**Returns:**
TRUE if the status allocation can be read and FALSE if it cannot be read.

**Example:**
```
udf_ReadStatusPoint (35, nStatus, nMinStatus, nSperrStatus)
```

## 12. Interfaces to Financial Accounting

### 12.1. Brilliant

**General:**
Transfer to BRILLIANT financial accounting system has been solved by customizing. The documentation on the customizing of the transfer to financial accounting is found in this document, in section Customizing.

**Interface description:**
`\\jupiter\DOKU DocuWare\ALFAK2000\Interfaces\FINAC\User Manuals\Brilliant`

**Settings:**
- In accordance with financial accounting, external keys for:
  - Tax
  - Payment Terms
- must be defined.
- In transfer to financial accounting, set the option "Customer account instead of customer number".
- Four formulas have to be defined and allocated to program items:

| No. | Formula | Program item |
| :-- | :--- | :--- |
| 1 | `Financ_Brilliant_Start.txt` | 300 - FinAcc transfer (start record) |
| 2 | `Financ_Brilliant_Head.txt` | 301 - FinAcc transfer (invoice header record) |
| 3 | `Financ_Brilliant_SalesAccount.txt` | 300 - FinAcc transfer (proceeds account record) |
| 4 | `Financ_Brilliant_TaxAccount.txt` | 300 - FinAcc transfer (tax record) |

The formulas number 1-4 are part of every ALFAK installation and are found in the Formula directory.

### 12.2. Datev

**General:**
Export of customer master data to Datev can be customised to match the requirements of the corresponding financial accounting program. The documentation on the customizing of the transfer to financial accounting is found in this document, in section Customizing.

**Interface description:**
`\\jupiter\DOKU DocuWare\ALFAK2000\Interfaces\FINAC\User Manuals\Datev`

**Settings:**
- A formula has to be defined and allocated to a program item:

| No. | Formula | Program item |
| :-- | :--- | :--- |
| 1 | `Financ_DATEV_CustomerExport.txt` | 307 - FinAcc transfer (customer export: customer record) |

The formula used, `Financ_DATEV_CustomerExport.txt`, is part of every ALFAK installation, to be found in directory Formula.

### 12.3. Varial

**General:**
Transfer to financial accounting writes three files for transferring invoices, credit notes, and costs, and another four files for account and address file for customers, and account and address file for suppliers. The target directories for the output files should be temporary directories. After transfer to financial accounting, the batch defined in master data will be executed, copying the output files to the target and backup directory.

**Interface description:**
`\\jupiter\DOKU DocuWare\ALFAK2000\Interfaces\FINAC\User Manuals Varial (Semco)`

**Settings:**
- **Company master data - tab FinAcc**
  - **Export/Import:** VARIAL 2.5
  - **Client:** maximally three-digit company number of the customer in VARIAL financial accounting
  - **Document export:** three path/file names, separated by semicolon
    - Example: `C:\Temp\XXSEQINP;C:\FiBu\XXSEQINP;C:\Temp\XXSEK000`
    - Path/file 1 for invoices
    - Path/file 2 for purchase orders
    - Path/file 3 for cost file
  - **Partner export:** four paths, files names separated by semicolons:
    - Example: `C:\Temp\XXSEQIPK;C:\Temp\XXSEQIKO`
    - Path/file 1 for debtor account file
    - Path/file 2 for debtor address file
    - Path/file 3 for creditor account file
    - Path/file 4 for creditor address file
  - **Batch file:** Create batch file for copying the output files to the target directory backup directory (optional)
  - **Options, cost accounting active 'on'**
  - Apart from the proceeds accounts, the cost centres of the proceeds accounts have to be maintained.
  - **Receivables report import:** path and file name
    - Example: The file includes four fields, Customer/Receivables amount/credit limit, and insured credit limit, separated by semicolons
    - Example: `(1000;14738;20000;25000)`

- **Settings: FinAcc transfer options**
  - Override output file "off"
  - Customer transfer disabled "off"
  - Customer account instead of customer number as required
  - Transfer to cost accounting „on"

- **The following external keys have to be maintained in ALFAK master data (to be agreed with financial accounting):**
  - Payment terms (external key max. three-digit)
  - Currencies (external key max. three-digit)
  - Tax (external key max. three-digit)
  - Field service (name max. 15)
  - Titles (name max. four-digit)
  - Counties/provinces (name max. three-digit)
  - Languages (external key max. two-digit)
  - Countries (name max. three-digit)
  - Debtor/credit account for tax

**Special features:**
- For invoices for miscellaneous customers, master data transfer is always made based on the order data.
- Invoice numbers of purchase orders are entered at invoice check as: `invoice no. supplier # internal batch no.` (e.g.: `123456#000001`).
- Cost accounting records are issued only for invoices (positive amount) and credit notes, document type `<n.e.>` (negative amount). The cost unit is created from the profit account's cost centre in the following way:
  `Cost centre = 4100102` → `Cost unit = 200410010`
  The cost unit always has nine digits. The first digit is always the last digit of the profit account, followed by the rest of the profit account (filled up to eight digits to the left using zeros).
  `2 + 00 + 410010`
- Profit accounts are transferred without the last digit.
- Record number + text of external record.

| | Invoice | Credit note | P.O. with invoice no. | P.O. w/o invoice no. |
| :--- | :--- | :--- | :--- | :--- |
| **Field17** | Invoice no. | Invoice no. | Invoice no. | Internal batch no. |
| **Field49** | `RE" + Invoice no. + "/AU" + Document no.` | `RE" + Invoice no. + "/AU" + Document no.` | `Invoice no. + "/" + Matchcode supplier` | `Internal batch no. + "/" + Matchcode supplier` |

- **Settlement document**
| | Invoice | Credit note | Purchase Order |
| :--- | :--- | :--- | :--- |
| **Field80** | empty | Invoice no. reference order | Invoice no. Lieferant (supplier) |

- **Cost unit in profit account record**
| | Invoice | Credit note | P.O. profit account starts with 5 | P.O. other profit accounts |
| :--- | :--- | :--- | :--- | :--- |
| **Field55** | 2 | 2 | empty | 1 |
| **Field56** | Cost centre of profit account w/o last digit | Cost centre of profit account w/o last digit | empty | Cost centre of profit account w/o last digit |

### 12.4. eGecko

**General:**
Transfer to financial accounting creates one file (or two files if invoices received have to be written as well) for transferring invoices, credit notes, or costs, and another file for customer master data. The target directories for the output files should be temporary directories.

**Interface description:**
`\\jupiter\DOKU DocuWare\ALFAK2000\Interfaces\FINAC\User_Manuals\eGecko`

**Settings:**
- **Company master data - tab FinAcc**
  - **Export/Import:** CSS eGecko (GER)
  - **Client:** max. four-digit company number of customer in Gecko financial accounting
  - **Booking area:** Two booking codes must be entered, for orders and credit notes. These are read by the program, and saved in the appropriate places in the FinAcc transfer file.
  - **Document export:** path and file name or, if required, another file name for invoices received, separated by semicolon (P.O.)
    - Example 1: `c:\temp\Fan\%d%M%y*buch-dat.xml`
    - Example 2: `c:\SNH\%d%M%y*AUS-dat.xml;c:\SNH\%d%M%y*EIN-dat.xml`
  - **Partner export:** path and file name
    - Example: `c:\temp\Fan\adress*.xml`
  - **Receivables report import:** path and file name
    - Example: `c:\temp\Fan\salden.dat`

- **Settings: FinAcc transfer options**
  - OEM conversion active
  - Automatic sorting active (customer/invoice/order)

- **The following external keys have to be maintained in ALFAK master data (to be agreed with financial accounting):**
  - Payment terms (external key max. three-digit)
  - Languages (external key max. two-digit)
  - Countries (name max. three-digit)
  - Titles (name max. four-digit)

**Special features:**
- Phone and fax number are included in the export of customer data. This is done automatically in connection with transfer to financial accounting based on a change of customer master data. In customer master data, the phone and fax number (area code and phone number) have to be entered separately. The separator is a minus sign but /, \ or a blank can be used as well.
- **Booking area**
  | eGecko | ALFAK |
  | :--- | :--- |
  | **buchungsschluessel** | Booking area acc. to company master data |
  | 210 | For orders/invoices (customer account) |
  | 150 | For orders/invoices (profit account) |
  | 250 | For credit notes (customer account) |
  | 110 | For credit notes (profit account) |
- **Document no.**
  | eGecko | ALFAK |
  | :--- | :--- |
  | **referenznr** | Record number (invoice number) from the document header |
- **Booking text**
  | eGecko | ALFAK |
  | :--- | :--- |
  | **buchungstext** | Name of customer shown on the invoice |
- **Customer account**
  | eGecko | ALFAK |
  | :--- | :--- |
  | **Acct. No.** | Customer # |

### 12.5. Customizing of the Transfer to Financial Accounting

Every record type written during transfer to financial accounting can be overridden by a formula, i.e. the record structure and the contents of the record are defined by the formula (formula items 300 to 308). It is also possible to add information to an existing record, i.e. an existing format will still be used, completed by a new field (formula items 309 to 316). The formula transfers this record to the transfer to financial accounting which again transfers it to the financial accounting file. The customizing management offers on tab `Programs` 16 new customizing items.

#### 12.5.1. Customising items
Each of these items corresponds to the transfer of a record type, each item can be allocated a separate formula:

**Tab. 51: Customizing- Points**

| Point | Record type | Meaning |
| :--- | :--- | :--- |
| 300 - FinAcc transfer (start record) | Start record | This record is written once, when transfer is started |
| 301 - FinAcc transfer (invoice header record) | Invoice header record | This record is written once per invoice in the number manager |
| 302 - FinAcc transfer (proceeds account record) | Proceeds account record | This record is written for every proceeds account of an invoice |
| 303 - FinAcc transfer (tax record) | Tax rate | This record is written once per invoice (VAT) |
| 304 - FinAcc transfer (end record) | End record | This record is written once, to complete the transfer |
| 305 - FinAcc transfer (receivables report) | Report on receivables | This formula is executed once for every imported receivables record |
| 306 - FinAcc transfer (customer export start record) | Start record | This record is written once, when transfer is started |
| 307 - FinAcc transfer (customer export customer record) | Customer record | This record is written for every customer exported |
| 308 - FinAcc transfer (customer export End record) | End record | This record is written once, to complete the transfer |
| 309 - FinAcc transfer (add to start record) | Start record | The return value of this formula is added to the start record, or the record is directly changed via UDF function |
| 310 - FinAcc transfer (add to invoice header record) | Invoice header record | The return value of this formula is added to the start record, or the record is directly changed via UDF function |
| 311 - FinAcc transfer (add to proceeds account record) | Proceeds account record | The return value of this formula is added to the start record, or the record is directly changed via UDF function |
| 312 - FinAcc transfer (add to proceeds account record) | Tax rate | The return value of this formula is added to the start record, or the record is directly changed via UDF function |
| 313 - FinAcc transfer (add to end record) | End record | The return value of this formula is added to the end record, or the record is directly changed via UDF function |
| 314 - FinAcc transfer (customer export add to start record) | Start record | The return value of this formula is added to the start record, or the record is directly changed via UDF function |
| 315 - FinAcc transfer (customer export add to customer record) | Customer record | The return value of this formula is added to the start record, or the record is directly changed via UDF function |
| 316 - FinAcc transfer (customer export add to end record) | End record | The return value of this formula is added to the end record, or the record is directly changed via UDF function |

#### 12.5.2. Variables and functions used

**Invoice header - Variables (Tab. 52)**

| Variable | Description |
| :--- | :--- |
| `w_nGrossAmount` | Gross invoice amount |
| `w_nGrossAmountFW` | Gross invoice amount in foreign currency |
| `w_nInvoiceNo` | Invoice number |
| `w_sInvoiceNo` | Alpha-numerical invoice number / column NR_RECHNUNG (tables BW_BEST_MAN / BW_BEST_AUFTR) |
| `w_dInvoiceDate` | Invoice date |
| `w_dDueDate` | Due date |
| `w_nCustomerAccount` | Customer # |
| `w_fktDoc` | Order category |
| `w_fktDKP` | Customer category |

**Proceeds account - variables (Tab. 53)**

| Variable | Description |
| :--- | :--- |
| `w_sSalesAccount` | Proceeds account |
| `w_nSalesAccountAmount` | Net amount of proceeds account |
| `w_sSalesAccountCostCenter` | Cost centre of proceeds account |
| `w_bSplit` | TRUE = invoice has more than one profit account, FALSE otherwise |
| `w_bSplitERLKOMitBetrag` | TRUE = invoice has more than one profit account with an amount, FALSE otherwise |

**Tax - Variables (Tab. 54)**

| Variable | Description |
| :--- | :--- |
| `w_nTax1Percentage` | Percentage of tax 1 |
| `w_nTax2Percentage` | Percentage of tax 2 |
| `w_nTaxAmount1` | Amount of tax 1 |
| `w_nTaxAmount2` | Amount of tax 2 |
| `w_nTax1AmountFC` | Amount of tax 1 in foreign currency |
| `w_nTax2AmountFC` | Amount of tax 2 in foreign currency |
| `w_nTax1BaseAmount` | Basic amount of tax 1 |
| `w_nTax2BaseAmount` | Basic amount of tax 2 |
| `w_nTax1BaseAmountFC` | Basic amount of tax 1 in foreign currency |
| `w_nTax2BaseAmountFC` | Basic amount of tax 2 in foreign currency |

**Discount and external key - Variables (Tab. 55)**

| Variable | Description |
| :--- | :--- |
| `w_nDiscountAmount` | Cash discount |
| `w_nDiscountAmountFC` | Cash discount in foreign currency |
| `w_sTax1ExternalKey` | External key for tax 1 |
| `w_sTax2ExternalKey` | External key for tax 2 |
| `w_sPaymentTermsFKey` | External key for payment condition 'invoice' |
| `w_sCurrencyExternalKey1` | External key 1 for the invoiced currency |
| `w_sCurrencyExternalKey2` | External key 2 for the invoiced currency |

#### 12.5.3. Customer category w_fktDKP

To export customer master data, the object `w_fktDKP` can be used to access the data of the customer to be exported. The name of the customer is determined by `w_fktDKP.m_sNAME1` for example, and the street by `w_fktDKP.m_sSTRASSE`. All database fields of the document can be accessed this way.

**More examples:**

| Object Property | Description |
| :--- | :--- |
| `w_fktDKP.m_sPLZ` | ZIP code |
| `w_fktDKP.m_sTLF1` | Telephone 1 |
| `w_fktDKP.m_sUST_ID` | VAT ID |
| `w_fktDKP.m_nKREDIT_LIMIT` | ALFAK credit limit |

#### BRILLIANT: Example of a completely customized transfer to financial accounting
The BRILLIANT transfer consists of a start record which is written once per transfer, an invoice header for every invoice in the number manager, the variable number of proceeds account records per invoice, and a tax record per invoice. Customer master data transfer is handled by customizing too.

First, set the financial accounting interface (Master data > Company > Company data > tab FinAcc) to „Customizing" in company parameters, and fill in the required parameters (e.g. output file).

Define the necessary formulas in formula management (Master data > Company > Formulas). The example formulas for the BRILLIANT transfer are found in the formula directory of every ALFAK installation (Financ_Brilliant..).

**Important:** In all formulas of transfer to financial accounting, the text allocated to variable sResult is written in a line of the financial accounting output file. The formulas have to be allocated to the corresponding program items in Customizing management.

#### 12.5.4. Format functions

**`Adjust_NrToStr(value, fieldLength, digits)`**
This function converts a numeric entry `value` into a string. The number `digits` defines the number of decimals of the `value` to be adopted. The number `fieldLength` defines the length of the string. If the number is shorter than `fieldLength`, the entry will be headed by zeros.
- `Adjust_NrToStr(4.25, 8, 2)` → return "00004.25"
- `Adjust_NrToStr(8500, 4, 0)` → return "8500"

**`Adjust_NrToStrB(value, fieldLength, digits)`**
The function converts like Adjust_NrToStr but fills up with BLANKS.
- `Adjust_NrToStrB(4.25, 8, 2)` → return " 4.25"
- `Adjust_NrToStrB(8500, 4, 0)` → return "8500"

**`Adjust_String(value, fieldLength)`**
Brings a value string to the necessary field length by adding BLANKS if necessary.
- `Adjust_String("Dieter Endres", 20)` → return "Dieter Endres "
- `Adjust_String("Dieter Endres", 4)` → return "Diet"

**`SalNumberToStrX(Number, DecimalPlaces)`**
Converts a number with the defined number of decimals into a string.
- `SalNumberToStrX(4711, 0)` → return "4711"
- `SalNumberToStrX(4711.452, 2)` → return "4711.45"

**`SalStrLeftX(String, Number)`**
Returns the defined number of characters from a string.
- `SalStrLeftX("Dieter", 10)` → return "Dieter"
- `SalStrLeftX("Dieter", 3)` → return "Die"

**`SalStrLength(String)`**
Returns the number of characters of a string.
- `SalStrLength("Dieter")` → return: 6

**`Adjust_Date_YYYYMMDD(Date)`**
Formats the transferred date in the format yyyyMMdd (yyyy=year, MM=month, dd=day) and returns it as a string.
- `Adjust_Date_YYYYMMDD(28.9.2009)` → return: "20090928"

**`Adjust_Date_DDxMMxYYYY(Date, Separator)`**
Formats the transferred date in the format ddxMMxYYYY (yyyy=year, MM=month, dd=day) - x being the separator sign – and returns it as a string.
- `Adjust_Date_DDxMMxYYYY(28.9.2009, "/")` → return: "28/09/2009"

#### 12.5.5. UDF functions for manipulating/adding fields
> **IMPORTANT:** The mentioned udf functions can be used to change or add an existing record and will always affect the record defined by the formula allocation.
> If for instance the udf function is used in the formula allocation 315 - FinAcc transfer (customer export: add to/insert in customer record), the udf function will affect the customer record at master data export!

**`udf_XMLAddNode (NodeName, NodeText, ParentNode)`**
For XML interfaces: adds a new junction to the parent junction and sets the value of the new junction.
**Example:** `Udf_XMLAddNode ('mahnbar', 'j', 'PersonenKonto')`
Adds the new junction 'remindable' with the value 'j' as a sub-junction of 'Personal account'.
```xml
<PersonalAccount>
  <Nummer>1000</Nummer>
  <Name>Müller</Name>
  <mahnbar>j</mahnbar>
</PersonalAccount>
```

**`udf_XMLSetText (NodeName, NodeText)`**
For XML interfaces: sets the text for an existing junction.
**Example:** `Udf_XMLSetText ('mahnbar', 'n')`
Sets the text for the junction 'remindable' to 'n'.
```xml
<PersonalAccount>
  <Nummer>1000</Nummer>
  <Name>Müller</Name>
  <mahnbar>n</mahnbar>
</PersonalAccount>
```

**`udf_SeparatedFieldAddField (FieldSeparator, FieldText)`**
For interfaces with field separator: adds a field separator and a new field at the end of the interface.
**Example:** `udf_SeparatedFieldAddField (';', 'no reminder')`

**`udf_SeparatedFieldSetText (FieldNumber, FieldSeparator, FieldText)`**
For interfaces with field separator: changes the contents of the field with the transferred field number to the new value.
**Example:** `udf_SeparatedFieldSetText (2, ';', 'no reminder')`
Sets the contents of the second field to 'no reminder'.

**`udf_FixedFieldAddField (FieldLength, FieldText)`**
For interfaces of fixed field length: adds a new field at the end of the interface.
**Example:** `udf_FixedFieldAddField (13, 'no reminder')`

**`udf_FixedFieldSetText (FieldOffset, FieldLength, FieldText)`**
For interfaces with field separator: changes the contents of the field in the transferred place to the new value. Attention: Offset is zero-based.
**Example:** `udf_FixedFieldSetText (0, 13, 'no reminder')`
Sets the contents of the first field to 'no reminder'.

### 12.6. Export debtors and creditors in the workflow

#### 12.6.1. With file
The export of the debtors and creditors can now be done via workflow formula. However, this depends on the financial accounting interface; it has to be set in the company parameters. The export only works if the interface also supports the export of this data.
The task can be set up with the sample formula `ExchangeService\workflow_finacdebitorcreditorexport.txt`.
The udf function `"udf_FinacDebitorCreditorExport(Client, Type, Filename)"` is documented in the customizing function reference `"Formula\customizing documentation.htm"`.
Which data records are transferred is determined by the database column `KZ_STATUS>0` of the `KU_KUNDEN/LI_LIEFERANTEN` table.
The export generates messages in the Exchange Service Monitor.

#### 12.6.2. With Webservice (eGecko)
The export of the debtors and creditors can now also be done via Webservice for the eGecko FinAc.
The FinAc must be configured for eGecko as if it would be done via file. The export file must also be set, for first a file is generated and this is then transferred to the eGecko Webservice.
The task can be set up with the sample formula `ExchangeService\workflow_finacdebitorcreditorexportWS.txt`.
The udf function `"udf_FinacDebitorCreditorEGeckoWSExport( Client, Type, serviceUrl, User, Password)"` is documented in the customizing function reference `"Formula\customizing documentation.htm."`.
Which data records are transferred is determined by the database column `KZ_STATUS>0` of the `KU_KUNDEN/LI_LIEFERANTEN` table.
No user/password is required in order to address the Webservice. With the call `<Url Webservice>?WSDL` it is possible to check whether it can be reached.
The export generates messages in the Exchange Service Monitor.

### 12.7. CAM credit management interface

CAM is a system for risk management from `prof-schumann.com`. For this, in addition to data from the FinAc (open items), it also uses insured credit limits and data from various information services. Within this system, decisions about the creditworthiness and the limit assignment to individual sites are made. Even urgent inquiries, for example for limit increase or redistribution, are processed here in timely fashion.

The overall process is organized in 3 partial areas:
1.  **Application for increase of the credit limit.**
    If for the entry of an order, the credit limit approved for the customer is exceeded, a dialog can be called up with which the person entering the order can apply for an increase of the credit limit automatically and electronically. The application should be logged.
2.  **Transfers of current data from CAM to A+W Business**
    The changes in the CAM system (new limits, creditworthiness indicators or changed open items) should be transmitted without delay to the ERP systems and become effective there.
3.  **Automatic release of locked orders**
    Today's manual process for releasing locked orders should be automated. After new limits, open items, etc. have been transmitted, there is a check whether locked orders can be released automatically. The release is then done automatically by A+W Business.

Due to the compatibility with old customer numbers, an expansion has been undertaken. If a creditor account has been stored in the customer master data, then the transfer to CAM is done and the processing of the credit limit increase via this account number; it includes the customer's old account number.

#### Credit limit changes from CAM
The WebService receives the data from CAM and saves it as data records with the type 60 in the tables FS_POOL and FS_POOLKOPF. Processing is not done in the WebService.

The WebService has a new interface 'ErpCredit'; it includes the new method:
`public bool StoreCreditData(ErpSettings erpSettings, Credit credit, out string result)`

For the call of the web service, the database connection and the logical A+W Business user must be transferred. The database connection is made via integrated security, to have access to the database with the pool user application. The logical A+W Business user must be created and its password must also be transmitted.

The parameters in detail are:

**ErpSettings**
| Parameter | Description |
| :--- | :--- |
| Server | Name of the SQLServers incl. instance |
| Database | Database name (catalog) of the A+W Business |
| USER | Logical A+W Business user for login to the database |
| PASSWORD | Password for login to the database |
| ClientType | Always 2= A+W Business |
| DatabaseType | Always 3 = SQLServer |
| ConfigurationFile | Always empty |

**Credit**
| Parameter | Description |
| :--- | :--- |
| `CreditDetails<CreditDetail>` | Collection of all changed credit data of the client |

**CreditDetail to AWBusiness Mapping**
| CreditDetail Field | Description | AWBusiness Field |
| :--- | :--- | :--- |
| CustomerNo | Customer number | `KU_KUNDEN.ID` |
| Rating | Credit standing (CAM) | `KU_KLASSI_WERTE.ID=6` |
| Limit 1 | Credit limit | `KU_KUNDEN.KREDIT_LIMIT` |
| Limit 2 | Delivery limit | `KU_KUNDEN.KREDIT_LIMIT1` |
| Limit 3 | Insurance limit (CCI) | `KU_KLASSI_WERTE.ID=8` |
| Ranking | Ranking (CAM) | `KU_KLASSI_WERTE.ID=7` |
| Lock | Lock ID (0=not locked, 1=locked) | `KU_KUNDEN.KZ_GESPERRT` |
| OpenItems | Receivables | `KU_KUNDEN.SALDO_J` |

The record structure in the `FS_POOL` type 60 looks like this:

| Field | Position | Length | Description |
| :--- | :--- | :--- | :--- |
| Customer # | 0 | 15 | Customer number for the credit data |
| Limit 1 | 15 | 15 | Credit limit 1 (credit limit) |
| Limit 2 | 30 | 15 | Credit limit 2 (delivery limit) |
| Limit 3 | 45 | 15 | Credit limit 3 (insurance limit, classifier = 8) |
| Lock | 60 | 2 | Lock ID (0=not locked, 1=locked) |
| Ranking | 62 | 10 | Creditworthiness ranking, e.g. "AAA" (classifier = 6) |
| Rating | 72 | 10 | Creditworthiness, e.g. 0-100 (classifier = 7) |
| Receivables | 82 | 15 | Customer open items |

For the processing, a workflow must be created, which calls the function `udf_ProcessCreditLimit()`. Example in `..\Formula\workflow_creditlimitCAM_import.txt`. The data is updated in the customer master data and the processing is logged in the workflow management.

If the reporting produces a positive balance for the customer, then after the entry sequence, the orders are released with credit limit lock until the balance is 0 once again. For the credit limit lock, the status point 700 is used; for the release, the status point 701 is used. Caution: The status of the order is reset. The status points must be assigned.

#### Application for credit limit increase
The credit limit increase application dialog displays all applications existing in the table. The status (0=created, 2=processed, 9=error) indicates what the status of the application is.

If several applications are made at the same time, then only the last one is transferred; the others are set to processed. In the Result table column, a corresponding error message from CAM is displayed. There can only ever be one application unprocessed in CAM; the 2nd application will be declined with error message.

The table updates itself automatically, however the user does not have to wait for the transfer; this is done in the background by the Exchange Service. There is no feedback.

The dialog contains a credit limit and delivery limit; the application can be time-limited and limits can be defined according to the time limit.

The entry of the records is done in the table `KU_LIMITREQUEST`. A workflow must be created that transfers the data to CAM. Example: `..\Formula\workflow_creditlimitCAM_export.txt`.

The transfer is done by the function `udf_RequestCreditlimitCAMWSExport (URL, User, Password)`. If there are errors during transmission, then the record is set to the error status; there is no new transfer. The application must be made again.

### 12.8. Fibu-WebService via customizing (Beta not released)

#### 12.8.1. Overview
The possibility has been created to approve web queries via the customizing. Here, both the header and body data can be released; XML and JSON are supported for the data transfer. It must be noted that for the JSON transfer to a Web service, an XML input is required; the XML data is converted within the RestRequest functionality. During the transfer of an XML data structure to a Web service, XML can be created directly by the customizing; the XML data is not processed further.

#### 12.8.2. Functions
This functionality makes it possible to send Web queries via POST and GET to any end point and to receive the corresponding answer. The following UDF functions have been added in the course of the development:

**`udf_GenericWebService_RestRequest`**
- **Parameter:**
  - `string xmlConfiguration`
  - `string xmlPayload`
- **Return:** `string Return (as XML construct)`
- **Description:** The query is sent to the desired Webservice with the appropriate configuration in the `xmlConfiguration-XML-String`. The configured parameters and body are used from the `xmlPayload` parameter. All required parameters must be filled out. To make parameter input easier, there are help functions provided (see below).

**`udf_GenericWebService_Payload_Body_Create`**
- **Parameter:**
  - `string sValue` (example: 1234,56): The value to be created in this body parameter.
  - `string sName` (example: Parameter1): The name of the value to be created in this body parameter.
  - `Number nType` (example: 1): The type for the specified sValue.
    - 0 = sValue is a string
    - 1 = sValue is a float/double (has places after the decimal point)
    - 2 = sValue is an integer (has no places after the decimal point)
- **Return:** `string xmlBody (as XML construct)`
- **Description:** This function creates the `sBody` used in the call of '`udf_GenericWebService_BuildPayload`'. To join several body parameters, the return value of this function can be attached to a previous return value. It is important that the right `nType` is used for the respective `sValue`.

**`udf_GenericWebService_Payload_Header_Create`**
- **Parameter:**
  - `string sValue` (example: 1234,56): The value to be created in this header parameter.
  - `string sName` (example: Parameter1): The name of the value to be created in this header parameter.
  - `Number nType` (example: 1): The type that determines how this header is transferred.
    - 0 = unprocessed header (no changes)
    - 1 = Query Parameter
    - 2 = Automatic (WebClient decides per query type where the header will be written)
- **Return:** `string xmlBody (as XML construct)`
- **Description:** This function creates the `sBody` used in the call of '`udf_GenericWebService_BuildPayload`'. To join several body parameters, the return value of this function can be attached to a previous return value. It is important that the right `nType` is used for the respective `sValue`.

**`udf_GenericWebService_BuildPayload`**
- **Parameter:**
  - `(optional) string sBody`: Data to be transferred in the query, generated via '`udf_GenericWebService_Payload_Body_Create`'. Mandatory for a JSON query.
  - `(optional) string sHeaders`: Other headers to be transferred, generated via '`udf_GenericWebService_Payload_Header_Create`'.
- **Return:** `string xmlPayload` (finished XML payload for '`udf_GenericWebService_RestRequest`'.)
- **Description:** This function builds the XML payload. The call is mandatory, even if both parameters are empty.

The '`GenericWebServiceResponseDto`' structure is returned by the function '`udf_GenericWebService_RestRequest`'. This is always a string that contains this structure as XML.

**Example of an XML return:**
```xml
<?xml version="1.0" encoding="utf-16"?>
<GenericWebServiceResponseDto xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <Success>true</Success>
  <HttpStatusCode>200</HttpStatusCode>
  <ResultContent>{
    "data": "example return data",
    "value": "{\"someNumberValue\":\"1234\",\"moreNumberValues\":164384.4}"
  }</ResultContent>
  <HasException>false</HasException>
  <ExceptionMessage />
</Return>
```

#### 12.8.3. Trace notes
For the execution of the function `"udf_GenericWebService_RestRequest"` the traces are written under the category `"CommercialExchange"`. The parameters of the query for use of the `"Debug"` trace level and the result are written too. For execution without `"Debug"` trace level, the parameters are only repeated if an exception occurs. Trace entries are written under the name `"GenericWebServiceSendRequest"`.

Example: use of the generic Web service using the customized Web service FinAc implementation for C.Bergmann can be found here: `"Financ\Customized Web-Service-FIBU\C.Bergmann \WF-Fibu-302-Erlöskontensatz.txt"`. In the example, with the help of the new UDF functions, an XML document is built and sent to an endpoint provided by the customer.

### 12.9. FinAc - workflow functionality

#### 12.9.1. Overview
With the introduction of this new option, it is now possible to execute the FinAc completely in a workflow in the background. This option must be activated explicitly. The new option is in "Company Data" > "FinAc" > "Financial Accounting" > "Enable Workflow". With the activation of this class, currently the entire FinAc class is replaced with the new implementation; the consequence of this is that all functions that are not directly dialog-related are no longer represented in the `frmFIBU` class. A new functional class has been added for this, which now includes these functions (cfktFibu). Upon activation, this new class is used in the interactive FinAc execution and in the workflow. However, this option is only available for FinAcs that use the standard `abcfibu.exe`; this excludes all numeric FinAcs and some country-specific FinAcs. The "Enable workflow" option is deactivated automatically insofar as the workflow execution is not available.

#### 12.9.2. Workflow execution
To start the FinAc workflow, the following UDF function is used:
**`udf_FIBU_Workflow(nNV_FaktTyp, nMandant, sNVName)`**
The UDF function returns a Boolean that is TRUE with successful execution and FALSE in case of an error. Traces are written depending on which error occurred. Traces are written under the function name.

For the execution in the workflow, it is assumed that all formulas that are executed in the customizing of the FinAc have already been adjusted to the new naming of the variables! If no formulas are used, then no changes must be made.

#### 12.9.3. Functioning and special functions
With activation of the workflow functionality of the FinAc, a new class is used that can execute the entire implementation of the FinAc apart from a dialog.
It must be noted that for workflow execution, no dialogs can be displayed. This means that all errors and any messages are displayed in the workflow log.

If there is no revenue account, the error message is displayed in the log. There is no interactive query of the revenue account. If a revenue account is not found at the beginning of workflow execution, the entire execution is interrupted and noted with an error. The revenue accounts must be created correctly so that an execution of the workflow is possible.

For the workflow, the original variable names are taken over nearly identically; however, each variable has a `m_` placed in front of it. That is, if a variable was previously called `"w_sInvoiceNo"`, it will be called `"m_sInvoiceNo"` in the workflow environment. This applies for all variables except for global variables; these can be reached normally. It must be noted that all local function variables have still received the original naming; all Instance/ex. window variables are affected by the renaming.

For the implementation, only the AW standard FinAcs have been tested in connection with the workflow implementation; all other FinAcs must be checked before first use. Insofar as customizing is used, it must be adjusted. It is recommended that you create a copy of each FinAc customizing formula used in order to ensure data back-up of the original formula; this way, if an error occurs, the original formula will still be present. The variables must be adapted according to the new naming in the copy of the formula.

#### 12.9.4. Sample implementation
An example of a complete implementation of a customized Web service FinAc can be found under this path: `"Financ\Customized Web-Service-FIBU\C.Bergmann"`.

## 13. Databases

### 13.1. Replication

Replication serves to transfer data from a company's headquarters to its subsidiaries/sites. This requires the creation of data structures in the databases in which the amended or new data headquarters data will be saved. By means of replication, the data will be distributed from headquarters to all sites, to be added or updated. So-called Triggers have to be installed to be able to collect the newly created or changed data at headquarters. Triggers are database processes that can respond to events such as Insert or an update. These triggers make it easy to log data changes without major program amendments.

At the individual sites, it must be possible to disable certain data fields in the management programs for products, customers, and suppliers so that these fields can only be changed by headquarters, via replication. Other data such as the route in customer data, have to be processed by the individual sites. It is therefore necessary to select all records created or changed via replication to be able to process the local data, and correct them if necessary. The local data are defined by means of the replication management program.

The program `Basic number areas` has been added in master data, General; it is used to manage the number areas for most of the catalogue tables. This is essential as the primary keys of these catalogue tables are the names themselves while ALFAK uses the background number for identification. The number areas allow to define special, non-clashing number areas for every site.

#### 13.1.1. Activating replication
Please find below a description of how to prepare ALFAK for replication.

**Database update**
To guarantee that replication works properly, it is essential that the data structure of all databases involved has the same release. This is why all update scripts should be run via script management on the database first.

**Setting the company parameters**
To make sure that the master data management programs behave correctly, you need to enable the code for active replication in company parameters. As a result, all non-local data fields will be locked in the management programs for partners and products; these can be changed only by headquarters, via replication. This setting has to be made for the subsidiaries only.

When replication is active, the administration dialogs for products, customers, and company parameters will find out which fields contain local data, and which do not. Non-local fields cannot be processed by the user. The local data are defined in the replication administration program. If field Route 1, Route 2 and the Delivery terms are defined as local fields in replication management, this will be reflected in the customer management UI.

The lock code in product and partner management was extended to allow the receiving site to select and process the records easily. Replicated records can be easily selected in QBE mode. The tagged data are available in the system only after the user has gone through the data, edited them, and set the lock code to `not locked`.

To allow the replication core to tag the replicated data in the target system, use the replication management program to define a default receipt value for the lock code. This value is the same for product and partner management. First, activate the indicator for a default value, then enter the default itself. The following list shows the value and its meaning.

- `0` = not locked
- `1` = locked
- `2` = replicated

**Defining rights for catalogue tables**
It is essential that the receiving sites cannot change the existing catalogue data as this might corrupt the replication. To ensure this, the rights for all users have to be defined accordingly. Rights should be allocated in such a way that new data can be created, but existing data cannot be changed.

**Defining the sites in the head office's database**
In the database of head office, you need to define all sites to which data shall be replicated. This is done in the replication management program. Please make sure to enter the subsidiaries' data correctly as the database login in the target system will be using this information. You have to use different paths for the individual subsidiaries to save the export files and import the receipts for the subsidiaries.

**Defining the jobs**
The replication creates the data based on so-called Jobs. These jobs define the tables to be included in the replication of headquarters. To replicate customer data for example, enter a job for the Customer table in the management program. All tables customer master data refer to, will be replicated this way.

**Exclusion of tables**
Tab 3 can be used in the Master to exclude tables from replication. This is set by means of „Disabled (manually)" in the table view. When a table is disabled, the system checks whether table `RR_TODO` includes data for the replication of this table. If records are found for this table, the program will want to know whether existing records shall be removed. If this is affirmed by „Yes", all data still to be replicated will be removed from table `RR_TODO`. Manually disabled tables will never be transferred by replication.

For tables which are explicitly excluded from replication, a sending default must be set for the reference tables to avoid a „Foreign Key" error at the import. When a table is disabled, the program will check now whether a sending default shall be set for the reference tables. An entry can be made or selected from the dialog; this will be used as the sending default for all reference tables.

**Transfer of replication data**
To copy the data to the subsidiaries, an automatic task for the ALFAK Interface Service will be entered at headquarters. Add the formula from the file `Workflow_ReplicationExport.txt` to this task. The function loaded by this formula will export the replication data for every headquarters and for every job. The data will be saved in the directory defined for the subsidiary in replication management. Before the export, the receipts from the subsidiaries' directory will be processed.

Every subsidiary must define an automatic task for the ALFAK Interface Service to which the formula from file `Workflow_ReplicationImport.txt` will be added. This formula imports all import files for this subsidiary from the directory defined in replication management, and creates a receipt for every file. This completes the replication cycle. The result must be emailed and also appears on the ALFAK Service Monitor.

**Installation and update of replication management**
The replication is automatically updated when the ALFAK installation is updated by means of the SetupLauncher. The components for the replication core are installed and updated by the ALFAK Interface Service; the Udf functions can be found in the ALFAK Com object `abcreceiveXX.exe` which is installed and updated by the ALFAK basic setup.

**Disabling the old replication call**
When the new replication is installed by AIS, the old replication needs to be disabled by means of the VB scripts. Possibly existing tasks have to be disabled in the operating system or in the backup.

#### 13.1.2. Defaults
Replication uses three types of defaults.
- **Dispatch default** - will always be saved in the transfer file instead of the original value when the data are transferred to the subsidiary
- **Receipt default** – after receipt of the data, this will be saved in the database instead of the transfer data, distinguishing:
  - **conditional default** (only for newly created records)
  - **unconditional default** (will always be set)
- **Default filler** – if a field (column) is missing from the transfer file, this value will be entered in the column in the target database.

#### 13.1.3. Known Problems
Replication will not work if umlauts are used in connection with the Unify SQL Base 11.5 PTF3. This can be corrected by Unify's EMP5258EDP and replacing `SQLBaseODBC.dll`. This hotfix is not included in the standard installation and has to be installed if required.

**Procedure:**
After installing PTF3 of SQLBase, the files of the archives EMP5258EDP.zip have to be copied onto the installation. Now replace `SQLBaseODBC.dll`. This is not necessary for PTF4 because it includes the error correction. The necessary files are part of the diskset of the installation directory of Unify SQLBase 11.5.

During installation, you can check whether the necessary version have been installed on the computer. The files of EMP5258EDP have file version 11.5.3.7145 and the new `SQLBaseODBC.dll` has the file version 11.5.3.7362. The files of PTF4 have file version 11.5.4.7773. The following list can be used to check the installation of SQLBase:

| File | PTF3 + EMP + ODBC Hotfix | PTF4 |
| :--- | :--- | :--- |
| CSFCNV32.dll | 6.0.0.4 | 6.0.0.4 |
| Csfedt32.dll | 11.5.3.7145 | 11.5.4.7773 |
| Daemon32.exe | 11.5.3.7145 | 11.5.4.7773 |
| EFDAEMON.exe | 11.5.3.7145 | 11.5.4.7773 |
| efhost.exe | 11.5.3.7145 | 11.5.4.7773 |
| Pswdhlpr.dll | | |
| Sqlbapw.dll | 11.5.3.7145 | 11.5.4.7773 |
| SQLBaseODB.dll | 11.5.3.7362 | 11.5.4.7773 |
| SQLBaseODBCSetup.dll | 11.5.3.7145 | 11.5.4.7773 |
| SQLBaseOLEDB.dll | 11.5.3.7145 | 11.5.4.7773 |
| SQLBaseUtil.dll | 11.5.3.7145 | 11.5.4.7773 |
| Sqlcrt32.dll | | |
| SQLNTTLK.exe | 11.5.3.7145 | 11.5.4.7773 |
| Sqltalk.exe | 11.5.3.7145 | 11.5.4.7773 |
| Sqltne.dll | 11.5.3.7145 | 11.5.4.7773 |
| Tlkc32.dll | 11.5.3.7145 | 11.5.4.7773 |
| Tlkc32sp.dll | 11.5.3.7145 | 11.5.4.7773 |

The files must exist in the export and import systems.

### 13.2. SQL Server Migration

The migration tool generally permits database porting from SQL Base to SQL Server. As from ALFAK Version 2012, migration is possible between the database systems. This is done with the Unicode option switched on (automatically). Since ALFAK 2012 can handle Unicode, database conversion to Unicode, even from SQL Base to SQL Base and SQL Server to SQL Server, is compulsory. After that, the database can be used only with ALFAK 2012 and later with a 2012 version.

> **IMPORTANT:** the archive databases that are in use must also be migrated with the migration tool before you start up ALFAK 2012.

#### 13.2.1. Database Connection
Originally, a SQL Base source and a SQL Server target for database migration could be entered. In view of ALFAK Version 2012, the database migration tool has been extended. The first new feature is the database login of the dialog: The connection for source and target database can now be set. Valid options are:
- SQL Base Native
- SQL Server OLEDB
  - You also need to enter the server on which SQLServer has been installed.
  - For SQLServer Express, you have to enter SQLEXPRESS apart from the server name: `<ServerName>\SQLEXPRESS`

The database, the user, and the password have to be entered as usual. The SQL Server database is accessed by an integrated security in the Windows login. For details please refer to the SQL Server setup.

#### 13.2.2. Limitations
- User authentication only in connection with the integrated Windows security. From ALFAK Version 2012, the Application Role will be created for SQL Server.
- The replication of A+W has not been changed to SQLServer. This is scheduled for ALFAK Version 2012.
- No master data history available.
- Competing master data access will not be blocked; the last one wins. For SQL Base, the first one wins.

#### 13.2.3. SQL Server setup
SQLServer must be installed with combined user authentication. The passwords for the SA user have to be noted and kept in a safe place. Login authorization and database user have to be defined in Management Studio. A login for the user group has to be defined (database server/security/registrations). This gives the users access to the database server. The server should be set to Public which suffices for ALFAK users.

The user group has to be given access to all necessary databases including archives (database server/databases/<database>/security/user). The database role should be set to `DB_Owner`. `DB_Datareader`+`DB_Datawriter` is also sufficient. In this case, database updates have to be made by a user with `DB_Owner`. This is possible after the databases have been created.

Activate the TCP/IP log in the SQLServer configuration manager (Start->Programs->Microsoft SQLServer 2008->Configuration tool) and start the SQLServer Browser service. This is necessary for the clients to address the SQLServer.

To test the database connection you can create a file with suffix `.UDL`. Double-clicking on this file will open the database connection dialog. Here, select `Microsoft OLEDB Provider for SQLServer` as a provider. Now choose the database server. Select Windows authentication. The connection can be tested when the databases are visible.

**Client setup**
Client PCs may require the installation of MDAC 2.8 (Microsoft Data Access Components). This depends on the other programs installed (ALFAK setup does not handle this at present).

#### 13.2.4. Migrating an existing database
The source database has to have the status of ALFAK 2008 prior to migration. For migration with Unicode option, the database must be updated to the latest version of ALFAK 2011 at least. This is the only way to make sure that the data types and definitions permit the migration without errors. Prior to migration, there has to be a registration that permits access to the database. The database must be accessible.

**Migration tool settings**
Migration is done in five steps. First configure the migration tool. Enter the source database connection in Source. This is done by means of the server, database, user, and password (for migration with Unicode option, choose the source's codepage). User and password have to be a real user (SYSADM).

`Target` configures all details referring to the target database, i.e. definition of server, database, user, and password. The possible source and target database combinations (with or without Unicode option) are enabled automatically (according to the ALFAK Version).

> **Important:** The database names have to be different. The migration tool does not execute an „InPlace-Migration".

The checkbox `SQLExpress` no longer exists. This extension must be entered by hand for the SQL Server name. If SQL Server is chosen as the target database, a button after the database name is enabled in order to define the starting size of the SQL Server database. This prevents defragmentation due to too many enlargements during migration. The tables are allocated to individual file groups. These can be split to different disks in case of performance problems. This allows parallel access. Furthermore, a pattern name must be defined for SQL Server (SYSADM). The file paths define the files for the scripts. They should not be changed. The migration tool has been configured now, and data migration can begin. Settings are stored. Migration of archives databases works in the same way; you only have to set the checkbox `Archives` as well.

**Creating the database and pattern**
First, use the button `Get Binary` to load the database, the binary data or long strings (`Long String`) into the table. The table serves for overview and the records can not be edited.

The database migration tool has been completed by a conversion function. Microsoft SQL Server offers the data type `date` from Version 2008 R2 upwards. As from now, the SQL Base `date` data type can be converted to a SQL Server `date` data type. Based on the text file `DBMigration_DateColumns.txt` which must be saved in the `<Alfak installation directory>\Cmd\`, one can find out which columns previously used the `date` data type in databases that could not be converted before. You can also create the text file `DBMigration_DateColumns.txt` yourself by means of migrating a SQL Base database to SQL Server.
