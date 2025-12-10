---
title: "EN-UM-AWEnterprise_15"
source: "EN-UM-AWEnterprise_15.pdf"
tags: ["A+W Enterprise", "Software Reference", "Sales Module", "Invoicing", "Order Management", "Credit Notes", "ERP", "Document Management", "Technical Manual", "Help Cards"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical software reference guide for the A+W Enterprise Sales module. It details functionalities for managing invoices, credit notes, forms, and order statuses, including manual and automatic processing, document booking, and printing. The guide also includes a 'Help Cards' section with step-by-step workflows for common tasks like creating quotations and orders."
long_description: "This document is a comprehensive software reference manual for the A+W Enterprise Sales module. It provides detailed descriptions of various features and dialogs, aimed at users and system administrators. The manual is divided into several key sections. The 'Invoices' section covers the creation, booking, and management of manual, partial, and final invoices, as well as cash transactions. The 'Credit Notes' section explains how to enter and book credit notes. The 'Forms' section details procedures for direct printing, form printing, and sending documents via e-mail. The 'Order Status' section offers an in-depth look at tracking order information through various stages, including purchasing, production, dispatch, and barcoding. Each feature description includes technical information such as database fields and table names. Additionally, the document contains a 'Help Cards' section, which serves as a quick-start guide, providing step-by-step, workflow-based instructions for common sales processes like creating quotations, entering orders with references, changing shipping details, and managing order items. This practical guide is designed to help users efficiently navigate and utilize the A+W Enterprise Sales software."
---

# Software Reference

---
## Invoices

- **Qty:**
  - Units of the item.
  - Technical info: numerical field, DB field: kpos.menge
- **Width:**
  - Width of the lite entered in the item in millimeters.
  - Technical info: numerical field, database field: kpos.laenge
- **Height:**
  - Height of the lite entered in the item in millimeters.
  - Technical info: numerical field, database field: kpos.breite
- **Price/pc.:**
  - Price per piece of the item.
  - Technical info: numeric field, DB field: kpos.nstpreis
- **Item price:**
  - Price of the complete item.
  - Technical info: numeric field, DB field: kpos.npospreis

Use `<F2>` to change to the Item Info II tab.

### Item info II tab

The columns are described for the *Item Info I* tab:
⇨ "Item info I tab" on page D-1400

In addition, the following columns are displayed:

- **Shp:**
  - Shape number for the item article.
  - Technical info: numeric field, DB field: kpos.modnr
- **Deliv.:**
  - Number of units that have already been delivered.
  - Technical info: numeric field, DB field: kpos.geslief
- **(Field without description):**
  - Indication of whether the item is invoiced.
  - Technical info: display field, DB field: kauf.fakturakz
- **Invoiced:**
  - Number of units that were already invoiced.
  - Technical info: numeric field, DB field: kpos.gesberech
- **AIR1, AIR2:**
  - Width of the airspace in millimeters. For multiple-lite insulated glass, the first airspace is displayed in AIR1 and the second in AIR2.
  - Technical info: numeric fields, DB fields: kpos.szr, kpos.szr2

### Invoices (manual)

**Sales > Invoices > Manual Invoice**

*Fig. D-148 Invoices (manual)*

On this dialog, you can edit or create invoices. Then you can transfer the invoices to the FinAc if the system is configured appropriately.

If you would like to create a manual partial or final invoice, you can select it directly using the appropriate menu element. In order to create a partial invoice manually, for example, select Manual Invoice in the menu path for partial invoices.

The fields are described for the Order Entry dialog:
⇨ "Order entry" on page D-1133

In addition, the following fields are displayed:

**Header**

**Invoice no.** Invoice number. If you create an invoice, the system creates a temporary number for the invoice. After completion of invoicing, the system assigns a final invoice number. This way, the invoices are numbered sequentially. If you specify an existing invoice number, the corresponding invoice is opened.
The invoices are saved in the database table kauf under vorgang with the value 7 with their final invoice number.
Technical info: numeric field, DB field: kauf.auftrnr

> **Entering invoices with reference**
> Generally invoices are always entered with reference to a document, e.g. a delivery note or an order. You can enter the document number for which you want to issue the invoice in the Ref. field in the header area.

**General tab**

**Itm** Item quantity that should be calculated. For a manual invoice, the field is pre-populated with the value Quantity from the document by default. You can reduce the value.
Technical info: numeric field, DB field: kpos.berechnet

**Footer**

If an invoice has already been created for the reference document, then the invoice amount from all invoices already created is displayed in the Net Total field.

### Cash transaction

**Sales > Invoices > Cash Transaction**

*Fig. D-149 Cash transaction*

On this dialog, you handle cash transactions for customers who pick their goods up themselves and pay directly. For a cash transaction, you enter the order data the the invoice and delivery note are then created right away.

The fields are described for the Order Entry dialog:
⇨ "Order entry" on page D-1133

### Booking of invoices

**Sales > Invoices -> Booking of Invoices**

*Fig. D-150 Booking of invoices*

Use this dialog to book invoices that have not yet been transferred to the FinAc. Generally invoices are booked automatically after generation.

In exceptional cases, the invoice can also be booked after the fact. In the invoice entry, depending on the configuration, when generating the invoice a query can be displayed asking whether the invoice should be booked. If you respond [No] to the query, you can import this unbooked invoice on the Booking of Invoices dialog and book it after the fact.

Use `<Ctrl>+<F8>` to import the data for all invoices that are generated in the specified period.

You can use `<Ctrl>+<F5>` to change to the selected invoice and check, however only as long as it is not yet booked. If the invoice is changed and saved with this procedure, it can also be booked directly on the Invoices dialog. Confirm the corresponding query with Yes.

The footer displays the customer name and total amount from the order for which the invoice is booked.

Use `<F3>` to book the selected invoices.

**Sales invoice tab**

- **Invoice:**
  - Invoice number. If you specify a number, the appropriate values are entered in the other columns.
  - Technical info: mandatory field, numeric field
- **SubNo:**
  - Display of the subnumber for partial invoices.
  - Technical info: display field, DB field: kauf.subnr
- **External no.:**
  - Display of the document number that is specified by the customer. For orders from another site, the order number of the sending site is in this field.
  - Technical info: display field, DB field: kauf.exaufnr
- **Reference:**
  - Display of the reference document type, e.g. Order.
  - Technical info: display field, DB field: kauf.refvorgang
- **Number:**
  - Display of the reference document number.
  - Technical info: display field, DB field: kauf.auftrnr
- **Subnr:**
  - Display of the subnumber for reference partial invoices.
  - Technical info: display field, DB field: kauf.subnr
- **Doc. date:**
  - Display of the date of the invoice creation.
  - Technical info: display field, DB field: kauf.edat
- **Amount:**
  - Display of the invoice total.
  - Technical info: display field, DB field: kauf.wpreis
- **User:**
  - Display of the employee's name.
  - Technical info: display field, DB field: kauf.eusr
- **Book. date:**
  - Display of the invoice booking date. By default, the current date is entered. If you want to specify another booking date, you have to enter the new date in the field, confirm the entry, and enter the new data again. The date is only taken over into the field after the second entry.
  - Technical info: date field, DB field: kauf.bdat
- **Bk.:**
  - Specification whether the invoice should be booked.
    - [x] The invoice will be booked.
    - [ ] The invoice will not be booked.
  - Technical info: checkbox

**Information on document tab**

The Information on Document tab only appears on the Invoices (automatic) and Delivery Notes (automatic) dialogs:
⇨ "Invoices (automatic)" on page D-1397
⇨ "Delivery notes (automatic)" on page D-1391

### Partial invoice (automatic)

**Sales > Invoices > Partial Invoice > Automatic Release**

*Fig. D-151 Partial invoice (automatic)*

Use this dialog to create the partial invoices for orders using a corresponding payment plan. If there are orders for the current day for which there is a payment plan, then you can import these orders with `<Ctrl>+<F8>`. You can also enter the order numbers manually or search for orders with `<F9>`.

The footer displays the customer name and total amount from the order for which a partial invoice is being created.

Use `<F3>` to have the system generate the partial invoices for the selected orders.

- **Order:**
  - Order number.
  - Technical info: mandatory field, numeric field, DB field: kauf.auftrnr
- **Site:**
  - Display of the site number.
  - Technical info: display field, DB field: kauf.hausnr
- **Amount:**
  - Partial amount from the payment plan.
  - Technical info: numeric field, DB field: zahlplan.betrag
- **Deliv. note:**
  - Indicates if there is already a delivery note or partial invoice. If there is a delivery note, the entry exists is in this field.
  - Technical info: display field
- **Date:**
  - Display of the due date for the partial amount.
  - Technical info: display field, DB field: zahlplan.ztplan
- **Chc:**
  - Checked. Indication whether the invoice has already been checked. Depending on the configuration, an invoice can only be created if it was already checked by the authorized employee.
    - [x] The invoice was checked and can be generated.
    - [ ] The invoice was not yet checked. Depending on the configuration, it may not be possible to generate the invoice.
  - Technical info: checkbox, display field
- **Cre:**
  - Create the partial invoice when you trigger invoice creation using `<F3>`.
    - [x] Create partial invoice.
    - [ ] Do not create partial invoice.
  - Technical info: checkbox

> **Payment conditions for deposit invoice**
> In the standard configuration, the deposit invoices are generated without payment conditions (such as Cash discount). This can be changed using a separate system configuration. In this case, deposit invoices are generated with cash discount for the order. For the final invoice, all automatically generated discounts for all existing deposit invoices are also marked as cash discounts. If you have additional questions about using this function, please contact the responsible A+W employee.

**Information on document tab**

The Information on Document tab only appears on the Invoices (automatic) and Delivery Notes (automatic) dialogs:
- "Invoices (automatic)" on page D-1397
- ⇨ "Delivery notes (automatic)" on page D-1391

### Partial invoice (manual)

**Sales > Invoices > Partial Invoice > Manual Invoice**

*Fig. D-152 Partial invoice (manual)*

Use this dialog to create partial invoices manually.

If there is a payment plan for the order, a notice appears asking whether the dates for the payment plan should be displayed. If you say yes, then you can select a date from the payment plan.

Manual partial invoices are entered like manual invoices. The Partial Invoice (manual) and Invoices (manual) dialogs look largely the same.

In the item area, a new item is displayed in the last line. It lists the partial amount with the amount from the payment plan.

The fields are described in connection with the Invoices (manual) dialog:
⇨ "Invoices (manual)" on page D-1402:

In addition, the following fields are displayed:

**Footer**

The total amount of the order is displayed in the Order field. If an invoice has already been generated for the reference document, the total amount of the invoice to which reference is being made is displayed in the Invoice Total field.

### Final invoices (automatic)

**Sales > Invoices > Final Invoice > Automatic Release**

*Fig. D-153 Final invoices (automatic)*

Use this dialog to create the final invoice for orders for which a payment plan was created. If there are orders for the current day for which there is a payment plan, then you can import the orders with `<Ctrl>+<F8>`. You can also enter the order numbers manually or search for them with `<F9>`.

The footer displays the customer name and total amount from the order for which a final invoice is being created.

Use `<F3>` to have the system generate the final invoices for the selected orders. In order entry, the individual orders are displayed as invoiced with the respective invoice number.

- **Order:**
  - Order number with payment plan. If you specify a number, the other fields are populated automatically with the appropriate values.
  - Technical info: mandatory field, numeric field, DB field: kauf.auftrnr, zahlplan.auftrnr
- **Amount:**
  - Amount of the final invoice. The final invoice is calculated from the total amount of the order together with the credits and less the already entered partial invoices.
  - Technical info: display field, DB field: zahlplan.betrag
- **Deliv. note:**
  - Indicates if there is already a delivery note or partial invoice. If a delivery note exists, then the entry exists is in this field.
  - Technical info: display field
- **Date:**
  - Display of the entry date of the document.
  - Technical info: display field, DB field: kauf.edat
- **Chc:**
  - Checked. Indication whether the invoice has already been checked. Depending on the configuration, an invoice can only be created if it was already checked by the authorized employee.
    - [x] The invoice was checked and can be generated.
    - [ ] The invoice was not yet checked. Depending on the configuration, it may not be possible to generate the invoice.
  - Technical info: checkbox, display field
- **Cr.:**
  - Created. Specification whether the invoice should be created.
    - [x] The final invoice will be generated.
    - [ ] The final invoice will not be generated.
  - Technical info: checkbox

### Final invoices (manual)

**Sales > Invoices > Final Invoice > Manual Invoice**

*Fig. D-154 Final invoices (manual)*

Use this dialog to create final invoices manually.

Manual final invoices are entered like manual invoices. The Final Invoice (manual) and Invoices (manual) dialogs look largely the same.

The fields are described in connection with the Invoices (manual) dialog:
⇨"Invoices (manual)" on page D-1402:

In addition, the following fields are displayed:

**Footer**

The total amount of the order is displayed in the Order field. If an invoice has already been generated for the reference document, the total amount of the invoice to which reference is being made is displayed in the Invoice Total field.

### Invoice log

**Sales > Invoices > Log**

*Fig. D-155 Invoice log*

This dialog displays the invoice log. All documents for the invoices are noted with specification of the date and time.

If you are working with internal site separation, first a dialog opens where you can specify the site number. The log displays only the documents for the selected site.

> **Invoice log for the current day**
> An invoice log is generated for the current day. If the error message is displayed that the file is empty or not readable, then no invoices have been generated on this day.

## Credit Notes

The following dialogs are described in this section:
- "Credit notes" on page D-1414
- "Book credit notes" on page D-1416

### Credit notes

**Sales > Credit Notes > Enter Credit Notes**

*Fig. D-156 Credit notes*

Use this dialog to enter credit notes. You can enter quantity credits or price credits. If you want to enter a quantity credit, you have to enter the article quantity that you want to credit in the Credit field of the appropriate item. If you want to enter a price credit, you have to enter the price that you want to credit in the price field of the appropriate item.

The fields are described for the Order Entry dialog:
⇨ "Order entry" on page D-1133

In addition, the following fields are displayed.

**Header**

**Number** Temporary number of the credit. After completion of the credit creation, the system creates a final credit number. Technical info: numeric field, DB field: kauf.auftrnr

**Ref.** Document number that is being referenced. By default, an invoice number is input for a credit.
Technical info: numeric field, DB field: kauf.referenz

**General tab**

**Cr. note** Number of credited units of the item.
Technical info: numeric field, DB field: kpos.berechnet

**Footer**

If an invoice has already been generated for the reference document, the total amount of the invoice to which reference is being made is displayed in the Invoice Total field.

### Book credit notes

**Sales > Credit Notes -> Book Credit Notes**

*Fig. D-157 Book credit notes*

Use this dialog to book credits that have not yet been transferred to the FinAc. Generally credits are booked automatically after generation.

In exceptional cases, the credit can also be booked after the fact. In the credit entry, depending on the configuration, when generating the credit a query can be displayed asking whether the credit should be booked. If you respond [No] to the query, you can import this unbooked credit on the Book Credit Notes dialog and book it after the fact.

Use `<Ctrl>+<F8>` to import the data for all credits that are generated in the specified period.

You can use `<Ctrl>+<F5>` to change to the selected credit and check, however only as long as it is not yet booked. If the credit is changed and saved with this procedure, it can also be booked directly on the Credits dialog. Confirm the corresponding query with Yes.
⇨ "Credit notes" on page D-1414

The footer displays the customer name and total amount from the order for which the credit is booked.

Use `<F3>` to book the selected credits.

**Credit notes tab**

- **Cre.note:**
  - Number of the credit.
  - Technical info: numeric field, DB field: kauf.auftrnr
- **External no.:**
  - Display of the document number that is specified by the customer. For credits from another site, the order number of the sending site is in this field.
  - Technical info: display field, DB field: kauf.exaufnr
- **Reference:**
  - Display of the reference document type, e.g. Order.
  - Technical info: display field, DB field: kauf.refvorgang
- **Number:**
  - Display of the reference document number.
  - Technical info: display field, DB field: kauf.auftrnr
- **Subnr:**
  - Display of the subnumber for reference partial invoices.
  - Technical info: display field, DB field: kauf.subnr
- **Doc. date:**
  - Display of the date of the credit creation.
  - Technical info: display field, DB field: kauf.edat
- **Betrag:**
  - Anzeige des gutgeschriebenen Beitrags.
  - Technical info: displaz field, DB field: kauf.wpreis
- **User:**
  - Display of the employee's name.
  - Technical info: display field, DB field: kauf.eusr
  - ⇨ "Credit notes" on page D-1414
- **Book date:**
  - Display of the date of the credit booking. By default, the current date is entered. If you want to specify another booking date, you have to enter the new date in the field, confirm the entry, and enter the new date again. The date is only taken over into the field after the second entry.
  - Technical info: date field, DB field: kauf.bdat
- **Bk.:**
  - Specification whether the credit should be booked.
    - [x] The credit will be booked.
    - [ ] The credit will not be booked.
  - Technical info: checkbox

Use `<F5>` to open the Items dialog on which additional details about the items are displayed.
⇨ "Item info" on page D-1400

**Information on document tab**

The Information on Document tab only appears on the Invoices (automatic) and Delivery Notes (automatic) dialogs:
⇨ "Invoices (automatic)" on page D-1397
⇨ "Delivery notes (automatic)" on page D-1391

## Forms

For the various documents, you can print forms or send them via e-mail. The forms can be generated via a REP generator or a print service with Crystal Reports.

The following dialogs are described in this section:
- "Direct printing" on page D-1418
- "Form printing" on page D-1419
- "E-mail" on page D-1423
- "Print on" on page D-1426
- "List printing" on page D-1427

### Direct printing

**Sales > Order Entry > Header, Footer area > `<F4>` > Direct Printing**

*Fig. D-158 Direct printing*

Use this dialog to print out a form for the open document. You select the form type and printer for printout on the selection dialogs.

**Form type** Specification of the form type that you want to print for the open document. Use `<F9>` to open a selection dialog with the available form types. The form types are stored in the system settings in the print management.
Technical info: numeric field, DB field: rep.formart

**Printer** Number of the printer for printing. Use `<F9>` to open a selection dialog with the available printers. The printers are stored in the system settings in the print management and assigned to the various form types.
Technical info: numeric field, DB field: drucker.drunr

Printing start if you have selected a form type and a printer and the system is configured appropriately. The Direct Printing dialog closes automatically.

### Form printing

**Sales > Forms > Print**

*Fig. D-159 Form printing*

Use these dialogs to select one or several documents for form printing.
On the Form Type selection dialog, you select the form type that you want to print. The selected form type is displayed in the upper left corner of the Form Printing dialog. Under some circumstances, you can also select several form types, e.g. order confirmation and advance delivery note.

**Sorted by** Sorting of the forms. By default, the forms are sorted by document number. The field is only activated if you have selected several form types.
- **NUMBERS:**
  - The forms are sorted by document number.
- **FORMS:**
  - The formst are sorted by form type.
Technical info: toggle field

**Additional copies** Number of additional print copies up to a maximum of 99. By default, a form is printed.
Technical info: numeric field

**(Field without name)** Specification how the documents for the form printing should be determined.
- **Enter Numbers:** In the header area of the Form Printing dialog, you can filter the documents according to various criteria. In the overview, only the documents are displayed for form printing that correspond to the filter criteria. By default, the field is pre-populated with this value.
  ⇨ "Overview" on page D-1421
- **Specify various numbers:**
  - No documents are displayed in the overview. You create the list of documents manually.
  - ⇨ "Overview" on page D-1421
Technical info: toggle field

Confirm your entry using `<Enter>`.

**Header (Select numbers)**

**from, to** Start and end value of the filter criteria:
- **Employ.:**
  - Number of the employee who entered the document. All employees with numbers between from and to will be used as filter criterion.
  - Technical info: numeric field, DB field: kauf.eust
- **Partners:**
  - All market partners for which the document was entered. All market partners with numbers between from and to will be used as filter criterion.
  - Technical info: numeric field, DB field: kauf.kunr
- **Req. On:**
  - Date on which the document was entered. By default, the current date is specified in the to field. How long the period between the two fields may be depends on the configuration in the master data.
  - ⇨ Master Data, "End of period" on page B-285
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
Technical info: toggle field

Use `<F3>` to start the search for documents that correspond to the filter criteria.

**Overview**

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

Open the following column using `<F2>`:

- **Market part.:**
  - Markdt partner number.
  - Technical info: display field, DB field: repform.kunr
- **Fax:**
  - Fax number of the market partner for the document.
  - Technical info: alphanumeric field, DB field: repform.faxnr

Use `<Shift>+<F3>` to start the printing.
⇨ "Print on" on page D-1426

### E-mail

**Sales > Forms > E-Mail/Fax**

*Fig. D-160 Dialogs under E-mail/Fax menu*

Via the dialogs under the E-mail/Fax menu element, you select a document for the dispatch of forms via e-mail.
So that forms can be sent via e-mail, the system must be configured appropriately. First, select the form type, e.g. Order confirmation, that should be sent. Then you select the type for how the document number determination should work.

**Form type** Specification of the form type that you want to send via e-mail or fax. The selected form type is displayed on the E-mail dialog in the top left corner.
Technical info: mandatory field, numeric field, DB field: rep.formart

**Select case by** Specification of which documents should be displayed.
- **Select numbers:**
  - For selection of this value, another dialog opens; in its header area, you can filter the documents according to various criteria. In the overview, only the documents for the form printing are displayed that correspond to the filter criteria.
  - ⇨ "Overview" on page D-1421
- **Specify various numbers:**
  - No documents are displayed in the overview. An empty overview dialog opens on which you can create a list of the documents manually.
  - ⇨ "Overview" on page D-1421
Technical info: toggle field

Confirm your entry using `<Enter>`.

You can only send forms to a market partner by e-mail or fax if the e-mail address and fax number are stored in the master data for this market partner. By default, this address or number is used on the E-mail dialog if you call up a document.

In the document entry, on the Addresses tab you can store an e-mail address and fax number that differ from the details in the master data. If on the E-mail dialog you call up a document with a different e-mail address or fax number, a message is displayed asking whether the different address or number from the document should be used.

**Header (select numbers)**

The header area is described for the Form Printing dialog:
⇨ "Form printing" on page D-1419

**Header (specify various numbers)**

The header area is described for the Form Printing dialog:
⇨ "Form printing" on page D-1419

**Results area**

*Fig. D-161 E-mail: Results area*

On the E-mail/Fax dialog, there are two tabs available in the results area: Overview and Additional data.

The fields are described for the Form Printing dialog:
⇨ "Form printing" on page D-1419

In addition, the following fields are displayed on the tabs:

**E-Mail:** E-mail address to which the form is sent. The e-mail address is drawn from the master data or the document.
Technical info: mandatory field, alphanumeric field

**sent:** Display of the date on which the document was sent.
Technical info: display field, DB field: druckhist.Itzdat

**CC:** E-mail address to which the form is sent in carbon copy (cc). The e-mail address is taken over from the master data or the document and it can be changed on this dialog or new information entered. The program does not check whether the e-mail address was entered correctly and/or whether the e-mail address exists.
Technical info: can field, alphanumeric field

**Bcc:** E-mail address to which the form is sent in blind carbon copy (bcc). The e-mail address is taken over from the master data or the document and it can be changed on this dialog or new information entered. The program does not check whether the e-mail address was entered correctly and/or whether the e-mail address exists.
Technical info: can field, alphanumeric field

### Print on

**Sales > Forms > Print > Select form > `<End>` > Enter data and select > `<Shift>` + `<F3>`**

*Fig. D-162 Print on*

On this dialog, you select the printer. In addition to a physical printer, you can output the form as file.

The footer indicates which form type is printed.

**Select printer** Number and description of the printer for printing. Use `<F9>` to open the list of the printers available.
Technical info: mandatory field, numeric field, DB field: repdruck.drunr

**File name** You must specify a file name for file print. This field is only shown if you select file print in the Select printer field. The output type of the printers is stored in the system settings in the print management.
Technical info: mandatory field, alphanumeric field

### List printing

**Sales > List printing > Select list**

*Fig. D-163 List printing*

Use this dialog to print out lists, e.g. the list of all orders received from particular representatives within a particular period.

First you select the list that you want to print. On the List Printing dialog you can then filter the list according to particular criteria.

**List name** Name of the list that should be printed.
Technical info: mandatory field, selection field

If you have selected a list, various fields are displayed with which you can restrict the entries in the list.
The display of the fields depends on the list selected and the SQL query in question.

If you have filled out the field, start list printing with `<F3>`.
⇨ "Print on" on page D-1426

## Order Status

For all orders, you can display the document information, e.g. the status changes.

### Order information

**Sales > Overview > Order Information > Enter order number**

This dialog displays the processing status of the selected order.

This dialog contains the following tabs:
- "Document info – order" on page D-1429
- "Document info - items" on page D-1431
- "Document info – purchasing" on page D-1433
- "Document info - goods received" on page D-1435
- "Document info – production" on page D-1437
- "Document info – dispatch" on page D-1438
- "Document info - barcoding" on page D-1440
- "Document info – racks" on page D-1442
- "Document info – stock" on page D-1444
- "Document info - linked production" on page D-1445
- "Document info – intermediate disp." on page D-1446

You can also open this dialog via order entry for the current order:
**Sales > Order Entry > Header, Footer area, Item level > `<Shift>` + `<F10>`**

### Document info - order

**Sales > Overview > Order Information > Enter order number > Document tab**

*Fig. D-164 Order information - Order tab*

This tab displays the history of the processing status of the selected document.

**Order tab**

- **Date:**
  - Date of the status booking.
  - Technical info: display field, DB field: kaufstat.datum
- **Activity:**
  - Description of the document status. The information displayed is drawn from the system. Depending on the processing status of the document, the data is drawn from A+W Enterprise or from another program, e.g. from A+W Production.
  - If you are working with internal site separation, the processing status per site is displayed.
  - Technical info: display field

**Description of buttons in footer**

**[Notes]** Branch to document notes in read mode for the selected order, if these exist. If the system is configured appropriately, notes can be changed or new ones entered. When saving, you will see a security check. If the order is locked elsewhere, the system will refuse to save. After the note changes, there is no order transfer to the background processes. This button is only available on the Document tab.

**[Prod.Report]** Branches to a production report for the selected order if this exists and the system is configured appropriately. The production report opens in a browser window.

**[Int.Order]** Branches to an internal order with individual order number for production if this exists and the system is configured appropriately. The internal orders can only be generated if the environment variable VORGANGSSTATUS_ADHOCSQL is active and you have incorporated an ad hoc SQL query. If the variable is not set, an appropriate error message is displayed.

### Document info - items

**Sales > Overview > Order Information > Enter order number > Items tab**

*Fig. D-165 Order information - Items tab*

The PO and order details for the items are displayed on this tab.

If the item status changes, the status of the appropriate item is displayed on the right of the dialog on the item level, e.g. packed, FIXED, local correction. Each item can have a different status. The item status displayed applies for the marked item.
⇨ "Explanation of symbols" on page D-1127

For additional information about the various status indicators, contact your A+W Software GmbH contact person.

**Items tab**

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

**Footer**

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Document tab:
⇨ "Document info - order" on page D-1429

In addition, the following button is displayed:

**[Info]** Displays the error message from production for the selected item. The button is only active if there is an error message for the selected item.

### Document info – purchasing

**Sales > Overview > Order Information > Enter order number > Purchasing tab**

*Fig. D-166 Order information – Purchasing tab*

> This tab displays information about the status of purchased parts.
>
> **Two fields for item numbers**
> This tab displays two Itm fields. They differ from one another and display different item numbers.

**Purchasing tab**

The columns are described for the Items tab:
⇨ "Document info - items" on page D-1431

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
- **Itm (field between POno and Ordered):**
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
- **PU price:**
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

**Footer**

The name of the supplier for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
⇨ "Document info – items" on page D-1431

### Document info – goods received

**Sales > Overview > Order Information > Enter order number > Goods Received tab**

*Fig. D-167 Order information - Goods received tab*

> **Two fields for item numbers**
> This tab displays two Itm fields. Column 1 displays the number of the order item and column 5 for purchased articles the number of the order item.

**Goods received tab**

The columns are described for the Items tab:
⇨ "Document info - items" on page D-1431

In addition, the following columns are displayed:

- **Ρ.Ο.:**
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
- **Deliv.date:**
  - Delivery date for the purchased parts.
  - Technical info: display field, DB field: bpol.ltplan
- **Received:**
  - Delivered quantity in the article quantity unit of the article ordered that has been booked in incoming goods.
  - Technical info: display field, DB field: kpos.geliefert
- **DPI:**
  - Delivery plan. Specification whether a delivery plan for the item exists.
    - D: There is a delivery plan for the item.
    - (blank): There is no delivery plan.
  - Technical info: display field

**Footer**

The description of the article and the name of the supplier for the selected item are displayed at the lower left of the dialog.

The buttons are described for the Items tab:
⇨ "Document info – items" on page D-1431

### Document info – production

**Sales > Overview > Order Information > Enter order number > Production tab**

*Fig. D-168 Order information - Production tab*

This tab displays the order status from the production system.

**Production tab**

The columns are described for the Items tab:
⇨ "Document info - items" on page D-1431

In addition, the following columns are displayed:
- **Status:**
  - Number of the production status.
  - Technical info: display field, DB field: kposstat.status
- **Information text:**
  - Description of the production status. The text is pre-populated by the system and displayed in the configured system language.
  - Technical info: display field, DB field: kposstat.infotxt
- **Date:**
  - Date of the reporting of the status displayed.
  - Technical info: display field, DB field: kposstat.datum
- **Time:**
  - Time of the reporting of the status displayed.
  - Technical info: display field, DB field: kposstat.zeit
- **Qty.:**
  - Quantity from the report in article quantity unit.
  - Technical info: display field, DB field: kpos.menge

**Footer**

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
⇨ "Document info - items" on page D-1431

### Document info – dispatch

**Sales > Overview > Order Information > Enter order number > Dispatch tab**

*Fig. D-169 Order information – Dispatch tab*

This tab displays information about the status of dispatch.

**Dispatch tab**

The columns are described for the Items tab:
⇨ "Document info - items" on page D-1431

In addition, the following columns are displayed:

- **Sta:**
  - Traffic light display of the current item status.
  - Technical info: display field
  - ⇨ "Explanation of symbols" on page D-1127
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
    - Exit: goods are being sent.
    - Inbound: goods will be received, e.g. after processing by a different site.
  - Technical info: display field, DB field: kposstat.status

**Footer**

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
⇨ "Document info – items" on page D-1431

### Document info – barcoding

**Sales > Overview > Order Information > Enter order number > Barcoding tab**

*Fig. D-170 Order information - Barcoding tab*

This tab displays the information about the barcoding status if you are working with plant data collection.

Use `<F5>` to change the view of the tab. The values are then displayed summarized by item and machine number.

**Barcoding tab**

The columns are described for the Items tab:
⇨ "Document info – items" on page D-1431

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
- **JobNo**
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

**Footer**

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
⇨ "Document info - items" on page D-1431

### Document info - racks

**Sales > Overview > Order Information > Enter order number > Racks tab**

*Fig. D-171 Order information - Racks tab*

This tab displays information from the packing planning per rack.
A line is displayed per rack, whereby it is possible that several items can be packed on a rack or an item can be distributed across several racks.

**Racks tab**

The columns are described for the Items tab:
⇨ "Document info - items" on page D-1431

In addition, the following columns are displayed:

- **Rack:**
  - Number of the rack on which the articles are planned. The number is assigned automatically by the system.
  - Technical info: display field, DB field: kposgest.vsgnr
- **External number:**
  - External PO number of the customer. For orders from another site, the order number of the sending site is in this field.
  - Technical info: display field, DB field: gestellz.exgnr
- **SerNo:**
  - Item number from the order.
  - Technical info: display field, DB field: kpos.Ifdpos
- **Deliv.date:**
  - Date of the delivery for the rack.
  - Technical info: display field, DB field: vsaufgest.Itplan
- **Route:**
  - Number of the route on which the rack is transported.
  - Technical info: display field, DB field: vsaufgest.routennr
- **ActQty:**
  - Quantity of articles that are planned on the rack.
  - Technical info: display field, DB field: lapool.iststk

**Footer**

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
⇨ "Document info - items" on page D-1431

### Document info – stock

**Sales > Overview > Order Information > Enter order number > Stock tab**

*Fig. D-172 Order information - Stock tab*

This tab displays the status information about the stock article that is entered in the order.

**Stock tab**

The columns are described for the Items tab:
⇨ "Document info - items" on page D-1431

In addition, the following columns are displayed:

- **Stocktype:**
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

**Footer**

Additional article information on the selected item.
The buttons are described for the Items tab:
⇨ "Document info - items" on page D-1431

### Document info – linked production

**Sales > Overview > Order Information > Enter order number > Linked Production tab.**

*Fig. D-173 Document info – Linked Production tab*

This tab displays the status information from the linked production if you are working with internal site separation.

For additional information about this area, contact your A+W Software GmbH contact person.

**Linked production tab**

The tab is structured the same way as the Production tab:
⇨ "Document info - production" on page D-1437

**Footer**

The description of the article for the selected item is displayed at the lower left of the dialog.

The buttons are described for the Items tab:
⇨ "Document info - items" on page D-1431

### Document info – intermediate disp.

**Sales > Overview > Order Information > Enter order number > Intermediate Disp. tab**

*Fig. D-174 Document info – Intermediate Disp. tab*

This tab displays information about the status of articles from the extended workbench.

**Intermediate disp. tab**

The tab is structured the same way as the Production tab:
⇨ "Document info - production" on page D-1437

## Document Research

To search for documents, there is a search with extensive search criteria available.

The following dialogs are described in this section:
- "Search document" on page D-1447
- "Items" on page D-1460

### Search document

**Sales > Overview > Search Document**

Use this dialog to search for documents. The results are displayed in a hit list.
This dialog contains the following tabs:
- "Search document – search mode" on page D-1447
- "Search document – overview" on page D-1451
- "Search document – employees” on page D-1453
- "Search document – details" on page D-1455
- "Document change log" on page D-1458

You can also open this dialog via the Info menu with `<Shift>+<F4>` in the header area of the order entry.

### Search document – search mode

**Sales > Overview > Search Document**

*Fig. D-175 Search document - search mode*

Use this dialog to restrict the search with the specified criteria. You specify the criteria with conditions. The more criteria you specify for the search, the more you restrict the search.

Use `<Shift>+<F8>` or `<Shift>+<F12>` to change the condition. The info line displays the meaning of the selected condition.

| Condition | Meaning |
| :--- | :--- |
| **=** | Search exactly for this value (e.g. market partner field = 600004 lists only documents relating to this market partner). |
| **>** | Search for larger values (e.g. market partner field > 600004 lists only documents with market partner numbers larger than 600004). |
| **p** | Search for patterns in text fields (e.g. field Shape 12 lists all documents with the reference text Shape 12.) |
| **0** | Search for values = 0 (e.g. market partner field 0 lists only market partners with the number 0). |
| **z** | Search all values in the range. |
| **!** | Search all values except for this value (e.g. Department field! 10 lists all departments except for the department with the number 10). |
| **<** | Search for smaller values (e.g. market partner field < 600004 lists only documents with market partner numbers smaller than 600004). |

*Tab. D-13 Meaning of the filter conditions*

**Site No.** Site number and description of the site. If you specify a number, the description of the site is displayed in plain text.
Technical info: numeric field, display field, DB fields: kauf.hausnr

**Company** Number of the company to which the site is assigned. The field is only enabled if you are working with internal site separation.
Technical info: display field, DB field: kauf.company

**Document** Document type. If you select a document type, the code number of the document type is displayed in plain text.
- Inquiries
- Purchase orders
- Receipt of goods
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
  - ⇨ "Document change log" on page D-1458
Technical info: toggle field, display field, DB field: kauf.vorgang

**Doc. date** Entry date of the document in the format DD.MM.YYYY.
Technical info: date field, DB field: kauf.edat

**Market partner** Market partner number and description. If you specify a number, the description of the market partner is displayed in plain text. The match code of the market partner is assigned to a market partner type.
Technical info: numeric field, display field, DB fields: kauf.kunr, mp.name

**(Matchcode)** Market partner type. In Sales, Customer is pre-populated as market partner type. If you select a market partner, the market partner's match code is displayed automatically next to the field.
Technical info: toggle field, DB field: mp.mpmc

**Cust. PO No.** Customer purchase order number.
Technical info: alphanumeric field, DB field: kauf.exaufnr

**External ref.** Reference text.
Technical info: alphanumeric field, DB field: komm.kommtxt

**Project** Project number and description of the project, e.g. construction site. If you specify a number, the description of the project is displayed in plain text.
Technical info: numeric field, display field, DB fields: kauf.objnr, mp.name

**Number** Document number.
Technical info: numeric field, DB field: kauf.auftrnr

**Subno** Subnumber, e.g. partial delivery note.
Technical info: numeric field, DB field: kauf.subnr

**Departm.** Number and name of the department of the person entering the document. If you specify a number, the name of the department is displayed in plain text.
Technical info: numeric field, display field, DB field: kauf.abtnr

**Invoice** Invoice number. The number is saved in the database table vorgang with the value 7.
Technical info: numeric field, DB field: kauf.auftrnr

**Sales repr.** Number and name of the representative. If you specify a number, the name of the representative is displayed in plain text.
Technical info: numeric field, display field, DB field: kauf.vertrerloe

**Ordered** PO date in the format DD.MM.YYYY.
Technical info: date field, DB field: kauf.bdat

**Route** Number and description of the route. If you specify a number, the description of the route is displayed in plain text.
Technical info: numeric field, display field, DB field: kauf.routenr

**Deliv. date** Planned delivery date in the format DD.MM.YYYY.
Technical info: date field, DB field: kauf.ltplan

**Entered** Number and name of the person entering the document. If you specify a number, the name of the person entering the document is displayed in plain text.
Technical info: numeric field, display field, DB field: kauf.eusr, mitarb.maname

**Suspended** Indication whether the document is suspended. The identifier and code number are set automatically if you select a document.
- **n:**
  - The document is not suspended. The code number 0 is displayed. By default, the field is pre-populated with the identifier n.
- **y:**
  - The document is suspended. The code number 1 is displayed. The identifier is set if in the Document field you have selected the document type SA cancellations or PU cancellations.
Technical info: toggle field, display field, DB field: kauf.storno

**Footer**

**Start**
Start search for documents with the specified criteria.

### Search document – overview

**Sales > Overview > Search Document > Enter search criteria > `<F3>` > Overview tab**

*Fig. D-176 Search document - overview*

This tab displays the hit list of documents matching the search criteria.

**Header**

The fields in the header area only provide information. You cannot edit the entries.

**Market partner** Number, matchcode, and name of the market partner.
Technical info: display fields, DB fields: mp.kuliflag, mp.mpnr, mp.mpmc

**Address** Street address of the market partner.
Technical info: display field, DB field: mp.str

**PCd.city** Postal code and city of the market partner.
Technical info: display fields, DB fields: mp.plz, mp.ort

**Phone** Telephone number of the market partner.
Technical info: display field, DB field: mp.telefon

**Fax** Fax number of the market partner.
Technical info: display field, DB field: mp.faxnr

**Evaluation** Number of the evaluation of the quality of the market partner. The evaluation is created in the market partner master data.
Technical info: display field, DB field: mp.qqual

> **Store evaluation in the master data**
> Store evaluations under the following path: Master data > Market partner > Select market partner > Evaluation tab > Quality field.

**Overview tab**

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
- **Del. date:**
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

**Footer**

For the values Net and Margin, the totals of the values of all items are listed. For % (percentage of price margin), the average value of the items is listed.

### Search document – employees

**Sales > Overview > Search Document > Enter search criteria > `<F3>` > Employee tab**

*Fig. D-177 Search document – employee*

This tab displays the employee information about the employee's documents.

**Header**

The fields are described on the Overview tab.
⇨ "Search document - overview" on page D-1451

**Employee tab**

Some columns are described for the Overview tab:
⇨ "Search document – overview" on page D-1451

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

### Search document – details

**Sales > Overview > Search Document > Enter search criteria > `<F3>` > Details tab**

*Fig. D-178 Search document - details*

Use this tab to display the details for the selected document.
Use `<Page Down>` to change to the next document, `<Page Up>` to the previous document.

**Header**

The fields are described on the Overview tab.
⇨ "Search document - overview" on page D-1451

**Details tab**

**Document** Number and subnumber of the document.
Technical info: numeric field, display field, DB fields: kauf.auftrnr, kauf.subnr

**Act.ref.no** Number of the original document for transferred documents. The site number of the sender is in the first field; the second number contains the original document number. Technical info: display fields, DB fields: kauf._orgauftrnr

**Prev.ref.no.** Previous document number for transferred documents, e.g. the reference number for the original document.
Technical info: display fields, DB field: kauf.referenz

**Market partner** Number and name of the market partner.
Technical info: display field, DB field: kauf. kunr, mp.name

**Delivery date** Delivery date.
Technical info: display field, DB field: kauf.Itplan

**Invoice** Invoice number pertaining to the document.
Technical info: display field, DB field: kauf.rechnr

**Cust. PO no.** External PO number for the customer. For orders from another site, the order number of the sending house is displayed in this field.
Technical info: display field, DB field: kauf.exaufnr

**P.O. date** Date of the P.O.
Technical info: display field, DB field: kauf.edat

**Proj.** Number and description of the project. A project can be a construction site or delivery address, for example.
Technical info: display fields, DB fields: kauf.objnr, kauf.orgname

**Departm.** Number and name of the department in which the order has been entered.
Technical info: display fields, DB field: kauf.abtnr

**Total sqft** Total glass area of the document in square meters.
Technical info: display field, DB field: kauf.gesm2

**Tot. pieces** Total number of pieces of units from all items of the order.
Technical info: display field, DB field: kauf.gesst

**Disc.** Discount granted for the total amount in percent and as amount.
Technical info: display fields, DB fields: kauf.gesfaktor

**Net total** Total of all item prices, minus the discounts and plus the surcharges.
Technical info: display field, DB field: kauf.nettototal

**Margin** Profit margin of the document in percent and in currency units.
Technical info: display fields, DB fields: kauf.dbvh, kauf.dbdm

**Pay. term** Term of payment and cash discount deductions that have been agreed upon with the market partner.
Technical info: display field, DB field: kauf.zahlziel

**Val.date** Period until the value date in days.
Technical info: display field, DB field: kauf. valuta

**Cash D. 1, 2, %** Period (number of days) during which a cash discount is applicable. The second field (%) reflects the percentage for the cash discount. The fields are preset with the market partner data.
Technical info: display fields, DB fields: kauf._skonto1, kauf.skvh1, kauf._skonto2, kauf.skvh2

**Ent'rd on, by** Date of the document entry, number and name of the person who entered it.
Technical info: display fields, DB fields, kauf.edat, kauf.eusr

**Receipt** Type of communication of the document entry, e.g. fax.
Technical info: display field, DB field: kauf.eingang
⇨ "Receipt" on page D-1137

### Document change log

**Sales > Overview > Search Document > Document field > Define the value to be changed as search criteria > `<Enter>`**

*Fig. D-179 Search document – document change log*

Use this dialog to display a log of document changes.

> **Automatic display of the dialog**
> The Document Change Log dialog is displayed automatically if you specify Change as search criterion in the Document field and change to the next field.

You can restrict the display of the document changes by date and document type. After entering the search criteria, the log is displayed in a view.
- Use `<Enter>` to display the log of the document changes.

**Log search**

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
Technical info: toggle field, DB field: kauf.vorgang

**from date** Display of document changes starting on this date. The format is DD.MM.YYYY. By default, the current date is pre-set.
Technical info: date field

**to date** Display of document changes up to this date. The format is DD.MM.YYYY. By default, the current date is pre-set.
Technical info: date field

**Log display**

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

**Sales > Overview > Search Document > Enter search criteria > `<F3>` > Select document > `<Shift>` + `<F9>`**

Use this dialog to display the information about the items of the selected document.

This dialog contains the following tabs:
- "Items - overview" on page D-1460
- "Items - details" on page D-1462

### Items - overview

**Sales > Overview > Search Document > Enter search criteria > [Start] > Select tab > Select document > `<Shift>` + `<F9>` >Overview tab**

*Fig. D-180 Items - overview*

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
- **Labor cost:**
  - Labor costs for the production / processing of the item. Is calculated in A+W Production and reported.
  - Technical info: display field, DB field: kposp.kolohn
- **Mach. costs:**
  - Machine costs for the production / processing of the item. Is calculated and reported in A+W Production.
  - Technical info: display field, DB field: kposp.kobm

**Footer**

The footer displays the type and number of the selected document.

### Items - details

**Sales > Overview > Search Document > Enter search criteria > [Start] > Select tab > Select document > `<Shift>` + `<F9>` > Details tab**

*Fig. D-181 Items - details*

Details about the items for the order are displayed on this tab.

**Item** Number of the item.
Technical info: numeric field, DB field: kpos.Ifdpos

**Article** Number and description of the article.
Technical info: display field, DB field: kpos.artnr

**Shape** Shape number of the article.
Technical info: display field, DB field: kpos.modnr

**Prod. group** Indicator of the product group allocated to the article.
Technical info: display field, DB field: kpos.wagrp

**Supplier** Supplier number.
Technical info: display field, DB field: kpos.liefnr

**Quantity** Item quantity.
Technical info: display field, DB field: kpos.menge

**Dims.** Width, height and airspace of this item in millimeters and total surface in square meters.
Technical info: display fields: DB fields: kpos.laenge, kpos.breite, kpos.szr, kpos.qm

**SA price, PU price**

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

**Costs**

**Mat. costs** Material costs of the item, e.g. the material value including waste.
Technical info: display field, DB field: kposp.komat

**Labor cost** Labor costs of the item.
Technical info: display field, DB field: kposp.kolohn

**Mach. costs** Machine costs calculated from the life and cost rate of the equipment.
Technical info: display field, DB field: kposp.kobm

**Proc.** Monetary value of sales.
Technical info: display field, DB field: kpos.erloes

**Margin** Margin between the sales price and purchase price.
Technical info: display field, DB field: kpos.spanne

**Footer**

The footer displays the type and number of the selected document.

## Overviews of Documents

There are various dialogs available in order to inform you about the state of documents. The dialogs display overviews of data that is determined from the documents.

The following dialogs are described in this section:
- "Order display" on page D-1465
- "Quotation display" on page D-1466
- "Resubmission" on page D-1467
- "Document change" on page D-1471
- "Overview of documents" on page D-1476

### Order display

**Sales > Overview > Order Display**

*Fig. D-182 Order display*

On this dialog you open an order in display mode. You can open an order in display mode at any time, e.g. even if the order is locked by a background process or is being edited by another user.

The data on the Order Display dialog serves only informational purposes. You cannot call up all order functions and you cannot edit the entries.

The tabs and fields are described for the Order Entry dialog:
⇨ "Order entry" on page D-1133

### Quotation display

**Sales > Overview > Quotation Display**

*Fig. D-183 Quotation display*

Use this dialog to open a quotation in display mode. You can open a quotation in display mode at any time, e.g. even if the quotation is locked by a background process or is being edited by another user.

The data on the Quotation Display dialog serves only informational purposes. You cannot call up all quotation functions and you cannot edit the entries.

The tabs and fields are described for the Order Entry dialog:
⇨ "Order entry" on page D-1133

### Resubmission

**Sales > Resubmission**
**Sales > Document Entry > Header, Footer area, Item level > `<F4>` > Resubmission**

*Fig. D-184 Resubmission*

Use this dialog to enter processing remarks for a resubmission. When the resubmission date has arrived, a message will be displayed for the selected employee at the program start or a reminder e-mail sent.

You can create process-free resubmissions without any reference to a document.

You can only create document-related resubmissions if you enter a quotation with a delivery date. These resubmissions are always related to a business process.

- Use `<F6>` to create additional resubmissions.
- Use `<F7>` to delete individual resubmissions.
- Use `<End>` to save the resubmission and close the dialog.

**Present.dat** Submission date when a reminder about the document is issued. Depending on the system configuration, the resubmission can also be displayed automatically or if particular conditions are fulfilled.
Technical info: mandatory field, date field, DB field: vorlage.vldat

**Present.type** Type of resubmission.
- **Memo in message system:**
  - The message system will transfer memos to the user. Use `<Ctrl>+<F4>` to retrieve messages in the mail system. If you are working with an external mail program, the system can be configured so that you can also call up the mails via the corresponding program.
  - If an e-mail address is stored, the message recipient will be sent an external e-mail.
- **Active resubmission:**
  - All messages are displayed on the screen when you start the program.
- **Direct deletion of the document:**
  - This function is only authorized for customer quotations and requests for quotations to suppliers. Thus, the resubmission for the document when the document date is reached is cancelled.
Technical info: toggle field, DB field: vorlage.modus

**Present to (employee)** Number of the employee who will receive the resubmission. By default, the individual entering the document is preset here. If you specify a number, the name of the employee is displayed in plain text. Technical info: numeric field, DB field: vorlage.outmanr

**Text fields** Fields for information texts about the document that are displayed at the time of resubmission. If you enter a document-related resubmission, the number of the quotation is displayed next to the first text field.
Technical info: alphanumeric fields, DB fields: vorlage.text1, vorlage.text2

### Completion report

**Sales > Completion Report**

*Fig. D-185 Completion report*

Use this dialog to report items for an order complete.

As a rule, completion reports are made from production or purchasing and do not have to be transmitted manually.
- Use `<F5>` to delete the items whose total item quantity is already reported complete. For these items, the Compl. field is empty.
- Use `<F3>` to book the completion report.

**Header**

**Site** Display of the site number.
Technical info: display field, DB field: kauf.hausnr

**Order** Order number.
Technical info: mandatory field, numeric field, DB field: kauf.auftrnr

**Dept.** Number of the department of the person who entered the order.
Technical info: numeric field, DB field: kauf.abtnr

**Deliv. date** Planned delivery date of the order.
Technical info: display field, DB field: kauf.ltplan

**Completion report** Date in the format DD.MM.YYYY on which the order should be reported complete. By default, the current date is pre-set.
Technical info: mandatory field, date field, DB field: kauf.bdat

**Overview**

- **Order:**
  - Order number.
  - Technical info: display field, DB field: kauf.auftrnr
- **Itm:**
  - Item number in the order.
  - Technical info: display field, DB field: kpos.posnr
- **Article:**
  - Description of the article from the selected item.
  - Technical info: display field, DB field: kpos.artnr, kpos.artbez1
- **Total:**
  - Total item quantity.
  - Technical info: display field, DB field: kpos.menge
- **So far:**
  - Quantity of the item already reported complete.
  - Technical info: display field, DB field:
- **Compl.:**
  - Quantity of the item that should be reported complete. By default, the difference of the total quantity of the item and the quantity previously reported complete is specified. You can edit the quantity that should be reported complete.
  - Technical info: numeric field, DB field:

**Footer**

**Book**
Books the completion report.

**Cancel**
Cancels the completion report.

### Document change

**Sales > Document Change**

*Fig. D-186 Document change*

Use this dialog to correct several documents simultaneously. The documents can be corrected faster than on other dialogs since no time is required to load an entire document. You cannot make corrections go documents at any time; they depend on the item status.
⇨ "Item status and item identifier" on page D-1127

The dialog is divided into three tabs, which branch to various fields.
- Use `<F2>` to change between the tabs on the dialog.
- Use the right mouse button to open the context menu.
- Use `<Ctrl>+<F10>` to search for documents with declarations of performance for a delivery date. All documents with declarations of performance for the delivery date searched for are displayed.
- Use `<Ctrl>+<F11>` to mark all records starting with the current one.
- Use `<Ctrl>+<F8>` to import the data for the document change. The data is imported via a freely configurable WQL query. The amount of data imported depends on the SQL query in question.
- use `<F5>` to display additional information about the document if any is stored.
- Use `<F3>` to trigger the booking of the corrections.
- Use `<Shift>+<F5>` to change to order entry.
⇨ "Order entry" on page D-1133

**General tab**

- **Document:**
  - Document type.
    - Order
    - Deliv.: Delivery
    - Quot.: quotation
  - Technical info: toggle field, DB field: zuaufint.vorgang
- **Number:**
  - Document number.
  - Technical info: numeric field, DB field: zuaufint.auftrnr
- **SubNo:**
  - Subnumber of the document.
  - Technical info: display field, DB field: zuaufint.subr
- **Info:**
  - Indication whether there is additional information about the document.
    - (blank): There is no additional information
    - /: There is additional information.
  - Technical info: display field, toggle field
- **Local Correct.:**
  - Information as to whether the document is in local correction status. The notice is only displayed if the document is in this stauts. The field is locked.
  - Technical info: display field, DB field:
- **Ccl:**
  - Cancellation. Specification whether the document should be cancelled.
    - [x] The document will be cancelled.
    - [ ] The document will not be cancelled.
  - Technical info: checkbox, DB field: zuaufint.storno
- **Site:**
  - Site number that is assigned to the document.
  - Technical info: mandatory field, numeric field, DB field: zuaufint.hnr
- **Route:**
  - Number of the shipping route.
  - Technical info: mandatory field, numeric field, DB field: zuaufint.route
- **Date:**
  - Date of the planned delivery in the format DD.MM.YYYYTechnical info: date field, DB field: zuaufint.Itidea.
- **PMS:**
  - Specification whether the document should be transferred to the production management system. The specification is only valid if the production management system is used.
    - [x] The document will be transferred to the production management system.
    - [ ] The document will not be transferred.
  - Technical info: checkbox, DB field: zuaufint.pmsflag
- **Dsp:**
  - Dispatch control. Specification whether the document should be transferred to the document control.
    - [x] The document is transferred to the document control.
    - [ ] The document will not be transferred.
  - Technical info: checkbox, DB field: zuaufint.lapoolflag
- **Txt.:**
  - Specification whether the texts for the document should be generated anew.
    - [x] The system will generate the texts anew.
    - [ ] The system will not generate the texts anew.
  - Technical info: checkbox, DB field: zuaufint.txtflag
- **PGr:**
  - Specification whether the product group assignment for the document should be created anew.
    - [x] The assignment will be updated for the document.
    - [ ] The assignment for the document will not be updated.
  - Technical info: checkbox, DB field: zuaufint.wgrpflag
- **Rel.:**
  - Specification whether the document should be released.
    - [x] The document will be released.
    - [ ] The document will not be released.
  - Technical info: checkbox, DB field: kauf.tekapkz

Use `<F2>` to change to the Dispatch tab. The following fields are displayed here:

- **Document:**
  - Document type.
    - Order
    - Deliv.: Delivery
    - Quot.: quotation
  - Technical info: toggle field, DB field: zuaufint.vorgang
- **Order:**
  - Document number.
  - Technical info: mandatory field, numeric field, DB field: zuaufint.auftrnr
- **SubNo:**
  - Subnumber of the document.
  - Technical info: display field, DB field: zuaufint.subr
- **Disp. Type:**
  - Number of the dispatch type.
  - Technical info: numeric field, DB field: zuaufint.sfill1
- **Deliv. type:**
  - Number of the delivery type.
  - Technical info: numeric field, DB field: zuaufint.sfill2
- **DepCusto:**
  - Code number of the outgoing customs office.
  - Technical info: numeric field, DB field: zuaufint.sfill3
- **DesCusto:**
  - Code number of the destination customs office.
  - Technical info: numeric field, DB field: zuaufint.Ifill1
- **Disp. info:**
  - Company-internal information text about the dispatch.
  - Technical info: alphanumeric field, DB field: zuaufint.cfill1
- **DP:**
  - Specification of whether there is a declaration of performance.
    - [x] There is a declaration of performance.
    - [ ] There is no declaration of performance.
  - Technical info: checkbox
- **Rel.:**
  - Specification whether the document should be released.
    - [x] The document will be released.
    - [ ] The document will not be released.
  - Technical info: checkbox, DB field: kauf.tekapkz

Use `<F2>` again to change to the Calculation tab. The following fields are displayed here:

- **Document:**
  - Document type.
    - Order
    - Deliv.: Delivery
    - Quot.: quotation
  - Technical info: toggle field, DB field: zuaufint.vorgang
- **Order:**
  - Document number.
  - Technical info: mandatory field, numeric field, DB field: zuaufint.auftrnr
- **SubNo:**
  - Subnumber of the document.
  - Technical info: display field, DB field: zuaufint.subr
- **DP:**
  - Specification of whether there is a declaration of performance.
    - [x] There is a declaration of performance.
    - [ ] There is no declaration of performance.
  - Technical info: checkbox
- **Calculation:** Type of calculation that can be executed. The following selection is possible with the [Spacebar].
  - No new calculation
  - Sales and purchase prices
  - Sales prices
  - Purchase prices
  - Technical info: alphanumeric field, DB field: zuaufint.rechart
- **Discounts:**
  - Type of correction for the discounts present in the document. The following selection is possible with the [Spacebar].
    - Update special discounts
    - New discount methods
    - All discounts new
  - Technical info: alphanumeric field, DB field: zuaufint.rabrechart
- **Rel.:**
  - Specification whether the document should be released.
    - [x] The document will be released.
    - [ ] The document will not be released.
  - Technical info: checkbox, DB field: kauf.tekapkz

### Overview of documents

**Sales > Overview > Orders not Invoiced, Invoices not Booked, Deliveries not Complete, Orders Locked for Invoicing > Enter date > [OK]**

*Fig. D-187 Orders not invoiced, Invoices not booked, Deliveries not complete, and Orders with invoice block*

These dialogs display the overviews for the following documents in the selected period:
- **Orders not invoiced:**
  - Displays all orders for which no invoice has been created.
- **Invoices not booked:**
  - Displays all documents for which an invoice has been created that was not yet booked.
- **Incomplete deliveries:**
  - Displays all documents for which there are incomplete deliveries.
- **Orders with invoice block:**
  - Displays all orders for which invoicing is blocked.

If you want to open one of the overviews, you first have to enter the start date for the search. If you do not specify a date, all corresponding documents will be displayed in the overview.

The display of the columns is freely configurable and depends on the customer-specific formatting of the SQL query in question.

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

### Sales

In Sales, information about customer acquisition and commission calculation is displayed and you can manage the project budgeting.

All dialogs that you can open via the Sales menu element are customer-specific program adjustments.

For additional information about this area, contact your A+W Software GmbH contact person.

---

# D A+W Enterprise Sales Help Cards

## This section provides information on the following subjects:

- Information about the Help Cards
- Quotation
- Order
- Order item
- Price Calculation
- Invoice
- Other topics

- **Information about the Help Cards** D-1482
- **Quotation** D-1483
  - Quick entry D-1484
  - Enter quotation D-1485
- **Order** D-1486
  - Enter header data D-1487
  - Enter order with reference D-1488
  - Specify order type D-1489
  - Edit properties D-1490
  - Change shipping address D-1491
  - Change delivery plan D-1492
  - Changing payment options D-1493
  - Release order D-1494
  - Show order information D-1495
  - Edit text in order D-1496
  - Editing notes D-1497
  - Attach file D-1498
- **Order item** D-1499
  - Enter item D-1500
  - Edit supplier D-1501
  - Exchange glass D-1502
  - Shape input D-1503
  - Enter processing step D-1504
  - Adopt processing from SN file D-1505
  - Add SN file D-1506
  - Synchronizing changes with SN file D-1507
  - Enter item in CAD D-1508
  - Enter stepped glass D-1509
  - Enter muntins D-1510
  - Edit muntin structure D-1511
  - Edge clearance and sealing depth D-1512
  - Enter edge stripping D-1513
  - Replace product D-1514
  - Fix product D-1515
  - Allocate declaration of performance D-1516
  - Enter technical values D-1517
- **Price Calculation** D-1518
  - Change item conditions D-1519
  - Change article prices D-1520
  - Edit footer discount, surcharge D-1521
  - Check production costs D-1522
  - Price report for LAMI D-1523
- **Invoice** D-1524
  - Create invoice manually D-1525
  - Create invoices automatically D-1526
  - Book invoice D-1527
  - Print invoice D-1528
  - Send electronic invoice (e-invoicing) D-1529
  - Configure customers for electronic invoices D-1530
  - Enter a credit note D-1531
- **Other topics** D-1532
  - Search for document D-1533
  - Document change D-1534

## Information about the Help Cards

The depictions in the Help Cards are based on the delivery version A+W Enterprise V 6. Individual steps in the workflows may deviate depending on the configuration.

**Orders as example**
Various functionalities can be started in several document types. In these help cards, they will always be shown using the example of an order.

**Keys and key combinations**
Knowledge of the operation is assumed as a precondition. In the steps, just one of the possible keys or key combinations will be named with which a function or menu can be called up. The functions and keys possible on the open dialog can be displayed in the prompt line at the lower edge of the dialog.

## Quotation

| Help Card | Topics |
| :--- | :--- |
| **Quick entry** | - Create quotation quickly.<br>- Create order quickly. |
| **Enter quotation** | - Enter quotation.<br>- Edit resubmission.<br>- Create manual resubmission. |

### Quick entry (SA 01-001)

*Image: Quick entry dialog*

**Goal of the action**
- Enter order quickly.
- Enter quotation quickly.

**Requirements**
- Quick entry must be configured.
- Master data must be adjusted.

**Additional info**
N/A

**Workflow**
1.  Select the menu `Sales > Quick entry`.
    The `Order entry` dialog is opened with Market partner search.
2.  Select customer and take over.
3.  Check and fill out mandatory fields *.
4.  Select the `Shipping address` area with [Address search].
    If necessary, create address with [New address].
5.  Change to the `Items` tab.
6.  `ProductCode` field: select or enter product code.
7.  Add item data.
8.  Repeat steps 6 and 7 for additional items as necessary.
9.  Change to the `Overview` tab.
10. Create order with [Save].

**Enter quotation quickly:**
11. Repeat steps 1 to 9.
12. Create quotation with [Save as quotation].
    The `Reason` dialog for the quotation opens.
13. Enter the reason and take over with [OK].
14. Confirm reference to new quotation number.

**Next step:**
- Create another order using the quick entry.
- Close the dialog with `<Esc>`.

### Enter quotation (SA 01-002)

*Image: Quotation entry and Resubmission dialogs*

**Goal of the action**
- Enter quotation.
- Edit resubmission.
- Create manual resubmission.

**Requirements**
- Automatic resubmission is set up:
  `System > Document Management > Resubmission`
  `Mode` menu.

**Additional info**
- Delete resubmission: Press `<F7>`.
- Automatic resubmissions are set up per document type.
- Enter manual resubmission for order: `Date > <Shift> + <F4> > Resubmission` field.
- Enter item
- Search for document

**Workflow**
1.  Select `Sales > Quotation Entry` menu.
    The `Quotation entry` dialog opens.
2.  Select customer.
3.  `Date` field: enter possible delivery date if necessary.
    Alternative: the delivery date is determined and written back by `A+W Production`.
4.  Enter items and save quotation.

**Edit resubmission:**
5.  Select `Sales > Resubmission` menu.
    The `Resubmission` dialog opens.
6.  Select current quotation:
    - Edit date for resubmission.
    - Enter remark.

**Create manual resubmission:**
7.  Select `Sales > Resubmission` menu > `<F6>`.
    A new line is added at the end of the list.
8.  Fill out the fields in the new line.
    - Enter the date.
    - Select the submission type and enter text.
    - Select the user.
9.  Close the dialog with `<End>`.

## Order

| Help Card | Topics |
| :--- | :--- |
| **Enter header data** | Create order. |
| **Enter order with reference** | Enter order with reference to quotation. Enter quotation with reference to earlier order. |
| **Specify order type** | Enter stock order. Enter top priority order. Enter redelivery as goodwill order. |
| **Edit properties** | Change dispatch information. Change invoice and print options for commercial papers. Change sales representative. |
| **Change shipping address** | Enter shipping address for order. Take over new shipping address in master data. |
| **Change delivery plan** | Specify delivery date for item and total quantity. Create delivery plan for partial deliveries of an item. |
| **Changing payment options** | Change payment options. |
| **Release order** | Release orders of a department and/or a user. Release all orders. Check reasons for lock. |
| **Show order information** | Check production status of the order. Check delivery date changes. |
| **Edit text in order** | Enter header or footer text for the order. Edit article and item text. Check article text in customer language. |
| **Editing notes** | Enter internal remark about the order header or footer. Enter internal remark about the item or article. |
| **Attach file** | Attach document for the customer. Attach document for the item. |

### Enter header data (SA 02-001)

*Image: Order entry dialog header*

**Goal of the action**
- Create order.

**Requirements**
- Master data is entered completely.

**Additional info**
- Quotations are entered in the same way as orders: Menu `Sales > Enter quotation`.
- ⇨ Enter quotation
- ⇨ Enter order with reference
- ⇨ Enter item

**Workflow**
1.  Select `Sales > Order entry` menu. The `Order entry` dialog opens.
2.  `Order` field: jump to the `Customer` field with `<Enter>`. The next free document number is entered in the `Order` field.
3.  Enter or select customer number.
4.  Go through the following fields with `<Enter>` and check them.
5.  `Reference` field: if necessary, select quotation with `<F9>` or enter number.
6.  `Date` field: enter possible delivery date if necessary. Alternative: the delivery date is determined and written back by `A+W Production`.
7.  `Route` field: check standard route from the customer master data and change if necessary.
8.  Check and add data in the other fields.
9.  `Project` field: if necessary, select project number or enter number.
10. Save header data with `<Enter>`.

### Enter order with reference (SA 02-002)

*Image: Find Reference Document dialog*

**Goal of the action**
- Enter order with reference to quotation.
- Enter quotation with reference to earlier order.

**Requirements**
- Master data is entered completely.

**Additional info**
- A quotation with reference to an order is entered in the same way.
- ⇨ Search for document
- ⇨ Enter item

**Workflow**
1.  Select `Sales > Order entry` menu. The `Order entry` dialog opens.
2.  `Order` field: jump to the `Customer` field with `<Enter>`. The next free document number is entered in the `Order` field.
3.  Enter or select customer number.
4.  Go through the following fields with `<Enter>` and check them.
5.  `Reference` field: press `<F9>`. The `Find Reference Document` dialog opens.
6.  `Document` field: select `Quotation` entry with `<F9>` and start search.
7.  Mark quotation and take over.
8.  Confirm query for takeover of the data:
    - **[Yes]:** take over header and item data.
    - **[No]:** Only take over the header data.
9.  If necessary, confirm query about the discounts.
10. Check the remaining header data and add any additional data.
11. Check items and add if necessary.
12. Save order and close.

### Specify order type (SA 02-003)

*Image: Order types selection dialog*

**Goal of the action**
- Enter stock order.
- Enter top priority order.
- Enter redelivery as goodwill order.

**Requirements**
- Order entry is open.

**Additional info**
- All order types are entered the same way.
- Enter order without price display: `Sales > Entry w/o Prices`. The SA prices are calculated when the order is printed.
- ⇨ Send electronic invoice (e-invoicing)

**Workflow**
1.  Enter order header up to the `Reference` field.
2.  Select order to which the redelivery refers.
3.  Continue filling fields up to the `Receipt` field.
4.  `Receipt` field: `<Ctrl>+<F12>` Receipt. The `Receipt types` dialog opens.
5.  Select order type: e.g. `Free-of-charge order`. The `Free-of-charge order` dialog opens.
6.  Enter item and complete entry.
7.  Confirm reference to zero amount with [No].
8.  If necessary, select details for the complaint.
9.  Confirm and take over details with `<Enter>`.
10. Confirm queries.
11. Confirm query about completeness of the order with [Yes].
12. Confirm question about release with [Yes].

### Edit properties (SA 02-004)

*Image: Order entry Properties tab*

**Goal of the action**
- Edit dispatch information.
- Change invoice and print options for commercial papers.
- Change sales representative.

**Requirements**
- Order entry is open.
- Order is entered.

**Additional info**
- Changes to the fields `Delivery type` and `Direct delivery` influence the entire order and PO process.
- Changes to the invoice options can activate surcharges, e.g. rush order.
- ⇨ Changing payment options

**Workflow**
1.  Change to the `Properties` tab.
2.  Change data in the `User information` area, e.g.:
    - `Ordered by` field: change contact person at the customer.
    - `Order date` field: check date and change if necessary.
3.  Change data in the `Dispatch information` area, e.g.:
    - `Packaging type` field: select packaging type, e.g. `Box`.
    - `Rack loading` field: select sort sequence for packaging in boxes or on racks, e.g., `by Consignment`.
4.  Change print options for commercial papers, e.g.:
    - `Glazing` field: show price of the glazing, e.g. `Calculate in item`.
    - `Print item text` field: Y = print texts.
    - `Print shapes` field: Y = print shape sketch.
    - `Suppress item prices` field: Y = do not print item prices.
5.  Change to the order header with `<End>`.
6.  Continue entry or save and close order.

### Change shipping address (SA 02-005)

*Image: Order entry Addresses tab*

**Goal of the action**
- Enter shipping address for order.
- Take over new shipping address in master data.

**Requirements**
- Order entry is open.
- Order header is entered.

**Additional info**
- Changes only affect the current order.

**Workflow**
1.  Change to the `Addresses` tab.
2.  Select address from master data: press `<Shift>+<F8>`. The addresses from the customer master data are displayed.
3.  Select and take over address.

**Search for address:**
4.  Start address search: press `<Ctrl>+<L>`. The `Address search` dialog opens.
5.  Search for and take over address.

**Enter alternative shipping address for the order.**
6.  Select `<F4> > Addresses > New Delivery Address`. The dialog for entry of the address data opens.
7.  Enter all required data.
8.  Take new address over into the order with [OK] and save.

**Take new address over into customer master data:**
9.  Enter new shipping address.
10. Start takeover with `<F3>` and confirm query.
11. Take new address over into the order with [OK] and save. The shipping address for the order is saved.
12. Continue entry or save and close order.

### Change delivery plan (SA 02-007)

*Image: Delivery plan dialog*

**Goal of the action**
- Specify delivery date for item and total quantity.
- Create delivery plan for partial deliveries of an item.

**Requirements**
- Order entry is open.
- Customer allows partial delivery.

**Additional info**
- Delivery notes are created in the dispatch planning depending on the configuration.

**Workflow**
1.  Order: select `<F4> > Delivery plan`. The `Delivery plan` dialog opens.
2.  `Delivery date` field: specify delivery date.
3.  `Route` field: select alternative route if necessary.
4.  Repeat steps for all items.
5.  Save changes with [OK].

**Partial delivery of an item:**
6.  `Planned` field: specify partial quantity. A new line with the remaining quantity is inserted.
7.  `Delivery date` field: specify delivery date for remaining quantity.
8.  `Route` field: select route for remaining quantity if necessary.
9.  Save changes with [OK].

**Next step:** create delivery note and plan dispatch

### Changing payment options (SA 02-006)

*Image: Order entry Miscellaneous tab*

**Goal of the action**
- Change payment options.

**Requirements**
- Order entry is open.
- Order header is entered.

**Additional info**
- The payment options are pre-populated with the data from the customer master data.
- Changes only affect the current order.

**Workflow**
1.  Change to the `Miscellaneous` tab.
2.  Enter data for complaint in the `Complaint information` area, e.g.:
    - `Type` field: select complaint type, e.g. `Packaging`.
    - `Location` field: select complaint location, e.g. `Load`.
3.  Enter data for payment mode in the `Payment options` area, e.g.:
    - `Payment term` field: enter number of days until due, e.g. 30 days.
    - `Cash discount 1, 2, 3` fields: select cash discount rates for scaled payment terms.
    - `Property, Payment term` fields: select type and manner of payment, e.g. `Bank debit`.
4.  `Details of the delivery` area: if necessary, select date of the goods receipt from purchasing.
5.  Change to the order header with `<End>`.
6.  Continue entry or save and close order.

**Next step:** Enter item

### Release order (SA 02-008)

*Image: Order release and Locking reasons dialogs*

**Goal of the action**
- Release orders of a department and/or a user.
- Release all orders.
- Check reasons for lock.

**Requirements**
- User rights are granted.
- Order is in the release pool.

**Additional info**
N/A

**Workflow**
1.  Select menu `Sales > Release order > Release`. The `Order release` dialog opens.
2.  Select selection criteria, e.g. department or user.
3.  Trigger search with [Start]. List of the orders is displayed.
4.  `Free` field: select YES.
5.  Select field `LSp`: Y.
6.  Trigger change with `<F3>`.

**Release series of orders:**
7.  Select first order starting with which all should be released: press `<Shift>+<F9>`.

**Release all orders:**
8.  Press `<Ctrl>+<F9>`.
9.  Confirm queries with [Yes].

**Check lock reasons:**
10. Mark non-released order.
11. Click [Lock list]. The `Blockage reasons for unsuccessful release` dialog is displayed.

### Show order information (SA 02-009)

*Image: Document info dialog showing production status*

**Goal of the action**
- Check production status of the order.
- Check delivery date changes.

**Requirements**
N/A

**Additional info**
- ⇨ Search for document

**Workflow**
1.  Select `Sales > Order entry` menu. The `Order entry` dialog opens.
2.  `Order` field: press `<F9>`. The `Find Orders` dialog opens.
3.  Search for order:
    - `Orders starting with` field: specify start number.
    - `Customer` field: specify customer number.
4.  Start search with `<F3>` and take over order from hit list.
5.  `Quantity` field: press `<Shift>+<F10>`. The `Order information` dialog opens.

### Edit text in order (SA 02-010)

*Image: Text editing dialog for an order item*

**Goal of the action**
- Enter internal header or footer text for the order.
- Edit article and item text.

**Requirements**
- Order entry is open.
- Item is entered completely.

**Additional info**
- Texts can be saved as text modules.
- Texts are displayed in the customer's language.
- Enter article or item text: press `<F5>` in the price field.
- Enter spacer, shape texts, product codes: `<F4> > Texts > Special texts`.

**Workflow**
1.  Cursor in order header or in order footer.
2.  Call up text entry: `<F4> > Texts > Header text` or `Footer text`. The `Texts` dialog opens.
3.  Select tab.
4.  Enter text freely and take over with [OK].

**Use text modules:**
5.  Use text module: `[Phrases] > Enter code > [OK]`.
6.  Select text module: `[Phrases] > Start search > Mark text module > [Adopt]`.
7.  `Forms` area: mark checkboxes of the forms on which the text should be printed.
8.  Confirm text with [OK].

**Check article text:**
9.  Press `<F5>` in price field. The `Texts` dialog opens.
10. Check entries.

### Editing notes (SA 02-011)

*Image: Notes dialog for an order*

**Goal of the action**
- Enter internal remark about the order header or footer.
- Enter internal remark about the item or article.

**Requirements**
- Document is open.
- Notes: are stored in the master data if necessary.

**Additional info**
- Notes are only displayed automatically if there is at least one line with the priority high.
- Notes from the master data are also displayed in the order with `<Shift> + <F4>`:

**Workflow**
1.  Cursor in the order header or footer: select `<Shift>+<F4> > Notes > Document notes`. The `Notes` dialog opens.
2.  Enter note.
3.  [Priority]: select priority high.
4.  Save note with [OK] and take over.
5.  Save order.

**Enter internal remark about the item or article:**
6.  `Items` tab: select `General > <Shift>+<F4> > Notes > Article notes`.
7.  Repeat steps 2 through 4.
8.  Save changes.

### Attach file (SA 01-012)

*Image: Allocation of Document Types dialog*

**Goal of the action**
- Attach document for the customer.
- Attach document for the item.

**Requirements**
- Document path must be set up.
- File must be available.
- Selection of the forms must be configured.

**Additional info**
- [Delete]: delete document allocation.
- [Reactivate]: restore document allocation.
- [Sever link]: only for orders that are entered with reference; for severing the link to the document path.

**Workflow**
1.  `Sales > Open document` menu.
2.  `Receipt` field, `Invoice type` field, `Project` field: press `<Ctrl>+<K>`. The `Allocation of document types` field is displayed.
3.  `DocType` field: select document type and use `<Tab>` to jump to `File` field.
4.  Search for file in Windows Explorer.
5.  Drag file to folder symbol on the `Allocation of Document Types` dialog and let it drop. File name is displayed in the `File` field; folder symbol changes to the `Document` symbol.
6.  `Forms` field: press `<F9>` and select form.
7.  Transfer document to production: Mark checkbox in `Prod` field with `<Blank>` or remove marking.
8.  Confirm allocation with [OK].

**Attach document for the item:**
9.  `General` tab: mark item.
10. Press `<Ctrl>+<K>`.
11. Repeat steps 3 through 8.
12. Save.

## Order item

| Help Card | Topics |
| :--- | :--- |
| **Enter item** | Enter order item. Add items. |
| **Edit supplier** | Change supplier. Change supply type. |
| **Exchange glass** | Change glass in product structure. Change assembly position of glass. |
| **Shape input** | Enter order item with shape. |
| **Enter processing step** | Enter processing manually. |
| **Adopt processing from SN file** | Take over processings from SN file in BOM. |
| **Add SN file** | Take over processings from SN file in BOM. Attach copy of SN file. |
| **Synchronizing changes with SN file** | Change or add processings in attached SN file. Change or add processings in BOM. |
| **Enter item in CAD** | Enter geometry and processings in A+W CAD Designer (Shapes), take over into item, and save as SN file. Interactive entry in A+W CAD Designer (Shapes). |
| **Enter stepped glass** | Enter stepping on multiple lite. |
| **Enter muntins** | Enter muntin structure. |
| **Edit muntin structure** | Edit muntin pattern with the muntin editor. Enter asymmetrical muntin structure. |
| **Edge clearance and sealing depth** | Enter edge clearance and sealing depth on IG lites. |
| **Enter edge stripping** | Enter edge stripping. |
| **Replace product** | Replace article in several order items. Edit lite structure in several order items. |
| **Fix product** | Fix article or order item. Take over fixed article into the master data. |
| **Allocate declaration of performance** | Check or allocate declaration of performance. |
| **Enter technical values** | Enter technical values. Generate new declaration of performance. |

### Enter item (SA 03-001)

*Image: Order entry dialog with focus on item entry*

**Goal of the action**
- Enter order item.
- Add items after the fact.

**Requirements**
- Article master data is present.
- Order entry is open.
- Order header is entered.

**Additional info**
- ⇨ Edit supplier
- ⇨ Enter stepped glass
- ⇨ Shape input
- ⇨ Enter muntins
- ⇨ Enter processing step

**Workflow**
1.  Use `<Enter>` to change from the order header to the `Items > General` tab.
2.  Select `Article` field: select article:
    - Enter article number.
    - Start article search with `<F9>`.
    Depending on the article data, various input fields are displayed.
3.  Enter quantity and jump to the next field with `<Enter>`.
4.  Enter dimensions or if necessary, select variant. For IG glass, also specify the dimension for the spacer (SZR).
5.  If necessary, change the commission rate in the `Comm:` field with `<F9>`.
6.  Check the field `S.Type`: supply type and change if necessary. The values for the fields `QU/pc`, `kg/pc` and the prices are calculated and filled.
7.  Add another item:
    - Insert at the end: press `<F6>`.
    - Insert over marked items: press `<Shift>+<F6>`.
    - Copy item: mark item and `<Alt>+<C>` or [Copy item].
    When entering an item with the same article number, the BOM structure is taken over.
8.  Complete entry in `Price` field:
    - Use `<End>` to save the order and check the footer data.
    - `<F2>`: change to the order header.
9.  Continue entry or save and close order.

