---
description: "EN_AWBusiness_Sales_4_6-2"
---


# Overviews and References concerning Header Data

---
## Search Documents – Details View

> Documents > Order > Search > Details View tab

| Item number | Product number | Product description | Qty. | Width |
| :--- | :--- | :--- | :--- | :--- |
| 1 | | 723 IG 5/12/Th6 A+W | 10 | 1255 |
| 2 | 998 | 723 IG 5/12/Th6 A+W | 10 | 1255 |
| | 6530 | Sonderrabatt | 10 | 1500 |

*Fig. C-271 Search Document - details view*

This tab displays a view of the document items of the document marked on the Table tab.

## Copy Documents

> Documents > Quotation, order, credit note, inquiry, P.O. > Quotation, order, credit note, inquiry, P.O > Functions menu> Document group > Copy documents

You can open the Copy documents dialog and corresponding menus from various dialogs. It may already be opened in Partial shipment, Complaint or Down payment mode. The dialog is described in connection with an Order in this manual.

⇨ Tutorial, "Copy Documents" on page C-240

> **Partial shipment, complaint, down payment**
> If you select Functions > Partial delivery, Complaint or Down payment from the menu, the appropriate fields are automatically enabled or locked on the Copy documents dialog.

This dialog offers the following tabs:

*   "Copy documents – Copy 1:1" on page C-531
*   "Copy documents – Copy by item" on page C-537
*   "Copy documents - Further options - target document" on page C-539
*   "Copy documents - Source document options" on page C-541
*   "Copy documents - Text/Attachments" on page C-542
*   "Copy documents - Shape parameters" on page C-543

### Menus

*   "Options menu" on page C-527
*   "Overviews Menu" on page C-529

### Options menu

> Documents > Quotation, order, credit note, inquiry, P.O. > Quotation, order, credit note, inquiry, P.O > Functions menu> Document group > Copy documents > Options menu

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

> **Activated options after opening the dialog**
> Please note that changed options will only become effective the next time you open the dialog.
> If an activated option has started a check, opening the document can be delayed. The extent of the delay depends on the performance of the computer.
> Activated options are described in the following.

### General group

*   **Search shipping date by route:**
    The shipping date is automatically set to the next possible route day.
*   **Always calculate purchase price:**
    The purchase price will always be calculated, even if pricing is disabled in the Target section.
*   **Down payment invoice with items:**
    Down payment invoices will show the order items.
*   **Number area for partial shipments not based on OM area:**
    The numbers for partial delivery notes do not consider the number area of the OM areas. The numbers are always loaded from number area <n.s.>.
*   **Number area for complaints not based on OM area:**
    The numbers for complaints do not consider the the number areas of the OM areas. The numbers are always loaded from number area <n.s.>.
*   **Delete stock code if status >= goods withdrawn:**
    This function is only enabled if you copy a document to a different database. The stock codes will be deleted in this case so as not to change the stock data in the target database.
*   **No shipping fee for partial shipments:**
    The shipping fee will not be applied to partial shipments, even if the code for this surcharge has been set in the master data.
*   **Complaint quantity matches item quantity:**
    For complaints, the entire item quantity will be suggested by default.
*   **Recreate settings for pricing:**
    The option Always carry out purchase price pricing is saved user-related when you exit the dialog. The option will be restored when you open the dialog again.
    If this setting has not been activated, then the option Always carry out purchase price pricing is always deactivated when you open the dialog.
*   **Consultant=user:**
    The Consultant field in the order automatically shows the name of the user registered in A+W Business or the user who has entered the document.
*   **Keep item reference:**
    References entered in the order will be adopted for the new order automatically.
    ⇨ "Consignment" on page C-452
*   **Perform product check:**
    When copying each item, it is checked whether the main product or a BOM element is locked or deleted. If this is the case, a corresponding message will be displayed at the end of the copying process.

### Surplus in partial shipments group

*   **No action:**
    Surplus entered by mistake for a partial shipment does not result in a message.
*   **Message:**
    A message will be issued if the quantity included in the partial shipment exceeds the item quantity.
*   **Impossible:**
    Surplus cannot be entered.

### Partially shipped quantities group

*   **Consider rack report for partial shipments:**
    The rack number will be reported for partial shipments.
*   **Consider quantity of goods received for partial shipments:**
    The quantity of the partial shipment is preset with the quantity of goods received.

### Down payment amount group

*   **Down payment amount:**
    *   **Gross:**
        The down payment amount is entered as the gross amount.
    *   **Net:**
        The down payment amount is entered as the net amount.
    *   **Percentage:**
        The down payment amount is entered as a percentage of the order total.

### Messages group

*   **Suppress error message for delivery date:**
    An error message will be shown if the shipping date from the source order is not kept for the target order. You can deactivate this message e.g. if you edit the new order after copying.
*   **Suppress error message for partial shipment:**
    If only part of an item is adopted for the partial shipment, a message to that effect will appear. This can be disabled e.g. if you usually issue partial shipments with partial quantities.
*   **Suppress all error messages and checks:**
    If you activate this option, all error messages and checks are switched off.

## Overviews Menu

> Documents > Quotation, order, credit note, inquiry, P.O. > Quotation, order, credit note, inquiry, P.O > Functions menu> Document group > Copy documents > Overviews menu

Use this menu to display overviews without having to close the present dialog.

### Overview group

*   **Partial shipment:**
    Opens the List of partial shipments dialog.
    ⇨ "Overview Partial Deliveries" on page C-553
*   **Complaint:**
    Opens the List of complaints dialog.
    ⇨ "Complaint Overview" on page C-555
*   **Down payment:**
    Opens the Down payment list dialog.
    ⇨ "List of Down Payments" on page C-556

### View group

*   **Show source document:**
    Opens the Document view dialog as a preview to the source document.
*   **Show target document:**
    Opens the Document view dialog as a preview of the document that has been created by copying.
    ⇨ "Document View" on page C-543

## Copy documents – Copy 1:1

> Documents > Order > Order > Functions menu > Document group > Copy documents > Copy 1:1 tab

*Fig. C-272 Copy documents – Copy 1:1*

Use this tab to define the settings for the document header.

> **Change document data**
> Please note that a new document will be created when you save your entries. You can then only enter subsequent changes in the new document.

### Select areas

**From, to** You can copy documents from any area in the from field to any area in the to field. You can even copy documents from archives.

**Target server/database** If you are using several databases on different servers, you can select another database.
Please check with your contact at A+W Software GmbH if you want to use additional databases on other servers.

### Mode

Choose an option to define the document type you want to create. The mode may already be active if you have selected the entry Partial shipment, Down payment or Complaint in the Functions menu of the document.

*   **Copy:**
    Enables all fields you need to create a new document. This option also allows you to copy all documents of a number manager.
    ⇨ Tutorial, "Copy Documents" on page C-240
*   **Partial delivery:**
    Locks all fields that have to be adopted from the order header without changes.
    ⇨ Tutorial, "Partial Deliveries" on page C-252
*   **Complaint:**
    Locks all fields that have to be adopted from the order header without changes and enables the Complaint section.
    ⇨ Tutorial, "Complaints" on page C-278
*   **Down payment:**
    Locks all fields that have to be adopted from the order header without changes, and enables the Down payment section.
    ⇨ Tutorial, "Down Payments" on page C-270

### Source

You can copy a single document or several documents from a number manager.

**Number** Number and selection of a single document. You can choose a document from another number manager only if you have selected the Copy mode.

**Number Manager** Name and selection of number manager. This option is only enabled if you have selected the Copy or Complaint mode.
Enable the Overview section with this option.

### Complaint

Complaints can only be created for individual documents. The fields in this area are enabled only if you have selected the Complaint mode.

> **Enter reason and cause per item**
> You can enter the details for the complaint items separately, e.g. if there are different causes.
>
> ⇨ "Complaint" on page C-501

**Cause** You can select a cause. This detail can be used for the statistical analysis. The system offers for selection all the causes that are defined in the master data.
⇨ Master Data, "Complaint Cause" on page B-574

**Reason** Allows you to select the reason of complaint. This detail can be used for statistical analysis. The system offers all the reasons defined in the master data for selection.
⇨ Master Data, "Complaint Reasons" on page B-575

**Free** A complaint can be billed or created free of charge.
*   The complaint will be billed. The prices for the complaint can differ from those in the original order e. g. for reasons of goodwill.
*   The complaint is free of charge. The customer will not receive a new invoice with the replacement. Complaint statistics will compare the sales price and the proceeds missed.

> **Credit note for complaint**
> You can issue a credit note for a complaint item. The replacement has to be invoiced in this case.

### Overview

The overview is only enabled if you have selected the Copy mode and Number manager as the source. The selected documents will be copied. You can select several documents at once.

### Down payment

The fields in this section are only enabled if you have chosen the Down payment mode.

> **Prerequisite**
> Down payments must be entered as a product of the product type Services/ surcharges. They have to be allocated as an automatic surcharge in Product allocation-surcharges.
>
> ⇨ Master Data, "Product Management - Product" on page B-591
> ⇨ Master Data, "Surcharge Product Assignment" on page B-1024

**Gross, net amount, percentage** The down payment can be entered as a gross or net amount, or as a percentage of the order total. This is defined in the Options menu.
⇨ "Down payment amount group" on page C-529

**Date** The current date is preset. You can change it.

### Archives

The Source field is enabled if you want to copy from archives. You can select the required archiving year.

### Change

**Production preparation** If you are using order areas, the system shows the order area defined in the source document.
*   The order area is adopted from the source document. The combo box is locked.
*   The order area can be changed. The combo box is enabled.
⇨ Master Data, "Order Areas" on page B-1014

**Document type** The fields are only enabled if you have chosen the Copy mode. For the other modes, the document type is already defined.
*   The document type is adopted from the source document or from the mode. The combo box is locked.
*   The document type can be changed. The combo box is enabled.

**Business type** The business type defines how the turnover will be analyzed in statistics.
*   The business type is adopted from the source document. The combo box is locked.
*   The business type can be changed. The combo box is enabled.
⇨ Master Data, "Business Type" on page B-887

**Client** If you are working with several clients, you can adopt order items this way. You may have to select an additional target database.
*   The client is adopted from the source document. The combo box is locked.
*   The client can be changed. The combo box is enabled.

**Lock codes** The fields are only enabled if you have chosen the Copy mode. For partial deliveries, this is automatically set based on the settings in the customer data or in the order.
*   The lock code is adopted from the source document. The combo box is locked.
*   The lock code can be changed. The combo box is enabled.
⇨ "Invoice” on page C-422
⇨ Master Data, "Lock status" on page B-423
⇨ Master Data, "Lock Code" on page B-897

**Net price** The fields only are enabled if you have chosen the Copy mode. Your entry defines whether discounts will appear on the printout.
*   The setting for entering prices is adopted from the source document. Options yes and no are locked.
*   The setting for entering prices can be changed. Options yes and no are enabled.

**Status** The fields are locked if you have chosen the Down payment mode. The status is automatically set to Down payment invoice issued.
*   The status cannot be changed. The combo box is locked.
*   The status can be changed. The combo box is enabled.

### Target

The number of the new document is automatically determined when you copy the document.

> **Change customer and supplier**
> The Further options - target document allows you to enter the customer, supplier, and a different shipping address.
>
> ⇨Copy documents - Further options - target document

These three options are only enabled if you have selected the Copy mode.

*   **Determine number automatically:**
    The new document is created with a new number. This option is automatically active in the Copy mode.
*   **Manual entry of number:**
    This option can be used to copy the items from the source document to a target document. The input field in which you can enter the target document's number is enabled.
*   **Adopt number from source:**
    This option is only enabled if you copy a document from archives or from another database. This way, you can retrieve a document from archives, e.g. to edit it.

**Target number manager** The number manager of the source document is displayed. You can create the new document in a different number manager.

**Price calculation** Prices can be recalculated to determine the correct (customized) prices.
*   Prices will not be recalculated. The prices are adopted from the source document. You should select this setting when issuing a credit note to make sure that the same price is credited.
*   The prices will be recalculated. Checkbox Delete settings is enabled. The standard price lists or the customized price lists will be applied.

> **Customized prices**
> The customized prices from the source document are adopted for the new order even if this is entered for another customer.

**Delete settings** With this setting you can define whether manually entered prices will be deleted.
*   Manually entered prices will be kept when prices are recalculated.
*   Manually entered prices will be reset when prices are recalculated.

**Update customer data from customer master data** Changed customer data will not be automatically updated when copying.
*   Customer data will not be reloaded. If customer master data has not been edited after the source document was issued, this checkbox can remain disabled.
*   Customer data will be reloaded. You should enable this function if customer master data has been changed.

**Reload product codes** Product data will not be automatically reloaded when copying.
*   Product codes will not be reloaded.
*   Product codes will be reloaded. You should enable this function if different product codes have been set for the customers, e. g. the supply type.

> **Keep settings**
> The settings Price calculation, Update customer data and Reload product code are separately saved for the Copy documents and Complaints modes. The Copy documents mode may therefore have different settings than the Complaints mode.

## Copy documents – Copy by item

> Documents > Order > Order > Functions menu > Document group > Copy documents > Copy by item tab

*Fig. C-273 Copy documents - by item*

Use this tab to define the items to be adopted for the target document.

> **Change document data**
> Please note that a new document will be created when you save your entries. You can amend the data in the new document only.

### Source

This section shows the items from the source document.
⇨ Tutorial, "Controls in the document header" on page C-40

> **Tag**
> Only selected items will be copied to the new document. The quantity can be changed.

**Document** Document number of the document from which the items are copied.

**Item** Number of items.
The overview lists all items of the source document.

### Target

The items are only shown once the copy has been created.

**Item (1:1)** You can adopt the item numbers for the new document unchanged, e. g. in partial deliveries with partial item quantities.
*   Item numbers will not be adopted. The adopted items will be renumbered in the new document.
*   Item numbers will be adopted.

**Document** The new document number will be displayed after the document has been created.

**Item** The number of items in the new document will be displayed after the document has been created.

## Copy documents – Further options - target document

> Documents > Order > Order > Functions menu > Document group > Copy documents > Further options - target document tab

*Fig. C-274 Copy documents – Further options - target document*

This tab defines the dates and the shipping address for the new document. The tab is only enabled if you have selected the option Set number automatically on the Copy 1:1 tab.

### Dates

The fields in this section are described in detail in the description on the document header data.
⇨ "Header data - Document" on page C-414

### Different

You may have to enter a different supplier if the target document is a P.O.

**Customer, supplier** You can enter a different customer and different supplier for the new document.
For purchase orders, these fields refer to the suppliers and the sub-suppliers.

**Delivery address**
You can enter a delivery address. If you leave these fields blank, the order will be shipped to the customer's address.
You can adopt one of the customer addresses that you have selected in the table as the delivery address by using the arrow buttons.

**Table**
If a different delivery address has been defined for the selected customer or supplier, it will be displayed here. If only one delivery address has been entered, the data is automatically adopted for the Delivery address section. It can be changed if required.

## Copy documents – Source document options

> Documents > Order > Order > Functions menu > Document group > Copy documents > Source document options tab

*Fig. C-275 Copy documents – Source document options*

Use this tab to define the following data:
*   The delivery date for partial deliveries.
*   The category for quotations.

### Dates

**Change shipping date of original order for partial deliveries** You can enter a new date for the remaining delivery of the original order.
*   **Date:**
    Enter a fixed date for the remaining delivery.
*   **Automatically by:**
    The shipping date of the original order is automatically extended by the defined number of days.
*   **Next shipping date:**
    The next shipping date is automatically entered as the shipping date.

### Changes

**Category** The category can be used to classify quotations by reasons for rejection, e.g. too expensive or no feedback. The categories can be used to evaluate quotations for statistical purposes.

## Copy documents - Text/Attachments

> Documents > Order > Order > Functions menu > Document group > Copy documents > Text/Attachments tab

*Fig. C-276 Copy documents - Text/Attachments*

Use this tab to add text for the target document or a file as an attachment.
The fields are described in detail in the description on the document header data.
⇨ "Header data - Attachments" on page C-431

You can either select one of your texts entered in the master data or enter a new one. You can define whether the text is to be displayed as header or footer.

## Copy documents - Shape parameters

> Documents > Order > Select order > Functions menu > Document group > Copy documents > Shape parameters tab

Use this tab to check the parameters for shapes.

## Document View

> Documents > Order > Select order > View menu > Document group > Document view

*Fig. C-277 Document view*

This dialog shows a short overview of all items included in the document.

> **Print document displayed**
> You can print the displayed documents. This is different from printing forms. The document status will only be raised in the printing of forms.
>
> ⇨ "Form/Label Printing" on page C-635

## Customer Info

> Documents > Order > Select order > View menu > Document group > Customer info

*Fig. C-278 Customer info*

This dialog displays general information on the current customer and on the attached documents applying to this customer. Details are adopted from the master data.
⇨ Master Data, "Specification" on page B-761

You can also retrieve this information from the item entry dialog.
In the document management, you can also call up this information on the Customer info tab.
⇨ "Header data - customer info" on page C-434

This dialog is automatically displayed if the option has been enabled in the customer master data.

## Capacity Overview

> Documents > Orders > Select order > View menu > Capacity overview group > Capacity overview

*Fig. C-279 Capacity overview*

This dialog displays the free capacities and assigned times, the status and the progress of production from A+W Production Capacity Planner.

This dialog is only displayed if you are working with A+W Production Capacity Planner and A+W Capa View. For detailed information about the capacity overview dialogs, see the documentation for A+W Capa View.

**[Shifts]** The overview is displayed by shifts.

**[Days]** The overview is displayed by days.

**[Machines]** The assignment of a particular machine is displayed. You select the machine on the combo box on which the available machines are displayed.

**[Groups]** The assignment of a particular machine group is displayed. You select the machine group on the combo box on which the available machine groups are displayed.

**(Combo box)** Selection of the machine or machine group. The defined machines and machine groups are offered for selection.

**Start date** Entry of the date starting on which the capacity overview should be displayed. You can enter the date manually or select it with the button [Calendar].

**[7 days], [10 days], [14 days]** The assignment of the machine or machine group is displayed across a period of 7, 10 or 14 days.

**[Left arrow]** The start date is set back by the specified period. The capacity overview is updated.

**[Right arrow]** The start date is set forward by the specified period. The capacity overview is updated.

> **Change view**
> You can change to the detail view of the capacity overview if you click a bar in the capacity display. You can close the detailed view again by clicking the [x] button in the upper left corner.

### Detail view

*Fig. C-280 Capacity overview – Detail view*

In the detail view of the capacity overview, the selected data is displayed by order or pieces.
The upper part of the dialog displays the selected data by time, area, and pieces.
You can select how the data is displayed on the lower part of the dialog:

*   **[Batch]** The overview is displayed per production run. It can be displayed summed up by time, pieces or amount.
*   **[Order]** The overview is displayed per order. It can be displayed summed up by time, pieces or amount.
*   **[Time]** The overview is displayed per order or pieces by time.
*   **[Pieces]** The overview is displayed per order or pieces summed up by amount.
*   **[Amount]** The overview is displayed per order or pieces by area.

## History

> Documents > Order > Select order > Functions menu > Document group > History

*Fig. C-281 History*

This dialog allows you to trace what the document has been used for. The display is updated once the current document is closed.
The top section shows the document type, number, and status of the current document.
⇨Tutorial, "Document History" on page C-213

### Overview

**Date / time** Date and time of processing.

**Transaction / action** Processing type.

**Status** Status created by the processing.

> **Automatic status changes**
> Automatic status changes can only result in raising the document status. The status can only be reset manually.

**Person in charge** Name of the employee registered in A+W Business and who has edited the document.

**Reference** Number of the referenced document:
*   The referenced document has been created from the current document, e. g. delivery note number.
*   The current document has been created from the referenced document, e. g. order number in the case of a purchase order.

**Comment** Details on content change, e. g. price change.

**Show last action first** You can sort the sequence of the shown entries. This setting is saved per document type.
*   The first action will be shown first.
*   The last action will be shown first.

## Status Change

> Documents > Order > Select order > Functions menu > Document group > Status change

*Fig. C-282 Change status*

Status changes can be made for individual orders, for several selected orders, or for all orders of a number manager. A change per number manager may be necessary e. g. if invoices were printed in the wrong number area.
⇨ Tutorial, "Copy entire Document" on page C-244

> **Change applies to the entire number manager**
> Before changing the status of all documents of a number manager, please check if this number manager actually only contains the documents to be changed.

### Mode

Select this option to define whether one or several documents will be changed:
*   **Number Manager:**
    The status of all documents of a number manager is changed. The combo box for selecting the number manager is enabled.
*   **Selection:**
    Only in number manager. The status of the selected documents changes. Multiple selection is possible using the <Ctrl> key.
*   **Number:**
    The status of a certain document is changed. The Number field in the document section is enabled.

### Document

**Number** Number of the document, the status of which will be changed. This field is only enabled if the option Number has been activated.

**Name** Name of the customer whose document will be changed.

**Street, place** Address from the document to be changed.

**Fill number manager** If you change the status of a single document, you can transfer it to the corresponding number manager at the same time. Checkbox is only enabled if the option Number has been activated.
*   The document will not be transferred to a number manager.
*   The document will be transferred to a number manager according to its new status.

### Status

**Old** Shows the status to be changed.
The field is only filled if the option Number has been enabled.

**New** Combo box to select the new status.

## NM Selection

> Documents > Order > Select order > Functions menu > Document group > NM selection

*Fig. C-283 NM selection*

Use this dialog to change the number manager for the current document.
⇨Tutorial, "Number Manager" on page C-176
⇨ "Number Manager" on page C-624

**Current number manager** Select the number manager to be accessed by the Document management dialog.
Enter a new name to create a new number manager with that name. Please note that the current document will be moved to the new number manager automatically.
