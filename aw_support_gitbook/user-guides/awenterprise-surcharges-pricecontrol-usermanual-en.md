---
title: "EN-UM-AWEnterprise_9"
source: "EN-UM-AWEnterprise_9.pdf"
tags: ["A+W Enterprise", "Software Reference", "Surcharges", "Price Control", "Conditions", "Pricing", "Glass Manufacturing", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference manual for A+W Enterprise, focusing on the configuration of surcharges, price controls, and conditions. It details how to manage various types of surcharges like shape, size, thickness, and processing group surcharges, and explains the setup of price control rules, bonus rules, and price list logic."
long_description: "This section of the A+W Enterprise Software Reference manual provides a comprehensive guide to configuring pricing structures, specifically focusing on surcharges, price controls, and various conditions. The document begins by explaining different types of surcharges, including shape, special shape, surcharge matrices, thickness vectors, and size surcharges. For each type, it describes the navigation path within the software, provides an overview of the user interface, and details the functionality of each field. This includes setting up percentage-based surcharges, minimum amounts, and surcharges for specific product groups or processing steps. The manual then transitions to 'Price Control,' where it outlines how to define rules for price calculations across different plants, set up discounts for bulk orders (e.g., Tmp price control), manage margins, and establish bonus rules. It also covers the logic for price list control and restrictions. The 'Conditions' section explains how to set up market-partner or product-group-specific conditions, distinguishing between daily, special, and product-group-specific rules. It covers general daily conditions, product group conditions, and then moves into 'Special Conditions,' which allows for more granular control over pricing for individual customers, suppliers, or objects. This includes special general conditions, product group conditions, article conditions, discount scaling, and various factor-based adjustments. The document concludes with 'Special Prices,' detailing how to override standard price lists for specific articles, variants, or processing types, ensuring flexible and precise pricing for any scenario within the A+W Enterprise system."
---

# Software Reference

---
## Surcharges

### Shape surcharges

**Master data > Prices > Surcharges > Shape surcharges**

Non-rectangular shapes (shapes) require higher prices than standard articles due to the increased amount of processing and handling they require. That's why surcharges on shapes can be managed separately.

These shape surcharges are defined for the glass price and for processings. You can create percentage surcharges for glass articles, processings, and accessory articles.

How the shape surcharges are calculated depends on the setting in the conditions or on a marker partner-specific setting.

⇨ "Conditions" on page C-827

In the price control, you can further define the calculation of the shape surcharges. For example, for the TG price control, you can specify that starting with a particular number of shapes, the shape surcharged is reduced by a certain percentage.

⇨ "Price control" on page C-821

For articles to which a shape is assigned in the article master data, no model surcharge is calculated.

The shapes are maintained under **Master Data > Keys > System > Shapes**.

⇨ Master Data, "Edge allocation" on page B-249
⇨ Master Data, "Shape descriptions" on page B-251

The following views are available for this dialog:

*   "Shape surcharges - overview" on page C-802
*   "Shape surcharges - details" on page C-804

---

### Shape surcharges - overview

**Master data > Prices > Surcharges > Shape surcharges**

*Abb. C-164 Shape surcharges - overview*

| Shape | Prod. Group | PLCD | Site | Shape Type | Surch. | Minimum | Processing |
| :---- | :---------- | :--- | :--- | :--------- | :----- | :------ | :--------- |
| 1     | 104         | 29   |      | IG-shape   | 40.00  |         | 40.00      |
| 1     | 105         | 29   |      | Lami-shape | 30.00  |         | 30.00      |
| 1     | 204         | 29   |      | IG-shape   | 40.00  |         | 40.00      |
| 2     | 104         | 29   |      | IG-shape   | 40.00  |         | 40.00      |
| 2     | 105         | 29   |      | Lami-shape | 30.00  |         | 30.00      |
| 2     | 204         | 29   |      | IG-shape   | 40.00  |         | 40.00      |
| 3     | 104         | 29   |      | IG-shape   | 70.00  |         | 70.00      |
| 3     | 105         | 29   |      | Lami-shape | 30.00  |         | 30.00      |
| 3     | 204         | 29   |      | IG-shape   | 70.00  |         | 70.00      |
| 4     | 104         | 29   |      | IG-shape   | 70.00  |         | 70.00      |
| 4     | 105         | 29   |      | Lami-shape | 30.00  |         | 30.00      |
| 4     | 204         | 29   |      | IG-shape   | 70.00  |         | 70.00      |
| 5     | 105         | 29   |      | Lami-shape | 40.00  |         | 40.00      |
| 5     | 204         | 29   |      | IG-shape   | 70.00  |         | 70.00      |
| 6     | 105         | 29   |      | Lami-shape | 40.00  |         | 40.00      |
| 6     | 204         | 29   |      | IG-shape   | 70.00  |         | 70.00      |
| 7     | 204         | 29   |      | IG-shape   | 100.00 |         | 100.00     |
| 8     | 204         | 29   |      | IG-shape   | 100.00 |         | 100.00     |
| 9     | 204         | 29   |      | IG-shape   | 100.00 |         | 100.00     |
| 10    | 204         | 29   |      | IG-shape   | 100.00 |         | 100.00     |

On this overview, you maintain the surcharges for shapes and processings on shapes. The surcharge for a shape is charged depending on the system configuration and setting in the conditions on the price-relevant components of the article produced. The surcharges apply starting with a specified PLCD.

You can create different surcharges per shape, which refer to the product group or to the shape type.

**<F2>**
Change to the detailed view.
⇨ "Shape surcharges - details" on page C-804

**<F4>**
Change to the Global Price Maintenance dialog.
⇨ "Global price maintenance" on page C-698

#### Field descriptions

**Shape**
Selection of the shape for which the surcharge is charged.
Technical info: numeric field, DB field: pkzmod.modnr

**Product group**
Selection of the product group for which the surcharge applies.
If you specify a product group, the Shape Type field is locked.
The price is then searched for using the product group logic. During the search, the product group is considered in the order item, not the product group from the master data.
Technical info: numeric field, DB field: pkzmod.wagrp

---

> **Example**
>
> The article in the order item belongs to product group 10 A2 21.
>
> During the price calculation, A+W Enterprise checks whether a surcharge is defined for precisely this product group. If no surcharge is found, A+W Enterprise searches in the product group 10 A2 **. If there is no surcharge found here, the product group 10 ** ** is checked.
>
> With an appropriate system setting, A+W Enterprise searches precisely to the place, that is, in the sequence: 10 A2 21, 10 A2 2*, 10 A2 **, etc.

**PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any surcharge in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which a surcharge is defined.
⇨ Tutorial, "From-PLCD logic" on page C-552
Technical info: numeric field, DB field: pkzmod.pkz

**Site**
Selection of the site for which the prices are defined (only in multi-site system).

**Shape type**
Selection of the shape type for which the surcharge applies. If you select the shape type, you may not specify a product group.
Technical info: alphanumeric field, toggle field, DB field: pkzmod.modeltyp

**Surcharge**
Specification of the percentage that is calculated for shapes.
With appropriate system configuration, this surcharge also applies for muntins.
How the shape surcharge is calculated depends on what is stored in the conditions. The surcharge is always calculated as a percentage of the glass unit price, from the basic price of the header article or from the basic price of the glass including any exchange glass.
Technical info: numeric field, DB field: pkzmod.zusch

**Minimum**
Specification of a fixed amount as minimum surcharge for the shape. The surcharge is charged in the specified currency on the glass price.
In the order, the minimum surcharge is charged if the calculated shape surcharge is less than this minimum surcharge.
Technical info: numeric field, DB field: pkzmod.minzusch

**Processing**
Specification of the percentage for processings or accessory articles for shapes. This surcharge does not apply for muntins in shapes.
This surcharge is only charged if in the master data the price calculation on the Price Properties dialog is activated for the processing or the accessory.
⇨ Master Data, "Price characteristics" on page B-444
Technical info: numeric field, DB field: pkzmod.beamodzusch

---

### Shape surcharges - details

**Master data > Prices > Surcharges > Shape surcharges > <F2>**

*Abb. C-165 Shape surcharges - details*

On this dialog, you can edit the shape surcharges individually.

**<F2>**
Change to overview.
⇨ "Shape surcharges - overview" on page C-802

**<F4>**
Change to the Global Price Maintenance dialog.
⇨ "Global price maintenance" on page C-698

#### Field description

The fields are described for the Shape Surcharges - Overview dialog:
⇨ "Shape surcharges - overview" on page C-802

---

### Special shape surcharges

**Master data > Prices > Surcharges > Special shape surcharges**

On this dialog, you can display and edit all shape surcharges for a shape number. If you do not specify a shape number, alternatively you can display all shape surcharges that are defined for the selected price list code (PLCD).

For the special shape surcharges, the same conditions apply that are described on the Shape Surcharges dialog.
⇨ "Shape surcharges - overview" on page C-802

The following views are available for this dialog:

*   "Special shape surcharges - overview" on page C-805
*   "Special shape surcharges - details" on page C-806

#### Special shape surcharges - overview

**Master data > Prices > Surcharges > Special shape surcharges**

*Abb. C-166 Shape surcharges - overview*

| Shape | Prod. Group | PLCD | Site | Shape Type | Surch. | Minimum | Processing |
| :---- | :---------- | :--- | :--- | :--------- | :----- | :------ | :--------- |
| 4     | 104         |      | 29   | IG-shape   | 70.00  |         | 70.00      |
| 4     | 105         |      | 29   | Lami-shape | 30.00  |         | 30.00      |
| 4     | 204         |      | 29   | IG-shape   | 70.00  |         | 70.00      |

On this overview, you maintain all shape surcharges for a shape number. Alternatively, you can display all shape surcharges that are defined for a price list code (PLCD).

**<F2>**
Change to the detailed view.
⇨ "Special shape surcharges - details" on page C-806

---

#### Header

**Shape**
Specification of the shape number for which the shape surcharges should be displayed. If you do not specify a shape number, alternatively you can display all shape surcharges that are defined for the selected PLCD.
Technical info: numeric field, DB field: pkzmod.modnr

**Site**
Selection of the site for which the prices are defined (only in multi-site system).

**PLCD**
Selection of the price list code (PLCD) for which the shape surcharges should be displayed. If you do not specify a PLCD, alternatively you can display all shape surcharges that are defined for the selected shape number.
Technical info: numeric field, DB field: pkzmod.pkz

#### Field descriptions

The fields and functions are described for the Shape Surcharges - Overview dialog:
⇨ "Shape surcharges - overview" on page C-802

#### Special shape surcharges - details

**Master data > Prices > Surcharges > Special shape surcharges > <F2>**

*Abb. C-167 Shape surcharges - details*

On this dialog, you can display and edit a particular shape surcharge individually.

**<F2>**
Change to overview.
⇨ "Special shape surcharges - overview" on page C-805

#### Field descriptions

The fields and functions are described for the Shape Surcharges - Details dialog:
⇨ "Shape surcharges - details" on page C-804

---

### Surcharge matrices

**Master data > Prices > Surcharges > Surcharge matrices.**

*Abb. C-168 Surcharge matrices*

On this dialog, you maintain scaled surcharges in the form of matrices.
⇨ Tutorial, "Surcharge matrix" on page C-627

In a surcharge matrix, you can create the following surcharges:

*   Percentage surcharges.
*   Fixed amounts in a currency, e.g. €, SFR, $, ...
*   Piece discounts.

You can assign the surcharge matrices except for the single lites to the following prices:

*   IG basic prices.
*   Article vectors.
*   Processing vectors.
*   Single lites for IG articles.

#### Field descriptions

**Site**
Selection of the site for which the prices are defined (only in multi-site system).

**Matrix**
Selection of the surcharge matrix. If you want to create a new surcharge matrix, specify a unique matrix number.
Technical info: numeric field, DB field: zumat.matnr

---

**Name**
Display or input of the name of the surcharge matrix. If you create a surcharge matrix, select a brief description of the purpose as name, e.g. overlengths LAMI.
Technical info: alphanumeric field, DB field: zumat.bez

**Priority**
Specification whether the surcharge matrix should have a higher priority for the price calculation than the size surcharges. The field is only displayed with appropriate configuration.

The prioritization is only considered for the pricing methods IG-current, Calculation by single lites, and PCD-LAMI.

*   **Y:**
    The surcharge for a single lite has higher priority than the size surcharges. If for the price calculation in this surcharge matrix a surcharge is found, the size surcharges are no longer evaluated.
*   **N:**
    The surcharge for a single lite from this surcharge matrix does not have a higher priority than the size surcharges. The size surcharges are also evaluated.
    ⇨ Tutorial, “Size surcharges" on page C-629

Technical info: alphanumeric field, toggle field, DB field: zumat.prio

**Type**
Specification of to what the surcharge or discount refers:

*   **CU Value:**
    The surcharge or discount is calculated as fixed amount.
*   **Percent:**
    The prices are calculated as a percentage of the basic price of the header article. This price type is only selected for exchange articles or processings.

Technical info: alphanumeric field, toggle field, DB field: zumat.typ

**Type**
Selection of the surcharge type. With this entry, you specify according to what the surcharge is scaled and how the surcharge is determined. The fields for the surcharge values are displayed accordingly for the selected surcharge type:

*   **Area:**
    The surcharge applies starting with the specified areas.
*   **Longer edge:**
    The surcharge applies starting with a specified length. Here, the length of the longer edge of the glass in the order item is always used.
*   **Side ratio:**
    The surcharge applies starting with the specified side ratio.
*   **Oversize surcharge:**
    The surcharge applies starting with the specified size (edge lengths).

---

*   **Glass basic price:**
    The surcharge applies if the surcharge matrix is assigned to a processing vector. As surcharge, you can only specify a single value, which depending on type is interpreted as percentage or fixed amount. The surcharge is charged on the basic price of the header article.
    If an IG is calculated by single lites, the basic prices of all single lites is increased.
    In addition, you can specify a minimum surcharge that is charged in addition regardless of the glass dimensions.
    Technical info: alphanumeric field, toggle field, DB field: zumat.art

**Min. price**
Specification of the minimum price of the surcharge. This price is charged if the calculated price in the order item is less than the specified minimum price.
*   Minimum prices for header articles are only evaluated for the pricing methods IG-Switzerland, PCD-LAMI, PCD-tempered, PCD-basic glass, PCD-finished glass or PCD-prices.
*   Minimum prices for BOM subparts are only evaluated if for the header article the pricing method IG-current, PCD-LAMI, PCD-tempered, PCD-basic glass, PCD-finished glass or PCD-glass doors is selected and the subpart is an accessory item with the pricing method PCD prices-general.
The field is only enabled with the surcharge type Glass basic price.
Technical info: numeric field, DB field: zumat.minpreis

**Limit values (rows, column header)**
Specification of the limit values starting with which the specified surcharge is charged.
*   If you have selected Longer edge, Side ratio or Oversize surcharge as surcharge type, specify the length in millimeters starting with which the surcharge should apply. In the columns, you specify the values for the longer edge; in the rows, the values for the shorter edges. Depending on the configuration, the edge lengths are evaluated with or without round size.
*   If you have selected Area as surcharge type, specify the area in square meters starting with which the surcharge should apply.
*   If you have selected the surcharge type Glass basic price, you cannot specify limit values.
Technical info: numeric fields, DB fields column header: zumat.lk1, zumat.lk2 ... zumat.lk6, DB fields row header: zumat.kk1, zumat.kk2 ... zumat.kk6, DB fields for surcharge type area: zumat.fl1, zumat.fl2 ... zumat.fl6

**Fields of the matrix**
Specification of the surcharge values. Depending on the surcharge type, the value is interpreted as percentage or amount.
*   **Longer edge, Side ratio or Oversize surcharge:**
    Depending on the configuration, the edge lengths are evaluated with or without round size. If the price-relevant length is greater than or equal to the specified limit value, the specified surcharge is charged.
*   **Area:**
    The area is calculated with the rounded dimensions. If the price-relevant area is greater than or equal to the specified limit value, the specified surcharge is calculated.
*   **Glass basic price:**
    You can only specify a single value, which depending on type is interpreted

---

as percentage or fixed amount.
Technical info: numeric fields, DB fields: zumat.zu11, zumat.zu12, ... zumat.zu16, zumat.zu21, zumat.zu22, ... zumat.zu26, ... zumat.zu66

#### Discount per piece

**from**
Specification of the discount limit values in pieces.
The discounts are only evaluated if the surcharge matrix is assigned to an article price. In addition, the header article has to be assigned the pricing method PCD-LAMI, PCD-tempered, PCD-basic glass, PCD-processing or PCD-prices general.
⇨ Tutorial, "Pricing methods" on page C-559
Technical info: numeric fields, DB field: zumat.abst1, zumat.abst2, ... zumat.abst5

**(Value)**
Specification of the discount per limit value. Depending on the surcharge type, the value is interpreted as percentage or amount.
If the quantity in the order item is greater than or equal to the specified limit value, the specified discount is deducted.
Technical info: numeric fields, DB fields: zumat.abwert1, zumat.abwert2, ... zumat.abwert5

### Thickness surcharge vectors

**Master data > Prices > Surcharges > Thickness surcharges vectors**

*Abb. C-169 Thickness surcharge vectors*

| fm Thick | Surcharge |
| :------- | :-------- |
| 12 mm    | 1.00      |
| 16 mm    | 1.50      |
| 20 mm    | 5.00      |
| 30 mm    | 8.00      |
| 50 mm    | 30.00     |

On this dialog, you create surcharges that are scaled by thickness. These surcharges are charged on the basic price of a processing, e.g. for drillings.

> **Thickness surcharge vectors**
> The surcharge is only added if the article is calculated according to the pricing method Processing matrices.
> This pricing method is replaced by the pricing method PCD-processings.

---

Per thickness surcharge vector, you can create 10 surcharge levels. The thickness surcharge is determined either as a percentage of the processing price or as a fixed amount on the quantity unit price or the piece price of the processing.

If the surcharge in the order should be calculated as a fixed amount, the currency of the price list code (PLCD) determined for the header article applies. The currency is not converted.

#### Field descriptions

**Site**
Selection of the site for which the prices are defined (only in multi-site system).

**Vector**
Selection or input of the vector number for the thickness surcharge.
Technical info: numeric field, DB field: bzuvek.veknr

**Vector name**
Display of the name. If you create a thickness vector, you select a brief description of the purpose as name, e.g. Drilling.
Technical info: alphanumeric field, DB field: bzuvek.vekbez

**Surcharge type**
Specification of to what the specified surcharge refers:
*   **CU/unit:**
    The surcharge is charged as fixed amount on the unit price of the item.
*   **CU/BQU:**
    The price is calculated per basic quantity unit.
*   **Percent:**
    The prices are calculated as a percentage of the basic price of the header article. This price type is only selected for exchange articles or processings.
Technical info: alphanumeric field, toggle field, DB field: bzuvek.zutyp

**frm Thick**
Specification of the glass thickness in millimeters, starting from which the surcharge applies.
Technical info: numeric fields, DB fields: bzuvek.ab1, bzuvek.ab2, ... bzuvek.ab10

**Surcharge**
Specification of the surcharge that is charged on the processing price. Depending on the surcharge type, the value is interpreted as percentage or fixed amount.
If the thickness of the article to be processed is greater than or equal to the specified limit value, the surcharge specified will be calculated.
Technical info: numeric fields, DB fields: bzuvek.zu1, bzuvek.zu2, ... bzuvek.zu10

---

### Size surcharges

**Master data > Prices > Surcharges > Size surcharges.**

On this dialog, you create surcharges that refer to the sizes in the order item. These include, e.g. lites in small sizes, overlengths, and oversizes. If the article entered exceeds or underruns the specified limit values, the surcharges are charged on the glass price.

⇨ Tutorial, “Size surcharges" on page C-629

> **Sequence of the surcharge levels**
> When checking the limit values for the surcharge levels, the dimensions are not sorted. This means that the limit values have to be specified in ascending order without gaps so that the correct surcharge is found.

Size surcharges can be assigned to IG base prices, article vectors, LAMI exchange/additional prices, special LAMI exchange/addition prices, special IG basic prices, and special article prices.

⇨ "IG base prices" on page C-704
⇨ "Article vectors" on page C-742
⇨ "LAMI exchange/additional p" on page C-772
⇨ "LAMI exchange/additional prices" on page C-963
⇨ "Special IG basic prices" on page C-942
⇨ "Article prices" on page C-899

#### Size Surcharges and pricing method

For the pricing methods PCD-LAMI, PCD-tempered, PCD-basic glass, PCD-processing, and PCD-prices general, IG-current by vector, you can create the following surcharges:

*   Small glass surcharges
*   Excess length surcharges
*   Oversize surcharges

For the pricing method IG-current by matrix and single lites, you can also create the following surcharges:

*   Side ratio surcharges
*   Surface surcharges

The following views are available for this dialog:

*   "Size surcharges - overview" on page C-813
*   "Size surcharges - other minor glass surcharges" on page C-817

---

### Size surcharges - overview

**Master data > Prices > Surcharges > Size surcharges**

*Abb. C-170 Size surcharges - overview*

On this dialog, you create surcharges for lites in small sizes, overlengths, and oversizes.

#### Field descriptions

**Site**
Selection of the site for which the prices are defined (only in multi-site system).

**Number, name**
Selection or specification of the surcharge number. When you create a size surcharge, select as name a brief description of the purpose, e.g. Small glass ornamental:
Technical info: numeric fields, DB fields: grosszu.grosszunr, grosszu.bez

#### Small glass surcharges

**to Qty ... sf**
Specification of the limit value in square feet. The surcharges are added up to the specified area.
If the area of the header article is less than or equal to the specified limit value, the surcharge is added. Here, round size and minimum calculation quantities are not considered.
You can use <F5> to define additional surcharge levels.
Technical info: numeric fields, DB fields: grosszu.menge1, grosszu.menge2, ... grosszu.menge5

---

**Surcharge**
Specification of the surcharge that is added up to the specified limit size.
Technical info: numeric fields, DB fields: grosszu.klzuschlag1, grosszu.klzuschlag2, ... grosszu.klzuschlag5

**Type**
Specification of to what the specified surcharge refers:

*   **CU/value:**
    The surcharge is charged as fixed value on the article price. If the surcharge is calculated as a fixed amount on the order, the currency of the PLCD determined for the header article applies. The currency is not converted.
*   **Percent:**
    The surcharge is charged as a percentage of the article price and added.

Technical info: numeric fields, toggle fields, DB fields: grosszu.klzutyp1, grosszu.klzutyp2, ... grosszu.klzutyp5

#### Excess length surcharges

**frm dims ... mm**
Specification of the limit value in millimeters. The surcharges are charged starting with the specified length for the longer glass edge.
If the longer edge of the header article is greater than or equal to the specified limit value, the surcharge is added. Here, round size and minimum calculation quantities are not considered.
Technical info: numeric fields, DB fields: grosszu.mass1, grosszu.mass2, grosszu.mass3

**Surcharge**
Specification of the surcharge that is added up to the specified limit size.
Technical info: numeric fields, DB fields: grosszu.uebzuschlag1, grosszu.uebzuschlag2, grosszu.uebzuschlag3

**Type**
Specification of to what the specified surcharge refers:

*   **CU/value:**
    The surcharge is charged as fixed value on the article price.
    If the surcharge on the order is charged as a fixed amount, the currency of the PLCD determined for the header article applies. The currency is not converted.
*   **Percent:**
    The surcharge is charged as a percentage of the article price and added.

Technical info: numeric fields, toggle fields, DB fields: grosszu.uebzutyp1, grosszu.uebzutyp2, gosszu.uebzutyp3

---

#### Oversize surcharges

**from dims ... mm x ... mm**
Specification of the limit value in millimeters. The surcharges are charged starting with the specified length. The surcharges are charged if both edges have reached or exceeded the specified lengths. Here, round size and minimum calculation quantities are not considered.
⇨ Tutorial, "Oversize surcharge" on page C-631
Technical info: numeric fields, DB fields: grosszu.uemass11, grosszu.uemass12, grosszu.uemass21, grosszu.uemass22, grosszu.uemass31,grosszu.uemass32

> **Sequence of the dimensions**
> The smaller edge of the lite is compared to the first value and the longer edge to the second value. If the dimension of the smaller lite is greater than or equal to the first value and the dimension of the longer edge is greater than or equal to the second value of the overlength, the next greater comparison is searched for. If this is not the case, there is no further search.
>
> Therefore, you need to pay attention that the dimensions are listed in the correct sequence.

**Surcharge**
Specification of the surcharge that is added up to the specified limit size.
Technical info: numeric fields, DB fields: grosszu.uebgrzuschlag1, grosszu.uebgrzuschlag2, grosszu.uebgrzuschlag3

**Type**
Specification of to what the specified surcharge refers:
*   **CU/value:**
    The surcharge is charged as fixed value on the article price.
    If the surcharge on the order is charged as a fixed amount, the currency of the PLCD determined for the header article applies. The currency is not converted.
*   **Percent:**
    The surcharge is calculated and charged as a percentage of the article price.
Technical info: numeric fields, toggle fields, DB fields: grosszu.uebgrzutyp1, grosszu.uebgrzutyp2, gosszu.uebgrzutyp3

#### Side ratio surcharges

**frm aspect ratio (1:x)**
Specification of the limit value for the aspect ratio. The limit values have to be specified in ascending order, e.g. 1:1.5, 1:2, 1:2.5.
The surcharges are charged starting with the specified aspect ratio.
If the aspect ratio of the two edge lengths of the header article is greater than or equal to the specified limit value, the surcharge is added. Here, round size and minimum calculation quantities are not considered.
Technical info: numeric fields, DB fields: grosszu.seivermass1, grosszu.seivermass2, ... grosszu.seivermass5

---

**Surcharge**
Specification of the surcharge that is added up to the specified limit size.
Technical info: numeric fields, DB fields: grosszu.seiverzuschlag 1, grosszu.seiverzuschlag2, ... grosszu.seiverzuschlag5

**Type**
Specification of to what the specified surcharge refers:
*   **CU/value:**
    The surcharge is charged as fixed value on the article price.
    If the surcharge on the order is charged as a fixed amount, the currency of the PLCD determined for the header article applies. The currency is not converted.
*   **Percent:**
    The surcharge is calculated and charged as a percentage of the article price.
Technical info: numeric fields, toggle fields, DB fields: grosszu.seiverzutyp1, grosszu.seiverzutyp2, grosszu.seiverzutyp5

#### Surface surcharges

**From... sf**
Specification of the limit value in square feet. The surcharges are charged starting with the specified area.
If the area of the header article is greater than or equal to the specified limit value, the surcharge is added. Here, round size and minimum calculation quantities are not considered.
Technical info: numeric fields, DB fields: grosszu.qmmass1, grosszu.qmmass2, ... grosszu.qmmass5

**Surcharge**
Specification of the surcharge that is added up to the specified limit size.
Technical info: numeric fields, DB fields: grosszu.qmzuschlag1, grosszu.qmzuschlag2, ... grosszu.qmzuschlag5

**Type**
Specification of to what the specified surcharge refers:
*   **CU/value:**
    The surcharge is charged as fixed value on the article price.
    If the surcharge on the order is charged as a fixed amount, the currency of the PLCD determined for the header article applies. The currency is not converted.
*   **Percent:**
    The surcharge is calculated and charged as a percentage of the article price.
Technical info: numeric fields, toggle fields, DB fields: grosszu.qmzutyp1, grosszu.qmzutyp2, ... gosszu.qmzutyp5

---

### Size surcharges - other minor glass surcharges

**Master data > Prices > Surcharges > Size surcharges > <F5>**

*Abb. C-171 Size surcharges - other minor glass surcharges*

On this dialog, you specify other minor glass surcharges. You can only open the dialog if you have filled out all fields for the minor glass surcharges on the Size Surcharges dialog.
⇨ "Size surcharges" on page C-812

#### Field descriptions

**To quantity**
Specification of the limit value in square feet. The surcharges are added up to the specified area.
If the area of the header article is less than or equal to the specified limit value, the surcharge is added. Here, round size and minimum calculation quantities are not considered.
Technical info: numeric field, DB field: grosszutab.menge

**Small glass surcharge**
Specification of the surcharge that is added up to the specified limit size.
Technical info: numeric field, DB field: grosszutab.menge

**Surcharge type**
Specification of to what the specified surcharge refers:
*   **CU/value:**
    The surcharge is charged as fixed value on the article price.
    If the surcharge on the order is charged as a fixed amount, the currency of the PLCD determined for the header article applies. The currency is not converted.
*   **Percent:**
    The surcharge is calculated and charged as a percentage of the article price.
Technical info: numeric field, DB field: grosszutab.klzutyp

---

### Processing group surcharges

**Master data > Prices > Surcharges > Processing surcharges**

*Abb. C-172 Processing group surcharges*

| Processing Group | Surch. | Type    |
| :--------------- | :----- | :------ |
| TG               | 3.00   | Percent |
| LM               | 5.00   | Percent |
| IG               | 6.00   | Percent |

On this dialog, you create surcharges for processing groups. These surcharges are added to the price of a processing or subpart if the processing group is assigned to the glass article in whose BOM the processing is included.

⇨ Master Data, "Prices" on page B-402

Processing group surcharges are only considered if the processing price is determined from the master data. They are not calculated if a special price is stored in the conditions.

The processing group surcharge is only calculated for processing articles with one of the following pricing methods:

*   7 - Processing matrices
*   25 - PC prices general
*   26 - PCD processings
*   31-PCD colored articles
*   60 - Protection

#### Field descriptions

**Processing group**
Specification of the processing group. The code consists of two alphanumeric characters. Upper and lower-case letters are distinguished, e.g. 5H and 5h.
⇨ Tutorial, "Processing group surcharges" on page C-632
Technical info: alphanumeric field, DB field: beagrpzu.bearbgrp

**Surcharge**
Specification of the surcharge. This surcharge is charged on the basic price of the processing. Depending on surcharge type, the value is interpreted as percentage or fixed amount.
If you specify a fixed amount, the value has to fit the currency of the price list code (PLCD) to which these surcharges are assigned.

---

In the order, the processing price is displayed in the item conditions including surcharge.
Technical info: numeric field, DB field: beagrpzu.zuschlag

**Price type**
Specification of to what the specified price refers:
*   **CU/value:**
    The surcharge is charged as fixed value on the processing price.
    If the surcharge on the order is charged as a fixed amount, the currency of the PLCD determined for the header article applies. The currency is not converted.
*   **Percent:**
    The surcharge is calculated and charged as a percentage of the processing price.
Technical info: alphanumeric field, toggle field, DB field: beagrpzu.preistyp

---

## Price Control

**Master data > Prices > Price control**

Calculation of prices includes, in addition to the codes and the price lists, also specifications of how particular prices are calculated. You create these definitions on the dialogs for price control. Some of these settings are for data exchange between the sites (plants, clients), and therefore only relevant for special customers.

This section provides information on the following subjects:

*   "Price control" on page C-821
*   "Rules SA-PU factor" on page C-823
*   "Bonus rules" on page C-824
*   "Price list control" on page C-825
*   "Price list restrictions" on page C-826

---

### Price control

**Master data > Prices > Price control > Price control**

*Abb. C-173 Price control*

On this dialog, you specify how the prices for the various plants are calculated.

#### Plant's prices

The fields in this area have to be configured specially. For customer-specific adjustments, contact your A+W Software GmbH contact person.

**Unprocessed goods + ... % on calculated purchase price**
Specification of the percentage that is charged on the PU price if unprocessed goods are sold to plants.

**Processed goods ... % on sales price**
Specification of the percentage that is deducted from the SA price for internal accounting.

**Tolerated deviation for supplier ... %**
Specification of the percentage by which the prices in the production site may deviate from the prices at the distributor.

#### Tmp price control

**frm ... identical shapes**
Number of identical TG lites starting with which a discount is granted on the shape surcharge. The TG shape surcharge is deducted directly. In the item conditions, the reduced shape surcharge is displayed. For identical shapes, only the item quantity is considered.

---

> **Example**
>
> You have specified that starting with 10 identical shapes, the TG shape surcharge should be reduced by 5%.
>
> In your order, an item with 10 identical shaped lites is entered. The reduced shape surcharge is calculated for these lites.
>
> If you enter these 10 shaped lites in an order in 2 items of 5 shaped lites apiece, the reduced shape surcharge is not considered; instead, the full shape surcharge is charged.

**...% less shape surcharge**
Specification of the percentage for a discount from the shape surcharge if the number of identical TG shapes has been reached.

#### Margin

**Message if less than ...%**
If the margin per order is less than the specified percentage, a message is displayed. The margin is displayed in the order footer.

**Message if more than ...%**
If the margin per order is greater than the specified percentage, a message is displayed.

**By mail ... days**
Number of days that are required for the exchange of information, e.g. the time between invoicing and invoice receipt by the customer. The specified time is considered for the calculation of discounts and payment deadlines.

**Last monthly closing**
Date of the last monthly closing. The date is drawn from the FinAc for the period delimitation.

> **Storing period end for SA invoices and credits**
> If in sales you want to specify a period end for invoices and credits, you have to specify a date in the Last Monthly Closing field in the price control. The current booking period ends with this date. In sales, only invoices and credits can be generated whose document date is before or on the specified date.

---

### Rules SA-PU factor

**Master data > Prices > Price control > Rules SA-PU factor**

*Abb. C-174 Rules SA-PU factor*

| Prod. Group | Description | PLCD | Sales | Purchase | Factors in % Supplier DI | Cust. CONS |
| :---------- | :---------- | :--- | :---- | :------- | :----------------------- | :--------- |
| 50A010      | IG heat protection 1 | 102 | 90.00 | 80.00 | 100 | 500000 |

On this dialog, you specify the PU factor for a particular product group, price list, a particular sales factor, and suppliers. The dialog is only used customer-specifically.

#### Field descriptions

**Prod. group, Description**
Selection of the product group for which the factors apply. You can also specify a superior or subordinate product group.
Technical info: alphanumeric field, DB field: ekvkzu.wagrp

**PLCD**
Selection of the price list code for which the factors apply.
Technical info: alphanumeric field, DB field: ekvkzu.pkz

**Sales**
Specification of the sales factor up to which the rule applies.
Technical info: alphanumeric field, DB field: ekvkzu.vkfaktor

**Purchase**
Specification of the purchasing factor that is used.
Technical info: alphanumeric field, DB field: ekvkzu.ekfaktor

**Supplier DI**
Specification of the supplier from the site that provides the goods.
Technical info: alphanumeric field, DB field: ekvkzu.linr

**Customer CONS**
Customer number of the CONSAFIS customer (only production). The customer is not currently evaluated.
Technical info: alphanumeric field, DB field: ekvkzu.kunr

---

### Bonus rules

**Master data > Prices > Price control > Bonus rules**

*Abb. C-175 Bonus rules*

| Site | Description | PLCD | Description | Prod. Group | Description | Factor | SC |
| :--- | :---------- | :--- | :---------- | :---------- | :---------- | :----- | :- |
| 21   | A+W Enterprise | 101 | IGU 5/2010 | 9025** | Plastics - processin | 101.00 | |

On this dialog, you specify the bonus rules for CONSAFIS transactions. The dialog is only used customer-specifically.

#### Field descriptions

**Site, Description**
Selection of the site for which the bonus rules apply.
Technical info: numeric field, DB field: conbon.hnr.

**PLCD, Description**
Selection of the price list code (PLCD) for which the bonus rules apply.
Technical info: numeric field, DB field: conbon.pkz.

**Prod. group, Description**
Selection of the product group for which the bonus rules apply.
Technical info: numeric field, DB field: conbon.wagr.

**Factor**
Specification of the factor up to which the bonus rules apply.
Technical info: numeric field, DB field: conbon.faktor.

**SC**
Specification of a pot code. You can assign up to ten bonus pots.
Technical info: numeric field, DB field: conbon.topf.

---

### Price list control

**Master data > Prices > Price control > Price list control**

*Abb. C-176 Price list control*

| PLCD | Description | Site | Basis PLCD | Description | Site | from logic |
| :--- | :---------- | :--- | :--------- | :---------- | :--- | :--------- |
| 104 | IGU 1/2015 | 29 | 102 | IGU 5/2012 | 29 | N |
| 103 | IGU 5/2013 | 29 | 102 | IGU 5/2012 | 29 | N |

On this dialog, you create a deviating procedure for a particular PLCD.

For the pricing, first the current PLCD is determined. After that, A+W Enterprise checks according to which deviating PLCD logic the search for the basic PLCD should be conducted.

⇨ Tutorial, "PLCD logics" on page C-550

#### Field descriptions

**PLCD, Description**
Selection of the price list code (PLCD) for which the deviating rules apply.
Technical info: numeric field, DB field: plkzsteuer.plkz.

**Site**
Display of the site for which the price list is created.

**Basis PLCD, Description**
Selection of the price list code (PLCD) on which the from-PLCD logic should fall back:
*   If you specify the same PLCD, there is only a search for the price in this PLCD. The from-PLCD logic is thus deactivated. An entry in the from logic field plays no role.
*   The specified basis PLCD is used as lower limit that the system uses as end for the search for the from-PLCD logic. For this, select Y in the from logic field.
*   The specified basis PLCD is used as second price list if the system finds no price in the first price list. For this, select N in the from logic field.
Technical info: numeric field, DB field: plkzsteuer.basisplkz

---

**Site**
Display of the site for which the price list is created (only in multi-site system).

**from logic**
Specification whether the from-PLCD logic should be used:
*   **Y:**
    The search for a price is continued in all numerically preceding PLCDs. If you specify a basis PLCD, the search ends with this PLCD.
*   **N:**
    The search is restricted to the PLCD and the basis PLCD.
Technical info: numeric field, DB field: plkzsteuer.ablogik.

### Price list restrictions

**Master data > Prices > Price control > Price list restrictions**

*Abb. C-177 Price list restrictions*

| Price Method | Description | Price list code | PLCD |
| :--- | :--- | :--- | :--- |
| 12 | PCD glass doors | 404 | SPEC-TSG 1/2015 |

On this dialog, you specify for individual pricing methods where the search for prices is canceled if you use the from-PLCD logic by default.

#### Field descriptions

**Price method, Description**
Selection of the pricing method for which the setting applies.
Technical info: numeric field, DB field: grenzplkz.vkptyp.

**Price list code**
Selection of the price list code (PLCD) for which a message is displayed during order entry.
Technical info: numeric field, DB field: grenzplkz.plkz.

---

## Conditions

**Master data > Conditions**

Use the Conditions menu to access all dialogs on which you specify market partner-specific or product group-specific conditions. For sales and purchasing, you can set up daily conditions separately.

Conditions form the basis for price calculation in A+W Enterprise. They are composed of surcharges, discounts or factors. A+W Enterprise distinguishes daily, customer, supplier, condition group, project, order, type, and item conditions, which are used with different priorities.

The conditions are structured in hierarchical fashion. For price calculation in the order, first the article price is determined and modified via the conditions. In the order, the condition with the highest priority is always used.

⇨ Tutorial, "Priorities of condition determination" on page C-637

The dialog descriptions for conditions are organized in the following topic areas.

⇨ "Daily Conditions" on page C-828
⇨ "Special Conditions" on page C-842
⇨ "Special Prices" on page C-898

> **Discounts**
> In addition to the conditions, you can define discounts that apply to particular product groups. You set up these discounts under **Master Data > Keys > Market Partners > Discounts**.

---

### Daily Conditions

With the Daily Conditions menu element, the conditions for purchasing and sales are created, which apply for all market partners and articles. The general daily conditions are always used if no other conditions for the price calculation are found. Furthermore, you can create product group-specific conditions that are evaluated before the general daily conditions.

The daily conditions are the basic conditions in A+W Enterprise. They are always evaluated first during price calculation; however, they can be overridden by entries in the Special Conditions or Special Prices and from the order.

⇨ Tutorial, "Priorities of condition determination" on page C-637

This section provides information on the following subjects:

⇨ "General daily conditions" on page C-829
⇨ "Product group conditions" on page C-836

---

### General daily conditions

**Master data > Conditions > Daily conditions > General daily conditions**

*Abb. C-178 Daily conditions*

On this dialog you specify the conditions that apply for the calculation of purchase prices and sales prices. These conditions are the basis for the price calculation.

If no conditions are stored on this dialog, no prices can be calculated.

For each pricing method, the price code (PCD) specifies from which price list the price should be read out. For this, you can specify a factor and a surcharge.

⇨ Tutorial, "Pricing methods" on page C-559

> **Working with cost calculation**
> If you are working with cost calculation in order entry, the material costs from the production cost price list are determined, which you can store in the purchasing conditions.

#### Field descriptions

**Condition type**
Selection whether the conditions apply for sales or purchasing:
*   **Sales:**
    The conditions apply for the calculation of sales prices.
*   **Purch.:**
    The conditions apply for the calculation of purchase prices.
    If you are working with the Cost Calculation module, the specifications apply for the determination of costs. For this, the price code (PCD) for the production costs is used.
Technical info: alphanumeric field, toggle field, DB field: kond.kondkz

---

The field descriptions for **PCD**, **SC**, **Factor**, and **Scal. Level** apply for all pricing methods. Deviations are specified in individual cases.

**PCD**
Price code. The PCD defines the price list from which the prices for the articles are drawn.
⇨ Tutorial, "Price List Code (PLCD)" on page C-540
⇨ Tutorial, "Price code (PCd)" on page C-541

**SC%**
Specification of a percentage surcharge. This surcharge is charged on the quantity unit price of the header article.
If you enter the value 0 or a value < 0, no surcharge is calculated.

**Factor %**
Specification of a percentage factor that is granted as discount if it is < 100.
With the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts.

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 <br> corresponds to a discount | 20.00 € | 16.00 € |
> | 150 <br> corresponds to a surcharge | 20.00 € | 30.00 € |

**Scal. level**
Specification of the price level from which the price is used. The field is only evaluated by the price calculation if for the relevant article price vector the price type 2 - Scaled Prices is specified.
The prices for the price levels are specified on the All Article Price Vectors or Special Article Price Vectors dialogs.
If 0 is entered in the relevant price level, an appropriate notice is displayed in the order entry.
⇨ "Article vectors" on page C-742
⇨ "Special article vectors" on page C-749

**Production costs**
Selection of the price code (PCD) for the cost calculation. The field is only displayed for the condition type **Purch**.
For the price calculation with the Cost Calculation module, the production costs are determined. The PCD refers to the price list from which the costs for articles with the procurement type Production or Stock are determined.
For articles with the procurement type PO, the PCD is used for the cost determination that is defined for the pricing method in question (IG, PCD-tempered, etc.).
For the cost calculation, you cannot specify a surcharge, factor or scale level.
Technical info: numeric field, DB field: kond.stafstuf

---

**IG**
Selection of the price code (PCD) with which the prices for IG articles are determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method IG-current or IG-Switzerland is assigned.
⇨ Tutorial, "PLCD logics" on page C-550
For IG articles, you cannot specify a scale level on this dialog.
Technical info: numeric fields, DB fields: kond.isopkz (PCD), kond.isotz (SU), kond.isofaktor (factor)

**PCD Temp**
Selection of the price code (PCD) with which the prices for tempered articles are determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method PCD-tempered is assigned.
Technical info: numeric fields, DB fields: kond.pkzesgpkz (PCD), kond.pkzesgtz (SU), kond.pkzesgfakt (factor), kond.pkzesgstaff (scal. level)

**PCD basic glass**
Selection of the price code (PCD) with which the prices for basic glass is determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method PCD-basic glass is assigned.
Technical info: numeric fields, DB fields: kond.pkzbaspkz (PCD), kond.pkzbastz (SU), kond.pkzbasfakt (factor), kond.pkzbasstaff (scal. level)

**PCD processing**
Selection of the price code (PCD) with which the prices for finished glass is determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method PCD-finished is assigned.
Technical info: numeric fields, DB fields: kond.pkzverpkz (PCD), kond.pkzvertz (SU), kond.pkzverfakt (factor), kond.pkzvertaff (scal. level)

**PCD gen. prices**
Selection of the price code (PCD) with which the prices are determined. The PCD refers to the price list from which the prices for articles are determined to which the pricing method PCD-prices general is assigned.
Technical info: numeric fields, DB fields: kond.pkzallpkz (PCD), kond.pkzalltz (SU), kond.pkzallfakt (factor), kond.pkzallstaff (scal. level)

**PCD LAMI**
Selection of the price code (PCD) with which the prices for LAMI articles are determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method PCD-LAMI is assigned.
Technical info: numeric fields, DB fields: kond.pkzvsgpkz (PCD), kond.pkzvsgtz (SU), kond.pkzvsgfakt (factor), kond.pkzvsgstaff (scal. level)

---

**PCD col. article**
Selection of the price code (PCD) with which the prices for articles with colored variants are determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method PCD-colored articles is assigned.
Technical info: numeric fields, DB fields: kond.pkzfarbpkz (PCD), kond.pkzfarbtz (SU), kond.pkzfarbfakt (factor), kond.pkzfarbstaff (scal. level)

**Muntins**
Selection of the price code (PCD) with which the prices for muntins are determined. The PCD refers to the price list from which the prices for BOM articles are determined to which the pricing method Muntins is assigned.
For muntins, no scale levels can be specified.
Technical info: numeric fields, DB fields: kond.sprospkz (PCD), kond.sprostz (SU), kond.sprosfaktor (factor)

#### Processing

If you enter the value 0 or a value < 0 for the surcharge, no surcharge is calculated.

**Processing in TG – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for corner processings on TG.
The surcharge and/or factor is calculated if the processing is attached on the BOM of a TG article with the pricing method PCD-tempered or PCD-glass doors.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Corner Processing selected.
*   The surcharge is added to the price of a corner processing. If you specify the value 0 or a value < 0, no surcharge is added.
*   The factor is calculated as discount for the corner processing in the BOM of a TG article. The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.esgbecktz (SU), kond.esgbeckf (factor)

**Processing in TG – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for edge processings on TG.
The surcharge and/or factor is calculated if the processing is attached on the BOM of a TG article with the pricing method PCD-tempered or PCD-glass doors.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Corner Processing selected.
*   The surcharge is added to the price of a edge processing.
*   The factor is calculated as discount for the edge processing in the BOM of a TG article. The factor is not evaluated if it is specified in the system settings that the same factor is used as for the glass article.
Technical info: numeric fields, DB fields: kond.esgbkantz (SU), kond.esgbkanf (factor)

---

**Surface in TG – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for surface processings on TG.
The surcharge and/or factor is calculated if the processing is attached on the BOM of a TG article with the pricing method PCD-tempered or PCD-glass doors.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Surface Processing selected.
*   The surcharge is added to the price of a surface processing.
*   The factor is calculated as discount for the surface processing in the BOM of a TG article. The factor is not evaluated if it is specified in the system settings that the same factor is used as for the glass article.
Technical info: numeric fields, DB fields: kond.esgbflatz (SU), kond.esgbflaf (factor)

**Processing on basic glass – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for corner processings.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Corner Processing selected.
*   The surcharge is added to the price of a corner processing.
*   The factor is calculated as discount for the corner processing on the BOM of an article to which the pricing method PCD-LAMI, PCD-basic glass, PCD-processing or IG-Switzerland general is assigned. The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.verbecktz (SU), kond.verbeckf (factor)

---

**Edges in basic glass – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for edge processings.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Corner Processing selected.
*   The surcharge is added to the price of a edge processing.
*   The factor is calculated as discount for the edge processing in the BOM of an article. The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.verbkantz (SU), kond.verbkanf (factor)

**Area in basic glass – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for surface processings.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Surface Processing selected.
*   The surcharge is added to the price of a surface processing.
*   The factor is calculated as discount for the surface processing in the BOM of an article. The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.verbflatz (SU), kond.verbflaf (factor)

**Accessory - SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for accessory articles.
The surcharge and/or factor is calculated if the accessory article is attached as subpart on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Accessory Selected selected.
*   The surcharge is added to the price of an accessory article.
*   The factor is calculated as discount for the accessory article in the BOM of an article. The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.zubetz (SU), kond.zubef (factor)

---

**Round price/pc.**
Specification of how the piece price should be rounded.
*   If you enter 1, the piece price is rounded to two places after the decimal point. The piece prices are displayed precisely in the order.
*   Any other entry in this field causes the amounts after the decimal point to be rounded up or down commercially to an amount divisible by this value.
⇨ Tutorial, "Unit price rounding" on page C-561
Technical info: numeric field, DB field: kond.stkprsrund

**Shape surch.**
Selection how a shape surcharge is calculated:
*   **Glass price:**
    The shape surcharge is added to the quantity unit price. This affects both the glass basic price of the header article as well as the exchange prices for IG or LAMI articles.
*   **Piece price:**
    A piece price is calculated from the quantity unit price. The shape surcharge is added to this piece price.
*   **Basic price:**
    The shape surcharge is added to the glass basic price of the header article.
Technical info: alphanumeric field, toggle field, DB field: kond.modzuvonstk

**Minimum processing price**
Selection whether the minimum processing prices for processings on TG and LAMI articles are evaluated in the price calculation. The setting only makes sense for the condition type Sales. This setting is not considered in the purchase price calculation.
Processing articles for which the minimum processing prices should be calculated have to be marked as minimum price-relevant in the article master data.
*   **N**
    The minimum processing prices for processings on TG and LAMI articles are not evaluated in the price calculation.
*   **Y**
    The minimum processing prices for processings on TG and LAMI articles are evaluated in the price calculation.
⇨ "Minimum processing prices" on page C-764
Technical info: alphanumeric field, toggle field, DB field: kond.minbeaprrel

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.

> **End of the validity**
> If the end date has been reached, you have to redefine the general daily conditions since otherwise basic information for the price calculation will be missing.

Technical info: date field, DB fields: kond.vondat, kond.adat

---

### Product group conditions

**Master data > Conditions -> Daily conditions > Product group conditions**

On this dialog, you specify the conditions that apply only for particular product groups. These conditions take precedence over the General daily conditions.

⇨ "General daily conditions" on page C-829

The following views are available for this dialog:

*   "Product group conditions - overview" on page C-836
*   "Product group conditions - details" on page C-838

#### Product group conditions - overview

**Master data > Conditions -> Daily conditions > Product group conditions**

*Abb. C-179 Daily product group conditions - overview*

> **Working with cost calculation**
> If you are working with cost calculation in order entry, the conditions for the purchasing are used to determine the costs.

On this overview, you maintain the product group conditions that are created either for the price calculation for purchasing or sales. The conditions for product groups apply only for the product group of the header article.

**<F2>**
Change to the detailed view.
⇨ "Product group conditions - details" on page C-838

---

#### Field descriptions

**Condition type**
Selection whether the conditions apply for sales or purchasing:
*   **Sales:**
    The conditions apply for the calculation of sales prices.
*   **Purch.:**
    The conditions apply for the calculation of purchase prices. If you are working with the Cost Calculation module, you cannot specify values for the material cost calculation that deviate from the general daily conditions.
Technical info: alphanumeric field, toggle field, DB field: wgkond.kondkz

**Prod. group**
Selection of the product group for which the conditions apply.
Technical info: alphanumeric field, DB field: wgkond.wagrp

**PCD**
Selection of the price code (PCD) from which the purchase or sales prices for articles in this product group are determined.
Technical info: numeric field, DB field: wgkond.pkz

**SC%**
Specification of a percentage surcharge for the entire product group. The surcharge is charged on the quantity unit price of the header article.
If you specify a value < 0, no surcharge is added.
Technical info: numeric field, DB field: wgkond.tz

**Factor %**
Specification of a percentage factor that is functions as discount if it is < 100%.
Technical info: numeric field, DB field: wgkond.faktor

**Offs.**
Specification of the price level from which the price is used. The field is only evaluated by the price calculation if for the relevant article price vector the price type 2 - Scaled Prices is specified.
The prices for the price levels are specified on the All Article Price Vectors or Special Article Price Vectors dialogs.
If 0 is entered in the relevant price level, an appropriate notice is displayed in the order entry.
⇨ "Article vectors" on page C-742
⇨ "Special article vectors" on page C-749
Technical info: numeric field, DB field: wgkond.staff

**Min. calcul.**
Number of quantity units in pieces, square meters, etc. for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is charged.
⇨ Tutorial, “Price-relevant quantity" on page C-562
Technical info: numeric field, DB field: wgkond.minber

**Round size**
Specification of the round size in mm for the price calculation of the articles in this product group, e.g. 30 mm.
For the price calculation, the edge lengths in the order item are rounded up to the next higher length that is divisible by the specified round size in mm.
Technical info: numeric field, DB field: wgkond.massrund

---

> **Example**
>
> 30 mm is defined as round size.
> The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 mm is 1020 mm.
> The price is calculated from the dimensions 1020 x 1020 mm = 1.04 square meters.

#### Product group conditions - details

**Master data > Conditions -> Daily conditions > Product group conditions > <F2>**

*Abb. C-180 Daily product group conditions - details*

On this dialog, you create the conditions for the daily product group conditions. In addition, you can specify surcharges and piece price rounding.

**<F2>**
Change to overview.
⇨ "Product group conditions - overview" on page C-836

##### Field descriptions

The fields in the header area are described for the Daily Product Group Conditions - Overview dialog:
⇨ "Product group conditions - overview" on page C-836

In addition, the following fields are displayed:

**Surcharge matrix**
Selection of a surcharge matrix for a general surcharge on the glass price of the product group.
⇨ "Surcharge matrices" on page C-807
Technical info: numeric field, DB field: wgkond.zumatnr

---

**Size Surcharges**
Selection of a size surcharge, e.g. small glass surcharge, overlength surcharge, etc. If the article of the product group exceeds or underruns the limit value specified in the surcharge, the price is increased by the surcharge.
⇨ "Size surcharges" on page C-812
Technical info: numeric field, DB field: wgkond.grosszu

**Muntin PCD**
Selection of the muntin price code (M-PCD) from which the prices for muntins are read.
⇨ "Muntin price code" on page C-695
Technical info: numeric field, DB field: wgkond.sprpkz

**Accessory SC %, Accessory factor %**
Specification of a percentage surcharge and/or the factor for accessory articles. The surcharge and/or factor applies for all articles of the product group.
The surcharge and/or factor is calculated if the accessory article is attached as subpart on the BOM of an article that is not assigned the pricing method PCD-prices general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Accessory Selected selected.
Technical info: numeric field, DB field: wgkond.zubetz, wgkond.zubef

**Round price/pc.**
Specification of whether the piece price should be rounded.
*   If you enter 1, the piece price is rounded to two places after the decimal point. The piece prices are displayed precisely in the order.
*   Any other entry in this field causes the amounts after the decimal point to be rounded up or down commercially to an amount divisible by this value.
⇨ Tutorial, "Unit price rounding" on page C-561
Technical info: numeric field, DB field: wgkond.stkprsrund

**AIR surch. vector**
Selection of a surcharge for the spacer in the airspace (AIR). This surcharge applies for all IG articles of the product group.
The specification is ignored if in the order conditions or in the general conditions for the market partner in question it is specified that no AIR surcharge should be calculated.
⇨ "AIR surcharges" on page C-736
Technical info: numeric field, DB field: wgkond.szrzutab

**Offset surcharge vector**
Selection of the surcharge for the offsets for IG lites or LAMI lites.
⇨ Tutorial, "Step surcharges" on page C-633

**SC ...%, Factor ...% – Corners**
Specification of a percentage surcharge and/or the factor for corner processings on articles of the product group.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.

---

On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Corner Processing selected.
*   The surcharge is added to the price of a corner processing.
*   If you specify a value < 0, no surcharge is added.
*   The factor is calculated as discount for the corner processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: wgkond.ecktz (SU), wgkond.eckf (factor)

**SC ...%, Factor ...% - Edges**
Specification of a percentage surcharge and/or the factor for edge processings on articles of the product group.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Edge Processing selected.
*   The surcharge is added to the price of a edge processing.
*   If you specify a value < 0, no surcharge is added.
*   The factor is calculated as discount for the edge processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: wgkond.kantz (SU), wgkond.kanf (factor)

**SC...%, Factor ...% – Surface**
Specification of a percentage surcharge and/or the factor for surface processings on articles of the product group.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Surface Processing selected.
*   The surcharge is added to the price of a surface processing.
*   If you specify a value < 0, no surcharge is added.
*   The factor is calculated as discount for the surface processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: wgkond.flatz (SU), wgkond.flaf (factor)

---

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: numeric fields, DB fields: wgkond.vondat, wgkond.abdat

> **End of the validity**
> The general daily conditions are always used if no other conditions for the price calculation are found.
>
> ⇨ "General daily conditions" on page C-829

---

## Special Conditions

**Master data > Conditions > Special Conditions**

Via the Special Conditions menu element, the conditions are entered that apply for individual objects, market partners, industries or product groups.

This section provides information on the following subjects:

⇨ "Special general conditions" on page C-843
⇨ "Special product group conditions" on page C-852
⇨ "Special article conditions" on page C-861
⇨ "Discount scaling" on page C-869
⇨ "Product group factors" on page C-871
⇨ "Article factors" on page C-874
⇨ "Muntin factors" on page C-877
⇨ "Shape surcharges" on page C-880
⇨ "AIR surcharges" on page C-884
⇨ "Exchange list factors" on page C-888
⇨ "IG single lites article factors" on page C-892
⇨ "IG single lites conditions - product group factors" on page C-895

---

### Special general conditions

**Master data > Conditions > Special conditions > General conditions**

*Abb. C-181 General conditions*

On this dialog, you specify conditions for market partners, objects, and industries. For the conditions for objects, you can distinguish between PU and SA conditions.

These conditions take precedence over the General daily conditions and the Product Group Conditions.

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Objecs supply:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market

---

partner group. Market partners for whom common conditions should apply have to be assigned to an industry in the market partner master data.
Technical info: numeric field, toggle field, DB field: kond.kondkz

**Market partner**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a condition industry.
Technical info: numeric field, DB field: kond.kunr

The field descriptions for **PCD**, **SC**, **Factor**, and **Scal. Level** apply for all pricing methods. Deviations are specified in individual cases.

**PCD**
Price code. The PCD defines the price list from which the prices for the articles are drawn.
⇨ Tutorial, "Price List Code (PLCD)" on page C-540
⇨ Tutorial, "Price code (PCd)" on page C-541

**SC %**
Specification of a percentage surcharge. This surcharge is charged on the quantity unit price of the header article.
If you specify a value < 0, no surcharge is added.

**Factor %**
Specification of a percentage factor that is granted as discount if it is < 100.

**Shape surcharge factor**
Specification of the factor for calculating shape surcharges. With the shape surcharge factor, the shape surcharge that is assigned to the PCD can be increased or reduced. The shape surcharge applies both for the glass as well as for the processings.
*   The shape surcharge factor is only calculated if the shape surcharge can be determined from the Prices > Shape Surcharges dialog.
    ⇨ "Shape surcharges" on page C-801
*   Shape surcharges from the Conditions > Shape Surcharges dialog are untouched by this factor.
    ⇨ "Shape surcharges" on page C-880

**Scal. level**
Specification of the price level from which the price is used. The field is only evaluated by the price calculation if for the relevant article price vector the price type 2 - Scaled Prices is specified.
The prices for the price levels are specified on the All Article Price Vectors or Special Article Price Vectors dialogs.
If 0 is entered in the relevant price level, an appropriate notice is displayed in the order entry.
⇨ "Article vectors" on page C-742
⇨ "Special article vectors" on page C-749

---

**Production costs**
Selection of the price code (PCD) for the cost calculation. The field is only displayed if internal site separation is active and Supplier is selected as condition type.
For the price calculation with the Cost Calculation module, the production costs are determined. The PCD refers to the price list from which the costs for articles with the procurement type Production or Stock are determined.
For articles with the procurement type PO, the PCD is used for the cost determination that is defined for the pricing method in question (IG, PCD-tempered, etc.).
For the cost calculation, you cannot specify a surcharge, factor or scale level.
Technical info: numeric field, DB field: kond.stafstuf

**IG**
Selection of the price code (PCD) with which the prices for IG articles are determined. The PCD refers to the price list from which the prices for header articles with the procurement type Production or Stock is determined, to which the pricing method IG-current or IG-Switzerland is assigned.
⇨ Tutorial, "PLCD logics" on page C-550
For IG articles, you cannot specify a scale level on this dialog.
Technical info: numeric fields, DB fields: kond.isopkz (PCD), kond.isotz (SU), kond.isofaktor (factor), kond.isomodzufak (shape surcharge)

**PCD Tmp**
Selection of the price code (PCD) with which the prices for tempered articles are determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method PCD-tempered is assigned.
Technical info: numeric fields, DB fields: kond.pkzesgpkz (PCD), kond.pkzesgtz (SU), kond.pkzesgfakt (factor), kond.esgmodzufak (shape surcharge), kond.pkzesgstaff (scal. level)

**PCD basic glass**
Selection of the price code (PCD) with which the prices for basic glass is determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method PCD-basic glass is assigned.
Technical info: numeric fields, DB fields: kond.pkzbaspkz (PCD), kond.pkzbastz (SU), kond.pkzbasfakt (factor), kond.basmodzufak (shape surcharge), kond.pkzbasstaff (scal. level)

**PCD processing**
Selection of the price code (PCD) with which the prices for finished glass is determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method PCD-processed glass is assigned.
Technical info: numeric fields, DB fields: kond.pkzverpkz (PCD), kond.pkzvertz (SU), kond.pkzverfakt (factor), kond.vermodzufak (shape surcharge), kond.pkzvertaff (scal. level)

---

**PCD gen. prices**
Selection of the price code (PCD) with which the prices are determined. The PCD refers to the price list from which the prices for articles are determined to which the pricing method PCD-prices general is assigned.
Technical info: numeric fields, DB fields: kond.pkzallpkz (PCD), kond.pkzalltz (SU), kond.pkzallfakt (factor), kond.pkzallstaff (scal. level)

**PCD LAMI**
Selection of the price code (PCD) with which the prices for LAMI articles are determined. The PCD refers to the price list from which the prices for header articles are determined to which the pricing method PCD-LAMI is assigned.
Technical info: numeric fields, DB fields: kond.pkzvsgpkz (PCD), kond.pkzvsgtz (SU), kond.pkzvsgfakt (factor), kond.vsgmodzufak (shape surcharge), kond.pkzvsgstaff (scal. level)

**PCD color**
Selection of the price code (PCD) with which the prices for articles with colored variants are determined. The PCD refers to the price list from which the prices for articles with header articles are determined to which the pricing method PCD colored article is assigned.
Technical info: numeric fields, DB fields: kond.pkzfarbpkz (PCD), kond.pkzfarbtz (SU), kond.pkzfarbfakt (factor), kond.pkzfarbstaff (scal. level)

**Muntins**
Selection of the price code (PCD) with which the prices for muntins are determined. The PCD refers to the price list from which the prices for BOM articles are determined to which the pricing method Muntin prices is assigned.
For muntins, no scale levels can be specified.

**Muntins - type**
Selection of the calculation type according to which the muntin prices are calculated:
*   **1 - Fields:**
    The price is calculated according to the number of fields.
*   **2 - LM+C+T:**
    The price is calculated per linear meter, per crossing, and per trim.
*   **3 - LM:**
    The price is calculated per linear meter.
*   **4 - LM+C:**
    The price is calculated per linear meter and per crossing.
*   **5 - LM+T:**
    The price is calculated per linear meter and per trim.
*   **6 - C:**
    The price is calculated per crossing.
*   **7 - C+R:**
    The price is calculated per crossing and per trim.
*   **8 - T:**
    The price is calculated per trim.
*   **9 - Special:**
    This form of calculation is configured customer-specifically.
*   **10 - Percent:**
    The price is calculated as percentage.
*   **11 - sf price:**
    The price is calculated per sqare foot of glass.

---

*   **12 - Field+LM:**
    The price is calculated per field and per linear meter.
*   **13 - Piece:**
    A total price is calculated for the muntin pattern.
*   **14 - C or LM:**
    The price is calculated per crossing or per linear meter.
    *   If crossing points arise on the muntin pattern, the muntins are calculated according to the number of crossings.
    *   If there are no crossing points, the muntins are calculated by linear meters.
*   **15 - Field+C+T:**
    The price is calculated per field, per crossing, and per trim.
Technical info: numeric fields, DB fields: kond.sprospkz (PCD), kond.sprostz (SU), kond.sprosfaktor (factor), kond.sprosart (type)

#### Processing

If you enter the value 0 or a value < 0 for the surcharge, no surcharge is calculated.

**Processing in TG – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for corner processings on TG.
The surcharge and/or factor is calculated if the processing is attached on the BOM of a TG article with the pricing method PCD-tempered or PCD-glass doors.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Corner Processing selected.
*   The surcharge is added to the price of a corner processing.
*   If you specify a value < 0, no surcharge is added.
*   The factor is calculated as discount for the corner processing in the BOM of a TG article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.esgbecktz (SU), kond.esgbeckf (factor)

**Edges in TG – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for edge processings on TG.
The surcharge and/or factor is calculated if the processing is attached on the BOM of a TG article with the pricing method PCD-tempered or PCD-glass doors.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Edge Processing selected.
*   The surcharge is added to the price of a edge processing.
*   If you specify the value 0 or a value < 0, no surcharge is added.
*   The factor is calculated as discount for the edge processing in the BOM of a TG article.

---

The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.esgbkantz (SU), kond.esgbkanf (factor)

**Surface in TG – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for surface processings on TG.
The surcharge and/or factor is calculated if the processing is attached on the BOM of a TG article with the pricing method PCD-tempered or PCD-glass doors.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Surface Processing selected.
*   The surcharge is added to the price of a surface processing.
*   If you specify a value < 0, no surcharge is added.
*   The factor is calculated as discount for the surface processing in the BOM of a TG article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.esgbflatz (SU), kond.esgbflaf (factor)

**Corners on basic glass – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for corner processings.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Corner Processing selected.
*   The surcharge is added to the price of a corner processing.
*   The factor is calculated as discount for the corner processing on the BOM of an article to which the pricing method PCD-tempered or PCD-prices general is assigned.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.verbecktz (SU), kond.verbeckf (factor)

**Edges in basic glass – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for edge processings.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Edge Processing selected.
*   The surcharge is added to the price of a edge processing.
*   The factor is calculated as discount for the edge processing in the BOM of an article.

---

The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.verbkantz (SU), kond.verbkanf (factor)

**Area in basic glass – SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for surface processings.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Surface Processing selected.
*   The surcharge is added to the price of a surface processing.
*   The factor is calculated as discount for the surface processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.verbflatz (SU), kond.verbflaf (factor)

**Accessory - SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for accessory articles.
The surcharge and/or factor is calculated if the accessory article is attached as subpart on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Accessory Selected selected.
*   The surcharge is added to the price of an accessory article.
*   The factor is calculated as discount for the accessory article in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: kond.zubetz (SU), kond.zubef (factor)

**Round Price/Pc.**
Specification of whether the piece price should be rounded.
*   If you enter 1, the piece price is rounded to two places after the decimal point. The piece prices are displayed precisely in the order.
*   Any other entry in this field causes the amounts after the decimal point to be rounded up or down commercially to an amount divisible by this value.
⇨ Tutorial, "Unit price rounding" on page C-561
Technical info: numeric field, DB field: kond.stkprsrund

**Offset surcharge**
Specification of the offset surcharge. This surcharge is calculated if in the BOM of the IG article an offset with the article type Offset with offset difference dimensions is attached.
Technical info: numeric field, DB field: kond.stufzu

---

**Offset surcharge, (surcharge type)**
You can specify an offset surcharge. This surcharge is charged if in the BOM of the IG or LAMI lite there is an offset. For this, you specify the value for the surcharge and specify how the value is interpreted.
*   **CU/pc ne:**
    The offset surcharge is charged according to calculation of the factor as fixed net amount per offset.
*   **CU/pc gr:**
    The offset surcharge is charged as gross amount per offset before calculation of the factor.
*   **Percent:**
    The offset surcharge is charged as a percent of the glass quantity unit price and the exchange prices.
*   **%/piece:**
    The offset surcharge is charged per offset as a percent of the glass quantity unit price and the replacement prices.
Technical info: alphanumeric field, toggle field, DB field: kond.stufzutyp

**AIR surch.**
Specification of whether the AIR surcharge from the Basic prices dialog should be evaluated:
*   **Y:**
    The AIR surcharge is calculated.
*   **N:**
    The AIR surcharge is not calculated.
⇨ "IG basic prices – details" on page C-706
⇨ "AIR surcharges" on page C-736
Technical info: alphanumeric field, toggle field, DB field: kond.szrflag

**Shape surch.**
Selection how a shape surcharge is calculated:
*   **Glass price:**
    The shape surcharge is added to the quantity unit price. This affects both the glass basic price of the header article as well as the exchange prices for IG or LAMI articles.
*   **Piece price:**
    A piece price is calculated from the quantity unit price. The shape surcharge is added to this piece price.
*   **Basic price:**
    The shape surcharge is added to the glass basic price of the header article.
Technical info: alphanumeric field, toggle field, DB field: kond.modzuvonstk

**Minimum processing price**
Selection whether the minimum processing prices for processings on TG and LAMI articles are evaluated in the price calculation. The setting only makes sense for the condition type Sales. The setting only makes sense for the condition type Sales.
Processing articles for which the minimum processing prices should be calculated have to be marked as minimum price-relevant in the article master data.
*   **N:**
    The minimum processing prices for processings on TG and LAMI articles are not evaluated in the price calculation.

---

*   **Y:**
    The minimum processing prices for processings on TG and LAMI articles are evaluated in the price calculation.
⇨ "Minimum processing prices" on page C-764
Technical info: alphanumeric field, toggle field, DB field: kond.minbeaprrel

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB field: kond.vondat, kond.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific conditions have to be redefined if you want to keep working with these conditions.
>
> ⇨ "General daily conditions" on page C-829

---

### Special product group conditions

**Master data > Conditions > Special conditions > Product group conditions**

On this dialog, you specify conditions for a market partner, an object or an industry, which apply for particular product groups.

In the detail views, you create the conditions for the price calculation, e.g. discount levels, minimum calculation price, round size, surcharges.

The following views are available for this dialog:

*   "Special product group conditions - overview" on page C-852
*   "Product group conditions - discounts" on page C-855
*   "Product group conditions - details" on page C-856

#### Special product group conditions - overview

**Master data > Conditions > Special conditions > Product group conditions**

*Abb. C-182 Special product group conditions - overview*

On this overview, you maintain conditions that apply for particular market partners and particular product groups.

**<F2>**
Change to discount 1 to 5.
⇨ "Product group conditions - discounts" on page C-855

**<F2> <F2>**
Change to the detailed view.
⇨ "Product group conditions - details" on page C-856

---

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Objecs supply:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry in the market partner master data.
Technical info: numeric field, DB field: wgkond.kondkz

**Market partner**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: wgkond.kunr

**Product group**
Selection of the product group for which the conditions apply.
Technical info: alphanumeric field, DB field: wgkond.wagrp

**PCD**
Selection of the price code (PCD) with which the prices for articles of the product group are determined.
Technical info: numeric field, DB field: wgkond.pkz

**SC%**
Specification of a percentage surcharge. This surcharge is charged on the quantity unit price of the header article.
If you specify a value < 0, no surcharge is added.
Technical info: numeric field, DB field: wgkond.tz

**Factor %**
Specification of a percentage factor that is granted as discount if it is < 100%.
Technical info: numeric field, DB field: wgkond.faktor

**Exch.factor**
Specification of the factor by which the exchange price in the product group is increased or reduced. This applies if a lite in a header article with the pricing method IG-current or PCD-LAMI is exchanged in.

---

Technical info: numeric field, DB field: wgkond.austfaktor

**Offs.**
Specification of the price level from which the price is used. The field is only evaluated by the price calculation if for the relevant article price vector the price type 2 - Scaled Prices is specified.
The prices for the price levels are specified on the All Article Price Vectors or Special Article Price Vectors dialogs.
If 0 is entered in the relevant price level, an appropriate notice is displayed in the order entry.
⇨ "Article vectors" on page C-742
⇨ "Special article vectors" on page C-749
Technical info: numeric field, DB field: wgkond.staff

**Min.calcul.**
Number of quantity units in pieces, square meters, etc. for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is charged.
⇨ Tutorial, “Price-relevant quantity" on page C-562
Technical info: numeric field, DB field: wgkond.minber

---

#### Product group conditions - discounts

**Master data > Conditions > Special conditions > Product group conditions > <F2>**

*Abb. C-183 Product group conditions - discounts*

On this dialog, you specify discounts for particular market partners. The conditions apply for the articles in the specified product group.

**<F2>**
Change to the detailed view.
⇨ "Product group conditions - details" on page C-856

**<F2> <F2>**
Change to overview.
⇨ "Special product group conditions - overview" on page C-852

##### Field descriptions

The fields in the header area are described for the Product Group Conditions - Overview dialog:
⇨ "Special product group conditions - overview" on page C-852

In addition, the following fields are displayed:

**Discounts 1 - 5**
Specifiation of the percentage for discounts.
The Factor and Discount 1 to Discount 5 fields depend on one another. If you want to grant a market partner a price reduction, you have two possibilities with these product group conditions:
*   You can specify a factor. If this factor is < 100%, the price is reduced. The fields Discount 1 to Discount 5 are set to 0.
*   You can scale a discount and specify percentages in the fields Discount 1 to Discount 5. From these specifications, the factor is calculated automatically. The discounts 1 to 5 are calculated one after another in this process.

---

Technical info: numeric fields, DB fields: wgkond.rab1, wgkond.rab2, wgkond.rab3, wgkond.rab4, wgkond.rab5

> **Example**
>
> **Discount 1**
> 80%
> Factor = 20% The customer pays 20% of the price.
> Base price = 100 €
> End price = 20 €
>
> ---
>
> **Discount 1**
> 80%
> Factor = 8%
> Base price = 100 €
> **Discount 2**
> 60%
> End price = 8 €
>
> 100 € - 80% = 20 €, 20 € - 60 % = 8 €

#### Product group conditions - details

**Master data > Conditions > Special conditions > Product group conditions > <F2> > <F2>**

*Abb. C-184 Product group conditions - details*

On this dialog, you specify the details for the market partner-specific product group conditions. In addition, you can specify surcharges and piece price rounding.

**<F2>**
Change to overview.
⇨ "Special product group conditions - overview" on page C-852

**<F2> <F2>**
Change to discounts 1 to 5.
⇨ "Product group conditions - discounts" on page C-855

---

##### Field descriptions

The fields in the header area are described for the Product Group Conditions - Overview and Product Group Conditions - Discounts dialogs:
⇨ "Special product group conditions - overview" on page C-852
⇨ "Product group conditions - discounts" on page C-855

In addition, the following fields are displayed:

**Round Size ... mm**
Specification of the round size in mm for the price calculation of the articles in this product group, e.g. 30 mm.
For the price calculation, the edge lengths in the order item are rounded up to the next higher length that is divisible by the specified round size in mm.

> **Example**
> 30 mm is defined as round size.
> The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 mm is 1020 mm.
> The price is calculated from the dimensions 1020 x 1020 mm = 1.04 square meters.

Technical info: numeric field, DB field: wgkond.massrund

**Surcharge matrix**
Selection of a surcharge matrix for a general surcharge on the glass price of the product group.
⇨ "Surcharge matrices" on page C-807
Technical info: numeric field, DB fields: wgkond.zumatnr

**Size surcharges**
Selection of a size surcharge, e.g. small glass surcharge, overlength surcharge, etc. If the article of the product group exceeds or underruns the limit value specified in the surcharge, the price is increased by the surcharge.
⇨ "Size surcharges" on page C-812
Technical info: numeric field, DB field: wgkond.grosszu

**Muntin PCD**
Selection of the muntin price code (M-PCD) from which the prices for muntins are read.
⇨ "Muntin price code" on page C-695
Technical info: numeric field, DB field: wgkond.sprpkz

**Offset surch.**
Specification of the offset surcharge. This surcharge is calculated if in the BOM of the IG or LAMI article an offset with the article type Offset with offset difference dimensions is attached. The surcharge only applies for the specified market partner and the product group.
Technical info: numeric field, DB fields: wgkond.stufzu

> **Expanded offset surcharge types in the special conditions**
> If you assign a product group in the form <nnnnnn> to <n*****> to the environment variable KONDITIONEN_VSG_WAGRP = <VSG Warengruppe>, you can also use the expanded offset surcharge types in the special product group conditions and the special article conditions.

---

**(Offset surcharge type)**
Selection of to what the surcharge refers.
*   **CU/pc ne:**
    The offset surcharge is charged according to calculation of the factor as fixed net amount per offset.
*   **CU/pc gr:**
    The offset surcharge is charged as gross amount per offset before calculation of the factor.
*   **Percent:**
    The offset surcharge is charged as a percent of the glass quantity unit price and the exchange prices.
*   **%/piece:**
    The offset surcharge is charged per offset as a percent of the glass quantity unit price and the replacement prices.
If an appropriate product group is assigned to the environment variable KONDITIONEN_VSG_WAGRP, you can select between the extended offset surcharge types.
The expanded surcharge types are described in detail for the LAMI basic prices:
⇨ "Surcharge Type" on page C-769

**Round price/pc.**
Specification of whether the piece price should be rounded for the specified market partner and articles in this product group.
*   If you enter 1, the piece price is rounded to two places after the decimal point. The piece prices are displayed precisely in the order.
*   Any other entry in this field causes the amounts after the decimal point to be rounded up or down commercially to an amount divisible by this value.
⇨ Tutorial, "Unit price rounding" on page C-561
Technical info: numeric field, DB field: wgkond.stkprsrund

**AIR surcharge vector**
Selection of a surcharge for the spacer in the airspace (AIR). This surcharge applies for all IG articles of the product group.
The specification is ignored if in the order conditions or in the general conditions for the market partner in question it is specified that no AIR surcharge should be calculated.
⇨ "AIR surcharges" on page C-736
Technical info: numeric field, DB field: wgkond.szrzutab

**Offset surcharge vector**
Selection of the surcharge for the offsets for IG lites or LAMI lites.
⇨ Tutorial, "Step surcharges" on page C-633
Technical info: numeric field, DB fields: wgkond.stufzunr

---

##### Accessory

**SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for accessory articles.
The surcharge and/or factor is calculated if the accessory article is attached as subpart on the BOM of an article that is assigned the pricing method PCD-LAMI, PCD-basic glass, PCD-processing, IG-current or IG-Switzerland general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Accessory selected.
*   The surcharge is added to the price of an accessory article.
*   If you specify a value < 0, no surcharge is added.
*   The factor is calculated as discount for the accessory article in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: wgkond.zubetz (SU), wgkond.zubef (factor)

##### Processings

If you enter a value < 0 for the surcharge, no surcharge is calculated.

**SC...%, Factor ...% – Corners**
Specification of a percentage surcharge and/or the factor for corner processings on articles of the product group.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is not assigned the pricing method PCD-tempered or PCD-prices general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Corner Processing selected.
*   The surcharge is added to the price of a corner processing.
*   The factor is calculated as discount for the corner processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: wgkond.ecktz (SU), wgkond.eckf (factor)

---

**SC...%, Factor ...% – Edges**
Specification of a percentage surcharge and/or the factor for edge processings on articles of the product group.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is not assigned the pricing method PCD-tempered or PCD-prices general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Edge Processing selected.
*   The surcharge is added to the price of a edge processing.
*   The factor is calculated as discount for the edge processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: wgkond.kantz (SU), wgkond.kanf (factor)

**SC...%, Factor ...% – Surface**
Specification of a percentage surcharge and/or the factor for surface processings on articles of the product group.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is not assigned the pricing method PCD-tempered or PCD-prices general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Surface Processing selected.
*   The surcharge is added to the price of a surface processing.
*   The factor is calculated as discount for the surface processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: wgkond.flatz (SU), wgkond.flaf (factor)

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: numeric fields, DB fields: wgkond.vondat, wgkond.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific conditions have to be redefined if you want to keep working with these special conditions.
>
> ⇨ "General daily conditions" on page C-829

---

### Special article conditions

**Master data > Conditions > Special conditions > Article conditions**

On this dialog, you specify conditions for particular articles that apply for a market partner, an object or an industry.

In the detail view, you create the conditions for the price calculation, e.g. discount levels, minimum calculation price, round size, surcharges.

The following views are available for this dialog:

*   "Article conditions - overview" on page C-861
*   "Article conditions - discounts" on page C-864
*   "Article conditions - details" on page C-865

#### Article conditions - overview

**Master data > Conditions > Special conditions > Article conditions**

*Abb. C-185 Article conditions - overview*

On this overview, you maintain conditions that apply for particular market partners and particular articles.

**<F2>**
Change to discounts 1 to 5.
⇨ "Article conditions - discounts" on page C-864

**<F2> <F2>**
Change to the detailed view.
⇨ "Article conditions - details" on page C-865

---

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
Technical info: numeric field, toggle field, DB field: artkond.kondkz

**Market partner**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: artkond.kunr

**Article**
Selection of the article for which the market partner-specific conditions apply.
Technical info: numeric field, DB field: artkond.artnr

**PCD**
Selection of the price code (PCD) from which the prices for the articles are determined.
The price list is used for header articles and for the BOM subparts to be calculated.
Technical info: numeric field, DB field: artkond.pkz

**SC%**
Specification of a percentage surcharge. This surcharge is applied to the price of an article if the article is used as header part.
If you specify a value < 0, no surcharge is added.
Technical info: numeric field, DB field: artkond.tz

**Factor %**
Specification of a percentage factor that is granted as discount if it is < 100%.
Technical info: numeric field, DB field: artkond.faktor

---

**Offs.**
Specification of the price level from which the price is used. The field is only evaluated by the price calculation if for the relevant article price vector the price type 2 - Scaled Prices is specified.
The prices for the price levels are specified on the All Article Price Vectors or Special Article Price Vectors dialogs.
If 0 is entered in the relevant price level, an appropriate notice is displayed in the order entry.
⇨ "Article vectors" on page C-742
⇨ "Special article vectors" on page C-749
Technical info: numeric field, DB field: artkond.staff

**Min.calcul.**
Number of quantity units in pieces, square meters, etc. for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is charged.
⇨ Tutorial, “Price-relevant quantity" on page C-562
Technical info: numeric field, DB field: artkond.minber

**Round Size ... mm**
Specification of the round size in mm for the price calculation of the article, e.g. 30 mm. The specification only makes sense for lites.
For the price calculation, the edge lengths in the order item are rounded up to the next higher length that is divisible by the specified round size in mm.

> **Example**
> 30 mm is defined as round size.
> The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 mm is 1020 mm.
> The price is calculated from the dimensions 1020 x 1020 mm = 1.04 square meters.

Technical info: numeric field, DB field: artkond.massrund

---

#### Article conditions - discounts

**Master data > Conditions > Special conditions > Article conditions > <F2>**

*Abb. C-186 Article conditions - discounts*

On this dialog, you specify discounts for particular market partners. The conditions apply for the articles in the specified article.

**<F2>**
Change to the detailed view.
⇨ "Article conditions - details" on page C-865

**<F2> <F2>**
Change to overview.
⇨ "Article conditions - overview" on page C-861

##### Field descriptions

The fields in the header area are described for the Article Conditions - Overview dialog:
⇨ "Article conditions - overview" on page C-861

In addition, the following fields are displayed:

**Discounts % 1, 2, 3, 4, 5**
Specifiation of the percentage for discounts.
The Factor and Discount 1 to Discount 5 fields depend on one another. If you want to grant a market partner a price reduction, you have two possibilities in these conditions:
*   You can specify a factor. If this factor is < 100%, the price is reduced. The fields Discount 1 to Discount 5 are set to 0.
*   You can scale a discount and specify percentages in the fields Discount 1 to Discount 5. From these specifications, the factor is calculated automatically. The discounts 1 to 5 are calculated one after another in this process.
Technical info: numeric fields, DB fields: artkond.rab1, artkond.rab2, artkond.rab3, artkond.rab4, artkond.rab5

---

> **Example**
>
> **Discount 1**
> 80%
> Factor = 20% The customer pays 20% of the price.
> Base price = 100 €
> End price = 20 €
>
> ---
>
> **Discount 1**
> 80%
> Factor = 8%
> Base price = 100 €
> **Discount 2**
> 60%
> End price = 8 €
>
> 100 € - 80% = 20 €, 20 € - 60 % = 8 €

#### Article conditions - details

**Master data > Conditions > Special conditions > Article conditions > <F2> > <F2>**

*Abb. C-187 Article conditions - details*

On this dialog, you specify the details for the market partner-specific article conditions. In addition, you can specify surcharges and piece price rounding.

**<F2>**
Change to overview.
⇨ "Article conditions - overview" on page C-861

**<F2> <F2>**
Change to discounts 1 to 5.
⇨ "Article conditions - discounts" on page C-864

---

##### Field descriptions

The fields in the header area are described for the Article Conditions - Overview and Article Conditions - Details dialogs:
⇨ "Article conditions - overview" on page C-861
⇨ "Article conditions - details" on page C-865

In addition, the following fields are displayed:

**Muntin PCD**
Selection of the muntin price code (M-PCD) from which the prices for muntins are read.
⇨ "Muntin price code" on page C-695
Technical info: numeric field, DB field: artkond.sprpkz

**Offset surch.**
Specification of the offset surcharge. This surcharge is calculated if in the BOM of the IG article an offset with the article type Offset with offset difference dimensions is attached. The surcharge only applies for the specified market partner and the article.
Technical info: numeric field, DB field: artkond.stufzu

> **Offset surcharge types in the special conditions**
> If you assign a product group in the form <nnnnnn> to <n*****> to the environment variable KONDITIONEN_VSG_WAGRP = <VSG Warengruppe>, you can also use the expanded offset surcharge types in the special product group conditions and the special article conditions.

**Offset surcharge type**
Selection of to what the surcharge refers.
*   **CU/pc ne:**
    The offset surcharge is charged according to calculation of the factor as fixed net amount per offset.
*   **CU/pc gr:**
    The offset surcharge is charged as gross amount per offset before calculation of the factor.
*   **Percent:**
    The offset surcharge is charged as a percent of the glass quantity unit price and the exchange prices.
*   **%/piece:**
    The offset surcharge is charged per offset as a percent of the glass quantity unit price and the replacement prices.
If an appropriate product group is assigned to the environment variable KONDITIONEN_VSG_WAGRP, you can select between the extended offset surcharge types.
The expanded surcharge types are described in detail for the LAMI basic prices:
⇨ "Surcharge Type" on page C-769
Technical info: numeric field, toggle field, DB field: artkond.stufzutyp

---

**Round price/pc.**
Specification of whether the piece price should be rounded for the specified market partner and article.
*   If you enter 1, the piece price is rounded to two places after the decimal point. The piece prices are displayed precisely in the order.
*   Any other entry in this field causes the amounts after the decimal point to be rounded up or down commercially to an amount divisible by this value.
⇨ Tutorial, "Unit price rounding" on page C-561
Technical info: numeric field, DB field: artkond.stkprsrund

##### Accessory

**SC ...%, Factor ...%**
Specification of a percentage surcharge and/or the factor for accessory articles.
The surcharge and/or factor is calculated if the accessory article is attached as subpart on the BOM of the article.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Accessory selected.
*   The surcharge is added to the price of an accessory article.
*   If you specify a value < 0, no surcharge is added.
*   The factor is calculated as discount for the accessory article in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: artkond.zubetz (SU), artkond.zubef (factor)

##### Processing

If you enter a value < 0 for the surcharge, no surcharge is calculated.

**SC...%, Factor ...% - Corners**
Specification of a percentage surcharge and/or the factor for corner processings on this article.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is not assigned the pricing method PCD-tempered or PCD-prices general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Corner Processing selected.
*   The surcharge is added to the price of a corner processing.
*   The factor is calculated as discount for the corner processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: artkond.ecktz (SU), artkond.eckf (factor)

---

**SC ...%, Factor ...% – Edges**
Specification of a percentage surcharge and/or the factor for edge processings on this article.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is not assigned the pricing method PCD-tempered or PCD-prices general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Edge Processing selected.
*   The surcharge is added to the price of a edge processing.
*   The factor is calculated as discount for the edge processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: artkond.kantz (SU), artkond.kanf (factor)

**SC...%, Factor ...% – Surface**
Specification of a percentage surcharge and/or the factor for surface processings on this article.
The surcharge and/or factor is calculated if the processing is attached on the BOM of an article that is not assigned the pricing method PCD-tempered or PCD-prices general.
On the Price Properties dialog, for the processing article or the article type, the price and/or discount calculation has to be activated and the calculation type Surface Processing selected.
*   The surcharge is added to the price of a surface processing.
*   The factor is calculated as discount for the surface processing in the BOM of an article.
*   The factor is not evaluated if it is specified in the system settings that the same factor is used for processings as for the glass article.
Technical info: numeric fields, DB fields: artkond.flatz (SU), artkond.flaf (factor)

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from .. to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB fields: artkond.vondat, artkond.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The market partner-specific conditions have to be redefined if you want to keep working with these special conditions.
>
> ⇨ "General daily conditions" on page C-829

---

### Discount scaling

**Master data > Conditions > Special conditions > Scales of discount**

*Abb. C-188 Discount scaling*

On this dialog, you create scaled discounts for a particular customer. These quantity discounts are only evaluated for header articles with the pricing method IG-Switzerland.

⇨ Tutorial, "Discount scaling" on page C-653

In the order, the scaled discounts can be viewed and changed.

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Customer**
Selection of the customer for whom the discounts apply.
Technical info: numeric field, DB field: rabatte.kunr

#### Qty scale discount 1, 2

The fields for the **Qty Scale Discount 1** apply for header articles, the fields for the **Qty Scale Discount 2** apply for the exchange lites.

**frm Qty**
Specification of the limit quantity for which the discount applies. This applies for articles with the IG-Switzerland pricing method.
Technical info: numeric fields, DB fields: rabatte.m1menge2, rabatte.m1menge3, rabatte.m1menge4, ..., rabatte.m1menge10, ..., rabatte.m2menge1, ..., rabatte.m10menge10

---

**Disc**
Specification of the discount in percent that applies for the limit quantity.
Technical info: numeric fields, DB fields: rabatte.m1rabatt1, rabatte.m1rabatt2, ..., rabatte.m1rabatt10, rabatte.m2rabatt1, rabatte.m2rabatt2,..., rabatte.m2rabatt10

#### Series disc.

**frm qty**
Specification of the limit quantity for which the series discount applies.
Technical info: numeric fields, DB fields: rabatte.smenge2, rabatte.smenge3, rabatte.smenge4, ..., rabatte.smenge10

**Disc**
Specification of the discount in percent that applies for the limit quantity.
Technical info: numeric fields, DB fields: rabatte.srabat1, rabatte.srabat2, rabatte.srabat3, ..., rabatte.srabat10

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB fields: rabatte.vondat, rabatte.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. You have to redefine the scaled discounts if you still want to work with these special conditions.
>
> ⇨ "General daily conditions" on page C-829

---

### Product group factors

**Master data > Conditions > Special conditions > Product group factors**

On this dialog, you specify product group-dependent and scaled factors for individual market partners or objects. You can specify the factors per item quantity. With a factor, a value can be increased or reduced.

You create the quantity levels and factors in the detail view.

The following views are available for this dialog:

*   "Product group factors - Overview" on page C-871
*   "Product group factors - details" on page C-873

#### Product group factors - Overview

**Master Data > Conditions > Special conditions > Product group factors**

*Abb. C-189 Product group factors - overview*

On this overview, you maintain product group-dependent and scaled factors for market partners or objects. You can scale the factors by quantity. If the factor is < 100%, then it is used as discount and reduces the price.

**<F2>**
Change to the detailed view.
⇨ "Product group factors - details" on page C-873

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

---

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
Technical info: numeric field, toggle field, DB field: kkuwgfa.kondkz

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: kkuwgfa.kunr

**Prod. group**
Selection of the product group for which the conditions apply.
Technical info: alphanumeric field, DB field: kkuwgfa.wagrp

**Type**
Specification of to what the quantity calculation applies. If you select a product group, **Per Item** is selected as type of the quantity calculation. The quantities for the scaling are determined precisely to the item. The field cannot be edited.
Technical info: display field, DB field: kkuwgfa.kondart

**Type**
Specification to what the limit values refer:
*   **Qty:**
    The limit values refer to the quantity.
*   **BQU:**
    The limit values refer to the basic quantity unit of the article, e.g. square meters, linear meters.
Technical info: alphanumeric field, toggle field, DB field: kkuwgfa.kondtyp

**frm Qty 1 ... 10**
Specification of the limit quantity starting with which the factor applies. The fields for the limit quantities 3 to 10 are in the detail view <F2>.
Technical info: numeric fields, DB fields: kkuwgfa.me1, kkuwgfa.me2, ..., kkuwgfa.me10

**Factor 1 ... 10%**
Specification of the factor that is considered with reaching of the limit quantity. If you specify a factor <100%, it is used as discount and reduces the price.

---

Technical info: numeric fields, DB fields: kkuwgfa.faktor1, kkuwgfa.faktor2, ..., kkuwgfa.faktor10

#### Product group factors - details

**Master data > Conditions > Special conditions > Product group factors > <F2>**

*Abb. C-190 Product group factors - details*

On this dialog, you specify the limit quantities and factors 3 - 10.

**<F2>**
Change to overview.
⇨ "Product group factors - Overview" on page C-871

##### Field descriptions

The fields are described for the Product Group Factors - Overview dialog:
⇨ "Product group factors - Overview" on page C-871

In addition, the following fields are displayed:

**Operator, input Date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB fields: kkuwgfa.vondat, kkuwgfa.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. After the end date, the general prices and conditions are used for the price calculation.

---

### Article factors

**Master data > Conditions > Special conditions > Article factors**

On this dialog, you specify product group-dependent and scaled factors for individual market partners or objects. You can specify the factors per item or per order. Furthermore, you can specify whether the factor is used if a particular quantity is reached. A value can be increased or reduced with a factor.

You create the quantity levels and factors in the detail view.

The following views are available for this dialog:

*   "Article factors - overview" on page C-874
*   "Article factors - details" on page C-876

#### Article factors - overview

**Master data > Conditions > Special conditions > Article factors**

*Abb. C-191 Article factors - overview*

On this overview, you maintain article-dependent and scaled factors for market partners or objects. You can scale the factors by quantity. If the factor is < 100%, it is used as discount and reduces the price.

**<F2>**
Change to the detailed view.
⇨ "Article factors - details" on page C-876

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

---

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
Technical info: numeric field, DB field: kkuartfa.kondkz

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: kkuartfa.kunr

**Article**
Selection of the article for whom the conditions apply.

**Type**
Specification of to what the quantity calculation applies. If you select a product group, Per Item is selected as type of the quantity calculation. The quantities for the scaling are determined precisely to the item. The field cannot be edited.
Technical info: alphanumeric field, toggle field, DB field: kkuwgfa.kondart

**Type**
Specification to what the limit values refer:
*   **Qty:**
    The limit values refer to the quantity.
*   **BQU:**
    The limit values refer to the basic quantity unit of the article, e.g. square meters, linear meters.
Technical info: alphanumeric field, toggle field, DB field: kkuartfa.kondtyp

**frm Qty 1 ... 10**
Specification of the limit quantity starting with which the factor applies. The fields for the limit quantities 3 to 10 are in the detail view <F2>.
Technical info: numeric fields, DB fields: kkuartfa.me1, kkuartfa.me2, ..., kkuartfa.me10

**Factor 1 ... 10%**
Specification of the factor that is considered with reaching of the limit quantity. If you specify a factor <100%, it is used as discount and reduces the price.
Technical info: numeric fields, DB fields: kkuartfa.faktor1, kkuartfa.faktor2, ..., kkuartfa.faktor10

---

#### Article factors - details

**Master data > Conditions > Special conditions > Article factors > <F2>**

*Abb. C-192 Article factors - details*

On this dialog, you specify the limit quantities and factors 3 - 10.

**<F2>**
Change to overview.
⇨ "Article factors - overview" on page C-874

##### Field descriptions

The fields are described for the Article Factors - Overview dialog:
⇨ "Article factors - overview" on page C-874

In addition, the following fields are displayed:

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB fields: kkuartfa.vondat, kkuartfa.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. After the end date, the general prices and conditions are used for the price calculation.

---

### Muntin factors

**Master data > Conditions > Special conditions > Muntin factors**

On this dialog, you create muntin factors for market partners or objects. The factors apply for the combinations of a muntin price class with a muntin price code. If the factor is < 100%, it is used as discount and reduces the price.

The following views are available for this dialog:

*   "Muntin factors - overview" on page C-877
*   "Muntin factors - details" on page C-879

#### Muntin factors - overview

**Master data > Conditions > Special conditions > Muntin factors**

*Abb. C-193 Muntin factors - overview*

On this overview, you maintain muntin factors for market partners or objects. If the factor < 100%, it is used as discount and reduces the price.

**<F2>**
Change to the detailed view.
⇨ "Muntin factors - details" on page C-879

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

---

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
Technical info: numeric field, toggle field, DB field: sprofakt.kondkz

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: sprofakt.kunr

**Muntin price class**
Selection of the muntin price class for which the factor applies.
Technical info: numeric field, DB field: sprofakt.spronr

**Muntin PCD**
Selection of the price code (PCD) for which the factor applies.
Technical info: numeric field, DB field: sprofakt.pkz

**Factor %**
Specification of the factor. If you specify a factor < 100%, it is used as discount and reduces the price.
Technical info: numeric field, DB field: sprofakt.faktor

---

#### Muntin factors - details

**Master data > Conditions > Special conditions > Muntin factors > <F2>**

*Abb. C-194 Muntin factors - details*

On this dialog, you specify the validity period for these conditions.

**<F2>**
Change to overview.
⇨ "Muntin factors - overview" on page C-877

##### Field descriptions

The fields are described for the Muntin Factors - Overview dialog:
⇨ "Muntin factors - overview" on page C-877

In addition, the following fields are displayed:

**Operator, Date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. You have to redefine the muntin factors if you want to keep working with these special conditions.

Technical info: date field, DB fields: sprofakt.vondat, sprofakt.abdat

---

### Shape surcharges

**Master data > Conditions > Special conditions > Shape surcharges**

On this dialog, you store shape surcharges for particular market partners or objects. You have to specify the surcharges for each individual shape. In the detail view, you specify the conditions for price calculation, e.g. a minimum surcharge.

The calculation of a surcharge can also be restricted to a product group, e.g. the surcharge for shape 5 and the product group LAMI.

The surcharge is always added if the shape in question is entered in the order for the market partner.

The following views are available for this dialog:

*   "Shape surcharges - overview" on page C-880
*   "Shape surcharges - details" on page C-883

#### Shape surcharges - overview

**Master data > Conditions > Special conditions > Shape surcharges**

*Abb. C-195 Shape surcharges - overview*

| Shape | Prod. Group | fr PLCD | Shape Type | Surch. | Minimum | Processing |
| :---- | :---------- | :------ | :--------- | :----- | :------ | :--------- |
| 5     | 45****      | 204     |            | 15.00  | 15.00   | 15.00      |
| 6     |             | 204     | IG-shape   | 12.00  | 10.00   |            |
| 7     |             | 204     | Trade-shape|        |         | 12         |

On this overview, you maintain shape surcharges for particular market partners or objects. Here you can distinguish between a surcharge for the shape and a surcharge for the processing on the shape.

The calculation of a surcharge can also be restricted to a product group, e.g. the surcharge for shape 5 and the product group LAMI.

You have to specify the surcharges for each individual shape.

In the price control, you can further define the calculation of the shape surcharges. For example, for the TG price control, you can specify that starting

---

with a particular number of shapes, the shape surcharged is reduced by a certain percentage.
⇨ "Price control" on page C-821

For articles to which a shape is assigned in the article master data, no model surcharge is calculated.

**<F2>**
Change to the detailed view.
⇨ "Shape surcharges - details" on page C-883

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. idustry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
Technical info: numeric field, toggle field, DB field: kumodzu.kondkz

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: kumodzu.kunr

**Shape**
Selection of the shape for which the market partner-specific shape surcharge is calculated.
Technical info: numeric field, DB field: kumodzu.modnr

**Prod. group**
Selection of the product group for which the shape surcharge applies. Leave the field empty if:
*   The shape surcharge is charged regardless of a product group.
*   The shape surcharge refers to a shape type.
Technical info: alphanumeric field, DB field: kumodzu.wagrp

---

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
⇨ Tutorial, "From-PLCD logic" on page C-552
Technical info: numeric field, DB field: kumodzu.plkz

**Shape type**
Selection of the shape type for which the shape surcharge applies. The field is locked if you have specified a product group. If you have not specified a product group, the shape surcharge is charged if the pricing method in question is assigned to the header article:
*   **IG-shape:**
    Pricing method IG-current or IG-Switzerland.
*   **TG shape:**
    Pricing method PCD-tempered.
*   **LAMI shape:**
    Pricing method PCD-laminated.
*   **Retail shape:**
    Pricing method PCD-basic glass or PCD-finished glass.
Technical info: alphanumeric field, toggle field, DB field: kumodzu.modtyp

**Surcharge**
Percentage that is calculated for the shape.
*   If you enter a value < 0 for the surcharge, no shape surcharge is calculated.
*   If you leave the field empty, only the surcharge for processings on the shape is created. The shape surcharge for the glass is then determined from the master data.
Technical info: numeric field, DB field: kumodzu.zuschlag

**Minimum**
Specification of a fixed amount as minimum surcharge for the shape.
If the calculated shape surcharge in the order is smaller than the defined minimum shape surcharge, this minimum surcharge is used.
Technical info: numeric field, DB field: kumodzu.minzuschlag

**Processing**
Entry of a processing surcharge for the shape. This surcharge is also charged for accessory articles.
The surcharge is charged as a percentage on the processing price if the processing or accessory article is attached to the BOM of the glass article.
*   If you enter a value < 0 for the processing surcharge, no processing surcharge is calculated.
*   If you leave the field empty, the processing surcharge from the Shape Surcharges dialog is used for price calculation.

> **Shape surch. on the glass**
> So that shape surcharges for processings are calculated, the **Price Calculation** and **Shape Surcharge** fields have to be marked on the Price Properties dialog for the articles.

---

If you create a new data record for a shape and exit the Surcharge field for the glass article with <Enter>, the Processing field is pre-populated by default with the shape surcharge for the glass article. The value can be changed appropriately.
Technical info: numeric field, DB field: kumodzu.beamodzusch

#### Shape surcharges - details

**Master data > Conditions > Special conditions > Shape surcharges > <F2>**

*Abb. C-196 Shape surcharges - details*

On this dialog, you specify the validity period for the shape surcharges.

**<F2>**
Change to overview.
⇨ "Shape surcharges - overview" on page C-880

##### Field descriptions

The fields are described for the Shape Surcharges - Overview dialog:
⇨ "Shape surcharges - overview" on page C-880

In addition, the following fields are displayed:

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB fields: kumodzu.vondat, kumodzu.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. You have to redefine the shape surcharges if you still want to work with these special conditions.

---

### AIR surcharges

**Master data > Conditions > Special conditions > AIR Surcharges**

On this dialog, you specify market partner-specific AIR surcharges. You can create surcharges for up to 12 different spacers (AIR). The AIR surcharges are charged if the AIR in the specified IG article underruns the specified mm scales.

The following views are available for this dialog:

*   "AIR surcharges - overview" on page C-884
*   "AIR surcharges - details" on page C-886

#### AIR surcharges - overview

**Master data > Conditions > Special conditions > AIR surcharges**

*Abb. C-197 AIR surcharges - overview*

On this overview, you maintain market partner-specific AIR surcharges. You can create surcharges for up to 12 different spacer sizes (AIR). The AIR surcharges are charged if the AIR in the specified IG article underruns the specified mm scales.

**<F2>**
Change to the detailed view.
⇨ "AIR surcharges - details" on page C-886

---

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
Technical info: numeric field, toggle field, DB fields: spezszrzu.kondkz

**(Market partner)**
Selection of the market partner for whom the conditions apply. Selection of the market partner for whom the conditions apply.
Technical info: numeric field, DB field: spezszrzu.kondnr

**Article**
Selection of the IG article for which the conditions apply.
Technical info: numeric field, DB field: spezszrzu.artnr

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
⇨ Tutorial, "From-PLCD logic" on page C-552
Technical info: numeric field, DB field: spezszrzu.plkz

**to AIR mm 1, 2... 12**
Specification of the limit value for the surcharge.
Technical info: numeric fields, DB fields: spezszrzu.szr1, spezszrzu.szr2, ..., spezszrzu.szr12

**Surcharge**
Specification of the surcharge for the specified limit value.
Technical info: numeric fields, DB fields: spezszrzu.zusch1, spezszrzu.zusch2, ... spezszrzu.zusch12

**Type**
Specification of to what the specified surcharge refers:

---

*   **CU/piece net:**
    The AIR surcharge is charged as fixed amount per intermediate space.
*   **CU/BQU:**
    Depending on the system configuration, the AIR surcharge is charged on the basic price or the glass price.
*   **Percent:**
    Depending on the system configuration, the AIR surcharge is charged as a percentage on the basic price or the glass price.
Technical info: alphanumeric fields, toggle field, DB fields: spezszrzu.zutyp1, ..., spezszrzu.zutyp12

#### AIR surcharges - details

**Master data > Conditions > Special conditions > AIR surcharges > <F2>**

*Abb. C-198 AIR surcharges - details*

On this dialog, you specify additional surcharge levels and the validity period for the AIR surcharges.

**<F2>**
Change to overview.
⇨ "AIR surcharges - overview" on page C-884

##### Field descriptions

The fields are described for the AIR Surcharges - Overview dialog:
⇨ "AIR surcharges - overview" on page C-884

In addition, the following fields are displayed:

**Operator, Input date**
Indication of the operator and entry or change date.

---

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB fields: spezszrzu.vondat, spezszrzu.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. You have to redefine the AIR surcharges if you still want to work with these special conditions.

---

### Exchange list factors

**Master data > Conditions > Special conditions > Exchange list factors**

On this dialog, you specify market partner-specific factors for exchange lists. These factors function as surcharges or discounts on the prices from the exchange/additional lists.

⇨ "Exchange/additionbut invoiced internallyal lists" on page C-692
⇨ "LAMI exchange/additional p" on page C-772

The following views are available for this dialog:

*   "Exchange list factors - overview" on page C-888
*   "Exchange list factors - details" on page C-890

#### Exchange list factors - overview

**Master data > Conditions > Special conditions > Exchange list factors**

*Abb. C-199 Special exchange list factors - overview*

On this overview, you maintain market partner-specific factors for exchange lists. These factors function as surcharges or discounts on the prices from the exchange/additional lists.

⇨ "Exchange/additionbut invoiced internallyal lists" on page C-692
⇨ "LAMI exchange/additional p" on page C-772

**<F2>**
Change to the detailed view.
⇨ "Exchange list factors - details" on page C-890

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

---

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
Technical info: numeric field, toggle field, DB field: spezatlfakt.kondkz

**Market partner**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: spezatlfakt.kondnr

**Exchange in**
Specification of the glass type for which the exchange list factor is calculated.
*   **IG:**
    The exchange list factor is calculated if a glass is exchanged into an IG header article.
*   **LAMI:**
    The exchange list factor is calculated if a glass is exchanged into a LAMI header article.
*   **IG+LAMI:**
    The exchange list factor is calculated if a glass is exchanged into an IG header article or a LAMI header article.
Technical info: numeric field, toggle field, DB field: spezatlfakt.austkz

**Prod. group, description**
Selection of the product group for which the exchange list factor applies.
By default, the product group refers to the product group of the exchange glass. A+W Enterprise can be configured this way with the environment variable SPEZATLFAKT_KOPFWAGRP so that the exchange lists for the product apply that arise due to the product group logic after the exchange for the header part.
Technical info: alphanumeric field, DB field: spezatlfakt.wagrp

**Exchange list, description**
Selection of the exchange/additional list for which the exchange list factor applies.
Technical info: alphanumeric field, DB field: spezatlfakt.atlnr

---

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
⇨ Tutorial, "From-PLCD logic" on page C-552
⇨ "Price lists (PLCD)" on page C-688
Technical info: numeric field, DB field: spezatlfakt.plkz

**Factor %**
Specification of the factor. If you specify a factor < 100%, it is used as discount and reduces the price.
Technical info: numeric field, DB field: spezatlfakt.faktor

#### Exchange list factors - details

**Master data > Conditions > Special conditions > Exchange list factors > <F2>**

*Abb. C-200 Special exchange list factors - details*

You specify the validity time period for an exchange list factor on this dialog.

**<F2>**
Change to overview.
⇨ "Exchange list factors - overview" on page C-888

##### Field descriptions

The fields in the header area are described for the Exchange List Factors - Overview dialog:
⇨ "Exchange list factors - overview" on page C-888

---

In addition, the following fields are displayed:

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from .. to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB field: spezatlfakt.vondat, spezatlfakt.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. You have to redefine the exchange list factors if you still want to work with these special conditions.

---

### IG single lites article factors

**Master data > Conditions > Special conditions > IG single lite conditions > Article factors**

On this menu, you specify market partner-specific factors for single lites, which can be installed as subpart in the BOM of an IG article.

These conditions only apply if you have assigned the article in question the type Single Lites in the IG basic prices.
⇨ "IG base prices" on page C-704

The market partner-specific IG article factors have a higher priority than the general article factors.
⇨ "Article factors" on page C-874

The following views are available for this dialog:

*   "Article factors - overview" on page C-892
*   "Article factors - details" on page C-894

#### Article factors - overview

**Master data > Conditions > Special conditions > IG single lite conditions > Article factors**

*Abb. C-201 IG single lites article factors - overview*

On this overview, you maintain market partner-specific article factors for all fixed dimension lites that can be installed in the BOM of an IG lite.

These conditions only apply if you have assigned the article in question the type Single Lites in the IG basic prices.
⇨ "IG base prices" on page C-704

**<F2>**
Change to the detailed view.
⇨ "Article factors - details" on page C-894

---

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom common conditions should apply have to be assigned to an industry.
Technical info: numeric field, toggle field, DB field: kezartfa.kondkz

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: kezartfa.kunr

**Article, Description**
Selection of the glass that is installed in the BOM of an IG lite.
Technical info: numeric field, alphanumeric field, toggle field, DB field: kezartfa.artnr

**Factor %**
Specification of the factor. If you specify a factor < 100%, it is used as discount and reduces the price.
Technical info: numeric field, DB field: kezartfa.faktor

---

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 <br> corresponds to a discount | 20.00 € | 16.00 € |
> | 150 <br> corresponds to a surcharge | 20.00 € | 30.00 € |

#### Article factors - details

**Master data > Conditions > Special conditions > IG single lite conditions > Article factors > <F2>**

*Abb. C-202 IG single lites article factors - details*

You specify the validity time period for the current condition on this dialog.

**<F2>**
Change to overview.
⇨ "Article factors - overview" on page C-892

##### Field descriptions

The fields are described for the IG Single Lites Article Factors - Overview dialog:
⇨ "Article factors - overview" on page C-892

In addition, the following fields are displayed:

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from ... to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB field: kezwgrpfa.vondat, kezartfa.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. You have to redefine the article factors for IG single lites if you still want to work with these special conditions.

---

### IG single lites conditions – product group factors

**Master data > Conditions > Special conditions > IG single lite conditions > Product group factors**

On this dialog, you specify market partner and product group-specific article factors for single lites.

These conditions only apply if you have assigned the article in question the type Single Lites in the IG basic prices.
⇨ "IG base prices" on page C-704

The following views are available for this dialog:

*   "Product group factors - overview" on page C-895
*   "Product group factors - details" on page C-897

#### Product group factors - overview

**Master data > Conditions > Special conditions > IG single lite conditions > Product group factors**

*Abb. C-203 Single lites product group factors - overview*

On this dialog, you maintain market partner and product group-specific article factors for single lites.

**<F2>**
Change to the detailed view.
⇨ "Product group factors - details" on page C-897

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

---

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom the common conditions should apply have to be assigned to an industry.
Technical info: numeric field, toggle field, DB field: kezwgrpfa.kondkz

**(Market partner)**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: kezwgrpfa.kunr

**Prod. group, description**
Selection of the product group of the exchanged glass for which the factor applies.
Technical info: alphanumeric field, DB field: kezwgrpfa.wgrp

**Factor %**
Specification of the factor. If you specify a factor < 100%, it is used as discount and reduces the price. The factor applies if the single lite belongs to the specified product group.
Technical info: numeric field, DB field: kezwgrpfa.faktor

---

> **Example**
>
> | Factor | Basic price | Final price |
> | :--- | :--- | :--- |
> | 100 | 20.00 € | 20.00 € |
> | 80 <br> corresponds to a discount | 20.00 € | 16.00 € |
> | 150 <br> corresponds to a surcharge | 20.00 € | 30.00 € |

#### Product group factors - details

**Master data > Conditions > Special conditions > IG single lite conditions > Product group factors > <F2>**

*Abb. C-204 Single lites product group factors - details*

You specify the validity time period for the conditions.

**<F2>**
Change to overview.
⇨ "Product group factors - overview" on page C-895

##### Field descriptions

The fields are described for the Product Group Factors - Overview dialog:
⇨ "Product group factors - overview" on page C-895

In addition, the following fields are displayed:

**Operator, Input date**
Indication of the operator and entry or change date.

**Cond. valid from to ...**
Specification of the date from which and to which the conditions are valid.
Technical info: date field, DB field: kezwgrpfa.vondat, kezwgrpfa.abdat

> **End of the validity**
> After the end date, the general prices and conditions are used for the price calculation. The product group factors for single lites have to be redefined if you want to continue working with these special conditions.

---

## Special Prices

**Master data > Conditions > Special prices**

With the Special Prices menu element, market partner-specific prices are created for various articles.

The special prices override the prices from the price lists. However, the conditions apply to the special prices nevertheless.

⇨ Tutorial, "Priorities of condition determination" on page C-637
⇨ "Conditions" on page C-827

This section provides information on the following subjects:

*   "Article prices" on page C-899
*   "Special variant prices" on page C-907
*   "Prices for colored articles" on page C-912
*   "Muntin prices" on page C-918
*   "Processing prices" on page C-923
*   "IG exchange prices" on page C-930
*   "Special prices for IG single lites" on page C-937
*   "Special IG basic prices" on page C-942
*   "UV coating prices" on page C-951
*   "Glazing prices" on page C-955
*   "Exchange prices pattern glass classes” on page C-959
*   "LAMI exchange/additional prices" on page C-963

---

### Article prices

**Master data > Conditions -> Special prices > Article prices**

On this dialog, you specify article prices for a market partner, an object or an industry.

In the detail views, you specify the conditions for the price calculation, e.g. price levels, minimum calculation quantity, round size, surcharges.

The market partner-specific article prices have a higher priority than the prices of the article vectors.

⇨ "Article vectors" on page C-693

The following views are available for this dialog:

*   "Article prices - overview" on page C-899
*   "Article prices - details" on page C-903

#### Article prices - overview

**Master data > Conditions -> Special prices > Article prices**

*Abb. C-205 Article prices - overview*

| Article | fr PLCD | Price Type | Description | Factor | Price 1 | Type |
| :------ | :------ | :--------- | :---------- | :----- | :------ | :--- |
| 150004  | 501     | 1          | Indiv.price | 100.00 | 69.18   | CU/QU|
| 500444  | 204     | 1          | Indiv.price | 100.00 | 226.63  | CU/QU|

On this overview, you maintain the article prices for a market partner, an object or an industry.

The market partner-specific article prices have a higher priority than the prices of the article vectors.

⇨ "Article vectors" on page C-693

---

**<F2>**
Change to the detailed view.
⇨ "Article prices - details" on page C-903

**<F2> <F2>**
Change to the detailed view with the levels 9 - 20.

#### Field descriptions

> **Customers and suppliers in the conditions**
> Customers and suppliers for whom a condition applies always refer to the condition debtor from the market partner master data below.

**Condition type**
Selection for whom the conditions apply:
*   **Customer:**
    The conditions apply for the calculation of sales prices for a particular customer.
*   **Supplier:**
    The conditions apply for the calculation of purchase prices for a particular supplier.
*   **Object sale:**
    The conditions apply for the calculation of sales prices for a particular sales object.
*   **Object purch.:**
    The conditions apply for the calculation of purchase prices for a particular purchasing object.
*   **Cond. industry:**
    The conditions apply for the calculation of prices for a particular market partner group. Market partners for whom the common conditions should apply have to be assigned to an industry.
Technical info: numeric field, toggle field, DB field: kuartprs.kondkz

**Market partner**
Selection of the market partner for whom the conditions apply. Depending on the condition type, you can specify a customer, a supplier, an object or a customer group.
Technical info: numeric field, DB field: kuartprs.kunr

**Article**
Selection of the article for which the market partner-specific article price should apply.
Technical info: numeric field, DB field: kuartprs.artnr

**fr PLCD**
Selection of the price list code (PLCD) starting from which the prices apply.
If A+W Enterprise does not find any prices in the order for the article for the current PLCD, the preceding numeric PLCD is determined for which the price data is defined.
⇨ Tutorial, "From-PLCD logic" on page C-552
Technical info: numeric field, DB field: kuartprs.plkz
