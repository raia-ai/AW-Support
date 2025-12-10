---
title: "EN-UM-AWBusiness_28"
source: "EN-UM-AWBusiness_28.pdf"
tags: ["Stock Management", "Inventory Control", "A+W Business", "Purchase Orders", "Stocktaking", "Production Orders", "Software Tutorial", "Software Reference", "ERP", "Glass Industry"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive guide to the Stock Management module in A+W Business software. It includes both a tutorial and a software reference section, covering topics such as searching for stock articles, managing purchase orders, handling production orders, and conducting inventory procedures like periodical and initial stocktaking."
long_description: "This document serves as a detailed manual for the Stock Management features within the A+W Business software, designed for users in the glass, windows, and doors industry. The guide is divided into two primary sections: a Tutorial and a Software Reference. The Tutorial section provides step-by-step instructions for common tasks. It covers how to search for stock articles within documents, check availability, and manage stock purchase orders (P.O.s), including both manual entry and automated proposals. It also details the process for creating and managing production orders to replenish stock. A significant part of the tutorial is dedicated to inventory management, explaining the procedures for periodical inventory (stocktaking) and the specialized process of conducting an initial inventory to set up the system. The Software Reference section acts as an in-depth appendix, offering detailed descriptions of every dialog box, menu option, and field within the Stock Management module. It systematically breaks down functions like Inventory Lists, Target Quantity determination, Inventory Management, Stock Movement bookings (dispatches, additions, transfers), and various queries such as the Booking Journal and Stock History. This reference is crucial for understanding the specific parameters and settings that control stock valuation (FIFO/LIFO), reservations, and statistical analysis."
---

# Tutorial

---
## Stock Articles in Documents

### Search Stock Article for an Item

This module will show you how to enter an item, at the same time checking the availability of the required product. Open dialog Stock search (which has been introduced in the previous module).

**Stock search at a P.O. entry**
You can also select a stock article via dialog Stock search when you enter a stock P.O. manually. The manual stock P.O. is described in the training module of the same name.

*⇨ "Manual Stock P.O." on page G-2550*

#### How to enter a stock article as an item

1.  Go to menu **Documents > Order > Order** and enter the order header.
2.  Go to item entry and enter the product number in the input line.
3.  Go to the menu **Start > Stock search** to open the dialog **Stock info**.

The selection in dialog Stock info is already restricted to the article you have entered for the item. You have to filter the view further now, e. g. by restricting the settings to stock sizes and stock on hand which are over zero.

*Fig. G-62 Filter for searching for stock articles*
*A Switch stock size display on or off*
*B Show only stock articles with a stock on hand of over 0*

4. Go to tab **Future stock on hand** to check whether the production dates are jeopardized.
Display of the future stock on hand in dialog Stock info has already been introduced in the module on Stock info.
*⇨ "Display of the future stock on hand" on page G-2523*

*Fig. G-63 Future stock on hand*

If the replacement time is too short, you can still enter the product then check whether another supplier is available or whether you have to change the delivery date.

5. Go to tab **Stock search** and double-click on the stock article you want to adopt for item entry.
*Fig. G-64 Select stock article*

Dialog **Stock info** closes and the item entry data is updated.

6. Enter all item data and return to the document header.
If the replacement times are too short, you can view the articles in question in dialog **Change delivery date**.

7. Click on the icon next to the shipping date to open the dialog.
*Fig. G-65 Check delivery date in the order*
*A Check delivery date*
*B Products for which the stock on hand is too low*
*C List of possible suppliers and shipping dates for the selected product*

Alternative suppliers from the supplier file are shown with the defined replacement time and the corresponding date.

Double-click on the article in the list on top (B) to open the **Stock info** with details on the articles.

8. If the scheduled delivery date is jeopardized, the following options are available:
    *   Change the supplier for the item in question or for the entire order.
    *   Change the delivery date and inform the customer.
    These steps are described in detail in the tutorial on Sales.

9. Go to the menu **Start > Save** to save the data.
The data is saved. You can now check the reservation of stock articles.

### Check the Bookings

In this module you will learn how to check the bookings for stock articles. Saving reserves the item. Withdrawal of goods is generally booked when the delivery note is printed. Printing depends on the settings in status management.
*⇨ "Status Changes due to Additions and Dispatches" on page G-2458*

#### How to check the bookings

1.  Open the **Booking journal** dialog as described in section Queries.
    *⇨ "Show Booking Journal" on page G-2513*
2.  Restrict the selection to the order for which you want to check the reservation.
    The list shows all order items with the current booking type.

*Fig. G-66 Booking - reserved*

The booking journal shows the booking type reserved only until withdrawal of goods is booked.

After the goods are withdrawn, the order items are marked as shipped.

*Fig. G-67 Booking - shipped*

The order history shows the individual status changes based on the print-outs and inventory bookings.

*Fig. G-68 Order history*

### Exercises

*   Enter an order with existing stock articles and check the entries in the booking journal:
    *   After order input.
    *   After printing the delivery note. Which changes are visible?
*   Enter an order and check the stock on hand and the reservations.
*   Issue an invoice for the order and check the stock reservations again.

### Manual Stock P.O.

**Objectives**
*   Introducing the special features of the stock P.O. in document management.

**Benefits**
*   Manual stock P.O.s are used to complete the stock on hand, e. g. for large-scale orders for which automatic reordering alone is insufficient.

> **Please note:**
>
> **Document type**: The document Stock P.O.is a separate document type. Receipt of goods can be booked to stock only for stock P.O.s.
>
> **Default settings**:
>
> *   **Master data:**
>     *   Product management
>     *   Supplier file
> *   **Company data:**
>     *   Parameters tab
>     *   Tab Stock/PP/EDI

### Manual Input of Stock P.O.

Purchase orders for stock articles can be triggered automatically, or entered manually. Automatic P.O. proposals have been introduced already in the module on the automatic stock P.O.
*⇨ "Stock P.O. (automatic)" on page G-2530*

This module will show you how to enter a stock P.O. manually. Document input is described in detail in sections Sales and Purchasing. The following instructions therefore concentrate on the main steps.

#### How to enter a stock P.O. manually

1.  Go to menu **Documents > P.O. > P.O.**
    The dialog **Document management** opens.
    *⇨ Sales, "Document - header data" on page C-1542*
2.  Enter the document header. Enter at least the supplier and the delivery date.

*Fig. G-69 Stock P.O.*
*A Document type*
*B Setting the document type*

3.  Select the entry **Stock P.O.** in field **Type (B)**.

> If you set another document type, receipt of goods is not automatically added to the stock on hand.

4.  Enter the item(s).

> **Items without stock codes**
> If you enter stock P.O.s with items which are not recorded as stock items, they will not be displayed at receipt of goods. You can however enable the corresponding option in master data **Company > Company data > tab Stock/PP/EDI**.
>
> *⇨ "Company data - Stock / PP / EDI" on page G-2455*

5.  Go to the menu **Start > Save** to save the data.
    The data is saved.
6.  Print and send the purchase order.
    This process is described in section Sales.
    *⇨ Tutorial, "Order header" on page C-1155*

### Exercises

*   Check the stock on hand for a stock article.
*   Enter a stock P.O. manually and check the corresponding values again in the Stock info dialog.

### Production Orders

**Objectives**
*   Introducing production orders.
*   Introducing the manual and automatic creation of work orders.

**Benefits**
*   Work orders are used to replenish the stock on hand.
*   When the stock on hand falls below the defined minimum, work orders can be created automatically if the diversion to an internal customer is enabled in the supplier file.

> **Please note:**
>
> *   **Procurement type**: All articles entered in a production order have to have the procurement type Production.
> *   **Booking type**: Unlike common orders, the entered items are not reserved on stock but are marked as ordered.
> *   **Addition to stock**: Stock additions based on work orders can be booked automatically or by hand:
>     *   Manual status change in module Production.
>     *   Automatic status reports from production.
> *   **Default settings**:
>     *   **Stock management:**
>         *   Minimum stock
>         *   Purchase order quantity
>     *   **Master data:**
>         *   Product management
>         *   Partner management (internal customer)
>         *   Supplier file (diversion to internal customer)
>     *   **Company data:**
>         *   Parameters tab
>         *   Tab Stock / PP / EDI > Registration point

### Stock Article as Part of the Production Order

Work orders are used to replenish the stock on hand. All articles entered in such an order are automatically changed to procurement type **Production**. Unlike customer orders, the items are not reserved on stock but are marked as **ordered**.

*Fig. G-70 Item entry – procurement type Production*

A production order differs from other orders only in its document type:

*Fig. G-71 Order entry - document type Production Order*

Work orders can be entered in different ways:

*   Enter a new document manually.
*   Copy a saved (dummy) article.
*   Automatic creation based on a shortage in the stock on hand.

### Manual Input by Copying

If you enter work orders on a regular basis, you can copy the previously entered order to make this task easier.

*   Before copying, you have to set the document type of the target document to **Production Order**.
*   If only certain items shall be adopted from the order, you can select them.
*   You can amend the data in the new document.

*Fig. G-72 Create production order by copying*
*A Copy from order to order*
*B Document type of the target order*

A detailed description of the function Copy documents can be found in section Sales.
*⇨ Sales, "New order based on copying" on page C-1366*

### Settings in Supplier File

If a minimum stock and a (standard) order quantity have been defined for the stock article in dialog **Stock management**, the system can create automatic P.O. proposals. These are listed in dialog **Stock P.O.**

This is how purchase orders of the type **Stock P.O.** are usually created. However, if an internal customer is entered in the supplier file instead of a standard supplier, work orders can be created automatically.

*Fig. G-73 Internal customer for work orders*
*A Product for which work orders shall be created*
*B Diversion to internal customer*
*C Customer selection*

In the supplier file, an internal customer is defined for which the work order is entered automatically. The option **Internal customer** can be enabled on product group or product level. The product settings have priority over the product group settings.

### P.O. Quantity after Stocktaking

The program checks whether the current stock on hand plus the already ordered quantities and minus the reserved quantities will fall below the minimum stock on hand.

If this is the case, the P.O. proposal shows the multiple of the (standard) P.O. quantity.

**Manual and automatic stock P.O.**

*Fig. G-74 Stock P.O. vs. production order*

This flow chart shows A+W Business's reactions to different presettings in the supplier file.

**Purchase order quantity**
The multiplier will be calculated so that as a result of the P.O. proposal the minimum stock is exceeded.

*Fig. G-75 Quantities for stock articles (dialog Stock management)*

**Example**
Tempered glass with article number 4008 is kept as a stock article.
Current stock on hand: 10 pcs.
Minimum stock: 30 pcs.
P.O. quantity: 5 pcs.
The P.O. quantity for tempered glass 4008 is calculated as follows:
Difference between current stock on hand and minimum stock on hand: 20 pcs. This difference includes the P.O. quantity of 5 pcs. four times.
P.O. quantity: 4 x 5 = 20 pcs.
Current stock on hand plus ordered quantity: 10 + 20 = 30 pcs.

The calculated quantity is adopted for the P.O. proposal. It can be amended in the **Stock P.O.** dialog.

*Fig. G-76 Stock P.O.- P.O. proposals*
*A Restriction to storage location*
*B P.O. proposal for production order*

In the **Stock P.O.** module you have already been shown how to edit and transfer purchase orders.
*⇨ "Transfer Stock P.O. to Purchasing" on page G-2532*

The production order is created by the transfer, in the last active order Number Manager.

*Fig. G-77 Production order in Number Manager for orders*
*A Automatically created production order*

The production order can now be opened as a document.

*Fig. G-78 Document Production Order*
*A Order header - Production order*
*B Ordered quantity*

The work order can be edited and transferred to production.

### Stock Addition based on Production Order

On tab **Stock / PP / EDI** in company data, set the limit status for registration points to define from which point on an order counts as produced. The limit status is the status defined for the selected registration point.

*Fig. G-79 Company data – Stock / PP / EDI: Registration point for status change*

There are two ways of entering additions to stock based on production orders:
*   If the status of the work order exceeds the defined status due to a report from production, the addition to stock is booked automatically.
*   If you do not use production reports, you can enter the addition to stock by means of the manual status report in the **Production** module. If you set the production order there to a status above the aforementioned limit, the stock withdrawal of the material consumed and the addition of produced stock articles to stock are booked automatically.

If no other storage location has been defined, the order quantity is allocated to the standard storage location.

The booking of work orders is described in detail in section **Production**.

**Additional information**
*   ⇨ Master data, "Company Data - Stock/Purchasing/EDI" on page B-981
*   ⇨ Sales, "Order header" on page C-1155
*   ⇨ Sales, "Change P.O. code" on page C-1432
*   ⇨ Production, “Production orders" on page E-2199

## Inventory

This section shows you how to correct the stock on hand in A+W Business by means of an inventory.

This includes the following training modules:
*   "Periodical Inventory" on page G-2565
*   "Initial Inventory" on page G-2582

### Periodical Inventory

**Objectives**
*   Getting familiar with the inventory process.
*   Learning about the inventory dialogs.
*   Carry out inventory.

**Benefits**
*   An inventory can be used to correct the stock on hand in A+W Business.
*   For big storage locations, the inventory can be organized in such a way that common business operations are impeded as little as possible.

> **Please note:**
>
> *   **No change of stock during the inventory**: On the day of the count, no orders, purchase orders or receipt of goods must be entered; no goods must be removed from or added to stock. The target inventory should be determined on the day of the count.
> *   **The inventory process**: The inventory is run in three steps:
>     *   Create inventory list
>     *   Determine target inventory
>     *   Enter counted values
>     *   Finalize inventory
> *   **Split stocktaking**: For large storage locations it may be useful to run the inventory in smaller units.
> *   **Separate stocktaking for boxes**: A special inventory list is created for boxes. The existing boxes are scanned individually.
> *   **No changes to the product master data**: As soon as the inventory list has been created, all the products that are listed on the inventory list are marked in product management (master data). The procurement type and stock code in these products are then blocked. The marking will be deleted once the inventory has been taken.
> *   **Complete the inventory list**: Additions must be made only before the target stock is determined.
> *   **Target inventory in the count list**: To print the target inventory on the count list you have to determine the target inventory before printing.
> *   **Final inventory by inventory list**: The final inventory can be run just once per inventory list.
> *   **Default settings**: None

### Stocktaking

At least once in every business year, stock has to be taken to check if the booked or target inventory shown in A+W Business Stockkeeping matches the actual stock. Inventory lists are created for this statutory annual stocktaking which help to count and enter the actual stock on hand. Stocktaking determines the existing stock by type, quantity, and value.

Basis for any stocktaking is the inventory list which can refer to selected stock articles and/or storage locations. This way, stock can be taken in several steps which presents less of an obstruction to the daily business.

A+W Business provides inventory lists and the target inventory for stocktaking. Stocktaking can be done in the conventional way or, for boxes, with the help of barcode registration.

Stocktaking is completed by the final inventory. After that, the quantities will be updated in A+W Business.

#### Actual stock on hand

The stock on hand is entered on the basis of count lists. New stock articles can be entered at the same time. During stocktaking, the stock articles on the inventory list are not locked for document entry. This is why no orders, purchase orders, or receipt of goods must be entered on the day of the count.

#### Target inventory

The target inventory must be determined no later than on the day of the count. This allows you to create the inventory list well in advance of the actual counting, input of the counted quantities, and the final inventory.

**Example**

| Activity | Date | Stock on hand | Target inventory |
| :--- | :--- | :--- | :--- |
| Inventory list created | 15 Dec | | 100 |
| Count stock on hand | 31 Dec | 80 | 100 |
| Sales | 01 Jan to 14 Jan | -30 | -30 |
| Purchasing | +10 | +10 |
| | 15 Jan | Actual stock on hand 60 | 80 |
| Final inventory | | New target inventory: | 60 |

With the final inventory, the actual stock is saved in the system as the new target inventory.

The target inventory can be printed on the count lists if required. If you do not print the target inventory you can practically neglect the "counted" quantities estimated on the basis of the target inventory.

#### sqm articles

If individual sheets of defined sizes are counted for a sqm article, these can be entered as units. At the final inventory, these will be converted into sqm and booked as such on stock (the printed closing inventory will show the counted quantity however).

#### Stocktaking of boxes

To take stock of boxes for the inventory list, first create an inventory list then determine the target inventory. Now scan or manually enter the box ID, the storage location, and - if applicable - a different number of sheets. Scanning a box will always add it to the latest inventory list. Now enter the remaining stock in Inventory Management if necessary, and book the final inventory.

**Example count list**

*Fig. G-80 Count list with fields for the counted quantities*

The counted quantities are entered in the count list and, later, in inventory management.
*⇨ "Enter Counted Values" on page G-2575*

### Create Inventory List

The inventory is based on lists in which the manually counted quantities are noted. These lists can be based on various criteria, and can be printed.

When you print these lists and realize that certain articles are missing, you can add a supplementary inventory. This way, you will not have to print all lists again.

> **No changes to the product master data**
> When the inventory list has been created, all products that appear on the inventory list are marked in product management (master data). The procurement type and stock code in these products are then blocked. This mark will be deleted when the inventory has been finalized; the data can be edited again.

This session shows you how to create inventory lists and open them again.

The following instructions exist for this training module:
*   "How to start an inventory" on page G-2569
*   "How to print the count lists" on page G-2571
*   "How to load a saved inventory list" on page G-2572
*   "How to complete an inventory list before counting" on page G-2572

#### How to start an inventory

1.  Go to menu **Stock management > Stocktaking > Inventory list**.
    Dialog **Inventory list** opens.
    *⇨ Software Reference, "Inventory list" on page G-2592*
2.  Go to the menu **Start > New** to switch to the input mode.

*Fig. G-81 Fields for the new inventory list are enabled*
*A All articles or sequence of article numbers*
*B Inventory date*
*C Restrictions*
*D Inventory evaluation*
*E Sorting the list*

The name for this inventory is a date (B). The system will suggest the current date by default. You can enter or select any other date of course.

3.  Choose the articles (A) for the inventory:
    *   **All articles:** You can take stock of all articles defined as products in the master data. In this case, the fields for the article numbers are locked. Enable this option for the initial inventory; for all other inventories, you can restrict the inventory lists to certain articles.
    *   **Article number:** You can restrict the inventory list to a sequence of article numbers. The fields are locked if you have selected the option All articles.

4.  If applicable, restrict the list further (C):
    *   **Only products with stock > 0:** You can restrict the inventory to stock articles with inventory. If you do not check the checkbox, the complete product master data will be included in the inventory list unless the selection is not restricted by other criteria.
    *   **Only products with assigned stock product:** You can restrict the inventory to the stock articles in stock management. If you do not select this checkbox, the entire product master data including stock size table will be included in the inventory list unless the selection is restricted by other criteria.
    *   **Only products with stock in the product:** You can restrict the inventory to products with procurement type Stock withdrawal.
    *   **No box with ID number and inventory = 0:** The stock on hand can include boxes which have already been shipped but not deleted. Their stock is correctly displayed as 0. You can hide these boxes because no quantities will be entered for them.
    *   **Only for defined storage location:** This setting activates the fields for selecting the storage location. If you want to take stock only for certain storage locations, you can create separate inventory lists. Please note that articles can also be booked to storage location <n.e.>. In case of comprehensive stocktaking you can also split the inventory list by storage location for the printout.

5.  Choose the inventory evaluation type (D).
    If you have enabled the options for PP calculation in the company data, you can have the stock evaluation calculated as follows:
    *   **PP price list:** The individual prices of the products from the PP rate assignment are used.
    *   **Lowest PP:** For all articles, the lowest value is used for the inventory valuation each time.
    *   **Cut PP:** For all articles, the average PP is used. For this, the **Article PP** option must be activated in the company data.

6.  Choose the sorting type (E).
    Sorting of articles on the inventory list should be based on the defined criteria. The option **Size** is useful for stock sizes for example.

7.  Go to the menu **Start > Save** to create the inventory list.
    The inventory list opens in the overview. You can now print the count lists and/or determine the target inventory.

> **No changes to the product master data**
> As soon as the inventory list has been created, all the products that are listed on the inventory list are marked in product management (master data). The procurement type and stock code in these products are then blocked. As soon as the inventory has been completed, the marking is deleted and the data can be edited again.

#### How to print the count lists

To print the target inventory on the count list you have to determine the target inventory prior to printing.
*⇨ "How to determine the target inventory for an inventory list" on page G-2574*

1.  Go to menu **Stock management > Stocktaking** and select the date of the inventory list.
2.  Go to the menu **Start > Search** to load the inventory list.
    These steps are redundant if you print the count list immediately after creating the inventory list.
3.  Go to menu **Print > Printer**.
    To check the result on screen first, select **Screen**. You can start the printout if you are satisfied with the result. The following steps are the same for both settings.

*Fig. G-82 Inventory - Print count list*
*A Page break*
*B Articles that shall be printed*
*C Sorting*

*⇨ Software Reference, "List printing" on page G-2595*
Print the count lists so that they match the tasks of your stocktaking staff.

4.  Define the point at which a new page (A) shall be started.
    If you did not define different storage locations, this setting can be omitted. If you have split the count areas by storage location, start a new page after the corresponding storage locations.
    You must select at least one warehouse (level 1) for the printout.

5.  Define the stock articles (B) to be printed on the list.
If different stock articles are stored in the individual storage locations, you can distinguish finished products and raw material. Finished products are stock articles which are not stored in the raw material stock.
The characteristics **Finished products** and **Raw material** have been assigned in stock definition.
*⇨ "Define Storage Location" on page G-2447*

6.  Sort (C) the articles on the count list depending on the selected criteria. The option **Article** makes sense for instance if the stock is organized by products.

7.  Click **[OK]** to start printing.
    The list is printed and can be used for counting.

#### How to load a saved inventory list

1.  Go to menu **Stock management > Inventory**.
2.  Go to field **Inventory date** and select the date on which the inventory list has been saved.
3.  Go to the menu **Start > Search** to load the inventory list.
    The inventory list opens.

#### How to complete an inventory list before counting

If you have already determined the target inventory for an inventory list, you cannot complete this list. In this case, close the inventory and enter the missing articles in a new inventory list.

1.  Go to menu **Stock management > Inventory**.
2.  Go to the menu **Start > New** to switch to the input mode.
    The fields will be enabled.
3.  Select the inventory list to which articles shall be added.
4.  Select the stock articles and/or storage locations.
5.  Go to the menu **Start > Save** to save the data.
    A query is displayed that allows you to abort this process or complete it.
6.  Select
    *   **[Yes]**: The existing list is displayed, the new articles are added at the end.
    *   **[No]** or **[Abort]**: The query is closed. You can change the date or other criteria and create a new inventory list.

### Determine Target Inventory

The target inventory has to be determined for every inventory list. It defines the quantities that should be on stock according to the system. To print the target inventory on the count lists you have to determine the target quantity prior to printing a list.

> **No inventory bookings on the count day**
> After the target quantity has been determined, the stock quantities must be counted. On the day of the count, no stock articles may be withdrawn and no stock movements may be booked until counting has been finalized. This applies to all manual or automatic stock withdrawals/additions, and all goods received into stock based on purchase orders. A+W Business is not automatically blocked for bookings.

This module shows you how to determine the target inventory for a saved inventory list.

#### How to determine the target inventory for an inventory list

1.  Go to menu **Stock management > Inventory > Target inventory**
    Dialog **Target inventory** opens.
    *⇨ Software Reference, "Target quantity" on page G-2597*
2.  Load the inventory list for which you want to determine the target inventory.

*Fig. G-83 Determine target inventory*

3.  Go to menu **Start > Execute** to determine the target inventory and confirm the query by **[Yes]**.
    The target inventory is entered in column **Target**. You can determine the target inventory just once per inventory list. The result will not be updated even if you execute this function several times.
    If the target inventory shall be printed on the count list, you can start the printout now.
    You can now start counting and subsequently enter the counted quantities.

### Enter Counted Values

Once you have entered the counted quantities in the printed count lists, you can enter the values in dialog **Inventory management**.

> **No inventory bookings on the count day**
> After the target quantity has been determined, the stock quantities must be counted. On the day of the count, no stock articles may be withdrawn and no stock movements may be booked until counting has been finalized. This applies to all manual or automatic stock withdrawals/additions, and all goods received into stock based on purchase orders. A+W Business is not automatically blocked for bookings.

This module will show you how to enter the counted quantities in A+W Business plus a new stock article if necessary.

The following instructions exist for this training module:
*   "How to enter the counted quantities" on page G-2575
*   "How to enter a new stock article during stocktaking" on page G-2576

#### How to enter the counted quantities

1.  Go to menu **Stock management > Inventory > Inv. Management**.
    Dialog **Inv. Management** opens.
    *⇨ Software Reference, "Management" on page G-2601*
2.  Load the inventory list.
    The table shows the records in the same sequence as on the printed list.
    Menu **Sorting** can be used to choose another sequence if this will facilitate the entry of the counted values.

*Fig. G-84 Inventory - Enter counted quantities*
*A Enter counted quantity*
*B List of records*

3.  Enter the quantity (A) for the first item in field **Qty** and confirm by <Enter>.
    The marking automatically switches to the next line where you can enter the next quantity.
4.  To enter the quantities in a different sequence, just select the line in question.

> **Quantity and storage location for several articles**
> You can select several records and set the quantity for all to zero or change the storage location by using the **Functions** menu.

5.  If necessary, you can change the storage location, the inventory price, and the category to be used for inventory evaluation.
    Changed inventory prices will not be saved in the purchase price table after the finalization of the inventory, and will not be considered for calculating the average purchase price.

6.  Go to the menu **Start > Save** to save the data.
    The data is saved. If you have not entered the data completely yet, you can resume the input later. Start from step 1 in this case.
    You can finish stocktaking when you have entered all quantities.

#### How to enter a new stock article during stocktaking

1.  Go to menu **Stock management > Inventory > Inv. Management** and select the current inventory.
2.  Select the record for which you want to enter a new stock article.
3.  Go to the menu **Start > New** to switch to the input mode.
    All data of the original stock article will be copied so that you only have to edit the data for the new stock article.
4.  Enter the width, height, storage location etc.
5.  Go to the menu **Start > Save** to save the data.
    The list is completed by the new stock article.

### Finalize Inventory

Stocktaking is finalized by booking the results of counting and updating the stock on hand.

The final inventory can be run just once per inventory list. Should you detect errors in the counted or entered quantities after closing, you have to correct the quantities in dialog **Inventory management**, or create and finalize a new inventory list for the corresponding article.

This module shows you how to finalize the inventory for an inventory list.

For instructions on this subject, please see:
*   "How to finalize the inventory" on page G-2578
*   "How to delete an inventory list after the final inventory" on page G-2579

#### How to finalize the inventory

1.  Go to menu **Stock management > Inventory > Final Inventory**.
    Dialog **Final Inventory** opens.
    *⇨ Software Reference, "Finalization" on page G-2606*
2.  Load the inventory you want to finalize.

*Fig. G-85 Inventory - Final Inventory*

The inventory list is displayed with the quantities entered.

3.  Check in the **Options** menu whether the stock on hand should be set to zero with or without query when no quantities have been entered.
4.  Select production preparation for which stocktaking has been restricted.
5.  Go to menu **Start > Execute** and confirm the query by **[Yes]** in order to finalize the inventory.
    The data will be saved and the stock on hand values and the prices for the inventory evaluation will be updated. Booked records are deleted from the list. The locks in the product master data will be removed.
    Records that could not be booked are kept on the list. You can complete the missing entries in dialog **Inv. Management**.
    If all records could be booked, the complete inventory list will be deleted from the final inventory.

> **Inventory errors**
> If errors have occurred during stocktaking and individual records are not deleted from the inventory list, you can use the log to search for the cause. Open the log via **System > Log**.

#### How to delete an inventory list after the final inventory

> **Do not delete individual records**
> After the final inventory, individual records cannot be deleted from the list.

1.  Go to menu **Stock management > Stocktaking > Inventory list**.
2.  Load the inventory list you have finalized.
3.  Go to menu **Start > Delete** and confirm the query by **[Yes]**.
    The inventory list is deleted. If further inventory lists were created, the next list will be loaded now.

### Add Supplementary Inventory

You can combine two separate inventories to print the final inventory. Both inventories have to be final (i.e. booked) for this purpose.

Chapter **Create inventory list** describes how to add further stock articles to an inventory list.
*⇨ "How to complete an inventory list before counting" on page G-2572*

This module shows you how to add a supplementary inventory to a main inventory.

#### How to add a supplementary inventory

1.  Go to menu **Stock management > Inventory > Final Inventory**.
    Dialog **Final Inventory** opens.
2.  Select the main inventory in field **Inventory date**.
3.  Select **Functions > Add supplementary inventory** from the menu.

*Fig. G-86 Select supplementary inventory*

4.  Select the date of the supplementary inventory and press **[OK]** to adopt it.
    The main inventory list will be enhanced by the items of the supplementary inventory. The supplementary inventory list is then deleted from dialog **Inventory list**.

### Exercises

*   Create an inventory list for a sequence of 5 articles.
*   Add two articles to the inventory list.
*   Determine the target inventory for the entire inventory list.
*   Enter the counted quantities.
*   Finalize the inventory.
*   Create another inventory list consisting of three articles. Add it to the first inventory as a supplementary inventory.

**Additional information**
*   ⇨ Software Reference, "Inventory list" on page G-2592
*   ⇨ Software Reference, "List printing" on page G-2595
*   ⇨ Software Reference, "Target quantity" on page G-2597
*   ⇨ Software Reference, "Management" on page G-2601
*   ⇨ Software Reference, "Finalization" on page G-2606

### Initial Inventory

**Objectives**
*   Getting familiar with the function of the initial inventory

**Benefits**
*   The initial inventory is used to put your stock into operation, including the stock articles and the current stock on hand.

> **Please note:**
>
> *   **Support for your initial inventory**: Before starting the initial inventory, please contact A+W Software GmbH. Your contacts there will support you with the completion.
> *   **No order processing**: As no orders must be processed during the initial inventory, the initial inventory should take place out of the daily business hours, e. g. on a weekend.
> *   **Prerequisite**: You have to be familiar with the process of periodical stocktaking before you start with the initial inventory. Please study the training module on section Periodical inventory carefully.
> *   **Default settings**: None

#### Initial Inventory Process

*   **Stock initialization**: the stock is deleted (module **Utilities**).
    From now on, new orders must not be entered, nor must old orders be processed.
*   **Create inventory list**.
*   **Determine target inventory**.
*   **Stock management**: Set all stock on hand to 0 and define the standard storage location for all stock articles.
*   **Finalize inventory**.
*   **Initialize stock** (module **Utilities**).
    Until now you have entered all actual stock articles and have set their quantities to 0. All previous (incorrect) values, e. g. test products and stock quantities to test functions, have been deleted.
    The values for purchase orders and reservations are checked and corrected if necessary.
*   **Execute complete inventory**:
    *   Create new inventory list.
    *   Print count list.
    *   Determine target inventory.
    *   Count quantities of stock articles.
    *   Do not book any stock withdrawals or additions while counting.
    *   Enter counted values.
    *   Finalize inventory.
*   **Initialize stock** (module **Utilities**).
    The values for purchase orders and reservations are checked again and applied to the stock articles.

> **No changes to the product master data**
> As soon as the inventory list has been created, all the products that are listed on the inventory list are marked in product management (master data). The procurement type and stock code in these products are then blocked. As soon as the inventory has been completed, the marking is deleted and the data can be edited again.

### Execute Initial Inventory

Initial stocktaking takes place before you start working with A+W Business inventory management for the first time. It is used to start up the stock with its articles and initial stock on hand.

> **You should be familiar with the regular stocktaking procedure**
> Before starting on the following actions you should read the instructions on the regular stocktaking process. The description of the initial inventory is based on the assumption that you are familiar with this process.

#### How to execute the initial inventory

> **Please contact our service team before you start the initial inventory**
> Before starting the initial inventory, please contact A+W Software GmbH. Your contacts there will support you with the completion.

1.  Start module **Utilities**.
2.  Go to menu **System > Initialize Stock**.

*Fig. G-87 Utilities - Initialize stock*

3.  Go to menu **Functions > Delete stock**.
    From now on, you must not enter new orders or edit existing orders until the stock has been initialized. If someone is still using the Document management dialog, storage location n.e. will be created again in inventory management, and is allocated to all stock articles.

4.  Now take the following steps to execute the initial inventory:
    *   **Create Inventory List.**
        Select the following criteria in dialog **Inventory list**:
        *   **For stock articles only**: Setting **All articles** would e. g. put even P.O. items on the list.
        *   **All storage locations.**
    *   **Determine Target Inventory.**
    *   **Enter Counted Values.**
        Set the quantities of all counted articles to 0 in dialog **Stock management - Management**.
        This process is described in the operation instructions for entering the counted quantities in the notes on step 4 and step 5.
    *   **Finalize Inventory.**

5.  Return to dialog **Initialize Stock**.
6.  To start the activity, go to the menu **Start > Execute**.
7.  Use a new inventory list for complete inventory taking:
    *   "How to start an inventory" on page G-2569
    *   "How to print the count lists" on page G-2571
    *   "How to determine the target inventory for an inventory list" on page G-2574
    Please make sure that no stock additions or withdrawals are booked during the counting. This also applies to entering received goods.

8.  Enter the counted quantities and the correct storage locations and finalize the inventory:
    *   "How to enter the counted quantities" on page G-2575
    *   "How to finalize the inventory" on page G-2578

9.  Open dialog **Stock initialization** as described in step 1 and 2.
10. To start the activity, go to the menu **Start > Execute**.
    From now on, the stock on hand and the storage locations reflect correct values.

### Exercises

Answer the following questions by explaining the corresponding settings.

*   When does the stock take reports from production, e. g. from A+W Production, into consideration?
*   Where do you define whether reserved stock products are withdrawn after delivery note printing or after invoice printing?
*   What do you have to do to book stock products which belong to an item in the shape of BOM components, automatically on stock?
*   What is the difference between the definition of stock sizes in dialog **Master data > Products > Article > Stock sizes** and in dialog **Stockkeeping > Inventory management**?
*   What is displayed on the first two tabs in dialog **Stock management > Stock management**? Describe the differences!
*   What is the difference between the booking journal and the stock history?
*   What is the purpose of the **Stock management > Stock P.O.** dialog?
*   What is the difference between a manual and an automatic stock P.O.?

# Software Reference

## Overview

This section provides information on the following subjects:

*   ⇨ Overview
*   ⇨ Inventory
*   ⇨ Inventory Management
*   ⇨ Final Inventory
*   ⇨ Stock Management
*   ⇨ Stock Movement
*   ⇨ Queries
*   ⇨ Search
*   ⇨ Stock P.O.
*   ⇨ Inventory Assessment

| Topic | Page |
| :--- | :--- |
| Overview | G-2590 |
| Inventory | G-2591 |
| Inventory list | G-2592 |
| List printing | G-2595 |
| Target quantity | G-2597 |
| Block entry | G-2599 |
| Delete inventory blocks | G-2599 |
| Inventory Management | G-2600 |
| Menus in inventory management | G-2600 |
| Options menu | G-2600 |
| Functions menu | G-2601 |
| Management | G-2601 |
| Go to article | G-2604 |
| Value correction | G-2604 |
| Final Inventory | G-2605 |
| Menus in final inventory | G-2605 |
| Options menu | G-2605 |
| Functions menu | G-2605 |
| Finalization | G-2606 |
| Select inventory list | G-2608 |
| Stock Management | G-2609 |
| Menus in stock management | G-2609 |
| Functions menu | G-2609 |
| Options menu | G-2610 |
| Print menu | G-2610 |
| Stock management | G-2610 |
| Stock management - stock articles | G-2611 |
| Stock management - prices | G-2615 |
| Stock management - supplement | G-2618 |
| Stock Movement | G-2620 |
| Options menu | G-2620 |
| Stock movement | G-2620 |
| Stock movement - dispatch, addition | G-2621 |
| Stock movement - transfer | G-2623 |
| Stock movement - number of Sheets | G-2623 |
| Stock movement - open boxes | G-2624 |
| Remark (stock movement) | G-2624 |
| Queries | G-2625 |
| Booking journal | G-2625 |
| Stock history | G-2627 |
| Stock history - selection | G-2628 |
| Stock history - table | G-2631 |
| Stock statistics | G-2631 |
| Stock statistics - products | G-2633 |
| Stock statistics - statistics | G-2634 |
| Stock statistics - FIFO/LIFO | G-2636 |
| Reserved stock products | G-2636 |
| Search | G-2638 |
| Stock search - stock search | G-2638 |
| Stock search - future stock on hand | G-2638 |
| Stock P.O. | G-2640 |
| Order pool menus | G-2640 |
| Functions menu | G-2640 |
| Options menu | G-2641 |
| Order pool | G-2643 |
| Inventory Assessment | G-2646 |
| Inventory assessment | G-2647 |
| Options menu | G-2647 |
| Stock assessment - selection | G-2648 |
| Stock assessment - assessment | G-2649 |

Use the module **Stock Management** to maintain and analyze all data concerning stock. Furthermore, use this module to carry out the inventory and book stock movements.

The Software Reference provides information on the following subjects:
*   "Inventory" on page G-2591
*   "Stock Management" on page G-2609
*   "Stock Movement" on page G-2620
*   "Queries" on page G-2625
*   "Search" on page G-2638
*   "Stock P.O." on page G-2640
*   "Inventory Assessment" on page G-2646

## Inventory

**Stock management > Inventory**

Carry out inventory taking in individual steps by using the dialogs in the Inventory menu: Create an inventory list, determine the target inventory, enter counted quantities and finalize the inventory.

You will find the following program items in the Inventory menu:
*   Inventory list
*   Target quantity
*   Inventory Management
*   Final Inventory

**Additional information**
*   ⇨Tutorial, "Periodical Inventory" on page G-2565
*   ⇨Tutorial, "Initial Inventory" on page G-2582

### Inventory list

**Stock management > Inventory > Inventory list**

To the dialog description:
*   ⇨List printing

**Functions menu**
The old inventory list is deleted with the function **Clear stock**. At the same time, all products from the stock master data that do not have a stock code or that do not make any sense are deleted, e. g a product without reference to the storage location.

> **This process may take quite a while**
> Depending on the size of the database and the computer performance, clearing the stock may run for a longer period of time. It may even run for several hours. During this time, you cannot work with A+W Business.

*Fig. G-88 Inventory list*

The inventory list forms the basis for the actual inventory process. Select the criteria for which the list shall be created. Since you cannot carry out any changes to the stock during the counting process, it makes sense for large stock to take inventory in smaller units, e. g. by storage places.
*   ⇨Tutorial, "Create Inventory List" on page G-2568*

> **No changes to the product master data**
> As soon as the inventory list has been created, all the products that are listed on the inventory list are marked in product management (master data). The procurement type and stock code in these products are then blocked. As soon as the inventory has been completed, the marking is deleted and the data can be edited again.

Once the inventory list has been created, the target stock for the articles that are listed on the inventory list can be determined.
*   ⇨Tutorial, "Inventory" on page G-2564*

> **Delete inventory list**
> Once you have completely finalized inventory taking, you should delete the relevant inventory list. However, you are also able to delete any inventory list at any time. The indicator **Article is on the inventory list** in the order and the block in the product master data are then removed.

**Parameters**
The fields in this area are only released when you create a new inventory list. You can have an inventory list displayed in the selection mode by using the date.

*   **Inventory date**: The inventory list is created at a certain date. All other inventory processes will always refer to the inventory date. The current date is shown automatically. It can be overwritten with the requested date, e. g. if you are preparing for inventory taking that will take place at a later date.
*   **All articles**: You can execute inventory taking for all articles that have been entered as products in the master data.
*   **Article number from ... to**: You can create the inventory list for a certain range of article numbers by entering the corresponding numbers. These fields are locked if the checkbox **All articles** is checked.

**Inventory valuation**
Choose an option to define how the inventory value for the inventory shall be determined. The corresponding value is shown in the column **PP/PU** on the inventory list. The value can be printed on the count list.
*   **PP price list:** The individual prices of the products from the PP rate assignment are used for stock evaluation.
*   **Lowest PP:** For all articles, the lowest value is used for the inventory valuation each time.
*   **Average PP:** For all articles, the average purchase price is used for the inventory valuation each time. For this purpose, the option **Average PP** must be activated in the company data.
    *   ⇨ Master data, "Average PP: The average purchase price will be recalculated in the following cases:" on page B-981

*   **Only products with stock on hand > 0**: You can limit the inventory to the stock articles with inventory. The complete product master data including stock dimension table is included in the inventory list, insofar as this selection is not limited by other criteria. Only the stock articles are taken over into the inventory list for which there is inventory. The **Only products with assigned stock product** and **No box with ID and inventory = 0** check boxes are checked and locked.
*   **Only products with assigned stock product**: You can limit the inventory to the stock articles. The complete product master data including stock dimension table is included in the inventory list, insofar as this selection is not limited by other criteria. Only the stock articles are taken over into the inventory list that are created in the stock management.
*   **Only products with stock flag in products**: You can limit the inventory to the products with a stock flag. The complete product master data including stock dimension table is included in the inventory list, insofar as this selection is not limited by other criteria. Only items with the procurement type **Stock removal** will be included in the inventory list. The check box is checked and locked if the **Only products with stock on hand > 0** check box is checked.
*   **No box with ID and inventory = 0**: The stock on hand may include boxes that have already been delivered, but have not been deleted. Their stock is correctly displayed as 0. All boxes are listed on the inventory list. Boxes with an ID and an inventory = 0 are not included in the inventory list. The check box is checked and locked if the **Only products with stock on hand > 0** check box is checked.
*   **Only for defined storage place**: You can limit the inventory to a storage place. Inventory is kept for all storage places. It is not limited to one storage place. The inventory is kept for a storage place. For determination of the storage place, the combo boxes **Warehouse**, **Corridor**, **Shelf** and **Tray** (levels 1 to 4) are enabled. This setting only makes sense if the inventories of your storage locations are checked in different periods.
    > **Storage location <n/a>**
    > Even if you have defined your own storage locations, storage locations <n/a> will remain and can be booked.
*   **No products from product stock dimensions**: You can create the inventory without taking over the product stock dimensions. The inventory will be created for all products. The inventory will be created without the automatic takeover of the product stock dimensions.
*   **Warehouse, Shelf, Corridor, Tray**: You can limit the Inventory list to a storage place. These fields are only enabled if the **Only for defined storage place** check box is checked.

**Sort by**
With the selection of this option, you specify the sorting for the inventory list. By default, the **Articles** option is activated.

**Overview**
The overview lists all articles that should be counted in the inventory and should be assessed.
*   **Record no.:** Sequential number in the inventory list.
*   **Art. no.:** Product number from the master data.
*   **Name:** Product name from the master data.
*   **Color:** The color is only specified if the product has been entered with variants/colors.
*   **Width, Height:** The dimensions are only displayed if the product is created as stock dimension or box with fixed dimensions. For all non-dimension-dependent products, the value 0 is displayed.
*   **PP/PU:** Purchase price (PP) per price unit. Depending on the settings, this is the lowest or the average PP.
*   **PU:** Price unit of the purchase price.
*   **PP/Sheet:** The purchase price per sheet is only displayed for stock dimensions. It is calculated from the PP/PU and the actual size of the sheet. If a piece price is stored, the values are identical in the PP/PU and PP/Sheet columns.
*   **nominal:** The nominal inventory specifies what quantity is stored in A+W Business according to the bookings made. It is only stored if the nominal inventory was determined. *⇨ "Target quantity" on page G-2597*
*   **QU:** Quantity unit with which the product is kept in stock.

### List printing

**Stock management > Inventory > Inventory list > Print menu**

*Fig. G-89 Print - Inventory list*

Use this dialog to set printing of the count lists. You can design the sheets according to manual stock entry and the inventory tasks of your employees.
*   ⇨Tutorial, "How to print the count lists" on page G-2571*

> **Target inventory in the count list**
> The target inventory can only be printed on the count list if it has been determined prior to printing.
> *⇨ "Target quantity" on page G-2597*

**Page break after changing from**
**Warehouse, Warehouse corridor, Warehouse shelf, Warehouse tray**: If you sort the count list by the storage location, you can also define after which storage levels a page break should be executed. This setting makes sense if you print the count list sorted by storage locations. You can then print an individual sheet for every level.
*   ⇨ "Sorted by" on page G-2596*

**Parameters**
Select an option to define which products shall be listed on the count list.
The options **Finished products** and **Raw material** refer to the **Raw material** indicator according to the stock definition. If the Raw material indicator has not been set, the system automatically takes the corresponding storage location as the storage location for the finished products.
*   ⇨ Master data, "Stock Definition" on page B-789*
*   **All articles:** All articles from the inventory list are printed on the count list.
*   **Finished products:** Only those articles from the inventory list, of which the storage location is not intended for raw materials, are printed.
*   **Raw material:** Only those products from the inventory list that are located at a storage location for raw materials are printed.
*   **Print prices:** The count list can be printed with or without prices.
*   **Print target inventory:** The target inventory can only be printed on count lists if the target inventory has been determined.
*   **0x0 records print for glass articles:** If on the printout glass articles with the dimensions 0x0 should be output, this option must be activated. Without the option, only glass articles with correct dimensions are printed on the inventory list.

**Sorted by**
Select an option to define how the articles shall be sorted on the count list:
*   **Article:** The list is sorted by product numbers.
*   **Dimensions:** If the count list includes stock sizes, those entries will be printed sorted by width/height.
*   **Storage location:** If the articles of the count list are stored at different storage locations sorting by storage locations makes sense. In addition, you can define the page feeds. *⇨ "Page break after changing from" on page G-2595*

**Print storage locations**
All the storage locations that have been defined in the master data or that have been selected for the inventory list are listed in the overview. You can determine whether the storage places should be printed on the count list. If you want to print the storage places you must select at least one.

> **Storage location <n/a>**
> Even if you have defined your own storage locations, storage locations <n/a> will remain and can be booked.

### Target quantity

**Stock management > Inventory > Target quantity**

*Fig. G-90 Target quantity*

The target quantity corresponds to the quantity that has been determined by the system resulting from automatic or manual bookings. It is determined each time for a certain inventory list or for all articles that are listed on the selected inventory list.
*   ⇨ Tutorial, "Determine Target Inventory" on page G-2572*

> **No inventory change on the day of the count**
> After the target quantity has been determined, the stock quantities must be counted. On the day of the count, no stock articles may be withdrawn and no stock movements may be booked until counting has been finalized. A+W Business is not automatically blocked for bookings.

**Parameters**
**Inventory date**: All inventory lists that are stored in the system are listed in the combo box. You cannot determine from the date whether the inventory has been concluded.

**List**
*   **Record no.:** Sequential number on the inventory list.
*   **Art. no.:** Product number according to the master data.
*   **Name:** Product name from the master data.
*   **ID:** Box ID (manual booking or from receipt of goods).
*   **Contents:** Value 1 is shown for stock articles and stock sizes and the number of sheets for boxes.
*   **Width, Height:** Dimensions are only shown if the product has been defined as a stock size or box.
*   **Color:** The color is only specified if the product has been entered as a variant.
*   **Storage location:** Storage location in the order of level 1 through 4.
*   **PP/PU:** Purchase price (PP) per price unit. Depending on the settings, this is the lowest or the average PP.
*   **PU:** Price unit of the purchase price.
*   **Cat.:** This function is used only for certain customers.
*   **Nominal:** Quantity that should be available according to the system. The values are only shown if the target quantity has been determined.
*   **QU:** Quantity unit with which the product is kept in stock.

## Inventory Management

**Stock management > Inventory > Management**

Enter the counted quantities in the Inventory Management dialog. You can book stock again directly after counting.

This chapter provides information on the following subjects:
*   "Menus in inventory management" on page G-2600
*   "Management" on page G-2601
*   "Go to article" on page G-2604

### Menus in inventory management

**Stock management > Inventory > Management**

The inventory management menus allow you to define the default settings for the dialog and open other dialogs without having to close inventory management.

This chapter provides information on the following subjects:
*   "Options menu" on page G-2600
*   "Functions menu" on page G-2601

#### Options menu

**Stock management > Inventory > Management**

The menu is divided into the following groups:
*   "Stock size group" on page G-2600
*   "Sort group" on page G-2600

**Stock size group**
*   **Calculate stock size surface automatically:** The surface of the counted stock plates is automatically shown in square meters.

**Sort group**
*   **Article / Storage location / Size:** The list is sorted by articles. This sorting makes sense if the same articles are stored at several different storage locations.
*   **Dimension / article / storage location:** The list is sorted by sizes of the stock size. This type of sorting makes sense if you have entered the stock sizes in individual count lists.
*   **Storage location / Article / Dimension:** The list is sorted by storage places. This type of sorting makes sense if you have also sorted the count lists by storage locations.
*   **Record no.:** Record number from the inventory list.

#### Functions menu

**Stock management > Inventory > Management**

The following entries are displayed:
*   **Go to article:** Opens the Go to Article dialog. *⇨ "Go to article" on page G-2604*
*   **Change quantity for marked articles to zero:** The quantity is changed to zero. This function is helpful if you are marking several documents. You do not need to change every single one to zero.
*   **Define storage location for tagged article:** The storage location is changed for all tagged documents.

### Management

**Stock management > Inventory > Management**

*Fig. G-91 Inventory management*

Use this dialog to enter counted quantities. The list shows the entries that you have selected with the inventory list. You can book stock again directly after counting.
*   ⇨ Tutorial, "Enter Counted Values" on page G-2575*

> **Take inventory of boxes**
> Once the target quantity for the inventory list has been created, boxes can also be entered by scanner and included on the inventory list. For this purpose, the box ID, storage location and any deviating sheet quantities must be scanned.

**Input screen**
*   **Inventory date**: Enter the date of the inventory list.
*   **Article number**: Number of the article the quantity of which shall be entered.
*   **Width, Height**: The sizes are entered only for stock plates and boxes. For all other articles, both fields will show a zero (0).
*   **Category**: This function is used only for certain customers in order to use categories for value correction of stock.
*   **Inv. price**: You can manually enter an inventory price for the inventory valuation. After completion of the inventory taking process, this price is not saved in the PP price table and is not included in the calculation of the average PP. If no inventory price is entered, depending on the inventory list settings, the lowest or the average PP applies.
*   **Content**: Shows the quantity of boxes. If boxes have been counted as a unit, a box make not be broken down, i. e. plates may not have been withdrawn.
*   **Name**: Article name from the product master data.
*   **Color**: For articles with color allocation (variant) you can enter the quantity per color.
*   **Ident**: Box ID (manual booking or from receipt of goods).
*   **Storage location**: Storage place of the counted article.
    > **Storage location <n.e.>**
    > Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.
*   **Quantity**: Enter the counted quantities from the count list in this field. You can only enter the quantities after you have determined the target quantity.

**Table**
The overview lists all the articles that are to be counted and valuated.
*   **Record no.:** Sequential number on the inventory list.
*   **Art. no.:** Product number according to the master data.
*   **Name:** Product name from the master data.
*   **Content:** Value 1 is shown for stock articles and stock sizes and the number of sheets for boxes.
*   **ID:** Box ID (manual booking or from receipt of goods).
*   **Width, Height:** Dimensions are only shown if the product has been defined as a stock size or box.
*   **Storage location:** Storage location in the order of level 1 through 4.
*   **PP/PU:** Purchase price (PP) per price unit. Depending on the settings, this is the lowest or the average PP.
*   **PU:** Price unit of the purchase price.
*   **Category.:** This function is used only for certain customers.
*   **Quantity:** Value that has been entered as the counted quantity.
*   **QU:** Quantity unit with which the product is kept in stock.

### Go to article

**Stock management > Inventory > Management > Functions menu > Go to article...**

*Fig. G-92 Go to article*

In this dialog you can set a marking for the first document relating to the specified article.

*   **Articles**: Number of the stock article on the list which you would like to go to.

### Value correction

**Stock management > Inventory > Management > Category field > Folder icon**

*Fig. G-93 Value correction*

Use this dialog to define the categories and percentages for correcting the stock value.
This dialog is enabled for individual customers only.

## Final Inventory

**Stock management > Inventory > Finalization**

You conclude inventory taking with the final inventory. You can book stock again directly after counting.

This chapter provides information on the following subjects:
*   "Menus in final inventory" on page G-2605
*   "Finalization" on page G-2606

### Menus in final inventory

**Stock management > Inventory > Finalization**

The menus can be used to define the standard settings or open other dialogs without closing this dialog.

This chapter provides information on the following subjects:
*   "Options menu" on page G-2605
*   "Functions menu" on page G-2605

#### Options menu

**Stock management > Inventory > Finalization**

The following entries are displayed:
*   **Do not print articles with stock on hand = 0:** Only articles with stock on hand that is more than 0 will be printed. This setting is helpful if you have many articles without stock figures. This makes the printed list clearer.
*   **Check whether the stock for uncounted articles shall be set to 0:** Use this function to define that the quantity of articles for which no stock has been entered is only then set to 0 when you have confirmed this for each article.

#### Functions menu

**Stock management > Inventory > Finalization**

The following entries are displayed:
*   **Add supplementary inventory:** Opens the dialog **Select inventory list** in order to print and analyze two different inventories in one joint list.
    *   ⇨ "Select inventory list" on page G-2608

### Finalization

**Stock management > Inventory > Finalization**

*Fig. G-94 Final inventory*

Use this dialog to finalize the inventory for each inventory list. With it, the entered values are adopted in the stock on hand (stock lists). Any goods issued or received in the meantime are taken into account. New stock articles from the inventory are automatically adopted in inventory management.
*   ⇨Tutorial, "Finalize Inventory" on page G-2578*

> **Per inventory list only one final inventory**
> The final inventory can only be executed once per inventory list. Any entry errors can only be corrected in inventory management after the final inventory. Alternatively, a new inventory list can be created with the incorrectly entered articles.

**Booking**
*   **Inventory date**: Date of the inventory that is to be finalized.
*   **Book by supply type as per production preparation**: If you work with order areas, stock may be allocated for a certain production preparation, e. g. for the production of LAMI. The field for selecting the production preparation is enabled only if you have checked the checkbox. The counted stock is allocated to the standard storage place. The stocks shall be allocated to a production preparation.
    *   ⇨ Master data, "Order Areas" on page B-1040
*   **Record no. from... to**: Displays the first and last record number of the loaded inventory list.

**Overview**
*   **Record no.:** Sequential number on the inventory list.
*   **Art. no.:** Product number according to the master data.
*   **Name:** Product name from the master data.
*   **Content:** Value 1 is shown for stock articles and stock sizes and the number of sheets for boxes.
*   **ID:** Box ID (manual booking or from receipt of goods).
*   **Width, Height:** Dimensions are only shown if the product has been defined as a stock size or box.
*   **Storage location:** Storage location in the order of level 1 through 4.
*   **Quantity:** Value that has been entered as the counted quantity.
*   **QU:** Quantity unit with which the product is kept in stock.
*   **Status:** The status is only shown if the record could not be booked. Use the logbook to check for the possible causes.

### Select inventory list

**Stock management > Inventory > Finalization > Functions menu > Add supplementary inventory**

*Fig. G-95 Add supplementary inventory*

A supplementary inventory can only be added if both inventories have been finalized. Both inventories can then be printed on a joint list and be analyzed.
*   ⇨Tutorial, "How to add a supplementary inventory" on page G-2580*

## Stock Management

**Stock management > Stock management**

Use the dialog **Stock management** to display all the stock articles that are managed.

This chapter provides information on the following subjects:
*   "Menus in stock management" on page G-2609
*   "Stock management" on page G-2610

### Menus in stock management

**Stock management > Stock management**

The menus can be used to define the standard settings of the dialog or open other dialogs without closing this dialog.

This chapter provides information on the following subjects:
*   "Functions menu" on page G-2609
*   "Options menu" on page G-2610
*   "Print menu" on page G-2610

#### Functions menu

**Stock management > Stock management > Functions menu**

This menu allows you to open other dialogs without closing stock management.

The following entries are displayed:
*   **Stock History:** Opens the dialog **Stock History** with the log of processes that have been booked in stock management.
    *   ⇨ "Stock history" on page G-2627
*   **Booking Journal:** Opens the dialog **Booking Journal** with the log of stock bookings from orders and purchase orders.
    *   ⇨ "Booking journal" on page G-2625

#### Options menu

**Stock management > Stock management > Options menu**

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

The following entries are displayed:
*   **Do not print articles with stock on hand = 0:** Only articles with stock on hand that is more than 0 will be printed. This setting is helpful if you have many boxes with an ID, but without stock. Usually, these have been delivered as boxes and were deleted from the stock. This setting applies only to printing; the dialog shows all the articles.
*   **Automatic ID allocation:** The box ID can be allocated automatically even it has been booked as stock manually.

#### Print menu

**Stock management > Stock management > Print menu**

Use this menu to start the printout of labels.

The following entries are displayed:
*   **Box labels:** Only labels for boxes will be printed. For this, the print point 973 must be created and the report boxlabel.qrp assigned in the form management.
*   **Standard:** Labels for stock articles will be printed.

### Stock management

**Stock management > Stock management**

In the **Stock Management** dialog you enter all the stock articles that are kept in the warehouse with stock on hand.

Stock sizes are maintained in A+W Business even in product management. They are used to allocate price codes, product groups, etc.

Dialog **Stock Management** offers the following tabs:
*   Stock management – stock articles
*   Stock management – prices
*   Stock management - supplement

> **Stock management at the level of bills of material**
> In the warehouse, you can also manage products that are included as bill of material components in other products. For this purpose, the checkbox **Stock keeping at BOM level** must be enabled in the company data.
> *   ⇨ Tutorial, "Stock control on BOM level" on page G-2484
> *   Master data, "Stock control on BOM level" on page B-984

#### Stock management – stock articles

**Stock management > Stock management > Stock articles tab**

*Fig. G-96 Stock management - stock articles*

Use this tab to check the articles that are managed in the warehouse. The shown stock is updated with each stock booking. You can add new articles and correct the different quantities.

For ordering purposes, you furthermore define minimum quantities and purchase order quantities.
*   ⇨Tutorial, "How to create a stock article" on page G-2497*

**Identification**
*   **Articles**: Product number according to master data. If you want to enter a new stock article, you have to enter it in the master data first.
*   **Stock ID**: Identification number, assigned on receipt of goods.
*   **Name**: Product names from the master data.
*   **Width x height / content**: Dimensions of the stock article in mm (only stock sizes) and content of box. For boxes, enter the number of sheets per box. For all other stock articles, a 1 is automatically shown.
*   **Variation**: If variations have been entered for an article, you will see the color here.
*   **Default storage location**: If you have defined storage locations, they will be offered for selection. If you keep one stock article at several storage locations, you can define a standard storage location. The shown storage location is not defined as standard for the stock article. The shown storage location is defined as standard for the stock article.
    *   ⇨ Master data, "Stock Definition" on page B-789
    > **Storage location <n.e.>**
    > Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.
*   **ID**: The box ID, is assigned on receipt of goods or manually. The ID is only shown if you have selected a box in the overview of stock articles.

**Details**
*   **Category**: If you have defined stock categories in the master data, you can use this field as a search criterion. When you enter new stock articles you can allocate a category.
*   **Del. ID**: The supplier's box ID is only shown if you have selected a box in the Stock articles section.
*   **Main product**: You can link stock articles with several dimensions by specifying a main product. The stock check (for the stock preview in the Stock info dialog) is then only executed for the main product and you only need to enter minimum stock for this main product. If you have also defined minimum stock for the allocated stock articles, they will be ignored for the check.
    *   ⇨ Tutorial, "Main Stock Products" on page G-2493
*   **Prod. batch / date**: Currently not being used.
*   **Date**: Date at which the stock article has been changed last time.
*   **In production**: In connection with A+W Production you can determine whether the stock article has been allocated to production. The stock article is disposable. The stock article has been allocated to production (info only).

**Inventories**
*   **Stock on hand**: Displays the current stock. The stock is updated with each booking of outgoing or incoming stock. For boxes with an ID, stock 1 is always shown. If you have created the stock article new, the field is enabled and you can enter the opening stock.
*   **Stock > 0**: This checkbox is only available in the selection mode. Use it to define as a search criterion whether articles should be shown without stock quantity. The search result also shows articles, the current stock of which is 0. The search result only shows articles, the current stock of which is at least 1.
*   **Min. stock**: The minimum stock forms the basis for automatic purchase order suggestions. They are created if stock falls below the minimum stock. Reservations and purchase orders are taken into account. You can check these automatic purchase order suggestions in the dialog **Stock P.O.**.
    *   ⇨ "Stock P.O." on page G-2640
*   **Minimum stock level > 0**: This checkbox is only available in the selection mode. You can use it to define as a search criterion whether the minimum stock must be more than 0. The search result shows all articles. The search result only shows articles, the minimum stock of which is more than zero.
*   **Purch. qty.**: This value specifies which quantity is ordered by default. This value is adopted for automatic stock ordering.
*   **Inventory < Min. inventory**: This checkbox is only available in the selection mode. You can use it to define as a search criterion whether the minimum stock must be below the minimum inventory. The search result shows all articles. The search result only shows articles, the current stock of which is less than the minimum inventory.
*   **Maximum stock level**: By entering maximum quantities per stock article you can prevent the warehouse becoming overstocked. The entered value is only used for the manual check.
*   **Target quantity**: Currently not being used.
*   **Inventory audit per stock location**: If you maintain stock per storage location you can check the stock per stock location. Stock is checked jointly for all storage locations. Stock is checked per storage location.
*   **Critical stock on hand**: For each stock article, you can specify the quantity starting with which a P.O. is absolutely necessary. So that the value entered is checked, the **Inventory check per storage location** option must be activated. In the stock management, the date is calculated on which the inventory of a stock article drops below this critical quantity. The date on which the stock article reaches the critical quantity is used in the PO pool.
    *   ⇨ Sales, "Order transfer - order pool" on page C-1756

**Stock articles**
The lists show stock articles that correspond to the search criteria. The top list shows all stock articles together. If you select one entry, the articles are shown per storage location in the bottom list. If the checkbox **Stock > 0** has been activated, only storage locations with stock of more than 0 are listed.

The following columns are displayed:
*   **Articles, Variation:** Article number, name, and color from stock management.
*   **Width, Height:** Dimensions from stock management.
*   **Content:** Number of sheets in one box.
*   **Total stock:** Total stock of the stock article at all storage locations.
*   **Min. stock level:** Quantity of the defined minimum stock level.
*   **Purch. quantity:** Defined purchasing quantity.

**Storage locations**
*   **ID:** Box ID (manual booking or from receipt of goods).
*   **Storage location:** Storage location in the order of level 1 through 4.
*   **Stock level:** Current stock level at the storage place.
*   **Del. ID:** Supplier's box ID (only if it has been entered at goods receipt).

#### Stock management – prices

**Stock management > Stock management > Prices tab**

*Fig. G-97 Stock management – prices*

This tab shows the current prices for a stock article. During updates, orders, purchase orders and stock rebookings are taken into account.
*   ⇨ Tutorial, “Prices" on page G-2474*

> **Prerequisite**
> The average purchase price (average PP) is only calculated and shown if the checkbox **Determine purchase price** and the option **Average PP** has been enabled in the company data.
> *   ⇨ Master data, "Average PP: The average purchase price will be recalculated in the following cases:" on page B-981*

The fields in the lists are described in detail in connection with the Stock Article tab.
*   ⇨ "Stock management - stock articles" on page G-2611*

**Purchase prices**
*   **Lowest price**: The lowest price this article has been purchased at.
*   **Max. price**: The highest price this article has been purchased at.
*   **Last price**: The latest price this article has been purchased at.
*   **Stock value**: The current stock prices are shown in this column. They are the result from the respective price and the quantity.

**Calculation of the average price (average PP)**
By selecting an option, determine which stock sizes should be taken into account on this list for the calculation. This setting only makes sense for lite with different stock sizes.
*   **Only this article:** For the calculation only the displayed article in the selected dimension is taken into account. The PP history of the current article is displayed.
*   **All sizes:** For the calculation all dimensions of the displayed glass are taken into account. The PP history of all dimensions of the article is displayed.

The average PP is calculated for each goods receipt, regardless of how it has been booked. Goods issued only reduce the stock. The list is reduced by archiving and auditing.

The first data record shows the opening stock and the original price. Underneath you will find the goods received and issued (minus sign). If goods have been received as a result of a stock P.O., the P.O. number and the P.O. item is furthermore displayed.

The average PP is updated during entering or changing purchase orders. It is determined by taking the total quantity into account.

**Example:**
100 pieces in stock each 15.00 € = 1500.00 €
40 pieces new booking each 18.00 € + 720.00 €
= 2200.00 €
2200.00/140 pcs. = 15.86 €

Automatic surcharges that are listed in the purchase orders, e. g. energy and transportation surcharge, are also included in the calculation.

**Overview**
The respective average prices are shown as history. This way, you can easily monitor price developments. Details displayed:
*   **Date:** Date of the last update.
*   **Quantity [QU]:** Quantity issued or received and quantity unit.
*   **Price/[PU]:** Purchase price per price unit at the time of booking.
*   **Stock on hand [QU]:** Stock on hand at the displayed date. If the average PP is shown for all dimensions, the stock on hand is always shown in sqm.
*   **Average price / [PU]:** Average price per price unit at the time of booking.
*   **P.O./item.:** Number of the purchase order and P.O. item.
*   **Stock value:** Stock value at the displayed date (calculation: purchase price * stock on hand).
*   **Type:** Type of booking that has caused the respective entry.

**Include in total PCH**: You can determine whether the article should be included in the calculation of the total average price of all variations of this article.
*   The article will not be considered for calculating the average price.
*   The article will be included in the calculation.

**Average price**: Current average price. Depending on the option for calculating the average PPs, the display for the current article or the display for all dimensions of the article applies.

> **Updating the display**
> The display of the average prices is updated for the respective stock article during archiving or auditing (invoice check). As a result, the display remains clearer. A+W Business assumes that the prices will not be changed anymore after these processes. However, if you still change prices after one of the processes, these changes are not included in the calculation of the average price.

#### Stock management – supplement

**Stock management > Stock management > Supplement tab**

*Fig. G-98 Stock management – table*

On this tab reservations for a selected stock article are shown.

The fields in the lists are described in detail in connection with the Stock Article tab.
*   ⇨ "Stock management - stock articles" on page G-2611*

**Reservation**
The fields in this area are enabled for individual customers only.
*   **Customer**: Number and name of customer for whom the selected stock article is reserved.
*   **Fully locked**: Currently not being used.
*   **Exclusive reservation**: Currently not being used.

**Supplier**
*   **Supplier**: Number and name of supplier from whom the stock article is ordered.

**Remark**
*   **Product related, Storage location related**: You can enter additional information for each stock article and each storage location, e. g. when and from which supplier glass/boxes were supplied, so that older deliveries are used first.

## Stock Movement

**Stock management > Stock movement**

You can manually book withdrawals and additions for stock articles, correct stock figures, rebook storage locations and resolve boxes.

This chapter provides information on the following subjects:
*   "Options menu" on page G-2620
*   "Stock movement" on page G-2620

### Options menu

**Stock management > Stock movement**

The following entries are displayed:
*   **Protocol at shut down:** When exiting the dialog, the stock history is automatically shown.
    *   ⇨ "Stock history" on page G-2627
*   **Stock > 0:** Only stock articles with a stock on hand of over 0 will be shown.

### Stock movement

**Stock management > Stock movement**

**To the dialog description:**
*   ⇨ Remark (stock movement)

Additions and dispatches of stock articles are automatically booked: for receipt of goods by delivery and for goods issued by orders. You can manually book additions or dispatches in the **Stock Movement** dialog, e. g to correct stock quantities.

Dialog **Stock Movement** offers the following tabs:
*   Stock movement - dispatch, addition
*   Stock movement - transfer
*   Stock movement - number of Sheets
*   Stock movement - open boxes

#### Stock movement – dispatch, addition

**Stock management > Stock movement > Dispatch tab, Addition tab**

*Fig. G-99 Stock movement – dispatch, addition*

You can manually book goods issued and received on the **Dispatch** and **Addition** tabs. You can select a certain stock article and enter the corresponding data. If you have all stock articles displayed you can select the requested article on the **Storage places** list. The fields in the **Change stock on hand** section are then enabled.
*   ⇨ Tutorial, "Withdrawals and Additions" on page G-2503*

If you have activated the option **Protocol at shut down**, the stock history is automatically shown on the **Table** tab when you close the dialog.
*   ⇨ "Stock history – table" on page G-2631*

> **Manually enter addition of boxes**
> Since every box is kept with its own ID, you can enter additions of boxes only via Goods Receipt or Stock Management. This process is explained in Box Management section.

**Stock product**
*   **Product**: Number and name of the stock article.
*   **ID no.**: You can only book stock dispatches via the ID no. Additions of boxes must be defined in Stock Management so that you can enter a new ID.
*   **Contents**: If you have selected a box, then its content is displayed. If a box with an ID no. that has already been allocated to an order is to be delivered or opened, a message is displayed. This prevents negative stock being created by the subsequent printing of the delivery note or invoice.
*   **Storage location**: Storage location that the stock article has been allocated to.
    > **Storage location <n.e.>**
    > Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.
*   **Average purch. price**: The average purchase price is only shown if the function has been activated in the master data.
    *   ⇨ Master data, "Calculate purchase price” on page B-981

**Change stock on hand**
*   **Quantity**: Enter the quantity that is to be booked out or in to stocks in pieces. If you go below the minimum stock when booking articles out of stock, a warning message is displayed.
*   **Width / Height**: These fields are only filled with quantity unit sqm if it involves stock sizes.
*   **Assessment price**: Enter the purchase price at which the goods received were supplied.
*   **Booking date**: The current date is shown automatically. It can be changed if required.
*   **Remark**: You can enter a remark or select from the combo box. The remark will be displayed in the stock history.
    *   ⇨ "Stock history – table" on page G-2631
    Use the button to add a new remark to the list.
    *   ⇨ "Remark (stock movement)" on page G-2624

**Storage locations**
*   **Color:** The color is only shown for variations.
*   **Width, Height:** Dimensions are only shown if the product has been defined as a stock size or box.
*   **Content:** Value 1 is shown for stock articles and stock sizes and the number of sheets for boxes.
*   **Storage location:** Storage location in the order of level 1 through 4.
*   **ID no.:** Box ID (manual booking or from goods receipt).
*   **Stock on hand:** Current stock
*   **QU:** Quantity unit with which the product is kept in stock.
*   **Del. ID:** Supplier's box ID.

#### Stock movement - transfer

**Stock management > Stock movement > Transfer tab**

*Fig. G-100 Stock movement - transfer*

Use this tab to book a stock article to a different storage location. When you transfer a storage location, the entire stock of this storage location is always booked to the other storage location.
*   ⇨Tutorial, "How to transfer the storage location" on page G-2508*

If you have activated the option **Protocol at shut down**, the stock history is automatically shown on the **Table** tab when you close the dialog.
*   ⇨ "Stock history - table" on page G-2631*

The fields in sections **Stock product** and **Storage locations** are described under tab **Dispatch**.
*   ⇨ "Stock movement - dispatch, addition" on page G-2621*

**Storage location**
**Storage location**: Displays the current storage place. You can allocate a different storage place. The combo box lists all stored storage places.

> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.

#### Stock movement – number of Sheets

**Stock management > Stock movement > No. of sheets tab**

*Fig. G-101 Stock movement – number of sheets*

Use this tab to correct the content of boxes.
*   ⇨ Box Management, "Correcting the box contents (number of sheets)" on page K-3061*

If you have activated the option **Protocol at shut down**, the stock history is automatically shown on the **Table** tab when you close the dialog.
*   ⇨ "Stock history – table" on page G-2631*

The fields in sections **Stock product** and **Storage locations** are described under tab **Dispatch**.
*   ⇨ "Stock movement - dispatch, addition" on page G-2621*

**Content change**
*   **Contents**: The number of sheets that are supposed to be included in a box is only shown if you have selected a box with an ID no. You can correct this entry.

#### Stock movement – open boxes

**Stock management > Stock movement > Open boxes tab**

*Fig. G-102 Stock movement – open boxes*

Use this tab to resolve boxes so that the individual sheets are available for production. During this process, the box is booked out of the inventory and the number of sheets is booked to the inventory of the stock size.
*   ⇨ Box Management, "Opening (resolving) boxes" on page K-3062*

> **Book box content to a different storage location**
> When you open a box, its content is booked to the same storage location of where the box is located. If you want to transfer the content, you must book it out of the previous storage location and subsequently, book it to the new storage location.

If you have activated the option **Protocol at shut down**, the stock history is automatically shown on the **Table** tab when you close the dialog.
*   ⇨ "Stock history – table" on page G-2631*

The fields in sections **Stock product** and **Storage locations** are described under tab **Dispatch**.
*   ⇨ "Stock movement - dispatch, addition" on page G-2621*

**Open box**
If a box with an ID no. that has already been allocated to an order is to be delivered or opened, a message is displayed. This prevents that negative stock is created by the subsequent printing of the delivery note or invoice.
*   **No. of boxes**: Number of boxes that are to be opened.
*   **Different contents**: The number of sheets is shown only if you have selected a box. You can correct this value.

### Remark (stock movement)

**Stock management > Stock Movement > [Remark]**

*Fig. G-103 Remark concerning stock movement*

Use this dialog to store remarks that are offered for selection in the **Stock movement** dialog. If you leave the first line blank you can also delete an allocated remark.

## Queries

**Stock management > Queries**

Use the different queries to get a quick overview of stock on hand, movements and values in your stock.

This chapter provides information on the following subjects:
*   "Booking journal" on page G-2625
*   "Stock history" on page G-2627
*   "Stock statistics" on page G-2631
*   "Reserved stock products" on page G-2636

### Booking journal

**Stock management > Queries > Booking journal**

*Fig. G-104 Booking Journal*

In this dialog you can select the criteria for the query. In the booking journal, all automatic order or purchase order processes that relate to the stock are logged, e. g. reservations, purchase orders, additions and dispatches.
*   ⇨Tutorial, "Show Booking Journal" on page G-2513*

#### Selection

*   **Booking type**: You can search the stock for the following booking types:
    *   **(No entry):** If you do not enter any booking type, all articles are shown.
    *   **Reserved:** Only the reserved articles are shown. An article remains reserved until the delivery note or invoice has been printed.
    *   **Delivered:** Only delivered stock articles are shown. An article is marked as delivered after the delivery note or invoice has been printed.
    *   **Ordered:** Only ordered stock articles are shown. The indicator is set as a result of a stock P.O.
    *   **Received:** Only delivered stock articles are shown. An article is considered delivered or received once it has been booked in goods receipt.
*   **Booking date from ... to**: You can restrict the search to a date or time period during which the articles were booked in the stock. When you select the date, pay attention to the time at which the booking was executed. If you have not restricted the display any further, all bookings during the specified time period are displayed.
*   **Storing place**: You can restrict the search to a storage place.
    > **Storage location <n.e.>**
    > Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.
*   **ID no.**: You can restrict the search to a box ID.
*   **Select by**: Choose an option to define what the search should refer to:
    *   **Articles:** You can search for one or several articles. The entry in the fields **Number from** and **to** refers to the product numbers. If you have not selected a booking type, all booking types will be listed.
    *   **Order:** You can search for articles that are included in orders. The entry in the fields **Number from** and **to** refers to the order numbers.
*   **Number from, to**: The search can be restricted to one number or a sequence of numbers.

#### Table

The result of the search is displayed on the list.
*   **Res. type:** Booking type in which the product has been booked.
*   **Order No./P.O. No..:** Number of the order or purchase order from which the booking has been created.
*   **Item No..:** Number of the order or purchase order item.
*   **Qty:** Item quantity.
*   **Product, Name:** Product number and name as per master data.
*   **Color:** The color is only shown for variations.
*   **Width, Height:** Dimensions of the item.
*   **ID:** Box ID (manual booking or from receipt of goods). If the entry is not a box, a zero is displayed.
*   **Del. ID:** Supplier's box ID.
*   **Storage location:** Location at which the product has been booked out or in.
*   **Booking date:** Date of goods receipt.
*   **PP:** Purchasing price of item. Any change of the purchase price at the receipt of goods, check of the delivery OC or invoice is updated in the P.O.

### Stock history

**Stock management > Queries > Stock history**

In the stock history, all processes that refer to the stock are logged. In addition to the booking types, this includes e. g. cut stock plates, corrections, new articles.

The **Stock history** dialog offers the following tabs:
*   Stock history - selection
*   Stock history – table

#### Stock history – selection

**Stock management > Queries > Stock history > Selection tab**

*Fig. G-105 Stock history – selection*

Select the criteria for the query on this tab. The result is automatically shown on the **Table** tab.
*   ⇨Tutorial, "Stock Movements" on page G-2502
*   ⇨Tutorial, "Show Booking Journal" on page G-2513*

**Booking type**
You can search the stock for the following booking types:
*   **(No entry):** If you do not enter any booking type, all articles are shown.
*   **Reserved:** Only the reserved articles are shown. An article remains reserved until the delivery note or invoice has been printed.
*   **Delivered:** Only delivered stock articles are shown. An article is marked as delivered after the delivery note or invoice has been printed.
*   **Cut SS:** This booking type is used by the A+W Optimizer report if an item has been cut from a stock size. The number of stock plates is analyzed.
*   **Ordered:** Only ordered stock articles are shown. The indicator is set as a result of a stock P.O.
*   **Received:** Only delivered stock articles are shown. An article is considered delivered or received once it has been booked in goods receipt.
*   **Manual stock addition/stock dispatch:** Only manually booked stock additions or stock dispatches are displayed.
*   **Stock transfer:** Only stock transfers are shown.
*   **New entry:** Displays only articles that have been newly entered for the stock. The data may have been created within the scope of an inventory or manually. All new articles as of the last archiving process are included.
*   **Correction:** Displays only articles the stock of which has been edited during inventory taking. All corrections as of the last archiving process are included.
*   **Transfer to Recycle Bin, Book back from Recycle Bin, Deleted from stock:** Internal booking types.

**Program**
You can restrict the search to articles that have been processed in a certain dialog of stock management, e. g. Stock transfers.

**Remarks**
You can restrict the search to articles for which a certain remark has been stored. The remark will be displayed underneath the input field.

**Article/order no.**
By selecting an option, you restrict the search to certain articles or orders:
*   **By product from to:** You can select one or several articles.
*   **By document no. from ... to:** You can select one or several orders or purchase orders.

> **Show daily activities**
> If you enter the same article or order number in both fields, all the activities will be displayed that have been booked for an article or order during a certain time period. For this purpose, also enter the booking time.

**Stock ID/serial no.**
*   **Stock ID from ... to**: You can choose one or several stock IDs.
*   **ID No. / Del. ID from ... to**: You can choose one or several IDs. The **ID no.** refers to the box and the **Del. ID** to the supplier's box ID.

**Storage locations**
You can restrict the search for stock articles that were rebooked from a particular level of the storage location to another particular level of the storage location.

**Employee/booking date**
*   **Employee**: You can restrict the search to articles that have been processed by the selected employee.
*   **Booking date from ... to**: You can restrict the search to a booking time period. Ensure that you also enter the time.

#### Stock history – table

**Stock management > Queries > Stock history > Table tab**

*Fig. G-106 Stock history – table*

The result of the query is displayed on this tab.

**Table**
*   **Res. type:** Booking type in which the product has been booked.
*   **Order/P.O. No..:** Number of the order/purchase order and item from which the booking has been created.
*   **Qty:** Item quantity.
*   **ID, Del. ID:** Box ID (manual booking or from receipt of goods) and supplier's box ID.
*   **Product, Name:** Product number and name as per master data.
*   **Color:** The color is only shown for variations.
*   **Width, Height:** Dimensions of the item.
*   **Contents:** Number of sheets in the case of boxes.
*   **PP/PU:** Purchase price per price unit.
*   **Total PP:** Purchasing price of item.
*   **PU:** Price unit of total PP.
*   **QU:** Quantity unit of the item.
*   **Booking date:** Booking date and time.
*   **Execution date:** Date and time at which the process has been booked.
*   **From storage location, To storage location:** Previous and new storage location for transfers.
*   **Employee, Program:** Name of the employee who has booked the process and name of the dialog in which the booking was carried out.
*   **Remarks:** For certain booking types, a remark is displayed, e. g. which corrections were carried out during inventory taking.

### Stock statistics

**Stock management > Queries > Stock statistics**

Stock statistics inform you which ones of your stock articles are hits and which ones are slow sellers. The analyses show initial and end stocks and additions and dispatches of your stock articles per month. This will provide you with information about the stock turnover, average storage duration and average stock on hand of your products.

The **Inventory statistics** dialog includes the following tabs:
*   Stock statistics – products
*   Stock statistics – statistics
*   Stock statistics – FIFO/LIFO

#### Stock statistics – products

**Stock management > Queries > Stock statistics > Products tab**

*Fig. G-107 Stock statistics – products*

Define on this tab the criteria for the statistical analysis. If you mark an entry in the hit list, the corresponding details are displayed on the **Statistics** tab.
*   ⇨Tutorial, "How to display the inventory statistics" on page G-2517*

**Selection**
*   **Year**: Select the year from which data shall be analyzed. You can use it to compare one particular time period with the same time period in the previous year.
*   **Month from ... to**: The selection of the month always refers to the set year. If you want to analyze more than one year you must split the analysis. If you require an analysis that stretches over the turn of the year, you must carry out two analyses consecutively.
*   **Product from ... to**: Select a product or a sequence of products. For each product number, all related stock articles are analyzed, e. g. all the stock sizes, boxes, storage places, etc. for product Float 4 mm.

**Overview**
The overview shows all stock articles matching the search criteria. If you mark an entry of the hit list, the corresponding details are displayed on the **Statistics** tab.
*   **Product:** Product number according to the master data.
*   **Name:** Name defined in the master data.
*   **Width, Height:** Dimensions for stored stock sizes.
*   **Content:** Number of sheets in a box.
*   **ID:** Box ID (manual booking or from receipt of goods).
*   **Color:** Only for variants that are kept on stock.
*   **Storage location:** Storage location of stock article.

> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.

#### Stock statistics – statistics

**Stock management > Queries > Stock statistics > Statistics tab**

*Fig. G-108 Stock statistics - statistics*

On this tab, details are shown for the entry that has been marked on the hit list on the **Product** tab.

**Stock article**
The data of the selected stock article is shown in this section.
*   **Product**: Product number and name according to the master data.
*   **Width / height**: Dimensions for stored stock sizes.
*   **Storage location**: Storage location of stock article.
*   **PP**: Average purchase price and quantity unit.
*   **Content**: Number of sheets in a box.

**Overview**
The overview displays the statistical values for the stock article per month.
*   **Month:** Depending on the selection, individual months or the entire year are/is displayed.
*   **Opening stock:** The closing stock of the previous month is used as the opening stock.
*   **Addition:** Total of all additions within the month. Additions are for example newly created stock articles, manual additions in stock movement and/or goods received from Purchasing.
*   **Dispatch:** Total of all dispatches within the month. Dispatches are either automatically booked when the delivery note or invoice is printed or in the form of manual stock movement.
*   **Closing stock:** Calculation: opening stock + addition - dispatch (within a month).
*   **Stock turnover:** Calculation: Stock dispatch ÷ average stock on hand. The higher the value, the lower the storage time for products.
*   **Average time in storage (in days):** Calculation: days of settlement period ÷ stock turnover. Number of days required to reduce the current closing stock based on the current dispatch.
*   **Average stock on hand:** Calculation: (opening stock + closing stock) ÷ 2.
*   **Initial value/Addition value/Dispatch value/End value:** The stock values are determined on the basis of the purchase price.
*   **Sum of stock on hand:** Calculation: (opening stock + (n * closing stock) / (n + 1), n = number of months.

#### Stock statistics – FIFO/LIFO

**Stock management > Queries > Stock Statistics > FIFO/LIFO tab**

*Fig. G-109 Stock statistics – FIFO/LIFO*

On this tab, the articles kept in stock are displayed assessed according to the FIFO and/or LIFO process. You can select the desired display on the **Options > Initial assessment by** menu.

The data is only displayed if you have started an assessment of the stock values on the **Stock assessment** dialog.
*   ⇨ "Inventory assessment" on page G-2647*

**Overview**
The overview displays the statistical values for the stock article per month.
*   **Date:** Date of the assessment or the inventory.
*   **Receipt:** Total of all receipts in the selected assessment period.
*   **QU:** Quantity unit of the stock article.
*   **Price, PU:** Price and price unit
*   **Residue qty FIFO:** Remaining quantity after the calculation.
*   **Price FIFO:** Price of the remaining quantity after the FIFO calculation.
*   **Residue qty LIFO:** Remaining quantity after the calculation.
*   **Price LIFO:** Price of the remaining quantity after the LIFO calculation.

There is a calculation example in the **Stock assessment** section:
*   ⇨ "Inventory Assessment" on page G-2646*

### Reserved stock products

**Stock management > Queries > Reserved stock products**

*Fig. G-110 Reserved stock products*

Use this dialog to display the orders of a Number Manager to check which stock articles have been reserved. The reserved articles are listed on the printout.
*   ⇨Tutorial, "Stock Control Mode and Reservation" on page G-2453
*   ⇨Tutorial, "How to print a list of reserved stock articles" on page G-2515*

**Selection**
*   **Employee**: Name of the logged-in employee.
*   **Number Manager**: Choose the Number Manager, the orders of which shall be analyzed.

**Table**
*   **Number:** Order number.
*   **Number Cust./Suppl.:** Customer number.
*   **Customer/Supplier:** Name of customer or supplier.
*   **Status:** Status of the order.
*   **Date Entry:** Date on which the order was entered.
*   **Date Delivery:** Date when the order shall be delivered.
*   **Date OC:** Date of the supplier's order confirmation
*   **Lock code:** Lock code from the order.

**Printed list**

*Fig. G-111 Reserved stock articles – output on the screen*

The reserved stock articles are listed per article number and storage place. If there are several storage places the total amount is displayed.

## Search

**Stock management > Search**

You can retrieve the stock on hand by individual stock articles or by product groups.

> **Set filter**
> If no filter is set, no data will be displayed.

The dialog is described in detail in the Sales part.
*   ⇨ Sales, "Stock info" on page C-1825*

Dialog **Stock search** offers the following tabs:
*   Stock search - stock search
*   Stock search - future stock on hand

### Stock search – stock search

**Stock management > Search > Stock search tab**

*Fig. G-112 Stock search - stock search*
