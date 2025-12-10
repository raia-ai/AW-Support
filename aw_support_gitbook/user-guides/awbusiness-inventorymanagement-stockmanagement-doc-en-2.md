---
title: "EN_AWBusiness_Inventory_Management_6_2-4"
source: "EN_AWBusiness_Inventory_Management_6_2-4.pdf"
tags: ["inventory management", "stock management", "A+W Business", "software reference", "final inventory", "stock movement", "queries", "booking journal", "average price calculation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical reference guide for the A+W Business Inventory Management software. It covers procedures for finalizing inventory counts, managing stock articles and prices, booking stock movements (dispatches, additions, transfers), and running queries like booking journals and stock histories."
long_description: "This document is a detailed software reference manual for the A+W Business Inventory Management module. It provides step-by-step instructions and field-level descriptions for several key inventory processes. The guide begins with the 'Final Inventory' process, explaining how to conclude inventory taking and finalize stock counts. It then moves to 'Stock Management,' detailing how to view, add, and manage stock articles, including their prices and supplementary data. This section covers the calculation of average purchase prices (average PP). The manual also explains 'Stock Movement,' which includes manually booking dispatches, additions, transfers, correcting sheet counts in boxes, and opening boxes. Finally, it describes the 'Queries' section, which allows users to generate reports like the Booking Journal and Stock History for a quick overview of stock on hand, movements, and values. The document is intended for users who need to perform and manage inventory tasks within the A+W Business software."
---

---
## Final Inventory

**Path:** `Stock management > Inventory > Finalization`

You conclude inventory taking with the final inventory. You can book stock again directly after counting.

This chapter provides information on the following subjects:
- "Menus in Final Inventory” on page G-180
- "Finalization" on page G-181

### Menus in Final Inventory

**Path:** `Stock management > Inventory > Finalization`

The menus can be used to define the standard settings or open other dialogs without closing this dialog.

This chapter provides information on the following subjects:
- "Options menu" on page G-180
- "Functions menu" on page G-180

#### Options menu

**Path:** `Stock management > Inventory > Finalization`

The following entries are displayed:

- **Do not print articles with stock on hand = 0:** Only articles with stock on hand that is more than 0 will be printed. This setting is helpful if you have many articles without stock figures. This makes the printed list clearer.
- **Check whether the stock for uncounted articles shall be set to 0:** Use this function to define that the quantity of articles for which no stock has been entered is only then set to 0 when you have confirmed this for each article.

#### Functions menu

**Path:** `Stock management > Inventory > Finalization`

The following entries are displayed:

- **Add supplementary inventory:** Opens the dialog Select inventory list in order to print and analyze two different inventories in one joint list.
  ⇨ "Select Inventory List" on page G-183

## Finalization

**Path:** `Stock management > Inventory > Finalization`

*(Fig. G-94 Final inventory)*

Use this dialog to finalize the inventory for each inventory list. With it, the entered values are adopted in the stock on hand (stock lists). Any goods issued or received in the meantime are taken into account. New stock articles from the inventory are automatically adopted in inventory management.

⇨ Tutorial, "Finalize Inventory" on page G-150

> **Per inventory list only one final inventory**
> The final inventory can only be executed once per inventory list. Any entry errors can only be corrected in inventory management after the final inventory. Alternatively, a new inventory list can be created with the incorrectly entered articles.

### Booking

- **Inventory date:** Date of the inventory that is to be finalized.
- **Book by supply type as per production preparation:** If you work with order areas, stock may be allocated for a certain production preparation, e. g. for the production of LAMI. The field for selecting the production preparation is enabled only if you have checked the checkbox.
  - The counted stock is allocated to the standard storage place.
  - The stocks shall be allocated to a production preparation.
  ⇨ Master Data, "Order Areas" on page B-1014
- **Record no. from ... to:** Displays the first and last record number of the loaded inventory list.

### Overview

- **Record no.:** Sequential number on the inventory list.
- **Art. no.:** Product number according to the master data.
- **Name:** Product name from the master data.
- **Content:** Value 1 is shown for stock articles and stock sizes and the number of sheets for boxes.
- **ID:** Box ID (manual booking or from receipt of goods).
- **Width, Height:** Dimensions are only shown if the product has been defined as a stock size or box.
- **Storage location:** Storage location in the order of level 1 through 4.
- **Quantity:** Value that has been entered as the counted quantity.
- **QU:** Quantity unit with which the product is kept in stock.
- **Status:** The status is only shown if the record could not be booked. Use the logbook to check for the possible causes.

## Select Inventory List

**Path:** `Stock management > Inventory > Finalization > Functions menu > Add supplementary inventory`

*(Fig. G-95 Add supplementary inventory)*

A supplementary inventory can only be added if both inventories have been finalized. Both inventories can then be printed on a joint list and be analyzed.

⇨ Tutorial, "How to add a supplementary inventory" on page G-152

## Stock Management

**Path:** `Stock management > Stock management`

Use the dialog Stock management to display all the stock articles that are managed.

This chapter provides information on the following subjects:
- "Menus in Stock Management" on page G-184
- "Stock Management" on page G-185

### Menus in Stock Management

**Path:** `Stock management > Stock management`

The menus can be used to define the standard settings of the dialog or open other dialogs without closing this dialog.

This chapter provides information on the following subjects:
- "Functions menu" on page G-184
- "Options menu" on page G-185
- "Print menu" on page G-185

#### Functions menu

**Path:** `Stock management > Stock management > Functions menu`

This menu allows you to open other dialogs without closing stock management.

The following entries are displayed:
- **Stock History:** Opens the dialog Stock History with the log of processes that have been booked in stock management.
  ⇨ "Stock History" on page G-204
- **Booking Journal:** Opens the dialog Booking Journal with the log of stock bookings from orders and purchase orders.
  ⇨ "Booking Journal" on page G-202

### Options menu

**Path:** `Stock management > Stock management > Options menu`

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

The following entries are displayed:
- **Do not print articles with stock on hand = 0:** Only articles with stock on hand that is more than 0 will be printed. This setting is helpful if you have many boxes with an ID, but without stock. Usually, these have been delivered as boxes and were deleted from the stock. This setting applies only to printing; the dialog shows all the articles.
- **Automatic ID allocation:** The box ID can be allocated automatically even it has been booked as stock manually.

### Print menu

**Path:** `Stock management > Stock management > Print menu`

Use this menu to start the printout of labels.

The following entries are displayed:
- **Box labels:** Only labels for boxes will be printed. For this, the print point 973 must be created and the report boxlabel.qrp assigned in the form management.
- **Standard:** Labels for stock articles will be printed.

### Stock Management Dialog

**Path:** `Stock management > Stock management`

In the Stock Management dialog you enter all the stock articles that are kept in the warehouse with stock on hand.

Stock sizes are maintained in A+W Business even in product management. They are used to allocate price codes, product groups, etc.

Dialog Stock Management offers the following tabs:
- Stock Management - Stock Articles
- Stock Management - Prices
- Stock Management - Supplement

> **Stock management at the level of bills of material**
> In the warehouse, you can also manage products that are included as bill of material components in other products. For this purpose, the checkbox Stock keeping at BOM level must be enabled in the company data.
> ⇨ Tutorial, "Stock control on BOM level" on page G-58
> ⇨ Master Data, "Stock control on BOM level" on page B-958

## Stock Management - Stock Articles

**Path:** `Stock management > Stock management > Stock articles tab`

*(Fig. G-96 Stock Management - Stock Articles)*

Use this tab to check the articles that are managed in the warehouse. The shown stock is updated with each stock booking. You can add new articles and correct the different quantities.

For ordering purposes, you furthermore define minimum quantities and purchase order quantities.

⇨ Tutorial, "How to create a stock article" on page G-71

### Identification

- **Articles:** Product number according to master data. If you want to enter a new stock article, you have to enter it in the master data first.
- **Stock ID:** Identification number, assigned on receipt of goods.
- **Name:** Product names from the master data.
- **Width x height / content:** Dimensions of the stock article in mm (only stock sizes) and content of box. For boxes, enter the number of sheets per box. For all other stock articles, a 1 is automatically shown.
- **Variation:** If variations have been entered for an article, you will see the color here.
- **Default storage location:** If you have defined storage locations, they will be offered for selection. If you keep one stock article at several storage locations, you can define a standard storage location.
  - The shown storage location is not defined as standard for the stock article.
  - The shown storage location is defined as standard for the stock article.
  ⇨ Master Data, "Stock Definition" on page B-736
> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.
- **ID:** The box ID, is assigned on receipt of goods or manually. The ID is only shown if you have selected a box in the overview of stock articles.

### Details

- **Category:** If you have defined stock categories in the master data, you can use this field as a search criterion. When you enter new stock articles you can allocate a category.
- **Del. ID:** The supplier's box ID is only shown if you have selected a box in the Stock articles section.
- **Main product:** You can link stock articles with several dimensions by specifying a main product. The stock check (for the stock preview in the Stock info dialog) is then only executed for the main product and you only need to enter minimum stock for this main product. If you have also defined minimum stock for the allocated stock articles, they will be ignored for the check.
  ⇨ Tutorial, "Main Stock Products" on page G-67
- **Prod. batch / date:** Currently not being used.
- **Date:** Date at which the stock article has been changed last time.
- **In production:** In connection with A+W Production you can determine whether the stock article has been allocated to production.
  - The stock article is disposable.
  - The stock article has been allocated to production (info only).

### Inventories

- **Stock on hand:** Displays the current stock. The stock is updated with each booking of outgoing or incoming stock. For boxes with an ID, stock 1 is always shown. If you have created the stock article new, the field is enabled and you can enter the opening stock.
- **Stock > 0:** This checkbox is only available in the selection mode. Use it to define as a search criterion whether articles should be shown without stock quantity.
  - The search result also shows articles, the current stock of which is 0.
  - The search result only shows articles, the current stock of which is at least 1.
- **Min. stock:** The minimum stock forms the basis for automatic purchase order suggestions. They are created if stock falls below the minimum stock. Reservations and purchase orders are taken into account. You can check these automatic purchase order suggestions in the dialog Stock P.О..
  ⇨ "Stock P.O." on page G-220
- **Minimum stock level > 0:** This checkbox is only available in the selection mode. You can use it to define as a search criterion whether the minimum stock must be more than 0.
  - The search result shows all articles.
  - The search result only shows articles, the minimum stock of which is more than zero.
- **Purch. qty.:** This value specifies which quantity is ordered by default. This value is adopted for automatic stock ordering.
- **Inventory < Min. Inventory:** This checkbox is only available in the selection mode. You can use it to define as a search criterion whether the minimum stock must be below the minimum inventory.
  - The search result shows all articles.
  - The search result only shows articles, the current stock of which is less than the minimum inventory.
- **Maximum stock level:** By entering maximum quantities per stock article you can prevent the warehouse becoming overstocked. The entered value is only used for the manual check.
- **Target quantity:** Currently not being used.
- **Inventory audit per stock location:** If you maintain stock per storage location you can check the stock per stock location.
  - Stock is checked jointly for all storage locations.
  - Stock is checked per storage location.
- **Critical stock on hand:** For each stock article, you can specify the quantity starting with which a P.O. is absolutely necessary. So that the value entered is checked, the Inventory check per storage location option must be activated. In the stock management, the date is calculated on which the inventory of a stock article drops below this critical quantity. The date on which the stock article reaches the critical quantity is used in the PO pool.
  ⇨ Sales, "Order Transfer - Order Pool" on page C-654

### Stock articles List

The lists show stock articles that correspond to the search criteria. The top list shows all stock articles together. If you select one entry, the articles are shown per storage location in the bottom list. If the checkbox Stock > 0 has been activated, only storage locations with stock of more than 0 are listed.

The following columns are displayed:

- **Articles, Variation:** Article number, name, and color from stock management.
- **Width, Height:** Dimensions from stock management.
- **Content:** Number of sheets in one box.
- **Total stock:** Total stock of the stock article at all storage locations.
- **Min. stock level:** Quantity of the defined minimum stock level.
- **Purch. quantity:** Defined purchasing quantity.

### Storage locations List

- **ID:** Box ID (manual booking or from receipt of goods).
- **Storage location:** Storage location in the order of level 1 through 4.
- **Stock level:** Current stock level at the storage place.
- **Del. ID:** Supplier's box ID (only if it has been entered at goods receipt).

## Stock Management - Prices

**Path:** `Stock management > Stock management > Prices tab`

*(Fig. G-97 Stock management - Prices)*

This tab shows the current prices for a stock article. During updates, orders, purchase orders and stock rebookings are taken into account.

⇨Tutorial, “Prices" on page G-48

> **Prerequisite**
> The average purchase price (average PP) is only calculated and shown if the checkbox Determine purchase price and the option Average PP has been enabled in the company data.
> ⇨ Master Data, "Average PP: The average purchase price will be recalculated in the following cases:" on page B-955

The fields in the lists are described in detail in connection with the Stock Article tab.
⇨ "Stock Management - Stock Articles" on page G-186

### Purchase prices

- **Lowest price:** The lowest price this article has been purchased at.
- **Max. price:** The highest price this article has been purchased at.
- **Last price:** The latest price this article has been purchased at.
- **Stock value:** The current stock prices are shown in this column. They are the result from the respective price and the quantity.

### Calculation of the average price (average PP)

By selecting an option, determine which stock sizes should be taken into account on this list for the calculation. This setting only makes sense for lite with different stock sizes.

- **Only this article:** For the calculation only the displayed article in the selected dimension is taken into account. The PP history of the current article is displayed.
- **All sizes:** For the calculation all dimensions of the displayed glass are taken into account. The PP history of all dimensions of the article is displayed.

The average PP is calculated for each goods receipt, regardless of how it has been booked. Goods issued only reduce the stock. The list is reduced by archiving and auditing.

The first data record shows the opening stock and the original price. Underneath you will find the goods received and issued (minus sign). If goods have been received as a result of a stock P.O., the P.O. number and the P.O. item is furthermore displayed.

The average PP is updated during entering or changing purchase orders. It is determined by taking the total quantity into account.

**Example:**

|               |           |              |           |
| :------------ | :-------- | :----------- | :-------- |
| 100 pieces    | in stock  | each 15.00 € | 1500.00 € |
| 40 pieces     | new booking | each 18.00 € | + 720.00 € |
|               |           | =            | 2200.00 € |

2200.00/140 pcs. = 15.86 €

Automatic surcharges that are listed in the purchase orders, e. g. energy and transportation surcharge, are also included in the calculation.

### Overview (Price History)

The respective average prices are shown as history. This way, you can easily monitor price developments. Details displayed:

- **Date:** Date of the last update.
- **Quantity [QU]:** Quantity issued or received and quantity unit.
- **Price/[PU]:** Purchase price per price unit at the time of booking.
- **Stock on hand [QU]:** Stock on hand at the displayed date. If the average PP is shown for all dimensions, the stock on hand is always shown in sqm.
- **Average price / [PU]:** Average price per price unit at the time of booking.
- **P.O./item.:** Number of the purchase order and P.O. item.
- **Stock value:** Stock value at the displayed date (calculation: purchase price * stock on hand).
- **Type:** Type of booking that has caused the respective entry.

- **Include in total PCH:** You can determine whether the article should be included in the calculation of the total average price of all variations of this article.
  - The article will not be considered for calculating the average price.
  - The article will be included in the calculation.
- **Average price:** Current average price. Depending on the option for calculating the average PPs, the display for the current article or the display for all dimensions of the article applies.

> **Updating the display**
> The display of the average prices is updated for the respective stock article during archiving or auditing (invoice check). As a result, the display remains clearer. A+W Business assumes that the prices will not be changed anymore after these processes. However, if you still change prices after one of the processes, these changes are not included in the calculation of the average price.

## Stock Management - Supplement

**Path:** `Stock management > Stock management > Supplement tab`

*(Fig. G-98 Stock management - table)*

On this tab reservations for a selected stock article are shown.
The fields in the lists are described in detail in connection with the Stock Article tab.
⇨ "Stock Management - Stock Articles" on page G-186

### Reservation

The fields in this area are enabled for individual customers only.

- **Customer:** Number and name of customer for whom the selected stock article is reserved.
- **Fully locked:** Currently not being used.
- **Exclusive reservation:** Currently not being used.

### Supplier

- **Supplier:** Number and name of supplier from whom the stock article is ordered.

### Remark

- **Product related, Storage location related:** You can enter additional information for each stock article and each storage location, e. g. when and from which supplier glass/boxes were supplied, so that older deliveries are used first.

## Stock Movement

**Path:** `Stock management > Stock movement`

You can manually book withdrawals and additions for stock articles, correct stock figures, rebook storage locations and resolve boxes.

This chapter provides information on the following subjects:
- "Options Menu" on page G-195
- "Stock Movement" on page G-195

### Options Menu

**Path:** `Stock management > Stock movement`

The following entries are displayed:
- **Protocol at shut down:** When exiting the dialog, the stock history is automatically shown.
  ⇨ "Stock History" on page G-204
- **Stock > 0:** Only stock articles with a stock on hand of over 0 will be shown.

### Stock Movement Dialog

**Path:** `Stock management > Stock movement`

Additions and dispatches of stock articles are automatically booked: for receipt of goods by delivery and for goods issued by orders. You can manually book additions or dispatches in the Stock Movement dialog, e. g to correct stock quantities.

Dialog Stock Movement offers the following tabs:
- Stock Movement - Dispatch, Addition
- Stock Movement - Transfer
- Stock movement - Number of Sheets
- Stock Movement – Open Boxes

## Stock Movement – Dispatch, Addition

**Path:** `Stock management > Stock movement > Dispatch tab, Addition tab`

*(Fig. G-99 Stock Movement – Dispatch, Addition)*

You can manually book goods issued and received on the Dispatch and Addition tabs. You can select a certain stock article and enter the corresponding data. If you have all stock articles displayed you can select the requested article on the Storage places list. The fields in the Change stock on hand section are then enabled.

⇨ Tutorial, "Withdrawals and Additions" on page G-77

If you have activated the option Protocol at shut down, the stock history is automatically shown on the Table tab when you close the dialog.
⇨ "Stock History – Table" on page G-208

> **Manually enter addition of boxes**
> Since every box is kept with its own ID, you can enter additions of boxes only via Goods Receipt or Stock Management. This process is explained in Box Management section.

### Stock product

- **Product:** Number and name of the stock article.
- **ID no.:** You can only book stock dispatches via the ID no. Additions of boxes must be defined in Stock Management so that you can enter a new ID.
- **Contents:** If you have selected a box, then its content is displayed. If a box with an ID no. that has already been allocated to an order is to be delivered or opened, a message is displayed. This prevents negative stock being created by the subsequent printing of the delivery note or invoice.
- **Storage location:** Storage location that the stock article has been allocated to.
> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.
- **Average purch. price:** The average purchase price is only shown if the function has been activated in the master data.
  ⇨ Master Data, "Calculate purchase price” on page B-955

### Change stock on hand

- **Quantity:** Enter the quantity that is to be booked out or in to stocks in pieces. If you go below the minimum stock when booking articles out of stock, a warning message is displayed.
- **Width / Height:** These fields are only filled with quantity unit sqm if it involves stock sizes.
- **Assessment price:** Enter the purchase price at which the goods received were supplied.
- **Booking date:** The current date is shown automatically. It can be changed if required.
- **Remark:** You can enter a remark or select from the combo box. The remark will be displayed in the stock history.
  ⇨ "Stock History – Table" on page G-208
  Use the button to add a new remark to the list.
  ⇨ "Remark (Stock Movement)" on page G-201

### Storage locations

- **Color:** The color is only shown for variations.
- **Width, Height:** Dimensions are only shown if the product has been defined as a stock size or box.
- **Content:** Value 1 is shown for stock articles and stock sizes and the number of sheets for boxes.
- **Storage location:** Storage location in the order of level 1 through 4.
- **ID no.:** Box ID (manual booking or from goods receipt).
- **Stock on hand:** Current stock
- **QU:** Quantity unit with which the product is kept in stock.
- **Del. ID:** Supplier's box ID.

## Stock Movement – Transfer

**Path:** `Stock management > Stock movement > Transfer tab`

*(Fig. G-100 Stock movement – Transfer)*

Use this tab to book a stock article to a different storage location. When you transfer a storage location, the entire stock of this storage location is always booked to the other storage location.

⇨Tutorial, "How to transfer the storage location" on page G-82

The fields in sections Stock product and Storage locations are described under tab Dispatch.
⇨ "Stock Movement - Dispatch, Addition" on page G-196

### Storage location

- **Storage location:** Displays the current storage place. You can allocate a different storage place. The combo box lists all stored storage places.
> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.

## Stock movement - Number of Sheets

**Path:** `Stock management > Stock movement > No. of sheets tab`

*(Fig. G-101 Stock movement - Number of sheets)*

Use this tab to correct the content of boxes.

⇨ Kistenmanagement, "Kisteninhalt korrigieren (Blattanzahl)" auf Seite K-66

The fields in sections Stock product and Storage locations are described under tab Dispatch.
⇨ "Stock Movement - Dispatch, Addition" on page G-196

### Content change

- **Contents:** The number of sheets that are supposed to be included in a box is only shown if you have selected a box with an ID no. You can correct this entry.

## Stock Movement – Open Boxes

**Path:** `Stock management > Stock movement > Open boxes tab`

*(Fig. G-102 Stock movement – Open boxes)*

Use this tab to resolve boxes so that the individual sheets are available for production. During this process, the box is booked out of the inventory and the number of sheets is booked to the inventory of the stock size.

⇨ Kistenmanagement, "Kisten aufbrechen (auflösen)" auf Seite K-67

> **Book box content to a different storage location**
> When you open a box, its content is booked to the same storage location of where the box is located. If you want to transfer the content, you must book it out of the previous storage location and subsequently, book it to the new storage location.

The fields in sections Stock product and Storage locations are described under tab Dispatch.
⇨ "Stock Movement - Dispatch, Addition" on page G-196

### Open box

If a box with an ID no. that has already been allocated to an order is to be delivered or opened, a message is displayed. This prevents that negative stock is created by the subsequent printing of the delivery note or invoice.

- **No. of boxes:** Number of boxes that are to be opened.
- **Different contents:** The number of sheets is shown only if you have selected a box. You can correct this value.

## Remark (Stock Movement)

**Path:** `Stock management > Stock Movement > [Remark]`

*(Fig. G-103 Remark concerning stock movement)*

Use this dialog to store remarks that are offered for selection in the Stock movement dialog. If you leave the first line blank you can also delete an allocated remark.

## Queries

**Path:** `Stock management > Queries`

Use the different queries to get a quick overview of stock on hand, movements and values in your stock.

This chapter provides information on the following subjects:
- "Booking Journal" on page G-202
- "Stock History" on page G-204
- "Stock Statistics" on page G-209
- "Reserved Stock Products" on page G-215

### Booking Journal

**Path:** `Stock management > Queries > Booking journal`

*(Fig. G-104 Booking Journal)*

In this dialog you can select the criteria for the query. In the booking journal, all automatic order or purchase order processes that relate to the stock are logged, e. g. reservations, purchase orders, additions and dispatches.

⇨ Tutorial, "Show Booking Journal" on page G-87

### Selection

- **Booking type:** You can search the stock for the following booking types:
  - **(No entry):** If you do not enter any booking type, all articles are shown.
  - **Reserved:** Only the reserved articles are shown. An article remains reserved until the delivery note or invoice has been printed.
  - **Delivered:** Only delivered stock articles are shown. An article is marked as delivered after the delivery note or invoice has been printed.
  - **Ordered:** Only ordered stock articles are shown. The indicator is set as a result of a stock P.O.
  - **Received:** Only delivered stock articles are shown. An article is considered delivered or received once it has been booked in goods receipt.
- **Booking date from ... to:** You can restrict the search to a date or time period during which the articles were booked in the stock. When you select the date, pay attention to the time at which the booking was executed. If you have not restricted the display any further, all bookings during the specified time period are displayed.
- **Storing place:** You can restrict the search to a storage place.
> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.
- **ID no.:** You can restrict the search to a box ID.
- **Select by:** Choose an option to define what the search should refer to:
  - **Articles:** You can search for one or several articles. The entry in the fields Number from and to refers to the product numbers. If you have not selected a booking type, all booking types will be listed.
  - **Order:** You can search for articles that are included in orders. The entry in the fields Number from and to refers to the order numbers.
- **Number from, to:** The search can be restricted to one number or a sequence of numbers.

### Table (Booking Journal)

The result of the search is displayed on the list.

- **Res. type:** Booking type in which the product has been booked.
- **Order No./P.O. No.:** Number of the order or purchase order from which the booking has been created.
- **Item No.:** Number of the order or purchase order item.
- **Qty:** Item quantity.
- **Product, Name:** Product number and name as per master data.
- **Color:** The color is only shown for variations.
- **Width, Height:** Dimensions of the item.
- **ID:** Box ID (manual booking or from receipt of goods). If the entry is not a box, a zero is displayed.
- **Del. ID:** Supplier's box ID.
- **Storage location:** Location at which the product has been booked out or in.
- **Booking date:** Date of goods receipt.
- **PP:** Purchasing price of item. Any change of the purchase price at the receipt of goods, check of the delivery OC or invoice is updated in the P.O.

## Stock History

**Path:** `Stock management > Queries > Stock history`

In the stock history, all processes that refer to the stock are logged. In addition to the booking types, this includes e. g. cut stock plates, corrections, new articles.

The Stock history dialog offers the following tabs:
- Stock History – Selection
- Stock History – Table
