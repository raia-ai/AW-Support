---
description: "EN-UM-AWEnterprise_10"
---


# Special Prices

---
## Calc. base, description

Selection of the calc. base with which the price is determined.
For prices that refer to a basic quantity, the quantity unit from the article master data is evaluated.
For scaled prices, the basic quantity from the order item is compared to the limit quantities of the price levels. The price is determined according to the price level that is achieved with this quantity:
-> Tutorial, "Calculation bases" on page C-563

1.  **Single price:**
    For price calculation, the level 1 price is used.
2.  **Scaled level:**
    The price level is determined that is specified in the conditions is used for price calculation.
    -> "Daily Conditions" on page C-828
    -> "Special Conditions" on page C-842
3.  **Quantity scale per item (BQU):**
    To determine the price level, the quantity of the item is determined using the basic quantity unit (BQU) of the article. The price is calculated in the order according to the price level that is achieved through the total quantity of the item.
    -> "Article prices - details" on page C-903
4.  **Quantity scale per unit (BQU):**
    The basic quantity in a unit of the item is determined for determination of the price level.
5.  **Units per item**
    The respective quantity of the individual items is determined for the price calculation.
6.  **Total quantity per order:**
    The total quantity of all items in the order is determined for price calculation.
7.  **Variants:**
    With this calculation base, the prices can be scaled depending on 2 dimensions, e.g. height and width. To determine the price level, the smaller dimension is compared to the first column, the larger with the second column. The price is calculated according to the price level with which the limit values of both dimensions are reached.
8.  **Variant scale:**
    This calc. base makes sense for glass doors.
    For this calc. base, the width of the glass door is compared to the value from the first column and the height of the glass door with the value from the second column. Here it is important that the dimensions are entered in ascending order, first according to the first column and then according to the second column. The price is calculated according to the price level with which the limit values of both dimensions are reached.

> **Variant scale vs. variant prices**
> For glass doors with standard dimensions, usual variant prices and for glass doors with special dimensions vector prices with the calc. base Variant scale are stored. If glass doors with standard dimensions are ordered, the variant prices are used. For special dimensions, A+W Enterprise determines the vector prices with the calculation base Variant Scale.

13. **Quantity scale/Package size:**
    This price type is used if a unit price for an article has a very low value that cannot be depicted with a precision of two places after the decimal point. These prices can also be scaled according to Quantity to. Depending on the configuration, the quantity specifications can be item quantities or item quantities in basic quantity units of the article.
    *Technical info: numeric field, DB field: kuartprs.part*

    **Example**
    The unit price for a sack with 1000 cork sheets is EUR 2.54.
    5 sheets are needed per lite. For an item quantity of 15 sheets, 75 sheets are needed.
    The item price is calculated as precise item price and then rounded to two places after the decimal point.
    75 pieces x 0.00254 € = 0.1905 €, after rounding, makes 0.19 €.

### Factor %

Specification of a factor by which the article price is multiplied. Using the factor, you can change the price calculation for the article without having to adjust all price levels, e.g. for a price increase. If you leave the field empty, the factor from the conditions applies according to the condition hierarchy.
*Technical info: numeric field, DB field: kuartprs.faktor*

**Example**

| Factor | Basic price | Final price |
| :--- | :--- | :--- |
| 100 | 20.00 € | 20.00 € |
| 80 corresponds to a discount | 20.00 € | 16.00 € |
| 150 corresponds to a surcharge | 20.00 € | 30.00 € |

### Price 1

Specification of the individual price. This price is calculated in the order is Indiv. price is specified or if the dimensions of the order item are smaller than the dimension or quantity specifications of all other price levels.
The field is locked if Quantity scale/package size is specified since with this calc. base, a quantity specification is required for each price level.
*Technical info: numeric field, DB field: kuartprs.preis1*

### Price type

Specification of to what the specified price refers:

*   **CU/BQU:**
    The price is calculated per basic quantity unit (BQU) from the article master data, e.g. per square meter, etc.
*   **CU/piece:**
    In the order, the price is calculated as fixed amount per piece in the item.

*Technical info: alphanumeric field, toggle field, DB field: kuartprs.ptyp1*

## Article prices - details

**Master data > Conditions -> Special prices > Article prices > <F2>**

On this dialog, you specify the details for the market partner-specific article conditions. In addition, you can specify surcharges and piece price rounding.

*(Image: Abb. C-206 Article prices - details. A dialog box titled 'Article Prices' showing conditions for a customer 'ABC Glass Company' and article 'A+W IGU 2x4'. Fields include Price Type, Surcharges, and a list of price levels with associated quantities and prices.)*

### Field descriptions

The fields in the header area are described for the Article Prices - Overview dialog:
-> "Article prices - overview" on page C-899

In addition, the following fields are displayed:

**Minim. calculat. ... QU**
Specification of the minimum quantity for which the price is calculated. The minimum quantity is specified according to the basic quantity unit in the article master data, e.g. area in square meters. If the area of the glass in the order item is smaller than the minimum calculation, the price for the minimum calculation is used.
-> Tutorial, “Price-relevant quantity" on page C-562
*Technical info: numeric field, DB field: kuartprs.minber*

**Round size ... mm**
Specification of the round size in mm for the price calculation of the article, e.g. 30 mm.
For the price calculation, the edge lengths in the order item are rounded up to the next higher length that is divisible by the specified round size in mm.
*Technical info: numeric field, DB field: kuartprs.massrund*

> **Example**
> 30 mm is defined as round size.
> The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 mm is 1020 mm.
> The price is calculated from the dimensions 1020 x 1020 mm = 1.04 square meters.

**Surcharge matrix**
Selection of a surcharge matrix for a general surcharge on the glass price.
-> "Surcharge matrices" on page C-807
*Technical info: numeric field, DB field: kuartprs.zumatnr*

**Size surcharge**
Selection of a size surcharge, e.g. small glass surcharge, overlength surcharge, etc. If the order item exceeds or underruns the specified limit value in the surcharge, the price is increased by the surcharge.
-> "Size surcharges" on page C-812
-> Tutorial, “Size surcharges" on page C-629
*Technical info: numeric field, DB field: kuartprs.grosszu*

**Offset surcharge vector**
Selection of the surcharge for the offsets for IG lites or LAMI lites.
-> Tutorial, "Step surcharges" on page C-633

**PU price CU**
Currently not used.
*Technical info: numeric field, DB field: kuartprs.ekpreis*

**Min.EdgeLength**
Specification of the edge length in millimeters for the price calculation. This size is used if the height or width of the glass in the order item is smaller than this minimum edge length.
*Technical info: numeric field, DB field: kuartprs.minkant*

**Min. price**
Specification of the minimum price. This price is charged if the calculated price in the order item is less than the specified minimum price.
*   Minimum prices for header articles are only evaluated for the pricing methods IG-Switzerland, IG-current (only with the calculation type Vector), PCD-LAMI, PCD-tempered, PCD-base glass, PCD-finished glass or PCD-prices.
*   Minimum prices for BOM subparts are only evaluated if for the header article the pricing method IG-current, PCD-LAMI, PCD-tempered, PCD-basic glass, PCD-finished glass or PCD-glass doors is selected and the subpart is an accessory item with the pricing method PCD prices-general.
*Technical info: numeric field, DB field: kuartprs.minpreis*

**Offs. from qty. ..., to qty. 2...**
Specification of the limit quantity per offset. Depending on the calc. base, from qty. or to qty. is displayed. The fields are locked if Indiv. Price is selected as calc. base.
*   **from qty.:**
    The specified price is used if in the order the quantity is greater than or equal to the limit value.
*   **to qty.:**
    The specified price is used if in the order the quantity is less than or equal to the limit value.
Depending on the calc. base, the limit value is interpreted as quantity, as quantity per basic quantity unit or as edge length.
You access the quantity fields up to level 20 with <F2>. If all 20 levels are created, you can store additional levels with <F2>.
*Technical info: numeric fields, DB fields: kuartprs.me2, kuartprs.me3, ... kuartprs.me20. kuartptab.mas1*

**(measurement 2)**
This field is only enabled if 11 Variant or 12 Variant Scale is selected as calc. base.
If in the order the edge lengths of the article are greater than or equal to the limit values, the price of this price level applies.
*Technical info: numeric fields, DB fields: kuartprs.mas2_2, kuartprs.mas2_3, ... kuartprs.mas2_20*

**Price**
Specification of the price per offset. Depending on the price type, the price is calculated per unit or per quantity unit.
If **Indiv. Price** is selected as calc. base, only the price of level 1 is used.
The field is locked if **Quantity scale/package size** is specified since with this calc. base, a quantity specification is required for each price level.
*Technical info: numeric fields, DB fields: kuartprs.preis2, kuartprs.preis3, ... kuartprs.preis20*

**Price type**
Specification of to what the specified price refers:
*   **CU/BQU:**
    The price is calculated per basic quantity unit (BQU) from the article master data, e.g. per square meter, etc.
*   **CU/piece:**
    In the order, the price is calculated as fixed amount per piece in the item.
*Technical info: alphanumeric fields, toggle fields, DB fields: kuartprs.ptyp2, kuartprs.ptyp3, ... kuartprs.ptyp20*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: kuartprs.vondat, kuartprs.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. You have to redefine the scaled discounts if you still want to work with these special conditions.

## Special variant prices

**Master data > Conditions > Special prices > Variant prices**

On this dialog, you specify prices for article variants that apply for a market partner, an object or an industry.
In the detail view, you create the conditions for the price calculation, e.g. discount levels, round size.
The market partner-specific variant prices have a higher priority than the general variant prices.
-> "Article vectors" on page C-742

The following views are available for this dialog:
*   "Special variant prices - overview" on page C-907
*   "Special variant prices - details" on page C-910

### Special variant prices - overview

**Master data > Conditions > Special prices > Variant prices**

On this dialog, you maintain prices for article variants that apply for a market partner, an object or an industry.
The market partner-specific variant prices have a higher priority than the general variant prices.
-> "Article vectors" on page C-742

**<F2>** Change to the detailed view.
-> "Special variant prices - details" on page C-910

*(Image: Abb. C-207 Special variant prices - overview. A dialog box titled 'Special Variant Prices' showing a table with columns for Article, Description, Var., Price Type, Factor, Price 1, and Type for a specific customer.)*

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom the common conditions should apply have to be assigned an industry.
*Technical info: numeric field, toggle field, DB field: spezvarprs.kondkz*

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: spezvarprs.kondnr*

**Article, Description**
Selection of the article for which the market partner-specific variant price should apply. The article has to be defined in the article master data as article with dimension or size variant.
*Technical info: numeric field, DB field: spezvarprs.artnr*

**fr PLCD**
Selection of the price list code (PLCD) starting from which the price data should apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: spezvarprs.plkz*

**Version**
Selection of the article variant for which the price applies.
*Technical info: numeric field, DB field: spezvarprs.varnr*

**Calc. base, Description**
Selection of the calc. base.
For prices that refer to a basic quantity, the quantity unit from the article master data is evaluated.
For scaled prices, the basic quantity from the order item is compared to the limit quantities of the price levels. The price is determined according to the price level that is achieved with this quantity:
*   **9 - Pieces per item:** To determine the price level, the number of pieces of the item is used.
*   **13 - Quantity scale/Package size:** This price type is used if a price for an article has a very low value that cannot be depicted with a precision of two places after the decimal point.
*Technical info: numeric field, DB field: spezvarprs.part*

> **Example**
> Article with unit price of 0.0254 EUR with quantity 100 = EUR 2.54 CU/piece.
> The unit price for a sack with 1000 cork sheets is EUR 25.40.
> 5 sheets are needed per lite.
> With an item quantity of 15 lites, 75 sheets are needed.
> The item price is calculated as precise item price and then rounded to two places after the decimal point.
> *   Calculation: 75 pieces x 0.0254 EUR = EUR 1.905
> *   after rounding = EUR 1.91

**Factor %**
Specification of a factor by which the variant price is multiplied. Using the factor, you can change the price calculation for the article without having to adjust all price levels, e.g. for a price increase. If you leave the field empty, the factor from the conditions applies according to the condition hierarchy.
*Technical info: numerisches Feld, DB field: spezvarprs.faktor*

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 corresponds to a discount | 20.00 € | 16.00 € |
> | 150 corresponds to a surcharge | 20.00 € | 30.00 € |

**Price 1**
Specification of the individual price. This price is calculated in the order is **Piece per item** is specified or if the quantity of the order item is smaller than the quantity specifications of all other price levels.
The field is locked if **Quantity scale/package size** is specified since with this calc. base, a quantity specification is required for each price level.
*Technical info: numeric field, DB field: spezvarprs.preis1*

**Price type**
Specification of to what the specified price refers:
*   **CU/piece:** In the order, the price is calculated as fixed amount per piece in the item.
*   **CU/BQU:** The price is calculated per basic quantity unit (BQU) from the article master data, e.g. per square meter, etc.
*Technical info: alphanumeric field, toggle field, DB field: spezvarprs.preistyp1*

### Special variant prices - details

**Master data > Conditions > Special prices > Variant prices > <F2>**

On this dialog, you create the scaled prices and a value for the round size for variants.

**<F2>** Change to overview.
-> "Special variant prices - overview" on page C-907

*(Image: Abb. C-208 Special variant prices - details. A dialog box titled 'Special Variant Prices' showing details for a specific variant, including Round Size, Factor, and a list of price levels based on quantity.)*

#### Field descriptions

The fields in the header area are described for the Variant Prices - Overview dialog:
-> "Special variant prices - overview" on page C-907

In addition, the following fields are displayed:

**Round size ... mm**
Specification of the round size in mm for the price calculation of the article, e.g. 30 mm.
For the price calculation, the edge lengths in the order item are rounded up to the next higher length that is divisible by the specified round size in mm.
*Technical info: numeric field, DB field: spezvarprs.massrund*

> **Example**
> 30 mm is defined as round size.
> The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 mm is 1020 mm.
> The price is calculated from the dimensions 1020 x 1020 mm = 1.04 square meters.

**from qty. ... to qty. ...**
Specification of the limit quantity per offset. Depending on the calc. base, **from qty.** or **to qty.** is displayed.
*   **from qty.:** The specified price is used if in the order the quantity is greater than or equal to the limit value.
*   **to qty.:** The specified price is used if in the order the quantity is less than or equal to the limit value.
Depending on the calc. base, the limit value is interpreted as quantity, as quantity per basic quantity unit or as edge length.
*Technical info: numeric fields, DB fields: spezvarprs.anz2, spezvarprs.anz, ... spezvarprs.anz5*

**Price**
Specification of the price per offset. Depending on the price type, the price is calculated per piece or per quantity unit.
*Technical info: numeric fields, DB fields: spezvarprs.preis2, spezvarprs.preis3, ... spezvarprs.preis5*

**Price type**
Specification of to what the specified price refers:
*   **CU/piece:** In the order, the price is calculated as fixed amount per piece in the item.
*   **CU/BQU:** The price is calculated per basic quantity unit (BQU) from the article master data, e.g. per square meter, etc.
If **Quantity scale/Package size** is specified as calc. base, you have to specify price levels.
*Technical info: alphanumeric fields, toggle fields, DB fields: spezvarprs.preistyp2, spezvarprs.preistyp3, ... spezvarprs.preistyp5*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: spezvarprs.vondat, spezvarprs.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific variant prices have to be redefined if you want to keep working with these conditions.

## Prices for colored articles

**Master data > Conditions > Special prices > Colored article**

On this dialog, you can display all market partner-specific prices for a colored article.
The article has to be defined in the article master data as colored article.
In the detail view, you create the conditions for the price calculation, e.g. price scales, minimum calculation quantity, round size.

The following views are available for this dialog:
*   "Prices for colored articles - overview" on page C-912
*   "Prices for colored articles - details" on page C-915

### Prices for colored articles - overview

**Master data > Conditions > Special prices > Colored articles**

On this overview, you maintain the market partner-specific prices for colored articles. These prices for colored articles have a higher priority than the general prices for colored articles.
-> "PCD prices for colored articles" on page C-777
The article has to be defined in the article master data as colored article.

**<F2>** Change to the detailed view.
-> "Prices for colored articles - details" on page C-915

*(Image: Abb. C-209 Prices for colored articles - overview. A dialog box titled 'Prices for Colored Articles' showing a table with columns for Article, Color, Price Type, and Price 1.)*

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
*Technical info: numeric field, toggle field, DB field: kufarbprs.kondkz*

**Market partner**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: kufarbprs.kunr*

**Article, description**
Selection of the colored article for which the market partner-specific price should apply.
*Technical info: numeric field, DB field: kufarbprs.artnr*

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: kufarbprs.plkz*

**Color**
Selection of the color variant for which the price applies.
*Technical info: numeric field, DB field: kufarbprs.farbnr*

**Calc. base, description**
Selection of the calc. base with which the price is determined.
For prices that refer to a basic quantity, the quantity unit from the article master data is evaluated.
For scaled prices, the basic quantity from the order item is compared to the limit quantities of the price levels. The price is determined according to the price level that is achieved with this quantity:
-> Tutorial, "Calculation bases" on page C-563

*   **1 - Single price:** For price calculation, the level 1 price is used.
*   **2 - Scaled level:** The price level is determined that is specified in the conditions is used for price calculation.
    -> "Daily Conditions" on page C-828
    -> "Special Conditions" on page C-842
*   **3 - Quantity scale per item (BQU):** To determine the price level, the quantity of the item is determined using the basic quantity unit (BQU) of the article. The price is calculated in the order according to the price level that is achieved through the total quantity of the item.
    -> "Article prices - details" on page C-903
*   **4 - Quantity scale per unit (BQU):** The basic quantity in a unit of the item is determined for determination of the price level.
*   **13 - Quantity scale/Package size:** This price type is used if a price for an article has a very low value that cannot be depicted with a precision of two places after the decimal point.
*Technical info: numeric field, DB field: kufarbprs.part*

> **Example**
> Article with unit price of 0.0254 EUR with quantity 100 = EUR 2.54 CU/piece.
> The unit price for a sack with 1000 cork sheets is EUR 25.40.
> 5 sheets are needed per lite.
> With an item quantity of 15 lites, 75 sheets are needed.
> The item price is calculated as precise item price and then rounded to two places after the decimal point.
> *   Calculation: 75 pieces x 0.0254 EUR = EUR 1.905
> *   after rounding = EUR 1.91

**Price type**
Specification of to what the specified price refers:
*   **CU/piece:** In the order, the price is calculated as fixed amount per piece in the item.
*   **CU/BQU:** The price is calculated per basic quantity unit of the colored article.
*Technical info: alphanumeric field, toggle field, DB field: kufarbprs.ptyp*

**Price 1**
Specification of the individual price. This price is calculated in the order is **Indiv. price** is specified or if the dimensions of the order item are smaller than the dimension or quantity specifications of all other price levels.
The field is locked for the price type **Quantity scale/Package size**.
*Technical info: numeric field, DB field: kufarbprs.peis1*

### Prices for colored articles - details

**Master data > Conditions > Special prices > Colored articles > <F2>**

On this dialog, you specify the conditions for the calculation of market partner-specific prices of a colored article, e.g. minimum calculation areas, round size, and scaled prices.

**<F2>** Change to overview.
-> "Prices for colored articles - overview" on page C-912

*(Image: Abb. C-210 Prices for colored articles - details. A dialog box for a specific colored article showing detailed fields like Round size, Minim. Calculat., Factor, and a grid for quantity offsets and prices.)*

#### Field descriptions

The fields in the header area are described for the Prices for Colored Articles Overview dialog:
-> "Prices for colored articles - overview" on page C-912
In addition, the following fields are displayed:

**Round size ... mm**
Specification of the round size in mm for the price calculation of the article, e.g. 30 mm.
For the price calculation, the edge lengths in the order item are rounded up to the next higher length that is divisible by the specified round size in mm.
*Technical info: numeric field, DB field: kufarbprs.massrund*

> **Example**
> 30 mm is defined as round size.
> The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 mm is 1020 mm.
> The price is calculated from the dimensions 1020 x 1020 mm = 1.04 square meters.

**Minim. calculat. ... units**
Specification of the minimum quantity that is calculated. Decisive is the quantity unit from the article master data. If the quantity in the order item is smaller than the specified value, this minimum calculation quantity is calculated.
-> Tutorial, “Price-relevant quantity" on page C-562
*Technical info: numeric field, DB field: kufarbprs.minber*

**Factor %**
Specification of a factor by which the market partner-specific article price is multiplied. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. If you leave the field empty, the factor from the conditions applies according to the condition hierarchy.
*Technical info: numeric field, DB field: kufarbprs.faktor*

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 corresponds to a discount | 20.00 € | 16.00 € |
> | 150 corresponds to a surcharge | 20.00 € | 30.00 € |

**Offset frm Qty 2 ... 10, to Qty 2 ... 10**
Specification of the limit quantity per offset. Depending on the calc. base, **from qty.** or **to qty.** is displayed. The fields are locked if **Indiv. Price** is selected.
*   **from qty.:** The specified price is used if in the order the quantity is greater than or equal to the limit value.
*   **to qty.:** The specified price is used if in the order the quantity is less than or equal to the limit value.
Depending on the calc. base, the limit value is interpreted as quantity, as quantity per basic quantity unit or as edge length.
*Technical info: numeric fields, DB fields: kufarbprs.me2, kufarbprs.me3, ... kufarbprs.me10*

**Price**
Specification of the individual price. This price is calculated in the order is **Indiv. price** is specified or if the dimensions of the order item are smaller than the dimension or quantity specifications of all other price levels.
The field is locked for the price type **Quantity scale/Package size**.
*Technical info: numeric field, DB field: kufarbprs.peis1*
*Technical info: numeric fields, DB fields: kufarbprs.preis2, kufarbprs.preis3, ... kufarbprs.preis10*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: kufarbprs.vondat, kufarbprs.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific variant prices have to be redefined if you want to keep working with these conditions.

## Muntin prices

**Master data > Conditions > Special prices > Muntin prices**

On this dialog, you create market partner-specific muntin prices. In the detail view, you create the conditions for the price calculation, e.g. minimum linear meters, minimum number of fields.
These muntin prices have a higher priority than the muntin prices from the muntin price classes.
-> "Muntin price classes" on page C-696

The following views are available for this dialog:
*   "Muntin prices - overview" on page C-918
*   "Muntin prices - details" on page C-921

### Muntin prices - overview

**Master data > Conditions > Special prices > Muntin Prices**

On this overview, you maintain the market partner-specific muntin prices.
These muntin prices have a higher priority than the muntin prices from the muntin price classes.
-> "Muntin price classes" on page C-696

**<F2>** Change to the detailed view.
-> "Muntin prices - details" on page C-921

*(Image: Abb. C-211 Muntin prices - overview. A dialog box titled 'Muntin Prices' showing a table with columns for Article, Calc. Type, Lin. Meter, Cross, Trim, and Fields.)*

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom the common conditions should apply have to be assigned to an industry.
*Technical info: numeric field, toggle field, DB field: kuspropr.kondkz*

**Market partner**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: kuspropr.kunr*

**Article, description**
Selection of the muntin article for which the market partner-specific price applies.
*Technical info: numeric field, DB field: kuspropr.artnr*

**fr PLCD**
Selection of the price list code (PLCD) of the item article starting from which the muntin price data applies.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: kuspropr.plkz*

**Calc. type, description**
Selection of the calculation type according to which the muntin prices are calculated:
1.  **1 - Fields:** The price is calculated per field.
2.  **2 - LM+C+T:** The price is calculated per linear meter, per crossing, and per trim.
3.  **3 - LM:** The price is calculated per linear meter.
4.  **4 - LM+C:** The price is calculated per linear meter and per crossing.
5.  **5 - LM+T:** The price is calculated per linear meter and per trim.
6.  **6 - C:** The price is calculated per crossing.
7.  **7 - C+R:** The price is calculated per crossing and per trim. (Note: 'R' likely means 'Trim' here)
8.  **8 - T:** The price is calculated per trim.
9.  **9 - Special:** This form of calculation is configured customer-specifically.
10. **10 - Percent:** The price is calculated as a percentage from the basic price of the header article. The percentage is specified in the detail view in the **Percent** field.
11. **11 - sqm price:** The price is calculated per square meter of the glass. The price is specified in the **Sq m price** field.
12. **12 - Field+LM:** The price is calculated per field and per linear meter.
13. **13 - Piece:** A total price is calculated for the muntin pattern. The price is specified in the detail view in the **Unit price** field.
14. **14 - C or LM:** The price is calculated per crossing or per linear meter.
    *   If crossing points arise on the muntin pattern, the muntins are calculated according to the number of crossings.
    *   If there are no crossing points, the muntins are calculated by linear meters.
15. **15 - Field+C+T:** The price is calculated per field, per crossing, and per trim.
If in the conditions another calculation type is specified, the prices from the conditions apply.
*Technical info: numeric field, alphanumeric field, toggle field, DB field: kuspropr.berart*

**Lin. meter**
Specification of the price per linear meter. The price is evaluated for the calculation types LM, LM+C+T, LM+C, LM+T, Field+LM, and Special. The price is calculated from the total length of the muntins in the order.
*Technical info: numeric field, DB field: kuspropr.plm*

**Cross**
Specification of the price per crossing point. The price is evaluated for the calculation types C, C+T, LM+C, LM+C+T, C or LM, Field+C+R, and Special. In the order, the price is calculated according to the number of crossing points. If in a lite 2 different muntin articles are installed, the price is determined with the crossing price of the first muntin.
*Technical info: numeric field, DB field: kuspropr.pkr*

**Trim**
Specification of the price per trim. The price is evaluated for the calculation types T, LM+C+T, LM+T, C+T, Field+C+T, and Special. In the order, the price is calculated from the number of trims.
*Technical info: numeric field, DB field: kuspropr.pra*

**Fields**
Specification of the price per field. The price is evaluated for the calculation types Fields, Field+LM, Field+C+T, and Special. In the order, the price is calculated according to the number of fields. If in a lite 2 different muntin articles are installed, the price is determined with the field price of the first muntin.
*Technical info: numeric field, DB field: kuspropr.pfe*

### Muntin prices - details

**Master data > Conditions > Special prices > Muntin prices > <F2>**

On this dialog, you create the conditions for calculating muntin prices, e.g. for the calculation type Percent or Special.

**<F2>** Change to overview.
-> "Muntin prices - overview" on page C-918

*(Image: Abb. C-212 Muntin prices - details. A dialog box showing detailed fields for Muntin Prices, including Lin. Meter, Cross, Trim, Fields, Percent, Price/Sqft, and Unit Price for a specific calculation type.)*

#### Field descriptions

The fields in the header area are described for the Muntin Prices - Overview dialog:
-> "Muntin prices - overview" on page C-918

In addition, the following fields are displayed:

**Fields2**
Specification of the price per field if there are no crossing points in the muntin pattern. The price is calculated with the calculation type 9 Special.
*Technical info: numeric field, DB field: kuspropr.pfe2*

**Percent**
Specification of the percentage. The price is evaluated for the calculation types Percent and Special.
In the order, the price from the item price of the header article is calculated including all processings.
*Technical info: numeric field, DB field: kuspropr.prozent*

**Sqm price**
Specification of the square meter price. The price is evaluated with the calculation type **sqm price**.
In the order, the price is calculated from the number of square meters of the IG Unit.
*Technical info: numeric field, DB field: kuspropr.qmpreis*

**Unit price**
Specification of the unit price. The price is evaluated with the calculation type **Unit**.
In the order, the item price is calculated for the whole muntin pattern.
*Technical info: numeric field, DB field: kuspropr.stckpreis*

**Min. lin. meter**
Specification of the muntin length in meters, for which the price is calculated at a minimum. The price is evaluated for the calculation type **LM**.
In the order, the price is calculated for this muntin length if the actual muntin length in total is less than this value.
If you configure the **Minimum linear meter calculation for muntin partial items** via the environment variable `MINBER_AUF_TEILSPROSSE`, this value is evaluated for each individual muntin.
*Technical info: numeric field, DB field: kuspropr.minlm*

**Min. no. of fields piece**
Specification of muntin fields for which the minimum price is calculated. The price is evaluated for the calculation type **Field**.
In the order, the price for this number of fields is calculated if the actual number of fields is smaller than this value.
*Technical info: numeric field, DB field: kuspropr.minfeld*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from .. to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: kuspropr.vondat, kuspropr.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific muntin prices have to be redefined if you want to keep working with these conditions.

## Processing prices

**Master data > Conditions > Special prices > Processing prices**

On this dialog, you specify processing prices for market partners, objects, and industries. In the detail view, you create the conditions for the price calculation, e.g. price scales, minimum calculation quantity, surcharges.
These processing prices have a higher priority than the prices from the processing vectors.
-> "Processing vectors" on page C-753

The following views are available for this dialog:
*   "Processing prices - overview" on page C-923
*   "Processing prices - details" on page C-927

### Processing prices - overview

**Master data > Conditions > Special prices > Processing prices**

On this overview, you maintain the market partner-specific processing prices.

**<F2>** Change to the detailed view.
-> "Processing prices - details" on page C-927

*(Image: Abb. C-213 Processing prices - overview. A dialog box titled 'Processing Prices' showing a table with columns for Article, to Thckn., fr. Qty., Calc. Type, and Price 1.)*

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom the common conditions should apply have to be assigned an industry.
*Technical info: numeric field, toggle field, DB field: kubeapr.kondkz*

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: kubeapr.kunr*

**Article**
Selection of the article for which the market partner-specific conditions apply.
*Technical info: numeric field, DB field: kubeapr.kunr*

> **Vector-related processing prices**
> If you store the market partner-specific processing prices per processing vector, your system can be configured explicitly for this. In such a configuration, you must enter the number of the processing vector manually in the **Article** field. If you are interested, please contact an A+W Software GmbH employee.

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: kubeapr.plkz*

**To thckn.**
Specification of the thickness in millimeters up to which the price specifications apply. The thickness refers to the article to which the processing is attached in the BOM.
*Technical info: numeric field, DB field: kubeapr.dicke*

**fr. qty.**
Specification of the limit quantity starting from which the price specifications are considered. For quantities before the limit quantity is reached, the general processing price applies.
The quantity refers to the basic quantity unit (BQU), which is assigned to the processing article in the master data, e.g. area, pieces, length.
*Technical info: numeric field, DB field: kubeapr.menge*

**Calc. type**
Selection of the calculation type according to which the processing prices are scaled:
*   **Offs. 1:** The price from the **Offset 1** field is used as the processing price.
*   **Area:** The price is scaled according to the area of the lite (after round size, without minimum calculation). If the area is greater than or equal to the specified limit, the appropriate scaled price is used as the processing price.
*   **Longer edge:** The price is scaled according to the longest edge (after round size). If the longest edge is greater than or equal to the specified limit, the appropriate offset price is used as the processing price.
*   **Circumference:** The price is scaled according to the circumference of the lite (after round size). If the circumference is greater than or equal to the specified limit, the appropriate offset price is used as the processing price.
*   **Offs.:** The price of the price level that is specified in the conditions is used as processing price.
*   **Area/item:** The price is scaled according to the area of the lite (after round size, without minimum calculation) per item. For this, the area of the lite is calculated after round size and multiplied by the quantity from the item. If the calculated total area is greater than or equal to the specified limit, the appropriate offset price is used as processing price.
*   **2 edges:** The price is scaled depending on the two edge lengths. The two edge lengths are compared to the stored limit values. Here, the shorter edge is compared to the smaller limit and the longer edge to the larger limit from the processing vector. If one of the two edge lengths is on a higher price level than the other, the scaled price of the higher price level in question is used as processing price.
*   **Pieces/Item:** The price is scaled according to the number of lites per item. If the total quantity of the item is greater than or equal to the specified limit, the corresponding offset price is used as processing price.
*Technical info: alphanumeric field, toggle field, DB field: kubeapr.berart*

**Price type**
Specification of to what the specified price refers:
*   **CU/piece:** In the order, the price is calculated as fixed amount per piece in the item.
*   **CU/BQU:** The price is calculated per basic quantity unit (BQU), which is stored in the article master data, e.g. per piece, linear meter, etc.
*   **Percent:** The price is calculated and charged as a percentage of the glass basic price.
*   **CU/sqm:** The price is calculated per square meter.
*   **CU/Im:** The price is calculated per linear meter.
*Technical info: alphanumeric field, toggle field, DB field: kubeapr.ptyp*

**Price 1**
Specification of the individual price. This price is used in the order if no scaling is defined or if the dimension of the article underruns the quantity specifications of the defined price levels. A minimum calculation quantity can be specified in the detail view.
*Technical info: numeric field, DB field: kubeapr.preis1*

### Processing prices - details

**Master data > Conditions > Special prices > Processing prices > <F2>**

On this dialog, you specify the conditions for calculating market partner-specific processing prices. In addition, you can specify scaled prices for the selected processing article.

**<F2>** Change to overview.
-> "Processing prices - overview" on page C-923

*(Image: Abb. C-214 Processing prices - details. A dialog box showing detailed fields for a processing price, including Surcharge Matrix, Minim. Calculat., Factor, and a grid for quantity offsets and prices.)*

#### Field descriptions

The fields in the header area are described for the Processing Prices - Overview dialog:
-> "Processing prices - overview" on page C-923

In addition, the following fields are displayed:

**Surcharge matrix**
Selection of a surcharge matrix for a general surcharge on the processing price.
-> "Surcharge matrices" on page C-807
You can also assign a surcharge matrix of the type **Glass basic price**. Thus, the surcharge is not levied on the processing price, but on the glass price.
*Technical info: numeric field, DB field: kubeapr.zumatnr*

**Minim. Calculat.... BQU**
Specification of the quantity in basic quantity units that are charged as a minimum. The basic quantity unit is determined from the article master data.
If the price-relevant quantity in the order item is smaller than the defined minimum quantity, the price for this minimum quantity is calculated.
-> Tutorial, “Price-relevant quantity" on page C-562
*Technical info: numeric field, DB field: kubeapr.minber*

**Factor ...%**
Specification of a factor by which the market partner-specific processing price is multiplied. Using the factor, you can change the price calculation for the article without having to adjust all price levels, e.g. for price increases or a market partner-specific discount. If you leave the field empty, the factor from the conditions applies according to the condition hierarchy.
*Technical info: numeric field, DB field: kubeapr.faktor*

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 corresponds to a discount | 20.00 € | 16.00 € |
> | 150 corresponds to a surcharge | 20.00 € | 30.00 € |

**Offs. from quantity ...**
Specification of the limit quantity per offset. The fields are displayed for all calculation types except for **2 edges**. The limit value is interpreted depending on the calculation type as quantity, area or edge length. The specified price is used if in the order the quantity is greater than or equal to the limit value.
*Technical info: numeric fields, DB fields: kubeapr.me2, kubeapr.me3, ..., kubeapr.me10*

**Offs. to quantity ...**
Entry of the limit quantities per offset. The fields are only displayed for the calculation type **2 edges**. Per offset, you have to specify two limit values for both edges. The specified price is used if in the order the quantity is less than or equal to the specified limit values.
*Technical info: numeric fields, DB fields: kubeapr.me1, kubeapr.mas2_1, kubeapr.me2, kubeapr.mas2_2, ... kubeapr.me10, kubeapr.mas2_10*

**(Dimension)**
Specification of the limit value in mm per offset. These fields are only enabled if **11 Variant** or **12 Variant Scale** is selected as calc. base.
If in the order the edge lengths of the article are greater than or equal to the limit values, the price of this price level applies.
*Technical info: numeric fields, DB fields: kubeapr.mas2_1, kubeapr.mas2_2, ..., kubeapr.mas2_10*

**Price**
Specification of the price per price level.
If calculation type **Offs. 1** is selected, only the field from the **Offs. 1** field is used.
*Technical info: numeric fields, DB fields: kubeapr.preis2, kubeapr.preis3, ..., kubeapr.preis10*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: kubeapr.vondat, kubeapr.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific processing prices have to be redefined if you want to keep working with these conditions.

## IG exchange prices

**Master data > Conditions > Special prices > IG exchange prices**

On this dialog, you specify IG exchange prices for market partners, objects, and industries. In the detail view, you create the conditions for the price calculation, e.g. minimum calculation quantity, round size, small glass surcharges, and excess length surcharges.
These exchange prices have a higher priority than the general exchange prices.
-> "TG/LAMI/Special exchange prices" on page C-730

The following views are available for this dialog:
*   "IG exchange prices - overview" on page C-930
*   "IG exchange prices – details" on page C-933

### IG exchange prices - overview

**Master data > Conditions > Special prices > IG exchange prices**

In this overview, you maintain the exchange prices for TG, LAMI, and float lites that should be installed in an IG lite. These prices apply for a market partner, an object or an industry. These changes have a higher priority than the general exchange prices.

**<F2>** Change to the detailed view.
-> "IG exchange prices - details" on page C-933

*(Image: Abb. C-215 Exchange prices - overview. A dialog box titled 'Exchange Prices' showing a table with columns for Article, Exchange List, frm Piece, Factor, and Price 1.)*

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom the common conditions should apply have to be assigned to an industry.
*Technical info: numeric field, toggle field, DB field: kuaustpr.kondkz*

**Market partner**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: kuaustpr.kunr*

**Article, description**
Selection of the exchange glass for which the market partner-specific exchange prices apply.
*Technical info: numeric field, DB field: kuaustpr.artnr*

**Exchange list, description**
Selection of the exchange list for which the market partner-specific exchange prices apply.
*Technical info: alphanumeric field, DB field: kuaustpr.atlnr*

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: kuaustpr.plkz*

**frm ... Piece**
Limit quantity in pieces starting from which the price information applies. The data from this dialog is used for price calculation if the number of lites in the item in the transaction for item entry is greater than or equal to the specified quantity.
*Technical info: numeric field, DB field: kuaustpr.stueckzahl*

**Factor %**
Specification of a factor by which the market partner-specific exchange price is multiplied. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. If you leave the field empty, the factor from the conditions applies according to the condition hierarchy.
*Technical info: numeric field, DB field: kuaustpr.faktor*

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 corresponds to a discount | 20.00 € | 16.00 € |
> | 150 corresponds to a surcharge | 20.00 € | 30.00 € |

**Price 1**
Specification of the individual price for the exchange glass that applies starting with the specified quantity. If the quantity is not reached in the order, the general exchange prices and conditions are used.
*Technical info: numeric field, DB field: kuaustpr.preis1*

### IG exchange prices – details

**Master data > Conditions > Special prices > IG exchange prices > <F2>**

On this dialog, you specify the conditions for the calculation of IG exchange prices, e.g. price scales, minimum calculation areas, round size, surcharges.

**<F2>** Change to overview.
-> "IG exchange prices - overview" on page C-930

*(Image: Abb. C-216 Exchange prices – details. A dialog box showing detailed fields for IG exchange prices, including Minim. Calculat., Round Size, Calc. Type, Surcharges, and a grid for dimensional prices.)*

#### Field descriptions

The fields in the header area are described for the Exchange Prices - Overview dialog:
-> "IG exchange prices - overview" on page C-930

In addition, the following fields are displayed:

**Minim. calculat.... QU**
Specification of the minimum quantity for which the price is calculated. The minimum quantity is specified according to the basic quantity unit in the article master data, e.g. area in square meters. If the area of the glass in the order item is smaller than the minimum calculation, the price for the minimum calculation is used.
Depending on the configuration, the calculation of the exchange price can refer to the header article or the exchange article.
*   If the variable `MINBER_AUSTAUSCH_OHNE_MAX` is active, for articles with the pricing method IG-current, only the specified minimum calculation unit is evaluated.
*   If the variable `MINBER_AUSTAUSCH_OHNE_MAX` is not active, for articles with the pricing method **IG-current**, the minimum calculation of base articles and exchange articles is used and the larger of the two calculations is evaluated.
Regardless of this setting, the higher price is always calculated.
-> Tutorial, “Price-relevant quantity" on page C-562
*Technical info: numeric field, DB field: kuaustpr.minber*

**Round size**
Specification of the round size in mm for the price calculation of the article, e.g. 30 mm.
For the price calculation, the height and width of the order item are rounded up to the next-higher length in mm, which can be divided by the specified round size.
*Technical info: numeric field, DB field: kuaustpr.massrund*

> **Example**
> 30 mm is defined as round size.
> The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 mm is 1020 mm.
> The price is calculated from the dimensions 1020 x 1020 mm = 1.04 square meters.

**Calc. type**
Selection of the calculation type according to which the exchange prices are scaled:
*   **Area:** The price is scaled according to the area of the lite (after round size, without minimum calculation). If the area is greater than or equal to the specified limit, the scaled price is used as exchange price.
*   **1 edge:** The price is scaled according to the area of the edge (after round size). If the longest edge is greater than or equal to the specified limit, the scaled price is used as exchange price.
*   **2 edges:** The price is scaled depending on the two edge lengths. The two edge lengths are compared to the stored limit values. Here, the shorter edge is compared to the 1st dimension and the longer edge to the 2nd dimension. By default, the exchange price for the respective level is only used if both dimensions exceed the limits. If the variable `ISOAUST_2KANTEN_BIS` is active, the exchange price is also used if only one limit is exceeded.
*   **Matrix:** The price is scaled according to the assigned matrix. You assign the matrix in the **Matrix** field. By default, as exchange price, a mixed price from `(lite basic price + matrix price) / 2 - lite basic price` is calculated. If the variable `ISOAUST_KEINE_MISCHMATRIX` with the value ON is active, the scaled price is drawn directly as exchange price from the appropriate matrix.
*   **Percent:** The price is scaled according to the area of the glass (after round size, without minimum calculation). If the area is greater than or equal to the specified limit, the scaled price is used as exchange price. The price is calculated as a percentage from the basic price of the header article and added.
*Technical info: alphanumeric field, toggle field, DB field: kuaustpr.berechart*

**Matrix**
Specification of the matrix that is used for calculation. The field is only displayed if you have specified **Matrix** as calculation type. The fields for the dimension levels and scaled prices are then locked.
*Technical info: numeric field, DB field: kuaustpr.matrix*

**Dimensions**
**frm ...** Specification of the limit values for scaled prices. The price of a level applies until the next higher value is reached.
Depending on the calculation type selected, you have to enter the values in the following dimensional units:
*   **Area:** Number of square meters starting with which the assigned price is calculated.
*   **Edge:** Number of millimeters starting with which the assigned price is calculated.
*   **Percentage:** Number of surfaces in percent starting with which the assigned price is calculated.
*   **Matrix:** The prices are calculated according to the assigned matrix. The fields for the limit values and prices are locked.
*Technical info: numeric fields, DB fields: kuaustpr.grenz21, kuaustpr.grenz31, kuaustpr.grenz41, kuaustpr.grenz51*

**Price 2-5**
Specification of the price for the dimension step in question. The price applies until the next higher value is reached.
*Technical info: numeric fields, DB fields: kuaustpr.preis2, kuaustpr.preis3, ... kuaustpr.preis5*

**Small glass surcharges**
**to ... sf** Specification of limit values for price surcharges. The price is added to the price of the exchange glass if the area entered is smaller than or equal to the specified value, e.g. up to 0.5 sqm.
This surcharge makes sense if the lites are too small to process with the machine.
*Technical info: numeric fields, DB fields: kuaustpr.kleinme1, ..., kuaustpr.kleinme4*

**(Value)**
Specification of the surcharge that is charged if the area of the exchange glass is less than or equal to the specified limit value.
*Technical info: numeric fields, DB fields: kuaustpr.kleinzu1, ..., kuaustpr.kleinzu4*

**(Surcharge type)**
Specification of to what the specified surcharge refers:
*   **CU/sqm:** The surcharge is added per square meter, e.g. up to 0.5 sqm a price surcharge of 10 € per sqm is due.
*   **Percent:** The surcharge is added as a percentage to the price of the exchange glass, e.g. up to 0.5 sqm a price surcharge of 10% is due.
*Technical info: alphanumeric fields, toggle fields, DB fields: kuaustpr.kleinptyp1, ... kuaustpr.kleinptyp4*

**Excess length surcharges**
**frm... mm** Specification of limit values for percentage price surcharges. The surcharge is charged as a percentage of the price of the exchange glass if the dimension entered including round size is greater than or equal to the specified dimension, e.g. from 2200 mm. The specification always refers to the longer edge regardless of the calculation type.
If the environment variable `ISO_UELZUSCHLAG_NUR_AUSTAUSCH` is active, the overlength surcharge for the pricing method IG-current is only added to the exchange prices and not to the basic price.
*Technical info: numeric fields, DB fields: kuaustpr.uelme1, kuaustpr.uelme2*

**(Value) %**
Specification of the percentage that is charged if an edge length of the exchange article is longer than or equal to the specified limit value.
*Technical info: numeric fields, DB fields: kuaustpr.uelzu1, kuaustpr.uelzu2*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: kuaustpr.vondat, kuaustpr.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific exchange prices have to be redefined if you want to keep working with these conditions.

## Special prices for IG single lites

**Master data > Conditions > Special prices > Single lites for IG products**

On this dialog, you specify market partner-specific prices for the single lites that are installed in IG articles. The fixed dimension articles that are on the first level of the BOM below the IG article count as single lites. The prices for single lites are used if the calculation type **Single Lites** is assigned to the article in the IG basic prices.
-> "Prices for IG single lites" on page C-710

In the detail view, you create the conditions for the price calculation, e.g. price scales, minimum calculation price, surcharges.
These prices have a higher priority than the general prices for IG Single Lites.

The following views are available for this dialog:
*   "Single lites for IG products – overview" on page C-937
*   "Single lites for IG products – detail" on page C-940

### Single lites for IG products – overview

**Master data > Conditions > Special prices > Single lites for IG products**

In this overview, you maintain the market partner-specific prices for single lites that are installed in IG articles. The fixed dimension articles that are on the first level of the BOM below the IG article count as single lites.

**<F2>** Change to the detailed view.
-> "Single lites for IG products – detail" on page C-940

*(Image: Abb. C-217 Single lites for IG articles - overview. A dialog box showing a table with columns for Article, Price Type, Factor, and Price 1 for single lites in IG products.)*

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom the common conditions should apply have to be assigned to an industry.
*Technical info: numeric field, DB field: spezeinz.kondkz*

**Market partner**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: spezeinz.kondnr*

**Article, description**
Selection of the glass article for which the market partner-specific prices apply.
*Technical info: numeric field, DB field: spezeinz.artnr*

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: spezeinz.plkz*

**Calc. base**
Selection of the calc. base that determines from which price level the price is determined.
*   **1 - Single price:** For price calculation, the level 1 price is used.
*   **3- Quantity scale per item (BQU):** To determine the price level, the quantity of the item is determined using the basic quantity unit (BQU) of the article. The price is calculated according to the price level that is reached through the total quantity of the item.
*   **4 - Quantity scale per unit (BQU):** The basic quantity in a unit of the item is determined for determination of the price level. For price calculation, the price is multiplied by the quantity.
*Technical info: numeric field, DB field: spezeinz.part*

**Price type**
Specification of to what the specified price refers:
*   **CU/BQU:** The price is calculated per basic quantity unit (BQU) from the article master data, e.g. per square meter, etc.
*   **CU/piece:** In the order, the price is calculated as fixed amount per piece in the item.
*Technical info: alphanumeric field, toggle field, DB field: spezeinz.ptyp*

**Factor**
Specification of a market partner-specific factor by which the price is multiplied. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. If you leave the field empty, the factor from the conditions applies according to the condition hierarchy.
*Technical info: numeric field, DB field: spezeinz.faktor*

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 corresponds to a discount | 20.00 € | 16.00 € |
> | 150 corresponds to a surcharge | 20.00 € | 30.00 € |

**Price 1**
Specification of the basic price for the single lite. If **1 - Single Price** is selected as calc. base, only the price from this field is used for price calculation.
*Technical info: numeric field, DB field: spezeinz.preis1*

### Single lites for IG products – detail

**Master data > Conditions > Special prices > Single lites for IG products > <F2>**

On this dialog, you create the conditions for the calculation of market partner-specific prices for the single lite, e.g. the scaled prices.
The prices for single lites are used if the calculation type **Single Lites** is assigned to the article in the IG basic prices.

**<F2>** Change to overview.
-> "Single lites for IG products – overview" on page C-937

*(Image: Abb. C-218 Single lites for IG products - details. A dialog box showing detailed settings for a single lite, including Surcharge matrix, Min. Price, and a grid for quantity-based price offsets.)*

#### Field descriptions

The fields in the header area are described for the IG Single Lites - Overview dialog:
-> "Single lites for IG products – overview" on page C-937

In addition, the following fields are displayed:

**Surcharge matrix**
Selection of the surcharge matrix for a general surcharge on the single lite. In the order entry, the price of the single lite is displayed including this surcharge.
-> "Surcharge matrices" on page C-807
*Technical info: numeric field, DB field: spezeinz.zumatnr*

**Min. price**
Specification of the minimum price for the single lite. This price is charged if the calculated price in the order item is less than the specified minimum price.
The minimum price for header articles with the pricing method **IG-current** can be evaluated according to the minimum prices for single lites. For this, the IG basic price of the article is determined from the total of the single lites and the IG minimum price from the total of minimum prices for the single lites. If the price of the IG article including the defined surcharges and the factor is less than the minimum price, the minimum price is calculated. This calculation can be used for purchasing and sales prices.
*Technical info: numeric field, DB field: spezeinz.minpreis*

**Offs. frm qty**
Specification of the quantity starting with which the price of the offset is calculated. If in the order the quantity in basic quantity units (BQUs) is greater than or equal to the specified value, the assigned price is calculated.
The prices for offsets are used only for price calculation for the calc. bases **3 - Quantity scale per item (BQU)** or **4 - Quantity scale per unit (BQU)**.
*Technical info: numeric fields, DB fields: spezeinz.me2, spezeinz.me3, ..., spezeinz.me10*

**Price for offset**
Specification of the price that is calculated for the offset.
*   For the calc. base **1 - Single Price**, only the price for offset 1 is used.
*   For the calc. base **3 - Quantity scale per item (BQU)** or **4 - Quantity scale per unit (BQU)**, the prices are determined from the associated price level.
*Technical info: numeric fields, DB fields: spezeinz.preis2, spezeinz.preis3 ..., spezeinz.preis10*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: spezeinz.vondat, spezeinz.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific prices for single lites have to be redefined if you want to keep working with these conditions.

## Special IG basic prices

**Master data > Conditions > Special prices > IG basic prices**

On this dialog, you assign the IG articles special price matrices, price vectors or prices for single lites. This assignment applies only for the selected market partner.
On the detail view, you create the conditions for the price calculation, e.g. minimum edge length, round size, minimum calculation, and various surcharges.
These market partner-specific prices have a higher priority than the general IG basic prices.
-> "IG base prices" on page C-704

The following views are available for this dialog:
*   "Special IG basic prices – overview" on page C-942
*   "Special IG basic prices – details" on page C-945
*   "Special IG basic prices - exchange lists" on page C-949

### Special IG basic prices – overview

**Master data > Conditions > Special prices > IG basic prices**

On this overview, you maintain the assignments of market partner-specific prices to IG articles. These market partner-specific prices have a higher priority than the general IG basic prices.

*(Image: Abb. C-219 IG basic prices – overview. A dialog box showing a table with columns for Article, Type (Matrix/Vector), and the corresponding Matrix/Vector number and description.)*

**<F2>** Change to the detailed view.
-> "Special IG basic prices – details" on page C-945

**<F2> <F2>** Change to the detailed view for exchange lists.
-> "Special IG basic prices - exchange lists" on page C-949

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condit. type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom the common conditions should apply have to be assigned to an industry.
*Technical info: numeric field, toggle field, DB field: spezpisomat.kondkz*

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: spezpisomat.kondnr*

**Article**
Selection of the IG article for which the market partner-specific conditions apply.
*Technical info: numeric field, DB field: spezpisomat.artnr*

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: spezpisomat.vpkz*

**Type**
Selection of the type according to which the IG article is calculated:
*   **Matrix:** The price for the IG article is calculated from the assigned price matrix. For this, you have to select the number of the price matrix. This is the default method for IG.
*   **Vector:** The price for the IG article is calculated from the assigned vector. For this, you have to select the number of the price vector.
*   **Single lites:** The price for the IG article is calculated from the individual prices of the lites from which the IG lite is made. The prices for single lites are entered on the **Single Lites for IG Articles** dialog. This also applies for exchange lites.
    -> "Prices for IG single lites" on page C-710
*Technical info: alphanumeric field, toggle field, DB field: spezpisomat.matvek*

**Matrix, description**
Selection of the price matrix for the IG article. The field is only enabled if the type **Matrix** is selected.
You create the prices themselves on the **Matrix Editor** dialog.
-> "Matrix editor" on page C-715
*Technical info: numeric field, DB field: spezpisomat.matnr*

**Vector, description**
Selection of the vector for the IG article. The field is only enabled if the type **Vector** is selected.
You create the prices themselves on the **Article Vectors** dialog.
-> "Article vectors" on page C-693
*Technical info: numeric field, DB field: spezpisomat.veknr*

### Special IG basic prices – details

**Master data > Conditions > Special prices > IG basic prices > <F2>**

On this dialog, you create the conditions for the calculation of market partner-specific basic prices, e.g. surcharges and exchange lists.

**<F2>** Change to the detailed view for exchange lists.
-> "Special IG basic prices - exchange lists" on page C-949

**<F2> <F2>** Change to overview.
-> "Special IG basic prices – overview" on page C-942

*(Image: Abb. C-220 IG basic prices – details. A dialog box showing detailed surcharge and rounding settings for an IG basic price, including fields for Minimum Edge Length, Surcharge Matrix, and various other surcharges.)*

#### Field descriptions

The fields in the header area are described for the IG-Basic Prices - Overview dialog:
-> "Special IG basic prices – overview" on page C-942

In addition, the following fields are displayed:

**Minimum edge length ... mm**
Specification of the edge length in mm. This size is used for the price calculation if the height or width of the lite in the order item is smaller than the minimum edge length.
-> Tutorial, “Price-relevant quantity" on page C-562
*Technical info: numeric field, DB field: spezpisomat.minkan*

**Minim. calculat.... sf**
Specification of the area in square feet. This size is used for price calculation if the area of the glass in the order item is smaller than this minimum calculation area. For shapes, the circumscribing rectangle of the IG unit is used as price-relevant area.
-> Tutorial, “Price-relevant quantity" on page C-562
*Technical info: numeric field, DB field: spezpisomat.minbereh*

**Round size ... mm**
Specification of the round size in mm for the price calculation of the glass area. For the price calculation, the edge lengths in the order item are rounded up to the next higher length that is divisible by the specified round size in mm. If the minimum edge length of a lite is not reached, this is used first. The round size is then calculated.
-> Tutorial, “Price-relevant quantity" on page C-562
*Technical info: numeric field, DB field: spezpisomat.massrd*

> **Example**
> 30 mm is defined as round size.
> The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 mm is 1020 mm.
> The price is calculated from the dimensions 1020 x 1020 mm = 1.04 square meters.

**Surcharge matrix**
Selection of the surcharge matrix for a general surcharge:
*   For the price calculation according to a matrix, the surcharge is charged on the IG unit.
*   For the price calculation for single lites, the surcharge is charged on each single lite.
In the order entry, the price including this surcharge is displayed.
-> "Surcharge matrices" on page C-807
-> Tutorial, "Surcharge matrix" on page C-627
*Technical info: numeric field, DB field: spezpisomat.zumatnr*

**Surcharge**
Specification of the price surcharge that is always added, e.g. for IG with thermo lite. You specify the surcharge type in the next field.
*Technical info: numeric field, alphanumeric toggle field, toggle field, DB field: spezpisomat.zuschl*

**Surcharge (type)**
Specification of to what the specified surcharge refers:
*   **CU/sqm:** The surcharge is charged on the IG basic price and multiplied by the price-relevant quantity in square meters.
*   **Percent:** The surcharge is charged as a percentage on the IG basic price.
*Technical info: numeric field, alphanumeric toggle field, toggle field, DB field: spezpisomat.zutyp*

**Surcharge roundg**
Specification of how the calculated surcharge is rounded:
*   **Up:** The price that is entered in the following field is rounded up to the hundredth value in currency units.
*   **Down:** The price that is entered in the following field is rounded down to the hundredth value in currency units.
*   **Com:** The price that is entered in the following field is rounded up or down to the hundredth value.
*Technical info: alphanumeric field, toggle field, DB field: spezpisomat.zurdtyp*

**Up**
Specification of the value to which rounding up will be done, e.g. to 1, 10, 100.
*Technical info: numeric field, DB field: spezpisomat.zurund*

> **Example**
>
> | Rounding | Value | from | to |
> | :--- | :--- | :--- | :--- |
> | to 10 | 4.32 € | 4.40 € | rounded up |
| | 4.78 € | 4.80 € | |
| from 10 | 4.32 € | 4.30 € | rounded down |
| | 4.78 € | 4.70 € | |
| Com 10 | 4.32 € | 4.30 € | rounded down |
| | 4.78 € | 4.80 € | rounded up |
| Com 100 | 4.32 € | 4.00 € | rounded down |
| | 4.78 € | 5.00 € | rounded up |

**AIR surcharge vector**
Selection of a surcharge for the spacer in the airspace (AIR).
-> "AIR surcharges" on page C-736
The specification is ignored if in the order conditions or in the conditions for the market partner in question it is specified that no AIR surcharge is calculated.
-> "Special general conditions" on page C-843
*Technical info: numeric field, DB field: spezpisomat.szrzutab*

**Decorative glass surch.**
Specification of a surcharge for decorative glass. This surcharge is calculated if in the BOM of the IG lite a lite with the article type **Decorative Glass** is added. The surcharge is only charged if the decorative glass is attached as exchange glass with exchange code in the IG article.
*Technical info: numeric field, DB field: spezpisomat.kunver*

**Offset surch.**
Specification of a market partner-specific offset surcharge. This surcharge is charged if in the BOM of the IG lite an offset with the article type **Offset with offset difference dimensions** is attached.
*Technical info: numeric field, DB field: spezpisomat.stufe*

**Offset surcharge type**
Specification of to what the specified surcharge refers:
*   **CU/pc ne:** The offset surcharge is charged according to calculation of the factor as fixed net amount per offset.
*   **CU/pc gr:** The offset surcharge is charged as gross amount per offset before calculation of the factor.
*   **Percent:** The offset surcharge is charged as a percent of the glass quantity unit price and the exchange prices.
*   **%/piece:** The offset surcharge is charged per offset as a percent of the glass quantity unit price and the replacement prices.
*Technical info: alphanumeric field, toggle field, DB field: spezpisomat.stuftyp*

**Size surcharges**
Specification of a size surcharge. The surcharge is charged on the order item on the basic glass price.
If the IG article is assigned to the pricing method **IG-current** and the environment variables `ISO_GROSSZU_AUF_AUSTAUSCH` and/or `GROSSZU_AUF_SZR` are configured appropriately, the surcharge is also charged on the exchange and/or spacer price.
-> "Size surcharges" on page C-812
-> Tutorial, “Size surcharges" on page C-629
*Technical info: numeric field, DB field: spezpisomat.grosszu*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: spezpisomat.vondat, spezpisomat.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific basic prices have to be redefined if you want to keep working with these conditions.

### Special IG basic prices – exchange lists

**Master data > Conditions > Special prices > IG basic prices > <F2> > <F2>**

In these fields, you assign exchange lists to the IG article. These lists are always used for price calculation if in the order item a glass of the IG lite is exchanged.
-> "Exchange/additional lists" on page C-692

**<F2>** Change to overview.
-> "Special IG basic prices – overview" on page C-942

**<F2> <F2>** Change to the detailed view.
-> "Special IG basic prices – details" on page C-945

*(Image: Abb. C-221 IG basic prices - exchange prices. A dialog box showing assignments of various exchange lists (Patterned GI., Special Glass, LAM, Tmp) to an IG article, categorized by installation position: Extern. Lite, Center Lite, Intern. Lite.)*

#### Field descriptions

The fields in the header area are described for the IG-Basic Prices - Overview dialog:
-> "Special IG basic prices - details" on page C-945

In addition, the following fields are displayed:

**Extern. lite, center lite, intern. lite**
You can specify the exchange lists depending on the installation position in which the exchange lite is installed in the IG unit.

**Patterned gl.**
If in the order item a patterned glass is exchanged into the BOM of the IG lite, the exchange price from the assigned exchange list is calculated.
*Technical info: numeric fields, DB fields: spezpisomat.gussatph, spezpisomat.kalpkz, spezpisomat.gussatpb*

**Special glass**
If in the order item a special glass is exchanged into the BOM of the IG lite, the exchange price from the assigned exchange list is calculated.
*Technical info: numeric fields, DB fields: spezpisomat.sonatph, spezpisomat.prsrdtp, spezpisomat.sonatpb*

**LAMI**
If in the order item a LAMI is exchanged into the BOM of the IG lite, the exchange price from the assigned exchange list is calculated.
*Technical info: numeric fields, DB fields: spezpisomat.vsgatph, spezpisomat.prsrd, spezpisomat.vsgatpb*

**TG**
If in the order item a TG is exchanged into the BOM of the IG lite, the exchange price from the assigned exchange list is calculated.
*Technical info: numeric fields, DB fields: spezpisomat.esgatph, spezpisomat.minprstp, spezpisomat.esgatpb*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: spezpisomat.vondat, spezpisomat.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific prices for UV protection have to be redefined if you want to keep working with these conditions.

## UV coating prices

**Master data > Conditions > Special prices > UV protection prices**

On this dialog, you specify market partner-specific prices for UV protection. You create additional scaled prices in the detailed view.
These prices have a higher priority than the general prices for UV protection.
-> "UV protection" on page C-738

The following views are available for this dialog:
*   "UV protection prices – overview" on page C-951
*   "UV protection prices – details" on page C-953

### UV protection prices – overview

**Master data > Conditions > Special prices > UV protection prices**

On this overview, you maintain the market partner-specific prices for UV protection. These prices have a higher priority than the general prices for UV protection.

**<F2>** Change to the detailed view.
-> "UV protection prices – details" on page C-953

*(Image: Abb. C-222 UV protection - overview. A dialog box titled 'UV Protection' showing a table with columns for Article, fr PLCD, and price scales 1 through 5.)*

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condit. type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
*Technical info: numeric field, DB field: kupuvab.kondkz*

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: kupuvab.kunr*

**Article**
Specification of the article from the article type **UV Protection** for which the prices apply.
*Technical info: numeric field, DB field: kupuvab.artnr*

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: kupuvab.plkz*

**Scale 1 - 10 (price)**
Specification of the scaled prices. The price applies per quantity unit of the UV protection.
In the detailed view, you specify the limit values for the dimensions. The price applies until the next-higher limit value is reached.
-> "UV protection prices - details" on page C-953
*Technical info: numeric fields, DB fields: kupuvab.preis1, kupuvab.preis2, ... kupuvab.preis10*

### UV protection prices – details

**Master data > Conditions > Special prices > UV protection prices > <F2>**

On this dialog, you specify the market partner-specific limit values for the price scales.

**<F2>** Change to overview.
-> "UV protection prices - overview" on page C-951

*(Image: Abb. C-223 UV protection - details. A dialog box showing a list of width limits and corresponding prices for a UV protection article.)*

#### Field descriptions

The fields in the header area are described for the UV Protection - Overview dialog:
-> "UV protection prices – overview" on page C-951

In addition, the following fields are displayed:

**Width to ... mm**
Specification of the width of the UV protection up to which the price applies.
*Technical info: numeric fields, DB fields: kupuvab.bis1, kupuvab.bis2, ... kupuvab.bis9*

**Price**
Specification of the scaled prices. The price applies per quantity unit of the UV protection.
The price applies until the next-higher limit value is reached, which is specified in the **Width to ... mm** fields.
*Technical info: numeric fields, DB fields: kupuvab.preis2, ... kupuvab.preis10*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: kupuvab.vondat, kupuvab.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific prices for UV protection have to be redefined if you want to keep working with these conditions.

## Glazing prices

**Master data > Conditions > Special prices > Glazing prices**

On this dialog, you specify market partner-specific prices for glazing and sealing. In the detailed view, you also create a minimum calculation price.
These prices have a higher priority than the general glazing prices.
-> "PCD glazing prices" on page C-790

> **Prerequisite**
> The prices for glazing and/or sealing can only be calculated if an article is attached to the BOM for which in the article master data the article type 520 Glazing or 525 Installation and the pricing method PCD-glazing is defined.

The following views are available for this dialog:
*   "Glazing prices - overview" on page C-955
*   "Glazing prices - details" on page C-957

### Glazing prices - overview

**Master data > Conditions > Special prices > Glazing prices**

On this overview, you maintain the market partner-specific prices for glazing and sealing. In the detailed view, you can also create a minimum calculation price.

**<F2>** Change to the detailed view.
-> "Glazing prices - details" on page C-957

*(Image: Abb. C-224 Glazing - overview. A dialog box titled 'Glazing' showing a table with columns for Article, Invoice Type, Sealing Price/lm, and Glazing Price/sqm.)*

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condit. type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
*Technical info: numeric field, toggle field, DB field: kuverglas.kondkz*

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: kuverglas.kunr*

**Article**
Selection of the glazing article for which the market partner-specific price applies.
*Technical info: numeric field, DB field: kuverglas.artnr*

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: kuverglas.pkz*

**Calculation type**
Selection of the calculation type. This type specifies how the prices are calculated:
*   **Glazing:** The glazing is calculated according to the area of the lite.
*   **Sealing:** The sealing is calculated according to the circumference of the lite.
*   **Glazing + Sealing:** Glazing and sealing are calculated.
*Technical info: alphanumeric field, toggle field, DB field: kuverglas.typ*

**Sealing**
**Price/Im** Specification of the price per linear meter.
*Technical info: numeric field, DB field: kuverglas.vklmpreis*

**Glazing**
**Price/sqm** Specification of the price per square meter.
*Technical info: numeric field, DB field: kuverglas.vkqmpreis*

### Glazing prices - details

**Master data > Conditions > Special prices > Glazing prices > <F2>**

On this dialog, you create the market-specific minimum prices for glazing and sealing.

**<F2>** Change to overview.
-> "Glazing prices - overview" on page C-955

The fields in the header area are described for the Glazing - Overview dialog:
-> "Glazing prices - overview" on page C-955

In addition, the following fields are displayed:

*(Image: Abb. C-225 Glazing - details. A dialog box showing fields for entering minimum prices for both Sealing and Glazing.)*

#### Sealing

**Min. price**
Specification of the minimum price for the sealing. This price is calculated if the calculated price in the order item is less than the specified minimum price.
*   Minimum prices for header articles are only evaluated for the pricing methods IG-Switzerland, IG-current (only with the calculation type Vector), PCD-LAMI, PCD-tempered, PCD-base glass, PCD-finished glass or PCD-prices.
*   Minimum prices for BOM subparts are only evaluated if for the header article the pricing method IG-current, PCD-LAMI, PCD-tempered, PCD-basic glass, PCD-finished glass or PCD-glass doors is selected and the subpart is an accessory item with the pricing method PCD prices-general.
The price is used for the calculation types **Sealing** and **Glazing + Sealing**.
*Technical info: numeric field, DB field: kuverglas.vkminversieg*

#### Glazing

**Min. price**
Specification of the minimum price for the glazing. This price is calculated if the calculated price in the order item is less than the specified minimum price.
*   Minimum prices for header articles are only evaluated for the pricing methods IG-Switzerland, IG-current (only with the calculation type Vector), PCD-LAMI, PCD-tempered, PCD-base glass, PCD-finished glass or PCD-prices.
*   Minimum prices for BOM subparts are only evaluated if for the header article the pricing method IG-current, PCD-LAMI, PCD-tempered, PCD-basic glass, PCD-finished glass or PCD-glass doors is selected and the subpart is an accessory item with the pricing method PCD prices-general.
The price is used for the calculation types **Glazing** and **Glazing + Sealing**.
*Technical info: numeric field, DB field: kuverglas.vkminpreis*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: kuverglas.vondat, kuverglas.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific prices for glazing have to be redefined if you want to keep working with these conditions.

## Exchange prices pattern glass classes

**Master data > Conditions > Special prices > Exchange prices pattern glass classes**

On this dialog, you specify market partner-specific exchange prices for patterned glass classes. In the detailed view, you specify the conditions for the price calculation, e.g. minimum calculation quantity, factor.
These prices have a higher priority than the general exchange prices for patterned glass.
-> "Pattern exchange prices" on page C-728

The following views are available for this dialog:
*   "Exchange prices pattern glass - overview” on page C-959
*   "Exchange prices pattern glass classes - details" on page C-961

### Exchange prices pattern glass - overview

**Master data > Conditions > Special prices > Exchange prices pattern glass classes**

On this overview, you maintain the market partner-specific exchange prices for patterned glass classes. You can also specify a factor.

**<F2>** Change to the detailed view.
-> "Exchange prices pattern glass classes - details" on page C-961

*(Image: Abb. C-226 Exchange prices pattern glass - overview. A dialog box showing a table with columns for Exchange List, Patt. Cat., fr PLCD, Factor, Price, and Type.)*

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
*Technical info: numeric field, toggle field, DB field: spezpgssat.kondkz*

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: spezpgssat.kondnr*

**Exchange list, description**
Selection of the exchange list for the assignment of market partner-specific exchange prices.
*Technical info: numeric field, DB field: spezpgssat.atlnr*

**Patt. cat.**
Specification of the patterned glass class (price group) for the exchange list. The glass is assigned to the pattern glass classes on the **Pattern Glass Exchange** dialog.
-> "Pattern exchange prices" on page C-728
*Technical info: alphanumeric field, DB field: spezpgssat.klasse*

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
-> Tutorial, "From-PLCD logic" on page C-552
*Technical info: numeric field, DB field: spezpgssat.plkz*

**Factor**
Specification of a factor by which the exchange price is multiplied. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. If you leave the field empty, the factor from the conditions applies according to the condition hierarchy.
*Technical info: numeric field, DB field: spezpgssat.faktor*

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 corresponds to a discount | 20.00 € | 16.00 € |
> | 150 corresponds to a surcharge | 20.00 € | 30.00 € |

**Price**
Specification of the price for the patterned class in question. With it, you override the price from the patterned glass class for the current market partner.
*Technical info: numeric field, DB field: spezpgssat.preis*

**Price type**
Specification of to what the specified price refers:
*   **CU/sqm:** The price is calculated per square meter.
*   **Percent:** The price is calculated as a percentage from the basic price of the header article including the surcharge.
*Technical info: alphanumeric field, toggle field, DB field: spezpgssat.preistyp*

### Exchange prices pattern glass classes - details

**Master data > Conditions > Special prices > Exchange prices pattern glass classes > <F2>**

On this dialog, you specify the market partner-specific minimum calculation price for the exchange article.

*(Image: Abb. C-227 Exchange prices pattern glass classes - details. A dialog box showing fields for Factor, Price, Type, and Minim. Calculat. for a patterned glass class.)*

**<F2>** Change to overview.
-> "Exchange prices pattern glass - overview" on page C-959

#### Field descriptions

The fields in the header area are described for the Exchange Prices Pattern Glass - Overview dialog:
-> "Exchange prices pattern glass - overview" on page C-959

In addition, the following fields are displayed:

**Minim. calculat.... sf**
Specification of the minimum area in square meters for which the price is calculated. If the area of the exchange glass in the order item is smaller than the minimum calculation area, the price for this area is used.
-> Tutorial, “Price-relevant quantity" on page C-562
*Technical info: numeric field, DB field: spezpgssat.minber*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: spezpgssat.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific exchange prices for patterned glass have to be redefined if you want to keep working with these conditions.

## LAMI exchange/additional prices

**Master data > Conditions - Special prices > LAMI exchange/additional**

On this dialog, you specify the market partner-specific exchange prices for glass and foils that are exchanged into LAMI articles or added. In the detailed view, you create the conditions for the price calculation, e.g. scaled prices, minimum calculation quantity, round size, size surcharges.
These prices have a higher priority than the general LAMI exchange prices.
-> "LAMI exchange/additional prices - overview" on page C-772

The following views are available for this dialog:
*   "LAMI exchange/additional prices – overview" on page C-964
*   "LAMI exchange/additional prices – details" on page C-967

### LAMI exchange/additional prices – overview

**Master data > Conditions - Special prices > LAMI exchange/additional**

On this overview, you maintain market partner-specific exchange prices for glass and foils that are exchanged into or added to LAMI articles. These prices have a higher priority than the general LAMI exchange prices.

**<F2>** Change to the detailed view.
-> "LAMI exchange/additional prices – details" on page C-967

*(Image: Abb. C-228 LAMI exchange/additional prices - Overview. A dialog box showing a table with columns for Article, List, fr PLCD, Calc. Type, Factor, and Price 1.)*

### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condit. type**
Selection for whom the conditions apply:
*   **Customer:** The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:** The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:** The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:** The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:** The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
*Technical info: numeric field, toggle field, DB field: spezvsgaust.kondkz*

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
*Technical info: numeric field, DB field: spezvsgaust.kondnr*

**Article, description**
Selection of the LAMI article for which the market partner-specific LAMI exchange/additional prices apply.

**List**
Selection of the exchange list in which you specify the prices.
The code of the exchange list is created on the **Exchange/additional lists** dialog.
-> "Exchange/additional lists" on page C-692
*Technical info: numeric field, DB field: spezvsgaust.artnr*

**fr PLCD**
Selection of the price list code (PLCD) starting from which the price data applies.
The price list code is created on the **Price List Code** dialog.
-> "Price lists (PLCD)" on page C-688
*Technical info: numeric field, DB field: spezvsgaust.plkz*

**Calc. type**
Selection of the calculation type according to which the exchange prices are calculated:
*   **Area:** The price is scaled according to the area of the lite (after round size, without minimum calculation). If the area is greater than or equal to the specified limit, the scaled price is used as exchange price.
*   **1 edge:** The price is scaled according to the area of the edge (after round size). If the longest edge is greater than or equal to the specified limit, the scaled price is used as exchange price.
*   **2 edges:** The price is scaled depending on the two edge lengths. The two edge lengths are compared to the stored limit values. Here, the shorter edge is compared to the 1st dimension and the longer edge to the 2nd dimension. By default, the exchange price for the respective level is only used if both dimensions exceed the limits. If the variable `ISOAUST_2KANTEN_BIS` is active, the exchange price is also used if only one limit is exceeded.
*   **Matrix:** The price is scaled according to the assigned matrix. You assign the matrix in the **Matrix** field. By default, as exchange price, a mixed price from `(lite basic price + matrix price) / 2 - lite basic price` is calculated. If the variable `ISOAUST_KEINE_MISCHMATRIX` with the value ON is active, the scaled price is drawn directly as exchange price from the appropriate matrix.
*   **Percent:** The price is scaled according to the area of the glass (after round size, without minimum calculation). If the area is greater than or equal to the specified limit, the scaled price is used as exchange price. The price is calculated as a percentage from the basic price of the header article and added.
*Technical info: alphanumeric field, toggle field, DB field: spezvsgaust.berechart*

**Factor**
Specification of a factor by which the exchange price is multiplied. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. If you leave the field empty, the factor from the conditions applies according to the condition hierarchy.
*Technical info: numeric field, DB field: spezvsgaust.faktor*

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 corresponds to a discount | 20.00 € | 16.00 € |
> | 150 corresponds to a surcharge | 20.00 € | 30.00 € |

**Price 1**
Specification of the individual price. You enter scaled prices in the detailed view.
-> "LAMI exchange/additional prices – details" on page C-967
*Technical info: numeric field, DB field: spezvsgaust.preis1*

### LAMI exchange/additional prices – details

**Master data > Conditions - Special prices > LAMI exchange/additional > <F2>**

On this dialog, you specify conditions for the price calculation, e.g. price scales, minimum calculation quantity, round size, surcharges.

**<F2>** Change to overview.
-> "LAMI exchange/additional prices – overview" on page C-964

*(Image: Abb. C-229 LAMI exchange/additional prices - details. A dialog box showing detailed settings for LAMI exchange prices, including Minim. Calculat., Round Size, Size Surcharges, and a grid for dimensional prices.)*

#### Field descriptions

The fields in the header area are described for the LAMI Exchange/Additional Prices - Overview dialog:
-> "LAMI exchange/additional prices - overview" on page C-964

In addition, the following fields are displayed:

**Minim. calculat. ... QU**
Specification of the minimum quantity for which the price is calculated. The minimum quantity is specified according to the basic quantity unit in the article master data, e.g. area in square meters. If the area of the glass in the order item is smaller than the minimum calculation, the price for the minimum calculation is used.
Depending on the configuration, the calculation of the exchange price can refer to the header article or the exchange article.
*   If the variable `MINBER_AUSTAUSCH_OHNE_MAX` is active, for articles with the pricing method IG-current, only the specified minimum calculation unit is evaluated.
*   If the variable `MINBER_AUSTAUSCH_OHNE_MAX` is not active, for articles with the pricing method **IG-current**, the minimum calculation of base articles and exchange articles is used and the larger of the two calculations is evaluated.
Regardless of this setting, the higher price is always calculated.
-> Tutorial, “Price-relevant quantity" on page C-562
*Technical info: numeric field, DB field: spezvsgaust.minber*

**Round size ... mm**
Specification of the round size in mm for the price calculation of the article, e.g. 30 mm.
For the price calculation, the height and width of the order item are rounded up to the next-higher length in mm, which can be divided by the specified round size.
*Technical info: numeric field, DB field: spezvsgaust.massrund*

> **Example**
> 30 mm is defined as round size.
> The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 mm is 1020 mm.
> The price is calculated from the dimensions 1020 x 1020 mm = 1.04 square meters.

**Size surcharges**
Selection of a size surcharge. This can be a small glass surcharge, an excess length surcharge, and/or an oversize surcharge. If the article over or underruns this size, the surcharge is charged on the glass price.
-> "Size surcharges" on page C-812
*Technical info: numeric field, DB field: spezvsgaust.grosszu*

**Dimensions**
**frm ...** Specification of the limit values for scaled prices. The price of an offset applies until the next higher value is reached.
Depending on the calculation type selected, you have to enter the values in the following dimensional units:
*   **Area:** Number of square meters starting with which the assigned price is calculated.
*   **Edge:** Number of millimeters starting with which the assigned price is calculated.
*   **Percentage:** Number of surfaces in percent starting with which the assigned price is calculated.
*   **Matrix:** The prices are calculated according to the assigned matrix. The fields for the limit values and prices are locked.
*Technical info: numeric fields, DB fields: spezvsgaust.grenz21, spezvsgaust.grenz22, spezvsgaust.grenz31, spezvsgaust.grenz32, spezvsgaust.grenz41, spezvsgaust.grenz42, spezvsgaust.grenz51, spezvsgaust.grenz52*

**Price**
Specification of the price for the dimension step in question. The price applies until the next higher value is reached.
*Technical info: numeric fields, DB fields: spezvsgaust.preis2, spezvsgaust.preis3, ... spezvsgaust.preis5*

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
*Technical info: date field, DB field: spezvsgaust.vondat, spezvsgaust.abdat*

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific exchange and additional prices for LAMI have to be redefined if you want to keep working with these conditions.

# A+W Enterprise Sales

## Revision overview of the module

| Date | Description |
| :--- | :--- |
| 05-2023 | Creation of tutorial, update of software reference |
| 02-2020 | Complete revision |
| 01-2017 | Product and company names adjusted. |
| 07-2013 | Complete revision and adjustment to new CI |
| 01-2010 | Minor corrections/identifier |
| 01-2008 | Price calculation |
| 02-2007 | Combination of Sales/Purchasing |
| 12-2006 | Change of part Sales |
| 02-2006 | Original version |

This module provides information on the following subjects:
-> Tutorial
-> Software Reference

# Tutorial

## This section provides information on the following subjects:
- Introduction
- General Operation and Shortcuts
- Overview of the Sales Menu
- Quotations
- Orders
- Delivery Notes
- Invoices
- Credit Notes
- Order Release
- Print
- Overview Functions in Sales
- Resubmission
- Modification Functions in Sales

### Table of Contents
*   Introduction D-976
*   General Operation and Shortcuts D-977
    *   Operation in the order D-977
    *   Shortcuts D-978
    *   Glossary D-979
    *   Search for documents D-980
*   Overview of the Sales Menu D-982
*   Quotations D-983
*   Orders D-985
    *   Order header and footer area D-986
    *   Enter new order D-986
    *   Enter order with reference D-990
    *   Order with consignments D-992
    *   Addresses in the order D-993
    *   Enter text and phrases D-995
    *   Additional documents in the order D-996
    *   Complete order entry D-997
    *   Change/correct order D-997
*   Item entry D-1000
    *   Enter new items D-1001
    *   Entering items (depending on product type) D-1007
    *   Edit BOM D-1010
    *   Muntin entry D-1018
    *   Stepped entry D-1022
    *   ITOE - entry and reworking D-1025
    *   Product replacement D-1029
*   Entry without prices D-1032
*   Price Calculation D-1032
*   Entry without prices D-1032
*   Delivery Notes D-1035
*   Invoices D-1036
*   Credit Notes D-1037
*   Order Release D-1038
*   Print D-1039
*   List printing D-1041
*   Overview Functions in Sales D-1042
    *   Overview D-1042
    *   Order Information D-1043
    *   Background checks D-1043
*   Resubmission D-1044
*   Modification Functions in Sales D-1047
*   Document change D-1048

## Introduction

The tutorial for the Sales module focuses on work in the sales department, the steps for which are depicted in A+W Enterprise. The tutorial builds on knowledge about the article master data and general commercial principles.

> **The functions depend on the released modules**
> Please note that the individual functions are available only if the corresponding modules and interfaces have been released.
> If you detect functions in this description that are not available in your version, please contact A+W Software GmbH.

### Prerequisite knowledge

The tutorial is aimed at users who are active in the Sales sector, who have daily contact with their own customers and suppliers, and who form a central position in A+W Enterprise for all operational flows.
These users have to be familiar with the concept of sales and the operating elements with which functions are called up and started. The basic principles of operation are described in the Overview section.
-> "Overview," on page A-52

### Goal of the tutorial

*   To provide an overview of the Sales functions.
*   To get to know the operating steps for selected topics.

### Tutorial structure

The tutorial consists of subjects with several training modules each. Each learning unit consists of the following elements:

*   **Overview**: Each training session starts with an overview of the major topics:
    *   Objectives: What shall be conveyed?
    *   Benefit: What can this knowledge be used for?
    *   Maxims: Which correlations are to be remembered?
*   **Concepts**: Concepts and terms of the corresponding training session will be explained first. This is followed by examples and operating instructions.

## General Operation and Shortcuts

A+W Enterprise can generally be operated both via the keyboard and with mouse support. The quick order enterer works primarily with the keys or with key combinations. Exiting a field in order to move down the dialog is generally done with the [Enter] key.
The following chapters provide you with the most important flows and frequently used keys and key combinations:
-> "Operation in the order" on page D-977
-> "Shortcuts" on page D-978
-> "Glossary" on page D-979
-> "Search for documents" on page D-980

### Operation in the order

*(Image: Fig. D-1 Flow scheme for document entry. A flowchart shows the progression from Header data, to Body data, to Footer, with options to reject or save the order.)*

The flow for document entry works according to a particular scheme. The combination of the keys `<Home>`/`<F12>` and `<End>` determines how far the document entry goes with what the result of the entry is.
*   Use `<Enter>` to move from field to field and change from one entry level to the other, e.g. from the header level to the body level.
*   Use `<Home>` or `<F12>` to go to the section above, or reject the order.
*   Use `<End>` to go to the section below or save the order.

### Shortcuts

The following table lists the most frequently used keys. The table may not be complete. Generally, within a dialog, you can use various other keys and key combinations, which are mentioned accordingly:

| Key | Explanation |
| :--- | :--- |
| `<Enter>`/`<Return>` | Use these keys to leave a field or a dialog and to confirm your entry. |
| `<Pos1>` | Use this key to leave a field or a dialog and discard your entry. |
| `<F1>` | Use this key to start the online help. |
| `<F2>`/`<Mode>` | Use this key to change between Shp dialogs if these exist. |
| `<F3>`/[Start] | Use this key to trigger an action. |
| `<F4>` | Use this key to start the supplementary menu. |
| `<F5>` | Use this key to start the detailed information about the current data record if there is one. |
| `<F6>` | Use this key to add a new line or a new record. |
| `<F7>` | Use this key to delete the line or field content. Depending on the context, you can also delete the current record with [F7]. |
| `<F8>` | Use this key to jump to the first record on a hit list dialog. Depending on the context, you can start a matchcode search with [F8]. |
| `<F9>` | Use this key to start the search for a value. |
| `<F10>` | Use this key to jump to the last record on a hit list dialog. |
| `<F11>` | Use this key to jump from one area to another if the areas are specified, e.g. as in the document entry. This way, you can skip some fields on the dialog. |
| `<F12>` | Use this key to move backwards on a dialog. |
| `<End>` | Use this key to exit a dialog and save the changes. |

### Glossary

| Term | Explanation |
| :--- | :--- |
| **Document type** | All commercial documents are saved program-internally in the database table `kauf`. These documents are distinguished by type. The number of the document type is assigned automatically by the system and has the fixed assignment:<br>- (Supplier) inquiries (`kauf.vorgang=1`)<br>- Purchase orders (`kauf.vorgang=2`)<br>- Receipt of goods (`kauf.vorgang=3`)<br>- Quotations (`kauf.vorgang=4`)<br>- Orders (`kauf.vorgang=5`)<br>- Delivery notes (`kauf.vorgang=6`)<br>- Invoices (`kauf.vorgang=7`)<br>- PU invoices (`kauf.vorgang=8`)<br>- Credit notes (`kauf.vorgang=9`)<br>- PU credit notes (`kauf.vorgang=10`)<br>- Product sets (`kauf.vorgang=14`) |
| **Order type** | You distinguish between different kinds of orders. Depending on the type of order in question, the orders are handled differently in the system:<br>- normal (`kauf._kaufart=0`)<br>- company-internal (`kauf._kaufart=1`)<br>- free (`kauf._kaufart=2`)<br>- Reservation (`kauf._kaufart=3`)<br>- Advance order (NIU) (`kauf._kaufart=4`)<br>- Advance invoice (NIU) (`kauf._kaufart=5`)<br>- Advance credit note (NIU) (`kauf._kaufart=6`)<br>- Calculation type (`kauf._kaufart=7`)<br>- group-internal (`kauf._kaufart=8`)<br>- On call order (`kauf._kaufart=9`)<br>- Stock order (`kauf._kaufart=10`)<br>- High-priority order (`kauf._kaufart=11`)<br>- Replacement order (`kauf._kaufart=12`)<br>- Reference price list (`kauf._kaufart=13`)<br>- Advance internet order (`kauf._kaufart=14`)<br>- Breakage order (`kauf._kaufart=15`)<br>- Customer stack order (`kauf._kaufart=16`)<br>- Stock stack order (`kauf._kaufart=17`)<br>- Dispatch order (`kauf._kaufart=18`)<br>- Gestrech (NIU) (`kauf._kaufart=20`)<br>- Return order (`kauf._kaufart=21`) |

### Search for documents

**Objectives**
*   Get to know A+W Enterprise document search.
*   Be able to use the dialog.
*   Know tips and tricks for the search function.
*   Recognize benefits of the function.

**Benefits**
*   The document search is one of the central functions, not just in Sales, but also in the entire A+W Enterprise program. The search for a particular document using less-familiar criteria enables the quick handling of tasks in the course of daily work.

> **Note**
> **Direct search**: This term includes the older direct `<F9>` search for document numbers. Here, only the start value number entry is possible. This search possibility must be activated explicitly if needed.
> **Extended search**: This search is already a standard function in A+W Enterprise. This is a search possibility with the entry of several search criteria. -> "Find orders" on page D-1069

You can search for existing documents (e.g. orders or quotations). Use `<F9>` from a document field to start the search dialog, whose fields are described in the following chapter:
-> Sales, "Find orders" on page D-1069

#### Here's how to search for an order
1.  Open the **Sales -> Order Entry** dialog.
2.  Start the search dialog in the **Order** field with `<F9>`. The dialog opens the first tab, **Document Codes**.
3.  Search for the document as follows:
    *   In the **Orders starting with** field, enter the document number (if known).
    *   Enter additional search criteria (for example, the customer's order number) if you want to restrict the search further.
    *   Use `<F2>` to change to the **Item Codes** tab to enter search criteria there as well.
    *   Use `<F3>` to start the search.
    *   Or, if you are still working with the old search logic, the dialog starts with the **Direct Search** tab.
        *   In the **Orders starting with** field, enter the document number (if known).
        *   Use `<F3>` to start the search.
    *   Or press `<Ctrl>` + `<T>` to open the **Document search**.
        *   Enter the search criteria (e.g. the customer's external number).
        *   Use `<F3>` to start the search.
        *   Load the desired document with `<F3>`.
    *   Or use `<F5>` to search for the external number.
    *   Or press `<Shift>` + `<F5>` to search for the reference.
4.  Confirm your entry with `<Enter>`.
5.  If the system reports that the document could not be found or is currently being processed by the system, change the search criteria and start the search again after a while.

> **Document search with <F8>**
> The search possibility with `<F8>` has been adjusted in A+W Enterprise: any user can now use `<F8>` to search in the Order field to view their last documents entered. It can be configured via an environment variable how many days in the past the document should count as *Last entered*.

## Overview of the Sales Menu

*(Image: Fig. D-2 Sales menu. A screenshot of the Sales menu dropdown, showing options like Quick Entry, Quotation Entry, Order Entry, etc.)*

In this module, there is an overview of the functions for commercial steps that occur in the sales department. This document includes the following chapters:
*   Quotations
*   Orders
*   Entry without prices
*   Delivery Notes
*   Invoices
*   Credit Notes
*   Order Release
*   Print
*   Overview Functions in Sales
*   Resubmission
*   Modification Functions in Sales

> **Scope of the tutorial in the Sales sector**
> The number of functions and their variety is extensive in the Sales sector. This tutorial includes only selected topics and does not claim to be complete. The tutorial is updated constantly.
> Many functions and steps can be used on many or several document dialogs. Such topics will be described exclusively in the Order Entry chapter.

## Quotations

**Objectives**
*   Get to know A+W Enterprise functions for quotation entry.
*   Operation in the quotation entry, insofar as there are differences from order entry.
*   Understand differences between quotations and orders.
*   Recognize function benefits and consequences.

**Benefits**
A quotation refers to a declaration of will that includes all components essential to a contract and that is created so that only the user's permission is required to conclude the contract. Therefore, A+W Enterprise offers all commercial functions for creating an extensive customer quotation.

> **Note: VOKA**
> Access to the Order Entry dialog is controlled by the EDI module abbreviation VOKA. For information about various other restrictions within order entry, please contact an A+W employee.

**Quotation entry** allows you to create a complete quotation for your customer, from the variety of products available. This quotation is assigned a quotation number and is saved under this number.
-> Sales, "Quotation entry" on page D-1131

The main difference between a quotation and an order is that for quotations, you do not need to enter the delivery date. Other differences will be discussed explicitly in this chapter.

If you enter a delivery date in a quotation, it can lead to resubmission or deletion of the quotation if you configure this in the system.
-> Sales, "Resubmission" on page D-1044

There is another simplification in the quotation regarding processing entry. If your customer wants to calculate a quotation with more than one same processing on the glass, e.g. with several drilled holes, you do not have to dimension these drilled holes individually in the quotation. You only enter the desired quantity for the processing. If an order arises from this quotation, this processing will be multiplied in order to dimension it individually for production.

In addition, in the quotation entry, you can get an overview of production utilization. This function offers you the opportunity while entering larger quotations to heed production deadlines and thus to avoid having to shift delivery dates. This function must be configured separately in the system. If you are interested, please contact an A+W employee.

A quotation has a flow status. You can find the **Angeb.Status** field in **Quotation > Dialog Header > Miscellaneous** tab. The following options are available for selection:
*   **open**: This status is set automatically in a new quotation.
*   **confirmed**: This status is set automatically in a new quotation as soon as an order with reference to the current quotation is created.
*   **lost**: This status must be set manually in a new quotation if the customer does not agree to the quotation. You can configure the system so that such quotations are deleted after a certain period of time. For additional information, see the following chapter: -> Sales, "Resubmission" on page D-1044
*   **undecided**: This status can only be set manually and is used for internal customer evaluations.

## Orders

With **order entry**, you enter the orders received from your customers and transfer them to the system for further processing. The individual processing steps will be scheduled based on the requested delivery date. Products kept in stock will be reserved while those to be ordered from one of your suppliers are passed on to Purchasing. After that, the order will be transferred to Production. At the end of the production chain, the order will be ready for delivery in Dispatch and it can be invoiced. The process is accompanied by the necessary papers. The possible changes are checked for feasibility before adjustment. The legal provisions are also included in the program.

There are many functions in order entry. Many steps depend on the configuration. Last but not least, the master data have particular consequences in order entry. In the following chapters, we will describe insofar as possible both the operating and configuration requirements explicitly.

A+W Enterprise order entry is split into three sections:
*   Header
*   Body
*   Footer

The frequently used functions are described in these areas. Especially documentation-worthy functions are in separate chapters, such as:
-> Sales, "ITOE - entry and reworking" on page D-1025
-> Sales, "Product replacement" on page D-1029

General partner data are entered in the order header, or are loaded from master data.
-> Sales, "Order header and footer area" on page D-986

Items are entered in the order body. They include the product information.
-> Sales, "Item entry" on page D-1000

The footer completes the quotation or order entry. The total is calculated, and discounts and surcharges are applied.

For detailed field descriptions of the fields on the Order Entry dialog, please refer to the following chapter in the "Software reference":
-> Sales, "Order entry" on page D-1133

This chapter describes how to enter orders. If you want to enter a quotation, open the **Sales > Quotation Entry** menu.

### Order header and footer area

**Objectives**
*   Get to know the variety of A+W Enterprise in the order environment.
*   Understand master data dependency and entry and changing this data in the order.
*   Recognize use of some important functions.

**Benefits**
*   Order entry is the core of A+W Enterprise. Order entry forms the basis of commercial, production-related, and legal processes. The functions that apply globally in an order are assigned to the order header. Order-completing actions are summarized in the footer area.

> **Note: VOKA**
> Access to the Order Entry dialog is controlled by the EDI module abbreviation VOKA. For information about various other restrictions within order entry, please contact an A+W employee.

In the header area, you specify the basis for an order. First the order number is assigned automatically by the system. The number assignment is done via so-called number ranges, which are specified during the installation and configuration. The numbers for the orders are not without gaps: if an order is discarded and a subsequent order has already been entered, then the discarded number will not be reused. However, this logic is not used in the invoice and credit note entry.

#### Enter new order

##### Here's how to enter an order
1.  Open the **Sales -> Order Entry** menu element. A+W Enterprise shows the selected dialog.
2.  Press `<Enter>` in the **Order** (or Quotation) field. A+W Enterprise automatically assigns and shows the next free document number. The cursor goes to the **Customer** field.
    -> Sales, "Order" on page D-1134
3.  Select a customer:
    *   Enter the customer number, if you know it.
    *   Or press `<F9>` to search by customer number, or `<F8>` to search by matchcode. The **Search partner** dialog opens. The cursor is on the **Starting with number** field if you start with `<F9>` or on the **Matchcode** field if you start with `<F8>`:
        *   Enter the search criteria.
        *   Use `<F3>` to start the search.
        -> Software Reference, "Find market partner" on page D-1087
        -> Sales, "Customer" on page D-1135
4.  If you enter the order with reference to an existing document, carry out the following steps:
    -> Sales, "Here's how to enter a new order with reference to an existing quotation or order" on page D-990
5.  Use the `<Enter>` key to go through the fields up to **Date**. If you have to enter a date other than today as **Entry Date**, the program makes you enter it twice.
6.  Enter the delivery date requested by the customer in the **Date** as CW (calendar week) field or as a fixed **Date**. Entry of the delivery date is only mandatory for an order. Note the consequences of the delivery date entry for quotations:
    -> Sales, "Resubmission" on page D-1044
    If you are working with the route plan, you can also select a route day directly. To display all route days in the selected week, press `<F9>` and choose the date. This function is available only if you are using the route plan.
    -> Master Data, "Route plan" on page B-263
    Based on several criteria such as calendar entries, route days, driving and handling time, the program calculates a planned delivery date right away. The possible shift by production is only done when the order is transferred.
7.  Assign the document to a project (optional) to take into account special conditions for this document.
    *   Press `<F9>` in the **Project** field. Select a project from the list. All project-related fields will be preset from master data.
8.  Enter the references (optional) to enter reference text.
    -> Sales, "Order with consignments" on page D-992
9.  With another `<Enter>` you can reach the item entry. Use the steps described below for this:
    -> Sales, "Here's how to enter an item with article number" on page D-1001

##### Here's how to influence rush surcharge calculation
1.  Enter an order header up to the **Date** field.
2.  In the **Date** field, enter a date in the near future.
    You can determine the rush date in the system configuration; that is, up to how many days in the future orders count as rush orders.
    The selected date must be in the period between TODAY() + rush date.
3.  In the **Term. Art** field, select the value **rush**.
4.  Enter the order up to the **Discount** field in the order footer.
5.  Use `<F2>` to change to the discount overview. If you have stored a rush order surcharge, this is determined automatically.
    You should define a rush order surcharge in advance under **Master Data > Keys > Market Partners > Document Discounts > Discounts**.
    Note here that it is not the **Rush order** field on the Properties tab that is evaluated for the surcharge.
    You can also recalculate all discounts and surcharges via the menu `<F4> > Price Details > Recalculate Discounts`.
6.  Enter the order to the end.

##### Here's how to save the order temporarily
Especially for larger orders with several items or complicated entries, it is advised that you save the order in question temporarily. The advantage is that if a problem occurs, you will be able to use the saved state after restart.
1.  Enter an order header up to the point that seems sensible for saving. However, at least one item must be entered completely so that the Save button is activated automatically.
    A data record is created in the table `kauf` with `kauf.still=999`.
2.  You can save the order again at a later time, e.g. after entering additional items. Here the first data record saved in the table `kauf` is overwritten.
3.  If an order is entered completely and saved, the `kauf.still=-3` is set and the order will be presented to the background process `intauf` for further processing. Alternatively, the order entered can also be placed in the release pool.
4.  In the case that the entry is interrupted by a technical problem so that A+W Enterprise has to be restarted, the program offers the following possibility:
    *   When starting the order entry, you get a notice that there are still documents whose entry has not been completed.
    *   If you confirm this notice, the overview dialog with the saved documents opens:
        *   All documents are displayed on this dialog whose entry was not completed and for which there is a back-up.
        *   Use [Cancel] to close this overview dialog and return to the Order Entry dialog. You can edit documents not completely entered at a later time. This overview dialog always starts when entering order entry as long as there are additional documents.
        *   If you use [OK] or previous document selection if there are several documents, you start the document for further entry. The last backed-up status of the document is restored.
5.  Then you can continue entering the document.

> **Limitations**
> Please note the following limitations:
> *   Backed-up documents are kept in the system for a maximum of 30 days.
> *   The overview dialog lists only the individual documents, that is, not those from another user.
> *   The Save function is available for quotations, orders, inquiries, and POs.

### Enter order with reference
You can enter a new order (or quotation) with reference to an existing quotation or order. Here the data from the reference document are copied and you can adjust them or process them further in the new document. An order or quotation from any customer can be used as an order reference. In rare cases, a supplier inquiry or a PO can also be transformed into a sales document. Here, the data for the new document must be checked carefully.
-> Sales, "Pre-selecting document type for the reference" on page D-1135

Please note that you may have to change some information such as the delivery date in field **Date** or the reference text. You may have to recalculate the order. This applies especially if you have copied other customers' documents to the order.

> **Enter an order with reference to quotation for the same customer**
> To change a quotation into an order for the same customer, you can enter the quotation number in **Reference** field. The existing data from the quotation will be loaded into the dialog. This procedure is only possible, however, if the system is configured for the standard reference document=Quotation.
> A+W Enterprise automatically assigns the quotation the quotation status *received* (**Quotation > Miscellaneous tab > field Spec. Status = received**). This information can be used if necessary for customer-specific evaluations and statistics.

#### Here's how to enter a new order with reference to an existing quotation or order
1.  Start the **Order Entry** dialog. Use `<Enter>` in the **Order** field to assign a new order number.
2.  Enter the desired customer number or select it.
3.  Proceed as follows in the **Reference** field:
    *   Use `<F8>` to select the document type of the document to which reference will be made.
        *   The standard default setting for the document type is specified in the system settings and displayed here.
        *   Confirm the default value with `<Enter>`.
    *   Or use `<F9>` to select another document type.
        *   Select the document type of the reference document from the list.
        *   Confirm your entry with `<Enter>`.
    *   Next, the customer number will be taken over into the field from the new order.
    *   You can confirm the current customer number with `<Enter>`.
    *   To refer to another customer's document, enter his customer number or open the partner search with `<F9>`. For inquiries and purchase orders, only the suppliers will be displayed for selection.
    *   Confirm your entry with `<Enter>`.
    *   Enter the document number or search for all documents of the selected type for this customer using `<F9>`.
    *   Confirm your selection and exit the **Reference** field with `<Enter>`.
    *   The **Reference** field displays the document number.
4.  The data for the selected reference document can be copied either completely or just the header data to the new document.
5.  Furthermore, some data can be redetermined or recalculated, e.g.:
    *   **Recalculation of the order to be entered:** The query about recalculation is posed on a separate dialog. This query is always pre-populated with the value *No recalculation*. Via a system setting, you can determine these default settings yourself. The following values are possible:
        *   0 - No recalculation (default setting)
        *   1 - SA + PU prices
        *   2 - SA prices
        *   3 - PU prices
    This way you can configure which value is pre-populated during entry with reference. In addition, you can determine which value is pre-populated if in the new document the recalculation is called in the header or in the item, insofar as this function is used.
    *   **Discount determination in the order to be entered:** if there are market partner-related discounts in the document and the document entry with reference causes a market partner change, you can decide whether the discounts will be recalculated. You will be asked to do this by a program message.
6.  You can now continue order entry; if necessary, use the information described in the following chapters:
    -> Sales, "Here's how to enter an order" on page D-986
    -> Sales, "Enter new items" on page D-1001

### Order with consignments
A consignment is a group of particular items of an order under a certain header. Depending on how the field **Consignment** is configured, the cursor jumps from the **Project** field to the **Consignment** field or skips the field so that you can start to enter the first item.
-> Sales, "Ref." on page D-1167

#### Here's how to enter a consignment text
You can enter consignment text to be printed on both the documents and on the label.
1.  Start the order entry and enter the data in the order header as described in the following chapter:
    -> Sales, "Here's how to enter an order" on page D-986
2.  Enter the consignment text in field **Consign.**
    The text can exceed the visible field length. Use the `<arrow keys>` (left/right) to view the text.
3.  Confirm your entry with `<Enter>`. This consignment applies for the entire order. If you would like to enter an item-specific consignment text, move to the item level with the menu path `<F4>` **consignments > New Consignment**. The cursor goes to the first item on tab **General**.

#### Here's how to enter further consignment texts
The consignment text will be kept for all following items until you enter a new text. New consignment text for the following items can be entered as follows.
-> Sales, "Order entry - general" on page D-1165
1.  For the item to be changed, press `<Shift>` + `<F11>` on the **General** tab. The cursor goes to field **Consign.**.
2.  Change the consignment text as required and confirm your entry with `<Enter>`. The cursor returns to the item in tab **General** you have just edited.

#### Here's how to change consignment texts
You can change or correct consignment texts. The changes refer to all items for which this consignment is valid, even to all previous ones.
1.  For the item to be changed, press `<Ctrl>` + `<F11>` on the **General** tab. Or use `<F4>` to load the **Supplementary menu**.
    *   Select **Consignment**.
    *   Select sub-menu **Change consignment**.
    The cursor goes to field **Consign.**.
2.  Change the consignment text as required and confirm your entry with `<Enter>`. The cursor returns to the item in tab **General** you have just edited.

### Addresses in the order
You can enter or select a different shipping address for the order than the address from the master data. The field description for the **Addresses** dialog is in the following chapter:
-> Master Data: Software Reference, "Addresses" on page B-139

The function scope for the determination, entry, and takeover of addresses in a document is extensive. An address change can cause a subsequent change in other areas, such as:
*   Redetermination and calculation of delivery surcharges and other discounts.
*   Change of the type of the EDI and PO-related data
*   New transfer to production insofar as the order is production-relevant
*   Effects on rack planning and dispatch control, etc.
It must therefore be noted that the changes to an existing address can affect not just an existing or new document, but under some circumstances, a series of documents.

> **Address logic**
> Contact an A+W employee if you can to adjust and configure customer and shipping addresses to the way you work.

#### Here's how to select a different shipping address
You can select a different shipping address for this order or enter a new one.
-> Sales, "New delivery address" on page D-1191
1.  Press `<Ctrl>` + `<L>` in the order. Or use `<F4>` to call up the **Supplementary** menu.
    *   Select **Addresses**.
    *   Choose the **Select shipping address** submenu.
    The **Address Search** dialog opens.
2.  On the search dialog, you can restrict the search to particular criteria. For the dialog description, see the following chapter:
    -> Sales, "Find addresses" on page D-1095
3.  Use the mouse or the `<arrow keys>` to select an address from the hit list, and confirm your selection with `<Enter>`.
4.  Quit the dialog using `<End>`. A+W Enterprise closes the dialog and shows the selected address as shipping address for this order.

#### Here's how to enter a new shipping address
You can enter a different new shipping address for the order. The new address can be taken over in the master data as one-time address (only applies to this order) or for further use.
1.  Use `<F4>` > to select the **Supplementary menu > Addresses > New Shipping Address**.
2.  Fill out the fields for a new address.
    You can use an existing address as template. Use the `<Template>` button to start the Address Search again; you can use this to select a new address. Change the details if necessary.
3.  Then you can store the new address in the market partner master data with `<F3>`. Alternatively, the new addresses are only valid in this order after saving.
4.  Quit the dialog using `<End>`. A+W Enterprise closes the dialog and shows the selected address as shipping address for this order.

#### Here's how to delete a shipping address
You can delete the shipping address in the order.
1.  Use `<F4>` to call up the Supplementary menu.
2.  Select **Addresses**.
3.  Select the sub-menu **Delete shipping address** and confirm with `<Enter>`. A+W Enterprise deletes the shipping address from the order.

### Enter text and phrases
You can enter and insert text in various places. The generation and output of texts is done automatically in the rules based on the system configuration, the master data, and other settings.

#### Here's how to enter order header or footer text
This item on the **Supplementary menu** in order entry allows you to enter free text to be printed in the order header or footer of customer-bound documents.
-> Sales, "Texts submenu" on page D-1062
-> Sales, "Header and footer texts" on page D-1308
1.  Use `<F4>` to call up the **Supplementary menu** then select **Text**.
2.  Select the **Header** or **Footer** submenu. A+W Enterprise opens a dialog for text input.
3.  Enter the required text or choose a text element (predefined in master data) from the list.
4.  Finish text input with `<End>`.

#### Here's how to create new text elements (phrases) or change these
You can define individual text elements (phrases) or change existing ones as required.
-> Sales, "Header and footer texts" on page D-1308
Start the **Header Text** or **Footer Text** dialog from the `<F4>` menu.
1.  To save a new text element in the master data, press `<Shift>` + `<F10>` on the **Header Text** or **Footer Text** dialog or use the **[New phrases]** button. A+W Enterprise opens an input dialog.
2.  Enter a new code and confirm with `<Enter>`. The code for the phrase can be numeric and alphanumeric.
3.  Enter the text for the new text element or change the existing text and confirm with `<Enter>`.
4.  Use `<End>` to quit the dialog.

### Additional documents in the order
You can assign or add documents to an order or individual order items, e.g. scanned sketches, CAD drawings, notes, emails, etc. These can be deleted if required.

> **Information on saving data**
> Please make sure that the file name does not contain special characters or blanks. The file cannot be saved otherwise.
> -> Sales, "Allocation of document types" on page D-1223

#### Here's how to assign documents
1.  Use `<Ctrl>` + `<K>` to assign files
    *   starting from field **Cust.Itm** in the order header and/or footer if you want to assign a file to an order.
    *   in the order body, tab **General**, in the corresponding item to assign a file to an individual item.
    A+W Enterprise opens the dialog **File assignment**.
    *(Image: Dialog 'Allocation of Document Types' with a file 'ASSkizze.JPG' assigned.)*
2.  Open the (Windows) Explorer and mark the file in question.
3.  Use to mouse to drag this file to the folder icon on the **File assignment** dialog and press [OK].
    The file name and the assigned item are displayed on the **File assignment** dialog and are saved in the database.
    Repeat the process to assign further files.
4.  After the assignment, the folder icon may change depending on what icons are used for the default applications on your computer.
5.  To remove a file from an order, mark the required entry then press [Delete]. The file is removed from the document.

### Complete order entry
The order can be completed when all customer and item data have been entered.
When you save the order, the data will be processed for and transferred to other A+W Enterprise components (production, purchasing, stock, dispatch).

#### Here's how to save or reject an order
1.  Confirm your entry in field **Net total** with `<Enter>` or quit the addition area with `<End>`.
    If you do not want to save the order, press `<Home>` repeatedly to reject all entries.
2.  Confirm the query about whether the order is complete with [YES].
3.  Confirm the question as to whether the order shall be released for further processing with [YES] to transfer the data immediately to production, purchasing, stock, and dispatch.
    If you answer this question with [No], the order will not be released. The order has been saved and is now in the release pool. You can release it later.

### Change/correct order
Changes to an order after the fact include all changes after the first saving of the order. It is recommended that you make all changes in the order before the order is locked in *local correction*. If, however, you would like to permit changes up to a certain degree, contact an A+W employee to configure your system accordingly. Please note that there are changes that are only made in the individual items and changes that are made on the order header level. Changes on the header level mean that the change type is not transferred to all non-canceled items if the class of the change is higher than any present in the item. If, for example, the quantity is changed in an item and then the shipping address, then all non-changed items receive the status "Info to production" (`kpos.aendkz=4`) and the changed position then "production-relevant change" (`kpos.aendkz=5`).

The following chapter assumes that the order changes are permissible:
*   Sales, "Here's how to add additional items" on page D-1003
*   Sales, "Here's how to edit the properties of individual items" on page D-1003
*   Sales, "Here's how to change supplier-related data" on page D-1004
*   Sales, "Here's how you can change an article in the BOM" on page D-1012

Orders can be changed in mode **Correction** and **local correction**.
They cannot be changed in the modes **Global local correction**, **cancelled (system or user)** and **Invoiced**.
Whenever an order is changed, A+W Enterprise checks the limit and the contribution margin.
Generally the user entering the order (`kauf.eusr`) is informed of the change. If you configure e-mail dispatch, the employee receives an e-mail.

Furthermore, it is possible to configure the system so that order changes that are made by the system, e.g. shipping date change or incorrect scheduling do not go to the user entering the order, but rather to the employee who made the last change to the order. This makes the information chain clearer.

#### Here's how to change an existing order
1.  Load the order in question.
    *   Enter the order number if you know it.
    *   Or search for the order.
        -> Sales, "Overview" on page D-1042
2.  Change the appropriate fields in the order.
    If you change the delivery date for instance, the **Cause** field appears. Enter the cause for the change of delivery date.
3.  Use `<End>` to quit the order.
4.  Rerun packaging planning if necessary.
    -> Sales, "Specs. packaging planning" on page D-1292
5.  Answer the question **Transfer the change to purchasing, stock, and production?** with Yes or No and decide whether the change has to be transferred.

> **Please answer this question explicitly!**
> For all changes relevant for purchasing, stock, and production, you must answer with [Yes].
> Please note that changed or added items will not be transferred to production if you answer this question with [No]. The order will not be passed on, and will not be transferred to the release pool!

#### Here's how to view the delivery date change log
Use `<Shift>` + `<F4>` to open the menu **Delivery date changes** menu element. The **Delivery date change log** dialog shows all changes. The latest change will be displayed only after you have saved and reopened the order.
-> Sales, "Delivery date change log" on page D-1230

#### Here's how to recalculate an order
With changed payment conditions, it can happen that an existing order must be recalculated. This possibility assumes that the order in question is not yet invoiced. If you want to re-present several orders for cost calculation, use the function on the **Document Change** dialog.
-> Sales, "Here's how to recalculate a quotation or an order" on page D-1050
1.  Load the order in question.
    *   Enter the order number if you know it.
    *   Or search for the order.
        -> Sales, "Overview" on page D-1042
2.  Place the cursor on one of the following fields: **Ent.Date**, **Cust.POnr.**, **Date**, **Route** or **Cust.Item**.
3.  Use `<Ctrl>`+`<F9>` to initiate the recalculation of the document. You can choose:
    *   No calculation
    *   Sales prices
    *   Purchase prices
    *   Sales and purchase prices
4.  Then you must save the document and exit with `<End>`.

## Item entry

**Objectives**
*   Get to know various functions on the item level.
*   Note possibilities and restrictions of item entry.
*   Get to know the functions on the item level.

**Benefits**
The functions on the item level can help with fast and safe order entry. On the item level, individual products are entered that the customer orders. Preventing entry errors reduces possible mistaken production.

> **Note**
> **Edit BOM**: This function offers the possibility to make changes to the existing BOM. You can call up this function with `<F5>` directly after entering the article number, however, the BOM structure will only be edited after the complete dimensioning.
> **Attachments (1)**: In a document on the header/footer level and also on the item level, documents can be assigned with `<Ctrl>`+`<K>`. The **Attachments(X)** button indicates with a number in parentheses how many documents have already been assigned. You can use this button to start the document assignment.

The individual order items are entered after the same fashion.
-> Sales, "Order items" on page D-1165

The properties for the entry of various product types (e.g. base glass, TG, LAMI, IG, muntins, processings, fittings, services, etc.) are in the following chapter:
-> Sales, "Entering items (depending on product type)" on page D-1007

Extensive or complex topic blocks will be described in separate chapters, e.g.:
-> Sales, "iTOE - entry and reworking" on page D-1025
-> Sales, "Product replacement" on page D-1029

