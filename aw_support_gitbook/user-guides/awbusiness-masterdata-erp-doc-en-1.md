---
title: "A+W Business Master Data Reference"
source: "EN_AWBusiness_Master_Data_9_11-2.pdf"
tags: ["A+W Business", "Master Data", "Software Reference", "ERP", "Formulas", "Interface Service", "Customizing", "Forms Management", "Production Reports"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A reference guide for managing Master Data in the A+W Business software, covering formulas, interface services, customization, text management, and form management."
long_description: "This document is a detailed software reference manual for the A+W Business Master Data module. It provides comprehensive instructions and explanations for various configuration and management tasks. Key sections include: **Formulas**, which details the creation and management of formulas for task automation; **Interface Service**, which explains how to define interfaces for data exchange with A+W Production and other programs, including settings for production formats, scheduling, barcode reports, and financial accounting data; **Customizing**, which describes how to adjust A+W Business functions to specific company requirements; **Data Container**, for managing customizing data; **Text Management**, which covers the creation and use of text codes, standard texts, system texts, and reminder texts for documents; and **Forms Management**, which details the configuration of print forms, headers, footers, and other print-related settings. The guide is intended for administrators and advanced users responsible for setting up and maintaining the A+W Business system."
---

---
## Formulas

**Master Data > Company > Formulas**

[Image: Fig. B-267 Formula management showing two formula dialog windows.]

This dialog contains all formulas that can be used for automating certain tasks in A+W Business. Tab **Formula** shows the syntax of the formula selected on tab **Table**.

> **i**
>
> **Adding or editing a formula**
> If you need more formulas or a formula needs to be amended please contact A+W Software GmbH.

**Options menu**

This menu can be used to enable the formula check during input. You will be notified of any errors occurred when you save your entries.

## Interface service

**Master Data > Company > Interface Service**

Use this dialog to define the interfaces to be used for exchanging data between A+W Business and other programs.

Dialog Interface Service offers the following tabs:
- Interface Service - Settings for A+W Production Formats
- Interface Service – Settings for other formats
- Interface Service - Options

### Interface Service – Settings for A+W Production Formats

**Master Data > Company > Interface Service > Settings for A+W Production formats tab**

[Image: Fig. B-268 Production reports - Settings for A+W Production formats.]

This tab is used for selecting the reports you want to receive and import from A+W Production in file format.

If you are using STSP-, STSL-, STSD-, STSB-, STSG files for the reports you have to select a registration point in section **Order produced at** that is allocated to a status point. If such a registration point was not assigned, the report generates an error.

> **i**
>
> Registration points are entered in dialog **Production registration points**.
> ⇨ "Registration Points - Production" on page B-869
>
> **Locked fields**
> The fields are locked if the checkbox **Import of production reports** is active on the **Settings of further formats** tab. In this case, you cannot make any settings for A+W Production formats.

**Identification**

**Settings for** Employee to whom the settings should apply. If the settings are to be valid for all users, please select the entry **Administrator**. With this settings, you have to select the same registration point in section **Order produced at** as defined in Company data > tab **Stock/PCH/EDI**.

**A+W Production formats**

This is where you can select the reports to be loaded from A+W Production. The directory for the report file can be entered in the following field. The same directories have to be entered in A+W Production to make sure that the files are saved correctly. The files are imported by A+W Commercial Exchange Service.

**Import of production reports** STSP reports are mainly made by piece. For the registration point in question you can define whether the status should be raised with the first lite or only when all lites of the order have been reported.

- [ ] Report files from the shop floor will not be imported.
- [x] The report from the shop floor is sent as a STSP file. The order status, production date, and the header or item number will be updated.

**Production release for order if sub-order has been produced** This field is accessible only if production reports are imported.
Partial orders can be created for an order. If a production report refers to such a sub-order, the status of the whole order can be changed.

- [ ] An order is not automatically set to the Production release status.
- [x] When the sub-orders are reported as produced, the status of the main order is automatically raised to Production release.

**Adopt batch no. from order header** This field is accessible only if production reports are imported.
If the defined registration point has no status allocated, the report is processed by A+W Business capacity planning, and the status is changed accordingly.

- [ ] The batch numbers of the items are updated separately from the batch number in the order header.
- [x] After the order header has been updated, all items with an item status over/equal with the status of the registration point produced will get the order number's batch number.
⇨ "Reg. point allocation" on page B-961

**Import scheduling reports** The STSL data of rough and detailed scheduling can be imported from production. If the defined registration point has no status allocated, the report is processed by capacity planning, and the status is changed accordingly.

- [ ] Reports from rough and detailed scheduling will not be imported.
- [x] Reports from rough and detailed scheduling will be imported. The order status will be raised according to the defined registration point. The registration points for capacity planning (time management) have to be defined in section Options for this purpose.
⇨ "Registration Points - Production" on page B-869

**Import barcode reports** The STSD report from shop floor data collection (barcoding) serves for to update the order status, the production date, and the header and/or item number in A+W Business.
Reports are made mainly by piece. You can define whether the status should be raised with the first lite or only when all lites of the order have been reported.
If the defined registration point has no status allocated, the report is processed by capacity planning, and the status is changed accordingly. The registration points for capacity planning (time management) have to be defined in section Options for this purpose.

- [ ] Barcode reports will not be imported.
- [x] Barcode reports will be sent as STSD files.

**Adopt production rack number for item** This field is accessible only in connection with the import of barcode reports.
If the barcode report includes rack numbers of items, these can be allocated to the items in A+W Business.

- [ ] Rack numbers will not be adopted for the item.
- [x] The reported rack numbers will be saved in the order and allocated to the corresponding item.

**Import rack allocation reports** The STSG report defines the rack that is allocated to the corresponding order item and the quantities produced. The rack number is printed on the delivery note.

- [ ] Rack allocation reports will not be imported.
- [x] The rack allocation report is sent as a STSG file.

> **i**
>
> **Rack report for partial delivery**
> For partial deliveries, the quantity of the partial delivery item can be determined based on the quantity reported by the STSG file as having been packed. To do this you have to check the option **Partial delivery qty. > Take rack report into account for partial deliveries when copying the order**.
> The quantity of the partial delivery item is preset by the total quantity from the STSG reports for the corresponding order item in this case. It cannot be changed.

**Update production list through registration point** This field is accessible only in connection with the import of rack allocation reports.
In this field, choose the registration point used by the rack reports to raise the status. Based on the selected registration point, the production list in dialog **List of status reports** will be updated.
⇨ Sales, "Status Message Overview" on page C-574

**Import rack receipt/exit reports** The STSK report specifies the rack status and the dates on which the rack was received/shipped.

- [ ] Reports on the receipt and shipping of racks will not be imported.
- [x] Reports on racks received and shipped will be imported. After checking whether customer and rack do exist, shipment or return of the rack will be booked. If the rack does not exist in A+W Business yet, it will be entered as type <n.e>.

**Import breakage reports** The STSB report is used for reporting complaints and the lites broken on the shop floor. A+W Business can automatically turn these into complaint orders.
If the defined registration point has no status allocated, the report is processed by capacity planning, and the status is changed accordingly. The registration points for capacity planning (time management) have to be defined in section **Options** for this purpose.

- [ ] Breakage reports will not be imported.
- [x] The breakage report is sent as STSB file.

**Create complaint orders** This field is accessible only in connection with the import of breakage reports.

- [ ] Complaint orders will not be created automatically.
- [x] A complaint order will be automatically created based on a breakage report. This function can be allocated a standard cause and a standard reason which can be changed for the individual complaint order.

**Cause** This field is accessible only in connection with the automatic creation of complaint orders.
You can select a cause that is adopted for the automatically created complaint order. It will be loaded irrespective of the settings in **Company Data > Archives** tab.
⇨ "Default complaint place" on page B-966

**Reason** This field is accessible only in connection with the automatic creation of complaint orders.
You can select a reason that is adopted for the automatically created complaint order.

**Free** This checkbox is available only in connection with the automatic creation of complaint orders.

- [ ] Automatically created complaint orders are not free of charge as a standard.
- [x] Automatically created complaint orders are free of charge by default. The setting can be changed in the complaint order.

**Order area** This field is released only in connection with the automatic creation of complaint orders. You can select an order area: the order number will be taken from its number range.

**Target NM** This field is released only in connection with the automatic creation of complaint orders. You can select a number manager to which the automatically created complaint order should be transferred.

**Import XTV reports** XTV reports serve to withdraw the stock sizes to be cut for an order. For articles with stock mode combined, the sqm reservations will be deleted from the orders.

- [ ] XTV reports will not be imported.
- [x] The optimization report is sent as a PRODBDA* file.

#### Options

The fields in this section are available only if reports are imported for which further details can be entered.

**Allow qty. above item qty. in STSB, STSD, STSG, STSL, STSP** The shop floor can report larger quantities per item than stated in the order.

- [ ] Larger quantities per item are not permitted.
- [x] Reports can be processed even for larger quantities.

**Capacity planning processes STSD and STSB** STSD and STSB reports can be processed by capacity planning (time management).

- [ ] Capacity planning processes no data from STSD and STSB files.
- [x] Capacity planning will process STSD and STSB files.

**Registration point STSD** Registration point used to change the status if the STSD report is processed by capacity planning.

**Registration point STSB** Registration point used to change the status if the STSB report is processed by capacity planning.

#### Order produced at

To report an order completed, you have to enter a registration point for the reports.
If the settings should apply to all users you have to choose the same registration point as in dialog **Company data**.
⇨ "Company Data - Stock/Purchasing/EDI" on page B-955

**REGISTRATION POINT** Registration point that can trigger the following (additional) actions following a report:
- The production date and job number are raised in the order.
- For production orders, the receipt of goods on stock is booked.

### Interface Service – Settings for other formats

**Master Data > Company > Interface Service > Settings for other formats tab**

[Image: Fig. B-269 Production reports - Settings for other formats.]

From this tab choose the reports you want to receive and import from shop floor data collection (barcoding), from ALFERT, and from financial accounting.

#### Barcode and ALFERT formats

> **i**
>
> **Locked fields**
> The fields in section **Barcode and ALFERT formats** are locked if the checkbox **Import production reports** is checked on tab **Settings**. You will not be able to make any settings for barcode formats in this case.

**Import of production reports** Reports are made mainly by piece. You can define in A+W Business whether the status should be raised with the first lite or only after reports on all lites of an order have been made.

- [ ] Report files from the shop floor will not be imported.
- [x] Reports from production will be loaded from the AWB_STAT file.

**Adopt batch no. from order header** This field is accessible only if production reports are imported.
The batch number shown in the order header can be adopted for the items.

- [ ] The batch numbers of the items are updated separately from the batch number in the order header.
- [x] After the order header has been updated, all items with an item status over/equal with the status of the registration point produced will get the order number's batch number.

**Import rack report files** The AH_GEST.DAT report specifies the rack status and the dates on which the rack was received/shipped.

- [ ] Reports on the receipt and shipping of racks will not be imported.
- [x] Reports on the receipt and shipment of racks will be imported.

**Import AWPool files** The AWPool report updates the order status, production date, header and item number in A+W Business. Allocation of the AWPool status to an A+W Business status is predefined.

- [ ] AWPool reports will not be imported.
- [x] AWPool reports are imported as POOL*.DAT files. Field **Update production date from status** is accessible.

**Update production date from status** This field is accessible only in connection with the import of AWPool reports.

- [ ] The production date will not be updated in the order.
- [x] The production date will be updated in the order if one of the available statuses has been set.

#### Financial Accounting

You can use this section to make the settings for the reporting of receivables that are automatically imported by A+W Commercial Exchange Service (AIS).

**Import receivables reports** Receivables can be reported by the financial accounting program in file format. This only applies to the customer accounts.

- [ ] Receivables reports will not be imported.
- [x] Receivables reports are imported in file format. The fields for the storage place, a backup, and a batch file are made accessible.

**Create backup file** This field is accessible only in connection with the import of receivables reports. You can save an additional backup file and enter the number of days for which it is going to be saved.

- [ ] No backup file will be saved for the receivables report.
- [x] A backup file of the receivables reports (including a time stamp) will be saved elsewhere. The fields for selecting the directory and the storage days are made available.

**Storing days for backup files** This field is available only if a backup file is going to be saved. You can enter the number of days for which this file must remain unchanged.

**Batch file** Name of the batch file that is required for copying the files.

### Interface Service - Options

**Master Data > Company > Interface service > Options tab**

[Image: Fig. B-270 Production reports - Options.]

You can use this tab to define the intervals in which the program should search for new reports.

**Interval**

**Standard ... minute(s)** Interval for A+W Commercial Exchange Service (AIS). If you enter 2, for example, AIS will check whether there are new reports from Production every 2 minutes and, if so, import them.

**Receivables: Report** Interval for the receivables report. If you enter 120 for instance, new reports will be imported via batch every two hours.

Receivables reports can be imported only if the corresponding function is enabled on tab **Settings for other formats**.
The checkboxes for receivables reports must be checked in dialog **Company data** for this purpose.
⇨ "Company Data > Financial Accounting" on page B-923

**Settings for automatic email dispatch**

**Email dispatch** Emails from a specific sender can be automatically dispatched to a defined address.

- [ ] Emails will not be sent.
- [x] Emails will be sent. The fields will be enabled.

**Server** Name of the server controlling the dispatch of emails.

**Port** Number of the port for email dispatch.

**Sender address, Recipient address** Email addresses to be used by default.

**Authentication** An authentication can be used for data transfer.

- [ ] The transmission confirmation will not be sent without authentication.
- [x] The transmission confirmation requires authentication. The fields for entering the registration data are accessible.

**Use SSL encryption** Secure Sockets Layer (SSL); encryption program for safe data transfer in the Internet.

- [ ] The transmission confirmation will not be encoded.
- [x] The transmission confirmation will be encoded acc. to the SSL log.

**User, Password** Registration data the sender uses for authentication.

## Customizing

**Master Data > Company > Customizing**

[Image: Fig. B-271 Customizing.]

This dialog is used for adjusting A+W Business and its functions to your company's requirements.

You will only be able to open this dialog if you have been logged in as an administrator, with the appropriate rights.

> **i**
>
> **Customizing**
> Customizing may have far-reaching effects on the functions of A+W Business. To adjust A+W Business further to your company's needs please contact A+W Software GmbH to discuss and agree the required amendments.

## Data Container

**Master Data > Company > Data Container**

[Image: Fig. B-272 Customizing data - Data container.]

This dialog is used for managing data that is necessary for customizing in the A+W Business database. The names of the tabs and table columns can be configured as well.

## Text

**Master Data > Text**

This program section is used for managing text and text codes that are required for editing documents.

Menu **Text** offers the following entries:
- "Text Code" on page B-1039
- "Text" on page B-1040
- "System Text" on page B-1041
- "Reminder Text" on page B-1042
- "File Attachment Types" on page B-1043
- "File Attachment Remarks" on page B-1044
- "Technical Values" on page B-1044

### Text Code

**Master Data > Text > Text code**

[Image: Fig. B-273 Text identifier.]

This dialog is used for entering the text codes. Text codes serve for allocating text modules to subjects, e.g. P for production, D for delivery note, T for common text. Text codes can be used to define which text is to appear on the individual documents.
⇨ Tutorial 2, "Text Types" on page B-461

**Identifier** Text code, e.g. P for production text, D for postponed dates.

**Name** Name, e.g. **Production** for text to be transferred to production.

### Text

**Master Data > Text > Text**

[Image: Fig. B-274 Multilingual text.]

This dialog can be used for entering standard text that is frequently used, e.g. spacer text or text for postponements. The text can include wildcards which will be replaced by the actual values only when the document is printed.
⇨ Tutorial 2, "Text Codes and Standard Text" on page B-463

In case of multilingual operation, all text modules have to be entered in the corresponding language(s). Please make sure that the text numbers are not changed in the course of translation.
⇨ "Languages" on page B-554

**Language** Select the language in which the text should be printed.

**Number** Random number for the text. You should collect the text modules per text code in number ranges, e.g. 1-99 for invoices, 100-199 for quotations. If you are using module Multilingual operation, at least one text of number 0 must exist before you start entering text in a foreign language.

**Matchcode** Input of the matchcode is optional.

**Identifier** These text code is used for allocating the text for printing. By entering the code D for delivery note you can e. g. define in dialog **Forms** whether or not the text should be printed.

**Text type A+W Production** Item text will be transferred to production if the text code (P) for the transfer to production permits this. For those text modules you can enter the text type (external key) that is used in A+W Production for the text. If no text type has been entered, text type 1 will be transferred by default.

**Selection**
This list shows all text matching the selection criteria.

**Edit text**
**Buttons** You can change the font type and size and add hyperlinks, images and tables.
⇨ Tutorial, "Enter text" on page C-54

**(Input field)** Standard text or spacer text. You can use wildcards (variables) for spacer text and certain types of standard text.
⇨ Tutorial 2, "Text Input" on page B-469

### System Text

**Master Data > Text > System text**

[Image: Fig. B-275 System Text.]

This dialog is used for maintaining the system text. This text modules have fixed lines in the dialogs and in the forms. They can be changed (without falsifying the sense) e.g. for another language.
⇨ Tutorial 2, "System Text" on page B-461

> **i**
>
> **Do not delete text**
> Logical changes can be made to the system text. System text cannot be deleted however, nor can you add new system text. Wildcards (variables) can be moved to another position in the text.

**Language** Select the language in which the text should be printed.

**Number** Shows the text number.

**Edit text** You can edit the system text, e.g. translate it into another language.

**Selection**
The list shows the numbers of the system text modules.

### Reminder Text

**Master Data > Text > Reminder text**

[Image: Fig. B-276 Reminder Text.]

You can use this dialog to enter the text to be used for reminders. This text only serves for information.
⇨ Sales, "Reminding" on page C-731

**Name** Name of the reminder text.

**External key** External key for communicating with other programs, e.g. for transfer to financial accounting.

**Locked** Reminder text can be locked for document input if it is no longer required.

- [ ] The reminder text can be allocated.
- [x] The reminder text is locked and cannot be assigned. If it has been assigned before in a document, it will still be shown and printed however.

### File Attachment Types

**Master Data > Text > File attachment types**

[Image: Fig. B-277 File attachment types.]

Use this dialog for entering the codes for file attachments. By default, all attachments are marked as type A (all) and will always be transferred except at transfer to purchasing.
The codes can be used to control the transfer of the attached files (documents, images):

- **Transfer to production:**
  File attachments for transfer in OrderXML, e. g. product information.
  ⇨ Production, "Settings for Transfer to Production - Text/Attachments" on page E-185
- **Copy documents:**
  Quotation to order, e. g. calculation information.
  ⇨ Sales, "Copy documents - Text/Attachments" on page C-545
- **P.O. transfer, e.g. product information.**
  ⇨ Sales, "Further Settings - General" on page C-664

### File Attachment Remarks

**Master Data > Text > File attachment remarks**

[Image: Fig. B-278 Remarks for file attachments.]

On this dialog, you store standard remarks that are used very frequently. These standard remarks are offered for selection on the **Order entry > Details** tab.
⇨ Sales, "Header data - Attachments" on page C-433

### Technical Values

**Master Data > Text > Technical Values**

[Image: Fig. B-279 Texts for the technical values for declarations of performance.]

On this dialog, you store the technical values for the generation of declarations of performance.
The texts must be entered for each language so that declarations of performance can be generated with the appropriate translation of the characteristics into the appropriate language.
This information is not required if the user already has finished declarations of performance.

## Forms

**Master Data > Forms**

Forms can be printed or displayed on screen. Apart from documents, these can lists and reports.

Menu **Forms** offers the following entries:
- "Form Management” on page B-1045
- "Order Forms" on page B-1061
- "Print Jobs" on page B-1062
- "Crystal Reports" on page B-1068

### Form Management

**Master Data > Forms > Form Management**

Management of forms allows to edit the general settings for printing forms. The forms themselves can only be changed by A+W Software GmbH.

Dialog **Management of Forms** offers the following tabs:
- Form Management - Form
- Form Management - Headers/Footers
- Form Management – Text
- Form Management – Options 1
- Form Management – Options 2
- Form Management – Sketch Printing
- Form Management – Customizing

The settings are used for printing, e.g. order confirmations.
⇨ Sales, "Form/Label Printing" on page C-638

> **i**
>
> **Connection to the Algeier scanView DMS system**
> During the printing process, a PDF file can be created from the current document and transferred for DMS archiving to the Allgeier scanView system. This functionality can be used even across sites. Contact A+W Software GmbH if you want to use this functionality.

### Form Management - Form

**Master Data > Forms > Form Management > Form tab**

[Image: Fig. B-280 Form Management - Form.]

This tab serves to define the forms to be used for the individual print items. The print item is the status point used by the program internally.
⇨ "Status Allocation" on page B-886

**Print points**

Choose an option to define whether you want to view or change customer or supplier forms.
- **Standard:**
  The forms are generally valid.
- **Customers, Suppliers:**
  The forms are valid just for a customer or a supplier. The field for selecting the partner is accessible.

**Print point** Print point allocated to a form. A print point can be allocated to any number of forms.
Once a form has been entered and the print point allocated, the print point cannot be changed in the form.
If e.g. an order confirmation with print point 100-Print OC is printed, the order automatically gets the user status 21.

**Form settings**

**Name** (Internal) name of the form.

**Quantity** Number of copies to be printed. Each page of the form will be printed several times. The number of copies is entered on tab **Options 1**.

**Standard** If your company uses different forms for printing a document you have to define which of them will be used by default.

- [ ] The form will not be used by default.
- [x] This form will be used by default when you start printing, e. g. an order confirmation for a certain customer.

**Language** Language allocated to the selected form. An appropriate form must be defined for every language. This function is active only if the multi-lingual version of A+W Business has been installed.
A language is assigned to every customer, and all related documents. When a document is printed, the system checks the language code and uses the appropriate form. The text will be printed in the correct language.

**Change document language** This setting can be used to change the language defined in field **Language**.

- [ ] The form is printed in the selected language (standard setting).
- [x] The selected language will be changed. Check the checkbox if a form is used as a production paper for instance. In this case, the production papers have to be printed in your national language (irrespective of the document's language code).

**Report**

**File Name** Allocate the form to a report file. Without this allocation, reports cannot be created.
Examples of allocations used by default in A+W Business:
- Quotation = ANGEB.QRP
- Order confirmation = AUFTRAG.QRP
- Delivery note = LIEFER.QRP
- Invoice = RECHN.QRP
- Credit note = GUTSCH.QRP
- PO request = ANFRAGE.QRP
- P.O. = BESTELL.QRP

**Print service report** Selection of the printer with which the report will be created.
For declarations of performance, for example, the value **006 - Declaration of Performance** must be entered together with the appropriate language for the report. In addition, the transfer to the DMS system can be activated.
⇨ "Archiving of documents" on page B-1054

**Transfer to iQuote** Forms output can also be transferred to iQuote.

- [ ] The printed form is not transferred to iQuote.
- [x] The printed form is transferred to iQuote.

**Other form status**

**Status point** Each form can be assigned a different status item. This is usually only necessary for cash sale forms. In this case, select the status point **Cash sale**.
A cash sale invoice is generally printed for cash sales. The customer pays in cash. No invoice must be issued for this kind of orders; the amount received must not be transferred to financial accounting.
If there is no status item for cash sale in your system, please create it only after checking with A+W Software GmbH.

**Declaration of performance**

**Send by email** You can specify when a declaration of performance should be dispatched.

- [ ] No declaration of performance will be dispatched when the selected form is printed.
- [x] When the selected form is printed, a declaration of performance will be emailed automatically.

**Forms**
The list shows all forms matching the selection criteria.

### Form Management - Headers/Footers

**Master Data > Forms > Form management > Headers/footers tab**

[Image: Fig. B-281 Form Management - Headers/Footers.]

This tab is used for selecting the text always to be printed on the form in question, e. g. if you want to appear information regarding your next company holidays on all your order confirmations.

> **i**
>
> **Prerequisite**
> The appropriate text must be entered in dialog **Text**.

The fields in the section **Forms** are explained in connection with tab **Forms**.
⇨ "Form Management - Form" on page B-1046

**Text**

Use the zoom icon to select one of the existing text modules for every header and footer.
⇨ "Text" on page B-1040

**Header** The selected text will appear on the form header.

**Footer** The selected text will appear on the form footer.

### Form Management – Text

**Master Data > Forms > Form Management > Text tab**

[Image: Fig. B-282 Form Management – Text.]

Enter all differences from standard printing.
The fields in the sections **Print items** and **Forms** are explained in connection with tab **Forms**.
⇨ "Form Management - Form" on page B-1046

**Text not to be printed** Codes of the text modules that should not appear on the selected form. An order confirmation e.g. should not include text with the text code D (delivery note) and P (production).
This setting always refers to all text modules of the selected text code. To exclude certain text modules from printing, enter them in field **Variable Text**.
⇨ "Text Code" on page B-1039

**Variable text** Up to ten variable text modules can be managed per form. This text can be used at random on forms, e.g. as an alternative header. The settings can be especially used for supplier- and customer-specific text. The text has to be defined in text management.
