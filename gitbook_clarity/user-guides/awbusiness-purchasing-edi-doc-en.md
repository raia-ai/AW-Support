---
description: "EN_AWBusiness_Purchasing_3_30_2-4"
---


# Tutorial

---
## Electronic document exchange

4. Go to the **Selection** tab.

**Fig. D-113: Interface management**
*   **A** Interface type
*   **B** Specifications for the target file
*   **C** Specifications for the log file
*   **D** Path for the backup file

5. Enter the directories and file names (B) of the export file and the backup file (D).
6. Select the interface version (A) your system uses.
   If you also want to transfer order confirmations and invoices electronically (openTRANS-Format) you have to choose the version you have been using so far for transferring the data. The version is defined when A+W Business is installed.

**Fig. D-114: Settings for EDI document export**

7. Go to the menu **Start > Save** to save the data. The data is saved.
8. Go to the **Parameters** tab.

**Fig. D-115: Parameter for EDI exchange**
*   **A** Compulsory referencing
*   **B** Access lock and time of lock
*   **C** Parameters for EDI import of orders (only for customers)

9. Mark the checkboxes for export:
    *   **Compulsory referencing (A):** If an item without a reference is transferred to an (external) product, this item can be ignored. An error report will be made in the logbook in this case. If this checkbox is not marked, the product number is imported from the master data to the interface file. This is useful, for example, if the sending and the receiving system use the same product master data. In this case it is not necessary to enter data in the reference tables.
    *   **Locking active** and **Maximum lock time (B):** With this setting, you prevent that only one program can access the same interface during the specified period.
    *   **Import from customer orders (C):** When you set up data for customers, you can also define extra settings for import.

10. Repeat the steps for all suppliers with whom you exchange data via EDI.

11. Now go to the menu **Master data > B2B > Customer > Customer** and repeat the steps for all customers with whom you exchange data via EDI.

### Exporting of purchase orders

When you export purchase orders, the data is saved in an ASC file. This file is then saved in a defined directory. The file is then transferred to the supplier via the EDI interface.

#### How to export a purchase order

1. Go to the menu **Documents > P.O.s > Export**.
The **Export** dialog is opened and the purchase orders in the current Number Manager are shown.

**Fig. D-116: Export of purchase orders**

2. To start the export, go to the menu **Start > Execute**. Export begins. The progress report shows which purchase order is being transferred.
3. Go to the **Pool** tab to check the export status. You can update the view by means of **[Queries]**.

**Additional Information**
⇨ Sales, "Document Import" on page C-330
⇨ Master Data, "Interface Service" on page B-995

# Software Reference

## Overview

In document management you can enter and edit all documents required for purchasing, e.g. inquiries about shipments and orders. You can also enter receipt of goods, check and correct delivery dates and verify suppliers' invoices.

The Software Reference provides information on the following subjects:
*   Inquiry (menu)
*   Purchase order (menu)
*   Order confirmation
*   Receipt of goods
*   Invoice
*   Invoicing of basic glass

The following dialogs are the same for all document types and are therefore explained just once, in the Sales section:
*   Transfer to financial accounting
*   Transfer to archives
*   Search

> **Dialogs are accessible from different points**
> Please note that many of the functions and overviews in the field of purchasing can be accessed from different dialogs in A+W Business. The corresponding dialogs will only be described once in this document.
> Dialogs which are also required for sales are described in detail in the Sales section.

> **Dialog descriptions in the Sales section**
> ⇨ Software Reference, "Document Management" on page C-359
> ⇨ Software Reference, "Overviews and References concerning Header Data" on page C-454
> ⇨ Software Reference, "Item Data" on page C-385
> ⇨ Software Reference, "Overviews and References concerning Items" on page C-503
> ⇨ Software Reference, "Number Manager" on page C-540
> ⇨ Software Reference, "Printing" on page C-548
> ⇨ Software Reference, "Transfer to Archives" on page C-594

## Inquiry (menu)

*Documents > Inquiry*

You can access the following program items via the Inquiry menu:
*   **NM inquiry:**
    The Number Manager function is the same for all documents. It is described in detail with the orders.
    ⇨ Sales, "Number Manager" on page C-540
*   **Inquiry:**
    Document input is the same for all document types. It is described in detail with the orders.
    ⇨ Sales, "Document Management" on page C-359
    ⇨ Sales, "Item Data" on page C-385
*   **Print inquiry:**
    Form and label print is the same for all documents. It is described in detail with the orders.
    ⇨ Sales, "Printing" on page C-548
*   **Journal:**
    Printing of journals is the same for all documents. It is described in detail with the orders.
    ⇨ Sales, "Journal" on page C-632
*   **Transfer to archives:**
    Transfer to archives is the same for all documents. It is described in detail with the orders.
    ⇨ Sales, "Transfer to Archives" on page C-594
*   **Search:**
    Search is identical for all documents. It described in detail with the orders.
    ⇨ Sales, "Search Document" on page C-455

### Inquiry (document management)

*Documents > Inquiry > Inquiry*

**Fig. D-117: Document management – Inquiry**

This dialog is used to enter and edit inquiries for your suppliers. Inquiries can either be created manually or they are created during the P.O. transfer, provided the option Inquire immediately is selected in the order pool.
⇨ Tutorial, "Inquiry" on page D-108
⇨ Sales, "P.O. Transfer – P.O. Numbers" on page C-568

The fields in the Document management dialog and at item entry are the same for all document types. They are described in detail with the orders:
⇨ Sales, "Document - Header Data" on page C-365
⇨ Sales, "Document - Items" on page C-394

## Purchase order (menu)

*Documents > Purchase order*

You can access the following program items via the Purchase order menu:
*   **NM purchase order:**
    The number manager function is the same for all documents. It is described in detail with the orders.
    ⇨ Sales, "Number Manager" on page C-540
*   **Purchase order:**
    Document input is the same for all document types. It is described in detail with the orders.
    ⇨ Sales, "Document Management" on page C-359
    ⇨ Sales, "Item Data" on page C-385
*   **Partial delivery:**
    Creation of partial deliveries is the same for all document types. It is described in detail with the orders.
    ⇨ Verkauf, "Teillieferungen" auf Seite C-603
*   **Replenishment order:**
    Use this dialog to re-order, complain, invoice purchased parts that have been reported broken or to reduce the order quantity.
    ⇨ "Replenishment Order" on page D-189
*   **Print purchase order:**
    Form and label print is the same for all documents. It is described in detail with the orders.
    ⇨ Sales, "Printing" on page C-548
*   **Export (EDI):**
    You can use this dialog to export purchase orders via the EDI interface.
    ⇨ "Export (EDI)" on page D-191
*   **Journal:**
    Printing of journals is the same for all documents. It is described in detail with the orders.
    ⇨ Sales, "Journal" on page C-632
*   **OC supplier:**
    This dialog lets you create and check your suppliers' order confirmations (OC).
    ⇨ "OC supplier" on page D-195
*   **Order confirmation:**
    *   **Price control:**
        Use this dialog to check the order confirmations of your suppliers and correct prices if required.
        ⇨ "Order confirmation" on page D-202
    *   **Electr. price control:**
        You can use this dialog to check the prices and references in electronically transferred order confirmations.
        ⇨ "Order confirmation" on page D-202
    *   **Reminder:**
        You can use this dialog to create reminders for outstanding deliveries.
        ⇨ "Reminder" on page D-223
*   **Receipt of goods**
    *   **Receipt of goods:**
        Use this dialog to create receipts of goods for purchase orders and stock purchase orders.
        ⇨ "Receipt of goods" on page D-225
    *   **Incoming control:**
        Use this dialog to check whether the receipts of goods are complete.
        ⇨ "Inspection of goods received" on page D-239
*   **Invoice:**
    *   **Invoice control:**
        Use this dialog to check the invoices of your suppliers and correct prices if required.
        ⇨ "Invoice control - Purchase orders" on page D-246
    *   **Electr. invoice control:**
        Use this dialog to check the prices and references in electronically transferred invoices.
        ⇨ "Electronic invoice control" on page D-254
*   **Transfer to FinAc:**
    Transfer to financial accounting is the same for all documents. It is explained using an order as an example.
    ⇨ Sales, "Transfer to FinAcc" on page C-588
*   **Transfer to archive:**
    Transfer to archives is the same for all documents. It is described in detail with the orders.
    ⇨ Sales, "Transfer to Archives" on page C-594
*   **Search:**
    Search is identical for all documents. It described in detail with the orders.
    ⇨ Sales, "Search Document" on page C-455
*   **Single glass settlement:**
    Use this to manage internal profit center calculations. Basic glass calculation is only released for specific customers.

### Purchase order (document management)

*Documents > Purchase order > Purchase order*

**Fig. D-118: Document management - P.О.**

This dialog is used to enter and edit purchase orders.
⇨ Tutorial, "Manual purchase order" on page D-77

The Document management dialog and the corresponding menus are the same for all document types. We are going to describe it in connection with an Order.
⇨ Sales, "Document - Header Data" on page C-365
⇨ Sales, "Document - Items" on page C-394

> **Enter purchase order**
> You can create purchase orders in the same way as an order. Make sure to select the correct document type:
> *   **Stock P.O.:**
>     This setting lets you order stock articles. The delivered items are booked into Stock automatically upon receipt of goods. You must select the stock purchase orders in this purchase order with the stock search <F3>. The Stock P.O. type is shown in the Type field.
> *   **<n.s.>:**
>     Use this setting to order all products which are not booked through stock.
>     ⇨ Sales, "Type" on page C-369
>     ⇨ Tutorial, "Entering an independent P.O." on page D-79

If you enter a stock P.O. with products which are not recorded as stock articles, the receipt of goods for these products cannot be booked into stock automatically. A message to that effect will be issued when entering the purchase order.

> **Items without stock codes**
> If you enter stock P.O.s with items which are not recorded as stock items, they will not be displayed at receipt of goods. You can however activate the corresponding option in the company data.
> ⇨ Master Data, "Show items w/o stock code at receipt of goods on stock" on page B-933

### Replenishment Order

*Document > P.O. > Replenishment Order*

**Fig. D-119: Replenishment**

Use this dialog you manage orders with ordered parts that are reported as broken from production. You can reorder the ordered parts, make a complaint, invoice them or reduce the order quantity.

#### Selection

*   **Order from, to:** Restrict the search to an order or a sequence of orders.
*   **Delivery date from, to:** Restrict the search to a specific delivery date or set of delivery dates.

#### Documents

The list shows all orders with breakage matching the search criteria.

*   **Order:** Order number.
*   **Order item:** Item number from the order.
*   **Delivery date:** Delivery date shown in the order header.
*   **Ρ.Ο.:** Purchase order number.
*   **Purchase Item:** Item number from the purchase order.
*   **Supplier:** Name of the supplier from the purchase order.
*   **Product:** Number and name of the product.
*   **Order quantity:** Quantity from the order.
*   **Purchase qty.:** Quantity that is ordered.
*   **Breakage Quantity:** Quantity reported broken.
*   **Feedback date:** Date of breakage report.
*   **Action:** Selection of the action:
    *   **Replenishment order:** The purchase order is created and moved to the selected Number Manager.
    *   **Complaint:** A complaint is created for the ordered parts. If this option is selected, the reason and cause of the complaint can be specified.
    *   **Booking in terms of value:** The purchase order is created with a negative item quantity. Thus, the broken quantity is booked out and the value of the broken quantity is offset against the value of the order.
    *   **Reduce order quantity:** The original order is reduced by the broken quantity. This excludes the possibility of reordering.
*   **Complaint reason:** The complaint reason is specified only if Complaint is selected as the action.
*   **Complaint cause:** The complaint cause is specified only if Complaint is selected as the action.
*   **Comment:** You can enter comments, e. g. agreements in connection with this replenishment or complaint.
*   **Label:** Number of the label from production. The number can not be changed.

#### Goal

*   **Number Manager:** Number Manager to which the replenishment orders shall be moved.

### Export (EDI)

*Documents > Purchase order > Export*

**Export (EDI):** You can use this dialog to export P.O.s in order to transfer them to the respective supplier via the EDI interface.
⇨ Tutorial, "Data export/import (EDI)" on page D-174

> **Prerequisite**
> For this purpose, the parameters for the interface have to be defined for each individual supplier/customer with whom you would like to exchange documents via the external interface. These parameters have to be configured in the menu **Master data > B2B**.

This chapter provides information on the following subjects:
*   "Functions menu" on page D-192
*   "Export - export” on page D-193
*   "Export - pool" on page D-194

### Functions menu

*Documents > P.O. > Export > Functions menu*

Use this menu to open other dialogs without closing the Export dialog.

#### Edit group

*   **Copy:**
    Opens the Copy number manager dialog to create a new number manager.
    ⇨ Sales, "Copy Number Manager" on page C-545
*   **Status change:**
    Opens the Status change dialog to change the status manually and to amend the Number Manager.
    ⇨ Sales, "Status Change" on page C-479

#### Documents group

*   **Show document:**
    Opens the Document view dialog and provides a print preview.
    ⇨ Sales, "Complaint" on page C-510
*   **History:**
    Opens a list of status changes for the selected document.
    ⇨ Sales, "History" on page C-478
*   **Document data:**
    Opens the Document data dialog to correct the dates and the status if necessary.
    ⇨ Sales, "Document Data" on page C-646
*   **Document entry:**
    Opens the Document management dialog to create or change documents.
    ⇨ Sales, "Document Management" on page C-359

#### Document copy group

*   **Copy documents:**
    Opens the Copy documents dialog to copy a document to the same or another document type.
    ⇨ Sales, "Copy Documents" on page C-461
*   **Partial delivery:**
    Opens the Copy documents dialog to enter a partial delivery.
    ⇨ Sales, "Copy Documents" on page C-461

### Export - export

*Documents > P.O.> Export > Export tab*

**Fig. D-120: Export - Export**

This tab is used to export purchase orders. The data is saved in an ASC file. This file is then saved in a defined directory. The file is then transferred to the supplier via the EDI interface.
The settings for the export are defined by supplier in the module **Master data > B2B**.
⇨ Tutorial, "Data export/import (EDI)" on page D-174

#### Select by

*   **Employee:** Name of the employee logged in to A+W Business.
*   **Number manager:** Choose the Number Manager that the Export dialog is to access.
*   **[Logbook]:** Button that opens the system logbook.

#### Documents

A list of all documents included in the selected Number Manager. They shall be sent to the supplier by way of interfaces.
*   **Number:** Number of the document
*   **Cust./suppl. number:** Customer or supplier number
*   **Customer/supplier:** Customer or supplier name
*   **Status:** Status of the document
*   **Input date:** Date on which the document was entered
*   **Delivery date:** Delivery date
*   **OC date:** Date of order confirmation
*   **Lock code:** Code indicating whether the document is locked – the lock code is rarely set for purchase orders

### Export - pool

*Documents > P.O. > Export > Pool tab*

**Fig. D-121: Export - Pool**

Use this tab to transfer the listed purchase orders via the EDI interface (electronically).

#### Transfer pool

The list shows all purchase orders to be transferred electronically.

*   **[Delete]:** This button is only enabled if an error has occurred during the transfer. This button allows you to delete an entry from the transfer pool.
*   **[Enable]:** This button is only enabled if an error has occurred during the transfer. You can correct the data and resubmit it for transfer if an error was found. You can start the transfer process with the [Enable] button.
*   **[Queries]:** Use this button to update the display to check the transfer status.

### OC supplier

*Documents > P.O.> OC supplier*

This dialog allows you to enter the order confirmation which your supplier sent for a purchase order. You can also enter the corresponding receipt of goods and/or check the dates for purchase orders and deliveries and correct them if required.

This chapter provides information on the following subjects:
*   "Options menu" on page D-195
*   "OC supplier - documents" on page D-196
*   "OC supplier – items" on page D-200
*   "OC Supplier - change delivery dates" on page D-201

#### Options menu

*Documents > P.O.> OC supplier > Options menu*

This menu allows you to define the default settings for the dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

The following entries are displayed:
*   **Stock booking date = Delivery date:** The delivery date from the P.O. is automatically taken as the booking date. If this option is disabled, the current date will be used by default.
*   **Check OC number:** This setting outputs a message if the number of the order confirmation has not been entered by the supplier.
*   **ID number assignment:** This setting is only needed for the receipt of boxes and stockplates.
    *   **Manually:** Use this option to assign the ID manually. The checkbox Assign ID(s) in the Options area is released.
        ⇨ "Options" on page D-196
    *   **Automatic:** Use this option for automatic assignment of IDs. A default can be defined. If this option is disabled, you have to enter the ID by hand.
    *   **Settings:** Opens the Settings dialog which lets you enter the settings for the automatic assignment of IDs.
        ⇨ "Settings (ID)" on page D-238

### OC supplier – documents

*Documents > P.O.> OC Supplier > Documents tab*

**Fig. D-122: OC supplier - Documents**

Use this tab to create an order confirmation from the supplier and/or the corresponding receipt of goods. You can also check the dates for purchase orders and deliveries and correct them if required.
All the data entered on this tab also applies to all items shown on the P.O. list. Go to the **Items** tab to enter data for individual items.
⇨ Tutorial, "Supplier's OC" on page D-85

#### Documents

Select the option to define which document type you would like to create the order confirmation for. Use the magnifier to search for the P.O. or order.
*   **P.O. number:** Selection of a purchase order. The purchase order input field is released.
*   **Order number:** Selection of a customer order used to generate a purchase order. The order number input field is released.

#### Options

*   **Fill order NM:** When booking an order confirmation from your supplier and – if applicable – also the receipt of goods for the P.O., the corresponding (customer) order can be automatically moved to another Number Manager.
    *   The reference (customer) order is not moved to another Number Manager.
    *   The reference (customer) order is moved to the selected Number Manager.
*   **Fill P.O. NM:** When you book an order confirmation from your supplier and – if applicable – the receipt of goods for this P.O., the corresponding P.O. can be automatically moved to another Number Manager.
    *   The purchase order is not moved to another Number Manager.
    *   The purchase order is moved to the selected Number Manager.
*   **Book goods received:** You can enter the entire receipt of goods if your supplier has delivered the goods together with the OC.
    *   Receipt of goods is not booked.
    *   Receipt of goods is booked as complete. If the delivery contains boxes, you have to check the settings for the box ID.
*   **Assign ID number(s):** This checkbox is enabled or disabled by means of the ID number assignment setting. IDs are usually assigned to boxes. You can set a default ID for booking the receipt of goods on stock. The checkbox is enabled only if you have selected Manually in the Options menu.
    *   The checkbox is disabled if you have selected Manual in the Options menu. The ID must be entered manually.
    *   The checkbox is active if you have selected Automatic in the Options menu.
    ⇨ "Settings (ID)" on page D-238

> **Enter partial receipt of goods**
> The complete receipt of goods for individual items can be entered on the Items tab. To enter partial receipt of goods for an item, go to the Receipt of goods dialog.
> ⇨ "Receipt of goods (dialog)" on page D-225

#### P.O. data

*   **Supplier:** The supplier name from the P.O or customer order.
*   **Status:** Status of the selected document.
*   **Total quantity:** Total quantity of all items in the selected document.
*   **Confirmed delivery date:** Date of delivery by the supplier. The date is adopted from the P.O. You can change it if required. The changed date will be saved in the P.O. and - if applicable - in the reference order.
    ⇨ "OC Supplier - change delivery dates" on page D-201
*   **Partial delivery date:** Delivery date specified in the supplier's order confirmation.
*   **OC number:** Order confirmation number provided by the supplier. This number is entered for all items shown on the P.O. list. If the order confirmation number is to apply to one item only, go to the Items tab.
    ⇨ "OC supplier – items" on page D-200

#### Order data

The data in this section is displayed only if an order or a P.O. for an order has been selected. The fields are empty for a stock P.O. (without an order).

*   **Customer:** Name of the customer for whom the P.O. was created.
*   **Status:** Status of the customer order.
*   **Total quantity:** Total quantity of all items in the customer order.
*   **Delivery date at the customer:** Delivery date at the customer. The date is adopted from the order. You can change it if required. The changed data will be saved in the P.O. and – if applicable - in the reference order.
    ⇨ Sales, "Delivery Date Check (Delivery Date Control)" on page C-489
    ⇨ Tutorial, "Change delivery dates, notify customer" on page D-100
    ⇨ "OC Supplier - change delivery dates" on page D-201
*   **Planned:** Originally planned delivery date at the customer.
*   **Shipping date:** Date on which the shipment is dispatched to the customer. This date is usually the same as the delivery date. The shipping date must be earlier than the delivery date only if the delivery takes longer than one day.
*   **Route:** Selection of the route by which the goods will be shipped to the customer.

#### P.O. items

List of all items of this P.O. If the purchase order was created from a customer order, the purchased items can be the items of the referenced order at the same time.

*   **Item:** P.O. item number. For a customer order, this can also be the item number from the order.
*   **Product description:** Number and description of the ordered item.
*   **Qty:** Quantity of the ordered item.
*   **Width / Height:** Dimensions of the ordered item.
*   **Supplier OC:** Number of the supplier's order confirmation. If you have entered the order confirmation number for the entire P.O., the same number is shown for all items.
*   **Partial delivery data:** Delivery date for partial deliveries.
*   **Pr./PU:** PU price per price unit of the ordered item.
*   **Pr./PU total:** Total price per price unit of the ordered item.
*   **List/key:** Price list and key which apply for the underlying purchase price (PU).
*   **Disc.:** Discount applied to the PP.
*   **Net/item:** Item price without a discount and/or surcharges.
*   **Net/item total:** Price of all items of purchase order without a discount and/or surcharges.
*   **Price unit qty.:** Quantity in displayed price unit.
*   **Price unit:** Price unit that applies to the displayed price.
*   **Unit price:** Unit price for the selected item including all components. It is calculated based on the price unit, surcharges and discounts.
*   **Order:** Order number.
*   **Description:** Product name from the referenced order. You can enter a different supplier description in the purchase order.

### OC supplier – items

*Documents > P.O. > OC supplier > Items tab*

**Fig. D-123: OC supplier - Items**

You can enter the same data on this tab as on the **Documents** tab. The entered data only refer to the defined items.

These fields in this tab are described in detail in connection with the Documents tab.
⇨ "OC supplier - documents" on page D-196

**Items from - to:** Item numbers for which you want to book an OC number and/or receipt of goods. This will indicate the items as delivered in full. The order number appears on the P.O. list only for the entered items.
Go to the **Receipt of goods** dialog to book partial delivery/receipt of goods for individual items.
⇨ Tutorial, "Enter receipt of goods" on page D-125
⇨ "Receipt of goods (dialog)" on page D-225
