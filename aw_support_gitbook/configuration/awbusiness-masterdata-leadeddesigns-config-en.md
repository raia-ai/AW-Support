---
title: "EN_AWBusiness_Master_Data_9_6-2"
source: "EN_AWBusiness_Master_Data_9_6-2.pdf"
tags: ["A+W Business", "Master Data", "Leaded Designs", "Cost Calculation", "Pricing", "Production Data Transfer", "Marginal Income", "System Configuration"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial section from the A+W Business Master Data guide, providing additional information on various features. It covers patterns for leaded designs, monitoring system changes, transferring master data to A+W Production, and detailed methodologies for price calculations, including mixed, French, and cost-plus-surcharge models. "
long_description: "This document, labeled 'Tutorial 2', is an excerpt from the A+W Business Master Data manual. It provides detailed supplementary information on several advanced configuration and data management topics within the A+W Business software. The first section illustrates the 14 default patterns available for leaded glass designs, such as Gothic, Stuart, and Windsor. The next major section details the 'Monitoring of Changes' feature, which allows administrators to track modifications to customer, supplier, price, and discount data at a granular level. It explains how to configure monitoring settings, define triggers, and analyze change history. A significant portion of the document is dedicated to the integration between A+W Business and A+W Production, outlining the process for transferring production-relevant master data. It provides extensive tables that map fields between the two systems for product management, glass types, cutting tables, and more. The final part of the tutorial focuses on various pricing and calculation methods. It covers 'Mixed Calculation', 'French Pricing', and a comprehensive guide to 'Cost and Surcharge Calculation'. This includes defining production costs, overheads, marginal income limits, and a complex, step-by-step example of an Insulated Glass (IG) unit cost calculation, breaking down the costs of lites, spacers, gas, and other consumables."
---

---
## Additional Information

### Patterns for Leaded Designs
The following patterns are defined by default for leaded designs:

| Type | Name | Type | Name |
| :--- | :--- | :--- | :--- |
| Type 1 | Gothic | Type 2 | Stuart |
| Type 3 | Diamonds | Type 4 | Cumberland |
| Type 5 | Hanover | Type 6 | Jacobean |
| Type 7 | Northumberland | Type 8 | Queen Anne |
| Type 9 | Queen Caroline | Type 10 | Rectangles |
| Type 11 | Square Gothic | Type 12 | Diamond Pillar |
| Type 13 | Westmorland | Type 14 | Windsor |

*Fig. B-78: Leaded design patterns*

---

## Monitoring of Changes
Changes in customer-, supplier-, price-, and discount management can be monitored. The individual dialogs offer the menu **History** for this purpose.

For all database tables accessed by a dialog you can define how changes shall be monitored. Detailed monitoring is possible if the tables in question are monitored on field level.

Monitoring of changes is set and enabled for every dialog separately. Generally, analysis shows the changes for the selected record. Apart from that, analysis can be based on number manager, or on all records.

Settings and analyses always refer to the currently set runtime mode. In price management for example, this applies to the analysis of changes of standard prices, customer prices, customer group prices, etc.

Apart from that, analysis can be restricted by various filters, e.g. to a certain user or period.

### Monitoring of Changes - Management
**Path:** `Utilities > System > Monitoring of changes`

*Fig. B-79 shows the "Monitoring of changes - management" dialog, which includes sections for General settings, Table settings, and Field settings. It allows users to define which database tables and fields are monitored for changes.*

This dialog serves to define the changes to be monitored and recorded. This function is available only if you have acquired the appropriate licenses.

### Menu Initialization
The entry **Initialize analysis** prepares the analysis. After that, it can be displayed or printed via menu `History > Analysis`.

### General settings
- **Language**: Output language for analyses.
- **Define trigger**: This button is available only if:
    - monitoring of changes has been initialized.
    - the setting for a table or a field has been edited.

> The database triggers for monitoring have to be created again after settings were redefined or changed. This can be started by hand (recommended). This is automatically done when you close the dialog. This process can take some time.

### Table Settings
> **General settings**
> If the settings for the monitoring of changes are made in `Utilities > System > Monitoring of changes - management`, they will apply to all available tables. The settings can also be made for the present dialog.

- **Name**: Name of the table. It can be changed. The names will appear in the analysis. If monitoring is active, all fields of this table will be shown in section **Field Descriptions**.
- **History**: The combo boxes in column **History** offer the following settings:
    - **None**: Changes will not be monitored. This setting means that no analysis will be shown.
    - **Complete**: Changes are monitored for the entire database table. You have to select this setting for all price tables in price management if you want to see the former status as well.
    - **Detailed**: Changes will be monitored by field.

### Field Settings
If the table is monitored on field level, you can define the fields that trigger the monitoring.

- **Name**: Field name. It can be changed. The names will appear in the analysis.
- **Refers to**: Changes are detected by means of the key columns of the individual tables. If the key fields are reference fields, this column shows the reference table.
- **Display column**: The reference table can show a name in addition to the key value. Valid names can be selected from the combo box in this column. The field **Price key** for instance refers to the database table **Price keys**. The Price key number or the **Name** from this table can be displayed. If there are no names apart from the key itself, this combo box remains blank.
- **On/off**: This column and the checkboxes are displayed only if the entry **detailed** has been selected in the table settings in column **History**. The analysis only shows the fields which have been enabled by ticking these checkboxes. A maximum of 80 fields can be displayed.
- **Selection**: The two selection buttons can be used to enable or disable all checkboxes in column **on/off**. After that, individual checkboxes can be enabled or disabled. The options can be enabled or disabled per order.

---

## A+W Production
Production-relevant data can be transferred to A+W Production.
A+W Production uses the same master data as A+W Business. Any changes of master data must be transferred to A+W Production. The product number guarantees that both programs use the same product. A+W Business sets a processing code for every product. This creates the so-called production bills of material for the transfer.

### Transfer File
An ASCII file is written in directory `AWPOOL` for the transfer. You define the parameters to be transferred for this file.

> **Example**
> - Customized logo number
> - Relevant text codes
> - Edge protection per order (aluminium tape, IG only)
> - Spacer (via external keys as per product definition)
> - Gas code

### Master Data Transfer from A+W Business to A+W Production
The following data can be transferred if the supplement **Master Data Transfer** has been installed. Without this supplement, identical data have to be entered in both programs.

**Tab. B-10: Transferring master data from A+W Business to A+W Production**

| Dialog in A+W Business | Field | Dialog in A+W Production | Field |
| :--- | :--- | :--- | :--- |
| **Product Management** | | | |
| Tab **Product**: | Name (1-3)<br><br>for product types:<br>- HW<br>- Annealed<br>- Tempered glass<br>- IG<br>- LAMI<br>- CR | Article master data: | Name<br>Article text (1-2)<br>Checkbox **Release part active** |
| | Grill thickness | Processing article: | Thickness |
| For processing | ProductGroup<br>Quantity unit | | Category<br>Time s/ |
| *Short info and product info will not be transferred* | | | |
| *The grinding group is loaded from A+W Production* | | | |
| Tab **Production**: | Sense of pattern | Glass types: | Structure |
| Tab **Stock/Purchasing**: | Procurement type | Article master data: | Procurement type |
| | Automatic Cutting | Glass article: | Can be optimized |
| | Technical article number | | Article code |
| Tab **A+W Production**: | Glass type<br>Grinding group<br>Shape<br>Trim (t, b, r, l)<br>Max. Subplate Width<br>Min. distance X-Y cuts<br>Seq. opti.<br>Pattern position<br>Coating position | Article master data:<br><br>Glass article: | Glass type<br>Grinding group<br>Shape trim<br>Trim<br>Max. subplate width<br>Min. distance X-Z<br>Opti rank<br>Pattern position<br>Coating position |
| *The transition time will not be transferred (field remains blank)* | | | |
| **Glass types** | Name<br>Product group<br>Glass type group<br>Structure<br>Coating<br>Product group<br>Name | Glass types:<br><br>Article master data: | Name<br>Article type<br>Glass type group<br>Structure<br>Coating<br>Article type<br>Name |
| **Glass type - jumbos** | Jumbo width / height<br>Priority for opti.<br>Subplate flag:<br>- X direction<br>- Y direction<br>- at choice | Stock sizes: | Width / Height<br>Price<br>Subplates |
| **Jumbo cutting tables**| Loader code<br>Quantity | Stock sizes: | Loader code<br>Quantity |
| **Cutting tables** | | | |
| Tab **Values**: | Name<br>Width / Height<br>Reference point<br>Z cut<br>Start of breakout<br>Racks per cycle<br>Special<br>Rank | Tables: | Description<br>Width / Height<br>Reference<br>Z cut<br>Start of breakout<br>Racks/Cycle<br>Special<br>Rank |
| Tab **Settings**: | Auto breakout<br>Automatic loader<br>Shapes<br>LAMI<br>Edge deletion<br>Manual cutting<br>max. subplate width may | Tables: | Auto breakout<br>Automatic loader<br>Shapes<br>LAMI<br>Edge deletion<br>Manual cutting<br>Maximum subplate width |
| Tab **Cuts**: | Min. dist. Y-Y cuts<br>Min. dist. X-X cuts<br>Max. dist. Y-Y cuts<br>Max. dist. X-X cuts | Tables: | Min X-X<br>Max X-X<br>Min Y-Y |
| *Entries for the maximum waste will not be transferred.* | | | |

### Processing Catalog
The defined processing catalogue contains all processing types and the necessary parameters. It serves as a central link between the existing programs of A+W Software GmbH.

This way, the processing steps including all related data can be transferred from **A+W Business** to **A+W Production** or via OrderXML.

For quick input of recurring, complex combinations of processing steps you can add a processing macro created by **Shaping & Nesting**.

**Additional information**
- ⇨ Software Reference, "Product Management - A+W Production" on page B-619
- ⇨ Software Reference, "Company Data – Production" on page B-983
- ⇨ Sales, "Parameters" on page C-467

---

## Mixed Calculation
For calculating customized prices, you can use mixed calculation instead of a replacement surcharge. This calculation type is used in Austria.

Up to three products can be combined to calculate a mixed price. For calculation, you need to define the (customized) price table to be used.

The calculation factors for mixed price calculation are entered in company data. You can also define if IG mixed calculation shall permit a search for discounts and/or individual prices.

The search for individual prices or discounts is disabled for mixed calculation by default.

> **Example**
> - **Basic price double IG =**
>   50% IG price table 1 + 50% IG price table 2.
> - **Basic price triple IG =**
>   50% IG price table 1 + 80% IG price table 2 + 50% IG price table 3.
>
> The price for the first lite of the IG unit is loaded from IG price table 1 and for the second lite of the IG unit, from IG price table 2. For triple IG, the price of the third lite is loaded from IG price table 3.

**Additional information**
- ⇨ Software Reference, "Mixed Price Calculation" on page B-696
- ⇨ Software Reference, "Mixed calculation factors" on page B-930
- ⇨ Software Reference, "Search discounts for mixed IG calculation" on page B-946
- ⇨ Software Reference, "Search individual price for mixed IG calculation" on page B-947

---

## French Pricing
The French IG pricing method means that the IG price consists of the following elements:
- Basic price for IG assembly
- Individual prices of the lites

Special keys and rates are usually defined for this purpose. The prices of the individual lites are defined as usual. They must be entered in the same price key as the basic IG price. The price unit `<sqm+UP>` must be used for IG.

The products are entered as usual. A **Miscellaneous surcharge** for spacers is entered and allocated to the IG price.

> **IG and laminated glass**
> The option **IG and laminated glass single price calculation** must not be enabled in company data in connection with French pricing.
>
> ⇨ Software Reference, "IG + LG single price calculation" on page B-947

---

## Calculation

### Objectives
- Cost calculation elements.
- Entering the settings for prime cost calculation.
- Defining the marginal income calculation.

### Benefits
- The prime cost is set globally and is taken into account for calculating the marginal income and the purchase prices.
- The marginal income will be recalculated automatically if prices are changed in the document at item entry.

### Please note
- **Production costs**: Production costs consist of: Material-, machine-, and labour costs plus overheads.
- **Overheads**: The proportional shares for overheads are entered in company data.
- **Calculation**: Cost calculation is activated per rate (price list and key):
    - If only purchase price calculation is active in the rates, costs and surcharges will only be calculated up to cost price.
    - If calculation is enabled for the sales price rates, the sales price will be calculated as well.
- **Partial material costs**: Partial material costs are calculated from the quantity (including product-related waste) and the price per quantity unit.
- **Full material costs**: To the partial material costs, an overhead surcharge is added which takes the product's procurement type into account.
- **Marginal income**: For marginal income calculation, minimum and maximum values are defined per customer and product group. The current marginal income is calculated and displayed per document. The marginal income analysis determines the marginal income for any defined period.

### Marginal Income Limits
The marginal income is displayed in the order and only refers to the items of this order.

*Fig. B-80: Display of the current marginal income in the order and per item. This UI shows fields like Material cost, Time cost, DB Total/%, Total cost, Proceeds, and CM in %.*

The marginal income analysis can be used for checking and printing the marginal income for order items for a defined period. This analysis is started in module **Documents**.

*Fig. B-81: Analysis of Marginal Income. This is a table view showing a list of order items with columns for Order, Item, Customer, Product, PGR, CM in %, MI min, MI max, Item price, and Status.*

The minimum and maximum marginal income is defined per customer and product group in dialog **Marginal income limits**.

*Fig. B-82: Marginal income limits dialog. This UI allows users to: (A) Select the customer or customer group, (B) Select the product group, and (C) Enter the minimum and maximum marginal income limits as percentages.*

The limits are defined per customer or customer group (A). The analysis refers to a product group (B); you can choose all of the three levels (PGR, MPG, SPG).

For every combination of (A) and (B) you can define the percentage (C) for the upper and lower marginal income limits. This way you can easily check whether the marginal income for the customer or customer group lies within the required scope.

As the calculated prices can be changed in the actual order, a maximum and a minimum amount can be entered for the marginal income. This prevents gross miscalculations in case of manual pricing, e. g. a sales price that lies below the prime cost.

*Fig. B-83: Company data – standard marginal income. This UI screen shows the **Calculation** tab in company data where standard values are set. (A) Minimum marginal income and (B) Maximum marginal income can be set as defaults.*

For all customer/product group combinations which have not been explicitly defined, the standard values entered in company data on tab **Calculation** will apply.

---

## Cost and Surcharge Calculation
Cost/surcharge calculation determines the price per price unit. The prime cost shares defined in company data will be taken into account.

### Production costs
Production cost calculation is based on material-, machinery-, and labour costs. Add the overheads for material and special direct costs and you will get the full production costs.

Material overheads include the following procurement types:
- Purchase order
- Stock Withdrawal
- Production

To those, overheads for administration and sales are added. Add the proportional expected profit to get the sales price.

### Overheads include:
- **Non-wage labour costs**: e.g. costs for social security.
- **Sales overheads**: Cost which cannot be allocated to individual products, e. g. commission.
- **Administration overheads**: e.g. office rent, energy costs, administration staff, etc.
- **Profit margin**

The proportional shares for overheads are entered in company data.

*Fig. B-84: Company data – settings for cost calculation. This UI shows the configuration for (A) Surcharges for material costs (based on procurement type like Purchase, Stock withdrawal, Production) and (B) Surcharges for overheads (Ancillary labour costs, Sales overheads, etc.).*

These proportional surcharges (A, B) refer to the (net) purchase prices.
Cost calculation is enabled per rate (price list and key).

*Fig. B-85: Activation of cost calculation in the rates. This UI shows a list of price rates where checkboxes can be ticked for (A) Cost calculation for purchase price rates and (B) Cost calculation for sales price rates.*

If calculation in the rates is only enabled for purchase prices, cost and surcharge calculation will be performed only up to the price cost. If calculation is enabled for the sales price rates, the sales price will be calculated as well.

You can view the calculations for the current order in the document and in the items.

*Fig. B-86: Examples of calculation overviews. This figure shows two windows: (A) A summary calculation for an entire item, and (B) a detailed cost calculation for the BOM elements of that item, breaking down costs for each component like glass, spacer, and gas.*

These examples show the calculation for an item (A). The calculation for the BOM (B) can be checked at item entry. Prices which are included implicitly in a product will not be shown.

Calculation can be amended per item, e. g. for calculating certain extra costs with a different percentage or taking special costs into account.

*Fig. B-87: Overview: Item calculation. This UI allows for manual adjustments to an item's cost calculation, including (A) Adjustment of overheads and special surcharges, (B) Adjustment of expected profit, and (C) Input of special costs.*

Cost calculation for the individual items can be extended by special surcharges. If a surcharge is entered as a negative value, it represents a special discount on this item.

> **Machine and labour costs on the shop floor**
> The shares of machine and labour costs are calculated by means of the appropriate basic data from capacity planning. These cost factors are only available if A+W Business capacity planning has been released and if the shop floor reports the actual costs.

### Definition of Primary Cost Calculation
To calculate the primary costs for IG, enter the average consumption of auxiliary material such as Butyl, Thiokol etc. for every spacer.

> **Prerequisite**
> Consumption material to be entered in section **BOM product** have to be defined as products.

#### How to enter the settings for primary cost calculation
1.  Select menu `Master data > Products > Article > PP calculation`.
    Dialog **Calculation Settings** appears.
    ⇨ Software Reference, "Cost Calculation" on page B-645
2.  Go to the menu `Start > New` to switch to the input mode.
    *Fig. B-88: Costs Calculation dialog. This UI shows fields for defining primary costs, including (A) Spacer settings, (B) Cutback, (C) Volume of gas, and (D) Entries for BOM products.*
3.  Enter the article number of the spacer (A) to which the consumption of gas, drying agent, or edge seal shall be allocated. Detailed examples will be provided in the next session.
4.  Enter the required values in the fields:
    - **Cutback (single)** in mm (B)
    - **Expanded volume of gas** in liters (C)
5.  Go to the tab **BOM**.
6.  Go to section **BOM** and select a line with article number 0.
7.  Enter the product number, the consumption for this article, and the reference unit in section **BOM product** (D). The entries are displayed in section **BOM**.
8.  Select in the menu `Start > Save` to save the data. The data will be saved.

> **Cutback**
> **Cutback (single)** refers to the distance from the outside edge of the lite to the outside edge of the aluminium spacer. It is required for bending aluminium spacers.
> If the glass size is e.g. 1000 x 1000 mm and the cutback (single) 5 mm, the spacer size is 990 x 990 mm.

---

## Complex Example: IG Calculation
This example shows how primary cost calculation (purchasing) is set up for an in-house produced IG unit, and how it is shown in the order.

Calculation is described in the following chapters:
- Calculation of Lites
- Spacer calculation
- Gas Calculation
- Calculation of consumables

We have used no rounding, discounts or surcharges in this example to make it easy to understand the calculation.

### Display at item entry
*Fig. B-89: Display of purchase prices in the order. This screenshot shows an order item with a breakdown of its component costs.*

The purchase prices for an item can be displayed in menu **Display**. The values in this example are included in the following calculation:

**Tab. B-11: Purchase price calculation**
| Legend | Product | Price |
| :--- | :--- | :--- |
| 1 | 1st lite | + 8.57 |
| 2 | 2nd lite | + 10.91 |
| 3 | Consumables | + 3.68 |
| 4 | Spacer | + 1.60 |
| 5 | Gas | + 0.12 |
| 6 | **Unit cost** | **= 24.88** |

Calculation of numbers 1-5 is described in detail below.

### Calculation of Lites
Calculation of lites takes into account the purchase price from the allocated price table, the waste, and the rounding. No surface rounding has been defined in this example.

#### First lite
The purchase price from the price table is multiplied by the surface. In this example, height x width = 1 sqm. An amount allowing for the waste is added to the calculated value.

| PU | | (surface + waste) | |
| :-- | :-: | :-- | :-- |
| 8.24 | X | (1 + 4/100) | = 8.57 |
*Tab. B-12: Purchase price calculation for the first lite*

**Waste**
The price tables for sales and purchase prices are allocated in product master data, tab **Price/surcharges**, and the average waste is defined.

*Fig. B-90: Product master data – proportional waste, example: first lite. The screenshot highlights the 'Average waste' field set to 4%.*

**Price**
In the price table, enter the purchase price agreed with the supplier.

*Fig. B-91: Unit price of the first lite. The screenshot shows the price table where the net price is set to 8.57 per sqm.*

#### Second lite
Calculation of the second lite is also based on master data. The values can differ from the first lite.

| PU | | (surface + waste) | |
| :-- | :-: | :-- | :-- |
| 10.20 | X | (1 + 7/100) | = 10.91 |
*Tab. B-13: Calculation of the second lite*

As for the first lite, waste and price are defined in master data.

### Spacer calculation
In this example, the edge length is exactly 1000 mm. This results in a total spacer length of 4 m.

| PP spacers | | actual lin.m. | |
| :-- | :-: | :-- | :-- |
| 0.40 | X | 4 | = 1.60* |
*Tab. B-14: Spacer calculation*
*\*No. 4 in table "Purchase price calculation" on page B-545*

The price is also defined as a unit price in master data. In the price table, enter the purchase price per unit you have agreed with the supplier. In this example, it is 0.40 /lin.m.

### Gas Calculation
To calculate the gas, the defined volume of gas is multiplied with the spacer thickness.

| m³ | X | ASP/expanded gas volume | X | PP of gas (1 + waste/100) | |
| :-- | :-- | :-- | :-- | :-- | :-- |
| 1 | X | 12/21000 | X | 215.90/(1 + 0/100)* | = 0.12** |
*Tab. B-15: Calculation of gas*
*\*In this example, there is no waste for gas.*
*\*\*No. 5 in table “Purchase price calculation" on page B-545*

**Calculation basis**
Enter the expanded quantity of gas per cubic meter (without pressure, without cooling) in `Master Data > Products > Article > PP Calculation`.

*Fig. B-92: Basis for calculating the consumption of heat insulation gas. The screenshot highlights the 'Annealed quantity' field for gas, set to 21000.0000 m³.*

The price is also defined as a unit price in master data. In the price table, enter the purchase price per unit you have agreed with the supplier.

### Calculation of consumables
In addition to the lites, spacers and gas filling, you can define other material needed to produce an IG unit.

| | PU |
| :--- | ---: |
| Butyl PP | 2.2 |
| + Thiokol PP | 0.028696 |
| + PP drying agents | 1.4484 |
| | **3.68*** |
*Tab. B-16: Calculation of consumables*
*\*No. 3 in table "Purchase price calculation" on page B-545*

The following paragraphs show how the three individual amounts were calculated.

#### Calculation of Butyl
| PP Butyl | X | actual linear meters | X | Consumption per unit | |
| :-- | :-: | :-- | :-: | :-- | :-- |
| 100 | X | 4 | X | 0.0055 | = 2.20 |
*Tab. B-17: Calculation of Butyl*

Calculation of the consumption is based on the quantity per unit. In this example, 0.0055 kg per linear meter (of spacer) are calculated. The price is also defined as a unit price in master data.

#### Calculation of Thiokol
| Thiokol PP | X | actual lin.m. | X | Consumption per unit | |
| :-- | :-: | :-- | :-: | :-- | :-- |
| 1.17 | X | 4 | X | 0.0422 | = 0.028696 |
*Tab. B-18: Calculation of Thiokol*

Calculation of the consumption is based on the quantity per unit. In this example, this is 0.0422 kg per linear meter (of spacer). The purchase price per price unit is defined as a unit price in the price table.

#### Calculation of Drying Agents
| PP drying agents | X | actual lin.m. | X | Consumption per unit | |
| :-- | :-: | :-- | :-: | :-- | :-- |
| 8.50 | X | 4 | X | 0.0426 | = 1.4484 |
*Tab. B-19: Calculation of the drying agent*

Calculation of the consumption is based on the quantity per unit. In this example, this is 0.0426 kg per linear meter (of spacer). The purchase price per price unit is defined as a unit price in the price table.

**Additional information**
- ⇨ Tutorial 2, "Definition of Primary Cost Calculation" on page B-543
- ⇨ Software Reference, "Purchasing" on page B-955
- ⇨ Software Reference, "Company Data > Calculation" on page B-977
