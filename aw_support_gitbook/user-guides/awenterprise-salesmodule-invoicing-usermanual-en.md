---
title: "EN-UM-AW_Enterprise-Sales_4_8"
source: "EN-UM-AW_Enterprise-Sales_4_8.pdf"
tags: ["A+W Enterprise Sales", "Software Reference", "Sales Module", "Invoicing", "Order Management", "Credit Notes", "Document Research", "Form Printing", "Order Status", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A software reference manual for the A+W Enterprise Sales module, version 4.00. This guide provides detailed descriptions of dialogs, fields, and functions related to managing sales documents, including invoices, credit notes, forms, order status tracking, and document research."
long_description: "This document is a comprehensive software reference guide for the A+W Enterprise Sales module, version 4.00, dated March 2020. It is intended for users and administrators of the A+W Enterprise software. The manual meticulously details the functionalities within the Sales module, breaking down complex processes into understandable sections. Key areas covered include: **Invoices**, with instructions for creating partial, final, manual, and automatic invoices; **Credit Notes**, explaining how to enter and book credits; **Forms**, detailing procedures for direct printing, form printing, and sending documents via email; **Order Status**, offering an in-depth look at the Order Information dialog with its numerous tabs for tracking every aspect of an order from items and purchasing to production, dispatch, and barcoding; and **Document Research**, which explains how to use the powerful search tool to find documents based on a wide range of criteria. Each section provides navigation paths, screenshots of the user interface, and detailed descriptions of every field, tab, and function, including technical information like database field names. This guide serves as an essential resource for day-to-day operations and for understanding the full capabilities of the A+W Enterprise Sales system."
---

---
## Invoices

- **Date:**
    - Display of the due date for the partial amount.
    - Technical info: display field, DB field: zahlplan.ztplan
- **Chc:**
    - Checked. Indication whether the invoice has already been checked. Depending on the configuration, an invoice can only be created if it was already checked by the authorized employee.
    - ☐ The invoice was checked and can be generated.
    - ☐ The invoice was not yet checked. Depending on the configuration, it may not be possible to generate the invoice.
    - Technical info: checkbox, display field
- **Cre:**
    - Create the partial invoice when you trigger invoice creation using <F3>.
    - ☑ Create partial invoice.
    - ☐ Do not create partial invoice.
    - Technical info: checkbox

### Information on Document tab

The Information on Document tab only appears on the Invoices (automatic) and Delivery Notes (automatic) dialogs:
- ⇨ "Invoices (automatic)" on page D-341
- ⇨ "Delivery Notes (automatic)" on page D-335

## Partial Invoice (manual)

**Sales > Invoices > Partial Invoice > Manual Invoice**

*Fig. D-146 Partial Invoice (manual)*

Use this dialog to create partial invoices manually.

If there is a payment plan for the order, a notice appears asking whether the dates for the payment plan should be displayed. If you say yes, then you can select a date from the payment plan.

Manual partial invoices are entered like manual invoices. The Partial Invoice (manual) and Invoices (manual) dialogs look largely the same.

In the item area, a new item is displayed in the last line. It lists the partial amount with the amount from the payment plan.

The fields are described in connection with the Invoices (manual) dialog:
- ⇨ "Invoices (manual)" on page D-346:

In addition, the following fields are displayed:

### Footer

The total amount of the order is displayed in the Order field. If an invoice has already been generated for the reference document, the total amount of the invoice to which reference is being made is displayed in the Invoice Total field.

## Final Invoices (automatic)

**Sales > Invoices > Final Invoice > Automatic Release**

*Fig. D-147 Final Invoices (automatic)*

Use this dialog to create the final invoice for orders for which a payment plan was created. If there are orders for the current day for which there is a payment plan, then you can import the orders with <Ctrl>+<F8>. You can also enter the order numbers manually or search for them with <F9>.

The footer displays the customer name and total amount from the order for which a final invoice is being created.

Use <F3> to have the system generate the final invoices for the selected orders. In order entry, the individual orders are displayed as invoiced with the respective invoice number.

- **Order:**
    - Order number with payment plan. If you specify a number, the other fields are populated automatically with the appropriate values.
    - Technical info: mandatory field, numeric field, DB field: kauf.auftrnr, zahlplan.auftrnr
- **Amount:**
    - Amount of the final invoice. The final invoice is calculated from the total amount of the order together with the credits and less the already entered partial invoices.
    - Technical info: display field, DB field: zahlplan.betrag
- **Deliv. Note:**
    - Indicates if there is already a delivery note or partial invoice. If a delivery note exists, then the entry exists is in this field.
    - Technical info: display field
- **Date:**
    - Display of the entry date of the document.
    - Technical info: display field, DB field: kauf.edat
- **Chc:**
    - Checked. Indication whether the invoice has already been checked. Depending on the configuration, an invoice can only be created if it was already checked by the authorized employee.
    - ☑ The invoice was checked and can be generated.
    - ☐ The invoice was not yet checked. Depending on the configuration, it may not be possible to generate the invoice.
    - Technical info: checkbox, display field
- **Cr.:**
    - Created. Specification whether the invoice should be created.
    - ☑ The final invoice will be generated.
    - ☐ The final invoice will not be generated.
    - Technical info: checkbox

## Final Invoices (manual)

**Sales > Invoices > Final Invoice > Manual Invoice**

*Fig. D-148 Final Invoices (manual)*

Use this dialog to create final invoices manually.

Manual final invoices are entered like manual invoices. The Final Invoice (manual) and Invoices (manual) dialogs look largely the same.

The fields are described in connection with the Invoices (manual) dialog:
- ⇨"Invoices (manual)" on page D-346:

In addition, the following fields are displayed:

### Footer

The total amount of the order is displayed in the Order field. If an invoice has already been generated for the reference document, the total amount of the invoice to which reference is being made is displayed in the Invoice Total field.

## Invoice Log

**Sales > Invoices > Log**

*Fig. D-149 Invoice Log*

This dialog displays the invoice log. All documents for the invoices are noted with specification of the date and time.

If you are working with internal site separation, first a dialog opens where you can specify the site number. The log displays only the documents for the selected site.

> **Invoice log for the current day**
> An invoice log is generated for the current day. If the error message is displayed that the file is empty or not readable, then no invoices have been generated on this day.

## Credit Notes

The following dialogs are described in this section:
- "Credit Notes" on page D-356
- "Book Credit Notes" on page D-358

### Credit Notes

**Sales > Credit Notes > Enter Credit Notes**

*Fig. D-150 Credit Notes*

Use this dialog to enter credit notes. You can enter quantity credits or price credits. If you want to enter a quantity credit, you have to enter the article quantity that you want to credit in the Credit field of the appropriate item. If you want to enter a price credit, you have to enter the price that you want to credit in the price field of the appropriate item.

The fields are described for the Order Entry dialog:
- ⇨ "Order Entry" on page D-84

In addition, the following fields are displayed.

#### Header

**Number** Temporary number of the credit. After completion of the credit creation, the system creates a final credit number. Technical info: numeric field, DB field: kauf.auftrnr

**Ref.** Document number that is being referenced. By default, an invoice number is input for a credit.
Technical info: numeric field, DB field: kauf.referenz

#### General tab

**Cr.Note** Number of credited units of the item.
Technical info: numeric field, DB field: kpos.berechnet

#### Footer

If an invoice has already been generated for the reference document, the total amount of the invoice to which reference is being made is displayed in the Invoice Total field.

## Book Credit Notes

**Sales > Credit Notes -> Book Credit Notes**

*Fig. D-151 Book Credit Notes*

Use this dialog to book credits that have not yet been transferred to the FinAc. Generally credits are booked automatically after generation.

In exceptional cases, the credit can also be booked after the fact. In the credit entry, depending on the configuration, when generating the credit a query can be displayed asking whether the credit should be booked. If you respond [No] to the query, you can import this unbooked credit on the Book Credit Notes dialog and book it after the fact.

Use <Ctrl>+<F8> to import the data for all credits that are generated in the specified period.

The footer displays the customer name and total amount from the order for which the credit is booked.

Use <F3> to book the selected credits.

### Credit Notes tab

- **Cre. Note:**
    - Number of the credit.
    - Technical info: numeric field, DB field: kauf.auftrnr
- **SubNo:**
    - Display of the subnumber for partial credits.
    - Technical info: display field, DB field: kauf.subnr
- **External No.:**
    - Display of the document number that is specified by the customer. For credits from another site, the order number of the sending site is in this field.
    - Technical info: display field, DB field: kauf.exaufnr
- **Ref.:**
    - Invoice number from the field Reference in the Entry of credit notes dialog.
    - Technical info: display field, DB field: kauf.referenz
    - ⇨ "Credit Notes" on page D-356
- **Doc. Date:**
    - Display of the date of the credit creation.
    - Technical info: display field, DB field: kauf.edat
- **Book Date:** Display of the date of the credit booking. By default, the current date is entered. If you want to specify another booking date, you have to enter the new date in the field, confirm the entry, and enter the new date again. The date is only taken over into the field after the second entry.
    - Technical info: date field, DB field: kauf.bdat
- **Bk.:**
    - Specification whether the credit should be booked.
    - ☑ The credit will be booked.
    - ☐ The credit will not be booked.
    - Technical info: checkbox

Use <F5> to open the Items dialog on which additional details about the items are displayed.
- ⇨ "Item Info" on page D-344

### Information on Document tab

The Information on Document tab only appears on the Invoices (automatic) and Delivery Notes (automatic) dialogs:
- ⇨ "Invoices (automatic)" on page D-341
- ⇨ "Delivery Notes (automatic)" on page D-335

## Forms

For the various documents, you can print forms or send them via e-mail. The forms can be generated via a REP generator or a print service with Crystal Reports.

The following dialogs are described in this section:
- "Direct Printing" on page D-360
- "Form Printing" on page D-361
- "E-mail" on page D-365
- "Print on" on page D-367
- "List Printing" on page D-368

### Direct Printing

**Sales > Order Entry > Header, Footer area > <F4> > Direct Printing**

*Fig. D-152 Direct Printing*

Use this dialog to print out a form for the open document. You select the form type and printer for printout on the selection dialogs.

**Form Type** Specification of the form type that you want to print for the open document. Use <F9> to open a selection dialog with the available form types. The form types are stored in the system settings in the print management.
Technical info: numeric field, DB field: rep.formart

**Printer** Number of the printer for printing. Use <F9> to open a selection dialog with the available printers. The printers are stored in the system settings in the print management and assigned to the various form types.
Technical info: numeric field, DB field: drucker.drunr

Printing start if you have selected a form type and a printer and the system is configured appropriately. The Direct Printing dialog closes automatically.

### Form Printing

**Sales > Forms > Print**

*Fig. D-153 Form Printing*

Use these dialogs to select one or several documents for form printing.

On the Form Type selection dialog, you select the form type that you want to print. The selected form type is displayed in the upper left corner of the Form Printing dialog. Under some circumstances, you can also select several form types, e.g. order confirmation and advance delivery note.

**Sorted by** Sorting of the forms. By default, the forms are sorted by document number. The field is only activated if you have selected several form types.
- **NUMBERS:** The forms are sorted by document number.
- **FORMS:** The forms are sorted by form type.
- Technical info: toggle field

**Additional Copies** Number of additional print copies up to a maximum of 99. By default, a form is printed.
Technical info: numeric field

**(Field without name)** Specification how the documents for the form printing should be determined.
- **Enter Numbers:** In the header area of the Form Printing dialog, you can filter the documents according to various criteria. In the overview, only the documents are displayed for form printing that correspond to the filter criteria. By default, the field is pre-populated with this value.
    - ⇨ "Overview" on page D-363
- **Specify various numbers:** No documents are displayed in the overview. You create the list of documents manually.
    - ⇨ "Overview" on page D-363
- Technical info: toggle field

Confirm your entry using <Enter>.

#### Header (Select numbers)

**from, to** Start and end value of the filter criteria:
- **Employ.:** Number of the employee who entered the document. All employees with numbers between from and to will be used as filter criterion.
    - Technical info: numeric field, DB field: kauf.eust
- **Partners:** All market partners for which the document was entered. All market partners with numbers between from and to will be used as filter criterion.
    - Technical info: numeric field, DB field: kauf.kunr
- **Req. On:** Date on which the document was entered. By default, the current date is specified in the to field. How long the period between the two fields may be depends on the configuration in the master data.
    - ⇨ Stammdaten, "Periodenende" auf Seite J-214
    - Technical info: mandatory field, date field, DB field: kauf.edat
- **Docum.:**
    - Document number. All documents with numbers between from and to will be used as filter criterion.
    - Technical info: numeric field, DB field: kauf.auftrnr
- **Department:**
    - Department number. All departments with numbers between from and to will be used as filter criterion.
    - Technical info: numeric field, DB field: kauf.abtnr

**Output ... print** Specification of which documents should be listed in the overview. The system creates a print history.
- **All not output:**
    - Only documents that have not yet been printed and correspond to the filter criteria will be displayed.
- **All:**
    - All documents that correspond to the filter criteria are displayed. The displayed documents can already be printed. For documents that have already been printed, the date of printing is displayed in the printed column.
- **All new obligator.:**
    - Changed documents for which a new printout was specified as obligatory and that correspond to the filter criteria will be displayed. The selection is only possible if the system is configured appropriately. In this case, when saving a changed document, a query is displayed asking whether the document should be provided for printing. With confirmation of the query, the document is displayed under All new obligator. for form printing.
- Technical info: toggle field

Use <F3> to start the search for documents that correspond to the filter criteria.

#### Overview

Under the area for entry of the filter criteria, the documents are displayed in an overview that correspond to the filter criteria and are available for form printing. If you have selected Specify various numbers, the overview is empty and you can add documents manually. If you have selected Select numbers, all documents are displayed in the overview that correspond to the filter criteria. You can add documents manually.

- **Pc:**
    - Print code for the document.
        - Y: Print the form for the document.
        - N: Do not print the form for the document.
        - X: Lock the document for form printing.
    - Technical info: toggle field, DB field: repform.drflag
- **Docum.:**
    - Document number.
    - Technical info: mandatory field, numeric field, DB field: repform.auftrnr
- **SubNo.:**
    - Subnumber of the partial document, e.g. partial invoices or partial delivery notes.
    - Technical info: numeric field, DB field: repform.subnr
- **Partners:**
    - Matchcode of the market partner.
    - Technical info: display field, DB field: repform.kumc
- **Change:**
    - Date of the last document change.
    - Technical info: display field, DB field: repform.updat
- **Employ.:**
    - Number of the employee who entered the document.
    - Technical info: display field, DB field: kauf.eusr
- **Printed:**
    - Date on which the document was printed. If the document has not yet been printed, then the field is empty.
    - Technical info: display field, DB field: druckhist.Itzdat
- **Employ.:**
    - Number of the employee who last printed the form for this document.
    - Technical info: display field, DB field: druckhist.Itzmanr
- **Route:**
    - Route number.
    - Technical info: display field, DB field: repform.routenr
- **Date:**
    - Delivery date to the customer.
    - Technical info: display field, DB field: repform.liefdat

Open the following column using <F2>:
- **Market part.:**
    - Markt partner number.
    - Technical info: display field, DB field: repform.kunr
- **Fax:**
    - Fax number of the market partner for the document.
    - Technical info: alphanumeric field, DB field: repform.faxnr

Use <Shift>+<F3> to start the printing.
- ⇨ "Print on" on page D-367

### E-mail

**Sales > Forms > E-Mail/Fax**

*Fig. D-154 E-mail*

Use these dialogs to select a document for sending forms by e-mail or fax. So that forms can be sent via e-mail, the system has to be configured appropriately.

**Form Type** Specification of the form type that you want to send via e-mail or fax. The selected form type is displayed on the E-mail dialog in the top left corner.
Technical info: mandatory field, numeric field, DB field: rep.formart

**Select Case by** Specification of which documents should be displayed.
- **Enter Numbers:**
    - In the header area of the E-mail dialog, you can filter the documents according to various criteria. In the overview, only the documents are displayed for form printing that correspond to the filter criteria.
    - ⇨ "Overview" on page D-363
- **Specify various numbers:**
    - No documents are displayed in the overview. You create the list of documents manually.
    - ⇨ "Overview" on page D-363
    - Technical info: toggle field

Confirm your entry using <Enter>.

You can only send forms to a market partner by e-mail or fax if the e-mail address and fax number are stored in the master data for this market partner. By default, this address or number is used on the E-mail dialog if you call up a document.

In the document entry, on the Addresses tab you can store an e-mail address and fax number that differ from the details in the master data. If on the E-mail dialog you call up a document with a different e-mail address or fax number, a message is displayed asking whether the different address or number from the document should be used.

#### Header (Select numbers)

The header area is described for the Form Printing dialog:
- ⇨ "Form Printing" on page D-361

#### Header (specify various numbers)

The header area is described for the Form Printing dialog:
- ⇨ "Form Printing" on page D-361

#### Overview

The columns are described for the Form Printing dialog:
- ⇨ "Form Printing" on page D-361

In addition, the following columns are displayed:
- **E-Mail:**
    - E-mail address to which the form is sent. The e-mail address is drawn from the master data or the document.
    - Technical info: mandatory field, alphanumeric field
- **sent:**
    - Display of the date on which the document was sent.
    - Technical info: display field, DB field: druckhist.Itzdat

### Print on

**Sales > Forms > Print > Select form > <End> > Enter data and select > <Shift> + <F3>**

*Fig. D-155 Print on*

On this dialog, you select the printer. In addition to a physical printer, you can output the form as file.

The footer indicates which form type is printed.

**Select Printer** Number and description of the printer for printing. Use <F9> to open the list of the printers available.
Technical info: mandatory field, numeric field, DB field: repdruck.drunr

**File name** You must specify a file name for file print. This field is only shown if you select file print in the Select printer field. The output type of the printers is stored in the system settings in the print management.
Technical info: mandatory field, alphanumeric field

### List Printing

**Sales > List printing > Select list**

*Fig. D-156 List Printing*

Use this dialog to print out lists, e.g. the list of all orders received from particular representatives within a particular period.

First you select the list that you want to print. On the List Printing dialog you can then filter the list according to particular criteria.

**List name** Name of the list that should be printed.
Technical info: mandatory field, selection field

If you have selected a list, various fields are displayed with which you can restrict the entries in the list.
The display of the fields depends on the list selected and the SQL query in question.

If you have filled out the field, start list printing with <F3>.
- ⇨ "Print on" on page D-367

## Order Status

For all orders, you can display the document information, e.g. the status changes.

### Order Information

**Sales > Overview > Order Information > Enter order number**

This dialog displays the processing status of the selected order.

This dialog contains the following tabs:
- "Document Info – Order" on page D-370
- "Document Info – Items" on page D-371
- "Document Info – Purchasing" on page D-372
- "Document Info – Goods Received" on page D-374
- "Document Info – Production" on page D-375
- "Document Info – Dispatch" on page D-377
- "Document Info – Barcoding" on page D-378
- "Document Info – Racks" on page D-380
- "Document Info – Stock" on page D-381
- "Document Info – Linked Production" on page D-382
- "Document Info - Intermediate Disp." on page D-383

You can also open this dialog via order entry for the current order:
**Sales > Order Entry > Header, Footer area, Item level > <Shift> + <F10>**

### Document Info – Order

**Sales > Overview > Order Information > Enter order number > Document tab**

*Fig. D-157 Order information - Order tab*

This tab displays the history of the processing status of the selected document.

#### Order tab

- **Date:**
    - Date of the status booking.
    - Technical info: display field, DB field: kaufstat.datum
- **Activity:**
    - Description of the document status. The information displayed is drawn from the system. Depending on the processing status of the document, the data is drawn from A+W Enterprise or from another program, e.g. from A+W Production.
    - If you are working with internal site separation, the processing status per site is displayed.
    - Technical info: display field

#### Footer

- **Prod. Report**
    - Branches to a production report for the selected order if this exists and the system is configured appropriately. The production report opens in a browser window.
- **Int. Order**
    - Branches to an internal order with individual order number for production if this exists and the system is configured appropriately. The internal orders can only be generated if the environment variable VORGANGSSTATUS_ADHOCSQL is active and you have incorporated an ad hoc SQL query. If the variable is not set, an appropriate error message is displayed.

### Document Info - Items

**Sales > Overview > Order Information > Enter order number > Items tab**

*Fig. D-158 Order information - Items tab*

The PO and order details for the items are displayed on this tab.

If the item status changes, the status of the appropriate item is displayed on the right of the dialog on the item level, e.g. packed, FIXED, local correction. Each item can have a different status. The item status displayed applies for the marked item.
- ⇨ "Explanation of Symbols" on page D-79

For additional information about the various status indicators, contact your A+W Software GmbH contact person.

#### Items tab

- **Itm:**
    - Item number.
    - Technical info: display field, DB field: kpos.posnr
- **Article:**
    - Article number.
    - Technical info: display field, DB field: kpos.artnr
- **Qty:**
    - Quantity in the article quantity of the article ordered.
    - Technical info: display field, DB field: kpos.menge
- **Receipt:**
    - Quantity in the article quantity unit of the articles ordered, which are already booked as incoming goods.
    - Technical info: display field, DB field: kpos.geslief
- **Available:**
    - Quantity in the article quantity unit of the article reported complete in production that can be delivered.
    - Technical info: display field, DB field: lapool.gefstk
- **Packed:**
    - Quantity in the article quantity unit of the packed articles that are already ready to ship.
    - Technical info: display field, DB field: kpos.gespack
- **Deliv:**
    - Quantity in the article quantity unit of the articles that were already delivered.
    - Technical info: display field, DB field: kpos.geslief
- **Chargd:**
    - Quantity in the article quantity unit of the articles that have already been invoiced.
    - Technical info: display field, DB field: kpos.gesberech

#### Footer

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Document tab:
- ⇨ "Document Info - Order" on page D-370

In addition, the following button is displayed:
- **Info**
    - Displays the error message from production for the selected item. The button is only active if there is an error message for the selected item.

### Document Info – Purchasing

**Sales > Overview > Order Information > Enter order number > Purchasing tab**

*Fig. D-159 Order information – Purchasing tab*

This tab displays information about the status of purchased parts.

> **Two fields for item numbers**
> This tab displays two Itm fields. They differ from one another and display different item numbers.

#### Purchasing tab

The columns are described for the Items tab:
- ⇨ "Document Info - Items" on page D-371

In addition, the following columns are displayed:

- **Article:**
    - Article number and description of the purchased part. The number is drawn from the BOM.
    - Technical info: display field, DB field: aufstrukt.artnr
- **Description:**
    - Description of the purchased part.
    - Technical info: display field, DB field: artikel.artbez1
- **PO no:**
    - Order number of purchased part. The number of the PO is saved in the database field kauf.auftrnr for vorgang = 2.
    - Technical info: display field, DB field: kauf.auftrnr
- **Itm (field between PO no and Ordered):**
    - Item number of the article for which the articles are ordered.
    - Technical info: display field, DB field: aufstrukt.posnr
- **Ordered:**
    - Quantity of the article ordered.
    - Technical info: display field, DB field: kpos.menge
- **Received:**
    - Quantity of the articles received in incoming goods.
    - Technical info: display field, DB field: kpos.geslief
- **Ordered for:**
    - Requested delivery date of the article ordered.
    - Technical info: display field, DB field: kauf.ltplan
- **PU Price:**
    - Net unit price of the article ordered.
    - Technical info: display field, DB field: kpos.nstpreis
- **Compl:**
    - Item is complete if an asterisk * is displayed.
    - Technical info: display field, DB field: kposp.liefkompl
- **DPI:**
    - Delivery plan. Specification whether a delivery plan for the item exists.
        - D: There is a delivery plan for the item.
        - (blank): There is no delivery plan.
    - Technical info: display field

#### Footer

The name of the supplier for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
- ⇨ "Document Info - Items" on page D-371

### Document Info – Goods Received

**Sales > Overview > Order Information > Enter order number > Goods Received tab**

*Fig. D-160 Order information - Goods received tab*

This tab displays information about the status of goods received for purchased parts.

> **Two fields for item numbers**
> This tab displays two Itm fields. Column 1 displays the number of the order item and column 5 for purchased articles the number of the order item.

#### Goods Received tab

The columns are described for the Items tab:
- ⇨ "Document Info – Items" on page D-371

In addition, the following columns are displayed:

- **P.O.:**
    - Order number for the purchased parts.
    - Technical info: display field, DB field: kauf.auftrnr
- **Itm (column 5 between P.O. and Delivery):**
    - Item number of the article ordered in the PO.
    - Technical Info: display field, DB field: aufstrukt.posnr
- **Delivery:**
    - Order confirmation number of the supplier. The number of the order item is stored in DB field kpos.abnr.
    - Technical info: display field, DB field: bpos.abnr
- **SubNo.:**
    - Subnumber of the delivery.
    - Technical info: display field, DB field: kauf.subnr
- **Confirm.:**
    - Date of the delivery confirmation.
    - Technical info: display field, DB field: bpos.ltavis
- **Qty:**
    - Quantity of the article confirmed by the supplier in the quantity of the article ordered.
    - Technical info: display field, DB field: bpos.avismenge
- **Deliv. Date:**
    - Delivery date for the purchased parts.
    - Technical info: display field, DB field: bpol.ltplan
- **Received:**
    - Delivered quantity in the article quantity unit of the article ordered that has been booked in incoming goods.
    - Technical info: display field, DB field: kpos.geliefert
- **DPI:**
    - Delivery plan.
    - Specification whether a delivery plan for the item exists.
        - D: There is a delivery plan for the item.
        - (blank): There is no delivery plan.
    - Technical info: display field

#### Footer

The description of the article and the name of the supplier for the selected item are displayed at the lower left of the dialog.

The buttons are described for the Items tab:
- ⇨ "Document Info – Items" on page D-371

### Document Info – Production

**Sales > Overview > Order Information > Enter order number > Production tab**

*Fig. D-161 Order information - Production tab*

This tab displays the order status from the production system.

#### Production tab

The columns are described for the Items tab:
- ⇨ "Document Info - Items" on page D-371

In addition, the following columns are displayed:

- **Status:**
    - Number of the production status.
    - Technical info: display field, DB field: kposstat.status
- **Information text:**
    - Description of the production status. The text is pre-populated by the system and displayed in the configured system language.
    - Technical info: display field, DB field: kposstat.infotxt
- **date:**
    - Date of the reporting of the status displayed.
    - Technical info: display field, DB field: kposstat.datum
- **Time:**
    - Time of the reporting of the status displayed.
    - Technical info: display field, DB field: kposstat.zeit
- **Qty.:**
    - Quantity from the report in article quantity unit.
    - Technical info: display field, DB field: kpos.menge

#### Footer

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
- ⇨ "Document Info – Items" on page D-371

### Document Info – Dispatch

**Sales > Overview > Order Information > Enter order number > Dispatch tab**

*Fig. D-162 Order information – Dispatch tab*

This tab displays information about the status of dispatch.

#### Dispatch tab

The columns are described for the Items tab:
- ⇨ "Document Info - Items" on page D-371

In addition, the following columns are displayed:

- **Sta:**
    - Traffic light display of the current item status.
    - Technical info: display field
    - ⇨ "Explanation of Symbols" on page D-79
- **Site:**
    - Site number in which the order is created.
    - Technical info: display field, DB field: kauf.hausnr
- **Route:**
    - Number of the shipping route.
    - Technical info: display field, DB field: kauf.route
- **Delivery date:**
    - Date of the delivery.
    - Technical info: display field, DB field: kauf.ltplan
- **Call:**
    - Units of the article that the customer calls at the delivery date.
    - Technical info: display field, DB field: lapool.abrufstk
- **Sched.:**
    - Units of the article that are scheduled for the delivery date.
    - Technical info: display field, DB field: lapool.sollstk
- **Available:**
    - Quantity in the article quantity unit of the article reported complete in production that can be delivered.
    - Technical info: display field, DB field: kpos.gefstk
- **Packed:**
    - Quantity in the article quantity unit of the packed articles that are already ready to ship.
    - Technical info: display field, DB field: lapool.iststk
- **Dispatch:**
    - Dispatch type:
        - **Exit:** goods are being sent.
        - **Inbound:** goods will be received, e.g. after processing by a different site.
    - Technical info: display field, DB field: kposstat.status

#### Footer

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
- ⇨ "Document Info - Items" on page D-371

### Document Info - Barcoding

**Sales > Overview > Order Information > Enter order number > Barcoding tab**

*Fig. D-163 Order information – Barcoding tab*

This tab displays the information about the barcoding status if you are working with plant data collection.

Use <F5> to change the view of the tab. The values are then displayed summarized by item and machine number.

#### Barcoding tab

The columns are described for the Items tab:
- ⇨ "Document Info – Items" on page D-371

In addition, the following columns are displayed:
- **MaNo:**
    - Machine number.
    - Technical info: display field
- **Date:**
    - Completion date.
    - Technical info: display field
- **Shift:**
    - Number of the shift in the case of multiple-shift operation.
    - Technical info: display field
- **JobNo:**
    - Sequential number of the job.
    - Technical info: display field
- **Label:**
    - Number of the label for printing.
    - Technical info: display field
- **Targ. Qt:**
    - Quantity of the article that should be produced.
    - Technical info: display field
- **ActQty:**
    - Quantity of the article that has already been produced.
    - Technical info: display field
- **Rejct:**
    - Quantity of articles that have broken.
    - Technical info: display field

#### Footer

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
- ⇨ "Document Info - Items" on page D-371

### Document Info - Racks

**Sales > Overview > Order Information > Enter order number > Racks tab**

*Fig. D-164 Order information - Racks tab*

This tab displays information from the packing planning per rack.
A line is displayed per rack, whereby it is possible that several items can be packed on a rack or an item can be distributed across several racks.

#### Racks tab

The columns are described for the Items tab:
- ⇨ "Document Info – Items" on page D-371

In addition, the following columns are displayed:

- **Rack:**
    - Number of the rack on which the articles are planned. The number is assigned automatically by the system.
    - Technical info: display field, DB field: kposgest.vsgnr
- **External Number:**
    - External PO number of the customer. For orders from another site, the order number of the sending site is in this field.
    - Technical info: display field, DB field: gestellz.exgnr
- **SerNo:**
    - Item number from the order.
    - Technical info: display field, DB field: kpos.Ifdpos
- **Deliv. Date:**
    - Date of the delivery for the rack.
    - Technical info: display field, DB field: vsaufgest.Itplan
- **Route:**
    - Number of the route on which the rack is transported.
    - Technical info: display field, DB field: vsaufgest.routennr
- **ActQty:**
    - Quantity of articles that are planned on the rack.
    - Technical info: display field, DB field: lapool.iststk

#### Footer

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
- ⇨ "Document Info - Items" on page D-371

### Document Info - Stock

**Sales > Overview > Order Information > Enter order number > Stock tab**

*Fig. D-165 Order information - Stock tab*

This tab displays the status information about the stock article that is entered in the order.

#### Stock tab

The columns are described for the Items tab:
- ⇨ "Document Info - Items" on page D-371

In addition, the following columns are displayed:

- **Stocktyp:**
    - Number of the stock article. The stock articles are subparts of item articles for which stock items have to be entered.
    - Technical info: display field, DB field: auftrukt.artnr
- **Stock:**
    - Number of the stock from which the article is removed.
    - Technical info: display field, DB field: bpos.nr
- **Variant:**
    - Variant of the stock article from the article master.
    - Technical info: display field, DB field: artvarzu.bitnr
- **Pieces:**
    - Quantity in the article quantity unit that is required for the item.
    - Technical info: display field
- **Booked:**
    - Quantity of stock articles that are booked.
    - Technical info: display field
- **Status:**
    - Stock status:
        - No booking yet
        - Partial booking
        - Booked
    - Technical info: display field, DB field: kposstat.status

#### Footer

Additional article information on the selected item.

The buttons are described for the Items tab:
- ⇨ "Document Info – Items" on page D-371

### Document Info – Linked Production

**Sales > Overview > Order Information > Enter order number > Linked Production tab.**

*Fig. D-166 Document info – Linked Production tab*

This tab displays the status information from the linked production if you are working with internal site separation.

For additional information about this area, contact your A+W Software GmbH contact person.

#### Linked Production tab

The tab is structured the same way as the Production tab:
- ⇨ "Document Info – Production" on page D-375

#### Footer

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
- ⇨ "Document Info - Items" on page D-371

### Document Info – Intermediate Disp.

**Sales > Overview > Order Information > Enter order number > Intermediate Disp. tab**

*Fig. D-167 Document info – Intermediate Disp. tab*

This tab displays information about the status of articles from the extended workbench.

#### Intermediate Disp. tab

The tab is structured the same way as the Production tab:
- ⇨ "Document Info - Production" on page D-375

## Document Research

To search for documents, there is a search with extensive search criteria available.

The following dialogs are described in this section:
- "Search Document" on page D-384
- "Items" on page D-396

### Search Document

**Sales > Overview > Search Document**

Use this dialog to search for documents. The results are displayed in a hit list.

This dialog contains the following tabs:
- "Search Document – search mode” on page D-384
- "Search Document – Overview" on page D-388
- "Search document – Employees" on page D-390
- "Search Document – Details" on page D-391
- "Search Document - Document Change Log" on page D-394

You can also open this dialog via the Info menu with <Shift>+<F4> in the header area of the order entry.

### Search Document – search mode

**Sales > Overview > Search Document**

*Fig. D-168 Search Document - search mode*

Use this dialog to restrict the search with the specified criteria. You specify the criteria with conditions. The more criteria you specify for the search, the more you restrict the search.

Use <Shift>+<F8> or <Shift>+<F12> to change the condition. The info line displays the meaning of the selected condition.

| Condition | Meaning |
| :--- | :--- |
| = | Search exactly for this value (e.g. market partner field = 600004 lists only documents relating to this market partner). |
| > | Search for larger values (e.g. market partner field > 600004 lists only documents with market partner numbers larger than 600004). |
| p | Search for patterns in text fields (e.g. Reference field Shape 12 lists all documents with the reference text model 12.) |
| 0 | Search for values = 0 (e.g. market partner field 0 lists only market partners with the number 0). |
| Z | Search all values in the range. |
| ! | Search all values except for this value (e.g. Department field! 10 lists all departments except for the department with the number 10). |
| < | Search for smaller values (e.g. market partner field < 600004 lists only documents with market partner numbers smaller than 600004). |

*Tab. D-13 Meaning of the filter conditions*

**Site No.** Site number and description of the site. If you specify a number, the description of the site is displayed in plain text.
Technical info: numeric field, display field, DB fields: kauf.hausnr

**Company** Number of the company to which the site is assigned. The field is only enabled if you are working with internal site separation.
Technical info: display field, DB field: kauf.company

**Document** Document type. If you select a document type, the code number of the document type is displayed in plain text.
- Inquiries
- Purchase orders
- Receipt of goods.
- Quotations
- Orders
- Delivery notes
- Invoices
- PU invoice
- Credit notes
- PU credit
- SA cancellations (sales documents that were canceled)
- PU cancellations (purchasing documents that were canceled)
- Changes (documents that were changed)
- The Document Change Log dialog opens.
    - ⇨ "Search Document - Document Change Log" on page D-394
- Technical info: toggle field, display field, DB field: kauf.vorgang

**Doc. Date** Entry date of the document in the format DD.MM.YYYY.
Technical info: date field, DB field: kauf.edat

**Market Partner** Market partner number and description. If you specify a number, the description of the market partner is displayed in plain text. The match code of the market partner is assigned to a market partner type.
Technical info: numeric field, display field, DB fields: kauf.kunr, mp.name

**(Matchcode)** Market partner type. In Sales, Customer is pre-populated as market partner type. If you select a market partner, the market partner's match code is displayed automatically next to the field.
Technical info: toggle field, DB field: mp.mpmc

**STDDE** Customer purchase order number.
Technical info: alphanumeric field, DB field: kauf.exaufnr

**External Ref.** Reference text.
Technical info: alphanumeric field, DB field: komm.kommtxt

**Project** Project number and description of the project, e.g. construction site. If you specify a number, the description of the project is displayed in plain text.
Technical info: numeric field, display field, DB fields: kauf.objnr, mp.name

**Number** Document number.
Technical info: numeric field, DB field: kauf.auftrnr

**SubNo** Subnumber, e.g. partial delivery note.
Technical info: numeric field, DB field: kauf.subnr

**Departm.** Number and name of the department of the person entering the document. If you specify a number, the name of the department is displayed in plain text.
Technical info: numeric field, display field, DB field: kauf.abtnr

**Invoice** Invoice number. The number is saved in the database table vorgang with the value 7.
Technical info: numeric field, DB field: kauf.auftrnr

**Sales Repr.** Number and name of the representative. If you specify a number, the name of the representative is displayed in plain text.
Technical info: numeric field, display field, DB field: kauf.vertrerloe

**Ordered** PO date in the format DD.MM.YYYY.
Technical info: date field, DB field: kauf.bdat

**Route** Number and description of the route. If you specify a number, the description of the route is displayed in plain text.
Technical info: numeric field, display field, DB field: kauf.routenr

**Deliv. Date** Planned delivery date in the format DD.MM.YYYY.
Technical info: date field, DB field: kauf.ltplan

**Entered** Number and name of the person entering the document. If you specify a number, the name of the person entering the document is displayed in plain text.
Technical info: numeric field, display field, DB field: kauf.eusr, mitarb.maname

**Suspended** Indication whether the document is suspended. The identifier and code number are set automatically if you select a document.
- **n:**
    - The document is not suspended. The code number 0 is displayed. By default, the field is pre-populated with the identifier n.
- **y:**
    - The document is suspended. The code number 1 is displayed. The identifier is set if in the Document field you have selected the document type SA cancellations or PU cancellations.
- Technical info: toggle field, display field, DB field: kauf.storno

#### Footer

**Start** Start search for documents with the specified criteria.

### Search Document – Overview

**Sales > Overview > Search Document > Enter search criteria > <F3> > Overview tab**

*Fig. D-169 Search Document - Overview*

This tab displays the hit list of documents matching the search criteria.

#### Header

The fields in the header area only provide information. You cannot edit the entries.

**Market Partner** Number, matchcode, and name of the market partner.
Technical info: display fields, DB fields: mp.kuliflag, mp.mpnr, mp.mpmc

**Address** Street address of the market partner.
Technical info: display field, DB field: mp.str

**PCd.City** Postal code and city of the market partner.
Technical info: display fields, DB fields: mp.plz, mp.ort

**Phone** Telephone number of the market partner.
Technical info: display field, DB field: mp.telefon

**Fax** Fax number of the market partner.
Technical info: display field, DB field: mp.faxnr

**Evaluation** Number of the evaluation of the quality of the market partner. The evaluation is created in the market partner master data.
Technical info: display field, DB field: mp.qqual

> **Store evaluation in the master data**
> Store evaluations under the following path: Master data > Market partner > Select market partner > Evaluation tab > Quality field.

#### Overview tab

- **Docum.:**
    - Document number.
    - Technical info: display field, DB field: kauf.auftrnr
- **SubNo:**
    - Number of the partial delivery note or partial invoice.
    - Technical info: display field, DB field: kauf.subnr
- **Site:**
    - Site number.
    - Technical info: display field, DB field: kauf.hausnr
- **Tpe:**
    - Type of document, e.g. order.
    - Technical info: display field, DB field: kauf.vorgang
- **Del. Date:**
    - Delivery date.
    - Technical info: display field, DB field: kauf.ltplan
- **Disc.**
    - Percentage of discount granted on the total amount.
    - Technical info: display field, DB field: kauf.gesfaktor
- **Reduct.:**
    - Percentage of reduction granted on the total amount.
    - Technical info: display field, DB field: kauf.gesfaktor
- **Net:**
    - Net amount of the item.
    - Technical info: display field, DB field: kauf.nettototal
- **Span:**
    - Profit margin of the item in currency units.
    - Technical info: display field, DB field: kauf.dbdm
- **%:**
    - Percentage of price margin of the item in currency units.
    - Technical info: display field, DB field: kauf.dbvh

#### Footer

For the values Net and Margin, the totals of the values of all items are listed. For % (percentage of price margin), the average value of the items is listed.

### Search document – Employees

**Sales > Overview > Search Document > Enter search criteria > <F3> > Employee tab**

*Fig. D-170 Search Document – Employee*

This tab displays the employee information about the employee's documents.

#### Header

The fields are described on the Overview tab.
- ⇨ "Search Document - Overview" on page D-388

#### Employee tab

Some columns are described for the Overview tab:
- ⇨ "Search Document - Overview" on page D-388

In addition, the following columns are displayed:

- **SiteNo:**
    - Site number.
    - Technical info: display field, DB field: kauf.hausnr
- **MktPt:**
    - Number of the market partner.
    - Technical info: display field, DB field: kauf.kunr
- **Ent'rd:** Date of the document entry.
    - Technical info: display field, DB field: kauf.edat
- **Sales Rep:**
    - Number of the sales representative.
    - Technical info: display field, DB field: kauf.vertrerloe
- **Operator:**
    - Name of the operator.
    - Technical info: display field, DB field: kauf.abvertr
- **Route, Route Name:**
    - Number and description of the shipping route.
    - Technical info: display field, DB field: kauf.routenr

### Search Document – Details

**Sales > Overview > Search Document > Enter search criteria > <F3> > Details tab**

*Fig. D-171 Search Document - Details*

Use this tab to display the details for the selected document.
Use <Page Down> to change to the next document, <Page Up> to the previous document.

#### Header

The fields are described on the Overview tab.
- ⇨ "Search Document - Overview" on page D-388

#### Details tab

**Document** Number and subnumber of the document.
Technical info: numeric field, display field, DB fields: kauf.auftrnr, kauf.subnr

**Act.Ref.No** Number of the original document for transferred documents. The site number of the sender is in the first field; the second number contains the original document number.
Technical info: display fields, DB fields: kauf._orgauftrnr

**Prev.Ref.No.** Previous document number for transferred documents, e.g. the reference number for the original document.
Technical info: display fields, DB field: kauf.referenz

**Market Partner** Number and name of the market partner.
Technical info: display field, DB field: kauf.kunr, mp.name

**Delivery Date** Delivery date.
Technical info: display field, DB field: kauf.Itplan

**Invoice** Invoice number pertaining to the document.
Technical info: display field, DB field: kauf.rechnr

**Cust. PO No.** External PO number for the customer. For orders from another site, the order number of the sending house is displayed in this field.
Technical info: display field, DB field: kauf.exaufnr

**P.O. Date** Date of the P.O.
Technical info: display field, DB field: kauf.edat

**Proj.** Number and description of the project. A project can be a construction site or delivery address, for example.
Technical info: display fields, DB fields: kauf.objnr, kauf.orgname

**Departm.** Number and name of the department in which the order has been entered.
Technical info: display fields, DB field: kauf.abtnr

**Total Sqft** Total glass area of the document in square meters.
Technical info: display field, DB field: kauf.gesm2

**Tot. Pieces** Total number of pieces of units from all items of the order.
Technical info: display field, DB field: kauf.gesst

**Disc.** Discount granted for the total amount in percent and as amount.
Technical info: display fields, DB fields: kauf.gesfaktor

**Net Total** Total of all item prices, minus the discounts and plus the surcharges.
Technical info: display field, DB field: kauf.nettototal

**Margin** Profit margin of the document in percent and in currency units.
Technical info: display fields, DB fields: kauf.dbvh, kauf.dbdm

**Pay. Term** Term of payment and cash discount deductions that have been agreed upon with the market partner.
Technical info: display field, DB field: kauf.zahlziel

**Val.Date** Period until the value date in days.
Technical info: display field, DB field: kauf.valuta

**Cash D. 1, 2, %** Period (number of days) during which a cash discount is applicable. The second field (%) reflects the percentage for the cash discount. The fields are preset with the market partner data.
Technical info: display fields, DB fields: kauf._skonto1, kauf.skvh1, kauf._skonto2, kauf.skvh2

**Ent'rd on, by** Date of the document entry, number and name of the person who entered it.
Technical info: display fields, DB fields, kauf.edat, kauf.eusr

**Receipt** Type of communication of the document entry, e.g. fax.
Technical info: display field, DB field: kauf.eingang
- ⇨ "Receipt" on page D-88

### Search Document – Document Change Log

**Sales > Overview > Search Document > Document field > Define the value to be changed as search criteria > <Enter>**

*Fig. D-172 Search Document – Document Change Log*

Use this dialog to display a log of document changes.

> **Automatic display of the dialog**
> The Document Change Log dialog is displayed automatically if you specify Change as search criterion in the Document field and change to the next field.

You can restrict the display of the document changes by date and document type. After entering the search criteria, the log is displayed in a view.
- Use <Enter> to display the log of the document changes.

#### Log search

**Document** Type of document.
- All
- Inquiries
- Purchase orders
- Receipt of goods
- Quotations
- Orders
- Delivery notes
- Invoices
- PU invoices
- Credit notes
- PU credits
- Technical info: toggle field, DB field: kauf.vorgang

**from Date** Display of document changes starting on this date. The format is DD.MM.YYYY. By default, the current date is pre-set.
Technical info: date field

**to Date** Display of document changes up to this date. The format is DD.MM.YYYY. By default, the current date is pre-set.
Technical info: date field

#### Log display

In the view, you can see a log of the document changes that correspond to the search criteria. The log cannot be edited.

- **Document:**
    - Document number.
    - Technical info: display field, DB field: kaufedit.auftrnr
- **(Column without name):**
    - Subnumber of the document.
    - Technical info: display field, DB field: kaufedit.subnr
- **Document:**
    - Document type.
    - Technical info: display field, DB field: kaufedit.vorgang
- **Chgd:**
    - Date on which the document was changed.
    - Technical info: display field, DB field: kaufedit.datum
- **Time:**
    - Time at which the document was changed.
    - Technical info: display field, DB field: kaufedit.zeit
- **Change type:**
    - Type of change.
    - Technical info: display field, DB field: kaufedit.modus
- **Employ:**
    - Number of the employee who changed the document.
    - Technical info: display field, DB field: kaufedit.manr
- **Name:**
    - Name of the employee who changed the document.
    - Technical info: display field, DB field: mitarb.maname

### Items

**Sales > Overview > Search Document > Enter search criteria > <F3> > Select document > <Shift> + <F9>**

Use this dialog to display the information about the items of the selected document.

This dialog contains the following tabs:
- "Items - Overview" on page D-396
- "Items - Details" on page D-398

### Items - Overview

**Sales > Overview > Search Document > Enter search criteria > [Start] > Select tab > Select document > <Shift> + <F9> >Overview tab**

*Fig. D-173 Items - Overview*

The items for the order are displayed on this tab.

- **Itm:**
    - Item number.
    - Technical info: display field, DB field: kpos.posnr
- **Article:**
    - Article number.
    - Technical info: display field, DB field: kpos.artnr
- **(Column without name):**
    - Description of the article.
    - Technical info: display field, DB field: kpos.artbez1
- **Qty:**
    - Units of the item.
    - Technical info: display field, DB field: kpos.geliefert
- **Net Pr/Pc:**
    - Net price per piece for the item.
    - Technical info: display field, DB field: kpos.nstpreis
- **Margin:**
    - Margin between the sales price and purchase price.
    - Technical info: display field, DB field: kpos.spanne
- **Chg:**
    - Indicator whether the item was changed
    - Technical info: display field, DB field: kpos.poskoaendkz
- **Mat. costs:**
    - Material costs of the item from the master data if working with cost calculation. Material costs can be, for example, purchase prices or the material value including waste (if the material is taken from stock).
    - Technical info: display field, DB field: kposp.komat
- **Labor Cost:**
    - Labor costs for the production / processing of the item. Is calculated in A+W Production and reported.
    - Technical info: display field, DB field: kposp.kolohn
- **Mach. costs:**
    - Machine costs for the production / processing of the item. Is calculated in A+W Production and reported.
    - Technical info: display field, DB field: kposp.kobm

#### Footer

The footer displays the type and number of the selected document.

### Items - Details

**Sales > Overview > Search Document > Enter search criteria > [Start] > Select tab > Select document > <Shift> + <F9> > Details tab**

*Fig. D-174 Items - Details*

Details about the items for the order are displayed on this tab.

**Item** Number of the item.
Technical info: numeric field, DB field: kpos.Ifdpos

**Article** Number and description of the article.
Technical info: display field, DB field: kpos.artnr

**Shape** Shape number of the article.
Technical info: display field, DB field: kpos.modnr

**Prod. Group** Indicator of the product group allocated to the article.
Technical info: display field, DB field: kpos.wagrp

**Supplier** Supplier number.
Technical info: display field, DB field: kpos.liefnr

**Quantity** Item quantity.
Technical info: display field, DB field: kpos.menge

**Dims.** Width, height and airspace of this item in millimeters and total surface in square meters.
Technical info: display fields: DB fields: kpos.laenge, kpos.breite, kpos.szr, kpos.qm

#### SalesPrc, PU Price

**Net** Net final amount of the item.
Technical info: display fields, DB fields: kpos.nstpreis, kpos.eknstpreis

**Gross** Gross amount of the item.
Technical info: display fields, DB fields: kpos.bstpreis, kpos.ekbstpreis

**Factor** Calculation factor of the item.
Technical info: display fields, DB fields: kpos.vorvfaktor, kpos.ekfaktor

**PCD** Price code from the price list.
Technical info: display fields, DB fields: kpos.vorvkpkz, kpos.ekpkz

**Disc.** Percentage of price discount for the item. The field is only displayed for the sales price.
Technical info: display field, DB field: kpos.rabatt

**Reduct.** Percentage of reduction for the item. The field is only displayed for the sales price.
Technical info: display field, DB field: kpos.gesfaktor

#### Costs

**Mat. Costs** Material costs of the item, e.g. the material value including waste.
Technical info: display field, DB field: kposp.komat

**Labor Cost** Labor costs of the item.
Technical info: display field, DB field: kposp.kolohn

**Mach. Costs** Machine costs calculated from the life and cost rate of the equipment.
Technical info: display field, DB field: kposp.kobm

**Proc.** Monetary value of sales.
Technical info: display field, DB field: kpos.erloes

**Margin** Margin between the sales price and purchase price.
Technical info: display field, DB field: kpos.spanne

#### Footer

The footer displays the type and number of the selected document.

## Overviews of Documents

There are various dialogs available in order to inform you about the state of documents. The dialogs display overviews of data that is determined from the documents.

The following dialogs are described in this section:
- "Order Display" on page D-400
- "Quotation Display" on page D-401
- "Resubmission" on page D-402
- "Document Change" on page D-405
- "Overview of Documents" on page D-408

### Order Display

**Sales > Overview > Order Display**

*Fig. D-175 Order Display*

On this dialog you open an order in display mode. You can open an order in display mode at any time, e.g. even if the order is locked by a background process or is being edited by another user.
