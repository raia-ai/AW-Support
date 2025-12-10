---
title: "EN_AWBusiness_Inventory_Management_6_2-1"
source: "EN_AWBusiness_Inventory_Management_6_2-1.pdf"
tags: ["A+W Business", "Inventory Management", "Stock Management", "Purchase Order", "P.O. Proposal", "Stock Search", "Future Stock", "Automatic P.O.", "Manual P.O.", "Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial on stock management within the A+W Business software. This guide covers viewing future stock, handling automatic and manual purchase orders (P.O.s), transferring P.O. proposals to purchasing, comparing supplier prices, and managing stock articles within documents like sales orders."
long_description: "This document is a detailed tutorial from the A+W Business Inventory Management guide, focusing on stock management processes. It begins by explaining how to view future stock on hand, which helps in planning and forecasting. The guide then delves into the creation of Purchase Orders (P.O.s), differentiating between automatic and manual methods. It provides step-by-step instructions on how automatic P.O. proposals are generated when stock levels fall below a defined minimum and how these proposals can be reviewed, modified, and transferred to the purchasing department. The tutorial also covers how to manually create a stock P.O. The document details the process of comparing supplier prices for a P.O. proposal, allowing users to select the best supplier based on price or delivery time. Furthermore, it explains how to integrate stock articles into documents such as sales orders, including searching for available stock, handling reservations, and what happens to stock bookings when an order is modified. The guide uses screenshots and numbered steps to walk the user through various dialogs like 'Stock Search,' 'Stock P.O. - Order pool,' and 'Price Comparison.' It's designed for users who need to learn the practical application of inventory control features within the A+W Business software."
---

---
## Tutorial: Stock Management

7. Click on [End] to close the dialog.
   Dialog Stock search reopens.
8. To view the next withdrawals and receipts for a product or the future stock on hand, select the product in question and go to tab **Future stock on hand**.

*(Image: A screenshot of the 'Future stock on hand' tab showing a table with dates, reservations, purchase orders, and closing inventory.)*
**Fig. G-53 Future stock on hand**

The future stock on hand is shown for the future period that has been defined in the company data for the preview. Sundays and public holidays will be shown as well but they do not count.

### Exercises

-   Check the stock and reservations for Float 4 mm:
    Take a note of the individual values on tab **Future stock on hand**. In the next module, you are going to enter a P.O. and subsequently check how the values have changed.

### Additional information

⇨ Software Reference, "Search" on page G-217

## Stock P.O. (automatic)

### Objectives

-   Getting familiar with the Stock P.O. dialog.
-   Learning about automatic stock P.O.s.
-   Transferring automatic P.O. proposals to Purchasing.
-   Check the changes to the displayed values in the future stock on hand.

### Benefits

-   Purchase orders serve to complete the stock on hand to achieve the required target inventory or match the reservations.
-   If the stock on hand fails to reach the defined minimum, a P.O. proposal is created automatically. You can check this in dialog Stock P.O. and transfer it to Purchasing.

### Please note:

-   **Manual input of stock P.O.**: Stock POs are entered and edited in module Documents. This process is described in section Purchasing.
-   **P.O. proposals**: Automatic P.O. proposals are triggered when the stock fails to reach the defined minimum quantity. Reservations and open purchase orders are taken into account. P.O. proposals are created automatically and are manually transferred to Purchasing. This transfer creates a P.O. which can be sent to the supplier.

### Default settings

-   **Master data:**
    -   Product management
    -   Supplier file
-   **Company data:**
    -   Parameters tab
    -   Tab Stock/PP/EDI
-   **Stock management:**
    -   Minimum stock
    -   Purchase order quantity

## P.O. Proposals

Purchase orders are usually created through stock management in order to keep the stock on hand on the required level.

*(Image: A screenshot showing the 'Stock management - Stock on hand figures' dialog with fields for stock articles, minimum stock, and purchase quantities.)*
**Fig. G-54 Stock management - Stock on hand figures**
- **A** Minimum stock
- **B** Quantity for P.O. proposal

If you have defined minimum quantities (A) for a stock article in dialog Stock management, P.O. proposals are created automatically with the stored P.O. quantity (B). You can check these before they are transferred to Purchasing, and change the supplier and date if necessary. Transfer to Purchasing turns the proposal into a stock P.O.

Stock P.O.s can also be created manually, via document management. Manual stock P.O.s will be introduced in a separate training module.

## Transfer Stock P.O. to Purchasing

Automatically created P.O. proposals are shown in the dialog Stock P.O - Order pool. You can change the supplier and the date. The P.O. is issued upon transfer to Purchasing. This has to be sent to the supplier.

If several suppliers have been entered for a product, you can compare delivery dates and prices in the order pool and select another supplier if required.

This module shows you how to transfer a P.O. proposal to Purchasing.

> **Stock P.O. dialog**
> Dialog **Stock P.O. - Order pool** is almost identically structured as the dialog P.O. transfer which has been introduced in the session on Purchasing. The dialogs are different however. For every P.O. proposal you will therefore find just one entry for which there are no reference documents.

The following instructions exist for this training module:
-   "How to transfer P.O. proposals to Purchasing" on page G-105
-   "How to change the supplier and the delivery date" on page G-108

### How to transfer P.O. proposals to Purchasing

1.  Go to menu **Stock management > Stock P.O.**
    Dialog **Stock P.O.** opens.
    If you do not want to view P.O. proposals for the entire stock, you can restrict the view to certain storage locations.
2.  To restrict the view, define the requested storage location in the fields **Warehouse**, **Corridor**, **Shelf**, and **Tray**.

*(Image: A screenshot of the 'Stock P.O.' dialog, showing the 'Order pool' tab which is currently empty.)*
**Fig. G-55 Order pool**

In this example, no storage location is selected so that the stock on hand is listed for all storage locations.

3.  To start the search, go to the menu **Start > Search**.
    The proposals are loaded and listed.

*(Image: A screenshot of the 'Order pool' tab now populated with 20 P.O. proposals, showing columns for Supplier, Article, Quantity, and Delivery date.)*
**Fig. G-56 Stock P.O.- P.O. proposals**

4.  Select the P.O. proposals you want to transfer to Purchasing.

> **Select several entries at once**
> You can select several P.O. proposals at once by opening the dialog **Marking options** in the **Functions** menu. For example, if you enter a certain product in this dialog, then all P.O. proposals for this product are marked with a cross in the line header.

*(Image: The same 'Order pool' screenshot as before, but with 'X' marks next to three selected line items.)*
**Fig. G-57 Selected P.O. proposals**

Double-click on the corresponding line header. Only the proposals marked by an X will be selected.

5.  To start the transfer to Purchasing, go to the menu **Start > Execute**.
    Confirm the message regarding the number of transferred proposals.
    Purchase orders are created and the transferred proposals are removed from the list.

### How to change the supplier and the delivery date

1.  Load the P.O. proposals in dialog Stock P.O. as described above.
2.  Select the proposal the supplier and/or delivery date of which shall be changed.
    Double-click on the corresponding line header. Only the proposals marked by an X will be selected.

*(Image: A screenshot of the 'Order pool' with a specific proposal selected, ready to be assigned a different supplier.)*
**Fig. G-58 Proposal to be assigned a different supplier**

3.  Go to the menu **Functions > Change supplier/delivery dates**.

*(Image: A small dialog box titled 'Change supplier and delivery dates' allowing the user to change the supplier and delivery date for the selected P.O. proposal.)*
**Fig. G-59 Change delivery date**

4.  Enter another supplier and/or delivery date.
5.  Click on [OK] to adopt the change.
    The dialog **Change supplier and delivery date** closes. The proposal is listed with the new supplier and/or delivery date.
    You can now transfer the P.O. proposal to Purchasing.

## Compare Prices before Transfer to Purchasing

If several suppliers have been selected for a product, you can compare prices before the transfer, and choose a different supplier. This module shows you how to compare prices and choose the supplier with the best price or the shortest delivery time.

### How to compare the prices in a P.O. proposal

1.  Go to menu **Stock management > Stock P.O.**
    Dialog **Stock P.O.** opens.
2.  Select the requested storage location in the fields **Warehouse**, **Corridor**, **Shelf**, and **Tray**.
3.  To import the P.O. proposals, go to the menu **Start > Execute**.
    The proposals are loaded and listed.
4.  Select the proposal the supplier prices of which you want to compare.
    Double-click on the corresponding line header. Only the proposals marked by an X will be selected.

*(Image: A screenshot of the 'Order pool' with a specific P.O. proposal selected, ready for price comparison.)*
**Fig. G-60 Item the prices of which shall be compared**

5.  Go to the menu **Functions > Supplier prices**.

*(Image: The 'Price comparison' dialog showing different suppliers for an item, their prices, delivery times, and highlighting the default and low-price suppliers.)*
**Fig. G-61 Change the supplier of the selected item**

-   **A** Standard supplier (text in red)
-   **B** Checkbox of standard supplier (not selected)
-   **C** Selected supplier for the current P.O.
-   **D** Checkbox for selecting the supplier (selected)
-   **E** Text color red: Standard supplier
-   **F** Text in green: most favorable supplier in terms of price
-   **G** Text color blue: Standard supplier is the most favorable in terms of price
-   **H** !!! for all text colors: Delivery date may be too late for timely production and shipment to the customer

6.  Check the checkbox left from the supplier to whom the purchase order for this item is to be sent.
7.  Click on [OK] to adopt the change.
    The dialog **Price comparison** closes. The proposal is listed with the new supplier and/or delivery date.
    You can now transfer the P.O. proposal to Purchasing.

### Exercises

-   Define the minimum and P.O. quantity for a stock article so that an automatic P.O. proposal is created. Choose the stock article for which you have noted the values of the future stock on hand in the previous exercise.
-   Check the P.O. proposal and change the supplier or delivery date. If no alternative suppliers are displayed, you have to check and amend the supplier file in the master data.
-   Transfer the P.O. proposals to Purchasing.
-   Check the changed values in dialog Stock search.

### Additional information in section Sales

-   ⇨ Sales, "Order Header" on page C-38
-   ⇨ Sales, "Change P.O. Code" on page C-306
-   ⇨ Purchasing, "Supplier file amendment" on page D-32
-   ⇨ Purchasing, "Document P.O." on page D-43
-   ⇨ Purchasing, "Enter receipt of goods" on page D-125
-   ⇨ Purchasing, "Dealing with boxes" on page D-134

## Stock Articles in Documents

In this thematic block you will learn how orders and manual purchase orders access stock management.
This includes the following training modules:

-   "Order Entry of Stock Products" on page G-114
-   "Manual Stock P.O." on page G-122
-   "Production Orders" on page G-126

## Order Entry of Stock Products

### Objectives

-   Search stock articles for item entry.
-   Check reservation.
-   Check changes to stock on hand after a change of order.

### Benefits

-   The availability of a product can be checked at item entry. In case of bottlenecks, the supplier or delivery date can be changed directly in the document.

### Please note:

-   **Item entry**: Stock articles are selected at item entry by means of the stock search [F3].
-   **Reservation**: Stock articles entered in the order are marked as reserved on stock.

### Default settings

-   **Master data:**
    -   Product management
    -   Supplier file
-   **Company data:**
    -   Parameters tab
    -   Tab Stock/PP/EDI

## Reservation and Booking of Stock Articles

At order entry, the quantity or number of sqm of the stock articles is automatically reserved for the customer order. Goods withdrawn from stock are automatically booked upon printing of the delivery note or invoice. Based on the quantities sold and ordered, A+W Business calculates the actual stock on hand.

### Stock on hand after a change of order

What happens to the stock on hand if orders are changed for which goods have already been withdrawn? In the following examples, withdrawal of goods will be booked when the delivery note is printed.

| Change of order | Result in order | Stock booking |
| :--- | :--- | :--- |
| Change order header, no change of items | Status remains the same. | When the initial delivery note is printed again, no additional stock withdrawal will be booked. |
| Delete item afterwards | Status is 72 and remains unchanged. | Query whether the stock on hand shall be corrected. |
| Add new item afterwards | | Query whether the stock on hand shall be corrected. |
| Additional change of quantity afterwards | | Stock on hand is automatically corrected, without any further notification. |

The next modules will show you how to enter a stock article in a document, and check the booking.

## Search Stock Article for an Item

This module will show you how to enter an item, at the same time checking the availability of the required product. Open dialog Stock search (which has been introduced in the previous module).

> **Stock search at a P.O. entry**
> You can also select a stock article via dialog Stock search when you enter a stock P.O. manually. The manual stock P.O. is described in the training module of the same name.

### How to enter a stock article as an item

1.  Go to menu **Documents > Order > Order** and enter the order header.
2.  Go to item entry and enter the product number in the input line.
3.  Go to the menu **Start > Stock search** to open the dialog **Stock info**.
    The selection in dialog **Stock info** is already restricted to the article you have entered for the item. You have to filter the view further now, e. g. by restricting the settings to stock sizes and stock on hand which are over zero.

*(Image: A 'Filter options' dialog for searching stock articles.)*
**Fig. G-62 Filter for searching for stock articles**
- **A** Switch stock size display on or off
- **B** Show only stock articles with a stock on hand of over 0

4.  Go to tab **Future stock on hand** to check whether the production dates are jeopardized.
    Display of the future stock on hand in dialog **Stock info** has already been introduced in the module on Stock info.
    ⇨ "Display of the future stock on hand" on page G-97

*(Image: A screenshot of the 'Future stock on hand' tab within the Stock info dialog.)*
**Fig. G-63 Future stock on hand**

If the replacement time is too short, you can still enter the product then check whether another supplier is available or whether you have to change the delivery date.

5.  Go to tab **Stock search** and double-click on the stock article you want to adopt for item entry.

*(Image: A screenshot of the 'Stock search' tab showing a list of stock articles with details like name, dimensions, storage place, and stock on hand.)*
**Fig. G-64 Select stock article**

Dialog **Stock info** closes and the item entry data is updated.

6.  Enter all item data and return to the document header.
    If the replacement times are too short, you can view the articles in question in dialog **Change delivery date**.
7.  Click on the icon next to the shipping date to open the dialog.

*(Image: A screenshot of an order document header with the 'Edit delivery date' dialog open. This dialog shows products with low stock and lists possible suppliers with new delivery dates.)*
**Fig. G-65 Check delivery date in the order**
- **A** Check delivery date
- **B** Products for which the stock on hand is too low
- **C** List of possible suppliers and shipping dates for the selected product

Alternative suppliers from the supplier file are shown with the defined replacement time and the corresponding date.

Double-click on the article in the list on top (B) to open the **Stock info** with details on the articles.

8.  If the scheduled delivery date is jeopardized, the following options are available:
    -   Change the supplier for the item in question or for the entire order.
    -   Change the delivery date and inform the customer.

These steps are described in detail in the tutorial on Sales.

9.  Go to the menu **Start > Save** to save the data.
    The data is saved. You can now check the reservation of stock articles.

## Check the Bookings

In this module you will learn how to check the bookings for stock articles. Saving reserves the item. Withdrawal of goods is generally booked when the delivery note is printed. Printing depends on the settings in status management.

### How to check the bookings

1.  Open the **Booking journal** dialog as described in section Queries.
2.  Restrict the selection to the order for which you want to check the reservation.
    The list shows all order items with the current booking type.

*(Image: A screenshot of the 'Booking Journal' showing two items for an order with the booking type 'reserviert/reserved'.)*
**Fig. G-66 Booking - reserved**

The booking journal shows the booking type **reserved** only until withdrawal of goods is booked.

After the goods are withdrawn, the order items are marked as **shipped**.

*(Image: A screenshot of the 'Booking Journal' showing the same two items, now with the booking type 'ausgeliefert/delivered'.)*
**Fig. G-67 Booking - shipped**

The order history shows the individual status changes based on the print-outs and inventory bookings.

*(Image: A screenshot of the 'History - Order' dialog, showing a log of all actions and status changes for a specific order, from entry to invoice printing.)*
**Fig. G-68 Order history**

### Exercises

-   Enter an order with existing stock articles and check the entries in the booking journal:
    -   After order input.
    -   After printing the delivery note. Which changes are visible?
-   Enter an order and check the stock on hand and the reservations.
-   Issue an invoice for the order and check the stock reservations again.

## Manual Stock P.O.

### Objectives

-   Introducing the special features of the stock P.O. in document management.

### Benefits

-   Manual stock P.O.s are used to complete the stock on hand, e. g. for large-scale orders for which automatic reordering alone is insufficient.

### Please note:

-   **Document type**: The document **Stock P.O.** is a separate document type. Receipt of goods can be booked to stock only for stock P.O.s.
-   **Default settings**:
    -   **Master data:**
        -   Product management
        -   Supplier file
    -   **Company data:**
        -   Parameters tab
        -   Tab Stock/PP/EDI

## Manual Input of Stock P.O.

Purchase orders for stock articles can be triggered automatically, or entered manually. Automatic P.O. proposals have been introduced already in the module on the automatic stock P.O.

This module will show you how to enter a stock P.O. manually. Document input is described in detail in sections Sales and Purchasing. The following instructions therefore concentrate on the main steps.

### How to enter a stock P.O. manually

1.  Go to menu **Documents > P.O. > P.O.**
    The dialog **Document management** opens.
2.  Enter the document header. Enter at least the supplier and the delivery date.

*(Image: A screenshot of the document header for a new P.O., showing fields for supplier, delivery date, and document type.)*
**Fig. G-69 Stock P.O.**
- **A** Document type
- **B** Setting the document type

3.  Select the entry **Stock P.O.** in field **Type** (B).
    If you set another document type, receipt of goods is not automatically added to the stock on hand.
4.  Enter the item(s).

> **Items without stock codes**
> If you enter stock P.O.s with items which are not recorded as stock items, they will not be displayed at receipt of goods. You can however enable the corresponding option in master data **Company > Company data > tab Stock / PP / EDI**.

5.  Go to the menu **Start > Save** to save the data.
    The data is saved.
6.  Print and send the purchase order.
    This process is described in section Sales.

### Exercises

-   Check the stock on hand for a stock article.
-   Enter a stock P.O. manually and check the corresponding values again in the **Stock info** dialog.

