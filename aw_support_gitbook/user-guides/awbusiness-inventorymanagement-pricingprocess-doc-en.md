---
description: "A+W Business Inventory Management Tutorial"
---


---
## The pricing process

This section outlines the logical flow the system follows to determine the price of a product.

*   **1. Start Price Search:** The process begins.
*   **2. Manual Price Code Input?**
    *   **Yes:** The system searches the Purchase Price (PP) in the rate allocation of the manually defined price key. The process then ends.
    *   **No:** Proceed to the next step.
*   **3. Exists in Product Stock Sizes?**
    *   **Yes:** Proceed to check how the price is determined from stock.
        *   **A. Search by Average Price Active?**
            *   **Yes:**
                1.  **Exact Product Variant in Stock?**
                    *   **Yes:** The system selects the average Purchase Price (PP) from the specific stock article.
                    *   **No:** The system creates a weighted average price for all stock products for which the corresponding code has been enabled.
                2.  **Calculated Price > 0?**
                    *   **Yes:** The process ends.
                    *   **No:** The process continues as if the average price search was inactive (see step B).
            *   **No:** Proceed to the next check.
        *   **B. Different Price Code for PP Defined?**
            *   **Yes:** The system searches the PP in the rate allocation of the defined price key. The process then ends.
            *   **No:** The system searches the PP in the standard rate allocation. The process then ends.
    *   **No:** The product does not exist in stock sizes.
        *   **Search by Average Price Active?**
            *   **Yes:** The process loops back to determine the average price (Step 3.A.1).
            *   **No:** The process ends.

## Notes on the pricing process

Pricing first searches in product stock sizes whether the article exists in just the defined variant.

*   If so, the average price of the stock article will or will not be calculated, depending on the code. If the code is inactive, the system will search for the price in the standard purchase rate. If a different PP code has been defined, it has priority over the standard rate.
*   If the article cannot be found in product stock sizes, the system goes on searching for the average price on stock.

### Average price

Average price calculation goes through the following levels:

*   If the average price is determined from stock, the system first searches for the exact stock article. If this article exists, the defined price will be used.
*   If the article does not exist, the weighted average price for all products of this article number with an active code will be determined.
*   If the determined price is 0, the system will search for the price in the standard purchase price allocation.
*   If the price code has been entered manually at order entry, the price is calculated only from the rate allocated to the selected price key, without searching for an average price.

The codes do not influence the saving of costs for the corresponding stock article.

Here are some examples for the price search process.

**Product stock dimensions**

| Article | Size | Calculate average price | Diff. price key |
| :--- | :--- | :--- | :--- |
| 1004 | 3210 x 6000 | Yes | Stock sizes |
| 1004 | 3210 x 3000 | No | <n.e.> |
| 1004 | 3210 x 2000 | No | Stock sizes |

**Stock management**

| Article | Size | Overall average price calculation | Stock on hand | Average price |
| :--- | :--- | :--- | :--- | :--- |
| 1004 | 3210 x 6000 | Yes | 100 pcs | 1.25 €/qm |
| 1004 | 2000 x 2000 | Yes | 40 pcs | 1.84 €/qm |
| 1004 | 1500 x 3000 | No | 45 pcs | 1.99 €/qm |

**Prices acc. to rate allocation in price management**

| Price Key | Price |
| :--- | :--- |
| Default | 1.50 €/qm |
| Stock sizes | 1.00 €/qm |

**Order with calculated purchase prices**

| Itm. | Article | Size | Price key definition | PP |
| :--- | :--- | :--- | :--- | :--- |
| 1 | 1004 | 3210 x 6000 | No | 1.25 €/qm |
| 2 | 1004 | 2000 x 2000 | No | 1.44 €/qm |
| 3 | 1004 | 3210 x 3000 | No | 1.50 €/qm |
| 4 | 1004 | 3210 x 2000 | No | 1.00 €/qm |
| 5 | 1004 | 1250 x 1433 | No | 1.30 €/qm |
| 6 | 1004 | 3210 x 6000 | yes (stock sizes) | 1.00 €/qm |

## Check Settings for Purchase Price Calculation

You have already set the stock control mode in the company data. Now enable the purchase price calculation and select the calculation type.

### How to check the settings for the purchase price

1.  Select menu **Master Data > Company > Company Data**.
2.  Go to the **Stock / PCH / EDI** tab.
3.  Check the checkbox **Calculate purchase price (A)** to enable the options:
    *   **Average PP:** The average purchase price will be recalculated whenever goods are added to stock.
    *   **Last PP:** The last purchase price booked on stock when goods were received or an invoice was checked, will be used for stock evaluation.
    *   **Ignore combined articles without sizes:** Check this checkbox if combined stock articles without sizes shall not be considered for average purchase price calculation.
4.  Go to Menu **Start > Save** to save the data.

The data is saved.

*In the `Company data - Stock / PCH / EDI` screen (Fig. G-23), key settings include:*
*   **A**: `Calculate purchase price` checkbox.
*   **B**: Purchase price calculation type radio buttons (`Average purch. price`, `Last purch. price`).
*   **C**: `Ignore combined stock articles without sizes` checkbox, an additional function for the combined stock control mode.

## Check Prices

This section tells you how to define purchase prices.

The following conditions must be fulfilled to calculate the average purchase price:

*   The product has to be defined as a stock article.
*   The PP code must be set in company data.

As a general rule, just one price key is entered for the PP but you can use several PP price keys if required. Next, all price keys for the PP have to be defined as a combined rate. If there are several price keys for the PP, a default price list should be defined. You can enter a price if required. This will not be changed when the average price is calculated. The average PP appears in special fields in stock management.

### How to check the master data of your price lists

1.  Go to menu **Master data > Prices** and check the settings in the dialogs **Year, Key,** and **Rate**. You only need to check the entries used for the prices (and other internal calculations) for stock sizes and boxes.
2.  Select menu **Master Data > Prices > Prices**.
3.  Please check if all purchase and sales prices have been defined and are up to date, and complete or correct them as necessary.
4.  Go to the tab in which the price is defined, check if the purchase price has been entered correctly, and correct it if necessary.
5.  Go to Menu **Start > Save** to save the data. The data is saved.

### Exercises

*   Check whether the correct price lists have been allocated to the stock sizes.
*   Create a new price list with an individual purchase price for a stock article.

### Additional information

*   ⇨ Software Reference, "Reserved Stock Products" on page G-215
*   ⇨ Software Reference, "Purchase prices" on page G-190
*   ⇨ Master Data, "Status Allocation" on page B-426
*   ⇨ Master Data, "Input of Unit Prices" on page B-236
*   ⇨ Master Data, "Prices" on page B-713
*   ⇨ Master Data, "Rates" on page B-662
*   ⇨ Master Data, "Calculate purchase price" on page B-955
*   ⇨ Master Data, "Stock control mode" on page B-958

## Stock control on BOM level

### Objectives

*   Getting familiar with the relation of the procurement type on the main product levels and the BOM components.
*   Checking the settings in the company data.

### Benefits

*   BOM components required for production can be kept as stock articles.

### Please note:

| Level | Description |
| :--- | :--- |
| **Level: main article** | If the main article is already defined as a stock article, all BOM components are automatically defined as stock articles. |
| **Level: BOM** | Each BOM component can be defined as a stock article even if the main product's procurement type is Production. |
| **Default settings** | **Master data:** Product management, Supplier file. **Company data:** Parameters tab, Tab Stock/PP/EDI. |

## Reservation and booking of BOM components

Stock articles can be both main products or BOM components. For a complete door which is sold including the fittings, you can define the glass as an in-house product and the fittings as stock articles.

If the main article is already defined as a stock article, all BOM components are automatically defined as stock articles.

*In the product settings screen (Fig. G-26), you can set the procurement type for a main product and its BOM components.*
*   **A (Procurement type main product):** The procurement type for the main product (e.g., `Waschtisch`) is set, for example, to `Lagerentnahme/Stock withdrawal`.
*   **B (Procurement type BOM component):** The procurement type for a component within the BOM (e.g., `Handtuchhalter`) can also be set to `Lagerentnahme/Stock withdrawal`.

When you enter such a BOM article in the order, every component defined as a stock article will be displayed in the stock search. If you check this main product on the Stock info dialog, all BOM components will be shown as well.

*In the order entry screen (Fig. G-27), when a BOM article is added:*
*   **A (Order item):** The main BOM product (e.g., `Waschtisch`) is shown with its components listed below it.
*   **B (Stock info - BOM components):** The stock information for each component defined as a stock article is displayed, showing quantity, stock on hand, reservations, etc.

All BOM components will be reserved after you have saved the order.

*The Booking Journal (Fig. G-28) will show the reserved BOM components after an order is saved, listing the article, quantity, order number, and booking date.*

If the BOM shows 2 pcs. of a primary component, the quantity of the secondary components (children) to be booked on stock is multiplied by 2.

### Checking the setting

Option **Stock control on BOM level** must be enabled in the company data. In the `Company data – Stock / PP / EDI` settings, ensure the `Stock control on BOM level` checkbox is checked.

## Checking Products

This module shows you how to check the procurement type of the BOM components in product management.

### How to set up your bills of material for stockkeeping

1.  Select menu **Master Data > Products > Articles > Articles**. The dialog **Product Management** opens.
2.  Search the product you want to keep on stock by means of bills of material.
3.  Go to tab **BOM**.
4.  Tag the corresponding BOM component and select the procurement type if this shall differ from the procurement type defined in this component's master data.
    *   In the Product Management screen (Fig. G-30), you can select a component and set its **Procurement type (A)** and enable **Calculate purchase price (B)**.
5.  If the procurement type for the main product is set to **Stock withdrawal**, this applies to all BOM components.
6.  If the procurement type for the main product has been set to **Production**, the BOM components can be kept as stock products at the same time. When you enter such a main product in your order, all BOM components will be set to reserved in the stock info.
7.  Go to Menu **Start > Save** to save the data.
8.  Repeat the steps for all eligible products.

## Stock Management

In this thematic block you will learn how to enter and maintain stock articles. This includes the following training modules:

*   "Stock Management" on page G-65
*   "Stock Booking" on page G-75
*   "Queries" on page G-85
*   "Stock information" on page G-94
*   "Stock P.O. (automatic)" on page G-103

### Objectives

*   Getting familiar with the Stock Management dialog
*   Create a stock article

### Benefits

*   Stock articles serve to define and maintain the stock on hand.
*   Stock on hand of stock articles is updated with the booking of goods withdrawals and additions.
*   Based on the stock articles, you can determine the current stock on hand including reservations and purchase orders.

### Please note:

| Topic | Detail |
| :--- | :--- |
| **Calculate the stock on hand** | Quantities and surfaces can be calculated correctly only if the stock articles have been properly created. |
| **Stock articles** | Only stock articles can be managed in the stock. Products defined in the master data will not be automatically kept as stock on hand. |
| **Receipt of goods, issue** | Receipt and issue of goods can only be booked for stock articles. |
| **Default settings** | **Master data:** Storage locations, Products, Stock sizes. |

### Elements in Stock management Dialog

Each stock article can be created in different variants, e.g. Float 5 mm in several sizes.

*Key elements in the Stock Management dialog (Fig. G-31) are:*
*   **A**: Product number
*   **B**: Stock article sizes
*   **C**: Standard storage location
*   **D**: Stock category
*   **E**: Main stock article code
*   **F**: Inventory audit for the stock preview
*   **G**: Defined stock articles list
*   **H**: Main product indicator
*   **I**: Number of sheets in boxes
*   **J**: Storage place (4 levels)

If the stock on hand is not checked for each storage location (F), a main product (E, H) must be allocated to determine the available square meters of the glass.

The stock on hand can be kept per storage location (J). The defined storage locations are allocated to the stock articles for this purpose. If a stock article is kept in different storage location, you must define a standard storage location(C).

Additions and withdrawals will be automatically booked at the standard storage place but can be changed manually.

### Stock Articles

Products defined in master data will not be kept on stock automatically. This makes sure that stockkeeping includes only articles that are actually kept on stock. Other articles which are stored only temporarily for the production of a special order, do not have to be kept as stock articles.

Every (glass) product is related to a stock size and a stock article. The relations have already been explained in the training module on Products.

#### Main Stock Products

You can link several stock sizes in stock management by defining a main stock product. The inventory check (for the stock preview in dialog Stock info) is executed only for the main stock product in this case; a minimum stock has to be defined only for this article.

> **Example**
>
> Article 1004 has been entered with the following sizes:
> 0 x 0, 500 x 600, 1200 x 1800, 3210 x 4000 and 3210 x 5000.
>
> For the sizes 3210 x 4000 and 3210 x 5000, article 0 x 0 has been defined as the main stock product. The minimum stock for this article has been specified as 19,000.00 sqm.
>
> The stock on hand of the sizes 3210 x 4000 and 3210 x 5000 are summed up and compared with the minimum stock of 19,000.00 sqm.
>
> Separate minimum stock has been defined for sizes 500 x 600 and 1200 x 1800 which will be used for checking.

If you have defined the stock articles each with a minimum stock, you can still allocate them to a main product later. Determination of the minimum stock only checks the settings for the main product; the minimum stock defined for the stock articles will be ignored.

### Minimum Stock

If the stock on hand for an article falls below a certain minimum quantity (taking into account the orders and purchase orders), replacement must be ordered in good time so as not to impede the production. A+W Business allows you to enter a threshold for the minimum stock. This is defined by article.

The minimum stock is a parameter the stock should not fall short of, neither in reality nor in connection with reservations made.

Based on the defined minimum stock, the inventory will automatically issue purchasing suggestions. These have to be released manually. Automatic purchase suggestions use the following key figures as a basis for calculating the quantities to be ordered:

*   Ordered quantity
*   Reservation
*   Minimum stock
*   Standard purchase quantity
*   Current stock on hand

To define the article precisely, width and height are evaluated, among other things.
Calculation of the purchase quantity will be introduced in a separate module.

⇨ "P.O. Quantity after Stocktaking" on page G-130

### Prices

The prices of a stock article are shown as average purchase prices (purchase prices) if this function is enabled in the company data. The display of the average prices is updated for the respective stock article during archiving or auditing (invoice check).

A+W Business assumes that the prices will not be changed after this process. However, if you still change prices after one of the processes, these changes are not included in the calculation of the average price.

*In the Prices tab of the Stock Management screen (Fig. G-32), you can see:*
*   **A (Display mode):** Options to calculate average price for "Only this article" or "All sizes".
*   **B (Average prices in purchasing):** A history of price changes from purchases and issues.
*   **C (Include in total PP):** A checkbox to include the current article's prices in the total calculation.
*   **D (Average price):** The calculated average price per article or for all sizes.
*   **E (Stock values):** Key price figures like lowest, max, and last price for the tagged article.

You can specify whether all sizes of an article shall be included in the average price calculation. Only if you have checked the check-box **Include in total PP (C)**, the prices of the current article will be included in the calculation.

The selected mode (A) determines the price view:

*   **Only this article:** For the calculation only the displayed article in the selected size is taken into account. The PP history of the current article is displayed.
*   **All sizes:** For the calculation all dimensions of the displayed glass are taken into account. The PP history of all dimensions of the article is displayed.

The average PP is calculated for every record, except for goods issued. Goods issued only reduce the stock. The displayed list of recalculations (B) is reduced by archiving and the invoice check. As a result, the view remains clearer.

The first data record shows the opening stock and the original price. Underneath you will find the goods received and issued (minus sign). If goods have been received as a result of a stock P.O., the P.O. number and the P.O. item are furthermore displayed.

The average PP is updated during entering or changing purchase orders. It is determined by taking the total quantity into account.

> **Example:**
>
> 100 pieces on stock each 15.00 € = 1500.00 €
> 40 pieces new booking each 18.00 € = + 720.00 €
> **Total = 2220.00 €**
>
> 2200.00 / 140 pcs. = 15.86 €

Automatic surcharges that are listed in the purchase orders, e.g. energy and transportation surcharge, are also included in the calculation.

#### Distribution of surcharges

Costs incurred by a stock P.O. will be added to the purchase prices of all articles of the P.O. These costs can be freight, energy surcharge, or any other costs related to the provision of stock articles.

This redistribution depends on the price unit of the surcharge. If the price unit is kg, the surcharge is redistributed based on the item weight. For all other price units, redistribution is based on the item price.

Since every change of item will influence the redistribution to all other items, redistribution for the entire document will always be made after an item has been changed, i.e. when all items have been entered.

Changes of items will update the PP only until the invoice is checked.

Footer surcharges have been introduced in the training session on Purchasing.

## Create a Stock Article

This module shows you how to create the required stock articles. You have to define at least the following settings in order to manage the stock:

*   Article number and name
*   Dimensions for stock dimensions
*   Storage location and standard storage location (default storage location)
*   Stock on hand

> **Inventory start-up**
> If no stock articles have been entered at all, you can facilitate this task by running the so-called initial inventory. This process will be introduced in a separate training session.

### How to create a stock article

1.  Go to menu **Stock management > stock management**. The **Stock management** dialog opens.
2.  Go to the menu **Start > New** to switch to the input mode.
    If you open the Stock management dialog from the master data, this step can be omitted. The fields for articles and sizes are filled in already.
3.  Enter the number (A) and size (B), if applicable.
4.  Choose a storage location (C).
    If no storage location is selected, the storage location `<n.e.>` will be entered. In stock management, this will be treated like the defined storage locations, e.g. for stocktaking purposes and queries.
    If a stock article is kept in different storage locations, you have to define one of them as the standard storage location.
5.  Check checkbox **Default storage location**.
6.  Go to field **Main product (D)** and select the article for which you want to enter the minimum stock for the inventory audit.
    To define a separate minimum stock for the new stock article, select the size of the new article. However, the new size will be displayed only after you have saved the new article. We recommend to select any size then change it after you have saved the article.
7.  Check the checkbox **Inventory audit per stock location (F)** if all storage locations shall be evaluated separately when checking the inventory for this stock article.
8.  Enter the quantities in section **Stock on hand (E)** if required.
    Please make sure to enter an appropriately high minimum stock if you have defined the same main product for several sizes. The checkboxes are enabled only in selection mode. They serve to filter the search by stock article. These are the minimum entries for stock articles.
9.  Select in the menu **Start > Save** to save the data.
    The data is saved. At the same time, a dummy stock article without dimensions is created for the combined stock control mode.
    Thus all necessary information A+W Business needs for reservations and booking have been defined. Bookings for the new stock article can be made now.

### Exercises

Enter the following stock articles and allocate the appropriate price list:
*   Stock article kept on stock in units.
*   Stock article Handle which is kept on stock in its individual quantity unit.

### Additional information
*   ⇨ Software Reference, "Management" on page G-176
*   ⇨ Purchasing, "Document P.O." on page D-43

## Stock Booking

### Objectives

*   Introducing the booking types for stock articles.
*   Introducing automatic stock bookings.
*   Manual trigger of stock bookings.

### Benefits

*   When stock articles are ordered, receipt of goods is automatically booked on stock, as is the issue of goods for order items.
*   You can correct the stock on hand for individual storage places by transferring stock articles.

### Please note:

| Topic | Detail |
| :--- | :--- |
| **Automatic booking** | Automatic bookings of additions will be triggered if the status of the P.O. is changed upon receipt of goods. Automatic dispatch bookings will be released if the status of an order is changed by printing. |
| **Booking types** | The booking types for stock bookings are fixed in the system. |
| **Manual bookings** | The following bookings can be triggered manually: Addition and dispatch of goods, Change storage location. |
| **Default settings** | **Master data:** Status allocations. **Company data:** Tab Stock/PP/EDI. |
