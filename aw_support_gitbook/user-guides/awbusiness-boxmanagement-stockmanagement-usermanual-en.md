---
description: "A+W Business Box Management Tutorial and Reference"
---


# A+W Business Box Management Tutorial

This section provides information on the following subjects:
- Overview
- Basic Principles of Stock
- Basic Settings
- Master Data for Boxes
- Orders
- Stock Management for Boxes

---
## Table of Contents

- **Overview** - K-3005
  - Tutorial structure - K-3005
  - Menu overview - K-3006
- **Basic Principles of Stock** - K-3007
  - Stock sizes - K-3008
  - Stock management - K-3009
- **Basic Settings** - K-3011
  - Prices - K-3011
  - Company data - K-3013
  - Status changes due to additions and dispatches - K-3016
  - Stock categories - K-3017
- **Master Data for Boxes** - K-3018
  - Box data - K-3019
    - Define stock sizes for boxes - K-3020
    - Creating stock articles for box - K-3021
  - Box with BOM - K-3024
    - Master data for boxes with BOMs - K-3025
    - BOM box in stock management - K-3030
    - BOM box at item entry - K-3031
- **Orders** - K-3032
  - Sales order with box - K-3033
  - Production orders - K-3037
    - Settings in supplier file - K-3038
    - Enter production order - K-3040
- **Stock Management for Boxes** - K-3044
  - Stock management of boxes - K-3044
  - Stock P.O. of boxes - K-3045
  - Receipt of goods via barcode - K-3050
  - Shipping of boxes - K-3051
    - Withdrawal of boxes - K-3051
    - Booking of issued goods - K-3053
  - Manual stock bookings - K-3056
    - Manual input of addition - K-3056
    - Change storage location of a box - K-3060
    - Correcting the box contents (number of sheets) - K-3061
    - Opening (resolving) boxes - K-3062

## Overview

The box management tutorial discusses the settings for entering and booking boxes containing cut glass.

> **The functions depend on the released modules**
> Please note that the individual functions are available only if the corresponding modules and interfaces have been installed and released.
> If you detect functions in this description which are not available in your version, please contact A+W Software GmbH.

### Sets of Topics

This tutorial includes the following subjects:
- Basic Principles of Stock
- Basic Settings
- Master Data for Boxes
- Orders
- Stock Management for Boxes

### Required knowledge

The tutorial is meant for those who work with boxes in A+W Business. The participants must be familiar with the concept of master data, sales, and purchasing in A+W Business.

### Tutorial structure

The tutorial consists of subjects with several training modules each. Each session consists of the following elements:

- **Overview**: Each training session starts with an overview of the major topics.
- **Concepts**: Concepts and terms of the corresponding training session will be explained first.
- **Instruction**: The instructions are intended as examples to demonstrate the flow. The names they contain are fictitious.

### Menu overview

This chapter provides a brief overview of the program sections that contain the dialogs that are displayed in this documentation.

**(Fig. K-1 Box management menu)**

#### Master data
- **Stock size:** Use this dialog to enter the boxes with different price keys.

#### Stock management
- **Stock management:** Use this dialog to enter and maintain data for stock articles.
- **Stock movement:** Use this dialog to book goods received and issued, changes of stock locations and opening of boxes.
- **Search:** Use this dialog to check the product availability during a certain time period.

#### Production
- **Goods issues boxes:** Use this dialog to enter stock issue of boxes that are assigned to an order.

#### Documents
- **Goods received:** Use this dialog to enter the boxes that should be included in the inventory.

## Basic Principles of Stock

A+W Business's Stock Management module allows you to manage jumbo sizes, stock sizes, residual plates, boxes, all-glass doors, fittings, frame parts and accessories, such as mirror mountings, sealing tape, etc.

A detailed description of stock is in the Stock Management section. The most important points for box management will be summarized only briefly here.

### Stock control

Before you set up your stock in A+W Business, you have to decide on the basis of how your stocks should be managed: as an area (sqm) or in numbers of pieces. A third possibility is the combined stockkeeping, whereby the size-dependent stock mode is combined with the reports from the optimization so that in addition to the stock dimensions, the stock sizes cut can be booked out automatically.

After deciding about the mode, allocate the corresponding stock code per glass product and define the stockkeeping mode in the company data.

### Stock control mode and reservation

When a product with procurement type Stock Withdrawal is entered in a (production) order, the corresponding quantity (plus waste in the case of fixed sizes) of the stock article is marked as reserved. The reservation can optionally either be booked out of the current stock on hand or automatically when the delivery note or invoice is printed.

These settings are shown in the stock quantities display in dialog Stock Info (stock preview) and the automatic purchase order suggestions that can be triggered when minimum quantities are reached.

### Consumption of BOM elements in production orders

For production orders, the consumption of BOM elements in stock can be booked. Boxes then have a BOM if picture frame glass is packed in paper and these paper packages are on a pallet.

> **Example**
> In a production order, LAMI with 2xFloat 3 is entered. After reporting of the production order, the LAMI is booked to the stock, the Float 3 is booked out of the stock.
> If for the same LAMI a normal customer order is entered, only the LAMI is withdrawn from the stock. The Float 3 is not kept in the stock since it has already been withdrawn from the stock by the production order.

### Supplier list

If a box with the identical dimensions is purchased, you must enter the supplier in the supplier list. The supplier is found via the product group that is assigned to the box in the stock dimensions.

### Stock sizes

The stock size Box is mandatory for stock bookings. For entering a box as an order or purchase order item, a stock article/size called Box must therefore have been created.

If you have created a stock size in the master data, A+W Business provides you with the option to immediately switch to stock management.

**(Fig. K-2 Stock sizes (product management) and related stock articles)**

- **A**: Product management – stock sizes (master data)
- **B**: Product number pertaining to the stock sizes
- **C**: Stock sizes with different dimensions
- **D**: Stock articles relating to the stock sizes (stock management)
- **E**: Allocation of price tables
- **F**: Determining the PP in the stock

Each stock size can be allocated to a separate price table.

If you work with the stock code size-related, you must create stock articles for all stock sizes.

### Stock management

Every (glass) product is related to a stock size and a stock article. Each stock article can be created in different variants, e. g. Float 5 mm in several sizes.

**(Fig. K-3 Stock article definition)**

- **A**: Product number
- **B**: Stock article sizes
- **C**: Standard storage location
- **D**: Stock category
- **E**: Main stock article code
- **F**: Inventory audit for the stock preview
- **G**: Defined stock articles
- **H**: Main product
- **I**: Number of sheets in boxes
- **J**: Storage place (4 levels)

In stock sizes (master data), a box can be defined for every product with the procurement type Stock withdrawal, e.g. one box per size.

If there are boxes of the same size but with different numbers of sheets (I), separate stock articles must be defined for them. To define the exact box article, width and height (among others) are analyzed to determine the minimum stock.

A stock article is therefore required for every box variant, specifying the product number, the size, and the number of sheets.

You can link several stock sizes in stock management by defining a main stock product (H). The inventory check in dialog Stock info is executed only for the main stock product in this case; a minimum stock has to be defined only for this article.

If the stock on hand is not checked for each storage location (F), a main product (E, H) must be allocated to determine the available square meters of the glass.

## Basic Settings

In addition to the products and the stock articles, additional setting must be specified so that the boxes can be managed correctly.

This section provides information on the following basic settings:
- "Preise" auf Seite K-3289
- "Firmendaten" auf Seite K-3291
- "Statusänderungen durch Zu- und Abgänge" auf Seite K-3294
- "Lagerkategorien" auf Seite K-3295

### Prices

Via the price lists for boxes, the prices in purchasing and sales are calculated, e.g. also if individual sheets from a box are sold.

If you want to calculate the glass in boxes with other prices, you must create appropriate price lists for sale and purchase. If you also want to use different glass prices depending on the quantity, additional price lists are also required for this.

The prices are described in detail in the Master Data section.

**(Fig. K-4 Example of box prices)**
- **A**: Price keys for boxes
- **B**: Price per price key

In this example, you see that the prices for the glass in a box are calculated differently, e.g. for the whole box or for a single sheet from the box.

The following conditions must be fulfilled to calculate the average purchase price:
- The product has to be defined also as a stock article.
- The PP code must be set in company data.

#### Check price lists

**How to check the master data of your price lists**

1. Go to menu `Master data > Prices` and check the settings in the dialogs `Year`, `Key`, and `Rate`. You only need to check the entries used for the prices (and other internal calculations) for stock sizes and boxes.
2. Select menu `Master data > Prices > Prices`.
   **(Fig. K-5 PP price tables)**
   (See also: Master data, "Prices" on page B-770)
3. Please check if all purchase and sales prices have been defined and are up to date, and complete or correct them as necessary.
4. Go to the tab in which the price is defined, check if the purchase price has been entered correctly, and correct it if necessary.
   **(Fig. K-6 Defined purchase prices)**
5. Go to the menu `Start > Save` to save the changes. The data will be saved.

### Company data

In the company data, the settings for the receipt of boxes and stock receipts are specified through production orders. These settings are described in detail in the Stock management section.

#### Checking settings for boxes

**How to check the settings for the stock**

1. Go to menu `Master data > Company > Company data`.
   (See also: Master data, "Company Data" on page B-942)
2. Switch to the `Parameter` tab and check the settings for the virtual item numbers.
   **(Fig. K-7 Company data – parameters)**
   - **A**: Virtual item numbers for receipt of boxes
   The virtual item number is necessary for booking the receipt of box items with a quantity of > 1 correctly.

3. Go to the `Stock / PCH / EDI` tab.
   There are two ways of entering additions to stock based on production orders:
   - If the status of the work order exceeds the defined status due to a report from production, the addition to stock is booked automatically.
   - If you do not use production reports, you can enter the addition to stock by means of the manual status report in the Production module. If you set the production order there to a status above the aforementioned limit, the stock withdrawal of the material consumed and the addition of produced stock articles to stock are booked automatically.
   If no other storage location has been defined, the order quantity is allocated to the standard storage location.

   **(Fig. K-8 Company data - Stock / PP / EDI)**
   - **A**: Settings for determining the purchase price
   - **B**: Setting to update the stock on hand
   - **C**: Delete ID numbers
   - **D**: Stock bookings for production orders
   - **E**: Number of preview days for dialog Stock Info
   - **F**: Limit status for registration points (for production orders)

4. Select the settings for stock P.O.s (A).
   For the boxes, it is only important how the purchase price should be determined. The settings for determining the purchase price are described in the Master Data section. All other settings in this area are described in detail in the Stock Management section.

5. Select the functions that should be considered when updating the stock on hand in the `Stock Control Mode` (B).
   - **Reservation w/o stock update:** Enable this option if reserved quantities should not be booked out of the current stock. You must then manually carry out the withdrawal booking. The current stock is therefore not shown at order entry.
   - **Reservation with stock update:** This option is enabled by default so that reserved quantities are booked out from the current stock when the delivery note or invoice is printed.
   - **Stock control on BOM level:** Tick this checkbox if products should be managed in the stock even if they are part of a BOM.
   - **Execute stock booking before document printout:** Tick this checkbox if stock articles should be booked out before the document is printed. In the event of a problem with the stock withdrawal booking, the order is removed from the documents to be printed and is therefore not printed.
   - **Delete articles with ID if there is no stock on hand (C):** Boxes with the stock = 0 are no longer present in stock. Enable this checkbox if in the stock management the boxes with the ident numbers from the overview should be deleted for which no inventory is displayed.
   - **Consumption of BOMs in production orders (D):** If you are working with production orders, you can specify whether the consumption of BOM elements is booked out of stock automatically.

6. Enter the number of workdays (E).
   The number of workdays is analyzed for the preview in the `Stock Info` dialog. It specifies the time period for which the future stock on hand will be shown.

7. Go to the menu `Start > Save` to save the changes. The data will be saved. You should restart A+W Business after changing the company data.

> **Status allocation for stock withdrawal booking**
> If you have enabled the option `Execute stock booking before document printout` you should check the status allocation for the stock withdrawal booking. The minimum, assigning and lock status must be organized in a manner that stock withdrawal bookings can be executed prior to printing. If the status allocation does not allow reversal of the order it may be possible that the stock withdrawal booking is not executed.

### Status changes due to additions and dispatches

Goods dispatches and receipts can change the status of documents and result in stock changes due to the status change. If the status points and status allocations are defined correspondingly, this will also apply to partial deliveries.

If you have enabled the option `Execute stock booking before document printout`, the minimum, assigning and lock status must be organized in a manner that stock withdrawal bookings can be executed prior to printing. If the status allocation does not allow reversal of the order it may be possible that the stock withdrawal booking is not executed.

#### Check status allocations

A detailed description of stock sizes can be found in the `Stock Management` section.

**How to check the status management**

1. Go to menu `Master data > Order > Status management`. (See also: Master data, "Status Management" on page B-913)
2. Check whether the user status for stock additions and stock dispatch exists. Create them if necessary.
3. Next, check the status allocations. Select menu `Master Data > Order > Status allocation`. (See also: Master data, "Status Allocation" on page B-915)
4. Check whether the status allocations of stock addition and stock dispatch for document types `Order` and `P.O.` have been defined:
   - **Stock goods dispatch:** Status `Delivery note printed` or `Invoice printed`
   - **Stock goods receipt:** Status `Goods receipt booked`
5. Create missing allocations and correct existing ones if necessary.

### Stock categories

The stock categories are allocated to stock articles in dialog `Stock management`. The stock articles are summed up in groups (stock categories) which can be used as search criteria.

#### Check stock category

**How to define a stock category**

1. Select menu `Master data > Stock > Category`.
   **(Fig. K-9 Stock Categories)**
   (See also: Master data, "Stock Categories" on page B-791)
2. Go to the menu `Start > New` to switch to the input mode.
3. Enter an ID for the stock category, e. g. figures or names, such as raw material, boxes, production, etc.
4. Go to the menu `Start > Save` to save the data. The data will be saved.

## Master Data for Boxes

This chapter contains information about how you create the data in order to differentiate the price calculation for boxes and manage boxes in stock. This includes the definition of the stock sizes and the definition of the stock articles.

This section provides information on the following subjects:
- "Kistendaten" auf Seite K-3297
- "Kiste mit Stückliste" auf Seite K-3302

### Box data

**Objectives**
- Define stock sizes and stock articles for boxes.
- Define products (articles) for boxes.

**Benefit**
- If the products are defined correctly, pieces and surfaces can be calculated and reserved.
- The display of the actual stock on hand including reservations makes purchasing easier.

**Note**
- **Products**: The products defined in master data serve for the input and pricing of documents. They are not automatically kept as stock on hand; this is only the case as a result of additional settings and definitions.
- **Stock article**: All products that are kept in the warehouse with stock quantities must be created as stock articles.
- **Jumbo size**: Glass plate as delivered by the manufacturer. It is used to cut the glass pieces for Sales.
- **Stock plate**: Glass in certain sizes that is actually on hand in the warehouse, e. g. Float 4 mm in 1200 x 1800 mm or 3500 x 5100 mm. Stock plates with defined sizes are also called stock size.
- **Stock size (fixed dimension)**: Stock plates can be processed as a whole (1200 x 1800). However, it is also possible to use them to cut glass pieces, e. g. 600 x 900 from the plate 1200 x 1800 or from the plate 3210 x 5100. Sheets defined as stock sizes are sold without being cut. They have special price tables (stock size tables) allocated. A size-related stock article is always also a stock size.
- **Stock code (stock booking type)**: The stock code defines whether the stock on hand for an article is evaluated as a surface (sqm) or a quantity.
- **Procurement type**: This code defines the standard way of obtaining a product, e. g. by cutting, stock withdrawal, production, purchase order.
- **Default settings**: None

### Define stock sizes for boxes

The stock size `Box` is mandatory for stock bookings. For entering a box as an order or purchase order item, a stock article/size called Box must therefore have been created.

**How to define stock sizes in master data**
1. Select menu `Master data > Product > Products > stock sizes`. The dialog `Stock sizes` opens. (See also: Master data, "Stock Sizes" on page B-707)
2. Go to menu `Start > New` and enter the stock size.
   **(Fig. K-10 Create stock size for pricing)**
   - **A**: Dimensions of the sheets and content of the box
   - **B**: Price tables for sales and purchasing
   - **C**: Pricing in stock
   - **D**: Procurement type
3. If you have already defined a corresponding stock article in stock management, enter the same values for width and height (A).
4. Enter the number of sheets in the box in the `Contents` field.
5. Enter the price code for sales and purchasing (B). You must create an individual stock dimension if you calculate different prices, e.g. for the sale of the entire box, for individual sheets from the box, and/or for the cutting of individual sheets that are removed from the box.
6. Check the checkbox `Search stock PP` (C) if the stock size is to be included in pricing.
7. In addition, you can enter name and short name (matchcode), e.g. for better identification of stock articles.
8. Enter the procurement type (D), e.g. `Stock withdrawal` for stock articles.
9. Go to the menu `Start > Save` to save the data. The data will be saved. Next, the system will want to know whether you want to define this stock size as a stock product as well.
10. Choose [Yes] if the stock size is also to be managed as a stock article. The `Stock management` dialog opens.

### Creating stock articles for box

For a stock article `Box` you have to define at least the following settings in order to manage the stock:
- Article number and name
- Sizes for stock sizes, sizes and contents for boxes
- Storage location and standard storage location (default storage location)
- Inventories

> **Inventory start-up**
> If no stock articles have been entered at all, you can facilitate this task by running the so-called initial inventory. This function is described in the `Stock management` section.

**How to create a stock article**

1. Go to menu `Stock management > Stock management`. The `Stock management` dialog opens. (See also: Software Reference, "Stock management – stock articles" on page G-2611)
2. Go to the menu `Start > New` to switch to the input mode. If you open the `Stock management` dialog from the master data, this step can be omitted. The fields for articles and sizes are filled in already.
   **(Fig. K-11 Fields for new stock articles are enabled)**
   - **A**: Stock article number
   - **B**: Size and content of the box
   - **C**: Storage location
   - **D**: Main product
   - **E**: Stock on hand
   - **F**: Inventory audit
3. Enter the number (A) the size and the content of the box (B).
4. Choose a storage location (C). If no storage location is selected, the storage location `<n.e.>` will be entered. In stock management, this will be treated like the defined storage locations, e. g. for stocktaking purposes and queries. If a stock article is kept in different storage locations, you have to define one of them as the standard storage location.
5. Check checkbox `Default storage location`.
6. Go to field `Main product` (D) and select the article for which you want to enter the minimum stock for the inventory audit. For boxes, this is the stock plate from which the sheets are cut.
7. Check the checkbox `Inventory audit per stock location` (F) if all storage locations shall be evaluated separately when checking the inventory for this stock article.
8. Change to the `Prices` tab and enter the quantity unit with which the average price is calculated.
   **(Fig. K-12 Average price for stock articles)**
   - **A**: Average price
   - **B**: Quantity unit
9. Change to the `Supplement` tab and check whether the supplier 0 is entered for the boxes from production. With this setting, you specify that you yourself are the supplier. This setting has no effect on the boxes that you can alternatively order from a supplier, for such boxes are not kept in stock.
10. Go to the menu `Start > Save` to save the data. The data will be saved.
11. Repeat steps to for all fixed dimensions that can be entered as boxes. For boxes, you specify a stock article per glass, dimension, content, and price key. Thus all necessary information A+W Business needs for reservations and booking have been defined.

### Box with BOM

**Objectives**
- Getting familiar with the product structure of boxes with BOMs (pallets).

**Benefit**
- Boxes with a deeply graduated BOM can be defined and entered as products.

**Note**
- **Product structure**: The article structure of boxes with a BOM is more complex than that of simple glass boxes.
- **Default settings**:
  - Stock management
  - Master data:
    - Product Management
    - Supplier List
  - Company data:
    - Parameters tab
    - Tab Stock/PP/EDI

#### Master data for boxes with BOMs

Boxes with BOM are articles the structure of which is more complex than the glass boxes known so far. Picture frame glass can be wrapped in paper for example, and can then be put onto a pallet.

The pallet is defined as the main product and the paper box with the sheets, as its BOM. Both the pallet and the paper box belong to the product type `Box`.

> **Previous knowledge required for this unit**
> This session is not about working on new dialogs or functions. Boxes with BOMs have a special product structure that is defined by means of the already known tools.
> For information regarding the production BOMs, please see the Master Data section.

**BOM structure**
**(Fig. K-13 Product management – BOM with complex box)**
- **A**: Main product: pallet
- **B**: BOM: box with glass sheets

The illustration shows the BOM structure of such a pallet. You will thus require a product for the pallet, a product for the box and the glass itself.

#### Product type

To make sure that A+W Business interprets the pallet and the box as boxes, product type `200 - Box` must be set for both.
**(Fig. K-14 Product management – Product tab)**

#### Procurement type and stock booking type

To maintain both products on stock, the procurement type must be set to `Stock withdrawal`, and the stock booking type to `size-dependent`.
**(Fig. K-15 Product management – tab Stock/Purchasing)**

> **Define pallet with BOM**
> When you define the pallet and the BOM please make sure that the correct procurement type is adopted.

#### Standard sizes

Product input at item entry becomes a bit easier if a standard width and a standard height are entered for the product. After entering the article number, the matching box article will be automatically selected at item entry in this case.
**(Fig. K-16 Product management – Product tab (optional))**

#### Price code

Unlike for the boxes known already, the codes for Price-relevant SP/PP are analyzed for pricing on main product and BOM level.

So far, the box price used to be calculated and shown only in the box BOM. For boxes with BOMs, this can be configured by means of the Price-relevant codes. Depending on these codes, the sales price is thus determined by the price of the BOM element, the price of the main item, or both.

If in our example, the price of the pallet shall consist only of the total prices of the boxes, i.e. the BOM, the main article's code must be disabled and that of the first BOM component, i.e. of the box, must be enabled.

| Product | Price-relevant | Pricing |
| :--- | :--- | :--- |
| Pallet | Yes | Price per pallet and number of boxes |
| Box | Yes | |
| Pallet | Yes | Price per pallet |
| Box | no | |
| Pallet | No | Price based on the number of boxes |
| Box | Yes |
**Tab. K-1 Pricing in connection with the setting of the 'price-relevant' code**

#### Price management

Price management allows you to enter the box prices as usual.
**(Fig. K-17 Price management – Matrix tab)**

A matrix with the two limit types `Exact width` and `Exact height` can be useful for example. This allows you to define unit prices for the different sizes.

#### Stock sizes (product management)

A stock size must be defined for every pallet and box variant in dialog `Stock sizes`. The variants are the glass sizes. The procurement type must be set to `Stock withdrawal` so that the stock size can be kept on stock.

> **Example**
> The stock size Pallet with boxes shall consist of 80 boxes each, each of which again includes 25 sheets.
> It is essential that for every size, just one stock size is defined with unique contents. This means that you must not enter pallets of 50 and pallets with 80 boxes for the size 600 x 700.

**(Fig. K-18 Product management stock sizes – Pallet of 80 boxes and box of 25 sheets)**

You can define a diversion to other price keys for the stock sizes (as usual).

When the new stock size is saved, you can directly switch from the query to stock management to define the related stock articles.

### BOM box in stock management

Stock articles are defined in the same way as product stock sizes. The article is entered with the same sizes and contents. Additionally, the current stock on hand and the storage location are defined.

For the automatic creation of stock P.O.s, you also have to fill in the fields `Minimum stock` and `P.O. quantity`.

**(Fig. K-19 Stock management - Pallets of 80 boxes, box of 25 sheets)**

### BOM box at item entry

If you enter the pallet in an item, first enter the article number as usual:
- If the standard width and height have been defined in product master data, the box will be automatically created from the product stock sizes.
- To enter the product with other sizes or if no standard size has been defined, use stock search to select the required pallet.

On the `BOM` tab, the components are preset with the corresponding contents.

**(Fig. K-20 Document management - tab BOM: Pallet)**
- **A**: Number of boxes on the pallet
- **B**: Number of sheets per box

The box and its BOM can be entered like any other product. If kept as a stock article, it can also be used to replenish the stock on hand by means of production orders.

**Additional information**
- Sales, "Order header" on page C-1155
- Sales, "Change P.O. code" on page C-1432

## Orders

Orders for boxes come in two forms:
- **Sales order for a customer:** If in addition to the boxes produced, you also sell boxes ordered, the settings for the suppliers must also be specified on the Supplier tab.
- **Production order to fill up stock.**

This section provides information on the following subjects:
- "Verkaufsauftrag mit Kiste" auf Seite K-3311
- "Produktionsaufträge" auf Seite K-3315

### Sales order with box

In a sales order, you enter a box for a customer. This box can be removed from your stock on hand or ordered from a supplier.

**How to enter a box as an order item**

1. Go to menu `Documents > Order` and enter the order header.
   **(Fig. K-21 Order header for sales order)**
   - **A**: Order area
   - **B**: Order type
   Pay attention to the settings for the order area and the order type.
2. Save the data and change to the `Items` tab. Item entry opens.
3. Go to the menu `Start > New` to enter a new item.
4. Enter the product number of the glass for which you want to enter an entire box.
   **(Fig. K-22 Enter product number of the glass in the box)**
5. Go to the menu `Start > Stock search` to open the dialog `Stock info`.
   **(Fig. K-23 Stock information on boxes)**
   - **A**: Product number of the glass
   - **B**: Box (without inventory)
   The `Stock info` dialog shows a list of all boxes and stock sizes available for this product number. Boxes with the storage location `<n.e.>-<n.e.>-<n.e.>` are boxes that are created as stock articles. Boxes with inventory generally have an ID.
6. Adopt the marked box with a double-click. Pay attention to the specified dimensions if you are working with different boxes for a product.
7. The dialog is closed and you will find yourself back at item entry.
   **(Fig. K-24 Item with box entered)**
   - **A**: Procurement type
8. Select the procurement type (A).
   - **Stock withdrawal:** The box will be withdrawn from stock.
   - **Order (complete):** The box will be ordered from the supplier who is entered on the Supplier tab. For this setting, the order must then be transferred to purchasing.
9. If necessary, correct the quantity if you want to enter more than one box.
10. Go to the menu `Start > Save` to save the data. The data will be saved. You can now enter additional items and complete the order as usual.

If you book the goods receipt of the box delivery by a supplier, the boxes delivered will be assigned to the order. There is a detailed description in the Purchasing section.

### Production orders

Work orders are used to replenish the stock on hand. All articles entered in such an order are automatically changed to procurement type `Production`. Unlike customer orders, the items are not reserved on stock but are marked as ordered.

#### Manual and automatic stock P.O.

**(Fig. K-25 Stock P.O. vs. Production order)**
This flow chart shows A+W Business's reactions to different presettings in the supplier file. The program checks whether the current stock on hand plus the already ordered quantities and minus the reserved quantities will fall below the minimum stock on hand. If this is the case, the P.O. proposal shows the multiple of the (standard) P.O. quantity.

#### Settings in supplier file

If a minimum stock and a (standard) order quantity have been defined for the stock article in dialog `Stock management`, the system can create automatic P.O. proposals. These are listed in dialog `Stock P.O.`

This is how purchase orders of the type `Stock P.O.` are usually created. However, if an internal customer is entered in the supplier file instead of a standard supplier, work orders can be created automatically.

**(Fig. K-26 Internal customer for work orders)**

In the supplier file, an internal customer is defined for which the work order is entered automatically. The option `Internal customer` can be enabled on product group or product level. The product settings have priority over the product group settings.

#### Purchase order quantity

The multiplier will be calculated so that as a result of the P.O. proposal the minimum stock is exceeded.

**(Fig. K-27 Quantities for stock articles (dialog Stock management))**

> **Example**
>
> Laminated glass with article number 107 is kept as a stock article.
>
> - Current stock on hand: 10 pcs.
> - Minimum stock: 30 pcs.
> - P.O. quantity: 5 pcs.
>
> The P.O. quantity for laminated glass 107 is calculated as follows:
> Difference between current stock on hand and minimum stock on hand: 20 pcs. This difference includes the P.O. quantity of 5 pcs. four times.
>
> P.O. quantity: 4 x 5 = 20 pcs.
>
> Current stock on hand plus ordered quantity: 10 + 20 = 30 pcs.

The calculated quantity is adopted for the P.O. proposal. It can be amended in the `Stock P.O.` dialog. How you edit and transfer is described in the `Purchasing` section.

The production order is created by the transfer, in the last active order `Number Manager`. The work order can be edited and transferred to production.

### Enter production order

If you enter production orders manually, you can enter a previously entered order by copying it and transferring it to production.

> **Labels for receipt of goods**
> In order to enter a self-produced box in receipt of goods via PDC, a label/barcode is required. For this, the print item 973 must be assigned.

This section provides information on the following action sequences:
- "Entering header data for a production order" on page K-3040
- "How to enter the glass for the box" on page K-3042
- "How to enter a production order by copying" on page K-3043

**Entering header data for a production order**

1. Select `Documents > Order > Order`. The dialog `Document management` opens. In this description it is the `Edit` mode.
2. Go to the menu `Functions > Document > Select NM` and check if the correct number manager has been set, and correct the setting if necessary. The allocation of the order to a number manager is also shown in the order header.
3. Go to the menu `Start > New` to switch to the input mode.
4. Enter the required header data.
   **(Fig. K-28 Header data for production order)**
   - **A**: Order area
   - **B**: Production order
5. If necessary, enter an explanation for the order in the fields under the name; for example, that the sheets should be packed in boxes.
6. Choose the order type (B) `Production order`.
7. Check the other details.
8. Go to the menu `Start > Save` to save the data. The header data will be saved. Now you can go to the `Items` tab and enter the order items. The `Items` tab will be locked again if you change data in the order header. You have to save the changes to enable the `Items` tab again.

**How to enter the glass for the box**

1. Select `Documents > Order > Select order > Items tab` or `<F9>`. Item entry opens.
2. Go to the menu `Start > New` to enter a new item.
3. Enter the product number of the glass that should be produced as box.
   **(Fig. K-29 Enter product number of the glass in the box)**
4. Set the quantity to the content of the box or a multiple of the content.
5. Select in the menu `Start > Save` to save the data. The data will be saved. It is transferred to production.

If you enter work orders on a regular basis, you can copy the previously entered order to make this task easier. For a detailed description, please see the chapter Sales chapter.
- Before copying, you have to set the document type of the target document to `Production Order`.
- If only certain items shall be adopted from the order, you can select them.
- You can amend the data in the new document.

**How to enter a production order by copying**

1. Select `Documents > Order > Select Order`. The order entry opens.
2. Select menu `Functions > Copy documents`.
   **(Fig. K-30 Create production order by copying)**
   - **A**: Copy from order to order
   - **B**: Document type of the target order
3. Change to the `Copy by item` tab and mark the item(s) that should be copied.
4. Correct the target quantity if necessary.
5. To generate the copy, go to the menu `Start > Execute`.

## Stock Management for Boxes

For stock articles, both the goods receipt as well as the goods removal are entered so that you can manage inventories.

The receipt and withdrawal of boxes can be entered using barcodes (PDC) or manually.

This section provides information on the following subjects:
- "Stock management of boxes" on page K-3044
- "Stock P.O. of boxes" on page K-3045
- "Receipt of goods via barcode" on page K-3050
- "Shipping of boxes" on page K-3051
- "Manual stock bookings" on page K-3056

### Scanning

In connection with `AWPort`, stock bookings can also be entered via barcode. This does not only include receipt and withdrawal of goods but also opening of boxes and other reallocation actions.

By scanning, entire boxes can be allocated to a certain order or order item, or can be registered for the inventory including the sheets it contains.
(See also: "Receipt of goods via barcode" on page K-3050)

For more information on barcodes and barcode formats, please refer to the documentation on `AWPort`.

### Stock management of boxes

Delivered boxes generally have an ID from the supplier with which they are entered when received.

Every box is booked with its own box ID by which it is kept on stock. The checkbox for assigning virtual item numbers must be checked in the company data.
- "Company data" on page K-3013
- "Receipt of goods via barcode" on page K-3050

#### Open boxes

To register individual sheets of a box you have to open the box. First, a box (with ID) is removed from the stock on hand. The number of sheets is then added to the stock on hand for the corresponding stock article (stock size).

### Stock P.O. of boxes

The inventory of boxes can either be filled up with an automatically or manually generated production order.

Stock P.O.s can also be created manually, via document management.
(See also: "How to enter a stock P.O. with boxes" on page K-3047)

#### P.O. proposals

Purchase orders are usually created through stock management in order to keep the stock on hand on the required level.

**(Fig. K-31 Stock management - Stock on hand figures)**
- **A**: Minimum stock
- **B**: Quantity for P.O. proposal

If you have defined minimum quantities (A) for a stock article in dialog `Stock management`, P.O. proposals are created automatically with the stored P.O. quantity (B). You can check these before they are transferred to Purchasing, and change the supplier and date if necessary. Transfer to Purchasing turns the proposal into a stock P.O.

### Stock addition based on production order

On tab `Stock / PP / EDI` in company data, set the limit status for registration points to define from which point on an order counts as produced. The limit status is the status defined for the selected registration point.

**(Fig. K-32 Company data – Stock / PP / EDI: Registration point for status change)**

There are two ways of entering additions to stock based on production orders:
- If the status of the work order exceeds the defined status due to a report from production, the addition to stock is booked automatically.
- If you do not use production reports, you can enter the addition to stock by means of the manual status report in the Production module. If you set the production order there to a status above the aforementioned limit, the stock withdrawal of the material consumed and the addition of produced stock articles to stock are booked automatically.

If no other storage location has been defined, the order quantity is allocated to the standard storage location.

The booking of work orders is described in detail in section Production.

**Additional information**
- Master data, "Company Data - Stock/Purchasing/EDI" on page B-981
- Sales, "Order header" on page C-1155
- Sales, "Change P.O. code" on page C-1432
- Production, “Production orders" on page E-2199

### Entering manual stock P.O. of boxes

The following guideline shows how to enter a stock P.O. for boxes. Manual P.O.s are described in detail in the Purchasing section. (See also: Purchasing, "Manual purchase order" on page D-1900)

**How to enter a stock P.O. with boxes**

1. Go to the menu `Documents > P.O. > P.O.`. The dialog `Document management` opens.
2. Go to field `Type` and select the entry `Stock P.O.` If you set the type to `<n.s.>`, goods received cannot be automatically added to stock.
3. Go to the `Items` tab.
4. Enter the product number. You can specify the number after selecting the stock article. You do not need to enter sizes as they are taken from the stock article.
5. Go to the menu `Start > Stock search` to open the `Stock info` dialog. You can also open this dialog by pressing `<F3>`.
   **(Fig. K-33 Stock info - stock search)**
   - **A**: Product number of glass type
   - **B**: Box (without ID)
   (See also: Sales, "Stock info" on page C-1825)
   The `Stock info` dialog opens providing a list of all boxes and stock sizes. For boxes, the entry in column `Cont.` is greater than 1.
6. Select the required box without box ID and accept it by a double click. The dialog is closed and you will find yourself back at item entry. In the input line, you will find that all fields from `Quantity` onwards are locked for boxes. The price fields are updated.
7. Enter the amount required. The display of details is updated.
   **(Fig. K-34 Box at item entry)**
   - **A**: Quantity
   - **B**: Quantity
8. Repeat steps 4 to 7 to enter all P.O. items.
9. Go to the menu `Start > Save` to save the data. The data will be saved.
10. Print and send the purchase order.

### Receipt of goods via barcode

In general, all stock bookings are entered via PDC (plant data collection). For this, the boxes must each have their own barcode label.

> **Labels for receipt of goods**
> In order to enter a self-produced box in receipt of goods via PDC, a label/barcode is required. For this, the print item 973 must be assigned.

**How to enter a box via barcode**

1. Go to the menu `Documents > P.O.> Receipt of goods > Receipt of goods`.
2. Select the `Scanner` option and scan the box's label.
3. Go to menu `Start > Execute`. If you have a barcode for the receipt booking, you can scan it. This way, the box is included in the inventory in the default stock location. You can scan and then book all produced boxes one after another.
4. Change to the `Item-by-item` tab and check the `Book complete` checkbox for the box.
   **(Fig. K-35 Booking item by item)**
5. Go to menu `Start > Execute`. Thus the box is booked and present in the inventory.

### Shipping of boxes

Boxes are usually withdrawn from stock when the delivery note is printed. Printing of the invoice can also be used as a trigger for the withdrawal.

#### Withdrawal of boxes

Boxes are usually withdrawn from stock when the delivery note is printed. Printing of the invoice can also be used as a trigger for the withdrawal.

As the person who enters the order will not know which box is actually going to be shipped, he first enters a dummy box with the required sizes. The stock on hand can only be updated after the ID of the real box is entered and withdrawn from stock.

> **Example**
> A dummy box (without ID) with the required sizes is entered in the order. 3 is specified as the quantity. This reserves three of the dummy boxes.

| Withdrawal | Before printing the delivery note | After printing the delivery note |
| :--- | :--- | :--- |
| **Actions** | - The real box IDs are scanned in the issuing area. <br> - Reservation of the dummy box is canceled. <br> - The three boxes with IDs are marked as reserved. <br> - The delivery note is printed. Three boxes are booked upon issue of goods. | - The delivery note is printed. <br> - The reserved dummy boxes will be withdrawn. <br> - When the boxes are issued, the three real box IDs are scanned. <br> - Reservation of the dummy boxes is canceled. <br> - The three boxes are withdrawn. |
**Tab. K-2 Withdrawal of boxes before or after printing the delivery note**

The following steps have usually been taken already:
- The product was entered in the customer order.
- [F1] in the `Stock info` dialog was used to select the dummy box.
  **(Fig. K-38 Selection of the dummy box)**
- The box was added to the order and saved, e.g with an item quantity of 3.
  **(Fig. K-39 Item quantity 3 saved)**
- 3 additional reservations were booked for the dummy box on stock.
  **(Fig. K-40 Reservation)**
- The booking journal (stock management) shows the item quantity as reserved.
  **(Fig. K-41 Order item reserved)**

Next, boxes with IDs are allocated and withdrawn after printing the delivery note.

### Booking of issued goods

**How to book the issue of boxes**

1. Go to the menu `Production > Dispatch > Issue of boxes`.
2. Select the option `By scanner`.
   **(Fig. K-42 Issue of boxes - load customer order)**
3. Enter the barcode of the order number and item number. The numbers appear in the `Document` fields. If you are not using a scanner, choose the option `By order number` and enter the number.
4. To import order data, select `Start > Execute`. The display switches to the `ID` tab.
5. Each box is shown in a separate line as a virtual item. The fields in column `ID` are empty as no box with an ID has been allocated.
   **(Fig. K-43 Order item with sub-items)**
6. Scan the box ID of the first box to be reserved. If you do not use a scanner, go to field `ID` and select one of the displayed IDs. The list only shows box IDs of the defined type.
7. To allocate the boxes, go to the menu `Start > Execute`.
8. Repeat steps 5 and 6 to allocate more boxes with IDs.

**Additional Information**
- Master data, "Company Data - Parameters" on page B-958
- Master data, "Due date calculation for February (28 or 29 days)" on page B-965
- Sales, "Stock info" on page C-1825
- Software Reference, “Issue of Goods" on page E-2301

### Manual stock bookings

If you are not working with PDC, you also start all stock bookings manually.

This section provides information on the following subjects:
- "Zugang manuell erfassen" auf Seite K-3334
- "Lagerort einer Kiste ändern" auf Seite K-3338
- "Kisteninhalt korrigieren (Blattanzahl)" auf Seite K-3339
- "Kisten aufbrechen (auflösen)" auf Seite K-3340

#### Manual input of addition

You can receive boxes manually into inventory or withdraw them from inventory.

> **Prerequisite**
> The checkbox for the virtual assignment of item numbers must be checked in company data.
> (See also: "Company data" on page K-3013)

There are the following instructions for this session:
- "How to set the ID for boxes" on page K-3056
- "How to create a new box in inventory" on page K-3056
- "How to book the dispatch of goods manually" on page K-3058

**How to set the ID for boxes**

1. Go to the menu `Documents > P.O. > Receipt of goods > Receipt of goods`.
2. Go to the menu `Options > Group ID number allocation > Settings`.
3. Replace the sequence of letters with the desired ID. Please avoid overwriting the placeholders for the numbers.
4. Click on [OK] to save the changes.

**How to create a new box in inventory**

1. Go to menu `Stock management > stock management`. The `Stock management` dialog is displayed.
2. From the menu, select `Options > Assign ID number automatically`. This way, the automatic ID is assigned for boxes with the new ID. Counting begins with each new ID at 1 and is incremented by 1 each time. The `Ident` field on the `Stock article` tab is locked.
3. In the `Article` field, enter the product number of the glass for which a box should be booked.
4. Go to menu `Start > Search`.
   **(Fig. K-44 Box data)**
   - **A**: Storage location
   - **B**: Stock on hand
   - **C**: Box
   - **D**: Stock article without ID
5. Mark the box (C, D) for which you want to enter the stock on hand. Thus, all required data will be taken over and you can create a new box in the stock on hand.
6. Go to the menu `Start > New`. The fields will be enabled.
7. Select the storage location (A) where the new box is located.
8. Enter the number 1 in the `Stock on hand` field. Since each box should have its own ident number, you may only enter 1.
9. Go to the menu `Start > Save` to save the data. In the field for the stock on hand, a new box is displayed with an ID.
10. Repeat steps 6 and 9 until you have included all boxes in the stock on hand. Pay attention here whether all boxes should be booked to the same storage location. You don't need to change any other values until you have booked all boxes.

**How to book the dispatch of goods manually**

1. Go to menu `Stock management > Stock movement >` tab `Dispatch`.
2. Enter the either the product number or the ident number of the box and select `Start > Search` in the menu. The search will be restricted to this box in that case. Alternatively, you can restrict the search to a product code and the storage place. Section `Storage locations` lists all stock articles matching the search criterion.
   **(Fig. K-45 Manual stock dispatch of boxes)**
3. Mark the box that you want to withdraw.
4. Enter a 1 in the `Quantity` field in order to reduce the stock on hand by the marked box.
5. If necessary, change the booking date and enter a note.
6. Go to the menu `Start > Save` to save the changes. Data will be saved, and the stock on hand set to 0.

### Change storage location of a box

This module will show you how to move a box from one storage location to another. This movement will be entered with a rebooking. This way, the stock article will be booked from the old storage location as a withdrawal and as an addition to the new one.

**How to transfer the storage location**

1. Go to menu `Stock management > Stock movements`. Dialog `Stock movement` opens. (See also: Software Reference, "Stock movement" on page G-2620)
2. Go to tab `Transfer`.
3. Enter the product number in the `Product` field or the (box) ID.
4. To start the search, go to the menu `Start > Search`.
   **(Fig. K-46 Stock movement - transfer)**
   - **A**: Current storage location
   - **B**: Select new storage location
5. Mark the box that you want to transfer to another storage location.
6. Choose the new storage location in section `storage location` (B).
7. Go to the menu `Start > Save` to save the changes. The box is withdrawn from the old storage location, and added to the new one. If you have activated the `Log when finished` option, the `Stock history` dialog opens. All stock movements can then be printed in a log.

### Correcting the box contents (number of sheets)

If you find out in the warehouse that the content of a box does not match the quantity shown on the delivery note, the number of sheets needs correcting. This module will show you how to correct the contents of a box.

> **Only boxes with ID**
> The content of a box can be changed only if the box has been entered with its own box ID.

**How to correct the number of sheets in a box**

1. Go to menu `Stock management > Stock movements`. Dialog `Stock movement` opens.
2. Go to tab `No. of sheets`.
3. Enter the product number in the `Product` field or the box ID.
4. To start the search, go to the menu `Start > Search`.
   **(Fig. K-47 Correct the number of sheets)**
   - **A**: Box
   - **B**: Number of sheets
5. Select the required box (A). Field `Contents` is enabled.
6. Enter the new number of sheets (B).
7. Go to the menu `Start > Save` to save the changes. The data will be saved.

### Opening (resolving) boxes

You can open boxes in order to make the sheets available for production or enter them individually in the order. You can only open boxes with an ID.

> **Stock articles with sheet dimensions must be created**
> If you break up a box, the sheets are booked to the stock on hand. The stock sizes for the sheets are created automatically if necessary. In this case, the sheets are booked to the storage location of the opened box.

**How to open a box**

1. Go to menu `Stock management > Stock movements`. Dialog `Stock movement` opens.
2. Go to tab `Open boxes`.
3. Enter the product number in the `Product` field or the box ID.
4. To start the search, go to the menu `Start > Search`.
   **(Fig. K-48 Stock movement – Open box)**
   - **A**: Box shall be opened
   - **B**: Contents
   - **C**: Number of boxes
5. Select the required box. The fields `Number of boxes` (C) and `Different contents` (B) are enabled.
6. Enter 1 in field `Number of boxes` and check if the contents of the box are correct. If necessary, correct the entry in field `Different contents`.
7. Go to the menu `Start > Save` to save the changes. The box will be booked out and the lite as stock articles.
8. If necessary, update the view of storage locations by reloading them.
9. If necessary, delete the empty box from the stock on hand manually.

---

# A+W Business Box Management Software Reference

This section provides information on the following subjects:
- Overview
- Stock management
- Stock Movement
- Search
- Order pool
- Receipt and Shipping of Boxes

## Table of Contents

- **Overview** - K-3067
- **Stock management** - K-3068
  - Menus in stock management - K-3068
    - Functions menu - K-3068
    - Options Menu - K-3069
  - Stock management - K-3069
    - Stock management - stock articles - K-3070
    - Stock management - prices - K-3074
    - Stock management - supplement - K-3077
- **Stock Movement** - K-3078
  - Options menu - K-3078
  - Stock Movement - K-3078
    - Stock movement - dispatch, addition - K-3079
    - Stock movement - transfer - K-3081
    - Stock movement - number of Sheets - K-3081
    - Stock movement - open boxes - K-3082
  - Remark (stock movement) - K-3082
- **Search** - K-3083
  - Stock search - stock search - K-3084
  - Stock search - future stock on hand - K-3087
- **Order pool** - K-3088
  - Order pool menus - K-3088
    - Functions Menu - K-3088
    - Options menu - K-3089
  - Order pool - K-3091
- **Receipt and Shipping of Boxes** - K-3094
  - Receipt of goods (boxes) - K-3094
    - Receipt of goods - selection - K-3095
    - Receipt of goods -complete - K-3096
    - Receipt of goods - by item - K-3098
    - Receipt of goods - ID numbers - K-3101
    - Receipt of goods - protocol (ID numbers) - K-3103
  - Settings (ID) - K-3104
  - Shipping of boxes - K-3105

## Overview

Use the module `Stock Management` to maintain and analyze all data concerning stock. Furthermore, use this module to carry out the inventory and book stock movements.

The Software Reference provides information on the following subjects:
- "Stock management" on page K-3068
- "Stock Movement" on page K-3078
- "Search" on page K-3083
- "Order pool" on page K-3088
- "Receipt and Shipping of Boxes" on page K-3094

## Stock management

**Path:** `Stock management > Stock management`

Use the dialog `Stock management` to display all the stock articles that are managed.

This section provides information on the following subjects:
- "Menus in stock management" on page K-3250
- "Stock management" on page K-3251

### Menus in stock management

**Path:** `Stock management > Stock management`

The menus can be used to define the standard settings of the dialog or open other dialogs without closing this dialog.

This section provides information on the following subjects:
- "Functions menu" on page K-3250
- "Options Menu" on page K-3251

#### Functions menu

**Path:** `Stock management > Stock management > Functions menu`

This menu allows you to open other dialogs without closing stock management.

The following entries are displayed:
- **Stock History:** Opens the dialog `Stock History` with the log of processes that have been booked in stock management.
- **Booking Journal:** Opens the dialog `Booking Journal` with the log of stock bookings from orders and purchase orders.

#### Options Menu

**Path:** `Stock management > Stock management > Options menu`

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

The following entries are displayed:
- **Do not print articles with stock on hand = 0:** Only articles with stock on hand that is more than 0 will be printed. This setting is helpful if you have many boxes with an ID, but without stock. Usually, these have been delivered as boxes and were deleted from the stock. This setting applies only to printing; the dialog shows all the articles.
- **Automatic ID allocation:** The box ID can be allocated automatically even it has been booked as stock manually.

### Stock management (Dialog)

**Path:** `Stock management > Stock management`

In the `Stock Management` dialog you enter all the stock articles that are kept in the warehouse with stock on hand.

Stock sizes are maintained in A+W Business even in product management. They are used to allocate price codes, product groups, etc.

Dialog `Stock Management` offers the following tabs:
- Stock management – stock articles
- Stock management – prices
- Stock management – supplement

> **Stock management at the level of bills of material**
> In the warehouse, you can also manage products that are included as bill of material components in other products. For this purpose, the checkbox `Stock keeping at BOM level` must be enabled in the company data.
> (See also: Master data, "Stock control on BOM level" on page B-984)

### Stock management – stock articles tab

**Path:** `Stock management > Stock management > Stock articles tab`

**(Fig. K-49 Stock management - stock articles)**

Use this tab to check the articles that are managed in the warehouse. The shown stock is updated with each stock booking. You can add new articles and correct the different quantities.

For ordering purposes, you furthermore define minimum quantities and purchase order quantities.
(See also: Tutorial, "How to create a stock article" on page K-3021)

#### Articles
- **Article**: Product number according to master data. If you want to enter a new stock article, you have to enter it in the master data first.
- **Stock ID**: Identification number, assigned on receipt of goods.
- **Name**: Product names from the master data.
- **Width x height / content**: Dimensions of the stock article in mm (only stock sizes) and content of box. For boxes, enter the number of sheets per box. For all other stock articles, a 1 is automatically shown.
- **Variant**: If variations have been entered for an article, you will see the color here.
- **Default storage location**: If you have defined storage locations, they will be offered for selection. If you keep one stock article at several storage locations, you can define a standard storage location.
  - The shown storage location is not defined as standard for the stock article.
  - The shown storage location is defined as standard for the stock article.
  (See also: Master data, "Stock Definition" on page B-789)

> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations `<n.e.>` will remain and can be booked.

- **ID**: The box ID, is assigned on receipt of goods or manually. The ID is only shown if you have selected a box in the overview of stock articles.

#### Details
- **Category**: If you have defined stock categories in the master data, you can use this field as a search criterion. When you enter new stock articles you can allocate a category.
- **Del. ID**: The supplier's box ID is only shown if you have selected a box in the Stock articles section.
- **Main product**: You can link stock articles with several dimensions by specifying a main product. The stock check (for the stock preview in the `Stock info` dialog) is then only executed for the main product and you only need to enter minimum stock for this main product. If you have also defined minimum stock for the allocated stock articles, they will be ignored for the check. (See also: Tutorial, "Stock management" on page K-3009)
- **Prod. batch / date**: Not currently used.
- **Date**: Date at which the stock article has been changed last time.
- **In production**: In connection with A+W Production you can determine whether the stock article has been allocated to production.
  - The stock article is disposable.
  - The stock article has been allocated to production (info only).

#### Inventories
- **Stock on hand**: Displays the current stock. The stock is updated with each booking of outgoing or incoming stock. For boxes with an ID, stock 1 is always shown. If you have created the stock article new, the field is enabled and you can enter the opening stock.
- **Stock > 0**: This checkbox is only available in the selection mode. Use it to define as a search criterion whether articles should be shown without stock quantity.
  - The search result also shows articles, the current stock of which is 0.
  - The search result only shows articles, the current stock of which is at least 1.
- **Min. stock**: The minimum stock forms the basis for automatic purchase order suggestions. They are created if stock falls below the minimum stock. Reservations and purchase orders are taken into account. You can check these automatic purchase order suggestions in the dialog `Order pool`. (See also: "Order pool" on page K-3088)
- **Minimum stock level > 0**: This checkbox is only available in the selection mode. You can use it to define as a search criterion whether the minimum stock must be more than 0.
  - The search result shows all articles.
  - The search result only shows articles, the minimum stock of which is more than zero.
- **Purch. qty.**: This value specifies which quantity is ordered by default. This value is adopted for automatic stock ordering.
- **Inventory < Min. inventory**: This checkbox is only available in the selection mode. You can use it to define as a search criterion whether the minimum stock must be below the minimum inventory.
  - The search result shows all articles.
  - The search result only shows articles, the current stock of which is less than the minimum inventory.
- **Maximum stock level**: By entering maximum quantities per stock article you can prevent the warehouse becoming overstocked. The entered value is only used for the manual check.
- **Target quantity**: Not currently used.
- **Inventory audit per stock location**: If you maintain stock per storage location you can check the stock per stock location.
  - Stock is checked jointly for all storage locations.
  - Stock is checked per storage location.

#### Stock article
The lists show stock articles that correspond to the search criteria. The top list shows all stock articles together. If you select one entry, the articles are shown per storage location in the bottom list. If the checkbox `Stock > 0` has been activated, only storage locations with stock of more than 0 are listed.

The following columns are displayed:
- **Articles, Quantity unit - Variation:** Article number, name, quantity unit and color from stock management.
- **Width, Height:** Dimensions from stock management.
- **Content:** Number of sheets in one box.
- **Total stock:** Total stock of the stock article at all storage locations.
- **Min. stock level:** Quantity of the defined minimum stock level.
- **Purch. quantity:** Defined purchasing quantity.

#### Storage locations
- **ID:** Box ID (manual booking or from receipt of goods).
- **Storage location:** Storage location in the order of level 1 through 4.
- **Stock level:** Current stock level at the storage place.
- **Del. ID:** Supplier's box ID (only if it has been entered at goods receipt).

### Stock management – prices tab

**Path:** `Stock management > Stock management > Prices tab`

**(Fig. K-50 Stock management – prices)**

This tab shows the current prices for a stock article. During updates, orders, purchase orders and stock rebookings are taken into account.

> **Prerequisite**
> The average purchase price (average PP) is only calculated and shown if the checkbox `Determine average purchase price` has been enabled in the company data.
> (See also: Master data, "Average PP: The average purchase price will be recalculated in the following cases:" on page B-981)

The fields in the lists are described in detail in connection with the Stock Article tab. (See also: "Stock management – stock articles" on page K-3070)

#### Purchase prices
- **Lowest price**: The lowest price this article has been purchased at.
- **Max. price**: The highest price this article has been purchased at.
- **Last price**: The latest price this article has been purchased at.
- **Stock value**: The current stock prices are shown in this column. They are the result from the respective price and the quantity.

#### Calculation of the average price (average PP)
By selecting an option, determine which stock sizes should be taken into account on this list for the calculation. This setting only makes sense for lite with different stock sizes.
- **Only this article:** For the calculation only the displayed article in the selected size is taken into account. The PP history of the current article is displayed.
- **All sizes:** For the calculation all dimensions of the displayed glass are taken into account. The PP history of all dimensions of the article is displayed.

The average PP is calculated for each goods receipt, regardless of how it has been booked. Goods issued only reduce the stock. The list is reduced by archiving and auditing.

The first data record shows the opening stock and the original price. Underneath you will find the goods received and issued (minus sign). If goods have been received as a result of a stock P.O., the P.O. number and the P.O. item is furthermore displayed.

The average PP is updated during entering or changing purchase orders. It is determined by taking the total quantity into account.

> **Example:**
> 100 pieces in stock each 15.00 € = 1500.00 €
> 40 pieces new booking each 18.00 € = + 720.00 €
> ---
> **Total:** 2200.00 €
>
> 2200.00/140 pcs. = 15.86 €

Automatic surcharges that are listed in the purchase orders, e. g. energy and transportation surcharge, are also included in the calculation.

#### Overview
The respective average prices are shown as history. This way, you can easily monitor price developments. Details displayed:
- **Date:** Date of the last update.
- **Quantity [QU]:** Quantity issued or received and quantity unit.
- **Price/PU:** Purchase price per price unit at the time of booking.
- **Stock on hand [QU]:** Stock on hand at the displayed date. If the average PP is shown for all dimensions, the stock on hand is always shown in sqm.
- **Average price / PU:** Average price per price unit at the time of booking.
- **P.O. / item.:** Number of the purchase order and P.O. item.
- **Stock value:** Stock value at the displayed date (calculation: purchase price * stock on hand).
- **Type:** Type of booking that has caused the respective entry.

- **Include in total PCH**: You can determine whether the article should be included in the calculation of the total average price of all variations of this article.
  - The article will not be considered for calculating the average price.
  - The article will be included in the calculation.
- **Average price**: Current average price. Depending on the option for calculating the average PPs, the display for the current article or the display for all dimensions of the article applies.

> **Updating the display**
> The display of the average prices is updated for the respective stock article during archiving or invoice check. As a result, the display remains clearer. A+W Business assumes that the prices will not be changed anymore after these processes. However, if you still change prices after one of the processes, these changes are not included in the calculation of the average price.

### Stock management – supplement tab

**Path:** `Stock management > Stock management > Supplement tab`

**(Fig. K-51 Stock management - supplement)**

On this tab reservations for a selected stock article are shown. The fields in the lists are described in detail in connection with the Stock Article tab. (See also: "Stock management - stock articles" on page K-3070)

#### Reservation
The fields in this area are enabled for individual customers only.
- **Customer**: Number and name of customer for whom the selected stock article is reserved.
- **Fully locked**: Not currently used.
- **Exclusive reservation**: Not currently used.

#### Supplier
- **Supplier**: Number and name of supplier from whom the stock article is ordered.

#### Remark
- **Product related, Storage location related**: You can enter additional information for each stock article and each storage location, e. g. when and from which supplier glass/boxes were supplied, so that older deliveries are used first.

## Stock Movement

**Path:** `Stock management > Stock movement`

You can manually book withdrawals and additions for stock articles, correct stock figures, rebook storage locations and resolve boxes.

This section provides information on the following subjects:
- "Options menu" on page K-3261
- "Stock Movement" on page K-3261

### Options menu

**Path:** `Stock management > Stock movement`

The following entries are displayed:
- **Protocol at shut down:** When exiting the dialog, the stock history is automatically shown.
- **Stock > 0:** Only stock articles with a stock on hand of over 0 will be shown.

### Stock Movement (Dialog)

**Path:** `Stock management > Stock movement`

Additions and dispatches of stock articles are automatically booked: for receipt of goods by delivery and for goods issued by orders. You can manually book additions or dispatches in the Stock Movement dialog, e. g to correct stock quantities.

Dialog `Stock Movement` offers the following tabs:
- Stock movement - dispatch, addition
- Stock movement - transfer
- Stock movement - number of Sheets
- Stock movement – open boxes

### Stock movement – dispatch, addition

**Path:** `Stock management > Stock movement > Dispatch tab, Addition tab`

**(Fig. K-52 Stock movement – dispatch, addition)**

You can manually book goods issued and received on the `Dispatch` and `Addition` tabs. You can select a certain stock article and enter the corresponding data. If you have all stock articles displayed you can select the requested article on the `Storage places` list. The fields in the `Change stock on hand` section are then enabled.
(See also: Tutorial, "Stock Management for Boxes" on page K-3044)

If you have activated the option `Protocol at shut down`, the stock history is automatically shown on the `Table` tab when you close the dialog.

> **Manually enter addition of boxes**
> Since every box is kept with its own ID, you can enter additions of boxes only via `Goods Receipt` or `Stock Management`. In `Stock Management`, you create the box as a new stock article.

#### Stock product
- **Product**: Number and name of the stock article.
- **ID no.**: You can only book stock dispatches via the ID no. Additions of boxes must be defined in Stock Management so that you can enter a new ID. Boxes added have to be defined in inventory management in order to enter a new ID.
- **Content**: If you have selected a box, then its content is displayed. If a box with an ID no. that has already been allocated to an order is to be delivered or opened, a message is displayed. This prevents that negative stock is created by the subsequent printing of the delivery note or invoice.
- **Storage place**: Storage location that the stock article has been allocated to.

> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations `<n.e.>` will remain and can be booked.

- **Average PU**: The average purchase price is only shown if the function has been activated in the master data. (See also: Master data, "Calculate purchase price” on page B-981)

#### Change stock on hand
- **Quantity**: Enter the quantity that is to be booked out or in to stocks in pieces. If you go below the minimum stock when booking articles out of stock, a warning message is displayed.
- **Width, height**: These fields are only filled with quantity unit `sqm` if it involves stock sizes.
- **Assessment price**: Enter the purchase price at which the goods received were supplied.
- **Booking date**: The current date is shown automatically. It can be changed if required.
- **Remark**: You can enter a remark or select from the combo box. The remark will be displayed in the stock history. Use the button to add a new remark to the list. (See also: "Remark (stock movement)" on page K-3082)

#### Storage locations
- **Color:** The color is only shown for variations.
- **Width, Height:** Dimensions are only shown if the product has been defined as a stock size or box.
- **Contents:** Value 1 is shown for stock articles and stock sizes and the number of sheets for boxes.
- **Storage location:** Storage location in the order of level 1 through 4.
- **ID no.:** Box ID (manual booking or from goods receipt).
- **Stock on hand:** Current stock
- **QU:** Quantity unit with which the product is kept in stock.
- **Del. ID:** Supplier's box ID.

### Stock movement - transfer

**Path:** `Stock management > Stock movement > Transfer tab`

**(Fig. K-53 Stock movement - transfer)**

Use this tab to book a stock article to a different storage location. When you transfer a storage location, the entire stock of this storage location is always booked to the other storage location.
(See also: Tutorial, "How to transfer the storage location" on page K-3060)

The fields in sections `Stock product` and `Storage locations` are described under tab `Dispatch`.
(See also: "Stock movement - dispatch, addition" on page K-3079)

#### Storage place
- **Storage place**: Displays the current storage place. You can allocate a different storage place. The combo box lists all stored storage places.

> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations `<n.e.>` will remain and can be booked.

### Stock movement – number of Sheets

**Path:** `Stock management > Stock movement > No. of sheets tab`

**(Fig. K-54 Stock movement – number of sheets)**

Use this tab to correct the content of boxes.
(See also: Tutorial, "How to correct the number of sheets in a box" on page K-3061)

The fields in sections `Stock product` and `Storage locations` are described under tab `Dispatch`.
(See also: "Stock movement - dispatch, addition" on page K-3079)

#### Content change
- **Content**: Only if a box with an ID has been selected, the number of sheets that should in the box, is displayed. You can correct this value.

### Stock movement – open boxes

**Path:** `Stock management > Stock movement > Open boxes tab`

**(Fig. K-55 Stock movement – open boxes)**

Use this tab to resolve boxes so that the individual sheets are available for production. During this process, the box is booked out of the inventory and the number of sheets is booked to the inventory of the stock size.
(See also: Tutorial, "How to open a box" on page K-3062)

> **Book box content to a different storage location**
> When you open a box, its content is booked to the same storage location of where the box is located. If you want to transfer the content, you must book it out of the previous storage location and subsequently, book it to the new storage location.

The fields in sections `Stock product` and `Storage locations` are described under tab `Dispatch`.
(See also: "Stock movement - dispatch, addition" on page K-3079)

#### Open box
If a box with an ID no. that has already been allocated to an order is to be delivered or opened, a message is displayed. This prevents that negative stock is created by the subsequent printing of the delivery note or invoice.
- **No. of boxes**: Number of boxes that are to be opened.
- **Different contents**: The number of sheets is shown only if you have selected a box. You can correct this value.

### Remark (stock movement)

**Path:** `Stock > Stock movement > [Remark]`

**(Fig. K-56 Remark concerning stock movement)**

Use this dialog to store remarks that are offered for selection in the `Stock movement` dialog. If you leave the first line blank you can also delete an allocated remark.

## Search

**Path:** `Stock management > Search`

You can retrieve the stock on hand by individual stock articles or by product groups.

> **Set filter**
> If no filter is set, no data will be displayed.

The dialog is described in detail in the Sales part.
(See also: Sales, "Stock info" on page C-1825)

Dialog `Stock search` offers the following tabs:
- Stock search - stock search
- Stock search - future stock on hand

### Stock search – stock search

**Path:** `Stock management > Search > Stock search tab`

**(Fig. K-57 Stock search - stock search)**

Use this tab to display the current stock on hand, reserved quantities and future stock on hand for stock articles.
(See also: Tutorial, "Stock control mode and reservation" on page K-3007)

#### Selection
The fields are only enabled in selection mode.
- **Product**: Product number by which the product has been entered in the master data.
- **Type**: Product type this product has been assigned to in the master data.
- **Group**: Product group this product has been assigned to in the master data.
- **ID**: Identification number by which the stock article has been entered in the stock, e. g. for a box.
- **Categ.**: If you have defined stock categories in your company, these can be used as filters. (See also: Master data, "Stock Categories" on page B-791)
- **Color**: (Color) variations that have been defined for the selected product.
- **from, to PGR**: You can also enter product groups or product group areas. The overview then displays all the products of the selected product groups.
- **Thickness / width / height**: These details are transferred from stock management. Width and height are only displayed if the selected item has been entered as a stock size or box, including the corresponding details.
- **Storage place**: If you are using different storage locations, the storage location of the selected item will be shown, including all defined levels. (See also: Master data, "Stock Definition" on page B-789)
- **Supp. ID**: Identification number of the shipment from stock management. It is not identical with the entry in the ID column.
- **Remark**: Information stored for the selected item when delivered.
- **Contents from, to**: You can use the contents as a search criterion in the selection mode, e.g. all boxes with a content of 50 pieces. Contents = 1 always means stock size.
- **Availability**: Displays the available pieces.

#### Filter options
If no filter is set, no stock will be displayed. A filter is set if the corresponding checkbox is ticked. The following filters are available:
- **Stock articles:** Stock articles will be displayed.
- **Boxes (contents > 1):** Boxes with a content of > 1 will be displayed.
- **Stock sizes (contents = 1):** Stock sizes will be shown. Display of the quantity (= 1) helps to distinguish boxes of identical sizes.
- **Group boxes by storage location and supplier:** Only one line is displayed per storage location and supplier.
- **Articles without sizes:** Even stock articles for which no sizes have been entered will be shown.
- **No boxes with ID:** Boxes entered with an ID at receipt of goods shall not be shown.
- **Minimum qty > 0:** Only stock articles with a minimum quantity of over 0 should be displayed.
- **Stock > 0:** Only stock articles with actual stock should be displayed.
- **Stock = 0:** Only stock articles without stock should be displayed.
- **Stock < 0:** Only stock articles that have been reserved, but are without stock, should be displayed.

#### Print options
You can define the sorting of the list for printing purposes. The appropriate checkboxes will be enabled with the selected option. You can then additionally define where a subtotal will be printed.
The following entries are displayed:
- **Group by product no.:** The checkbox `Subtotal by product group` is enabled.
- **Group by product type/group:** The `Subtotal by superior product group` checkbox is enabled. `Product super group` is enabled.
- **Group by product group:** The `Subtotal by main product group` checkbox is enabled.

#### Overview
The overview lists all products that have been selected by means of the search. The columns provide details on the stored products.

The reserved quantities will be updated as soon as a corresponding item has been saved in the order. The details in column `Stock on hand` will be updated when a delivery note is issued.
The entries in the hit list are identified with the following colors:
- **Black:** Quantity-based stock article
- **Blue:** Stock article not quantity-based
- **Red:**
  - No stock article: articles that are not kept on stock.
  - This applies also to products which are no longer available, or which show negative quantities. Negative quantities occur if the stock on hand and the order quantity minus the reserved quantity <= 0.

#### Totals
The totals of the selected products are shown. If you have selected a PGR with different products, the totals of the selected product are shown.

### Stock search – future stock on hand

**Path:** `Stock management > Search > Future stock on hand tab`

**(Fig. K-58 Stock search - future stock on hand)**

Use this tab to check whether the replacement times for a certain product are sufficient to delivery an order in accordance with the schedule. The color red shows that scheduled dates cannot be met. Yellow indicates that the replacement time is sufficient if the purchase orders are received on time.

The replacement time results from the delivery time that has been defined in the supplier file for the article and the supplier's route days that are defined in route management.

#### Preview up to
The preview always starts with the current date. Set the number of days for the preview in the company data, e. g. 14 days.
- The list at the top shows the data for each selected product in one line.
- The list in the center shows the stock on hand per day.
- The list at the bottom displays details on the selected product.

The lines are red if production is impossible because the reservations exceed the stock on hand.

In order to increase the performance you can restrict the preview display by the following settings:
- You can remove certain articles from the stock preview and availability check in dialog `Product management > Stock/Purchasing > No availability check` checkbox, by disabling the availability check for these articles.
- In the `Company data` dialog you can set the time period displayed in the preview.
- You can link several stock sizes together in the dialog `Stock management` so that the stock check is only executed for the defined main stock article. (See also: "Main product" on page K-3071)

## Order pool

**Path:** `Stock management > Stock P.O.`

Use this dialog to check all suggested stock P.O.s and transfer them to Purchasing.

This section provides information on the following subjects:
- "Order pool menus" on page K-3274
- "Order pool" on page K-3277

### Order pool menus

By using the menus you can have the date fields updated automatically and open other dialogs additionally.

This section provides information on the following subjects:
- "Functions Menu" on page K-3274
- "Options menu" on page K-3275

#### Functions Menu

**Path:** `Stock management > Stock P.O. > Functions menu`

This menu can be used to open other dialogs without closing the P.O. transfer. The following entries are displayed:
- **Change supplier/delivery date:** Opens the dialog `Change supplier and delivery date`. (See also: "Change supplier and delivery dates" on page C-1758)
- **Marking options:** Opens dialog `Marking options`. (See also: "Marking options" on page C-1759)
- **Supplier prices:** Opens dialog `Price comparison`. (See also: "Price comparison" on page C-1759)

#### Options menu

**Path:** `Stock management > Stock P.O. > Options menu`

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

> **Activated options after opening the dialog**
> Please note that changed options will only become effective the next time you open the dialog.
> If an activated option has started a check, opening the document can be delayed. The extent of the delay depends on the performance of the computer.
> Activated options are described in the following.

**Transfer group**
- **Order-related transfer:** Purchase orders are transferred by order. Collective P.O.s can be created if this option is disabled.
- **P.O. number = order number:** This option is only available if the option `Order-related transfer` has been enabled.
- **Order pool by user:** You can create separate order pools for every user.

**Delivery date group**
- **Check delivery date:** The delivery date is checked automatically. The system will inform you if you have changed a delivery date to a date which is not a route day.
- **Consider supplier's route:** If the delivery date for the P.O. is not a route day, a message to that effect will be issued. This requires that supplier's routes have been defined in the master data. (See also: Master data, "Routes" on page B-894)
- **Determine lead days based on PGR combinations:** If lead days have been defined for PGR combinations, these will be used to calculate the delivery date. (See also: Master data, "Lead days" on page B-645)

**Product name group**
- **Product names as per the supplier file:** The names of the ordered products are adopted from the supplier file.
- **Product names as per master data (internal P.O.):** For internal purchase orders, the names of the ordered products are loaded from the product master data.

**Other group**
- **No saving of costs:** Costs are not written back to the purchase prices of the order.
- **Consider size surcharges:** Size surcharges will be transferred with the P.O.
- **Always set print code for processing:** On the P.O. processing steps shall always be printed. If this option is disabled, the print codes are adopted from the order into the P.O. without any changes.
- **Statistics PGR as per order:** The statistics PGR information is adopted from the order if different statistics PGRs have been defined for order and P.O.
- **Business type as per order:** The business type is adopted from the order if different business types have been defined for order and P.O.
- **OM area as per order:** The OM area is adopted from the order if different OM areas have been defined for order and P.O.
- **Consultant = user for new input:** The P.O. automatically shows the name of the user logged on to A+W Business.
- **Check change of status:** The query concerning the change of status is displayed.
- **Repeat transfer only up to lock status:** Purchase orders can be transferred several times but only until lock status has been reached.

**Further settings group**
- **Settings:** Opens the `Further settings` dialog in which you can define information concerning printing texts and file attachments.

### Order pool (Dialog)

**Path:** `Stock management > Stock P.O.`

**(Fig. K-59 Order pool)**

In this dialog you can view all suggested purchase orders for articles that fall short of the minimum stock. The order quantity is calculated by the quantity that has been defined in the dialog `Stock management`.

After the transfer, the purchase orders are created and can be printed and sent.
- Tutorial, "Stock P.O. of boxes" on page K-3045
- Tutorial, "Manual and automatic stock P.O." on page K-3037

#### Storage place
- **Warehouse, Corridor, Shelf, Tray**: You can restrict the display to individual storage locations. Please remember that stock articles may be booked to storage location `<n.e.>`. If you do not restrict the selection, purchase order suggestions are displayed for all articles that fall short of the minimum stock. The name of the storage locations can be changed in the master data.

#### Overview
The data relating to the purchase order suggestions is displayed in the overview. You can select a different supplier and view a price comparison.
- **Supplier:** The supplier is adopted from the supplier file. You can change the name if no supplier has been entered or if your standard supplier has supply problems.
- **Article/color:** Number and - if applicable - variant of the product to be ordered.
- **ID no.:** Box ID (manual booking or from receipt of goods)
- **Storage location:** Storage location where the stock on hand of the stock article falls short.
- **Quantity:** Quantity to be ordered. The standard purchase order quantity is multiplied until the minimum stock on hand is exceeded. You can also change the value directly on the list.
- **Width, Height:** Size of the lite to be ordered.
- **Contents:** Contents are only shown for boxes.
- **Deliv. supplier:** The supplier's delivery date is determined based on the entries in the supplier file. You can change the date if your standard supplier has supply problems.
  - Sales, "Change supplier and delivery dates" on page C-1758
  - Sales, "Price comparison" on page C-1759

#### Item for
The purchase order suggestions are displayed in different colors:
- **Red: internal order:** Internal orders are production orders that are created to fill stock on hand. The suggestion is automatically created if the corresponding option for the product has been enabled in the supplier file.
- **Blue: Inquiry:** Inquiry to a supplier e.g. to ask for prices and delivery times.
- **Green: Delivery might not be on time:** The current date is automatically set as the delivery date. As a result, the delivery is usually not possible on time. If you change the date the color for the entry changes to black.

#### Target Number Manager
- **Employee**: Name of the employee logged in to A+W Business or who has set up the Number Manager. If you create a new Number Manager you can allocate it to one particular employee.
- **Name**: Name of the target Number Manager for the purchase orders. A new Number Manager will be created when you enter a new name.

#### Target number area
- **Client**: If you have set up separate number areas for your clients you can select the requested client here.
- **Order area**: If you work with production preparations, you can allocate the purchase order to a certain order area.

## Receipt and Shipping of Boxes

You will find the complete descriptions of goods receipt and shipping of goods in the `Production` and `Purchasing` sections.

This section provides information on the following subjects:
- "Receipt of goods (boxes)" on page K-3280
- "Settings (ID)" on page K-3291
- "Shipping of boxes" on page K-3292

### Receipt of goods (boxes)

**Path:** `Documents > P.O. > Receipt of goods > Receipt of goods`

This dialog serves to enter the goods received for individual purchase orders or for the purchase orders in a Number Manager.

For booking stock on hand, you can define ID numbers to be automatically assigned if the stock P.O. includes items with a quantity of larger than 1. The ID numbers are assigned for boxes and glass (stockplates).

> **Prerequisite**
> The checkbox for the virtual assignment of item numbers must be checked in company data.
> (See also: "Company data" on page K-3013)

This dialog offers the following tabs:
- "Receipt of goods - selection" on page K-3281
- "Receipt of goods -complete" on page K-3283
- "Receipt of goods - by item" on page K-3285
- "Receipt of goods – ID numbers" on page K-3288
- "Receipt of goods - protocol (ID numbers)" on page K-3290

### Receipt of goods – selection

**Path:** `Documents > P.O. > Receipt of goods > Receipt of goods > Selection tab`

**(Fig. K-60 Receipt of goods – selection)**

This tab is used to filter the selection and display of documents for which receipt of goods shall be checked and/or entered.
(See also: Tutorial, "Receipt of goods" on page D-1941)

#### Selection
By choosing the option, you define how the purchase orders shall be filtered. Open purchase orders are displayed after the search in the `Complete` tab so that receipt of goods can be booked.
- **By P.O. number:** The input field for the P.O. number can be accessed. Tab `Complete` shows the required purchase order and all reference orders.
- **By order number:** The input field for the order number is released. The `Complete` tab shows all purchase orders issued for the defined order number.
- **By supplier:** The input field for the supplier number is accessible. Tab `Complete` shows all purchase orders placed with the selected supplier.
- **By delivery note number/notification, total quantity delivered:** The input field for the delivery note number or notification number and the field for entering the total quantity can be accessed. If a dispatch notification has been imported, the actually received quantities must be entered.
- **By supplier delivery date:** The input field for the delivery date is accessible. Tab `Complete` shows all purchase orders to be delivered on the selected date.
- **By number manager:** The combo box for selecting the number manager is accessible. Tab `Complete` shows all purchase orders in the selected number manager.
- **By scanner / document:** The fields for the barcode of the P.O. number or a P.O. item are released.

#### Target Number Manager
- **Target Number Manager**: After booking the receipt of goods, the stock P.O.s can be automatically transferred to a different Number Manager.
  - The stock P.O.s are not moved to a different Number Manager.
  - The fields in the Target number manager section are accessible. The orders are moved to the selected number manager.
- **Employee**: Name of the employee allocated to the target Number Manager.
- **Number Manager**: Number Manager to which the stock P.O.s with (complete) receipt of goods should be moved.

### Receipt of goods -complete

**Path:** `Documents > P.O.> Receipt of goods > Receipt of goods > Complete tab`

**(Fig. K-61 Receipt of goods – complete)**

This tab shows all purchase orders matching the search criteria. Select a purchase order to list all reference orders.
(See also: Tutorial, "Enter receipt of goods" on page D-1948)

#### Delivery date
- **Supplier's delivery date**: Shows the current date. You can change it to enter a delivery received before that date. The date will be adopted only for the documents selected in the list.
- **OC supplier**: You can also enter the supplier's order confirmation number for the goods received.

#### Documents
You can use these buttons to select some documents or cancel the selection.
The list shows all purchase orders matching the search criteria on the `Selection` tab. Complete receipt of goods is entered for the documents for which the `Book Complete` checkbox is ticked.
- **P.O. no.:** Purchase order number.
- **Book as complete:** A purchase order can be booked as complete when all items were delivered.
  - Receipt of goods is incomplete. Some deliveries have yet to be made.
  - Receipt of goods is incomplete; the purchase order will be booked as complete.
- **Status:** Current status. The status is changed after receipt of goods has been entered.
- **Supplier:** Name and number of the supplier.
- **Supplier's delivery date:** Delivery date stated by the supplier. This date is adopted from the purchase order or order confirmation. When you have entered the receipt of goods, the date is changed to the present date or to the date you have selected.
- **Contains boxes:** Shows the purchase orders which include boxes. This checkbox cannot be selected.

#### Appended orders
This list shows only the reference orders for the selected purchase order. If several purchase orders are selected, this list remains empty.
- **Delivery at the customer's site**: This date is adopted from the reference order. You can change it if the originally scheduled date cannot be adhered to.
