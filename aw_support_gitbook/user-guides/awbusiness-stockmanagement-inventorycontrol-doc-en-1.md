---
title: "EN_AWBusiness_Box_Management_1_1-4"
source: "EN_AWBusiness_Box_Management_1_1-4.pdf"
tags: ["stock management", "inventory control", "software reference", "A+W Business", "purchase orders", "stock movement", "inventory audit", "pricing", "average purchase price", "Kistenmanagement"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A software reference guide for the Stock Management module within the A+W Business Kistenmanagement system. It details functionalities for tracking stock levels, managing prices, handling stock movements, and generating purchase orders."
long_description: "This document serves as a comprehensive software reference for the Stock Management features in A+W Business Kistenmanagement. It provides detailed explanations of various functions, dialogs, and tabs available to users. Key topics covered include defining search criteria for stock articles (e.g., stock levels, minimum stock), managing inventory on a per-location basis, and understanding the system's logic for automatic purchase order suggestions. The guide also delves into the 'Prices' tab for viewing and calculating purchase prices, including the average purchase price (PP). It explains the process of handling stock movements such as dispatches, additions, transfers, correcting sheet counts, and opening boxes. Furthermore, the document covers the 'Search' functionality for retrieving stock information and analyzing future stock availability. Finally, it details the 'Stock P.O.' (Purchase Order) process, including the order pool, menu options, and the creation of purchase orders based on stock levels falling below minimums. This guide is intended for users who manage inventory and procurement within the A+W Business software."
---

---
## Stock Management

### Stock > 0
This checkbox is only available in the selection mode. Use it to define as a search criterion whether articles should be shown without stock quantity.

- The search result also shows articles, the current stock of which is 0.
- The search result only shows articles, the current stock of which is at least 1.

### Min. stock
The minimum stock forms the basis for automatic purchase order suggestions. They are created if stock falls below the minimum stock. Reservations and purchase orders are taken into account. You can check these automatic purchase order suggestions in the dialog Order pool.
⇨ "Stock P.O." on page K-96

### Minimum stock level > 0
This checkbox is only available in the selection mode. You can use it to define as a search criterion whether the minimum stock must be more than 0.

- The search result shows all articles.
- The search result only shows articles, the minimum stock of which is more than zero.

### Purch. qty.
This value specifies which quantity is ordered by default. This value is adopted for automatic stock ordering.

### Inventory < Min. Inventory
This checkbox is only available in the selection mode. You can use it to define as a search criterion whether the minimum stock must be below the minimum inventory.

- The search result shows all articles.
- The search result only shows articles, the current stock of which is less than the minimum inventory.

### Maximum stock level
By entering maximum quantities per stock article you can prevent the warehouse becoming overstocked. The entered value is only used for the manual check.

### Target quantity
Not currently used.

### Inventory audit per stock location
If you maintain stock per storage location you can check the stock per stock location.

- Stock is checked jointly for all storage locations.
- Stock is checked per storage location.

### Stock articles
The lists show stock articles that correspond to the search criteria. The top list shows all stock articles together. If you select one entry, the articles are shown per storage location in the bottom list. If the checkbox Stock > 0 has been activated, only storage locations with stock of more than 0 are listed.

The following columns are displayed:

-   **Articles, Quantity unit - Variation:**
    Article number, name, quantity unit and color from stock management.
-   **Width, Height:**
    Dimensions from stock management.
-   **Content:**
    Number of sheets in one box.
-   **Total stock:**
    Total stock of the stock article at all storage locations.
-   **Min. stock level:**
    Quantity of the defined minimum stock level.
-   **Purch. quantity:**
    Defined purchasing quantity.

### Storage locations
-   **ID:**
    Box ID (manual booking or from receipt of goods).
-   **Storage location:**
    Storage location in the order of level 1 through 4.
-   **Stock level:**
    Current stock level at the storage place.
-   **Del. ID:**
    Supplier's box ID (only if it has been entered at goods receipt).

## Stock Management - Prices
*Stock management > Stock management > Prices tab*

*Fig. K-50 Stock management - prices*

This tab shows the current prices for a stock article. During updates, orders, purchase orders and stock rebookings are taken into account.

> **Prerequisite**
> The average purchase price (average PP) is only calculated and shown if the checkbox **Determine average purchase price** has been enabled in the company data.
>
> ⇨ Master Data, "Average PP: The average purchase price will be recalculated in the following cases:" on page B-955

The fields in the lists are described in detail in connection with the Stock Article tab.
⇨ "Stock Management - Stock Articles" on page K-74

### Purchase prices
**Lowest price** The lowest price this article has been purchased at.
**Max. price** The highest price this article has been purchased at.
**Last price** The latest price this article has been purchased at.

### Stock value
The current stock prices are shown in this column. They are the result from the respective price and the quantity.

### Calculation of the average price (average PP)
By selecting an option, determine which stock sizes should be taken into account on this list for the calculation. This setting only makes sense for lite with different stock sizes.

-   **Only this article:**
    For the calculation only the displayed article in the selected size is taken into account. The PP history of the current article is displayed.
-   **All sizes:**
    For the calculation all dimensions of the displayed glass are taken into account. The PP history of all dimensions of the article is displayed.

The average PP is calculated for each goods receipt, regardless of how it has been booked. Goods issued only reduce the stock. The list is reduced by archiving and auditing.

The first data record shows the opening stock and the original price. Underneath you will find the goods received and issued (minus sign). If goods have been received as a result of a stock P.O., the P.O. number and the P.O. item are furthermore displayed.

The average PP is updated during entering or changing purchase orders. It is determined by taking the total quantity into account.

**Example:**

| | | | |
| :--- | :--- | :--- | :--- |
| 100 pieces | on stock | each 15.00 € | 1500.00 € |
| 40 pieces | new booking | each 18.00 € | + 720.00 € |
| | | **=** | **2200.00 €** |

2200.00/140 pcs. = 15.86 €

Automatic surcharges that are listed in the purchase orders, e. g. energy and transportation surcharge, are also included in the calculation.

### Overview
The respective average prices are shown as history. This way, you can easily monitor price developments. Details displayed:

-   **Date:**
    Date of the last update.
-   **Quantity [QU]:**
    Quantity issued or received and quantity unit.
-   **Price/PU:**
    Purchase price per price unit at the time of booking.
-   **Stock on hand [QU]:**
    Stock on hand at the displayed date. If the average PP is shown for all dimensions, the stock on hand is always shown in sqm.
-   **Average price / PU:**
    Average price per price unit at the time of booking.
-   **P.O. / item:**
    Number of the purchase order and P.O. item.
-   **Stock value:**
    Stock value at the displayed date (calculation: purchase price * stock on hand).
-   **Type:**
    Type of booking that has caused the respective entry.

### Include in total PCH
You can determine whether the article should be included in the calculation of the total average price of all variations of this article.

- The article will not be considered for calculating the average price.
- The article will be included in the calculation.

### Average price
Current average price. Depending on the option for calculating the average PPs, the display for the current article or the display for all dimensions of the article applies.

> **Updating the display**
> The display of the average prices is updated for the respective stock article during archiving or invoice check. As a result, the view remains clearer. A+W Business assumes that the prices will not be changed anymore after these processes. However, if you still change prices after one of the processes, these changes are not included in the calculation of the average price.

## Stock Management - Supplement
*Stock management > Stock management > Supplement tab*

*Fig. K-51 Stock management - supplement*

On this tab reservations for a selected stock article are shown.
The fields in the lists are described in detail in connection with the Stock Article tab.
⇨ "Stock Management - Stock Articles" on page K-74

### Reservation
The fields in this area are enabled for individual customers only.

**Customer** Number and name of customer for whom the selected stock article is reserved.
**Fully locked** Not currently used.
**Exclusive reservation** Not currently used.

### Supplier
**Supplier** Number and name of supplier from whom the stock article is ordered.

### Remark
**Product related, Storage location related** You can enter additional information for each stock article and each storage location, e. g. when and from which supplier glass/boxes were supplied, so that older deliveries are used first.

## Stock Movement
*Stock management > Stock movement*

You can manually book withdrawals and additions for stock articles, correct stock figures, rebook storage locations and resolve boxes.
This section provides information on the following subjects:

-   "Options Menu" on page K-83
-   "Stock Movement" on page K-83

### Options Menu
*Stock management > Stock movement*

The following entries are displayed:

-   **Protocol at shut down:**
    When exiting the dialog, the stock history is automatically shown.
-   **Stock > 0:**
    Only stock articles with a stock on hand of over 0 will be shown.

### Stock Movement
*Stock management > Stock movement*

Additions and dispatches of stock articles are automatically booked: for receipt of goods by delivery and for goods issued by orders. You can manually book additions or dispatches in the Stock Movement dialog, e. g to correct stock quantities.

Dialog Stock Movement offers the following tabs:

-   Stock Movement - Dispatch, Addition
-   Stock Movement - Transfer
-   Stock Movement - Number of Sheets
-   Stock Movement - Open Boxes

## Stock Movement – Dispatch, Addition
*Stock management > Stock movement > Dispatch tab, Addition tab*

*Fig. K-52 Stock movement – dispatch, addition*

You can manually book goods issued and received on the Dispatch and Addition tabs. You can select a certain stock article and enter the corresponding data. If you have all stock articles displayed you can select the requested article on the Storage places list. The fields in the Change stock on hand section are then enabled.
⇨ Tutorial, "Stock Management for Boxes" on page K-48

If you have activated the option Protocol at shut down, the stock history is automatically shown on the Table tab when you close the dialog.

> **Manually enter addition of boxes**
> Since every box is kept with its own ID, you can enter additions of boxes only via Goods Receipt or Stock Management. In Stock Management, you create the box as a new stock article.

### Stock product
**Product** Number and name of the stock article.

**ID no.** You can only book stock dispatches via the ID no. Additions of boxes must be defined in Stock Management so that you can enter a new ID. Boxes added have to be defined in inventory management in order to enter a new ID.

**Content** If you have selected a box, then its content is displayed. If a box with an ID no. that has already been allocated to an order is to be delivered or opened, a message is displayed. This prevents that negative stock is created by the subsequent printing of the delivery note or invoice.

**Storage location** Storage location that the stock article has been allocated to.

> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.

**Average purch. price** The average purchase price is only shown if the function has been activated in the master data.
⇨ Master Data, "Calculate purchase price" on page B-955

### Change stock on hand
**Quantity** Enter the quantity that is to be booked out or in to stocks in pieces. If you go below the minimum stock when booking articles out of stock, a warning message is displayed.

**Width, height** These fields are only filled with quantity unit sqm if it involves stock sizes.

**Assessment price** Enter the purchase price at which the goods received were supplied.

**Booking date** The current date is shown automatically. It can be changed if required.

**Remark** You can enter a remark or select from the combo box. The remark will be displayed in the stock history.
Use the button to add a new remark to the list.
⇨ "Remark (Stock Movement)" on page K-89

### Storage locations
-   **Color:**
    The color is only shown for variations.
-   **Width, Height:**
    Dimensions are only shown if the product has been defined as a stock size or box.
-   **Contents:**
    Value 1 is shown for stock articles and stock sizes and the number of sheets for boxes.
-   **Storage location:**
    Storage location in the order of level 1 through 4.
-   **ID no.:**
    Box ID (manual booking or from goods receipt).
-   **Stock on hand:**
    Current stock
-   **QU:**
    Quantity unit with which the product is kept in stock.
-   **Del. ID:**
    Supplier's box ID.

## Stock Movement – Transfer
*Stock management > Stock movement > Transfer tab*

*Fig. K-53 Stock movement - transfer*

Use this tab to book a stock article to a different storage location. When you transfer a storage location, the entire stock of this storage location is always booked to the other storage location.

⇨ Tutorial, "How to transfer the storage location" on page K-64

The fields in sections Stock product and Storage locations are described under tab Dispatch.
⇨ "Stock Movement - Dispatch, Addition" on page K-84

### Storage location
**Storage location** Displays the current storage place. You can allocate a different storage place. The combo box lists all stored storage places.

> **Storage location <n.e.>**
> Even if you have defined your own storage locations, storage locations <n.e.> will remain and can be booked.

## Stock Movement - Number of Sheets
*Stock management > Stock movement > No. of sheets tab*

*Fig. K-54 Stock movement - number of sheets*

Use this tab to correct the content of boxes.
⇨ Tutorial, "How to correct the number of sheets in a box" on page K-65

The fields in sections Stock product and Storage locations are described under tab Dispatch.
⇨ "Stock Movement - Dispatch, Addition" on page K-84

### Content change
**Content** Only if a box with an ID has been selected, the number of sheets that should in the box, is displayed. You can correct this value.

## Stock Movement – Open Boxes
*Stock management > Stock movement > Open boxes tab*

*Fig. K-55 Stock movement - open boxes*

Use this tab to resolve boxes so that the individual sheets are available for production. During this process, the box is booked out of the inventory and the number of sheets is booked to the inventory of the stock size.
⇨ Tutorial, "How to open a box" on page K-66

> **Book box content to a different storage location**
> When you open a box, its content is booked to the same storage location of where the box is located. If you want to transfer the content, you must book it out of the previous storage location and subsequently, book it to the new storage location.

The fields in sections Stock product and Storage locations are described under tab Dispatch.
⇨ "Stock Movement - Dispatch, Addition" on page K-84

### Open box
If a box with an ID no. that has already been allocated to an order is to be delivered or opened, a message is displayed. This prevents that negative stock is created by the subsequent printing of the delivery note or invoice.

**No. of boxes** Number of boxes that are to be opened.

**Different contents** The number of sheets is shown only if you have selected a box. You can correct this value.

## Remark (Stock Movement)
*Stock > Stock movement > [Remark]*

*Fig. K-56 Remark concerning stock movement*

Use this dialog to store remarks that are offered for selection in the Stock movement dialog. If you leave the first line blank you can also delete an allocated remark.

## Search
*Stock management > Search*

You can retrieve the stock on hand by individual stock articles or by product groups.

> **Set filter**
> If no filter is set, no data will be displayed.

The dialog is described in detail in the Sales part.
⇨ Sales, "Stock Info" on page C-736

Dialog Stock search offers the following tabs:

-   Stock Search - Stock Search
-   Stock Search - Future Stock on Hand

## Stock Search – Stock Search
*Stock management > Search > Stock search tab*

*Fig. K-57 Stock search - stock search*

Use this tab to display the current stock on hand, reserved quantities and future stock on hand for stock articles.
⇨ Tutorial, "Stock control mode and reservation" on page K-12

### Selection
The fields are only enabled in selection mode.

**Product** Product number by which the product has been entered in the master data.

**Type** Product type this product has been assigned to in the master data.

**Group** Product group this product has been assigned to in the master data.

**ID** Identification number by which the stock article has been entered in the stock, e. g. for a box.

**Category** If you have defined stock categories in your company, these can be used as filters.
⇨ Master Data, "Stock Categories" on page B-738

**Color** (Color) variations that have been defined for the selected product.

**from, to PGR** You can also enter product groups or product group areas. The overview then displays all the products of the selected product groups.

**Thickness / width / height** These details are transferred from stock management. Width and height are only displayed if the selected item has been entered as a stock size or box, including the corresponding details.

**Storage location** If you are using different storage locations, the storage location of the selected item will be shown, including all defined levels.
⇨ Master Data, "Stock Definition" on page B-736

**Del. ID** Identification number of the shipment from stock management. It is not identical with the entry in the ID column.

**Remark** Information stored for the selected item when delivered.

**Contents from, to** You can use the contents as a search criterion in the selection mode, e.g. all boxes with a content of 50 pieces. Contents = 1 always means stock size.

**Availability** Displays the available pieces.

### Filter options
If no filter is set, no stock will be displayed. A filter is set if the corresponding checkbox is ticked. The following filters are available:

-   **Stock articles:**
    Stock articles will be displayed.
-   **Boxes (contents > 1):**
    Boxes with a content of > 1 will be displayed.
-   **Stock sizes (contents = 1):**
    Stock sizes will be shown. Display of the quantity (= 1) helps to distinguish boxes of identical sizes.
-   **Group boxes by storage location and supplier:**
    Only one line is displayed per storage location and supplier.
-   **Articles without sizes:**
    Even stock articles for which no sizes have been entered will be shown.
-   **No boxes with ID:**
    Boxes entered with an ID at receipt of goods shall not be shown.
-   **Minimum qty > 0:**
    Only stock articles with a minimum quantity of over 0 should be displayed.
-   **Stock > 0:**
    Only stock articles with actual stock should be displayed.
-   **Stock = 0:**
    Only stock articles without stock should be displayed.
-   **Stock < 0:**
    Only stock articles that have been reserved, but are without stock, should be displayed.

### Print options
You can define the sorting of the list for printing purposes. The appropriate checkboxes will be enabled with the selected option. You can then additionally define where a subtotal will be printed.

The following entries are displayed:

-   **Group by product no.:**
    The checkbox Subtotal by product group is enabled.
-   **Group by product type/group:**
    The Subtotal by superior product group checkbox is enabled.
-   **Group by product group:**
    The Subtotal by main product group checkbox is enabled.

### Overview
The overview lists all products that have been selected by means of the search. The columns provide details on the stored products.

The reserved quantities will be updated as soon as a corresponding item has been saved in the order. The details in column Stock on hand will be updated when a delivery note is issued.

The entries in the hit list are identified with the following colors:

-   **Black:**
    Quantity-based stock article
-   **Blue:**
    Stock article not quantity-based
-   **Red:**
    No stock article: articles that are not kept on stock.
    This applies also to products which are no longer available, or which show negative quantities. Negative quantities occur if the stock on hand and the order quantity minus the reserved quantity <= 0.

### Totals
The totals of the selected products are shown. If you have selected a PGR with different products, the totals of the selected product are shown.

## Stock Search - Future Stock on Hand
*Stock management > Search > Future stock on hand tab*

*Fig. K-58 Stock search - future stock on hand*

Use this tab to check whether the replacement times for a certain product are sufficient to delivery an order in accordance with the schedule. The color red shows that scheduled dates cannot be met. Yellow indicates that the replacement time is sufficient if the purchase orders are received on time.

The replacement time results from the delivery time that has been defined in the supplier file for the article and the supplier's route days that are defined in route management.

### Preview up to
The preview always starts with the current date. Set the number of days for the preview in the company data, e. g. 14 days.
-   The list at the top shows the data for each selected product in one line.
-   The list in the center shows the stock on hand per day.
-   The list at the bottom displays details on the selected product.

The lines are red if production is impossible because the reservations exceed the stock on hand.

In order to increase the performance you can restrict the preview display by the following settings:

-   You can remove certain articles from the stock preview and availability check in dialog **Product management > tab Stock/Purchasing > No availability check** checkbox, by disabling the availability check for these articles.
-   In the **Company data** dialog you can set the time period displayed in the preview.
-   You can link several stock sizes together in the dialog **Stock management** so that the stock check is only executed for the defined main stock article.
    ⇨ "Main article" on page K-75

## Stock P.O.
*Stock management > Stock P.O.*

Use this dialog to check all suggested stock P.O.s and transfer them to Purchasing.

This section provides information on the following subjects:

-   "Order Pool Menus" on page K-96
-   "Order Pool" on page K-99

### Order Pool Menus
By using the menus you can have the date fields updated automatically and open other dialogs additionally.

This section provides information on the following subjects:

-   "Functions Menu" on page K-96
-   "Options Menu" on page K-97

### Functions Menu
*Stock management > Stock P.O. > Functions menu*

This menu can be used to open other dialogs without closing the P.O. transfer. The following entries are displayed:

-   **Change supplier/delivery date:**
    Opens the dialog Change supplier and delivery date.
    ⇨ "Change Supplier and Delivery Dates" on page C-657
-   **Marking options:**
    Opens dialog Marking options.
    ⇨ "Marking Options" on page C-658
-   **Supplier prices:**
    Opens dialog Price comparison.
    ⇨ "Price Comparison" on page C-659

### Options Menu
*Stock management > Stock P.O. > Options menu*

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

> **Activated options after opening the dialog**
> Please note that changed options will only become effective the next time you open the dialog.
> If an activated option has started a check, opening the document can be delayed. The extent of the delay depends on the performance of the computer. The following descriptions represent the activated option.

### Transfer group
-   **Order-related transfer:**
    Purchase orders are transferred by order. Collective P.O.s can be created if this option is disabled.
-   **P.O. number = order number:**
    This option is only available if the option Order-related transfer has been enabled.
-   **Order pool by user:**
    You can create separate order pools for every user.

### Delivery date group
-   **Check delivery date:**
    The delivery date is checked automatically. The system will inform you if you have changed a delivery date to a date which is not a route day.
-   **Consider supplier's route:**
    If the delivery date for the P.O. is not a route day, a message to that effect will be issued. This requires that supplier's routes have been defined in the master data.
    ⇨ Master Data, "Routes" on page B-861
-   **Determine lead days based on PGR combinations:**
    If lead days have been defined for PGR combinations, these will be used to calculate the delivery date.
    ⇨ Master Data, "Lead days" on page B-567

### Product name group
-   **Product names as per the supplier file:**
    The names of the ordered products are adopted from the supplier file.
-   **Product names as per master data (internal P.O.):**
    For internal purchase orders, the names of the ordered products are loaded from the product master data.

### Other group
-   **No saving of costs:**
    Costs are not written back to the purchase prices of the order.
-   **Consider size surcharges:**
    Size surcharges will be transferred with the P.O.
-   **Always set print code for processing:**
    On the P.O. processing steps shall always be printed. If this option is disabled, the print codes are adopted from the order into the P.O. without any changes.
-   **Statistics PGR as per order:**
    The statistics PGR information is adopted from the order if different statistics PGRs have been defined for order and P.Ο.
-   **Business type as per order:**
    The business type is adopted from the order if different business types have been defined for order and P.Ο.
-   **Production preparation as per order:**
    The production preparation is adopted from the order if different production preparations have been defined for order and P.O.
-   **Consultant = user for new input:**
    The P.O. automatically shows the name of the user logged on to A+W Business.
-   **Check change of status:**
    The query concerning the change of status is displayed.
-   **Repeat transfer only up to lock status:**
    Purchase orders can be transferred several times but only until lock status has been reached.

### Further settings group
-   **Settings:**
    Opens the Further settings dialog in which you can define information concerning printing texts and file attachments.

## Order Pool
*Stock management > Stock P.O.*

*Fig. K-59 Order pool*

In this dialog you can view all suggested purchase orders for articles that fall short of the minimum stock. The order quantity is calculated by the quantity that has been defined in the dialog Stock management.

After the transfer, the purchase orders are created and can be printed and sent.

⇨ Tutorial, "Stock P.O. of boxes" on page K-49
⇨ Tutorial, "Manual and automatic stock P.O." on page K-41

### Storage location
**Warehouse, Corridor, Shelf, Tray** You can restrict the display to individual storage locations. Please remember that stock articles may be booked to storage location <n.e.>. If you do not restrict the selection, purchase order suggestions are displayed for all articles that fall short of the minimum stock.
The name of the storage locations can be changed in the master data.

### Overview
The data relating to the purchase order suggestions is displayed in the overview. You can select a different supplier and view a price comparison.

-   **Supplier:**
    The supplier is adopted from the supplier file. You can change the name if no supplier has been entered or if your standard supplier has supply problems.
-   **Article/color:**
    Number and - if applicable - variant of the product to be ordered.
-   **ID no.:**
    Box ID (manual booking or from receipt of goods)
-   **Storage location:**
    Storage location where the stock on hand of the stock article falls short.
-   **Qty:**
    Quantity to be ordered. The standard purchase order quantity is multiplied until the minimum stock on hand is exceeded. You can also change the value directly on the list.
-   **Width, Height:**
    Size of the lite to be ordered.
-   **Contents:**
    Contents are only shown for boxes.
-   **Deliv. supplier:**
    The supplier's delivery date is determined based on the entries in the supplier file. You can change the date if your standard supplier has supply problems.
    ⇨ Sales, "Change Supplier and Delivery Dates" on page C-657
    ⇨ Sales, "Price Comparison" on page C-659

**Item for** The purchase order suggestions are displayed in different colors:
-   **Red: internal order:**
    Internal orders are production orders that are created to fill stock on hand. The suggestion is automatically created if the corresponding option for the product has been enabled in the supplier file.
-   **Blue: Inquiry:**
    Inquiry to a supplier e.g. to ask for prices and delivery times.
-   **Green: Delivery might not be on time:**
    The current date is automatically set as the delivery date. As a result, the delivery is usually not possible on time. If you change the date the color for the entry changes to black.

### Target Number Manager
**Employee** Name of the employee logged in to A+W Business or who has set up the Number Manager. If you create a new Number Manager you can allocate it to one particular employee.

**Name** Name of the target Number Manager for the purchase orders. A new Number Manager will be created when you enter a new name.
