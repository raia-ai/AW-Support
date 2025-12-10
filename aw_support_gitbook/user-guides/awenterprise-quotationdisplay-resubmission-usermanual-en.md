---
title: "EN-UM-AW_Enterprise-Sales_4_9"
source: "EN-UM-AW_Enterprise-Sales_4_9.pdf"
tags: ["A+W Enterprise Sales", "Quotation Display", "Resubmission", "Completion Report", "Document Change", "Order Management", "Sales Software", "ERP", "Software Reference", "Technical Documentation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical reference for the A+W Enterprise Sales software, detailing the functionality of various dialogs and overviews within the 'Sales' and 'Overview' modules. It covers informational displays like the Quotation Display, task management features such as Resubmission, and operational processes like the Completion Report and bulk Document Change."
long_description: "This software reference manual provides detailed instructions and field descriptions for several key features within the A+W Enterprise Sales application. The document is structured to guide users through specific user interface dialogs. It begins with the 'Quotation Display,' explaining its read-only nature for informational purposes. It then moves to 'Resubmission,' a feature for creating reminders and follow-up tasks related to documents, detailing different resubmission types and associated fields. The 'Completion Report' section describes how to mark order items as complete, outlining the fields in the header, overview, and footer of the dialog. The 'Document Change' feature is explained as a tool for simultaneously correcting multiple documents, with a comprehensive breakdown of its two-view table and all associated fields for batch updates. Finally, the 'Overview of Documents' section details how to access various lists, such as 'Orders not Invoiced' and 'Incomplete Deliveries.' Throughout the manual, navigation paths, technical field information (DB fields), and keyboard shortcuts are provided to assist users. The document is intended for trained users of the A+W Enterprise system."
---

---
## Quotation Display

The data on the **Order Display** dialog serves only informational purposes. You cannot call up all order functions and you cannot edit the entries.

The tabs and fields are described for the Order Entry dialog:
> ⇨ "Order Entry" on page D-84

### Sales > Overview > Quotation Display

[Image: Fig. D-176 Quotation Display screen showing customer, item, and pricing details for a quotation.]

**Fig. D-176: Quotation Display**

Use this dialog to open a quotation in display mode. You can open a quotation in display mode at any time, e.g. even if the quotation is locked by a background process or is being edited by another user.

The data on the **Quotation Display** dialog serves only informational purposes. You cannot call up all quotation functions and you cannot edit the entries.

The tabs and fields are described for the Order Entry dialog:
> ⇨ "Order Entry" on page D-84

## Resubmission

### Sales > Resubmission
### Sales > Document Entry > Header, Footer area, Item level > <F4> > Resubmission

[Image: Fig. D-177 Resubmission dialog showing presentation date, type, and employee assignment.]

**Fig. D-177: Resubmission**

Use this dialog to enter processing remarks for a resubmission. When the resubmission date has arrived, a message will be displayed for the selected employee at the program start or a reminder e-mail sent.

You can create process-free resubmissions without any reference to a document.

You can only create document-related resubmissions if you enter a quotation with a delivery date. These resubmissions are always related to a business process.

-   Use `<F6>` to create additional resubmissions.
-   Use `<F7>` to delete individual resubmissions.
-   Use `<End>` to save the resubmission and close the dialog.

**Present.Dat**
Submission date when a reminder about the document is issued. Depending on the system configuration, the resubmission can also be displayed automatically or if particular conditions are fulfilled.
*Technical info: mandatory field, date field, DB field: vorlage.vldat*

**Present.type**
Type of resubmission.
-   **Memo in message system:**
    The message system will transfer memos to the user. Use `<Ctrl>+<F4>` to retrieve messages in the mail system. If you are working with an external mail program, the system can be configured so that you can also call up the mails via the corresponding program. If an e-mail address is stored, the message recipient will be sent an external e-mail.
-   **Active resubmission:**
    All messages are displayed on the screen when you start the program.
-   **Direct deletion of the document:**
    This function is only authorized for customer quotations and requests for quotations to suppliers. Thus, the resubmission for the document when the document date is reached is cancelled.
    *Technical info: toggle field, DB field: vorlage.modus*

**Present to (employee)**
Number of the employee who will receive the resubmission. By default, the individual entering the document is preset here. If you specify a number, the name of the employee is displayed in plain text.
*Technical info: numeric field, DB field: vorlage.outmanr*

**Text fields**
Fields for information texts about the document that are displayed at the time of resubmission. If you enter a document-related resubmission, the number of the quotation is displayed next to the first text field.
*Technical info: alphanumeric fields, DB fields: vorlage.text1, vorlage.text2*

## Completion Report

### Sales > Completion Report

[Image: Fig. D-178 Completion Report dialog showing a list of order items with total, completed, and remaining quantities.]

**Fig. D-178: Completion Report**

Use this dialog to report items for an order complete.

As a rule, completion reports are made from production or purchasing and do not have to be transmitted manually.

-   Use `<F5>` to delete the items whose total item quantity is already reported complete. For these items, the `Compl.` field is empty.
-   Use `<F3>` to book the completion report.

### Header

**Site**
Display of the site number.
*Technical info: display field, DB field: kauf.hausnr*

**Order**
Order number.
*Technical info: mandatory field, numeric field, DB field: kauf.auftrnr*

**Dept.**
Number of the department of the person who entered the order.
*Technical info: numeric field, DB field: kauf.abtnr*

**Deliv. Date**
Planned delivery date of the order.
*Technical info: display field, DB field: kauf.ltplan*

**Completion Report**
Date in the format DD.MM.YYYY on which the order should be reported complete. By default, the current date is pre-set.
*Technical info: mandatory field, date field, DB field: kauf.bdat*

### Overview

-   **Order:**
    Order number.
    *Technical info: display field, DB field: kauf.auftrnr*
-   **Itm:**
    Item number in the order.
    *Technical info: display field, DB field: kpos.posnr*
-   **Article:**
    Description of the article from the selected item.
    *Technical info: display field, DB field: kpos.artnr, kpos.artbez1*
-   **Total:**
    Total item quantity.
    *Technical info: display field, DB field: kpos.menge*
-   **So far:**
    Quantity of the item already reported complete.
    *Technical info: display field, DB field:*
-   **Compl.:**
    Quantity of the item that should be reported complete. By default, the difference of the total quantity of the item and the quantity previously reported complete is specified. You can edit the quantity that should be reported complete.
    *Technical info: numeric field, DB field:*

### Footer

[Image: Book and Cancel buttons]

**Book**
Books the completion report.

**Cancel**
Cancels the completion report.

## Document Change

### Sales > Document Change

[Image: Fig. D-179 Document Change dialog showing two different table views for altering multiple documents simultaneously.]

**Fig. D-179: Document Change**

Use this dialog to correct several documents simultaneously. The documents can be corrected faster than on other dialogs since no time is required to load an entire document. You cannot make corrections go documents at any time; they depend on the item status.
> ⇨ "Item status and item identifier" on page D-79

The dialog has a second view on which additional columns of the table are displayed.

-   Use `<F2>` to change between the two views on the dialog.
-   Use `<Ctrl>+<F10>` to search for documents with declarations of performance for a delivery date. All documents with declarations of performance for the delivery date searched for are displayed.
-   Use `<Ctrl>+<F11>` to mark all records starting with the current one.
-   Use `<Ctrl>+<F8>` to import the data for the document change. The data is imported via a freely configurable WQL query. The amount of data imported depends on the SQL query in question.
-   Use `<F5>` to display additional information about the document if any is stored.
-   Use `<F3>` to trigger the booking of the corrections.
-   Use `<Shift>+<F5>` to change to order entry.
    > ⇨ "Order Entry" on page D-84

### Table

**Document:**
Document type.
-   Order
-   Deliv.: Delivery
-   Quot.: quotation
*Technical info: toggle field, DB field: zuaufint.vorgang*

**Number:**
Document number.
*Technical info: numeric field, DB field: zuaufint.auftrnr*

**SubNo:**
Subnumber of the document.
*Technical info: display field, DB field: zuaufint.subr*

**Info:**
Indication whether there is additional information about the document.
-   (blank): There is no additional information
-   /: There is additional information.
*Technical info: display field, toggle field*

**Local Correct.:**
Information as to whether the document is in local correction status. The notice is only displayed if the document is in this status. The field is locked.
*Technical info: display field, DB field:*

**Ccl:**
Cancellation. Specification whether the document should be cancelled.
-   ☑ The document will be cancelled.
-   ☐ The document will not be cancelled.
*Technical info: checkbox, DB field: zuaufint.storno*

**Site:**
Site number that is assigned to the document.
*Technical info: mandatory field, numeric field, DB field: zuaufint.hnr*

**Route:**
Number of the shipping route.
*Technical info: mandatory field, numeric field, DB field: zuaufint.route*

**Date:**
Date of the planned delivery in the format DD.MM.YYYY.
*Technical info: date field, DB field: zuaufint.ltidea*

**PMS:**
Specification whether the document should be transferred to the production management system. The specification is only valid if the production management system is used.
-   ☑ The document will be transferred to the production management system.
-   ☐ The document will not be transferred.
*Technical info: checkbox, DB field: zuaufint.pmsflag*

**Dsp:**
Dispatch control. Specification whether the document should be transferred to the document control.
-   ☑ The document is transferred to the document control.
-   ☐ The document will not be transferred.
*Technical info: checkbox, DB field: zuaufint.lapoolflag*

**Txt.:**
Specification whether the texts for the document should be generated anew.
-   ☑ The system will generate the texts anew.
-   ☐ The system will not generate the texts anew.
*Technical info: checkbox, DB field: zuaufint.txtflag*

**PGr:**
Specification whether the product group assignment for the document should be created anew.
-   ☑ The assignment will be updated for the document.
-   ☐ The assignment for the document will not be updated.
*Technical info: checkbox, DB field: zuaufint.wgrpflag*

**Rel.:**
Specification whether the document should be released.
-   ☑ The document will be released.
-   ☐ The document will not be released.
*Technical info: checkbox, DB field: kauf.tekapkz*

### Additional Fields (via <F2>)
Use `<F2>` to display the following additional fields on the **Document Change** dialog:

-   **Order:**
    Document number.
    *Technical info: mandatory field, numeric field, DB field: zuaufint.auftrnr*
-   **Disp. Type:**
    Number of the dispatch type.
    *Technical info: numeric field, DB field: zuaufint.sfill1*
-   **Deliv. type:**
    Number of the delivery type.
    *Technical info: numeric field, DB field: zuaufint.sfill2*
-   **DepCusto:**
    Code number of the outgoing customs office.
    *Technical info: numeric field, DB field: zuaufint.sfill3*
-   **DesCusto:**
    Code number of the destination customs office.
    *Technical info: numeric field, DB field: zuaufint.Ifill1*
-   **Disp. Info:**
    Company-internal information text about the dispatch.
    *Technical info: alphanumeric field, DB field: zuaufint.cfill1*
-   **DP:**
    Specification of whether there is a declaration of performance.
    -   ☑ There is a declaration of performance.
    -   ☐ There is no declaration of performance.
    *Technical info: checkbox*

## Overview of Documents

### Sales > Overview > Orders not Invoiced, Invoices not Booked, Deliveries not Complete, Orders Locked for Invoicing > Enter date > [OK]

[Image: Fig. D-180 showing several overlapping dialog windows related to 'Orders not invoiced', 'Invoices not booked', 'Deliveries not complete', and 'Orders with invoice block'.]

**Fig. D-180: Orders not invoiced, Invoices not booked, Deliveries not complete, and Orders with invoice block**

These dialogs display the overviews for the following documents in the selected period:

-   **Orders not invoiced:**
    Displays all orders for which no invoice has been created.
-   **Invoices not booked:**
    Displays all documents for which an invoice has been created that was not yet booked.
-   **Incomplete deliveries:**
    Displays all documents for which there are incomplete deliveries.
-   **Orders with invoice block:**
    Displays all orders for which invoicing is blocked.

If you want to open one of the overviews, you first have to enter the start date for the search. If you do not specify a date, all corresponding documents will be displayed in the overview.

The display of the columns is freely configurable and depends on the customer-specific formatting of the SQL query in question.

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

## Sales

In Sales, information about customer acquisition and commission calculation is displayed and you can manage the project budgeting.

All dialogs that you can open via the Sales menu element are customer-specific program adjustments.

For additional information about this area, contact your A+W Software GmbH contact person.
