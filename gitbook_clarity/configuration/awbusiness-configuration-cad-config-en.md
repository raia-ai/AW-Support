---
description: "EN-CONFIG-AW_Business-3"
---


---
## 2.13. Saving of TOE files of the CAD Designer (Shapes) in the database

The files of the CAD Designer (Shapes) have also been stored in the database since version 13.04.0637, insofar as these are files from the technical order entry (iTOE). These TOE files have as file name behind the automatically generated batch number also the abbreviation "_TOE" (e.g. 0023145_TOE.SN). This has the advantage that the database is sufficient for describing the item completely. As soon as the database is available, all TOE files also exist.

The system behavior is such that for access to a TOE file that is specified in a shape set, first there is a check whether the file exists. If so, then everything goes as previously and the file is displayed. If the file does not exist, the system checks whether a there is a file in the database and creates the file. From that moment, everything goes as previously. Attention must be paid that the path to the CAD files in the company master data has been entered correctly.

Another advantage is that the saving of the TOE file happens in the same transaction as the saving of the item itself. Thus, the file always corresponds to the state of the item.

The file is stored in the database in the shape table (BW_xxxx_MODELL) in the SN column. Because this is a BLOB column, it is not possible to output the data with Management Studio. However, it is possible to create a stored procedure with T-SQL that generates the CAD files.

### 2.13.1. Extracting the CAD files from the database with T-SQL

The following script creates a stored procedure in the database and can be executed with "exec save2file".

```sql
SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO
CREATE PROC [dbo].[save2file]
AS

declare @ObjectToken INT
declare @TheContent VARBINARY (MAX)
declare @Save2File VARCHAR(255)
declare @id int
declare @FileName varchar(255)

DECLARE TheCursor CURSOR FAST_FORWARD FOR
SELECT MOD_SN_NAME, SN
FROM SYSADM.BW_AUFTR_MODELL WHERE ID = 60000072 AND POS_NR = 1

OPEN TheCursor
FETCH NEXT FROM TheCursor INTO @FileName, @TheContent

WHILE @@FETCH_STATUS = 0
BEGIN
    SET @Save2File = 'C:\Temp\' + @FileName
    PRINT @Save2File

    EXEC sp_OACreate 'ADODB.Stream', @ObjectToken OUTPUT
    EXEC sp_OASetProperty @ObjectToken, 'Type', 1
    EXEC sp_OAMethod @ObjectToken, 'Open'
    EXEC sp_OAMethod @ObjectToken, 'Write', NULL, @TheContent
    EXEC sp_OAMethod @ObjectToken, 'SaveToFile', NULL, @Save2File, 2
    EXEC sp_OAMethod @ObjectToken, 'Close'
    EXEC sp_OADestroy @ObjectToken

    FETCH NEXT FROM TheCursor INTO @FileName, @TheContent
END

CLOSE TheCursor
DEALLOCATE TheCursor
GO
```

In the script, the path for the output (@Save2File) and the select statement for the selection of the shape must be adjusted for the given requirements.

Here, the TOE files are created by the database server, therefore it is important that the path must always be defined from the database server. This means that the path C:\Temp\ is not that of the client, but the path on the database server. If error messages occur during execution, the authorizations for executing the OLE automation functions probably do not exist. This can be achieved for the database server with a right-click on the server instance in Management Studio and selection of the "Facets" function.

In the dialog that opens, on the "Facet" combo box, the entry "Surface Area Configuration" is selected and both marked switched "OleAutomationEnabled" and "XPCmdShellEnabled" are set to True.

*Image: View Facets - AN-DEV13, showing OleAutomationEnabled and XPCmdShellEnabled set to True.*

## 2.14. Integrated Technical Order Entry (iTOE)

For start-up of the TOE, the scripts 20180810a.sql, 20190516a.sql and 20190516m.sql are absolutely necessary. Furthermore, the module (module number 159) requires a license. Microsoft SQL Server 2016 is required as the database system!

At the start, master data is not absolutely necessary, the system is "self-learning." After each import, the articles that correspond to no rules are displayed and they can be created there during the comparison and also changed.

*Figure: The rule editor*

The master data consists of rules with which it is specified which article should be transferred to the BOM during the comparison. These rules can either be created at the beginning in the rule editor (Master Data > Products > Articles > iTOE rules) or defined during the import. The rules are processed in the sequence of the specified priority.

In the processing entry, the comparison can be started either with a DXF file import or with the "iTOE" button on the ribbon (<CTRL>+<SHIFT>+<X>). In the CAD Designer, you make the changes to the glass unit and take over the data about the menu element "File > Save with File" or "File > Save without File" from there. With this, either an SN file (called TOE file below) should be created in the BOM or not. If an SN file is created, the comparison independently inserts a shape set if it does not exist yet and links the TOE file created. You can recognize the TOE files from their file names in the form XXXX_TOE.SN. Whereby the number at the front is determined by the number ranges of the SN files.

As soon as the changes have been applied, A+W Business displays the result of the rule check on a dialog.

*Figure: The result of the product comparison*

If a product was found for each processing, it will be displayed as in the example. If for a processing no rules applies, you can see this from the line with the dark background and from the fact that the article number is missing. Now with the "Edit rule" button, you can change directly to the rule editor in order to create the appropriate rule. Already-created rules can also be changed with this button. After you exit the rule editor, there is always a new comparison and the changes you just made to the rules display their effects immediately.

If you confirm the result of the product comparison, the complete BOM is generated in the processing entry and provided with the appropriate prices. The system compares changes that are now made in the processing entry with the TOE file. Changing properties that are not a component of the A+W processing type catalog are lost in the process. Such changes have to be made in the CAD Designer. For example, if a drilling row has series dimensions. These series dimensions would be deleted as soon as one of the participating drillings is changed in the processing entry.

### iTOE rules with priority

**Application example with correct creation of rules**
LAMI and TGH and a corner cut-out:
*   **Rule 1:** Corner cut-out **polished** on TGH (prio 2 with edge quality "polished")
*   **Rule 2:** Corner cut-out on TGH **arrissed** (prio 3 with edge quality "arrissed")
*   **Rule 3:** Corner cut-out on TGH **without edge quality** (prio. 4 with edge quality "not defined")

In this case, the program goes through the rules and processes them using the existing priority starting with 0 as well as reacts to the manual settings made during import on the DXF import dialog with regard to the selected edge qualities.

In the example described above, we assume that the user would like to map case 2 and selects corner cut-out on TGH arrissed accordingly (checked combo box in Figure 1).
Here, the program finds rule 2 and selects it because it is the first one found where all criteria are met.

Rule1 is checked as 1., but it is skipped since the edge quality does not match the manual selection on the DXF import dialog.

**Application example with incorrect creation of rules.**
LAMI and TGH and a corner cut-out:
*   **Rule 1:** Corner cut-out polished on TGH (prio 2 with edge quality "polished")
*   **Rule 2:** Corner cut-out on TGH arrissed (prio 3 with edge quality "arrissed")
*   **Rule 3:** Corner cut-out on TGH without edge quality (prio 1 with edge quality "not defined")

In the example described above, we assume that the user selects nothing on the import dialog when making the corner cut-out on TGH (figure below).

*Image: DXF Import and Product Zuordnung dialogs.*

Here, the program finds rule 3 and selects it. (2. Figure below)
In this example, the program actually always selects rule 3 since it is created with the highest priority and through the creation "without consideration of edge qualities" is always correct, regardless of what the user selects during DXF import.

### 2.14.1. Restrictions and configuration
For processings that have an edge quality (drillings, cut-outs), during the DXF import, the edge quality must always be defined on the import dialog; the iTOE rule must consider the edge quality and then select the product that corresponds to the edge quality. In A+W Business, the edge quality is not saved in the order; instead, it always comes from the base product. IF no quality is defined, the one from the master data processing is always used.

### 2.14.2. Shape rotation
See the SN.INI configuration under 16.17 shape rotation in the iTOE and DXF import

### 2.14.3. Rules with workflow formula
A formula can be stored as condition in the rule editor. Chapter 10.32 explains how this is to be implemented.

## 2.15. Document check (dual control principle)

The user can use the context menu to call up the check of the order from an existing number manager. The call is only possible for single documents.

*Fig. 57: Number manager context menu*

Now a dialog opens on which all items with their complete BOM are displayed. However, no production BOM breakdown is displayed. The user can check the data and mark each item as "OK." Separate tabs have been developed for checking header and item texts, which contain an overview table and a display of the actual text. In the item table on tab "1. Header/item data", the line header indicates whether an item text exists.

Double-clicking on the item line takes you directly to the tab.

*Fig. 58: Document check incl. header and item texts*

*Fig. 59: Item text (Image of a star shape)*
*Fig. 60: Header text (Image showing "THIS A TEST MESSAGE!")*

If all items (marked with an X in the example) were found to be "OK," the check flags are written to the items after pressing "Execute." The order is then set to the user status of the new status point "167 - Check performed" and a history entry is written.

*Fig. 61: Marking the checked order items*
*Fig. 62: New order status "check performed"*

The user can exit the check at any time. The items already checked are displayed again in case of another call. The new status of the order is visible in the number manager; thus, no new ID is required in the number manager. If a correction has to be made, then the user goes into the document entry via the context menu and makes the correction. Then he calls up the check again and marks it after successful checking of the item as OK (checkmark on the screen table). Now the status is incremented if the order has been checked completely.

In the screen table, it is possible to attach a customizing as you can do in the number manager (user-defined field) in order to reload particular information (see 10.30)!

*Fig. 63: Customizing in table in order to reload order information*

## 2.16. European article numbers (EANs) for variants and stock dimensions

In order to be able to use the EAN for variants and stock dimensions, the scripts 20200616a.sql and 20200616aa.sql for the archive are required. In the management programs for the variants and the stock dimensions, the fields for the EAN can then be edited and saved.

*Image: Stock Sizes and Product Variants/Colours dialogs showing EAN fields.*

The EANs entered there are saved during item entry in the item and in the BOM. If for an item there is an entry for the variant and one for the stock dimensions, the EAN of the variant always wins.

The EAN can be output with the reports for Crystal Reports. The fields for this are `{R0001deDE_PositionenErweiterung.EAN}`, `{R0001deDE_AuftragsStueckliste.EAN}` and `{R0001enUS_OrderItemsExtension.EAN}`, `{R0001enUS_OrderBillOfMaterial}`.

The transfer to production is done with the OrderXML Version 5.5 and higher.

## 2.17. Entry help postal code/city in document entry

A new database table called KA_POSTAL has been developed, in which data (postal code directory) can be imported from an Excel or CSV file via DB script. Such postal code directories are relatively easy to find on the Internet.
Ex.: `https://www.suche-postleitzahl.org/downloads`

If there are data records in the table, both the postal code and the city are in the header entry selection boxes, which fill in their content automatically during entry. As long as the header entry is open, the contents are retained. The selection boxes also contain only the entries that suit the user's entry. If a place is selected, then the associated postal code is loaded into the selection box and displayed. The same thing works the other way around.

*Images: Order entry dialog showing automatic fill-in for postal code and city.*

## 2.18. Due date calculation mode

You can set the due date calculation for every single customer. Calculation will be based on the invoice date stated in the order. Only mode 11 is based on the delivery date. The mode defines how due dates should be calculated for this customer. When you select a mode, a short text appears along with the calculation. The following calculation modes are available:

*Image: Customer master data screen showing due date calculation options.*

1.  **0: Date of issue:** The invoice is due immediately.
2.  **1: Date of issue + payment term:** By default this is invoice date + 30 days but other payment terms can be entered if required.
3.  **2: Date of issue + payment term rounded to 1. Date of payment or month's end:** If a date of payment is defined, the due date is calculated from the rounded total of date of issue + payment term. If no date of payment is defined, the date will be rounded to the month's end.
4.  **3: Date of issue + payment term, rounded to the 15th day of the month or end of month:** Like 2, rounded to the 15th day of the month or to month's end.
5.  **4: Date of issue + payment term rounded to the 10th or 20th day of month, or end of the month:** Like 2, rounded to the 10th or 20th of the month, or to month's end.
6.  **5: Date of issue + payment term + end of month:** Payment term will be added to the date of issue and then rounded to month's end.
7.  **6: Date of issue + month's end + payment term rounded to first payment date:** Like 5, rounded to the first payment date.
8.  **7: Date of issue + payment term, rounded to first, second, or third payment date:** Like 5, rounded to the next payment date in line.
9.  **8: Date of issue + payment term depending on the second payment date, rounded to the first or third payment date:** Like 5, rounded to the first or third payment date.
10. **11: Due date = delivery date + payment term:** Delivery date + payment term.

> **Warning:** With mode 5 and 6, the value in the Gross days field (payment term) should be divisible by 30. 30 Days = 1 Month, 60 Days = 2 Months, 90 Days = 3 Months, by which the 1st reference date will be increased.

## 2.19. Electronic invoice for the Polish market (Comarch/KSeF)

To start up the interface to the service provider Comarch and its reporting of the KSeF ID, the latest version of the following components is required:
*   A+W Business 6 (incl. Update Script 20240328a.sql)
*   AWSOA Commercial 6 B2B Services
*   AWSOA Infrastructure 6 Services

Initially the access data for the Comarch WebService is required, which must be stored in A+W business in the company master data on the tab "16.Miscellaneous".

*Image: A+W Business company master data screen, "16.Miscellaneous" tab, showing Comarch/KSeF user and password fields.*

In addition, it must be entered per customer whether electronic invoicing should be executed. In the customer master data, there is a selection box for this on the tab "2.Orders".

*Image: Customer master data screen, "2.Order" tab, showing "Electronic invoice" checkbox.*

The next step is the definition of the workflow through the suitable storage of user, minimum, and lock status in the various status points used for electronic invoicing. The status points are created by the script 20240328a.sql. The status to be used must be created manually, however, so that it fits the client's workflow. The affected status points are:
*   480 - lead-up electronic invoice (form print)
*   485 - send electronic invoice (customizing/workflow task)
*   490 - receipt electronic invoice (customizing/workflow task)
*   495 - confirmation of electronic invoice (customizing/workflow task)

**Workflow Diagram**

*Image: A flowchart illustrating the electronic invoice process between A+W Business and Comarch.*

The process is as follows:
1.  **Form Printing Dialog (eInvoice)**: This starts the process and sets the status to `480 - lead-up electronic invoice`. It sends the request to the AWB (A+W Business) database.
2.  **Exchange Service (Workflow)**: This service orchestrates the communication.
    *   It periodically checks for invoices with status `485`, `490`, or `495`.
    *   **udf_InvoicesSend**: Sends the invoice data to the **Invoice Service** and sets the status to `485 - Send electronic invoice`.
    *   **udf_InvoicesGet**: Retrieves the status and KSeF ID from the **Invoice Service**.
    *   **udf_InvoicesUpdate**: Updates the invoice in the AWB database with the KSeF ID and sets the status to `490 - Receive electronic invoice`.
    *   **udf_InvoicesCommit**: Confirms the successful update to the **Invoice Service** and sets the status to `495 - Confirmation electronic invoice`.
3.  **Invoice Service**: Acts as a middle layer.
    *   `SendInvoices`: Receives data from the Exchange Service.
    *   `GetInvoices`: Provides status updates.
    *   `CommitInvoices`: Receives confirmation.
    *   It communicates with the external **Comarch** service.
4.  **Comarch**: The external electronic invoicing service provider for the Polish market.

### 2.19.1. Lead-up
The status point 480 is used to create the invoice in A+W Business and is the beginning of the invoice creation. All functions are executed for this as for normal invoice printing, but for the actual printing out or mail dispatch of the document. The function is started in form printing on the tab "6.Electronic invoice".

*Image: Form printing dialog showing the "6.Electronic invoice" tab.*

The tab is only active if the form printing is in "invoice" mode. After that, pressing "OK" or "Enter" will start the lead-up.

### 2.19.2. Send
The customizing function "udf_InvoicesSend" is used to send the invoice to the Comarch WebService. The function determines all orders whose status is between the minimum and lock status of the status point 485 and sends it via the invoice service. Preferably a workflow task is used for this, which is executed cyclically by the exchange service.

### 2.19.3. Receipt
To save the KSeF ID in the documents of an invoice, it must be queried cyclically by the Comarch WebService. This happens with the help of two customizing formulas. The call of "udf_InvoicesGet(sXML)" delivers all invoice documents known to the Comarch WebService. Then the updating of the orders in A+W Business is started via the customizing formula "udf_InvoicesUpdate(sXML)". All documents in A+W Business that are in the appropriate status range for the status point 490 are thus updated. The KSeF ID is displayed in the history and it is stored in the database in the column BW_AUFTR_KOPF_EX.E_INVOICE_ID.

### 2.19.4. Confirmation
The customizing function "udf_InvoicesCommit" is used to communicate the successful updating in the database to the Comarch WebService. It sends all invoices whose documents are in the appropriate status range of status point 495 to the Comarch WebService. The transfer of the invoice data is thus complete.

All customizing formulas are in the formula folder of the A+W Business installation in the "ExchangeService" subfolder.
They are called "workflow_e_invoice_send.txt", "workflow_e_invoice_receive.txt" and "workflow_e_invoice_commit.txt".

# 3. Form printing

## 3.1. Document view variables
The report variables available in the document view are listed below.

### 3.1.1. Header

| Variable | Type | Description |
| :--- | :--- | :--- |
| F_ID | Number | Order number |
| F_AH_IDENT | Number | Customer # |
| F_AH_KOPF | String | Customer's title |
| F_AH_NAME1 | String | Customer name 1 |
| F_AH_NAME2 | String | Customer name 2 |
| F_AH_NAME3 | String | Customer name 3 |
| F_AH_STRASSE | String | Customer's street address |
| F_AH_ORT | String | Customer location |
| F_AH_PLZ | String | Customer's post code |
| F_AH_LAND | String | Customer's country |
| F_AH_TELEFON | String | Customer's phone number |
| F_AH_FAX | String | Customer's fax number |
| F_AL_IDENT | Number | Shipping address customer number |
| F_AL_KOPF | String | Shipping address customer's title |
| F_AL_NAME1 | String | Shipping address - customer name 1 |
| F_AL_NAME2 | String | Lieferadresse Kundenname 2 |
| F_AL_NAME3 | String | Shipping address - customer name 3 |
| F_AL_STRASSE | String | Shipping address - customer's street address |
| F_AL_ORT | String | Shipping address - customer's location |
| F_AL_PLZ | String | Shipping address - customer's post code |
| F_AL_LAND | String | Shipping address - customer's country |
| F_AR_IDENT | Number | Invoice address - customer number |
| F_AR_KOPF | String | Invoice address - customer's title |
| F_AR_NAME1 | String | Invoice address -customer name 1 |
| F_AR_NAME2 | String | Invoice address -customer name 2 |
| F_AR_NAME3 | String | Invoice address -customer name 3 |
| F_AR_STRASSE | String | Invoice address - customer's street address |
| F_AR_ORT | String | Invoice address - customer's location |
| F_AR_PLZ | String | Invoice address - customer's post code |
| F_AR_LAND | String | Invoice address - customer's country |
| F_DATUM_RECHNUNG | DateTime | Invoice date |
| F_DATUM_BEST | DateTime | P.O. date |
| F_DATUM_ERF | DateTime | Date of entry |
| F_DATUM_LIEFER_TAT | DateTime | Actual delivery date |
| F_DATUM_LIEFER_PLAN | DateTime | Scheduled delivery date |
| F_DATUM_LIEFERWUNSCH | String | Requested delivery (e.g. immediately) |
| F_DATUM_PROD1 | DateTime | IG production date |
| F_DATUM_PROD2 | DateTime | LG production date |
| F_DATUM_PROD3 | DateTime | TG production date |
| F_OR_BEARBEITER | String | Person in charge |
| F_OR_FACHBERATER | String | Consultant |
| F_OR_ADIENST | String | Salesman |
| F_OR_TOUR | String | Dispatch route |
| F_OR_LIEFERBED | String | Delivery terms |
| F_OR_VERPACKUNG | String | Packing type |
| F_OR_SPERRKZ | String | Lock code |
| F_FI_BETR_NETTO | Number | Net amount excluding VAT |
| F_FI_BETR_BRUTTO | Number | Gross amount and VAT |
| F_FI_MWST1_BASIS | Number | Basic VAT amount 1 |
| F_FI_BETR_MWST1 | Number | VAT amount 1 |
| F_FI_MWST2_BASIS | Number | Basic VAT amount 2 |
| F_FI_BETR_MWST2 | Number | VAT amount 2 |
| F_FI_BETR_BRUTTO | Number | Gross amount and VAT |
| F_FI_ZAHLBED | String | Payment terms |
| F_FI_ZAHLWEG | String | Payment mode |
| F_FI_WAEHRUNG | String | Currency |
| F_BEST_TEXT1 | String | Purchase text 1 |
| F_BEST_TEXT2 | String | Purchase text 2 |
| F_FI_MWST1 | Number | VAT % 1 |
| F_FI_MWST2 | Number | VAT % 2 |
| F_FI_UST_ID | String | VAT ID |
| F_AH_PLZ_POSTFACH | String | Post code for P.O. box |
| F_AH_POSTFACH | String | P.O. box |
| F_AR_PLZ_POSTFACH | String | Invoice address - post code for P.O. box |
| F_AR_POSTFACH | String | Invoice address - P.O. box |
| F_SU_STUECK | Number | Total quantity |
| F_SU_STUECK_ISO | Number | Total IG units |
| F_SU_LFM_REAL | Number | Total circumference, exact |
| F_SU_LFM_FAKT | Number | Total circumference, rounded |
| F_SU_QM_REAL | Number | Total surface, exact |
| F_SU_QM_FAKT | Number | Total surface, rounded |
| F_SU_GEWICHT | Number | Total weight of goods |
| F_STATUS | Number | State |
| F_NR_RECHNUNG | Number | Invoice number |
| F_KOPFTEXT | String/RTF | Document text (from 2012 RTF field) |
| F_AH_HAUPT_AUFTR | Number | Main order number for partial shipment |
| F_DOK_TYP | String | Document type |
| LADELISTE_NR | Number | Cargo list number |
| LADELISTE_SPEDITEUR | String | Forwarder's cargo list |
| LADELISTE_BEMERKUNG | String | Cargo list - notes |
| LADELISTE_DATUM | DateTime | Cargo list - date |
| LADELISTE_ANZTEILE | Number | Cargo list - number of packaging units |
| LADELISTE_GESGEWICHT | Number | Cargo list - total weight |
| LADELISTE_LIEFTEXT | String | Cargo list - shipping text |
| LADELISTE_VERSENDER | String | Cargo list - sender name 1 |
| LADELISTE_VERSENDER2 | String | Cargo list - sender name 2 |
| F_PRIORITAET | String | Order priority |
| USER_FIELD1 | String | User-defined field 1 |
| USER_FIELD2 | String | User-defined field 2 |
| USER_FIELD3 | String | User-defined field 3 |

*Tab. 6: Document view - main variables*

### 3.1.2. Item variables

| Variable | Type | Description |
| :--- | :--- | :--- |
| F_PROD_BEZ1 | String | Product name 1 |
| F_PROD_BEZ2 | String | Product name 2 |
| F_PROD_BEZ3 | String | Product name 3 |
| F_PP_MENGE | String | Item quantity |
| F_PP_BREITE | String | Width |
| F_PP_HOEHE | String | Height |
| F_POS_KOMMISSION | String | Customer consignment |
| F_POS_KUNDENPOS | String | Customer's item number |
| F_PROD_KURZ_BEZ | String | Product short name |
| F_PROD_FARBE | String | Product color for articles |
| F_PROD_MEEINHEIT | String | Quantity unit |
| F_PROD_PRODART | Number | Product type |
| F_PROD_PRODGRP | Number | Product group |
| F_PR_EINHEIT | String | Price unit |
| F_PR_LISTE | String | Price year |
| F_PR_SCHLUESSEL | String | Price key |
| F_PP_QM | Number | Surface per piece |
| F_PP_QM_FAKT | Number | Surface per piece (rounded) |
| F_PP_LFM | Number | Circumference per piece |
| F_PP_LFM_FAKT | Number | Circumference per piece (rounded) |
| F_PP_GEWICHT | Number | Weight per piece |
| F_PP_DICKE | String | Glazing thickness |
| F_FI_PREIS_ME | Number | Price per price unit |
| F_FI_RABATT1 | Number | Discount |
| F_FI_BRUTTO | Number | Glass unit price prior to discount deduction |
| F_FI_NETTO | Number | Glass unit price after deduction of discount, without BOM items |
| F_FI_NETTO_GES | Number | Glass unit price multiplied by quantity |
| F_FI_POS_STK | Number | Total item unit price including surcharges and processing referring to one piece |
| F_FI_POS_GES | Number | Total item price including surcharges and processing, for total item quantity |
| F_EK_POS_GES | Number | Total item cost |
| F_POS_TEXT1 | String | Item text 1 |
| F_POS_TEXT2 | String | Item text 2 |
| F_POS_TEXT3 | String | Item text 3 |
| F_POS_TEXT4 | String | Item text 4 |
| F_POS_TEXT5 | String | Item text 5 |
| F_CE_CPIP | String | CPIP Code |
| F_TEXT1 | String/RTF | Item text before item (from 2012 RTF text) |
| F_TEXT2 | String/RTF | Item text after item (from 2012 RTF text) |
| F_PRODTEXT | String/RTF | Product text (from 2012 RTF text) |
| F_REF | String | Document reference |
| F_AB | String | Supplier OC no. |
| F_REFERENZ | String | P.O. reference |
| F_GEL_MENGE | Number | Quantity delivered |
| F_PROD_STRUKTSEITE | String | Pattern side |
| F_REKLA_ORT | String | Cause of complaint |
| F_REKLA_GRUND | String | Reason for complaint |
| F_PROD_ID | Number | Product number |
| F_FI_ZUBASIS | Number | Basic surcharge (amount) |
| F_ISO_AUFBAU_KEYNR | Number | Unique IG structure number |
| F_LIORDER_NR | Number | LIORDER production number |
| F_LIORDER_VSG | String | LIORDER production number for LG |
| F_POS_REFERENZ | String | Product reference number (e.g. DORMA product number) |
| F_VPOS_NR | String | Virtual item number |
| F_PROD_ID_MCODE | String | Product matchcode (master data) |
| **From ALFAK 2008 on:** | | |
| F_REF_BEST_ID | String | Reference for the previous P.O. number (only for orders and quotations). For credit notes, this field shows the invoice number of the order on which the credit note is based |
| F_REF_BEST_POS | String | Reference for the previous P.O. item number (only for orders and quotations) |
| F_REF_AUSLIEF_AUFTR_ID | String | Reference for shipping order number. For credit notes, this field shows the number of the order on which the credit note is based |
| F_REF_AUSLIEF_AUFTR_POS | String | Reference for the shipping item number. For credit notes, this field shows the order item on which the credit note is based |
| F_REF_ENDKUNDE_BEST_ID | String | Reference for the customer's P.O. number (not for credit notes) |
| F_REF_ENDKUNDE_BEST_POS | String | Reference for the customer's item number (not for credit notes) |
| F_PRCL_XXX | String | Value of product classifiers with names XXX |

*Tab. 7: Document view - item variables*

### 3.1.3. BOM variables

| Variable | Type | Description |
| :--- | :--- | :--- |
| F_STL_BEZ | String | Product Description |
| F_STL_FARBE | String | Product color |
| F_STL_KURZ_BEZ | String | Product short name |
| F_STL_PRODART | Number | Product type |
| F_STL_PRODGRP | Number | Product group |
| F_STL_MENGE | String | Quantity |
| F_STL_BREITE | String | Width |
| F_STL_HOEHE | String | Height |
| F_PP_DICKE | String | Thickness |
| F_STL_LFM | Number | Scope |
| F_STL_LFM_FAKT | Number | Circumference, rounded |
| F_STL_QM | Number | Area |
| F_STL_QM_FAKT | Number | Surface (rnd.) |
| F_STL_PR_EINHEIT | String | Price unit |
| F_STL_PR_RABATT | Number | Discount |
| F_STL_PREIS_OFFEN | Number | explicit price |
| F_STL_BETR_NETTO | Number | Net amount |
| F_STL_BETR_BRUTTO | Number | Gross amount |
| F_STL_NETTO_GES | Number | Total Price |
| F_STL_PREIS_ME | Number | Price per price unit |
| F_PARAM_MODELL | String | Shape parameter |
| F_PARAM_BEARB | String | Processing parameters |
| F_SPR_DIRECTION1 | Number | Georgian bar direction |
| F_SPR_MENGE1 | Number | Number of bars |
| F_SPR_DIRECTION2 | Number | Georgian bar direction |
| F_SPR_MENGE2 | Number | Number of bars |
| F_PARAM_SPROSSE | String | Muntin parameters |
| F_STL_STRUKTSEITE | String | Pattern side |
| F_BOM_PRODUKT | Number | Product number |
| F_STL_LIORDER_NR | Number | LIORDER production number |
| F_STL_LIORDER_VSG | String | LIORDER production number for LG |
| F_STL_REFERENZ | String | Product reference number (e.g. DORMA product number) |
| F_BOM_PRODUKT_MCODE | String | Product matchcode (master data) |
| F_STX_PRCL_XXX | String | Value of product classifiers with names XXX |

*Tab. 8: Document view BOM variables*

## 3.2. Form printing variables

The report variables available for printing documents are listed below.

### 3.2.1. Header

| Variable | Type | Description |
| :--- | :--- | :--- |
| AB_DATUM | Date/Time | Order confirmation date |
| AB_LIEFERANT_DAT | String | Supplier's order confirmation date |
| AH_ANREDE | String | Customer address (Mr, Mrs, etc.) |
| AH_ANREDE | String | Customer company |
| AH_FAX | String | Customer's fax number |
| AH_HAUPT_AUFTR | Number | Main order number |
| AH_IDENT | Number | Customer # |
| AH_KOPF | String | Customer's company name |
| AH_LAND_NAME | String | Country |
| AH_LAND | String | Customer's country |
| AH_LIEFER_KZ | Number | Delivery code for shipping address |
| AH_LIEFERANT | Number | Supplier number in order header |
| AH_LIEFERANT_NAME1 | String | Supplier name 1 in order header |
| AH_LIEFERANT_NAME2 | String | Supplier name 2 in order header |
| AH_LIEFERANT_ORT | String | Supplier's location in order header |
| AH_LIEFERANT_PLZ | String | Supplier's post code in order header |
| AH_LIEFERANT_STRASSE | String | Supplier's street in order header |
| AH_MAIL | String | Email address acc. to document header |
| AH_MCODE | String | Customer's short name |
| AH_NAME1...AH_NAME3 | String | Customer name |
| AH_PARTNER | String | Customer's contact |
| AH_PLZ | String | Customer's post code |
| AH_PLZ_POSTFACH | String | Post code (post box) |
| AH_POSTFACH | String | Customer's post box |
| AH_PROVINZ | String | Customer county/state |
| AH_STRASSE | String | Customer's street address |
| AH_TELEFON | String | Customer's phone number |
| AL_ANREDE | String | Address (shipping address) |
| AL_FAX | String | Fax number (shipping address) |
| AL_IDENT | Number | Customer number (shipping address) |
| AL_KOPF | String | Address (shipping address) |
| AL_LAND_NAME | String | Country |
| AL_LAND | String | Country (shipping address) |
| AL_NAME1 | String | Shipping address - name 1 |
| AL_NAME2 | String | Shipping address - name 2 |
| AL_NAME3 | String | Shipping address - name 3 |
| AL_ORT | String | City (shipping address) |
| AL_PARTNER | String | Customer's contact for delivery |
| AL_PLZ | String | Post code (shipping address) |
| AL_PROVINZ | String | County/state (shipping address) |
| AL_STRASSE | String | Shipping address - street |
| AL_TELEFON | String | Phone number for alternative Shipping address |
| AR_ANREDE | String | Address (invoice address) |
| AR_FAX | String | Fax number (invoice address) |
| AR_IDENT | Number | Customer number (invoice address) |
| AR_KOPF | String | Address (invoice address) |
| AR_LAND_NAME | String | Country |
| AR_LAND | String | Country (invoice address) |
| AR_NAME1 | String | Invoice name 1 |
| AR_NAME2 | String | Invoice name 2 |
| AR_NAME3 | String | Invoice name 3 |
| AR_ORT | String | City (invoice) |
| AR_PARTNER | String | Customer's contact (invoice) |
| AR_PLZ | String | Post code (invoice address) |
| AR_PLZ_POSTFACH | String | Post code and post box (invoice address) |
| AR_POSTFACH | String | Post code (invoice address) |
| AR_PROVINZ | String | County/state (invoice address) |
| AR_STRASSE | String | Street of the invoice address |
| AR_TELEFON | String | Phone number (invoice address) |
| AUFTR_REF | Number | Original order number (for partial shipments) |
| BANK_NAME | String | Customer's bank name (form option 1) |
| BEST_TEXT1 | String | Purchase text 1 |
| BEST_TEXT2 | String | Purchase text 2 |
| BRUTTO_TAGE | Number | Gross days (payment terms) |
| CONTR_BRUTTO_AMNT | Number | Gross amount of the present claim |
| CONTR_CURRENT_AMNT | Number | Amount to be paid at present |
| CONTR_FI_NETTO_GES | Number | Net amount of the corresponding overall order |
| CONTR_MWST_AMNT | Number | VAT for the present claim |
| CONTR_PAID_AMNT | Number | Total claims paid |
| CONTRACT_ORDER_ID | Number | Number of the corresponding overall order |
| DATUM_AB | Date/Time | Order confirmation (printout date) |
| DATUM_ANLIEFERUNG | Date/Time | Delivery date |
| DATUM_BEST | Date/Time | Purchase date |
| DATUM_ERF | Date/Time | Input date of the order |
| DATUM_FAELLIGK | Date/Time | Due date |
| DATUM_LIEFER_TAT | Date/Time | Actual shipping date |
| DATUM_LIEFERSCHEIN | Date/Time | Delivery note date |
| DATUM_LIEFERWUNSCH | String | Delivery request |
| DATUM_PROD1...3 | Date/Time | Production date IG, laminated glass, toughened glass |
| DATUM_RECHNUNG | Date/Time | Invoice date |
| DATUM_SKONTO | Date/Time | Cash discount date |
| DATUM_VALUTA_SPLIT1 | Date/Time | 1st due date (for graduated due dates) |
| DATUM_VALUTA_SPLIT2 | Date/Time | 2nd due date (for graduated due dates) |
| DATUM_VALUTA_SPLIT3 | Date/Time | 3rd due date (for graduated due dates) |
| DATUM_VALUTA_SPLIT4 | Date/Time | 4th due date (for graduated due dates) |
| DATUM_VALUTA_SPLIT5 | Date/Time | 5th due date (for graduated due dates) |
| DEBKRED_KTO | String | Debtor/creditor account (form option 1) |
| DOC_SU_GEWICHT | Number | Total weight (for the document) |
| DOC_SU_LFM_FAKT | Number | Total linear meters - invoiced (for the document) |
| DOC_SU_LFM_REAL | Number | Total linear meters - actual (for the document) |
| DOC_SU_QM_FAKT | Number | Total square meters - invoiced (for the document) |
| DOC_SU_QM_REAL | Number | Total square meters - actual (for the document) |
| DOC_SU_SPRLFM_FAKT | Number | Total linear meters of Georgian bars - invoiced per document |
| DOC_SU_SPRLFM_REAL | Number | Total linear meters of Georgian bars - actual per document |
| DOC_SU_STUECK | Number | Total quantity (for the document) |
| DOC_SU_QM_FAKT_TPS | Number | Total square meters of TPS - invoiced (for the document) |
| DOK_TYP | String | Document type |
| Print_item | Number | Print item acc. to management of forms |
| FAXHEADER | Number | Fax header for fax dispatch |
| FER_LINIE | Number | Production line |
| FI_BETR_BRUTTO | Number | Gross amount and VAT |
| FI_BETR_BRUTTO_FW | Number | Gross item amount in foreign currency |
| FI_BETR_FESTPR_FW | Number | Fixed document price in foreign currency |
| FI_BETR_FESTPREIS | Number | Fixed document price |
| FI_BETR_MWST1 | Number | Tax amount 1 |
| FI_BETR_MWST2 | Number | Tax amount 2 |
| FI_BETR_MWST3 | Number | Tax amount 3 |
| FI_BETR_MWST4 | Number | Tax amount 4 |
| FI_BETR_MWST5 | Number | Tax amount 5 |
| FI_BETR_MWST1_FW | Number | Tax amount 1 in foreign currency |
| FI_BETR_MWST2_FW | Number | Tax amount 2 in foreign currency |
| FI_BETR_MWST3_FW | Number | Tax amount 3 in foreign currency |
| FI_BETR_MWST4_FW | Number | Tax amount 4 in foreign currency |
| FI_BETR_MWST5_FW | Number | Tax amount 5 in foreign currency |
| FI_BETR_NETTO | Number | Net document amount |
| FI_BETR_NETTO_FW | Number | Net document amount in foreign currency |
| FI_BETR_SKONTO | Number | Cash discount |
| FI_BRUTTO | Number | Gross document amount |
| FI_BRUTTO_FW | Number | Gross document amount in foreign currency |
| FI_KOPF_RABATT | Number | Main discount (document) |
| FI_MWST1 | Number | VAT% 1 |
| FI_MWST2 | Number | VAT % 2 |
| FI_MWST3 | Number | VAT % 3 |
| FI_MWST4 | Number | VAT % 4 |
| FI_MWST5 | Number | VAT % 5 |
| FI_MWST1_BASIS | Number | Basic VAT amount 1 |
| FI_MWST2_BASIS | Number | Basic VAT amount 2 |
| FI_MWST3_BASIS | Number | Basic VAT amount 3 |
| FI_MWST4_BASIS | Number | Basic VAT amount 4 |
| FI_MWST5_BASIS | Number | Basic VAT amount 5 |
| FI_MWST1_BASIS_FW | Number | Basic VAT amount 1 in foreign currency |
| FI_MWST2_BASIS_FW | Number | Basic VAT amount 2 in foreign currency |
| FI_MWST3_BASIS_FW | Number | Basic VAT amount 3 in foreign currency |
| FI_MWST4_BASIS_FW | Number | Basic VAT amount 4 in foreign currency |
| FI_MWST5_BASIS_FW | Number | Basic VAT amount 5 in foreign currency |
| FI_MWST1_ID | Number | VAT ID 1 |
| FI_MWST2_ID | Number | VAT ID 2 |
| FI_MWST3_ID | Number | VAT ID 3 |
| FI_MWST4_ID | Number | VAT ID 4 |
| FI_MWST5_ID | Number | VAT ID 5 |
| FI_SKONTO_BASIS | Number | Basic cash discount amount |
| FI_SKONTO_BASIS_FW | Number | Basic cash discount amount in foreign currency |
| FI_UST_ID | String | VAT ID |
| FI_VALUTAKURS | Number | Exchange rate |
| FI_WAEHRUNG | String | Currency used for calculating the item |
| FI_ZAHL_TAG1...FI_ZAHL_TAG3 | Number | Payment days 1-3 |
| FI_ZAHLBED | String | Payment terms |
| FI_ZAHLWEG | String | Method of payment |
| SITENO | Number | Subsidiary number |
| FIRMA_FAX | String | Company's fax number |
| FIRMA_NAME1 | String | Company name 1 |
| FIRMA_NAME2 | String | Company name 2 |
| FIRMA_NAME3 | String | Company name 3 |
| FIRMA_ORT | String | Company location |
| FIRMA_PLZ | String | Post code (headquarters) |
| FIRMA_STRASSE | String | Street address (headquarters) |
| FIRMA_TLF1 | String | Company's phone number |
| FIRMA_UST_ID | String | Company's VAT ID |
| FIRMA_STEUER_NR | String | Company's tax ID |
| FORM_PATH | String | Path for the forms in the INI file (w/o backslash at the end) |
| FREMD_KEY | String | Foreign key |
| KO_FAXVERSAND | Number | Flag for faxing the document |
| KO_KSCHUTZ | Number | Edgework code |
| KO_MASSEINH | Number | Measurement imperial/metric |
| KO_NETTOPREISE | Number | Flag for output of net prices |
| KO_OBJEKT_KUNDE | String | Customer's project name |
| KO_OBJEKT_LIEF | String | Supplier's project name |
| KO_TEILFAK | Number | Partial invoicing flag |
| Copies | Number | Number of document copies |
| KPF_TEXT_KZO...KPF_TEXT_KZx | String | Text code for customized headers |
| KPF_TEXTO...KPF_TEXTx | String | Customized headers |
| KPF_TEXT_RTFO...KPF_TEXT_RTFx | RTF | Customized RTF headers (from 2012 on) |
| Loading_list | Number | Print loading list |
| LAUF_PROD1 | Number | Production job number IG |
| MAIL_BETREFF | String | Reference line for email dispatch |
| MAIL_FILE | String | Name of PDF file for emailing without file suffix |
| MAILHEADER | Number | Defines whether the email header shall be printed (for emailing via PDF-Mailer) |
| MEMO | String | Memo field of the document |
| MOD_DRUCK | Number | Shape printing flag |
| MOD_LOGO | Object | Bitmap field for the shape on the form |
| MODUS | Number | 1=Quotation, 2=Order, 3=Credit note, 4=Inquiry, 5=Purchase order |
| NR_AUFTRAG | Number | Order number |
| NR_LIEFERSCHEIN | Number | Delivery note # |
| LS_NUMMERN | String | Delivery note numbers including prefix for printing invoices, and numbering per page |
| PRAEFIX_LIEFERSCHIEN | String | Delivery note prefix for numbering per page |
| PRAEFIX_RECHNUNG | String | Invoice prefix for numbering per page |
| NR_RECHNUNG | Number | Invoice number |
| OCR | String | OCR code for customers for invoice printing |
| OR_ADIENST | String | Salesman 1 |
| OR_AVBEREICH | String | Order area for the order |
| OR_AVBEREICH_FK | String | External code for OM area |
| OR_AWTOUR | String | Alternative route |
| OR_BEARBEITER | String | Author of this order |
| OR_FACHBERATER | String | Consultant for this order |
| OR_FACHBERATER_DURCHWAHL | String | Consultant's extension |
| OR_FACHBERATER_MAIL | String | Consultant's email address |
| OR_FACHBERATER_FAX | String | Consultant's fax number |
| OR_FAHRER | String | Driver delivering this order |
| OR_GESCHART | String | Business type of this order |
| OR_GRUPPE | String | Customer group |
| OR_LIEFERBED | String | Delivery terms for this order |
| OR_LKW | String | Truck name |
| OR_MANDANT | Number | Site |
| OR_SPERRKZ | String | Lock code for the document |
| OR_SPRACH_BASIS | Number | Native language number (0) |
| OR_SPRACH_ID | Number | Language number for the document |
| OR_TOUR | String | Route name |
| OR_VERPACKUNG | String | Packing type |
| OR_ZOLLTOUR | String | Customs route name |
| PMNT_AMOUNT | String | Deposit amount (SGG) |
| PMNT_CURRENCY | String | Deposit currency (SGG) |
| PMNT_DATE | String | Deposit date (SGG) |
| PMNT_MODE | String | Deposit payment type (SGG) |
| PMNT_REMARK | String | Deposit remarkes (SGG) |
| PMNT_REST_AMOUNT | String | Balance minus deposits (SGG) |
| PMNT_STATUS | String | Deposit status (SGG) |
| PMNT_SUM_AMOUNT | String | Total deposit amount (SGG) |
| PMNT_TIME | String | Deposit time (SGG) |
| PMNT_USER | String | Deposit made by (SGG) |
| PRIORITY | String | Production transfer priority |
| SEITE | Number | Actual number of pages of the document |
| SEITEN | Number | Actual number of pages of the document after change of form layout |
| SKONTOSATZ1 | Number | Cash discount rate 1 |
| SKONTOSATZ2 | Number | Cash discount rate 2 |
| SKONTOSATZ3 | Number | Cash discount rate 3 |
| SKONTOTAGE1 | Number | Cash discount days 1 |
| SKONTOTAGE2 | Number | Cash discount days 2 |
| SKONTOTAGE3 | Number | Cash discount days 3 |
| SQL_USER | String | Database login name |
| STATUS | Number | Document status |
| STEUERNUMMER | String | Customer's tax number |
| SU_BETR_BRUTTO_SPLIT1 | Number | 1st instalment on due date 1 (gross) |
| SU_BETR_BRUTTO_SPLIT2 | Number | 2nd instalment on due date 2 (gross) |
| SU_BETR_BRUTTO_SPLIT3 | Number | 3rd instalment on due date 3 (gross) |
| SU_BETR_BRUTTO_SPLIT4 | Number | 4th instalment on due date 4 (gross) |
| SU_BETR_BRUTTO_SPLIT5 | Number | 5th instalment on due date 5 (gross) |
| SU_BETR_EK1 | Number | Material costs |
| SU_BETR_EK2 | Number | Time costs |
| SU_SPRLFM_FAKT | Number | Total linear meters of Georgian bars (invoiced) |
| SU_SPRLFM_REAL | Number | Total linear meters of Georgian bars (actual) |
| TEXT_FUSS | String | Definable text (form footer) |
| TEXT_FUSS_RTF | RTF | Definable text in form footer (from 2012 RTF field) |
| TEXT_KOPF | String | Definable text (form header) |
| TEXT_KOPF_RTF | RTF | Definable text in form header (from 2012 RTF field) |
| TEXT_NRO...TEXT_NRx | String | Job number for customized headers |
| WH_DRUCK | Number | Flag for repeated printout |
| ZAHL_BLZ | String | Bank code (acc. to form option 1) |
| ZAHL_KTN | String | Account number (acc. to form option 1) |
| KOPF_RESTERROR | String | Bit vector for restriction violations. Collects all restriction violations for the item: 1. = max. purchase size exceeded, 2. = max. stocksize exceeded, 3. = min. sizes not met, 4. = max. surface exceeded, 5. = max. aspect ratio exceeded |
| SU_BETR_BRUTTO_STR | String | Gross amount in words |
| SU_BETR_BRUTTO_FW_STR | String | Foreign currency amount in words |
| ZUSCHLAG_BIT_STRING | String | Bit vector of surcharges (explanation on tab Bit vectors) |
| OR_ADIENST2 | String | Salesman 2 (as from 4.0 case 101086) |
| TLF2 | String | Customer's second phone number (via form option 'Read customer data (bank account)') |
| SU_UEBERTRAG | Number | Item amounts carried over to next page (only without Keep Group on Page of GRUPPENBEZ) |
| KZ_POSTFACH | Number | Defines whether the post box address shall be used (via form option 'Read customer data (bank account)') |
| PRT_CLASSxxx | String | Classifier value (xxx = classifier no. without zeros) Is enabled by form option; classifier notes have to start with <Print> |
| PREV_INVOICE_NET | Number | Net amount of last month's invoice (form option 'previous invoice data') |
| PREV_INVOICE_TAX1 | Number | Tax amount 1 of last month's invoice (form option 'previous invoice data') |
| PREV_INVOICE_TAX2 | Number | Tax amount 2 of last month's invoice (form option 'previous invoice data') |
| PREV_PAYMENTTYPE | String | Payment method of last month's invoice (form option 'previous invoice data') |
| CUST_RECEIVABLES | Number | Customer's receivables (form option 'previous invoice data') |
| TEXT1, TEXT2, ...TEXT10 | String | Variable text from management of forms |
| TEXT1_RTF,...TEXT10_RTF | RTF | Variable text from management of forms |
| KO_OBJEKT_KUNDE_NR | Number | Customer's project number |
| KO_OBJEKT_LIEF_NR | Number | Supplier's project number |
| DOC_NR_C39 | String | Barcode with order number Structure: *Oxxxxxxxx* whereby x= 8-digit order number with heading zeros |
| TRANSPORT_ID | Number | Brazilian taxation: forwarder's ID |
| TRANSPORT_RESPONSE | Number | Brazilian taxation: responsibility |
| TRANSPORT_NAME1 | String | Brazilian taxation: forwarder's name |
| TRANSPORT_STRASSE | String | Brazilian taxation: forwarder's street address |
| TRANSPORT_ORT | String | Brazilian taxation: forwarder's location |
| TRANSPORT_PROVINZ | String | Brazilian taxation: forwarder's state |
| TRANSPORT_UST_ID | String | Brazilian taxation: tax number of the state in which the forwarder is located |
| TRANSPORT_STEUERNUMMER | String | Brazilian taxation: government's tax number |
| VALOR_UNITARIO_MODE | Number | Valor Unitario mode (0=in price unit, 1= in units) |
| COPYCOUNTER | Number | Copy counter (0=Original, 1= first copy,...) |
| FIRMA_CERT_CODE | String | Company's certification code |
| HASH_CODE | String | Digital signature/hash code of the document (digits 1, 11, 21 and 31, separated by -) |
| ANLIEFERZEIT | String | Delivery time window (from – to) |
| USER_FIELD1 | String | User-defined field 1 |
| USER_FIELD2 | String | User-defined field 2 |
| USER_FIELD3 | String | User-defined field 3 |

*Tab. 9: Printing of forms - header variables*

### 3.2.2. Item variables

| Variable | Type | Description |
| :--- | :--- | :--- |
| AB_DATUMO | Date/Time | Supplier's order confirmation date for a customer's item |
| AB_LIEFERANT_DAT | String | Supplier's order confirmation date |
| AB_LIEFERANTO | String | Supplier's order confirmation for a customer's item |
| AGGREGATE | String | Time management: machines sorted by process sequence |
| AH_HAUPT_AUFTR | Number | Main order number for partial shipments |
| ALTERNATIV | Number | Alternative item number |
| AUFTR_REF | Number | Order reference for partial shipment |
| BA_PRODUKT_INFO | String | Article info (form option:read product data) |
| BEARBTEXT | String | Text showing all processing steps for an article |
| CE_CPIP | String | CPIP code (SGG only) |
| CE_FLAG | Number | CPIP check active (0 = disabled, 1= active) (SGG only) |
| CE_KZ | String | CE code |
| CE_LEVEL | Number | CPIP level (0=self-explanatory, 1=certified, 2=certified with size restriction) (SGG only) |
| CONTR_AMNT_ACT | Number | Amount of the actual claim |
| CONTR_AMNT_PREV | Number | Amount of previous claims |
| CONTR_CLAIM_TYPE | String | Claim type (percentage, quantity, or amount) |
| CONTR_CLAIMED_ACT | Number | Quantity for the actual claim |
| CONTR_CLAIMED_PREV | Number | Quantity of previous claims |
| DOC_POS_C39 | String | Barcode with order and item number. Structure: *Cxxxxxxxxppp* whereby x=8-digit order number with heading zeros and p=3-digit item number with heading zeros |
| EAN | String | EAN number as per product master data |
| EINHZAEHLER | Number | Numbering of unit labels |
| EK_POS_GES | Number | Total purchase price of the item |
| EK_POS_STK | Number | Cost per piece |
| EK_PREIS_ME | Number | Cost per price unit |
| EK_PREIS_ME_GES | Number | Cost per price unit including implicit Bills of material |
| EK_ZEIT_STK | Number | Labour cost per piece acc. to capacity planning |
| FER_BESCHAFFARTNR | Number | Supply type number |
| FER_BESCHICH_SEITE | Number | Coated side of main product |
| FER_GEST_TYP | String | Rack type and rack number from production feedback |
| FER_KSCHUTZ | Number | Edgework code |
| FER_KZ_BESCHICHTET | Number | Coating code acc. to product master data |
| FER_LAUF1 | Number | Production job number |
| FER_LINIE | Number | Production line |
| FER_RAHMENNR | Number | Spacer text number |
| FER_RAHMENTEXT | String | Spacer text number |
| FER_STRUKTURSEITE | Number | Pattern side |
| FER_STRUKTURVERL | Number | Sense of pattern |
| FER_UVRAND | Number | UV edgework code |
| FI_BRUTTO | Number | Gross item price |
| FI_BRUTTO_FW | Number | Gross item price in foreign currency |
| FI_KZ_STEUER | Number | Tax code |
| FI_NETTO | Number | Net amount (article) |
| FI_NETTO_FW | Number | Net amount (article) in foreign currency |
| FI_NETTO_GES | Number | Total amount net |
| FI_NETTO_GES_FW | Number | Total amount net in foreign currency |
| FI_POS_GES | Number | Total item price |
| FI_POS_GES_BEM | String | Remarks/reason for price change |
| FI_POS_GES_BIT | Number | Price change report not printed (1= not printed) |
| FI_POS_GES_FW | Number | Total item price in foreign currency |
| FI_POS_GES_MAN | Number | Total item price without manual presetting |
| FI_POS_GES_RAB | Number | Total item price without discount and individual price |
| FI_POS_STK | Number | Total item price |
| FI_POS_STK_FW | Number | Total item price in foreign currency |
| FI_PREIS_ME | Number | Article's price quantity unit |
| FI_PREIS_ME_FW | Number | Article price per price unit in foreign currency |
| FI_PREIS_ME_FW_SHEET1..3 | Number | Price per quantity unit for 1st and 3rd sheet of IG unit (in foreign currency) |
| FI_PREIS_ME_GES | Number | Price per price unit including implicit Bills of material |
| FI_PREIS_ME_GES_FW | Number | Price per price unit including implicit BOM in foreign currency |
| FI_PREIS_ME_GES_FWNET | Number | Net price per quantity unit in foreign currency including replacement sheets (IG) |
| FI_PREIS_ME_GESNET | Number | Net price per quantity unit including replacement sheets (IG) |
| FI_PREIS_ME_SHEET1..3 | Number | Price per quantity unit for 1st and 3rd sheet of IG unit |
| FI_RABATT_SHEET1..3 | Number | Discount for 1st and 3rd sheet of IG unit |
| FI_RABATT1 | Number | Article discount |
| FI_ZUBASIS | Number | Basic surcharge (amount) |
| FORMGRUPPE | Number | Form group for split printout |
| GAS[1-n] | String | Name of 1.-n. gas |
| GEL_MENGEX | Number | Delivered quantity (goods received) for P.O. (x = 0-x P.O. references) |
| GLAS_BS[1-n] | Number | Coated side of IG sheets |
| GLAS_SS[1-n] | Number | Patterned side of IG sheets |
| GLAS_SV[1-n] | Number | Sense of pattern of IG sheets |
| GLAS[1-n]_BESCH | Number | Coating code of IG sheets acc. to product master data |
| GLASBEZ[1-n] | String | Glass name 1-n |
| GROUP | Number | Internal group number |
| GRUPPE_BIS | Number | End of group - item number |
| GRUPPE_EQUAL | Number | Flag for printing identical, consecutive items |
| GRUPPE_LFM_FAKT | Number | Total circumference for a group |
| GRUPPE_NETTO | Number | Net group price |
| GRUPPE_NETTO_FW | Number | Net group prices in foreign currency |
| GRUPPE_PRINT | Number | Print subtotal |
| GRUPPE_QM_FAKT | Number | Total surface of the group |
| GRUPPE_STK | Number | Total quantity for a group |
| GRUPPE_VON | Number | Start of group - item number |
| ISO_AUFBAU_KEYNR | Number | Unique IG structure number |
| KISTE_INHALT | Number | Box contents |
| KOSTENART | String | Cost type |
| KOSTENSTELLE | String | Cost center |
| KUNDE_NAME | String | Customer name of P.O. forms from P.O. transfer |
| KZ_AUTOZUSCHN | Number | Code 'automatic cutting - main product' |
| KZ_AUTOZUSCHN[1-n] | Number | Code 'automatic cutting - 1st-nth glass' |
| KZ_BESTELLUNG | Number | P.O. code: 0=in-house production/glass supplied, 1=purchased article, 2=article completely purchased |
| KZ_LAGER | Number | Stockkeeping code: 0=own production, 1=stock product |
| KZ_SERIE | Number | Serial code |
| LAG_LAGER_BEZ | String | Warehouse name |
| LAG_LAGER_ID | Number | Stock product name |
| LAGER_IDENT | String | Stock ID number |
| LIEFERANT_NAME | String | Supplier name for this item (only if form option 'print references' is active) |
| LIEFERANT_NR | Number | Supplier number for this item (only if form option 'print references' is active) |
| MAKRO_NAME | String | Name of the selected macro (from 2006) |
| MOD_SN_TEMPLATE | String | Template name of SN file (from 2009) |
| MOD_SN_NAME | String | Shaping+Nesting file name |
| OR_FACHBERATER_DURCHWAHL | String | Consultant's extension |
| OR_SPRACH_BASIS | Number | Native language |
| OR_SPRACH_ID | Number | Language in which the document shall be printed |
| POS_BIT | Number | Modification bit for this item |
| POS_BIT_STRING | String | 1. string with manual amendment flags |
| POS_BIT2_STRING | String | 2. string with manual amendment flags |
| POS_BIT3_STRING | String | 3. string with manual amendment flags |
| POS_GRUPPE | Number | Item group of counter pane |
| POS_KOMMISSION | String | Item reference text |
| POS_KUNDENPOS | String | Customer item |
| POS_NR | Number | Item number |
| POS_PREIS_BIT_STRING | String | Bit vector for pricing information |
| POS_REF | Number | Item number of original item (for partial shipment) |
| ITM_REFERENCE | String | Product reference number (DORMA product number) |
| POS_RESTERROR | String | Bit vector for restriction violations. Digit 1 = max. purchase size exceeded, 2 = max. stocksize exceeded, 3 = min. size not met, 4 = max. surface exceeded, 5 = max. aspect ratio exceeded |
| POS_STATUS | Number | Item status |
| POS_STTXT_NR | Number | Text number |
| POS_TEXT | String | Item text |
| POS_TEXT1 | String | Item text 1 |
| POS_TEXT2 | String | Item text 2 |
| POS_TEXT3 | String | Item text 3 |
| POS_TEXT4 | String | Item text 4 |
| POS_TEXT5 | String | Item text 5 |
| POS_VERPACKUNG | String | Packing type |
| PP_BREITE | Number | Article width in mm |
| PP_BREITE_INCH | String | Article width in inch |
| PP_DICKE | Number | Article thickness in mm |
| PP_DICKE_INCH | String | Article thickness in inch |
| PP_FALZ | Number | Tight size |
| PP_GEWICHT | Number | Article weight in kg |
| PP_GEWICHT_TARA | Number | Article tara |
| PP_HOEHE | Number | Article height in mm |
| PP_HOEHE_INCH | String | Article height in inch |
| PP_LFM | Number | Article - lin.m. |
| PP_LFM_FAKT | Number | Article - lin.m. invoiced |
| PP_MENGE | Number | Article quantity |
| PP_ORIG_MENGE | Number | Original item quantity |
| PP_ORIG_MENGE_TEIL | Number | Original item quantity (partial shipment) |
| PP_PLANSTK | Number | Default quantity |
| PP_QM | Number | Article surface in sqm |
| PP_QM_FAKT | Number | Article surface, invoiced |
| PP_TEILGEL_MENGE | Number | Partially shipped item quantity |
| PP_TEILGEL_MENGE_TEIL | Number | Partially shipped item quantity (partial shipment) |
| PR_EINHEIT | String | Price unit |
| PR_EINHEIT_ID | Number | Price unit ID |
| PR_GRUPPE | String | Diff. customer price group |
| PR_LISTE | String | Item price list |
| PR_QM | Number | Price per sqm |
| PR_SCHLUESSEL | String | Price code for this item |
| PROD_DES1 | String | Article descript. 1 |
| PROD_DES2 | String | Article descript. 2 |
| PROD_DES3 | String | Article descript. 3 |
| PROD_FARBE | String | Article color |
| PROD_ID | Number | Product Code |
| PROD_KMB | String | Product group combination - discount |
| PROD_KMB_STAT | String | Product group combination - statistics |
| PROD_KOMONR | Number | KOMO number quality code |
| PROD_KURZ_BEZ | String | Product short name |
| PROD_LAGERORT | Number | Warehouse number |
| PROD_MCODE | String | Product matchcode |
| PROD_MEEINHEIT | String | Article - quantity unit |
| PROD_MEEINHEIT_ID | Number | Product quantity unit ID |
| PROD_PRODART | Number | Product type this article belongs to |
| PROD_PRODGRP | Number | Product group this article belongs to |
| PROD_WGR | String | Product group discounts |
| PROD_WGR_STAT | String | Product group statistics |
| REF_AUSLIEF_AUFTR_ID | String | Reference for shipping order number. For credit notes, this field shows the number of the order on which the credit note is based |
| REF_AUSLIEF_AUFTR_POS | String | Reference for the shipping item number. For credit notes, this field shows the order item on which the credit note is based |
| REF_BEST_ID | String | Reference for the previous P.O. number (only for orders and quotations). For credit notes, this field shows the invoice number of the order on which the credit note is based |
| REF_BEST_POS | String | Reference for the previous P.O. item number (only for orders and quotations) |
| REF_ENDKUNDE_BEST_ID | String | Reference for the customer's P.O. number (not for credit notes) |
| REF_ENDKUNDE_BEST_POS | String | Reference for the customer's item number (not for credit notes) |
| REF_ID0 | Number | From P.O. number' allocated to the order item after transfer to purchasing |
| REF_ID1 | Number | To P.O. number' allocated to the order item after transfer to purchasing |
| REF_POS0 | Number | From P.O. item' allocated to the order item after transfer to purchasing |
| REF_POS1 | Number | To P.O. item' allocated to the order item after transfer to purchasing |
| REKLA_GRUND | String | Reason for complaint |
| REKLA_ORT | String | Complaint place |
| SZR[1-n] | String | Name of spacer 1-n |
| SZR[1-n]FARBE | String | Color of spacer 1-n |
| TEXT_BEZ1 | String | Text before item |
| TEXT_BEZ1_RTF | RTF | RTF texts before item (from 2012) |
| TEXT_BEZ2 | String | Text after item |
| TEXT_BEZ2_RTF | RTF | RTF texts after item (from 2012) |
| TEXT_PROD | String | Product-related text |
| TEXT_PROD_RTF | RTF | Product-related RTF texts (from 2012) |
| VERSK_DRUCK | Number | 1=print dimensioned sketch |
| VPOS_NR | String | Virtual item number (sub-items 1 / 1.1/1.2 / 1.3 etc.) |
| ZWPRODENDE | Date | End of production (time management) |
| ZWPRODSTART | Date | Start of production (time management) |
| PROD_GESTELLNR | String | Production rack number |
| POS_BETR_MWST[1-5] | Number | Item tax 1-5 |
| POS_BETR_MWST[1-5]_FW | Number | Item tax - foreign currency 1-5 |
| POS_ITEM_MWST[1-5] | Number | Item's tax share 1-5 |
| POS_ITEM_MWST[1-5]_FW | Number | Item's tax share (foreign currency) 1-5 |
| POS_MWST[1-5]_BASIS | Number | Tax basis 1-5 |
| POS_MWST[1-5] | Number | Tax rate 1-5 |
| TAX_IVA | Number | IVA percentage for ICMS |
| FI_PREIS_ME_TAX | Number | Price per quantity unit including tax |
| PP_MENGE_GES | Number | Total item quantity |
| FI_PREIS_ME_GES | Number | Price per price unit for the complete item |
| FI_POS_GES_TAX | Number | Total item price including tax |
| TAX_CST | String | CST code |
| TAX_CFOP | String | CFOP code |
| TAX_NCM | String | NCM code |
| POS_PRCL_XXX | String | Value of product classifier with name XXX |

*Tab. 10: Printing of forms - item variables*

### 3.2.3. Footer variables

| Variable | Type | Description |
| :--- | :--- | :--- |
| DOC_SU_GEWICHT | Number | Total weight of goods per document |
| DOC_SU_LFM_FAKT | Number | Total circumference (rounded) per document |
| DOC_SU_LFM_REAL | Number | Total circumference (exact) per document |
| DOC_SU_QM_FAKT | Number | Total surface (rounded) per document |
| DOC_SU_QM_REAL | Number | Total surface (exact) per document |
| DOC_SU_STUECK | Number | Total quantity per document |
| DOC_SU_QM_FAKT_TPS | Number | Total TPS surface per document |
| DOC_SU_GEWICHT_TPS | Number | Total TPS weight per document |
| LAST_PAGE | Number | Flag for last page of form |
| SU_BETR_BRUTTO | Number | Total gross amounts |
| SU_BETR_BRUTTO_FW | Number | Total gross amounts in foreign currency |
| SU_BETR_BRUTTO_STR | String | Gross amount as string |
| SU_BETR_MWST1 | Number | Total VAT 1 |
| SU_BETR_MWST2 | Number | Total VAT 2 |
| SU_BETR_MWST3 | Number | Total VAT 3 |
| SU_BETR_MWST4 | Number | Total VAT 4 |
| SU_BETR_MWST5 | Number | Total VAT 5 |
| SU_BETR_MWST1_FW | Number | Total VAT 1 in foreign currency |
| SU_BETR_MWST2_FW | Number | Total VAT 2 in foreign currency |
| SU_BETR_MWST3_FW | Number | Total VAT 3 in foreign currency |
| SU_BETR_MWST4_FW | Number | Total VAT 4 in foreign currency |
| SU_BETR_MWST5_FW | Number | Total VAT 5 in foreign currency |
| SU_BETR_NETTO | Number | Total net amounts |
| SU_BETR_NETTO_FW | Number | Total net order amount in foreign currency |
| SU_BETR_SKONTO | Number | Total cash discount 1 |
| SU_BETR_SKONTO_FW | Number | Total cash discount 1 in foreign currency |
| SU_BETR_SKONTO2 | Number | Total cash discount 2 |
| SU_BETR_SKONTO2_FW | Number | Total cash discount 2 in foreign currency |
| SU_BETR_SKONTO3 | Number | Total cash discount 3 |
| SU_BETR_SKONTO3_FW | Number | Total cash discount 3 in foreign currency |
| SU_BETR_SKONTOSATZ1 | Number | Total cash discount rate 1 |
| SU_BETR_SKONTOSATZ2 | Number | Total cash discount rate 2 |
| SU_BETR_SKONTOSATZ3 | Number | Total cash discount rate 3 |
| SU_BRUTTO_WERT | Number | Gross value without surcharges |
| SU_BRUTTO_WERT_FW | Number | Gross value in foreign currency |
| SU_GEWICHT | Number | Total weight |
| SU_LFM_FAKT | Number | Total lin.m. invoiced |
| SU_MWST1_BASIS | Number | Total VAT basis 1 |
| SU_MWST2_BASIS | Number | Total VAT basis 2 |
| SU_MWST3_BASIS | Number | Total VAT basis 3 |
| SU_MWST4_BASIS | Number | Total VAT basis 4 |
| SU_MWST5_BASIS | Number | Total VAT basis 5 |
| SU_MWST1_BASIS_FW | Number | Total VAT basis 1 in foreign currency |
| SU_MWST2_BASIS_FW | Number | Total VAT basis 2 in foreign currency |
| SU_MWST3_BASIS_FW | Number | Total VAT basis 3 in foreign currency |
| SU_MWST4_BASIS_FW | Number | Total VAT basis 4 in foreign currency |
| SU_MWST5_BASIS_FW | Number | Total VAT basis 5 in foreign currency |
| SU_QM_FAKT | Number | Total sqm invoiced for the order |
| SU_QM_REAL | Number | Actual total sqm for an order |
| SU_LFM_REAL | Number | Actual total linear meters for an order |
| SU_STUECK | Number | Total quantity for the document |
| SU_EINFACHGLAS | Number | Number of single annealed sheets (item only) |
| SU_ESG | Number | Number of toughened sheets (item only) |
| SU_VSG | Number | Number of laminated sheets (item only) |
| SU_ISOEINH | Number | Total IG per order |
| AUSW_GESTELLE | String | Comma-separated string of own, off-site racks |
| FREMD_GESTELLE | String | Comma-separated string of off-site, external racks |

*Tab. 11: Printing of forms - footer variables*

### 3.2.4. BOM variables

| Variable | Type | Description |
| :--- | :--- | :--- |
| FI_PREIS_ME_SHEET1...FI_PREIS_ME_SHEET2 | Number | Price per quantity unit for glass 1 + glass 2 |
| FI_RABATT_SHEET1...FI_RABATT_SHEET2 | Number | Discounts for glass 1 + glass 2 |
| MOD_PO_PR_BETR_BRUTTO | Number | Shape - gross price |
| MOD_PO_PR_BETR_BRUTTO_FW | Number | Shape - gross price in foreign currency |
| MOD_PO_PR_BETR_NETTO | Number | Shape - net price |
| MOD_PO_PR_BETR_NETTO_FW | Number | Shape - net price in foreign currency |
| MOD_PO_PR_NETTO_GES | Number | Shape - net total |
| MOD_PO_PR_NETTO_GES_FW | Number | Shape - net total in foreign currency |
| MOD_PO_PR_PREIS_ME | Number | Shape price per price unit |
| MOD_PO_PR_PREIS_ME_FW | Number | Shape price per price unit in foreign currency |
| MOD_PO_PR_RABATT | Number | Shape discount |
| MOD_PO_PR_EINHEIT | String | Shape - price unit |
| MOD_ITEM_MWST1 | Number | BOM Tax 1 share (only if option is set) |
| MOD_ITEM_MWST1_FW | Number | BOM Tax 1 share in foreign currency (only if option is set) |
| MOD_ITEM_MWST2 | Number | BOM Tax 2 share (only if option is set) |
| MOD_ITEM_MWST2_FW | Number | BOM Tax 2 share in foreign currency (only if option is set) |
| MODELLBEZ | String | Model name |
| MODELLPARAM | String | Shape parameters (height, width, height 1 etc.) |
| MOD_BIT_STRING | String | 1. string with manual amendment flags |
| MOD_BIT2_STRING | String | 2. string with manual amendment flags |
| MOD_BIT3_STRING | String | 3. string with manual amendment flags |
| MOD_PREIS_BIT_STRING | String | Bit vector for pricing information |
| **1st grid** | | |
| SP1_PO_PR_BETR_BRUTTO | Number | Gross Georgian bar price (1st grid) |
| SP1_PO_PR_BETR_BRUTTO_FW | Number | Gross Georgian bar price in foreign currency (1st grid) |
| SP1_PO_PR_BETR_NETTO | Number | Net Georgian bar price (1st grid) |
| SP1_PO_PR_BETR_NETTO_FW | Number | Net Georgian bar price in foreign currency (1st grid) |
| SP1_PO_PR_NETTO_GES | Number | Total net Georgian bar price (1st grid) |
| SP1_PO_PR_NETTO_GES_FW | Number | Total net Georgian bar price in foreign currency (1st grid) |
| SP1_PO_PR_PREIS_ME | Number | Georgian bar price per price unit (1st grid) |
| SP1_PO_PR_PREIS_ME_FW | Number | Georgian bar price per price unit in foreign currency (1st grid) |
| SP1_PO_PR_RABATT | Number | Georgian bar discount (1st grid) |
| SP1_PO_PR_EINHEIT | String | Georgian bar price unit (1st grid) |
| SP1_ITEM_MWST1 | Number | BOM Tax 1 share (only if option is set - 1st grid) |
| SP1_ITEM_MWST1_FW | Number | BOM Tax 1 share in foreign currency (only if option is set - 1st grid) |
| SP1_ITEM_MWST2 | Number | BOM Tax 2 share (only if option is set - 1st grid) |
| SP1_ITEM_MWST2_FW | Number | BOM Tax 2 share in foreign currency (only if option is set - 1st grid) |
| SPRO_SZR1 | Number | Grid in 0=main item, 1=1. AIR, 2=2. AIR (1st grid) |
| SPR1_ERFASSUNGSTYP | Number | Input type 0=Standard bar, 1=template bar (1st grid) |
| SPR_BER_KZ1(2) | Number | Drill holes: 0=drill point-symm.; 1=field-symm.; 2=drill point-asymm.; 3=field-assym. (1st grid) ATTENTION: only for vertical bars, the first parameter is the vertical bar |
| SPR1_ASSYM_MASSE | String | Horizontal bar: drill point-asymmetrical sizes as string |
| SPR2_ASSYM_MASSE | String | Vertical bar: drill point-asymmetrical sizes as string |
| SPR1_ASSYM_MASSE_INCH | String | Horizontal bar: drill point-asymmetrical sizes as string (in inch) (1st grid) |
| SPR2_ASSYM_MASSE_INCH | String | Vertical bar: drill point-asymmetrical sizes as string (in inch) (1st grid) |
| KZ_SPR_KONSTR1(2) | Number | Georgian bars: 0=Standard; 1=T bar on top; 2=T bar at the bottom (1st grid) ATTENTION: only for vertical bars, the first parameter is the vertical bar |
| SPROANZ1 | Number | No. of horizontal bars (1st grid) |
| SPROANZ2 | Number | No. of vertical bars (1st grid) |
| SPROBEZ1 | String | Georgian bar name 1 (1st grid) |
| SPROBEZ2 | String | Georgian bar name 2 (1st grid) |
| SPROFARBE1 | String | Georgian bar color - horizontal (1st grid) |
| SPROFARBE2 | String | Georgian bar color - vertical (1st grid) |
| SPR_BREITE1 | Number | Georgian bar width - horizontal (1st grid) |
| SPR_BREITE_INCH1 | String | Georgian bar width in inch, horizontal (1st grid) |
| SPR_BREITE2 | Number | Georgian bar width vertical (1st grid) |
| SPR_BREITE_INCH2 | String | Georgian bar width in inch, vertical (1st grid) |
| SPR_DICKE1 | Number | Georgian bar thickness horizontal (1st grid) |
| SPR_DICKE_INCH1 | String | Georgian bar thickness in inch, horizontal (1st grid) |
| SPR_DICKE2 | Number | Georgian bar thickness vertical (1st grid) |
| SPR_DICKE_INCH2 | String | Georgian bar thickness in inch, vertical (1st grid) |
| SPR_BIT_STRING1 | String | 1st string with manual amendment flags (1st grid) |
| SPR_BIT2_STRING1 | String | 2nd string with manual amendment flags (1st grid) |
| SPR_BIT3_STRING1 | String | 3rd string with manual amendment flags (1st grid) |
| SPR_PREIS_BIT_STRING1 | String | Bit vector for pricing information (1st grid) |
| SPR_BIT_STRING2 | String | 1st string with manual amendment flags (2nd grid) |
| SPR_BIT2_STRING2 | String | 2nd string with manual amendment flags (2nd grid) |
| SPR_BIT3_STRING2 | String | 3rd string with manual amendment flags (2nd grid) |
| SPR_PREIS_BIT_STRING2 | String | Bit vector for pricing information (2nd grid) |
| **2nd grid** | | |
| SP11_PO_PR_BETR_BRUTTO | Number | Gross Georgian bar price (2nd grid) |
| SP11_PO_PR_BETR_BRUTTO_FW | Number | Gross Georgian bar price in foreign currency (2nd grid) |
| SP11_PO_PR_BETR_NETTO | Number | Net Georgian bar price (2nd grid) |
| SP11_PO_PR_BETR_NETTO_FW | Number | Net Georgian bar price in foreign currency (2nd grid) |
| SP11_PO_PR_NETTO_GES | Number | Total net Georgian bar price (2nd grid) |
| SP11_PO_PR_NETTO_GES_FW | Number | Total net Georgian bar price in foreign currency (2nd grid) |
| SP11_PO_PR_PREIS_ME | Number | Georgian bar price per price unit (2nd grid) |
| SP11_PO_PR_PREIS_ME_FW | Number | Georgian bar price per price unit in foreign currency (2nd grid) |
| SP11_PO_PR_RABATT | Number | Georgian bar discount (2nd grid) |
| SP11_PO_PR_EINHEIT | String | Georgian bar price unit (2nd grid) |
| SP11_ITEM_MWST1 | Number | BOM Tax 1 share (only if option is set - 2nd grid) |
| SP11_ITEM_MWST1_FW | Number | BOM Tax 1 share in foreign currency (only if option is set - 2nd grid) |
| SP11_ITEM_MWST2 | Number | BOM Tax 2 share (only if option is set - 2nd grid) |
| SP11_ITEM_MWST2_FW | Number | BOM Tax 2 share in foreign currency (only if option is set - 2nd grid) |
| SPRO_SZR11 | Number | Grid in 0=main item, 1=1. AIR, 2=2. AIR (2nd grid) |
| SPR11_ERFASSUNGSTYP | Number | Input type 0=Standard bar, 1=template bar (2nd grid) |
| SPR_BER_KZ11(22) | Number | Drill holes: 0=drill point-symm.; 1=field-symm.; 2=drill point-asymm.; 3=field-assym. ATTENTION: only for vertical bars, the first parameter is the vertical bar |
| SPR11_ASSYM_MASSE | String | Horizontal bar: drill point-asymmetrical sizes as string (1st grid) |
| SPR22_ASSYM_MASSE | String | Vertical bar: drill point-asymmetrical sizes as string (2nd grid) |
| SPR11_ASSYM_MASSE_INCH | String | Horizontal bar: drill point-asymmetrical sizes as string (in inch) (2nd grid) |
| SPR22_ASSYM_MASSE_INCH | String | Vertical bar: drill point-asymmetrical sizes as string (in inch) (2nd grid) |
| KZ_SPR_KONSTR11(22) | Number | Georgian bars: 0=Standard; 1=T bar on top; 2=T bar at the bottom (2nd grid) ATTENTION: only for vertical bars, the first parameter is the vertical bar |
| SPROANZ11 | Number | No. of horizontal bars (2nd grid) |
| SPROANZ22 | Number | No. of vertical bars (2nd grid) |
| SPROBEZ11 | String | Georgian bar name 1 (2nd grid) |
| SPROBEZ22 | String | Georgian bar name 2 (2nd grid) |
| SPROFARBE11 | String | Georgian bar color - horizontal (2nd grid) |
| SPROFARBE22 | String | Georgian bar color - vertical (2nd grid) |
| SPR_BREITE11 | Number | Georgian bar width - horizontal (2nd grid) |
| SPR_BREITE_INCH11 | String | Georgian bar width in inch, horizontal (2nd grid) |
| SPR_BREITE22 | Number | Georgian bar width vertical (2nd grid) |
| SPR_BREITE_INCH22 | String | Georgian bar width in inch, vertical (2nd grid) |
| SPR_DICKE11 | Number | Georgian bar thickness horizontal (2nd grid) |
| SPR_DICKE_INCH11 | String | Georgian bar thickness in inch, horizontal (2nd grid) |
| SPR_DICKE22 | Number | Georgian bar thickness vertical (2nd grid) |
| SPR_DICKE_INCH22 | String | Georgian bar thickness in inch, vertical (2nd grid) |
| SPR_BIT_STRING11 | String | 1st string with manual amendment flags (2nd grid) |
| SPR_BIT2_STRING11 | String | 2nd string with manual amendment flags (2nd grid) |
| SPR_BIT3_STRING11 | String | 3rd string with manual amendment flags (2nd grid) |
| SPR_PREIS_BIT_STRING11 | String | Bit vector for pricing information (2nd grid) |
| SPR_BIT_STRING22 | String | 1st string with manual amendment flags (2nd grid) |
| SPR_BIT2_STRING22 | String | 2nd string with manual amendment flags (2nd grid) |
| SPR_BIT3_STRING22 | String | 3rd string with manual amendment flags (2nd grid) |
| SPR_PREIS_BIT_STRING22 | String | Bit vector for pricing information (2nd grid) |
| SPR_FELDANZAHL | Number | Number of fields |
| SPRO_PARAM | String | Georgian bar parameters (see BOM parameter description) |
| NOPPEN_KZ | Number | Georgian bar felts (-1=small bars, 0=no, 1=yes) |
| STX_AUTOZUSCHN | Number | Code 'automatic cutting' |
| STX_BEZ | String | BOM name |
| STX_MENGE | Number | Number of BOM elements |
| STX_PARAM | String | BOM parameter string for product type, width, height, quantity, sense of pattern, shape parameters. |
| STX_PR_BETR_BRUTTO | Number | Gross BOM amount |
| STX_PR_BETR_BRUTTO_FW | Number | Gross BOM amount in foreign currency |
| STX_PR_BETR_NETTO | Number | Net BOM amount |
| STX_PR_BETR_NETTO_FW | Number | Net BOM amount in foreign currency |
| STX_PR_EINHEIT | String | BOM price unit |
| STX_PR_MEEINHEIT | String | BOM quantity unit |
| STX_PR_NETTO_GES | Number | Total net BOM amount |
| STX_PR_NETTO_GES_FW | Number | Total net BOM amount in foreign currency |
| STX_PR_PREIS_ME | Number | BOM price per quantity unit |
| STX_PR_PREIS_ME_FW | Number | BOM price per quantity unit in foreign currency |
| STX_PR_PREISDRUCK | Number | Print BOM price |
| STX_PR_RABATT | Number | Discount on BOM |
| STX_EK_NETTO_GES | Number | Total cost for this BOM |
| STX_ITEM_MWST1 | Number | BOM Tax 1 share (only if option is set) |
| STX_ITEM_MWST1_FW | Number | BOM Tax 1 share in foreign currency (only if option is set) |
| STX_ITEM_MWST2 | Number | BOM Tax 2 share (only if option is set) |
| STX_ITEM_MWST2_FW | Number | BOM Tax 2 share in foreign currency (only if option is set) |
| STXSCHKZ | Number | Sheet code: 0=no sheet processed; 1=1st sheet processed; 2=2nd sheet processed; 3=3rd sheet processed. |
| GLAS1_BESCH...GLAS2_BESCH | Number | Coating code for both IG sheets: 1=coated |
| STXKZ_BESTELLUNG | Number | BOM purchasing code |
| STX_FER_BESCHAFFARTNR | Number | Supply type number of this BOM |
| STX_AGGREGATE | String | Time management: machines sorted by process sequence (glass only) |
| STX_BIT_STRING | String | 1. string with manual amendment flags |
| STX_BIT2_STRING | String | 2. string with manual amendment flags |
| STX_BIT3_STRING | String | 3. string with manual amendment flags |
| STX_GEBOGEN | String | Parameter string for curved glass (structure see tab 'curved glass') |
| STX_PREIS_BIT_STRING | String | Bit vector for pricing information |
| SZR1_RUECKSCHNITT | String | Cutback per edge in airspace 1 (00/00/00/00/-/-/-/-) |
| SZR1_RUECKSCHNITT_INCH | String | Cutback per edge in airspace 1 (00/00/00/00/-/-/-/-) in inch |
| SZR2_RUECKSCHNITT | String | Cutback per edge in airspace 2 (00/00/00/00/-/-/-/-) |
| SZR2_RUECKSCHNITT_INCH | String | Cutback per edge in airspace 2 (00/00/00/00/-/-/-/-) in inch |
| SPR_SKIZZE | Object | Georgian bar sketch/pattern |
| STX_BOMID | Number | ID of respective BOM element |
| STX_PROD | Number | Product number of respective BOM element |
| STX_BESCHAFFART_BEZ | String | Procurement type |
| STX_PRCL_XXX | String | Value of product classifier with name XXX |

*Tab. 12: Printing of forms - BOM variables*

### 3.2.5. BOM parameters: (STx_PARAM)
If the product type is not 12 (shape/step)
| Displacement | Length | Description |
| :--- | :--- | :--- |
| 0 | 3 | Product type |
| 3 | 15 | Width |
| 18 | 15 | Height |
| 33 | 5 | Quantity |
| 38 | 1 | Sense of pattern |
| 39 | 10 | Sqm invoiced |
| 49 | 10 | Lin.m. invoiced |
| 59 | 20 | Quantity unit |
| 79 | 3 | Product group |
| 82 | 40 | Color |
| 122 | 15 | Width Inch |
| 137 | 15 | Height Inch |
| 152 | 1 | Coated side |
| 153 | 1 | Pattern side |

*Tab. 13: Printing of forms - BOM parameters*

**Georgian bar parameters SPRO_PARAM**
| Displacement | Length | Description |
| :--- | :--- | :--- |
| 0 | 10 | Lin.m. of Georgian bars for this item |
| 10 | 10 | Price per lin.meter |

*Tab. 14: Printing of forms - Georgian bar parameters*

**If the product type is 12 (shape/step)**
| Displacement | Length | Description |
| :--- | :--- | :--- |
| 0 | 3 | Product type |
| 3 | 80 | Shape/step parameters |

*Tab. 15: Printing of forms - shape parameters*

### 3.2.6. Bit vector structure

**POS_BIT_STRING and STX_BIT_STRING**
Position of the bit in the string, starting from the right!
1.  Sales price list
2.  Sales price code
3.  Sales price unit
4.  Sales price per quantity unit
5.  Change of basic product (2x replacement)
6.  Sales discount
7.  Purchase price list
8.  Purchase price code
9.  Purchase price unit
10. Purchase price per quantity unit
11. Purchase discount
12. Product group
13. Product group - statistics
14. Performance
15. Shape width and height
16. BOM width and height
17. BOM quantity
18. Sales BOM quantity
19. Purchase BOM quantity
20. Supply type
21. <internal>
22. Product name 1 or BOM name
23. Product name 2 or BOM short name
24. Product name 3 or processing remarks
25. Cutback
26. Commission rate 1
27. Commission rate 2
28. Sales price relevant
29. Purchase price relevant
30. Spacer text
31. Weight

*Tab. 16: Bit vectors*

**ZUSCHLAG_BIT_STRING**
Position of the bit in the string, starting from the right!
1.  Pattern
2.  Edge stripping
3.  Maximum surface
4.  Maximum aspect ratio
5.  Edge protection
6.  free
7.  free
8.  Weight, rounded
9.  Transport
10. Shipping fee
11. Express surcharge
12. Recycling
13. Special discount 1
14. Special discount 2
15. Special discount 3
16. Special discount 4
17. Rack 1
18. Monthly invoice
19. AIR
20. Invoicing
21. Deposit
22. Special discount 5
23. Special discount 6
24. Special discount 7
25. Special discount 8
26. Felt pads
27. Shortfall
28. Rack 2
29. Energy
30. Special discount 9
31. Special discount 10

*Tab. 17: Surcharge bits*

**POS_BIT2_STRING und STX_BIT2_STRING**
Position of the bit in the string, starting from the right!
1.  Thickness
2.  Minimum quantity
3.  VAT code
4.  Insurance product
5.  Item text 1
6.  Item text 2
7.  Item text 3
8.  Item text 4
9.  Item text 5
10. Total item price - sales
11. Total item price - purchasing
12. Production costs (PCC)
13. Minimum quantity calculation switched off
14. Individual price calculation switched off
15. Miscellaneous surcharges switched off
16. Stock size recognition switched off
17. Sales production cost switched off
18. Purchase production cost switched off
19. <internal>
20. <internal>
21. PCC calculated
22. <internal>
23. <internal>
24. PCC main discounts
25. <internal>
26. <internal>
27. <internal>
28. Label control

*Tab. 18: BIT 2 item and BOM*

**POS_BIT3_STRING and STX_BIT3_STRING:**
Position of the bit in the string, starting from the right! Not used at present!

**POS_PREIS_BIT_STRING and STx_PREIS_STRING:**
1.  Minimum quantities calculated
2.  Individual price calculated
3.  Miscellaneous surcharge calculated
4.  Stocksize calculated

*Tab. 19: BIT 3 item and BOM*

**Example: use in connection with report builder**
The expression is TRUE if the sales discount and the item thickness were changed:
`StrToNumber (StrMid (POS_BIT_STRING, 26, 1 ) ) * StrToNumber ( StrMid (POS_BIT2_STRING, 31, 1))`

### 3.2.7. Parameters for bent glass (STx_GEBOGEN)

| Displacement | Length | Description |
| :--- | :--- | :--- |
| 0 | 10.2 | Outside chord size |
| 10 | 10.2 | Outside sectional height |
| 20 | 10.2 | Outside circumference |
| 30 | 10.2 | Outside radius |
| 40 | 10.2 | Neutral chord size |
| 50 | 10.2 | Neutral sectional height |
| 60 | 10.2 | Neutral circumference |
| 70 | 10.2 | Neutral radius |
| 80 | 10.2 | Inside chord size |
| 90 | 10.2 | Inside sectional height |
| 100 | 10.2 | Inside circumference |
| 110 | 10.2 | Inside radius |
| 120 | 10.2 | Degrees |
| 130 | 10.2 | Outside sectional height of biggest sheet |
| 140 | 10.2 | Outside chord size of biggest sheet |
| 150 | 10.2 | Shape type (0 = inside, 1 = outside) |

*Tab. 20: Bent glass parameters*

## 3.3. Print dimensioned sketches on forms

Prerequisite is the installation of Shaping & Nesting. The following amendments must be made in the initialization file SN.INI, section [Picture]:
`FontHeight = -10`
`Height = 261`
`Width = 261`

In section [Screen], parameter `ModelFrameCorrection` must be set to 0.

A new bitmap field called `MOD_LOGO_VSKZ` must be entered in the corresponding form. Also, you have to create the input variable `VERSK_DRUCK`, type `Number`. Size, position and other properties of the field can be adopted from a standard form (Speedy G:\Report\German\Auftrag.Qrp). Field `Print dimensioned sketches` has to be tagged in management of forms. To enlarge the sketch, you need to amend the bitmap field in the report as well as the settings for width and height in SN.INI to the new requirements.

> **IMPORTANT!** To guarantee a smooth and correct printout, you should install SN version 3.14-02 from directory Install_Speedy\Versions\Setup\Sn3_ALFAK2.4_2.

## 3.4. Printing of production sketches from version 3.3

A file name for a sketch can be entered (per product) in tab 1 in product master data. Also, you can define on tab “production” whether the sketch shall be printed on the order forms, or as a dimensioned sketch (special printout: product sketch). (Code: article sketch – print on forms)

In the order forms, the input variable PROD_BMP is filled as an OBJECT (see AUFTRAG.QRP), in the sketch printing form MODSKIZZE.QRP, the existing OBJECT variable MOD_LOGO_VSKZ is used since this is a special printout.

Article info (accessible from product management and item entry) defines the path in which ALFAK shall search for the product sketch. If no workstation-related path is defined, ALFAK will search for the sketch in path "...ALFAK2000 3.3\Products" by default.

Furthermore, article info provides information on prices and inventory.
Detailed information: `\\Hausi\BUG\A+W_Allgemein\Allgemeine Entwicklungen\Alfak2000 3.3\Spezifikation Produktskizzen.doc`

## 3.5. Print server installation

From ALFAK2000 version 4.1, printing of forms can be transferred from the clients to the server. Also, you can define print jobs, for example to print delivery note and invoice with the same job. ALFAK now also supports the mailing of PDF files via the gotomaxx PDF mailer. The print server will work only if a user has been registered on the server on which it is being run.

### 3.5.1. Installation of server and client
For server installation, please make sure to install SQL Base Engine Version 8.5 or higher. On the server, the print server (abcdruckserver.exe) has to be started by a link in the autostart directory of the registered user.

### 3.5.2. Configuration of the master data
Printing from the server usually requires the definition of print jobs. The appropriate dialog is found in master data, menu “Forms - Print jobs". You can define one or more print batches per print job. When you switch to the new input mode, first enter the name of the print job, then the document type. After saving the print job, click on the buttons „Add/Delete" to define the print batches. If an existing print job is selected prior to a new entry, the print batches involved will be imported as well. The sequence of the print batches is decisive as the document status is updated after each print job, and the lock and minimum statuses are checked before printing.

Please note that when you define the print jobs, the printer names must be available on the server. It is therefore best to enter the print jobs directly on the server as the combobox „Printer" only allows to select the printers installed on that computer.

### 3.5.3. Sending emails via PDF mailer
Server printout allows to email PDF files using the program „maxx PDFMAILER Professional" Version 3.0 by gotomaxx GmbH. Standard, Professional, and Promotion. Promotion and Standard will not recognise control codes and are therefore not suited to our needs.

The Professional version can be found in `\\Jupiter\ALFAK_Software\Utility Programme\PDFMailer\pdfmailer3prode.exe` and can be used for testing.

After installing PDFMAILER, you only need to set the printer name, and activate checkbox „mail" when you define the print job. In company master data, tab 4 Documents in mail options, you need to set Email via PDF file.

Then, only a couple of settings need to be checked/adapted in PDFMAILER. For this purpose, start the PDFMAILER using the Windows start button and program „gotomaxx". Via menu „Settings - Edit", access the settings dialog.

*Fig. 64: PDF- Mailer properties - Output*

The tab should look as shown above.

*Fig. 65: PDF- Mailer properties - Mailer*

Now set the email system in tab Mailer, and disable the checkbox Open email client.

### 3.5.4. The PDF mailer form
To transfer the mail address, the reference line, and the name of the PDF file from ALFAK2000 to the PDFMAILER, you need to enter a couple of control sequence in the form header. The form will be saved in the customer's form path, and will be set when defining the print job.

An example for such a form for printing order confirmations is installed with ALFAK2000 and is called „AUFTRAG_PDF.QRP". Variable „MAILHEADER" controls whether the control codes will be printed. A description of the control commands is available in the PDFMAILER documentation; also, the example form is self-explanatory.

Please make sure that the distance between first control line and top margin is at least 0.8 inches. If not, the PDFMailer will fail to recognise the control line; email despatch will not work correctly.

## 3.6. Form printing in the DMS system (Saperion)

The forwarding of the printout to a DMS system (e.g. Saperion) is controlled by a print driver and the batch bat\printdms.bat. This send the print order to the DMS system and to a printer driver for the physical printer. The 3 transfer parameters to the batch are:
1.  PCL output file with path
2.  Output printer driver is forwarded to the print order
3.  Target path for the DMS program

So that an INI file does not have to be created for each user in order to set up the transfer to the DMS system (e.g. Saperion), the logic was expanded in the INI file.

**Entry in the INI file:**
```ini
[DMS]
PrintDMS=C:\alfak\bat\printdms.bat (the batch file must still be specified)
File=C:\temp (if only a path is entered here, then the file alfak_<Loginname>.pcl is generated automatically)
```
The printer entry must be removed, then the printer DMS_<Loginname> is addressed. A writing back of the values to the INI file is no longer undertaken.
`Printer=ALFAKDMS_xx`

## 3.7. Portuguese certification

### 3.7.1. Introduction
As from 01.01.2011, regulations in Portugal demand that commercial software which is used for printing invoices must be certified by the government before using it. This function has been integrated in ALFAK and is described on the following pages. The user must run the appropriate scripts on the corresponding database first (20120116a.sql and 20120116aa.sql; language-based 20120116m.sql and 20120117a.sql).

### 3.7.2. Company Master Data
Company master data (Master data > Company > Company data > tab 5.Parameter) now allows to enable the certification for the Portuguese market. This function is licensed and comes with a new module.

*Fig. 66: Portug. Certi. Company master data settings*

The reason for this is the digital signature on invoices and credit notes. Portuguese certification can only be enabled by the system administrator. If it is active in the company master data, you can use the Parameter management button to start a dialog in which various parameters can be maintained. When you open the dialog for the first time, the private and the public key for the invoice signature will be created during the saving routine.

*Fig. 67: Portug. Certi. - Certification code*

These will be saved in the system (temporary Windows directory of the current user) and stored in the database. The certification code - which is assigned by the Portuguese government - must be entered in a special field. Once saved, these three parameters cannot be changed.

### 3.7.3. Invoice printing
To print invoices for the entered orders, go to dialog Form/label printing (Documents > Order > Print order). Digital signatures can be created there for printing Invoices (orders) and Credit notes. This is done in the background of the actual printing process. Prerequisite is the installation of the Freeware tool OpenSSL-Win32 which is installed on the system together with ALFAK. When you start the printing of invoices/credit notes, the private key will create a hash code with different parameters like e.g. the invoice number, invoice date, etc. This hash code is the digital signature for the current document and will be used as a parameter for creating the hash code of the next document, referring to the order area. The printout includes the certification code and four digits of the hash code (1., 11., 21. and 31. digit, separated by “ – “).

*Fig. 68: Portug. Certi. - Invoice printing*

The document status changes to „Invoice printed". This means that invoices must not be changed. This is achieved by enabling the option Lock documents after printing of invoice in company master data (Master data > Company > Company data > tab 5.Parameter). There, status point „0103 – Print invoice" must be defined for locking the document from this status point on.
