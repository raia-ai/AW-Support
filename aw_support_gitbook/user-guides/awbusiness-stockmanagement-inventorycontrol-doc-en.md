---
title: "EN_AWBusiness_Box_Management_1_1-3"
source: "EN_AWBusiness_Box_Management_1_1-3.pdf"
tags: ["stock management", "inventory control", "A+W Business", "box management", "purchase order", "barcode scanning", "goods receipt", "shipping", "software tutorial", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive guide for managing stock, specifically boxes, within the A+W Business software. It provides both a tutorial for common workflows and a detailed software reference for system dialogs and functions."
long_description: "This document serves as a user manual for the Box Management module in the A+W Business software. It is divided into two main parts: a Tutorial and a Software Reference. The Tutorial section provides step-by-step instructions for performing key stock management tasks related to boxes. These tasks include entering manual stock purchase orders (P.O.s), receiving goods via barcode scanning, processing the shipping and withdrawal of boxes from stock, and handling various manual stock adjustments. The manual booking section details how to create new boxes in inventory, book the dispatch of goods, change a box's storage location, correct the number of sheets in a box, and open (resolve) boxes into individual sheets. The Software Reference section offers a detailed description of the core modules and dialogs used for these processes. It covers the Stock Management and Stock Movement functionalities, explaining the various tabs, fields, menus, and options available to the user. This guide is intended for warehouse personnel, inventory managers, and system administrators who use A+W Business to control and track their inventory of boxes."
---

# Tutorial

---
## Stock Management for Boxes

### Entering manual stock P.O. of boxes

The following guideline shows how to enter a stock P.O. for boxes. Manual P.O.s are described in detail in the Purchasing section.
⇨ Purchasing, "Manual purchase order" on page D-77

**How to enter a stock P.O. with boxes**

1.  Go to the menu `Documents > P.O. > P.O.`
    The dialog **Document management** opens.
2.  Go to field **Type** and select the entry **Stock P.O.**
    *(The image displays a dropdown menu showing the selection of "Lagerbestellung / Stock P.O." for the "Type" field.)*

    > If you set the type to `<n.s.>`, goods received cannot be automatically added to stock.

3.  Go to the **Items** tab.
4.  Enter the product number, e.g. 1005.
    You can specify the number after selecting the stock article. You do not need to enter sizes as they are taken from the stock article.
5.  Go to the menu `Start > Stock search` to open the **Stock info** dialog.
    You can also open this dialog by pressing `<F3>`.

*(Fig. K-33: Stock info - stock search)*
The **Stock info** dialog opens providing a list of all boxes and stock sizes. For boxes, the entry in column `Cont.` is greater than 1. The image shows a dialog with a list of stock articles, with callout `A` pointing to the "Product number of glass type" and callout `B` pointing to a "Box (without ID)".

6.  Select the required box without box ID and accept it by a double click.
    The dialog is closed and you will find yourself back at item entry. In the input line, you will find that all fields from **Quantity** onwards are locked for boxes. The price fields are updated.

*(Fig. K-34: Box at item entry)*
The image shows the P.O. item entry screen after a box has been selected. The quantity fields are highlighted. Callout `A` points to the `Pcs.` (pieces) field and callout `B` points to the `Qty.` (quantity) field.

7.  Enter the amount required.
    The display of details is updated.
8.  Repeat steps 4 to 7 to enter all P.O. items.
9.  Go to the menu `Start > Save` to save the data.
    The data is saved.
10. Print and send the purchase order.

### Receipt of Goods via Barcode

In general, all stock bookings are entered via PDC (plant data collection). For this, the boxes must each have their own barcode label.

> **Labels for receipt of goods**
> In order to enter a self-produced box in receipt of goods via PDC, a label/barcode is required. For this, the print item 973 must be assigned.

**How to enter a box via barcode**

1.  Go to the menu `Documents > P.O.> Receipt of goods > Receipt of goods`.
2.  Select the **Scanner** option and scan the box's label.
3.  Go to menu `Start > Execute`.
    If you have a barcode for the receipt booking, you can scan it. This way, the box is included in the inventory in the default stock location. You can scan and then book all produced boxes one after another.
4.  Change to the **Item-by-item** tab and check the **Book complete** checkbox for the box.
    *(Fig. K-35: Booking item by item shows the 'Receipt/Dispatch' screen with the 'Per Item' tab active. The list shows an item '106-Float 6 mm Kiste/case' with a checkbox for 'Book'.)*
5.  Go to menu `Start > Execute`.
    Thus the box is booked and present in the inventory.

*(Fig. K-36: Warehouse search - box with ID in inventory shows a list of stock items, including boxes with and without specific IDs, displaying quantities like 'Stock on Hand', 'Res.' (Reserved), and 'Available'.)*

### Shipping of Boxes

Boxes are usually withdrawn from stock when the delivery note is printed. Printing of the invoice can also be used as a trigger for the withdrawal.

#### Withdrawal of boxes

Boxes are usually withdrawn from stock when the delivery note is printed. Printing of the invoice can also be used as a trigger for the withdrawal.

As the person who enters the order will not know which box is actually going to be shipped, he first enters a dummy box with the required sizes. The stock on hand can only be updated after the ID of the real box is entered and withdrawn from stock.

**Example**
A dummy box (without ID) with the required sizes is entered in the order. 3 is specified as the quantity. This reserves three of the dummy boxes.

**Table K-2: Withdrawal of boxes before or after printing the delivery note**

| Withdrawal Before printing the delivery note | Withdrawal After printing the delivery note |
| :--- | :--- |
| • The real box IDs are scanned in the issuing area. | • The delivery note is printed. |
| • Reservation of the dummy box is canceled. | • The reserved dummy boxes will be withdrawn. |
| • The three boxes with IDs are marked as reserved. | • When the boxes are issued, the three real box IDs are scanned. |
| • The delivery note is printed. Three boxes are booked upon issue of goods. | • Reservation of the dummy boxes is canceled. |
| | • The three boxes are withdrawn. |

The following steps have usually been taken already:
*   The product was entered in the customer order:
    *(Fig. K-37: Product 1005 entered shows an item line for the product.)*
*   `[F1]` in the Stock info dialog was used to select the dummy box:
    *(Fig. K-38: Selection of the dummy box shows the Stock Search dialog. Callout A points to a 'Dummy box without ID'. Callout B points to the 'Reservation of dummy box' column showing current reservations.)*
*   The box was added to the order and saved, e.g with an item quantity of 3:
    *(Fig. K-39: Item quantity 3 saved shows the item line in the order with a quantity of 3.)*
*   3 additional reservations were booked for the dummy box on stock:
    *(Fig. K-40: Reservation shows the stock overview with the dummy box reservation increased by 3, indicated by callout A.)*
*   The booking journal (stock management) shows the item quantity as reserved:
    *(Fig. K-41: Order item reserved shows the Booking Journal with a line item for the reservation of 3 units of the product.)*

Next, boxes with IDs are allocated and withdrawn after printing the delivery note.

### Booking of issued goods

**How to book the issue of boxes**

1.  Go to the menu `Production > Dispatch > Issue of boxes`.
    *(Fig. K-42: Issue of boxes - load customer order shows the 'Shipment cases' selection screen with options to load an order by various criteria like 'By Order Number' or 'By Scanner'.)*
2.  Select the option **By scanner**.
3.  Enter the barcode of the order number and item number.
    The numbers appear in the **Document** fields.
    If you are not using a scanner, choose the option **By order number** and enter the number.
4.  To import order data, select `Start > Execute`.
    The display switches to the **ID** tab.
    *(Fig. K-43: Order item with sub-items shows the ID tab where individual boxes (virtual items) for an order are listed. The 'ID' column is initially empty.)*
    Each box is shown in a separate line as a virtual item. The fields in column **ID** are empty as no box with an ID has been allocated.
5.  Scan the box ID of the first box to be reserved.
    If you do not use a scanner, go to field **ID** and select one of the displayed IDs. The list only shows box IDs of the defined type.
6.  To allocate the boxes, go to the menu `Start > Execute`.
7.  Repeat steps 5 and 6 to allocate more boxes with IDs.

**Additional Information**
*   ⇨ Master Data, "Company Data – Parameters" on page B-934
*   ⇨ Master Data, "Use virtual item numbers" on page B-940
*   ⇨ Sales, "Stock Info" on page C-736
*   ⇨ Software Reference, “Issue of Goods" on page E-236

### Manual Stock Bookings

If you are not working with PDC, you also start all stock bookings manually.
This section provides information on the following subjects:
*   "Manual input of addition" on page K-60
*   "Change storage location of a box" on page K-64
*   "Correcting the box contents (number of sheets)" on page K-65
*   "Opening (resolving) boxes" on page K-66

#### Manual input of addition

You can receive boxes manually into inventory or withdraw them from inventory.

> **Prerequisite**
> The checkbox for the virtual assignment of item numbers must be checked in company data.
> ⇨ "Company Data" on page K-18

The following instructions exist for this training module:
*   "How to set the ID for boxes" on page K-60
*   "How to create a new box in inventory" on page K-60
*   "How to book the dispatch of goods manually" on page K-62

**How to set the ID for boxes**

1.  Go to the menu `Documents > P.O.> Receipt of goods > Receipt of goods`.
2.  Go to the menu `Options > Group > ID number allocation > Settings`.
    *(The image shows a 'Settings' dialog for 'Stock ID Number' with a preset format 'AUTOXXXXXX'.)*
3.  Replace the sequence of letters with the desired ID.
    Please avoid overwriting the placeholders for the numbers.
4.  Click on [OK] to save the changes.

**How to create a new box in inventory**

1.  Go to menu `Stock management > stock management`.
    The **Stock management** dialog is displayed.
2.  From the menu, select `Options > Assign ID number automatically`.
    This way, the automatic ID is assigned for boxes with the new ID. Counting begins with each new ID at 1 and is incremented by 1 each time. The **Ident** field on the **Stock article** tab is locked.
3.  In the **Article** field, enter the product number of the glass for which a box should be booked.
4.  Go to menu `Start > Search`.
    *(Fig. K-44: Box data shows the Stock Management screen. Callouts point to A: Storage location, B: Stock on hand, C: Box, D: Stock article without ID.)*
5.  Mark the box (C, D) for which you want to enter the stock on hand.
    Thus, all required data will be taken over and you can create a new box in the stock on hand.
6.  Go to the menu `Start > New`.
    The fields will be enabled.
7.  Select the storage location (A) where the new box is located.
8.  Enter the number 1 in the **Stock on hand** field.
    Since each box should have its own ident number, you may only enter 1.
9.  Go to the menu `Start > Save` to save the data.
    In the field for the stock on hand, a new box is displayed with an ID.
10. Repeat steps 6 and 9 until you have included all boxes in the stock on hand.
    Pay attention here whether all boxes should be booked to the same storage location. You don't need to change any other values until you have booked all boxes.

**How to book the dispatch of goods manually**

1.  Go to menu `Stock management > Stock movement > tab Dispatch`
2.  Enter the either the product number or the ident number of the box and select `Start > Search` in the menu.
    The search will be restricted to this box in that case. Alternatively, you can restrict the search to a product code and the storage place. Section **Storage locations** lists all stock articles matching the search criterion.
    *(Fig. K-45: Manual stock dispatch of boxes shows the Stock Movement dialog on the 'Exit' tab, with a list of stock items in various storage places.)*
3.  Mark the box that you want to withdraw.
4.  Enter a 1 in the **Quantity** field in order to reduce the stock on hand by the marked box.
5.  If necessary, change the booking date and enter a note.
6.  Go to menu `Start > Save` to save the data.
    Data will be saved, and the stock on hand set to 0.

#### Change storage location of a box

This module will show you how to move a box from one storage location to another. This movement will be entered with a rebooking. This way, the stock article will be booked from the old storage location as a withdrawal and as an addition to the new one.

**How to transfer the storage location**

1.  Go to menu `Stock management > Stock movements`.
    Dialog **Stock movement** opens.
2.  Go to tab **Transfer**.
3.  Enter the product number in the **Product** field or the (box) ID.
4.  To start the search, go to the menu `Start > Search`.
    *(Fig. K-46: Stock movement - Transfer shows the 'Transfer' tab in the Stock Movement dialog. Callout A points to the current storage location, and B points to the field to select a new storage location.)*
5.  Mark the box that you want to transfer to another storage location.
6.  Choose the new storage location in section storage location (B).
7.  Go to menu `Start > Save` to save the data.
    The box is withdrawn from the old storage location, and added to the new one. If you have activated the **Log when finished** option, the **Stock history** dialog opens. You can then print out all stock movements as a log.

#### Correcting the box contents (number of sheets)

If you find out in the warehouse that the content of a box does not match the quantity shown on the delivery note, the number of sheets needs correcting. This module will show you how to correct the contents of a box.

> **Only boxes with ID**
> The content of a box can be changed only if the box has been entered with its own box ID.

**How to correct the number of sheets in a box**

1.  Go to menu `Stock management > Stock movements`.
    Dialog **Stock movement** opens.
2.  Go to tab **No. of sheets**.
3.  Enter the product number in the **Product** field or the (box) ID.
4.  To start the search, go to the menu `Start > Search`.
    *(Fig. K-47: Correct the number of sheets shows the 'No. of Sheets' tab in the Stock Movement dialog. Callout A points to the selected box in the list, and B points to the 'Contents' field where the number of sheets can be changed.)*
5.  Select the required box (A).
    Field **Contents** is enabled.
6.  Enter the new number of sheets (B).
7.  Go to menu `Start > Save` to save the data.
    The data is saved.

#### Opening (resolving) boxes

You can open boxes in order to make the sheets available for production or enter them individually in the order. You can only open boxes with an ID.

> **Stock articles with sheet dimensions must be created**
> If you break up a box, the sheets are booked to the stock on hand. The stock sizes for the sheets are created automatically if necessary. In this case, the sheets are booked to the storage location of the opened box.

**How to open a box**

1.  Go to menu `Stock management > Stock movements`.
    Dialog **Stock movement** opens.
2.  Go to tab **Open boxes**.
3.  Enter the product number in the **Product** field or the (box) ID.
4.  To start the search, go to the menu `Start > Search`.
    *(Fig. K-48: Stock movement – Open box shows the 'Open Boxes' tab. Callout A points to the box to be opened, B points to its 'Content', and C points to the 'Number of boxes' field.)*
5.  Select the required box.
    The fields **Number of boxes** and **Different contents** are enabled.
6.  Enter 1 in field **Number of boxes** and check if the contents of the box are correct.
    If necessary, correct the entry in field **Different contents**.
7.  Go to menu `Start > Save` to save the data.
    The box will be booked out and the lite as stock articles.
8.  If necessary, update the view of storage locations by reloading them.
9.  If necessary, delete the empty box from the stock on hand manually.

---

# Software Reference

## Overview

Use the module **Stock Management** to maintain and analyze all data concerning stock. Furthermore, use this module to carry out the inventory and book stock movements.

The Software Reference provides information on the following subjects:
*   "Stock Management" on page K-72
*   "Stock Movement" on page K-83
*   "Search" on page K-90
*   "Stock P.O.” on page K-96
*   "Receipt and Shipping of Boxes" on page K-102

## Stock Management

**Path:** `Stock management > Stock management`

Use the dialog **Stock management** to display all the stock articles that are managed.

This section provides information on the following subjects:
*   "Menus in Stock Management” on page K-72
*   "Stock Management" on page K-73

### Menus in Stock Management

**Path:** `Stock management > Stock management`

The menus can be used to define the standard settings of the dialog or open other dialogs without closing this dialog.

This section provides information on the following subjects:
*   "Functions Menu” on page K-72
*   "Options Menu" on page K-73

#### Functions Menu

**Path:** `Stock management > Stock management > Functions menu`

This menu allows you to open other dialogs without closing stock management.

The following entries are displayed:
*   **Stock History:** Opens the dialog **Stock History** with the log of processes that have been booked in stock management.
*   **Booking Journal:** Opens the dialog **Booking Journal** with the log of stock bookings from orders and purchase orders.

#### Options Menu

**Path:** `Stock management > Stock management > Options menu`

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

The following entries are displayed:
*   **Do not print articles with stock on hand = 0:** Only articles with stock on hand that is more than 0 will be printed. This setting is helpful if you have many boxes with an ID, but without stock. Usually, these have been delivered as boxes and were deleted from the stock. This setting applies only to printing; the dialog shows all the articles.
*   **Automatic ID allocation:** The box ID can be allocated automatically even it has been booked as stock manually.

### Stock Management Dialog

**Path:** `Stock management > Stock management`

In the Stock Management dialog you enter all the stock articles that are kept in the warehouse with stock on hand.

Stock sizes are maintained in A+W Business even in product management. They are used to allocate price codes, product groups, etc.

Dialog Stock Management offers the following tabs:
*   Stock Management - Stock Articles
*   Stock Management - Prices
*   Stock Management - Supplement

> **Stock management at the level of bills of material**
> In the warehouse, you can also manage products that are included as bill of material components in other products. For this purpose, the checkbox **Stock keeping at BOM level** must be enabled in the company data.
> ⇨ Master Data, "Stock control on BOM level" on page B-958

### Stock Management - Stock Articles

**Path:** `Stock management > Stock management > Stock articles tab`

*(Fig. K-49: Stock management - stock articles shows the main Stock Management dialog with the 'Stock Products' tab active, displaying a list of stock articles and their details.)*

Use this tab to check the articles that are managed in the warehouse. The shown stock is updated with each stock booking. You can add new articles and correct the different quantities.

For ordering purposes, you furthermore define minimum quantities and purchase order quantities.
⇨ Tutorial, "How to create a stock article" on page K-26

#### Field Descriptions

**Articles**
Product number according to master data. If you want to enter a new stock article, you have to enter it in the master data first.

**Stock ID**
Identification number, assigned on receipt of goods.

**Name**
Product names from the master data.

**Width x height / content**
Dimensions of the stock article in mm (only stock sizes) and content of box. For boxes, enter the number of sheets per box. For all other stock articles, a `1` is automatically shown.

**Variant**
If variations have been entered for an article, you will see the color here.

**Default storage location**
If you have defined storage locations, they will be offered for selection. If you keep one stock article at several storage locations, you can define a standard storage location.
*   🔲 The shown storage location is not defined as standard for the stock article.
*   ✅ The shown storage location is defined as standard for the stock article.
⇨ Master Data, "Stock Definition" on page B-736

> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations `<n.e.>` will remain and can be booked.

**ID**
The box ID, is assigned on receipt of goods or manually. The ID is only shown if you have selected a box in the overview of stock articles.

**Details**

**Category**
If you have defined stock categories in the master data, you can use this field as a search criterion. When you enter new stock articles you can allocate a category.

**Del. ID**
The supplier's box ID is only shown if you have selected a box in the Stock articles section.

**Main article**
You can link stock articles with several dimensions by specifying a main product. The stock check (for the stock preview in the Stock info dialog) is then only executed for the main product and you only need to enter minimum stock for this main product. If you have also defined minimum stock for the allocated stock articles, they will be ignored for the check.
⇨ Tutorial, "Stock Management" on page K-14

**Prod. batch / date**
Not currently used.

**Date**
Date at which the stock article has been changed last time.

**In production**
In connection with A+W Production you can determine whether the stock article has been allocated to production.
*   🔲 The stock article is disposable.
*   ✅ The stock article has been allocated to production (info only).

**Stock on hand**

**Stock on hand**
Displays the current stock. The stock is updated with each booking of outgoing or incoming stock. For boxes with an ID, stock `1` is always shown. If you have created the stock article new, the field is enabled and you can enter the opening stock.
