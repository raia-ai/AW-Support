---
title: "EN_UM_AW_SmartCompanion_1_2"
source: "EN_UM_AW_SmartCompanion_1_2.pdf"
tags: ["A+W Smart Companion", "Stock Module", "Inventory Management", "Goods Receipt", "Stock Movement", "Warehouse Management", "ERP", "Tutorial", "Stock Withdrawal"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial for the Stock module of the A+W Smart Companion application. It provides step-by-step instructions for core warehouse functions, including booking goods receipts, managing stock movements and withdrawals, conducting inventory counts, and handling administrative tasks like reprinting labels and editing box contents."
long_description: "This tutorial provides a comprehensive guide to using the Stock module within the A+W Smart Companion mobile application, designed to integrate with A+W Enterprise and A+W Production systems. The document details the complete digitalization of warehouse processes. It begins with instructions on booking goods receipts, covering how to select purchase orders, handle quantity discrepancies, override stock locations, and assign registration points for production orders. It then explains how to perform stock movements between different storage locations. The guide also covers two types of stock withdrawals: with reference to a specific order and without an order for general stock corrections. A significant portion is dedicated to the Inventory feature, explaining how to start and conduct an inventory count, add to already counted quantities, and use the checklist to track progress with list and chart views. Finally, the tutorial covers administrative actions available on the Info page, such as managing missing prices, reprinting box labels, and editing the contents of a box for reasons like breakage or relocation. The document is structured with clear, step-by-step instructions, screenshots, and explanations of UI elements to facilitate user training."
---

# Tutorial: A+W Smart Companion - Stock module

---
## Booking goods receipt

After you have logged in, you are on the **Goods receipt** page. Goods receipt is completely digitalized, both for A+W Enterprise and for A+W Production. Book the incoming goods here.

First, select the supplier/PO number.

### Here's how to select the supplier/PO number
1. Touch the **Supplier/PO number** field. The PO page opens.
2. Touch the desired PO. The PO number is loaded.
3. You are back on the main page.

To display the individual items of the PO, touch the blue **Display items** bar.

**(Image: Overview of the items of a PO)**
*   **Order:** 100300
*   **Supplier:** Spacer Store Corp.
*   **Consignment:** 071187/85.7.2546
*   **Date:** 10.11.20
*   **Item List Example 1:**
    *   **Item:** 300101, Spacer Alu, SP-Alu-12
    *   **Dimensions:** 2000 x 1250
    *   **Quantity:** 200/125
    *   **Storage location:** Table 1
    *   **Variant:** Dark ...
*   **Item List Example 2:**
    *   **Item:** 400101, Spacer PVC, SP-Black-14
    *   **Dimensions:** 6000 x 3210
    *   **Quantity:** 1500/1300
    *   **Storage location:** Stack Warehou...
    *   **Variant:** Black
*   **Item List Example 3:**
    *   **Item:** 500101, Spacer PVC, SPPVX-14
    *   **Dimensions:** 5000 x 4400
    *   **Quantity:** 300/300
    *   **Storage location:** Table 1
    *   **Variant:** White

### Explanation of the elements

The elements for the supplier are displayed in the top area. You see the PO number (order - 100100), the name of the supplier (Spacer Store Corp.), and the consignment (071187/85.7.2546). Next to the consignment is the customer reference number; that is, the number (or name) under which the order is known to the customer. The goods receipt date (11/10/2020) is displayed on the right.

Then the individual items of the PO are listed.
Using the different elements, you can see what kind of PO this is. The following values are possible:

#### Production order
This element represents a PO for a production order. If such goods receipt is booked, the system knows that these are goods that are intended for production. A+W Production and work preparation are informed automatically. You can initiate label printing (optional) and specify a rack (also third-party). This data is stored in A+W Enterprise and in the A+W Production PDC.

#### Stock order
This element represents a PO for a stock order in A+W Enterprise. Stock areas are, e.g. glass stock, hardware stock, stock for PSA, etc.

#### Stock order (Price not stored)
With this element, the employee in the warehouse is made aware that the appropriate price is not yet stored in A+W Enterprise. In this case, only the goods receipt can be booked at first. Then an employee in administration has to be informed via mail that the price has to be maintained for this article. Only if the price is stored can the article be booked to the stock.

In addition to the element, there is an entry in blue and under it, an entry in gray. The entry in blue is the article number and the article name from A+W Enterprise. The entries in gray identify the article number and article name of the supplier. This way, it can be checked quickly during goods receipt whether the goods delivered are those ordered.

> **Display supplier data**
> The supplier's article number and name can only be displayed if they are maintained appropriately in A+W Enterprise. If no supplier-specific data is stored in A+W Enterprise, there will be no gray entries in A+W Smart Companion.

Underneath are the individual items, with their dimensions, storage location, and variants. A variant is, for example, a packaging unit, a size, a color, etc.

### Delivered quantity
This element represents the ordered and delivered quantities.
*   A **gray number** indicates the expected quantity; that is, the quantity that was ordered.
*   A **blue number** indicates that the quantity delivered is identical to the quantity ordered.
*   A **red number** indicates an over- or underbooking of the quantity ordered. With the red numbers, you can get a quick overview of which quantities deviate from the quantity ordered.

#### Here's how to book a delivered quantity
1. In the appropriate item, touch the oval.
2. An area opens where you can change the quantity. By default, the number of the quantity ordered is pre-populated. You can make the entry either by swiping up or down or typing in Manual entry.
3. Enter the desired quantity.
4. Touch **Confirm**.
5. The area is closed and you are back in the overview.

### Tag item
There is a colored bar at the beginning of the line. The bar can be gray or blue. By default, the bar is gray. If you swipe on the item from left to right, a little checkbox appears. If you touch the checkbox, it disappears again and the bar is blue. This is how you can mark items. If you repeat this process, the bar turns gray again.

> **Marking by swiping**
> This item marks itself if you swipe far enough with your finger from left to right.

### Override stock location
If you swipe in the area from right to left, the **Storage location** page opens.

**(Image: Location selection screen)**
*   **Select Stock Location:** Dropdown menu (e.g., Box Warehouse)
*   **Apply Location to All:** Checkbox
*   **Save:** Button

If you touch the combo box, you will see all storage locations created in A+W Enterprise. If there are a lot of storage locations at your company and the page with all storage locations is unclear, you can use the search function to restrict the hit quantity.

If you activate the **Apply selection to all storage locations** checkbox, all items are booked to this storage location.

### Assign registration point
This function is only active if the goods are for a production order.

If you swipe in this area from right to left, the **Storage location** page opens.

**(Image: Registration Point screen)**
*   **Select Registration Point:** Dropdown menu (e.g., Table 1)
*   **Enter Rack Barcode:** Text field with a scan button
*   **Apply Location to All:** Checkbox
*   **Save:** Button

If you touch the combo box, you will see all registration points created in A+W Production. If there are a lot of registration points at your company and the page with all registration points is unclear, you can use the search function to restrict the hit quantity.

In the **Enter rack barcode** field, you can enter the appropriate barcode. If you want to scan the barcode, touch the scan element. An area for scanning opens.

If you activate the **Apply selection to all storage locations** checkbox, all items are booked to this registration point. Finally, touch [Save]. Your selections are taken over and you are back on the main page.

### Saving Inputs
To save your inputs, click the checkmark at the right bottom edge of the display.

If there are quantity differences, regardless of what type (over or underquantity), the following notice appears:

**(Image: Quantity difference options)**
*   Missing items are delivered later
*   Missing items are not delivered later
*   [Cancel] [Send]

Here, you have to specify how to proceed with the quantity differences. You have two possibilities:
*   Missing items are delivered later
*   Missing items are not delivered later

Select the desired option by touching it and then touch **[Send]** to save.

A successful booking is indicated with the following notice:
> **Receipt of goods successfully booked**

## Booking stock movements

With this function, you can book goods from one stock to another one.

**(Image: Stock Location selection screen)**
*   **Stock Location:** Dropdown menu (e.g., Regular Warehouse)

The **Storage location** combo box includes all storage locations created in A+W Enterprise.
The two colored rectangles (blue and gray) at the lower edge of the screen indicate that there are two views here. The active view is always the blue view.

Select the storage location from which you want to take the goods from the combo box. After selection, the system changes automatically to the second page of the view.

**(Image: Stock Movement details screen)**
*   **Stock Location:** Box Warehouse
*   **Stock Articles:** Dropdown menu (e.g., A+W Float 6 mm)
*   **Variant:** Dropdown menu (e.g., 500.0 x 800.0)
*   **Quantity in Stock:** 30
*   **Quantity to be moved:** 5
*   **Target Stock Location:** Dropdown menu (e.g., Single Lite Box Warehouse)

The current storage location is displayed to the right next to the element. In the example above, this is the Box warehouse.

Under that is the **Stock article** combo box. It includes all articles that are currently in the selected storage location.

> **Scanning stock articles**
> If an EAN barcode has been stored in A+W Enterprise for the article, you can also scan the article in question. To scan, touch the element at the end of the line. An area for scanning opens.

The **Variant** combo box includes all existing variants of the selected stock article. **Quantity in stock** shows you how many of the selected article are currently in stock. In the **Quantity that should be moved** field, you specify the quantity that should be rebooked.

The **Target storage location** combo box includes all storage locations created in A+W Enterprise. Select the storage location to which you want to book the article.

### Here's how to re-book articles
1. On the first page, touch the **Storage location** combo box.
2. From the list, select the storage location from which the article should be removed. The view changes automatically to the second page.
3. From the **Stock articles** combo box, select the article that you would like to move.
4. From the **Variant** combo box, select the appropriate variant.
5. In the **Quantity that should be moved** field, specify the appropriate quantity.
6. Select the **Target storage location** to which you want to book the article from the combo box.
7. Touch the white checkmark in the blue dot to save your inputs.

A successful shift is indicated with the following notice:
> **Stock movement successfully booked**

## Booking stock withdrawals

With this function, you can book remove goods from a stock. There are two kinds of stock withdrawals:
*   With order
*   Without order

### Stock withdrawal with order
If the stock withdrawal is done with reference to an order, all information about this order is available in A+W Smart Companion. This way, you always know what has to be removed from stock for this order.

**(Image: Stock withdrawal with order screen)**
*   **Tabs:** WITH ORDER (active) / WITHOUT ORDER
*   **Orders:** Dropdown/scan field (e.g., 100100)
*   **Button:** Show Items

The **Orders** combo box includes all orders created in A+W Enterprise.
Select an order from the combo box for which you want to remove goods from the stock. Alternatively, you can also scan the order number.

Then touch **Display items**. A detailed overview of the order appears.

**(Image: Order details for withdrawal)**
*   **Customer:** Glasshouse 24, Adresse: North York, Toronto, ON M3K 1E7
*   **Delivery Date:** 01.12.20
*   **Item List Example:**
    *   **Item:** 100101, Spacer Alu 12 mm
    *   **Quantity:** 70/70
    *   **Storage location:** Slot Warehouse
    *   **Variant:** Stock...

In the blue area at the top, you can see the customer including the address, as well as the delivery date at the outside right.

Then the individual items are listed. You see the item number, the dimension of the article, the stock location of the article, and, if present, the variant of the article.

In the top area, you can also use the swipe function (from left to right) to mark individual items.

The quantity element represents the ordered quantities and those removed from the stock.
*   A **gray number** indicates the quantity ordered by the customer.
*   A **blue number** indicates the quantity removed from the stock if this matches the quantity ordered.
*   A **red number** indicates an over- or underbooking.

#### Here's how to withdraw goods with reference to an order
1. Select the order from the **Orders** combo box for which you want to remove articles. Alternatively, you can also scan the barcode.
2. Touch **Display items**. The page for the selected order opens.
3. Remove the desired items from the storage location. Correct the quantity if necessary.
4. Touch the blue dot with the white checkmark to save your inputs.

A successful removal is indicated with the following notice:
> **Stock withdrawal (order) successfully booked**

### Stock withdrawal without order
For a stock withdrawal without reference to an order, you have to specify the storage location of the articles to be removed, as well as the quantity in question. This way, you can make stock corrections, for example.

**(Image: Stock withdrawal without order screen)**
*   **Tabs:** WITH ORDER / WITHOUT ORDER (active)
*   **Stock Location:** Dropdown (e.g., Box Warehouse)
*   **Stock Articles:** Dropdown/scan field (e.g., A+W Float 4 mm)
*   **Variants:** Dropdown (e.g., 1000.0 x 1000.0)
*   **Quantity in Stock:** 158
*   **Quantity to be withdrawn:** 1

The **Storage location** combo box includes all storage locations created in A+W Enterprise.
The **Stock articles** combo box includes all articles that are currently in the selected storage location.
The **Variant** combo box includes all existing variants of the selected stock article.

The **Quantity in stock** area shows you how many of the selected article are in stock.

In the **Quantity that should be removed** field, you specify the quantity that you would like to remove. If you remove a quantity that is larger than the quantity on hand, the field is outlined in red. In addition, the Save element is deactivated.

#### Here's how to withdraw goods without reference to an order
1. Use the **Storage location** combo box to indicate the storage location from which you want to take the articles.
2. From the **Stock articles** combo box, select the article that you would like to remove. Alternatively, you can also scan the barcode.
3. If the article comes in different variants, select the appropriate variant from the **Variants** combo box.
4. In the **Quantity that should be removed** field, specify the appropriate quantity.
5. Touch the blue dot with the white checkmark to save your inputs.

A successful removal is indicated with the following notice:
> **Stock withdrawal (order) successfully booked**

## Info page

Using this view, you can call up information about missing prices and take inventory. It is split into two areas:
*   Information
*   Actions

### Information Area
The Information area contains:
*   **Missing prices**

### Actions Area
The Actions area contains:
*   **Inventory**
*   **Print again**
*   **Editing a box**

### Missing prices
Here the articles are listed for which the price still has to be maintained in A+W Enterprise.

**(Image: Price Logs screen)**
*   **Title:** 13 Price Logs
*   **Example Log Entry:** Purchase Order 100100, Item 200102, Article Number 200102, Article Name Vienna - Muntin

The example above shows that there are still 13 articles for which the price is not yet maintained. The employees in the warehouse have no access to the prices here and the prices are also not displayed. In case of missing prices, the employees in the warehouse should make contact with the appropriate employee in administration.

### Inventory
This is where you take inventory.

> **Inventory as independent action**
> The Inventory action is licensed separately. This means that it is not coupled to the Stock module and for inventory you do not absolutely have to have the whole Stock module. This way, you can install the action on several smartphones.

Inventory is started in A+W Enterprise. Stock is not blocked during inventory. This means that during inventory, you can keep working normally. You can book goods receipts and withdrawals and make rebookings.

If the inventory is taken, it is completed in A+W Enterprise. In the next step, the inventory data from A+W Smart Companion is compared to the data in A+W Enterprise.

This saves you a lot of time and minimizes errors. There are no more inventory documents and the quantities counted no longer have to be entered manually.

Employees never see how many of which article should be in which stock. They have to count the quantities present and enter these. Only once an article has been counted is the appropriate value visualized and it can be checked by another employee.
⇨ Add quantity to a quantity already counted

After inventory has been started, the following screen appears:

**(Image: Inventory start screen)**
*   **Title:** Inventory
*   **Field:** Inventory Locations dropdown

#### Here's how to count inventory
1. Open the **Inventory stock** combo box. It includes all stocks created at your company. If you have selected a stock, the view jumps to the next page.
2. Select the article that you would like to count in the **Article number** field. If the appropriate EAN barcodes are stored in A+W Enterprise, you can also scan the article. Then the selected or scanned article is displayed in the field below.
3. If the article comes in different variants, select the appropriate one from the **Variants** field. If you touch the field, the list with all variants appears. Entries that have a green checkmark have already been counted.
4. Touch the **Quantity** field. A numeric keypad appears and you can enter the quantity counted.
5. Touch the blue dot with the white checkmark to save your input.

A successful counting is indicated with the following notice:
> **Stock inventory count successfully stored**

#### Add quantity to a quantity already counted
You can increase a quantity already counted at any time. This can be necessary, for example if articles in the same variant are distributed across several warehouses at your company.

If you select such an article, the following area appears in the display:

**(Image: Add to counted quantity screen)**
*   **Last modified by:** John Moore, 02:10:11 PM 01.12.20
*   **Current Count:** 150
*   **Quantity that should be added:** 56
*   **Actions:** `+` (add to total), `↔` (replace total)

Here you can see which employee counted the article in the appropriate variant on which day and at which time. In the example above, John Moore counted the article on 12/01/2020 at 2:10 AM.

Touch the **Quantity that should be added** field. A numeric keypad appears and you can enter the quantity.

Use the two icons to control what should be done with the quantity entered.
*   With the `+` sign, the quantity you have entered is added to the 150 pieces that John Moore counted.
*   With the `↔` sign, the quantity that John Moore counted is replaced by the quantity you counted.

The active icon is always the one with the blue background.

A successful counting is indicated with the following notice:
> **Stock inventory count successfully stored**

### Checklist
The checklist provides an overview of all articles counted and not counted. At the top, there are icons for two available views:
*   List view
*   Chart view

The active view is indicated in blue, the inactive one in gray.

**(Image: Checklist screen)**
*   **Toggle:** Articles without inventory
*   **Example Entry:** 100104, A+W Float 4 mm, 3/0 (3 variants, 0 counted)
*   **Example Entry:** 200101, Vienna - Muntin, 4/4 (4 variants, 4 counted)
*   **Example Entry:** 100112, A+W Float 12 mm, 2/1 (2 variants, 1 counted)

#### List view
This view shows a simple list of articles and their count status.

#### Chart view
In the **Inventory stock** area, the inventory for the selected stock is displayed. The **Inventory progress** area displays the progress for the selected inventory stock with reference to the variants. The **Inventory status** area displays the overall status of the inventory. The legend below provides information about the status:

*   **Finished (Green):** All variants of the article were counted in the respective stock. If you touch the green area, A+W Smart Companion shows you how many variants of the article were already counted.
*   **Partially (Yellow):** Some variants of the article were already counted, but not yet all. If you touch the yellow area, A+W Smart Companion shows you how many variants of the article were already counted.
*   **Not yet begun (Gray):** No variants of the article were counted. If you touch the gray area, A+W Smart Companion shows you how many variants of the article remain to be counted.

On the right side, there is a slider (**Articles without inventory**). You can use it to control the content of the screen.
*   If the slider is on the left (not active), you will see all articles and variants.
*   If the slider is on the right (active), you will see only the articles and variants for which no inventory has been taken yet. This means that the inventory is only finished when this list has been worked through.

The following status indicators are possible:
*   **Gray exclamation point:** This article has not yet been counted. The field on the right indicates that this article exists in `X` variants (`X`), but no counting has been done yet (`0`). (e.g., 3/0)
*   **Green arrow:** This article has already been counted completely. The field on the right indicates that this article exists in `X` variants (`X`) and that all `X` variants have been counted (`X`). (e.g., 4/4)
*   **Blue partial circle:** This symbol indicates that the counting has been started. The article exists in `X` variants (`X`) and `Y` variants have already been counted (`Y`). The size of the blue section indicates the relationship of counted variants to variants still to be counted. (e.g., 2/1)

### Print again
Here you have the opportunity to reprint labels for boxes. If a box label is no longer legible because it is damaged, for example, you can reprint the label right here. The label will be output immediately on the defined printer.

After you have touched the element, the following page appears:

**(Image: Reprint selection screen)**
*   **Field:** Supplier/Purchase Order Number

In the **Supplier/PO number** area, you will find all box POs for which you can reprint a label. You then only have to select the PO in question. After you have selected the PO, you are back on the main page.

Touch **Display items** in order to display all items for the selected PO. In our example, the PO includes four different articles. 25 pieces of article 100104 were ordered, which are in three different boxes (123, 124, and 125).

Now just touch the box(es) whose labels should be reprinted. After you have selected the box(es), the **Print icon** is enabled. From the number on the icon, you can see how many labels will be printed.

If you touch the icon, printing will start automatically.

#### Here's how to print the new label
1. Touch the **Supplier/PO number** field.
2. Select the appropriate PO.
3. Touch **Display items**.
4. Select the appropriate item(s)/box(es).
5. Touch **Print**.

### Editing a box
Here you have the opportunity to change the contents of a box. You can remove selected lites or break up the entire box. After you have touched the element, the following page appears where you can either scan or manually enter the label of the box in question. Then the following page appears:

**(Image: Edit Box screen)**
*   **Box Number:** 300056929
*   **Article:** 100104, Float 4 mm
*   **Pieces in Box:** 6
*   **Pieces to Move:** 1
*   **Reason Type:** Breakage (selected) / Location
*   **Reason:** Dropdown (e.g., Miscounted)
*   **Remarks:** Text field

The upper area provides information about the box and its contents. In the area below this, you can see in the **Pieces in box** field how many pieces there currently are in the box. In the **Pieces to move** field, enter how many pieces you would like to remove from the box.

Then you must specify the reason why you want to change the contents of the box. There are two different reasons available:
*   **Reason for removal**
*   **Storage location**

If you select the **Removal reason** radio button, you are removing the article because it is either damaged (e.g., broken) or it does not correspond to the details entered (e.g., wrong size). In this case, you must select the appropriate reason from the combo box below (e.g., broken). In the **Notes** field, you can leave an appropriate comment.

Enable the **Storage location** checkbox if you are removing one or several articles from the box in order to store it/them in an appropriate storage location. The combo box includes all storage locations created at your company. Select the desired storage location.

Touch the blue circle with the white checkmark to confirm the details entered.

#### Here's how to remove an article from the box, e.g. in case it is broken
1. Select the **Edit box** action.
2. Scan the box barcode or enter it manually.
3. In the **Pieces to move** field, enter how many pieces you would like to remove.
4. Enable the **Reason for removal** radio button.
5. From the **Reason** combo box, select the appropriate reason, e.g. broken.
6. In the **Notes** field, you can leave an appropriate note.
7. Touch the blue dot with the white checkmark to save your input.

A successful booking is indicated with the following notice:
> **Move from box successfully booked.**

#### Here's how to book an article out of the box to another storage location
1. Select the **Edit box** action.
2. Scan the box barcode or enter it manually.
3. In the **Pieces to move** field, enter how many pieces you would like to remove.
4. Enable the **Storage location** radio button.
5. From the **Storage location** combo box, select the storage location to which the lite should be booked, e.g., specialized warehouse.
6. Touch the blue dot with the white checkmark to save your input.

A successful booking is indicated with the following notice:
> **Move from box successfully booked.**

## Settings
The **Settings** are identical for the Production and Stock modules. To avoid redundant explanations, this process will be described in connection with the Production module.
⇨ Settings
