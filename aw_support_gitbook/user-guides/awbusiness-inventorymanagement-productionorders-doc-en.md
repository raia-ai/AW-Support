---
title: "EN_AWBusiness_Inventory_Management_6_2-2"
source: "EN_AWBusiness_Inventory_Management_6_2-2.pdf"
tags: ["Inventory Management", "A+W Business", "Production Orders", "Stocktaking", "Periodical Inventory", "ERP", "Tutorial", "Stock Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial for the A+W Business Inventory Management software. This guide details the process of creating and managing production orders to replenish stock and conducting periodical inventory and stocktaking to ensure data accuracy."
long_description: "This document is a comprehensive tutorial for the A+W Business Inventory Management system, focusing on two core areas: Production Orders and Inventory. The first section on Production Orders explains their purpose in replenishing stock on hand. It covers the objectives, benefits, and detailed settings for manual and automatic creation of work orders, including procurement types, booking types, and supplier file configurations. The process flow from detecting a stock shortage to creating a purchase order proposal or a production order is illustrated. The second major section covers Inventory management, detailing how to perform a periodical inventory and stocktaking. It provides a step-by-step guide on creating inventory lists, determining target inventory, entering counted values, and finalizing the inventory to update stock levels. The tutorial includes screenshots of the software's user interface, example calculations, and process flowcharts to guide users through each procedure effectively."
---

# Stock Articles in Documents

---
## Production Orders

### Objectives
- Introducing production orders.
- Introducing the manual and automatic creation of work orders.

### Benefits
- Work orders are used to replenish the stock on hand.
- When the stock on hand falls below the defined minimum, work orders can be created automatically if the diversion to an internal customer is enabled in the supplier file.

### Please note:

| Category | Description |
| :--- | :--- |
| **Procurement type** | All articles entered in a production order have to have the procurement type **Production**. |
| **Booking type** | Unlike common orders, the entered items are not reserved on stock but are marked as **ordered**. |
| **Addition to stock** | Stock additions based on work orders can be booked automatically or by hand: <ul><li>Manual status change in module **Production**.</li><li>Automatic status reports from production.</li></ul> |
| **Default settings** | **Stock management:**<ul><li>Minimum stock</li><li>Purchase order quantity</li></ul>**Master data:**<ul><li>Product management</li><li>Partner management (internal customer)</li><li>Supplier file (diversion to internal customer)</li></ul>**Company data:**<ul><li>Parameters tab</li><li>Tab Stock / PP / EDI > Registration point</li></ul> |

---

## Stock Article as Part of the Production Order

Work orders are used to replenish the stock on hand. All articles entered in such an order are automatically changed to procurement type **Production**. Unlike customer orders, the items are not reserved on stock but are marked as **ordered**.

*Fig. G-70 Item entry - procurement type Production*

A production order differs from other orders only in its document type:

*Fig. G-71 Order entry - document type Production Order*

Work orders can be entered in different ways:
- Enter a new document manually.
- Copy a saved (dummy) article.
- Automatic creation based on a shortage in the stock on hand.

---

## Manual Input by Copying

If you enter work orders on a regular basis, you can copy the previously entered order to make this task easier.

- Before copying, you have to set the document type of the target document to **Production Order**.
- If only certain items shall be adopted from the order, you can select them.
- You can amend the data in the new document.

*Fig. G-72 Create production order by copying (A: Copy from order to order, B: Document type of the target order)*

> A detailed description of the function **Copy documents** can be found in section Sales.

---

## Settings in Supplier File

If a minimum stock and a (standard) order quantity have been defined for the stock article in dialog **Stock management**, the system can create automatic P.O. proposals. These are listed in dialog **Stock P.O.**

This is how purchase orders of the type **Stock P.O.** are usually created. However, if an internal customer is entered in the supplier file instead of a standard supplier, work orders can be created automatically.

*Fig. G-73 Internal customer for work orders (A: Product for which work orders shall be created, B: Diversion to internal customer, C: Customer selection)*

In the supplier file, an internal customer is defined for which the work order is entered automatically. The option **Internal customer** can be enabled on product group or product level. The product settings have priority over the product group settings.

---

## P.O. Quantity after Stocktaking

The program checks whether the current stock on hand plus the already ordered quantities and minus the reserved quantities will fall below the minimum stock on hand.

If this is the case, the P.O. proposal shows the multiple of the (standard) P.O. quantity.

### Manual and automatic stock P.O.

*Fig. G-74 Stock P.O. vs. production order (Flowchart showing the logic: Start with 'Stock P.O. Storage location' -> 'Below minimum stock?' -> 'Standard P.O. quantity?' -> 'Search in supplier file'. Then it branches to 'Standard supplier?' which leads to 'P.O. proposal Stock P.O.', or 'Internal customer' which leads to 'Production order Document management'.)*

---

This flow chart shows A+W Business's reactions to different presettings in the supplier file.

### Purchase order quantity

The multiplier will be calculated so that as a result of the P.O. proposal the minimum stock is exceeded.

*Fig. G-75 Quantities for stock articles (dialog Stock management)*

> **Example**
>
> Tempered glass with article number 4008 is kept as a stock article.
>
> - Current stock on hand: 10 pcs.
> - Minimum stock: 30 pcs.
> - P.O. quantity: 5 pcs.
>
> The P.O. quantity for tempered glass 4008 is calculated as follows:
> Difference between current stock on hand and minimum stock on hand: 20 pcs. This difference includes the P.O. quantity of 5 pcs. four times.
>
> P.O. quantity: 4 x 5 = 20 pcs.
> Current stock on hand plus ordered quantity: 10 + 20 = 30 pcs.

The calculated quantity is adopted for the P.O. proposal. It can be amended in the **Stock P.O.** dialog.

---

*Fig. G-76 Stock P.O.- P.O. proposals (A: Restriction to storage location, B: P.O. proposal for production order)*

In the **Stock P.O.** module you have already been shown how to edit and transfer purchase orders.

⇨ "Transfer Stock P.O. to Purchasing" on page G-105

The production order is created by the transfer, in the last active order Number Manager.

---

*Fig. G-77 Production order in Number Manager for orders (A: Automatically created production order)*

The production order can now be opened as a document.

---

*Fig. G-78 Document Production Order (A: Order header – Production order, B: Ordered quantity)*

The work order can be edited and transferred to production.

---

## Stock Addition based on Production Order

On tab **Stock / PP / EDI** in company data, set the limit status for registration points to define from which point on an order counts as produced. The limit status is the status defined for the selected registration point.

*Fig. G-79 Company data – Stock / PP / EDI: Registration point for status change*

There are two ways of entering additions to stock based on production orders:
- If the status of the work order exceeds the defined status due to a report from production, the addition to stock is booked automatically.
- If you do not use production reports, you can enter the addition to stock by means of the manual status report in the **Production** module. If you set the production order there to a status above the aforementioned limit, the stock withdrawal of the material consumed and the addition of produced stock articles to stock are booked automatically.

If no other storage location has been defined, the order quantity is allocated to the standard storage location.

The booking of work orders is described in detail in section **Production**.

**Additional information**
- ⇨ Master Data, "Company Data – Stock/Purchasing/EDI" on page B-955
- ⇨ Sales, "Order Header" on page C-38
- ⇨ Sales, "Change P.O. Code" on page C-306
- ⇨ Production, "Production Orders" on page E-128

---

## Inventory

This section shows you how to correct the stock on hand in A+W Business by means of an inventory.

This includes the following training modules:
- "Periodical Inventory" on page G-137
- "Initial Inventory" on page G-153

---

## Periodical Inventory

### Objectives
- Getting familiar with the inventory process.
- Learning about the inventory dialogs.
- Carry out inventory.

### Benefits
- An inventory can be used to correct the stock on hand in A+W Business.
- For big storage locations, the inventory can be organized in such a way that common business operations are impeded as little as possible.

### Please note:

| Category | Description |
| :--- | :--- |
| **No change of stock during the inventory** | On the day of the count, no orders, purchase orders or receipt of goods must be entered; no goods must be removed from or added to stock. The target inventory should be determined on the day of the count. |
| **The inventory process** | The inventory is run in three steps: <ul><li>Create inventory list</li><li>Determine target inventory</li><li>Enter counted values</li><li>Finalize inventory</li></ul> |
| **Split stocktaking** | For large storage locations it may be useful to run the inventory in smaller units. |
| **Separate stocktaking for boxes** | A special inventory list is created for boxes. The existing boxes are scanned individually. |
| **No changes to the product master data** | As soon as the inventory list has been created, all the products that are listed on the inventory list are marked in product management (master data). The procurement type and stock code in these products are then blocked. The marking will be deleted once the inventory has been taken. |
| **Complete the inventory list** | Additions must be made only before the target stock is determined. |
| **Target inventory in the count list** | To print the target inventory on the count list you have to determine the target inventory before printing. |
| **Final inventory by inventory list** | The final inventory can be run just once per inventory list. |
| **Default settings** | None |

---

## Stocktaking

At least once in every business year, stock has to be taken to check if the booked or target inventory shown in A+W Business Stockkeeping matches the actual stock. Inventory lists are created for this statutory annual stocktaking which help to count and enter the actual stock on hand. Stocktaking determines the existing stock by type, quantity, and value.

Basis for any stocktaking is the inventory list which can refer to selected stock articles and/or storage locations. This way, stock can be taken in several steps which presents less of an obstruction to the daily business.

A+W Business provides inventory lists and the target inventory for stocktaking. Stocktaking can be done in the conventional way or, for boxes, with the help of barcode registration.

Stocktaking is completed by the final inventory. After that, the quantities will be updated in A+W Business.

### Actual stock on hand

The stock on hand is entered on the basis of count lists. New stock articles can be entered at the same time. During stocktaking, the stock articles on the inventory list are not locked for document entry. This is why no orders, purchase orders, or receipt of goods must be entered on the day of the count.

### Target inventory

The target inventory must be determined no later than on the day of the count. This allows you to create the inventory list well in advance of the actual counting, input of the counted quantities, and the final inventory.

> **Example**
>
> | Activity | Date | Stock on hand | Target inventory |
> | :--- | :--- | :--- | :--- |
> | Inventory list created | 15 Dec | | 100 |
> | Count stock on hand | 31 Dec | 80 | 100 |
> | Sales | 01 Jan to | -30 | -30 |
> | Purchasing | 14 Jan | +10 | +10 |
> | | 15 Jan | Actual stock on hand 60 | 80 |
> | Final inventory | | New target inventory: | 60 |

With the final inventory, the actual stock is saved in the system as the new target inventory.

The target inventory can be printed on the count lists if required. If you do not print the target inventory you can practically neglect the "counted" quantities estimated on the basis of the target inventory.

---

### sqm articles

If individual sheets of defined sizes are counted for a sqm article, these can be entered as units. At the final inventory, these will be converted into sqm and booked as such on stock (the printed closing inventory will show the counted quantity however).

### Stocktaking of boxes

To take stock of boxes for the inventory list, first create an inventory list then determine the target inventory. Now scan or manually enter the box ID, the storage location, and - if applicable - a different number of sheets. Scanning a box will always add it to the latest inventory list. Now enter the remaining stock in Inventory Management if necessary, and book the final inventory.

### Example count list

*Fig. G-80 Count list with fields for the counted quantities*

The counted quantities are entered in the count list and, later, in inventory management.

---

## Create Inventory List

The inventory is based on lists in which the manually counted quantities are noted. These lists can be based on various criteria, and can be printed.

When you print these lists and realize that certain articles are missing, you can add a supplementary inventory. This way, you will not have to print all lists again.

> **No changes to the product master data**
> When the inventory list has been created, all products that appear on the inventory list are marked in product management (master data). The procurement type and stock code in these products are then blocked. This mark will be deleted when the inventory has been finalized; the data can be edited again.

This session shows you how to create inventory lists and open them again.

The following instructions exist for this training module:
- "How to start an inventory" on page G-141
- "How to print the count lists" on page G-143
- "How to load a saved inventory list" on page G-144
- "How to complete an inventory list before counting" on page G-144

---

### How to start an inventory

1. Go to menu **Stock management > Stocktaking > Inventory list**.
   Dialog **Inventory list** opens.
2. Go to the menu **Start > New** to switch to the input mode.

*Fig. G-81 Fields for the new inventory list are enabled (A: All articles or sequence of article numbers, B: Inventory date, C: Restrictions, D: Inventory evaluation, E: Sorting the list)*

The name for this inventory is a date (B). The system will suggest the current date by default. You can enter or select any other date of course.

3. Choose the articles (A) for the inventory:
    - **All articles**:
      You can take stock of all articles defined as products in the master data. In this case, the fields for the article numbers are locked. Enable this option for the initial inventory; for all other inventories, you can restrict the inventory lists to certain articles.
    - **Article number**:
      You can restrict the inventory list to a sequence of article numbers. The fields are locked if you have selected the option **All articles**.

4. If applicable, restrict the list further (C):
    - **Only products with stock > 0**:
      You can restrict the inventory to stock articles with inventory. If you do not check the checkbox, the complete product master data will be included in the inventory list unless the selection is not restricted by other criteria.
    - **Only products with assigned stock product**:
      You can restrict the inventory to the stock articles in stock management. If you do not select this checkbox, the entire product master data including stock size table will be included in the inventory list unless the selection is restricted by other criteria.
    - **Only products with stock in the product**:
      You can restrict the inventory to products with procurement type **Stock withdrawal**.
    - **No box with ID number and inventory = 0**:
      The stock on hand can include boxes which have already been shipped but not deleted. Their stock is correctly displayed as 0. You can hide these boxes because no quantities will be entered for them.
    - **Only for defined storage location**:
      This setting activates the fields for selecting the storage location. If you want to take stock only for certain storage locations, you can create separate inventory lists. Please note that articles can also be booked to storage location `<n.e.>`. In case of comprehensive stocktaking you can also split the inventory list by storage location for the printout.

5. Choose the inventory evaluation type (D).
   If you have enabled the options for PP calculation in the company data, you can have the stock evaluation calculated as follows:
    - **PP price list**:
      The individual prices of the products from the PP rate assignment are used.
    - **Lowest PP**:
      For all articles, the lowest value is used for the inventory valuation each time.
    - **Cut PP**:
      For all articles, the average PP is used. For this, the **Article PP** option must be activated in the company data.

6. Choose the sorting type (E).
   Sorting of articles on the inventory list should be based on the defined criteria. The option **Size** is useful for stock sizes for example.

7. Go to the menu **Start > Save** to create the inventory list.
   The inventory list opens in the overview. You can now print the count lists and/or determine the target inventory.

> **No changes to the product master data**
> As soon as the inventory list has been created, all the products that are listed on the inventory list are marked in product management (master data). The procurement type and stock code in these products are then blocked. As soon as the inventory has been completed, the marking is deleted and the data can be edited again.

---

### How to print the count lists

To print the target inventory on the count list you have to determine the target inventory prior to printing.

1. Go to menu **Stock management > Stocktaking** and select the date of the inventory list.
2. Go to the menu **Start > Search** to load the inventory list.
   These steps are redundant if you print the count list immediately after creating the inventory list.
3. Go to menu **Print > Printer**.
   To check the result on screen first, select **Screen**. You can start the printout if you are satisfied with the result. The following steps are the same for both settings.

*Fig. G-82 Inventory - Print count list (A: Page break, B: Articles that shall be printed, C: Sorting)*

Print the count lists so that they match the tasks of your stocktaking staff.

4. Define the point at which a new page (A) shall be started.
   If you did not define different storage locations, this setting can be omitted. If you have split the count areas by storage location, start a new page after the corresponding storage locations.
   You must select at least one warehouse (level 1) for the printout.
5. Define the stock articles (B) to be printed on the list.
   If different stock articles are stored in the individual storage locations, you can distinguish finished products and raw material. **Finished products** are stock articles which are not stored in the raw material stock.
   The characteristics **Finished products** and **Raw material** have been assigned in stock definition.
   ⇨ "Define Storage Location" on page G-22
6. Sort (C) the articles on the count list depending on the selected criteria. The option **Article** makes sense for instance if the stock is organized by products.
7. Click **[OK]** to start printing.
   The list is printed and can be used for counting.

---

### How to load a saved inventory list

1. Go to menu **Stock management > Inventory**.
2. Go to field **Inventory date** and select the date on which the inventory list has been saved.
3. Go to the menu **Start > Search** to load the inventory list.
   The inventory list opens.

### How to complete an inventory list before counting

If you have already determined the target inventory for an inventory list, you cannot complete this list. In this case, close the inventory and enter the missing articles in a new inventory list.

1. Go to menu **Stock management > Inventory**.
2. Go to the menu **Start > New** to switch to the input mode.
   The fields will be enabled.
3. Select the inventory list to which articles shall be added.
4. Select the stock articles and/or storage locations.
5. Go to the menu **Start > Save** to save the data.
   A query is displayed that allows you to abort this process or complete it.
6. Select:
    - **[Yes]**: The existing list is displayed, the new articles are added at the end.
    - **[No]** or **[Abort]**: The query is closed. You can change the date or other criteria and create a new inventory list.

---

## Determine Target Inventory

The target inventory has to be determined for every inventory list. It defines the quantities that should be on stock according to the system. To print the target inventory on the count lists you have to determine the target quantity prior to printing a list.

> **No inventory bookings on the count day**
> After the target quantity has been determined, the stock quantities must be counted. On the day of the count, no stock articles may be withdrawn and no stock movements may be booked until counting has been finalized. This applies to all manual or automatic stock withdrawals/additions, and all goods received into stock based on purchase orders. A+W Business is not automatically blocked for bookings.

This module shows you how to determine the target inventory for a saved inventory list.

### How to determine the target inventory for an inventory list

1. Go to menu **Stock management > Inventory > Target inventory**.
   Dialog **Target inventory** opens.
2. Load the inventory list for which you want to determine the target inventory.

*Fig. G-83 Determine target inventory*

3. Go to menu **Start > Execute** to determine the target inventory and confirm the query by **[Yes]**.

The target inventory is entered in column **Target**. You can determine the target inventory just once per inventory list. The result will not be updated even if you execute this function several times.

If the target inventory shall be printed on the count list, you can start the printout now.

You can now start counting and subsequently enter the counted quantities.

---

## Enter Counted Values

Once you have entered the counted quantities in the printed count lists, you can enter the values in dialog **Inventory management**.

This module will show you how to enter the counted quantities in A+W Business plus a new stock article if necessary.

The following instructions exist for this training module:
- "How to enter the counted quantities" on page G-147
- "How to enter a new stock article during stocktaking" on page G-148

### How to enter the counted quantities

1. Go to menu **Stock management > Inventory > Inv. Management**.
   Dialog **Inv. Management** opens.
2. Load the inventory list.
   The table shows the records in the same sequence as on the printed list.
   Menu **Sorting** can be used to choose another sequence if this will facilitate the entry of the counted values.

*Fig. G-84 Inventory - Enter counted quantities (A: Enter counted quantity, B: List of records)*

3. Enter the quantity (A) for the first item in field **Qty** and confirm by `<Enter>`.
   The marking automatically switches to the next line where you can enter the next quantity.
4. To enter the quantities in a different sequence, just select the line in question.

> **Quantity and storage location for several articles**
> You can select several records and set the quantity for all to zero or change the storage location by using the **Functions** menu.

5. If necessary, you can change the storage location, the inventory price, and the category to be used for inventory evaluation.
   Changed inventory prices will not be saved in the purchase price table after the finalization of the inventory, and will not be considered for calculating the average purchase price.
6. Go to the menu **Start > Save** to save the data.
   The data is saved. If you have not entered the data completely yet, you can resume the input later. Start from step 1 in this case.
   You can finish stocktaking when you have entered all quantities.

### How to enter a new stock article during stocktaking

1. Go to menu **Stock management > Inventory > Inv. Management** and select the current inventory.
2. Select the record for which you want to enter a new stock article.
3. Go to the menu **Start > New** to switch to the input mode.
   All data of the original stock article will be copied so that you only have to edit the data for the new stock article.
4. Enter the width, height, storage location etc.
5. Go to the menu **Start > Save** to save the data.
   The list is completed by the new stock article.

---

## Finalize Inventory

Stocktaking is finalized by booking the results of counting and updating the stock on hand.

The final inventory can be run just once per inventory list. Should you detect errors in the counted or entered quantities after closing, you have to correct the quantities in dialog **Inventory management**, or create and finalize a new inventory list for the corresponding article.

This module shows you how to to finalize the inventory for an inventory list.

For instructions on this subject, please see:
- "How to finalize the inventory" on page G-149
- "How to delete an inventory list after the final inventory” on page G-150

### How to finalize the inventory

1. Go to menu **Stock management > Inventory > Final Inventory**.
   Dialog **Final Inventory** opens.
2. Load the inventory you want to finalize.

*Fig. G-85 Inventory - Final Inventory*

The inventory list is displayed with the quantities entered.

3. Check in the **Options** menu whether the stock on hand should be set to zero with or without query when no quantities have been entered.
4. Select production preparation for which stocktaking has been restricted.
5. Go to menu **Start > Execute** and confirm the query by **[Yes]** in order to finalize the inventory.

> The data will be saved and the stock on hand values and the prices for the inventory evaluation will be updated. Booked records are deleted from the list. The locks in the product master data will be removed.
>
> Records that could not be booked are kept on the list. You can complete the missing entries in dialog **Inv. Management**.
>
> If all records could be booked, the complete inventory list will be deleted from the final inventory.
>
> **Inventory errors**
> If errors have occurred during stocktaking and individual records are not deleted from the inventory list, you can use the log to search for the cause. Open the log via **System > Log**.

### How to delete an inventory list after the final inventory

> **Do not delete individual records**
> After the final inventory, individual records cannot be deleted from the list.

1. Go to menu **Stock management > Stocktaking > Inventory list**.
2. Load the inventory list you have finalized.
3. Go to menu **Start > Delete** and confirm the query by **[Yes]**.
   The inventory list is deleted. If further inventory lists were created, the next list will be loaded now.
