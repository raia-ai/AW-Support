---
title: "EN-CONFIG-AW_Business-5"
source: "EN-CONFIG-AW_Business-5.pdf"
tags: ["A+W Business", "Crystal Reports", "Troubleshooting", "Configuration", "Reporting Service", "PDF Generation", "DMS", "OAuth2", "Office365", "Technical Guide"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical guide for configuring and troubleshooting A+W Business software, focusing on the Reporting Service, Crystal Reports forms, and integration with external systems like Twinfax, DMS, and Office 365. It provides solutions to known problems, including printing, data formatting, and authentication."
long_description: "This document serves as a detailed configuration and troubleshooting manual for A+W Business, specifically addressing known issues and their solutions related to the Reporting Service and Crystal Reports. It covers a wide range of topics, including fixing form dispatch issues with Twinfax print drivers, correcting calculation formulas for net prices and totals in reports, and resolving collective printing discrepancies. The guide provides step-by-step instructions with UI screenshots for tasks such as restarting the queue manager, correcting database joins, and managing report group optimizations. It also details advanced configurations, such as accessing previous/subsequent data records in Crystal Reports, generating PDF files for DMS archiving with dynamic naming conventions, and handling user authentication for print jobs. Furthermore, it explains how to set up email dispatch with attachments, individual cover letters, and integration with Office 365 using OAuth2. The document is intended for system administrators and technical support personnel responsible for maintaining and customizing the A+W Business reporting environment."
---

---
## 3.10.11. Known problems and their solutions

### Problem: Twinfax Print Driver Dispatch Failure
The dispatch of forms via the Twinfax print driver did not work.

**Solution:**
It must absolutely be heeded that the line with the control characters is all by itself at the top edge. The font should be set to "Courier New" with a font size of 12. It must be checked whether this font is also installed on the PC on which the reporting service is executed. Furthermore, it must be checked whether the control characters were set correctly in the settings for the printer driver.

**Twinfax Properties Settings:**
- Go to `Twinfax Properties > Advanced > Control Sequences`.
- **Activate Control Sequences:** Yes
- **Start Control Sequence:** `1`
- **End Control Sequence:** `[`

If the fax dispatch still does not work, it may be necessary to restart the queue manager:

1.  Go to `Twinfax Properties > Advanced > Queue Manager`.
2.  Click `Queue Manager Configuration...`.
3.  In the `QueueManager Properties` dialog, under the `Queue manager services` tab, you can see the current service state.
4.  Click `Stop` and then `Start` to restart the service.

In addition, all processes with the name **"vs_win2app.exe"** and **"vsfaxdlg.exe"** must be ended in the task manager.

### Problem: Incorrect Price/Unit Net Calculation
The Price/unit net in BOM and item are not correct. The multiplication by the BOM quantity is missing in the BOM. This creates an incorrect total in the item line. (see case 440489)

**Solution:**
The affected forms include two incorrect formulas and two incorrect total fields. The A+W standard reports have already been reworked. However, customer reports must be corrected. The following formulas must be replaced with the functions below:

**BOMNetPricePerUnit:**
```vb
// Display the BOM item net price per unit (means per one piece of the line item)
// Either in own or foreign currency depending on header setting
WhilePrintingRecords;

if ({Header.Währung} <> {Company.Eigenwährung}) Then
(
    // Output foreign currency
    //(#440489-AN-18.02.2019)
    {BillOfMaterial.NettoPreisGesamtFremdwährung}
)
else
(
    // Output own currency
    //(#440489-ΑΝ-18.02.2019) Multiply by BOM qty.
    {BillOfMaterial.NettoPreisGesamt}
);
```

**LineltemNetPricePerPiece:**
```vb
// Display the line item net price per unit
// Either in own or foreign currency depending on header setting
local numbervar lineItemNetPricePerPiece=0;
WhilePrintingRecords;

if ({Header.Währung} <> {Company.Eigenwährung}) Then
(
    // Output foreign currency
    lineItemNetPricePerPiece := {LineItems.NettoPreisStueckFremdwährung};
    if (NOT IsNull({#SumPieceBOMForeignCurrency}) AND NOT IsNull({BillOfMaterial.Menge}) )
    Then lineItemNetPricePerPiece := lineItemNetPricePerPiece + {#SumPieceBOMForeignCurrency};
    lineItemNetPricePerPiece;
)
else
(
    // Output own currency
    lineItemNetPricePerPiece := {LineItems.NettoPreisStueck};
    if (NOT IsNull({#SumPieceBOM}) AND NOT IsNull({BillOfMaterial.Menge}) ) Then
    (
        lineItemNetPricePerPiece := lineItemNetPricePerPiece + {#SumPieceBOM};
    );
    lineItemNetPricePerPiece;
)
```
Furthermore, the following total fields must be corrected. The fields for the group result must be changed:

-   For the field **SumPieceBOM**, `BillOfMaterial.NettoPreisGesamt` is entered.
-   For the field **SumPieceBOMForeignCurrency**, `BillOfMaterial.NettoPreisGesamtFremdwährung` is entered.

The image shows the "Edit Running Total Field" dialog in Crystal Reports where the "Field to summarize" is being set to `BillOfMaterial.NettoPreisGesamt` for the running total named `SumPieceBOM`.

### Problem: Incorrect Totals in Collective Printing
During collective printing of documents, the totals are not correct. The share of the first document per collective printout is missing. Not affected are the forms for the invoice printing! (see case 442306)

**Solution:**
The affected forms include an incorrect formula in some of the total functions. Affected are the following total formulas:
-   `CollectiveTotalGross`
-   `CollectiveTotalVat`
-   `CollectiveTotalNet`
-   `CollectiveTotalWeight`
-   `CollectiveTotalCircumfence`
-   `CollectiveTotalSqm`
-   `CollectiveTotalQuantity`
-   `CollectiveTotalGrossForeignCurrency`
-   `CollectiveTotalVatForeignCurrency`
-   `CollectiveTotalNetForeignCurrency`

A formula to reset the totals is used in these collective functions. The effect of this is that at the end of a collective printout, the total is set to 0 and the process begins from the start with the totaling for the next collective printout. This formula must be replaced completely with this corrected version:

```vb
// Reset totals before start of collective printout or if no collective printout is done
WhilePrintingRecords;

({Header.Sammelausdruckkennzeichen}=2
OR
{Header.Sammelausdruckkennzeichen}=0)
AND
previous({Header.Sammelausdruckkennzeichen}) <> 2;
```
This formula should be used in the "Reset" section of the Running Total Field properties.

### Problem: Accessing Previous/Subsequent BOMs
Sometimes, it is necessary to access previous or subsequent BOMs (Bill of Materials) within the detail block. For example, to output the description of the gas directly next to the description of the spacer.

**Solution:**
Since all reports of the reporting service are structured so that the BOM elements are output in the detail area, it is not possible to access the BOM elements directly. To receive the description of the gas when outputting the spacer, you can use the Crystal Reports internal function `next(x)` to access the data record that follows directly.

The designation of the BOM is composed in the function `@BOMDescription`. Then, with `next({BillOfMaterial.ErweiterteProduktbezeichnung})` you can access the description of the next element. So that this only happens when the current focus is on the record for the spacer, the product type/group of the current element must be queried before this.

Example formula:
`if( {BillOfMaterial.Produktart} = 60 AND Next({BillOfMaterial.Produktgruppe})=41) Then ...`

To prevent the gas description from being output twice (once next to the spacer and once in its normal position), a suppression formula for the detail block is required. This formula must be `TRUE` in order to suppress the output.

Example suppression formula:
`( {BillOfMaterial.Produktart}=30 AND {BillOfMaterial.Produktgruppe}=41 )`
This is `TRUE` in the case of a gas and thus its printout is suppressed.

To access the directly preceding data record, the function `previous(x)` exists analogously.

If it is necessary to access data records that are not directly preceding or directly after the current data record, this must be done via an array which must be declared as "shared." This array is filled in a function with the current data records and can then be used in another function. It is important to know that Crystal Reports iterates through the data records in several phases.
- The formula for filling the data records is executed first with the keyword `WhileReadingRecords`.
- The formula that outputs the data (e.g., `@BOMDescription`) is then executed with the keyword `WhilePrintingRecords`.

Both keywords must always be at the beginning of a formula to specify the time of the execution.

### Problem: "Net Prices" Code Not Considered
In the formula, the "net prices" code from the document header is not considered.

**Solution:**
In the formula, all fields that contain a discount or a gross price must be adjusted.
1.  Right-click on the field and select the "Format object" function from the context menu.
2.  On the dialog, select the first tab "General" and click on the formula button for the suppression formula.
3.  Extend the formula so that the "net price" code from the document header is considered for the suppression. The field is suppressed with the following statement as soon as "net prices" is active in the document:
    ```
    {Header.RabattDruck}<>0;
    ```
The current formula type `R0001deDE_OrderConfirmation.rpt` already includes this change.

### Problem: Incorrect Grouping in English Invoice Forms
The English forms for the invoice printing do not have the invoice number `{Header.InvoiceNumber}` as the main break group, but rather the invoice customer number `{Header.Invoiceld}` of the document. Thus, no invoice is generated per invoice number, but rather per invoice customer number.

**Solution:**
In the current standard forms that are provided via setup, this error has already been eliminated. To convert customer forms, take the following steps:
1.  Start the **Group Expert** (`Report > Group Expert...`).
2.  In the `Group Expert` dialog, select the flawed field `{Header.Invoiceld}` in the "Group By" list and click the **Options** button.
3.  In the `Change Group Options` dialog, replace the field `{Header.Invoiceld}` with `{Header.InvoiceNumber}`.
4.  Confirm all dialogs with OK and save the report.
After that, the break group has been converted to the correct invoice number.

### Problem: Empty Documents Do Not Print Header Information
If a document is printed that does not contain any items, no header information is printed. The printed document is therefore empty and unusable. At least the information of the document header should be printed.

**Solution:**
The reason for this problem is the "Inner Join" of the SQL query with which the report retrieves its data from the database. This "Inner Join" must be changed to a "Right Outer Join" so that documents without items are also output. In the current standard forms, this error has already been eliminated. To convert customer forms, take the following steps:

1.  Start the **Database Expert** (`Database > Database Expert...`).
2.  In the Database Expert, switch to the **"Links"** tab.
3.  Select the link between the **Header** and **LineItem** tables.
4.  Select the **"Link Options"** button.
5.  Change the link type from **"Inner Join"** to **"Right Outer Join"**.
6.  Exit all dialogs with OK and save the report.

### Problem: Product Structure Not Output
The product structure is not output although it has changed with regard to the previous item. (see also case 460661).

**Solution:**
The correction can be examined in the standard reports (e.g. `R0001deDE_OrderConfirmation.rpt`). There, the formula `"SuppressionFormfeed"` has to be transferred into the customer report and placed directly next to the output of the product description. After that, the field with the formula is suppressed so that it is not printed; it should only fill the variables.

### Problem: Mapping Print Table Columns to Database Columns
How can I find out which database column belongs to a print table column?

**Solution:**
With this `SELECT` statement, you can determine the referencing column from the DB for your field.

**For German field names (e.g., `Auftragsreferenz`):**
```sql
SELECT
    B.SourceName AS SourceTableName,
    A.SourceName AS SourceColName,
    B.TargetName AS Report_TableName,
    A.TargetName AS Report_ColName,
    A.Description,
    A.ActionType
from dbo.Core_ReportFields A, dbo.Core_ReportTables B
where A.ReportTableGuid = B.Guid AND A.TargetNamePhrases like '%Auftragsreferenz%';
```
**Example Result:**
| SourceTableName | SourceColName | Report_TableName | Report_ColName | Description | ActionType |
| :--- | :--- | :--- | :--- | :--- | :--- |
| BW_ANFR_POS | AUFTR_REF | EnquiryItems | EnquiryReference | Enquiry reference | 0 |
| BW_AUFTR_POS | AUFTR_REF | OrderItems | OrderReference | Order reference | 0 |
| BW_BEST_POS | AUFTR_REF | PurchaseOrderItems | OrderReference | Order reference | 0 |

**For English field names (e.g., `TotalPricePerUnit`):**
```sql
SELECT
    B.SourceName AS SourceTableName,
    A.SourceName AS SourceColName,
    B.TargetName AS Report_TableName,
    A.TargetName AS Report_ColName,
    A.Description,
    A.ActionType,
    A.TargetNamePhrases
from dbo.Core_ReportFields A, dbo.Core_ReportTables B
where A.ReportTableGuid = B.Guid AND A.TargetName like 'TotalPricePerUnit';
```

**To find the database column for a print table column (e.g., `AH_HAUPT_AUFTR`):**
```sql
SELECT
    B.SourceName AS SourceTableName,
    A.SourceName AS SourceColName,
    B.TargetName AS Report_TableName,
    A.TargetName AS Report_ColName,
    A.Description
from dbo.Core_ReportFields A, dbo.Core_ReportTables B
where A.ReportTableGuid = B.Guid AND A.SourceName like '%AH_HAUPT_AUFTR%';
```
**Example Result:**
| SourceTableName | SourceColName | Report_TableName | Report_ColName | Description |
| :--- | :--- | :--- | :--- | :--- |
| BW_ANFR_KOPF | AH_HAUPT_AUFTR | EnquiryHeader | MainEnquiryId | Main Enquiry number |
| BW_GUTSCH_KOPF | AH_HAUPT_AUFTR | CreditNoteHeader | MainOrderId | Main order number |
| BW_AUFTR_KOPF | AH_HAUPT_AUFTR | OrderHeader | MainOrderId | Main order number |
| BW_ANGEB_KOPF | AH_HAUPT_AUFTR | QuotationHeader | MainQuotationId | Main Quotation number |
| BW_BEST_KOPF | AH_HAUPT_AUFTR | PurchaseOrderHeader | MainOrderId | Main order number |

## 3.10.12. PDF file generation for the DMS archiving with Crystal Reports
In the form management, the template name of the PDF to be created by the A+W SOA Reporting Service will be saved.

In the "Form Management" dialog, under `4.Options 1 > Archiving of documents`, you can specify a `PDF template` path.

-   **Active:** Check this box to enable DMS archiving.
-   **PDF template:** Define the file name structure using control codes.

Example template:
`<<PDFDIR>>100-<<ID>>-DMS BRA-<<DATE>>-<<TIME>>.pdf`

-   The tag `<<PDFDIR>>` is replaced during printing with the directory in which the file should be created.
-   The tag `<<ID>>` will be replaced with the document number.
-   You can also use `<<DATE>>` and `<<TIME>>` for the current date and time.

Example output file name:
`\\SERVER01\Mandant0815\100-47110815-DMS BRA-20190625-120000.pdf`

The value `100` after the storage directory stands for the print code of the document to be printed (here, 100 = order confirmation).

During the printing process, the AWSOA Reporting Service reads the information and creates the PDF file for the DMS archiving. Then the AWSOA Exchange Service transfers the PDF file to the DMS system and deletes it from the storage directory.

## 3.10.13. User name and print job number in the printer queue
The Reporting Service sends all print jobs with the user name that executes the Reporting Service. This means that it cannot be distinguished who started the print job. For this reason, the document name in the printer queue is used to display the user name and number of the print job.

Due to a Windows security guideline, the document names are only visible for the user who started the print job. To work around this, each user who wants to see the document name must have administrator rights on the print server.

The number of the print job is in the **Number** column in the A+W Business print job overview. This way, the print job in question can be started again if necessary.

## 3.10.14. Employee's sender when sending forms
Normally you use the configuration in the infrastructure or the "Different sender" field in the form management to control which sender address should be used when sending forms via e-mail.

With a new option in the form management, the sender can now be changed to the employee's e-mail address if this is entered. When this option is activated, the employee's address always takes precedence over the other two settings. This option is labeled "Absender des Mitarbeiters" in the UI.

## 3.10.15. Dimension type of muntin drilling points
The dimension type is now available for the output of the muntin drilling points in the Crystal Reports form. A+W Business internally saves all drilling points as a chain dimension. However, if the dimensioning type is set to "to reference point," the distances must be added up in a formula within Crystal Reports to ensure the printout corresponds to the input. This evaluation takes place in a formula named **"PrintGB"** found in the standard form for OC printing `"R0001deDE_OrderConfirmation.rpt"`.

## 3.10.16. Send file attachments via e-mail
If a printout is sent by e-mail, it is now possible to send any file in addition to the PDF file with the actual printout. These files must be located in the Crystal Report forms folder. This folder is found in the company master data on tab **"12.Print"**.

In the company master data, the path is specified under `Form printout via Crystal Reports > Path`.

The files are stored per form in the form administration. If there is more than one file, the file names must be separated by a semicolon (`;`). In the form management, the files are listed under the "Attachments" field.

In the print program, the file attachments appear in the table on tab **5.Attachments** when the form is selected. They are always appended by default but can be deselected by unchecking the checkbox.

## 3.10.17. Individual cover letter for mail dispatch
It is now possible to enter placeholders in the system text for the e-mail cover letter. These placeholders can be provided by the print program with any text to design the e-mail individually.

1.  Use placeholders in the system text in the format `<<text1>>`, `<<text2>>`, etc. Each placeholder must be supplied with a text from the print program.
2.  Assign this system text to the `Mail body` in the form administration.
3.  When the form for e-mail dispatch is selected in the printing program, the tab **4.Cover letter(mail)** is activated.
4.  Here, the required placeholders must be provided with texts. Predefined text modules can be created in the text management and selected here.

The Reporting Service uses the system text, replaces the placeholders with the texts specified in the print program, and converts the RTF to HTML. Bitmaps or tables used in the texts in the print program cannot be transferred to the cover letter.

## 3.10.18. Output in PDF file
To reroute the output of the form printing to a file, it is possible to store a path and file name in the form management. It is recommended that you use a UNC path to which the reporting service has access. The file name can be provided with placeholders.

The available placeholders are displayed when clicking on the button in front of the file name field:
- `<<ID>>`: Document Number
- `<<PDFDIR>>`: DMS Path
- `<<TYPE>>`: Print Point (Numeric)
- `<<USER>>`: User Name
- `<<LENR>>`: Declaration of Performance Number
- `<<DATE>>`: Date (yyyyMMdd)
- `<<TIME>>`: Time (hhmmss)

Example PDF File setting: `OrderConfirmation-<<ID>>-<<TYPE>>-<<USER>>.PDF`

For the output to go to a file, the output in the form printing has to be set to "File" with the radio button "Output to...".

## 3.10.19. Reprint
With a new functionality for repeated printing of forms, it is now possible (e.g., in case of a paper jam or for troubleshooting) to start an output with the Crystal Report form again.
-   Only the existing data at the time of the initial printing is printed out with the form current at the moment.
-   No data in the A+W Business database is used (no status check, no document locking, no stock removal, no invoice number generation).
-   Only the output of the document is stored with the current report in the AWSOA database and output on the original printer.
-   If the initial printing was sent via mail, the mail will be sent again, and a security query will appear.

To reprint a document, right-click on the desired print job in the "Druckaufträge" (Print Jobs) overview and select the **"Erneut drucken" (Reprint)** option.

## 3.10.20. Not supported RTF tags
Crystal Reports does not support all RTF tags. For details, use the following link to the SAP homepage:
[https://apps.support.sap.com/sap/support/knowledge/en/1214798](https://apps.support.sap.com/sap/support/knowledge/en/1214798)

Essentially, only texts should be used. Bitmaps and tables that are stored in A+W Business as RTF text will not be, or will only be incompletely, printed out. The complete RTF code might even be output as plain text.

## 3.10.21. PDF file names in mails
When sending forms via mail, it is now also possible to store a name for the PDF file. Previously, the name of the mail subject line was used. If no PDF file name is stored in the form, the program uses the mail subject line as before.

## 3.10.22. Customizing for mail subject line and PDF file name
In the form management, it is now possible to execute customizing functions for the mail subject line and for the PDF file name by using `<<FX(1234)>>`, where `1234` corresponds to the number of the formula.

The customizing function is called once for each document that should be printed. Transfer of data to the customizing formula is done via the following variables:
-   `m_nCurrentRow`: The index of the current row in the row array `m_Row[]`
-   `m_nCountRows`: The number of all rows to be printed in the row array `m_Row[]`
-   `m_Row[*]`: The array with all documents to be printed.
-   `m_Row[*].m_sPrintId`: The Print-ID of the respective row. All documents with the same Print-ID are output in the same PDF file. The Print-ID is only valid up to the current element.
-   `m_Row[*].m_nNUMMER`: The document number of the element.
-   `m_Row[*].m_nSTATUS`: The status of the element.

An example of such a formula is found on the diskset under the folder `...\Formula\Crystal Reports Formulas`.

## 3.10.23. Separate PDF files in the mail attachment
In the company master data, a setting allows you to select whether each document is sent in a separate mail or if all documents for a partner are written together in one PDF file.

-   **Company Master Data Setting (`12.Print` tab > `Fax/Email-options`):**
    -   `Email dispatch per document`: When checked, each document is sent in a separate email.
    -   `1-Email dispatch as PDF file`: When checked, documents for one recipient are combined into one email.

This setting can be overridden in the customer master data.
-   **Customer Master Data Setting (`2.Order` tab > `Document dispatch` > `Mail options`):**
    -   `0 - Standard (Company master data)`
    -   `1 - per document`
    -   `2 - per customer - documents together`
    -   `3 - per customer - documents individually`

The table below shows the behavior for different setting combinations:
| No. | Customer setting | Form setting | Result |
| :-- | :--- | :--- | :--- |
| 1 | `1 - per document` | Duplex printing: OFF | Several mails with one document apiece. Several PDFs for DMS. |
| 2 | `1 - per document` | Duplex printing: ON | Several mails with one document apiece. Several PDFs for DMS. |
| 3 | `2 - per customer - documents together` | Duplex printing: OFF | One mail with a PDF that contains several orders. One PDF for DMS that contains several orders. |
| 4 | `2 - per customer - documents together` | Duplex printing: ON | Several mails with one document apiece. Several PDFs for DMS. |
| 5 | `3 - per customer - documents individually` | Duplex printing: OFF | One mail with several PDF documents. Several PDFs for DMS. |
| 6 | `3 - per customer - documents individually` | Duplex printing: ON | Several mails with one document apiece. Several PDFs for DMS. |

> **Note:** With the activated option "Transfer in iQuote" in the form management, the mail dispatch option "2 - per customer - document together" is overridden, and a PDF per document is generated.

## 3.12.2. Form management change of the date data type in the Reporting Service
Starting with version 13.04.7949 of the A+W Infrastructure 6 Reporting Services, the data type of some date columns was changed from `Datetime` to `Date`. This requires acting for formulas in which the function `ToText(...)` and/or `Date(...)` is used.

Crystal Reports doesn't recognize the data type `date` and interprets this column as a string of characters, which can lead to error messages like:
`"Error in formula <FORMELNAME>: 'WhilePrintingRecords;'A date/time entry is required here."`

A flawed formula might look as follows:
- `ToText ({DateField}, "dd.MMM.yyy")` -> **Error**
- `ToText (Date({DateField}), “dd.MMM.yyy“)` -> **Error**

The correction is to convert the field to a CDate first:
- `CDate({DateField})` -> **Correct**

After converting with `CDate`, you can again set the desired date format via the field's properties.

**List of changed columns (datetime to date):**
| Table name | Column name |
| :--- | :--- |
| CreditNoteHeader | CreditNoteConfirmationDate |
| CreditNoteHeader | CreditNoteDate |
| CreditNoteHeader | DeliveryDate |
| ... | ... |
| OrderHeader | OrderConfirmationDate |
| ... | ... |
| QuotationHeader | ShipmentDate |
*(For the complete list, refer to pages 40-41 of the source document.)*

## 3.13. Stopping the reporting service
The reporting service can be stopped in the IceGrid (Service Locator). If it doesn't stop, it may be due to dependent processes. This is an alternative to restarting the entire server.

1.  Attempt to end all reporting services with the Service Locator.
2.  If at least one does not stop, take its process ID (PID).
3.  Open Task Manager, go to the `Details` tab, and find the process.
4.  Right-click the process and select **"Analyze wait chain"**.
5.  The "Analyze wait chain" dialog will show which other processes are blocking it (e.g., `splwow64.exe`).
6.  Select the blocking process in the tree and click **"End process"**.

## 3.14. Crystal Report+Workflow mail with Office365 + OAuth2
Starting in September 2025, Microsoft will completely switch off basic authentication (user/password) for Office365. The Crystal Report Service of A+W Business now supports token-based authentication via OAuth2 using MailKit.

### Configuration
The configuration is done in the infrastructure configuration tool.
1.  Navigate to `Workflow > Mail`.
2.  Check **Use MailKit**.
3.  Set **Authentication Type** to `Office365`.
4.  Enter the `Server name` (`smtp.office365.com`) and `Port` (`587`).
5.  Enter the **Tenant ID** and **Client ID** from your Azure App Registration.
6.  Enter the **Azure Account** (domain log-in name, e.g., `dlangsdorf@a-w.com`).
7.  Enter the **Sender address**.

> **CAUTION:** The authentication of Office365 must be done under the domain that is also running the ICE node infrastructure. The user must be a domain user.

### Authentication
Authentication happens in the "A+W Infrastructure Reporting Config" tool.
1.  Press the **"Authentication and mail dispatch"** button.
2.  The Azure authentication dialog opens. Enter your password and, if necessary, the MFA.
3.  A token is created, and a test mail is sent to the sender address.

> **CAUTION:** The test mail will be sent to the sender of the mail. If this should differ from your mail account, you should enter yourself in CC.

### 3.14.1. Saving of the tokens
After authentication, the tokens are saved in a token cache file in the `%PROGRAMDATA%` folder:
`C:\ProgramData\A+W\Clarity\Clarity.Mail.MailKit.0365.MSAL.Storage.bin`

### 3.14.2. Configuration OAuth2 in Azure (Office365)
The system administrator must perform these steps in advance.

**Creating the application:**
1.  Go to the [Azure portal](https://Portal.azure.com) and log in with an administrator account.
2.  Search for **"App registrations"** and click **"+ New registration"**.
3.  **Register an application:**
    -   **Name:** Give your application a user-facing display name.
    -   **Supported account types:** Select `Accounts in this organizational directory only (Single tenant)`.
    -   **Redirect URI (optional):** Select `Public client/native (mobile & desktop)` and enter the default URI: `https://login.microsoftonline.com/common/oauth2/nativeclient`.
4.  Click **Register**.
5.  After registration, the overview page will display the **Application (client) ID** and the **Directory (tenant) ID**. You need these for the infrastructure configuration.

Deviating dispatch addresses (e.g., per form) must be entered in the Exchange Admin Center.

### 3.14.3. Tracing
-   **A+W Business Exe:** The trace is found in `Commercial.ComProxy*.awtrc`. Search for `"SendMailKit"` to see the user, token store location, and number of tokens.
-   **Reporting Service:** The sending is done via the Ice Service; the core tracing must be switched on. In the A+W Protocolling Config tool for `Commercial ComProxy`, set the Trace Level for `Core` to `Info` or higher.

### 3.14.4. Workflow mail in A+W Business
In A+W Business, the configuration is done in the company parameters.
-   Check **Use MailKit**.
-   Set **Authentication type** to `2-Office365`.
-   Fill in the Server, Port, Client no. (Client ID), Azure user, and Sender address.

**Workflow Function:**
Mail can be sent with this function.
`Boolean = udf_SendMailEx( sFrom, sTo, sCC, sBCC, sSubject, sBody, sHTMLBody, sAttachmentNames, bAllowInteractive )`

-   **Description:** Sends an E-Mail via Mailkit or Standard mail based on the settings of the company data.
-   **bAllowInteractive (Boolean):** If `TRUE`, allows interactive authentication.

On first use, authentication must be performed for each computer and user. For workflow execution, the user who starts the Exchange service node must perform this authentication on the computer where the service is running.

## 3.15. El = electronic invoice (XRechnung, ZUGFeRD)

### 3.15.1. Introduction/requirements/architecture
**Introduction:**
Starting on 1/1/2027, the creation of electronic invoices is prescribed. The two permissible formats are:
-   **CII - Cross Industry Invoice:** [www.unece.org/cefact/xml_schemas/index](http://www.unece.org/cefact/xml_schemas/index)
-   **UBL - Universal Business Language:** [docs.oasis-open.org/ubl/cs1-UBL-2.1/UBL-2.1.pdf](http://docs.oasis-open.org/ubl/cs1-UBL-2.1/UBL-2.1.pdf)

ZUGFeRD is a hybrid data format that integrates structured invoice data in the XRechnung CII format into a PDF document (PDF/A-3). A+W Business supports:
-   ZUGFeRD 2.3.2 - CII 22B
-   XRechnung UBL 3.0.2
-   XRechnung CII 22B

A free online viewer is available at: [https://www.invoice-viewer.de/](https://www.invoice-viewer.de/)

**Prerequisites:**
-   The Reporting Service and B2B Service must be installed.
-   The export format must be defined per customer.
-   A series of master data must be entered.
-   Only the Crystal Report Service supports the creation of e-invoice formats (no Gupta forms).

**Architecture:**
The Reporting Service controls the creation and dispatch of the electronic documents. It uses the B2B Service to generate the XML data, which is then embedded into the PDF created by Crystal Reports.

**Flowchart:**
1.  **Form printing dialog** in AWB sends a print request with B2B settings to the **Reporting Service**.
2.  The **Reporting Service**'s `BusinessReportingCOM` component calls the **Business B2B Service** (`CreateB2BDocument`) to generate the XML invoice data.
3.  The **B2B Service** returns the XML data and a KSEF ID.
4.  The **Reporting Service**'s **Crystal Reports** engine generates the visual PDF.
5.  The XML data is embedded into the PDF, creating the final e-invoice.
6.  The file is then dispatched via **Mail** or saved to a **File** location.

## 3.11. Management tool Crystal Reports forms

### 3.11.1. Preparation and important notes
-   Before using the new Crystal Report Management tool, the AWSOA database and the Crystal Reports forms **must be backed up**.
-   To prevent changing original forms, you should work in a test directory. The path for Crystal Reports forms can be set in the company master data (`12.Print` tab).
-   Report groups 1 to 6 are pre-defined and cannot be changed. If you create a new report group (number > 6), it will generate new report tables not used by the standard reports and application.

### 3.11.2. Introduction
To improve performance for print jobs with many documents, a management tool was created to define your own, reduced Crystal Reports report groups. You can create a new group based on an existing one, but with a smaller, optimized set of data.

### 3.11.3. Creating a report group
1.  Open the **Crystal Reports administration(SOA)** tool.
2.  On the `1.Reports` tab, select an existing report type (e.g., `002-Order confirmation`) as a base.
3.  Enter a new `Name` and `Group` number (e.g., 007) for your new report group. This creates a copy of the existing group.
4.  On the `2.Groups` tab, select your new report group (`007`).
5.  In the **Dataset Definition**, uncheck the "Active" box for any tables or columns that are not needed for your specific report.
6.  Go to **Form Management**, create a new form or modify an existing one, and assign your new **Print service report** group (`007 - Order confirmation AUW60`) to it.

### 3.11.4. Optimizing a report group
After a Crystal Report is assigned to a form with your new report group, you can optimize the data set.
1.  In the management tool, select your report group.
2.  Click **Optimize**. A dialog will open showing all forms that belong to the group.
3.  Clicking OK will optimize the report group's data set based on only the fields actually used in the assigned Crystal Reports forms. This reduces the data queried and improves print time.

### 3.11.5. Optimizing Crystal Report
If you need to add a field back to a Crystal Report:
1.  In the management tool, load the report group and go to the `2.Groups` tab.
2.  Find the field you need and check the **Active** box to reactivate it. Save the changes.
3.  Open the Crystal Report form (`.rpt` file).
4.  Right-click on **Database Fields** and select **Set Datasource Location**.
5.  In the "Set Datasource Location" dialog, update the table that now contains the new field.
6.  If a whole table was re-activated (e.g., Customers), you must add it back to the report. Right-click on **Database Fields** and select **Database Expert...**.
7.  In the Database Expert, find the table under your connection, add it to the "Selected Tables" list, and give it the correct alias (e.g., `Customers`).
8.  Go to the "Links" tab to ensure it is correctly joined to the other tables. The customer data will now be available in the report again.

## 3.12. PDF generation in form printing

### 3.12.1. Settings
Several settings control PDF generation during Crystal Reports form printing:
-   **Support of double-sided printing** in form management (`Steuerung > Unterstützung beidseitiger Druck`).
-   **Document dispatch – mail options** in the customer master data.
-   **Mail dispatch per document** in the company data.

See the table in section **3.10.23** for a detailed breakdown of how these settings interact.

## 3.10.24. Carbon copy function / watermark
To activate the carbon copy function, enter the number of copies in the form management on tab `4. Options 1`. The Reporting Service will then output the specified number of copies for each print job.

To output a watermark on the copies, the column `{Header}.{CarbonCopyNumber}` (or `{Header}.{Durchschlagsnummber}`) can be used. The value is `0` for the original and `1`, `2`, etc. for the copies.

Since Crystal Reports does not have a native watermark function, a bitmap (e.g., an image of the word "Kopie") can be added to a section in the page header.

1.  In the Section Expert for the page header section containing the bitmap, activate the option **"Put beneath the following sections"** ("Folgende Sektionen unterlegen").
2.  Use the object formatter to create a suppression formula for the bitmap so it is only displayed on the copies:
    ```
    {Header.Durchschlagsnummer}=0;
    ```
This formula suppresses the bitmap when the copy number is 0 (the original).

## 3.10.25. Print QR codes
To print QR codes with Crystal reports, the QR code font and DLL from IDAutomation is used. This can be downloaded as a trial version but must be licensed by the customer.

**How to install:**
1.  Download the **QR Code Font and Encoder Package** from idautomation.com.
2.  Run the installer executable (e.g., `IDAutomation_QRCodeWindowsFontEncoderDEMO.exe`).
3.  In Crystal Reports, two new functions will be available under `Functions > Additional functions > COM and .NET UFLs (u212com.dll)`:
    -   `IDAutomationQRCodeEncoderQRSet`
    -   `IDAutomationQRCodeEncoderQRGet`

**Create a formula in Crystal Reports to generate the QR barcode string:**
```vb
stringVar DataToEncode:= ToText({Header.Angebotsnummer});
stringVar CompleteBarcodeString:="";
numberVar i:=0;
numberVar Segments:= IDAutomationQRCodeEncoderQRSet(DataToEncode,0,0,0,0,0,0);
For i:=0 to Segments Do
(
    CompleteBarcodeString := CompleteBarcodeString + IDAutomationQRCodeEncoderQRGet(i);
);
CompleteBarcodeString
```
-   Adjust the value to be coded (e.g., `{Header.Angebotsnummer}`).
-   Insert the formula field into the report from the Field Explorer.
-   Assign the **IDAutomation2D** font to this formula field.

> **Note:** The DEMO version will prefix the encoded data with the word "DEMO" and the resulting QR code will be unusable.

## 3.10.26. Saving the login data in the Crystal Report
Login data is now saved in Crystal Report and compared to the current login data at execution. If they are the same, the report executes much faster.

This only happens if the SOA database is accessed via Windows authentication. Crystal Reports does not allow storing a password for a database login in the report.

> **CAUTION:** If you make changes to a report locally and update its data source, it will save your local database connection info. This report will then fail to run at the customer site. Therefore, **always delete the login data from the report's comments before deployment**.

To delete login data:
1.  Open the report in Crystal Reports.
2.  Go to `File > Summary Info...`.
3.  Clear the text in the **Comments** field (which may contain XML-like connection strings, e.g., `DBSchema=0.70`).
4.  Save the report.

## 3.10.28. Timeouts in case of several network adapters
If computers have multiple network adapters (e.g., to separate production and commercial networks), timeouts of up to 30 seconds can occur when starting A+W Business or printing. This is caused by the Ice Service Locator searching for services on unreachable network segments.

**Solution 1: Blacklist**
In the A+W Infrastructure Config tool, add the IP ranges to exclude to the `Blacklist - IPs (optional)` field, separated by semicolons. Wildcards are supported (e.g., `10.3.3`).

**Solution 2: Fixed IP Addresses (Complete Fix)**
To stop timeouts completely, the Ice configuration must use fixed IP addresses.

1.  **Determine the Service Locator IP:** Find the hostname of the service locator in the registry at `HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Albat+Wirsam\Communication` under the `IceHost` key. Resolve this hostname to its IPv4 address.
2.  **Edit `config.registry`:** Open the file `C:\SANDPIPER1\InfrastructureServiceLocator\config.registry`.
3.  **Update Endpoints:** Replace `default` or existing IPs with the hardcoded IP address of the service locator for the following settings:
    -   `IceGrid.Registry.Client.Endpoints`
    -   `IceGrid.Registry.Server.Endpoints`
    -   `IceGrid.Registry.Internal.Endpoints`
    -   `IceGrid.Registry.AdminSessionManager.Endpoints`
    -   `IceGrid.Registry.SessionManager.Endpoints`

    Example: `IceGrid.Registry.Client.Endpoints=tcp -h 194.39.66.73 -p 12000`
4.  **Update IceStorm in IceGrid:**
    -   Open the IceGrid GUI.
    -   Find the IceStorm service definition.
    -   Open its definition for editing.
    -   Update the `topic-manager-endpoints` and `publish-endpoints` with the hardcoded IP address of the service locator.
    -   Save the changes.

