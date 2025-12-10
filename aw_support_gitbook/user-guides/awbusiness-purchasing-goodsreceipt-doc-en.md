---
title: "EN_AWBusiness_Purchasing_3_30_2-2"
source: "EN_AWBusiness_Purchasing_3_30_2-2.pdf"
tags: ["A+W Business", "Purchasing", "Goods Receipt", "Invoice Control", "Box Management", "EDI", "openTRANS", "Software Tutorial", "Inventory Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial for the A+W Business Purchasing module, covering the processes for handling deliveries, including complete and partial receipt of goods, managing box inventory with IDs, checking deliveries for completeness, and controlling prices and invoices."
long_description: "This document provides a detailed, step-by-step tutorial for the A+W Business Purchasing software, focusing on the 'Deliveries in receipt of goods' functionality. It guides users through various critical processes, starting with how to enter both complete and partial receipts of goods. The guide explains how to use the Number Manager and search by P.O. number. A significant portion is dedicated to the receipt and management of boxes, detailing how to deal with virtual item numbers, assign box IDs either automatically or manually, and print box labels. The tutorial also covers procedures for checking the completeness of deliveries and identifying quantity discrepancies. Furthermore, it explains price and invoice control, including how to check a supplier's invoice against purchase orders, handle price corrections, surcharges, and foreign currencies. The document concludes with an introduction to electronic document exchange (EDI) via openTRANS, outlining the benefits and prerequisites for exchanging purchase orders, order confirmations, and invoices electronically."
---

---
## Deliveries in receipt of goods

This section provides a tutorial on managing deliveries and receipt of goods.

### How to enter complete receipt of goods

1.  Go to the menu **Documents > P.O. > Receipt of goods > Receipt of goods**.

    *Fig. D-77: Receipt of goods – Selection by Number Manager* shows the "Receipt/despatch" window with the "Selection" tab active. Label A points to the "Selection by Number Manager" option, and Label B points to the "Number Manager" field where a manager can be selected.

2.  Go to **Selection area** and choose the option **by Number Manager**.

3.  To import the data, go to the menu **Start > Execute**.
    The display switches to the **Complete** tab where the purchase orders from the Number Manager are displayed.

    *Fig. D-78: Receipt of goods - Purchase orders* displays the "Complete" tab.
    - **A**: Delivery date and order confirmation for the selected P.O.
    - **B**: Points out a lock status.
    - **C**: Checkbox for complete receipt of goods ("Book completely").
    - **D**: Indicates that the P.O. includes boxes.

    The fields in section Delivery date (A) are locked if an order confirmation from the supplier has been entered for this purchase order.

4.  Select the purchase order for which you want to enter receipt of goods.
    The fields in Delivery date (A) area are accessible now. Normally, the delivery date and the OC number of the supplier have already been created. You can however add this data if it is missing.

5.  Tick the checkbox **book completely (C)**.

    *Fig. D-79: Receipt of goods – Report P.O. completed* shows a purchase order (P.O. 30097) with the "Book completely" checkbox ticked.

6.  To enter the receipt of goods, go to the menu **Start > Execute**.
    The data will be saved, and the P.O. status is changed. The stock on hand is updated if the P.O. includes stock articles. For reference P.O.s, receipt of goods is passed on to production and/or sales so that the corresponding customer order can be processed or completed.

### How to enter partial receipt of goods

1.  Go to the menu **Documents > P.O. > Receipt of goods > Receipt of goods**.

2.  Go to **Selection area** and choose the option **by P.O. number (A)** then enter the P.O. number (B).

    *Fig. D-80: Receipt of goods – Selection* shows the selection screen with "By P.O. number" selected (A) and a P.O. number entered in the corresponding field (B).

3.  To import the data, go to the menu **Start > Execute**.
    Data will be loaded; the display switches to the **Complete** tab.

    > Should you frequently select by P.O. or order number, you can define in the Options menu that after loading the document, the display should switch to the **By item** tab.

4.  Go to the **By item** tab if required.

    *Fig. D-81: Receipt of goods - Report partial quantity for the P.O.* displays the "by Item" tab.
    - **A**: Book item completely checkbox.
    - **B**: Storage place for stock articles.
    - **C**: Field to enter partial quantity as receipt of goods.
    - **D**: Quantity already delivered.
    - **E**: Accept surplus or shortfall checkbox.
    - **F**: Order confirmation number field.

    All P.O. items will be displayed. You can enter partial receipt of goods as follows:
    - Complete booking of one of the P.O. items (A).
    - Enter part (C) of the ordered quantity for an item.

    If for instance the quantity delivered for a stock P.O. does not exactly match the ordered quantity, you can accept a surplus or a shortfall (E), thus booking complete receipt of goods for an item.

5.  Select the item for which you want to enter receipt of goods.

6.  Go to field **Quantity received (C)** and enter the number of items received or tick the checkbox **Book completely (A)** to report the entire item as complete.

7.  Enter the supplier's order confirmation number (F) if required.

8.  For stock articles, choose the storage place (B).

    *Fig. D-82: Receipt of goods – Report partial quantity for the P.O.* shows an example where a partial quantity of 2.00 has been entered for an item, and a storage place has been selected.

9.  Go to the menu **Start > Execute** to save the data.
    Partial receipt of goods will be booked.
    The P.O. items are shown in blue if the purchase order/item has been delivered in full.
    Changes are adopted for the purchase order and the reference customer order if required.
    A surplus will be saved in the purchase order while a reference order will remain unaffected. On stock, the surplus will be booked automatically only for stock articles from stock P.O.s. The same applies to shortfalls theoretically; in practice however one would rather create a partial delivery and remind the supplier of the missing quantity.

### Check receipt of goods

You have to check deliveries for completeness in order to determine which orders can be processed further. If you know that the delivery has actually arrived you can enter the receipt of goods. You can check the following facts:
- Complete purchase orders per Number Manager
- Quantity discrepancies per P.O. item

#### How to check the receipt of goods

1.  Go to the menu **Documents > P.O. > Receipt of goods > Incoming control**.

    *Fig. D-83: Inspection of goods received – Complete P.O.* shows the "Incoming Control" window with the "Complete P.O.s" tab active, listing purchase orders that have been completely entered.

2.  Go to the **Complete P.O.s** tab and select the Number Manager for the purchase orders.
    In the **Receipt of goods complete** overview, all P.O.s are listed, whose P.O.s have been entered completely.

3.  Go to the **Qty. discrepancies** tab to display the incomplete items.

    *Fig. D-84: Inspection of goods received - Qty. discrepancies* shows the "Qty. discrepancies" tab.
    - **A**: Quantity partially delivered column ("Del. qty.").
    - **B**: "OK" checkbox to book complete receipt of goods.

    The overview lists all purchase orders for which no receipt has been booked, or incomplete receipt of goods.
    If you have moved the purchase order to a target Number Manager when booking the entire receipt of goods, no discrepancies should be shown here.

4.  Catch up on any overdue bookings by ticking the checkbox **OK (B)**.
    Please note that you can add only complete receipt of goods. To enter partial quantities, go to the **Receipt of goods** dialog.

5.  To start the booking of the receipt of goods, go to the menu **Start > Execute**.
    Receipt of goods will be booked. Completely booked purchase orders are removed from the list.

**Additional information**
- **Master Data**, "Show items w/o stock code at receipt of goods on stock" on page B-933
- **Master Data**, "Stock control mode" on page B-933
- **Sales**, "Stock Info" on page C-650
- **Software Reference**, "Receipt of goods" on page D-225

## Receipt of boxes

### Objectives
- Learning the meaning of the dummy box
- Learning about the assignment of IDs
- Learning about the settings for the automatic assignment of box IDs

### Benefits
- Upon receipt, every box gets an ID so that it can be clearly identified on stock, and can be reserved for an order.
- IDs can be assigned manually or automatically. You can also adopt the supplier's box ID.

### Please note:

- **Virtual item numbers**: If the quantity of a box item is over 1, a sub-item will be created for every box. These sub-items will get virtual item numbers consisting of the item number and the number of boxes, e.g. 1.1, 1.2 or 3.1, 3.2 etc.
- **ID**: When you enter receipt of goods, the box of every sub-item is assigned a separate ID.
- **Box identification**: Only a box with an ID can be booked as stock on hand and/or allocated to an order item.
- **Default settings**:
  - **Master data**:
    - Product Management
  - **Company data**:
    - Parameters tab
    - Stock/PP/EDI tab

### Dealing with boxes

Boxes are usually assigned ID numbers which may originate from the supplier or are maintained in your own system. These IDs are entered when boxes are received. Every box is booked with its own box ID by which it is kept on stock.

Even if the number of boxes of a P.O. item is over 1, every box is booked as a separate receipt of goods. The system automatically creates sub-items (virtual items) for the original item and allocates just one box to each of these items. This function must be enabled in company data.

An individual box ID must be allocated to each sub-position so that the stock on hand of the boxes can be maintained. These box IDs can be automatically assigned based on the values you define. An ID can also be entered manually, e.g. when adopting the box ID from the supplier's delivery note.

As part of the receipt of goods, a production date can also be specified in the automatic box ID dialog. For coated glass, this can be used for calculating the expiry date so that boxes can be handled according to the FiFo principle (FiFo = First in - First out).

When the IDs have been assigned, you can use the print function to print box labels with the IDs as barcodes, then stick them to the appropriate boxes.

Box barcodes are usually scanned upon issue of stock or when a box is broken up. This does not only serve to keep the number of boxes up to date but also for identifying the boxes.

### Check company data

The Master data section describes in detail how to define the master data for your company. The following description therefore only deals with the peculiarities you have to consider in connection with the receipt of boxes.

> **Reboot A+W Business**
> After changing company data, reboot A+W Business.

#### How to check company data

1.  Go to the menu **Master data > Company > Company data** and check the setting for the checkbox **Use virtual item numbers** on the **Parameters** tab.
    This setting is already explained in the unit on Receipt of goods.
    ⇨ "Company data - Parameters tab" on page D-124

2.  Go to the menu **Start > Save** to save the changes.
    The data is saved.

### Checking the settings for ID numbers

If you want to enter the boxes with a separate box ID, this ID can be assigned automatically. You have to define the necessary settings. These settings can be adapted before every receipt of boxes, e.g. to add a code for the supplier to the ID.

You can use a maximum of 20 characters which are automatically completed by a 5-digit number. The entered string is kept until it is changed manually. If you add a code for the supplier to the box ID, you have to make sure to change the ID before you enter the receipt of boxes for another supplier.

#### How to check the settings for the automatic allocation of ID numbers

1.  Go to the menu **Documents > P.O. > Receipt of goods > Receipt of goods**.
    The **Receipt of goods** dialog opens.

2.  Go to the menu **Options > Group > ID number allocation > Settings**.

3.  Enter the code.
    Please avoid overwriting the dummies (X) for the numbers.

4.  Click on **[OK]** to save the changes.
    The dialog closes. The settings are saved and will be kept until they are changed again manually.

5.  Go to the menu **Options > Group ID number allocation > Automatic allocation**.
    Automatic allocation of box IDs has been set now.

## Enter the receipt of boxes

When you enter the receipt of boxes, the box of every sub-item is assigned a separate ID. Then the respective labels are printed.

The following instructions exist for this training module:
- "How to enter receipt of boxes with automatic IDs" on page D-136
- "How to enter box IDs manually" on page D-139
- "How to print box labels" on page D-140

### How to enter receipt of boxes with automatic IDs

1.  Go to the menu **Documents > P.O. > Receipt of goods > Receipt of goods**.

    *Fig. D-85: Receipt of boxes - by Number Manager* shows the selection screen for receipt of goods. Label A points to the search options, and Label B points to the P.O. number field.

    Please make sure that automatic allocation of box IDs is active.

2.  Choose the option (A) which you would like to search for the open purchase orders, e.g. by P.O. number.

3.  Enter the P.O. number (B).

4.  To import the data, go to the menu **Start > Execute**.
    You will find yourself on the **Complete** tab. You can check the data again.

5.  Go to the **ID** tab.

    *Fig. D-86: Receipt of boxes – Enter receipt* shows the IDs tab.
    - **A**: Selected P.O.
    - **B**: Field to enter supplier's box ID.
    - **C**: Storage place.
    - **D**: One line per box (sub-item).

    If the quantity of the ordered item is larger than 1, the **Box items** overview lists a separate line for every box.
    You can select several boxes at once to book them in one step.

6.  Select a line that shows no virtual item number yet.

7.  Go to field **Supplier ID (B)** and enter the supplier's box ID or scan the box ID and use `<Tab>` to go to the next field.
    If more than one box was selected and the supplier ident numbers entered, the system calculates the box ident numbers for all marked entries.

8.  Choose the storage place, check the contents and price and correct them if necessary.

    *Fig. D-87: Receipt of boxes - Data for the selected line* shows that after entering a Supplier's box ID (A), the system has automatically assigned an internal ID and the data is populated in the fields for the selected line, ready to be booked (B).

    The input is adopted for the selected line.

9.  In the menu, go to **Start > Execute** in order to confirm the entries and to book the receipt of goods.

    *Fig. D-88: Receipt of boxes - New, virtual item number created* shows the result after booking. A virtual item number (booked sub-item) (A) is created, and the automatic box ID (B) is assigned.

    The box is booked and moved to the end of the **Box items** list together with the next virtual item number.

10. Repeat steps 7 to 9 until you have entered all receipt of goods.
    When you have entered all boxes you can start to print the box labels and the protocol.
    ⇨ "How to print box labels" on page D-140

### How to enter box IDs manually

1.  Go to the menu **Documents > P.O. > Receipt of goods > Receipt of goods**.
2.  Disable in the menu **Options > Group ID number allocation > Automatic allocation**.
3.  Make the preparations to enter the receipt of goods as described in the steps 2 to 7 of the previous sequence.

    *Fig. D-89: Receipt of boxes – Enter receipt* shows the IDs tab ready for manual entry.
    - **A**: Selected P.O.
    - **B**: Supplier's box ID field.
    - **C**: Manual box ID field.
    - **D**: One line per box (sub-item).

    If the quantity of the ordered item is larger than 1, the **Box items** overview lists a separate line for every box.

4.  Enter the box ID (C) by which the box shall be booked on stock.
    You can adopt the supplier's ID by moving the cursor to the field and scanning the supplier ID again.

5.  Choose the storage place, check the contents and price and correct them if necessary.
    These entries are only valid for box items selected from the list.

6.  To confirm the entries, go to the menu **Start > Execute**.
    The box is booked and moved to the end of the **Box items** list together with the next virtual item number.

7.  Repeat steps 4 to 6 until you have entered all receipt of goods.
    When you have entered all boxes you can start to print the box labels in order to print labels with the manually allocated IDs.

### How to print box labels

1.  After entering the boxes of a shipment, go to the menu **Print > Printer > Labels**.
    If you select the entry **Labels and protocol**, a protocol is also printed, which you can also view in the **Protocol (IDs)** tab.

    *Fig. D-90: Print box labels* shows the print dialog for box labels.
    - **A**: Quantity of copies to be printed.
    - **B**: Printer selection.

2.  Select the printer (B) and the number (A) of copies required.

3.  Click **[OK]** to start printing.
    The dialog closes and the labels are printed. All booked boxes and box IDs are listed in the protocol.

**Additional information**
- **Master Data**, "Use virtual item numbers" on page B-919
- **Software Reference**, "Settings (ID)" on page D-238

## Price and invoice control

### Objectives
- Entering the supplier's order confirmation.
- Check prices.
- Entering a collective order confirmation for several purchase orders.

### Benefits
- You can check the prices together with the order confirmation.
- The prices of several purchase orders can be checked in a collective order confirmation.

### Please note:

- **Status**: After checking the prices and invoices, the document status is raised. This is why price and/or invoice control cannot be repeated in connection with a lock status.
- **Differences**: You can complete the price or invoice control only if there is no difference between the defined total and the total of the purchase orders displayed.
- **Quick entry**: If you enable the menu **Options > Quick entry**, the cursor switches directly to field **Invoice total** or **OC total** when you enter the P.O. number. You can use this option if you usually enter just one P.O. number.
- **Document lock**: Reference documents are locked for other users while the price and invoice control is run.
- **Default settings**:
  - **Company data**:
    - Tax tab
    - Pricing tab
    - Print tab
    - Stock/PP/EDI tab

### Incoming invoice

Prices can be checked based on the supplier's order confirmation or based on the supplier's invoice. The **Price control** and **Invoice control** dialogs have the same structure. This allows you to correct the prices and update your purchase prices (PP) in the documents.

During price/invoice control, access of the respective purchase order will be blocked for other users. In order to be able to amend the purchase order during the price or invoice control, the document can be opened directly. This permits you e.g. to enter missing surcharges without leaving price and invoice control.

The prices and invoices in electronically exchanged documents can also be checked. This function is described in connection with Electronic document exchange:
⇨ "Export/Import (openTRANS)" on page D-149

### Price corrections

You can complete price or invoice control only if there is no difference between the defined total and the total of the purchase orders displayed. Such differences can e.g. be attributed to different prices, surcharges that have not been entered, or incorrect entries.

If the amount entered does not match the purchase order or the total of purchase orders, prices have to be corrected in the items or in the BOM – or return the order confirmation/invoice and ask for correction.

After invoice control, the purchase orders get the appropriate status and are now ready for to be released and transferred to financial accounting.

The status of the purchase order is changed accordingly after checking, correcting and confirming the prices.

### Purchase prices in the order

The PP of a reference order can only be updated for the amount of time allowed by the locking status. The status of the purchase order is raised after the invoice control is complete. Price or invoice control cannot be run again afterwards.

### Footer surcharges and discounts

The footer surcharges/discounts of a purchase order, e.g. an energy surcharge, are saved in the costs of the order. The footer surcharges/discounts are distributed to the individual items and are shown in document management. This way, the contribution margin shown at item entry is always up to date, even for ordered items.

As an option, the item **Delivery fee per P.O.** can be added during invoice control. This way, you do not have to enter it manually later in the purchase order.

### Foreign currency

If you are using several currencies, you can confirm the prices and invoices in foreign currency. The prices of the P.O. items are saved in national currency. The purchase prices are updated on the basis of the currency conversion.

### Collective order confirmation and collective invoice

If your supplier has collected several purchase orders in an order confirmation or invoice, this can be checked and accepted only if all purchase orders show the same VAT rate and the same currency.

If one of your suppliers usually issues collective invoices, it may be useful to define a special Number Manager for purchase orders sent to this supplier.

### Save purchase price

The purchase price is saved in the reference orders if it has been changed during price or invoice control and/or when booking the receipt of goods. The amended purchase prices are used to calculate the contribution margin, to evaluate the stock, or for stock P.O.s.

The corresponding option to determine the purchase price must be enabled in company data, and the purchase price tables must be maintained appropriately.

*Fig. D-91: Company data – Stock/PP/EDI tab* shows purchasing settings with options to calculate purchase price based on "Average purch. price" or "Last purch. price".

## Checking the invoice

Prices can be checked in the order confirmation as well as in the supplier's invoice. Two dialogs are available for this purpose which are identical in structure and function:
- Price control
- Invoice control

Price control has already been introduced in the unit *Enter order confirmation and check prices*. Just like with price control, you can check the supplier invoice and release for payment.

> **Define cursor position**
> If you enable the menu **Options > Quick entry**, the cursor switches directly to field **Invoice total** or **OC total** when you enter the P.O. number. You can use this option if you usually enter just one P.O. number.

### How to check a received supplier's invoice

1.  Go to the menu **Documents > P.O.s > Invoice > Invoice control**.

    *Fig. D-92: Invoice control* shows the "Invoice Control" window.
    - **A**: Invoice number field.
    - **B**: Invoice date field.
    - **C**: Invoice amount (net/gross) section.
    - **D**: Purchase order number(s) field.
    - **E**: Exchange rate field.

2.  Enter the invoice number (A), the date (B), and the P.O. number (D) and use `<Tab>` to go to the next field.
    The purchase order is displayed in the **P.O.s** overview.

    If an invoice covers several purchase orders, you can enter the P.O. numbers one by one. The P.O.s are added to the list. You can only combine purchase orders with the same tax rate however.
    To remove a purchase order from the overview, select it and press `<Del>`.

3.  Enter the invoice total (C).

    > **Currency**
    > If you are using just one currency (EUR), the entry in field **Rate (E)** must be 1.

4.  To confirm the entry, go to the menu **Start > Execute**.
    The amount will be checked and the **Items** tab appears.

    *Fig. D-93: Invoice control – Items* shows the "Items" tab.
    - **A**: Item price, which can be edited.
    - **B**: Difference across all items, which should be zero for completion.

    You can level out price differences by changing an item price. Amended amounts will be saved in the reference documents.

5.  If no (more) differences are shown, go to **Start > Execute**.
    The data is saved, and the status of the purchase order(s) changed. Invoice control cannot be run again for this document after that.
    Purchase price calculation is corrected in the corresponding purchase orders and orders if this option has been enabled in the menu **Options > Group > Settings**.

**Additional information**
- **Software Reference**, "Price control" on page D-203
- **Software Reference**, “Invoice control – Purchase orders" on page D-246

## Exercises

The structure of the exercises is such that every aspect of purchasing is conveyed. This means that you are going to further edit the purchase orders from the previous subject now.

**Enter receipt of goods**
Enter all receipt of goods for a reference P.O. and check if the status of the order has changed.

**Enter partial receipt of goods**
Enter a partial delivery for a reference P.O. and for a manual P.O.
Enter receipt of goods for a stock P.O. and for an item that includes products which are not kept on stock (partly or completely).

**Enter receipt of boxes**
Enter the partial or complete receipt of boxes.

**Check deliveries for completeness**
Search for purchase orders, for which items or sub-items have not been delivered yet.
Make up for the entry of the receipt of goods by making a complete booking.

**Check the invoice**
Enter the invoice for the receipt of goods.

## Electronic document exchange

This subject shows you how to adapt A+W Business for electronic document exchange, and how to export and import documents.

You can exchange documents electronically with your suppliers/customers.

To exchange purchase orders, data is saved in an ASC file. In order to exchange invoices or order confirmations, data must be available in openTRANS format (XML format).

*Fig. D-94: Data export and import*
This diagram illustrates the flow of electronic documents.
- A **Customer** using **A+W Business** creates a "Customer order" which is a "purchase order".
- This is sent via **EDI** to the **A+W Business** system of the **Supplier**, where it becomes a **P.O.**.
- The **Supplier** then sends an "Order confirmation (OC)" and an "Invoice" back to the **Customer** via the **openTRANS** format.

Purchase orders can be exchanged via EDI. From the customer's point of view, the customer order is a purchase order while for A+W Business, it is an order.

Order confirmations and invoices can be exchanged in openTRANS format. This requires that all parties involved are using A+W Business. This function will be explained in detail in the following chapters.

### Export/Import (openTRANS)

#### Objectives
- Learning about the functional principle of electronic document exchange
- Learning about the settings and how to adapt them
- Learning about mandatory fields in documents
- Dispatch and import of electronic documents

#### Benefits
- Electronic document exchange can be used to import documents from your customers and suppliers without having to enter the individual data.
- Data import helps to reduce input errors.

#### Please note:

- **Prerequisite**:
  - The supplier/customer has to have the same A+W Business version as yourself, at least A+W Business 5.
  - The necessary services must be installed and started.
- **Data format**: Electronic documents can be exchanged in openTRANS and in XML format.
- **Data import**: Data can be sent as files by email or saved on a shared drive on a server.
- **Data export**: Whenever an order confirmation or an invoice is printed, the program checks whether there are documents with the code for the export flag. These documents will be automatically sent to the defined email address.
- **References**: Document references are created from the following fields:
  - In the order header, field **P.O. text1**
  - At item entry, field **Customer item**
  These fields always have to be filled in.
  If these references cannot be established in imported documents, allocation has to be done later by hand, when checking the electronic document.
- **Partial deliveries**: Partial deliveries can be created from an electronic order confirmation.
- **Rounding differences**: At price and invoice control, rounding differences of just a few cents are acceptable if a so-called balancing item has been defined in product management to which differences can be booked.
- **Collective invoices**: For collective invoices issued by the supplier, a surcharge which appears just once can be distributed to all items of the purchase orders or P.O. items involved.
- **Document lock**: Reference documents are locked for other users while the price and invoice control is run.
- **Default settings**:
  - **Master data**:
    - Product data
    - Customer/supplier data
    - Status definition
    - Status allocation
    - Currencies
  - **Company data**:
    - Parameters tab
  - **Master data**:
    - B2B customer/supplier
