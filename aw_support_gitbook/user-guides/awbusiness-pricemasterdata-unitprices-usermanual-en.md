---
description: "EN-UM-AWBusiness_4"
---


# Tutorial 1: Price Master Data

---
## Input of Unit Prices

Unit prices are normally used for single lites and single products. For practicality's sake, the number of the price table should be the same as the number of the product for which the new prices are defined. This way, price tables can be easily allocated to the products.

The standard settings from the price tables and rates can be changed in the order - just like every individual price.

There are the following instructions for this session:
- "Just copy one of the existing prices and amend the data for the new price." on page B-301
- "How to create a price table for a unit price" on page B-302
- "How to enter a unit price" on page B-304

> **Prerequisite**
> Definition of prices is based on existing price years, price keys, and rates.
>
> ⇨ "Editing rates" on page B-292

The steps for defining a new price table are always the same. They will therefore be explained only briefly in connection with the other types.

> **How to enter a price table for a product**
> Copy prices You do not have to enter the prices from scratch if similar prices have been defined before.
>
> ⇨ "Copying and Changing Prices" on page B-311

- **Just copy one of the existing prices and amend the data for the new price.**

1.  Go to menu Master data > Products > Articles > Articles.
    Dialog Product management appears.
    ⇨ Software Reference, "Product Management" on page B-664
2.  Search the product for which you want to define a price.
3.  Go to tab Price/surcharge.

*A+W Business Master data*
*B-301*

## Price Master Data

*A screen capture of the 'Product management' window, showing the 'Price/surcharge' tab for product 150134/A+W IG Training.*

**A** Sales price list
**B** Purchase price list

*Fig. B-144: Entering price tables for a product*

4.  Click on the price list icon.
    Price management appears with a message that there are no data for these tables.
5.  Acknowledge the message by [OK].
    The message disappears. You can now enter the price for your product. Proceed as described in the following instructions from step 2 onwards.

### How to create a price table for a unit price

1.  Select menu Master data > Prices > Prices.
    Dialog Prices appears.
    ⇨ Software Reference, “Prices" on page B-770
2.  Go to the menu Start > New to switch to the input mode.

*B-302*
*A+W Business Master data*

## Price Master Data

*A screen capture of the 'Prices' window, tab '1.Price selection', showing various fields for defining a new price table.*

**A** Number of the price table
**B** Search by product number
**C** Price list, key (rate)
**D** Restriction to group or partner

*Fig. B-145: Fields for the new price table (unit price) is accessible*

3.  Fill in the fields in section Identification.
    The number of the table (A) already appears if you have accessed this dialog from product management.
    If no number is shown you can use the zoom icon (B) to search for the product in order to adopt the number.
    Alternatively, you can enter a number you have defined acc. to other criteria.
4.  Choose the year, the key, and the key text (C).
    Please remember that you can select only combinations of price list and key which have been defined as rates.
5.  Skip the field in sections Other surcharges, Prices, and - if applicable - Differences. You can enter these data later, after handling the subject of Surcharges.

*A+W Business Master data*
*B-303*

## Price Master Data

> **Individual price**
> If the price shall be valid only for a certain customer, select this customer in section Prices for (D). For purchase prices you can select a supplier. You can enter the prices for a customer group or a supplier group. The following steps are identical.

6.  Select in the menu Start > Save to save the data.
    The price table will be saved. Now enter the price. A unit price is entered as described below. The other price types are described in separate units.

### How to enter a unit price

1.  Go to tab Unit price.
    All price lists are shown in red as long as no prices have been defined.

*A screen capture of the 'Unit price' tab in the 'Prices' window, showing a list of price rates in red, indicating no prices have been defined yet.*

**A** Price
**B** Unit for calculating the price.
**C** Currency

*Fig. B-146: Unit price - minimum entries*

2.  Position the cursor in field Price (A) and enter the amount.
    Please make sure to choose the correct rate.
3.  Go to field Price unit (B) and choose the reference unit for this price.
    You can position the cursor on this field to open a combo box.

*B-304*
*A+W Business Master data*

## Price Master Data

*A screen capture of a dropdown menu for the 'Price unit' field, showing options like 'qm', 'kg', 'Lfm', etc.*

4.  Skip the entries for the minimum values and for the rounding. These can be added later.
5.  Choose the currency (C).
    If the column is invisible you can use the `<Tab>` key to access the field or move the view using the scroll grill.
6.  Select in the menu Start > Save to save the data.
    The price will be saved. The entries in the line appear in black letters.

*A screen capture of the 'Unit price' tab after a price has been entered. The previously red lines are now black, and values for price, price unit, and currency are filled in.*

The price table can now be allocated to the product in product definition.
⇨ "Product Definition" on page B-245

*A+W Business Master data*
*B-305*

## Price Master Data

### Defining a Shape Price

Shape prices are usually a surcharge on the glass price. These surcharges can be defined for all glass types used for the production of shapes.

The general shape surcharge for single annealed is defined for the product group <n.e.>. For all other product types, different shape surcharges are entered, e.g. for tempered glass lites with shapes. Shape surcharges can also be graduated by means of limits.

> **Knowing the input principles**
> Before entering a price for shapes you should have entered at least a unit price. The following description is based on this knowledge.
>
> Shape prices can be graduated by a limit type. If you want to define a graduation please read the chapter on graduated prices. Shape prices can be graduated in the same way. These steps are not included in the following instructions. If graduated prices are required for one product group only we recommend to create a special table for this, e. g. for the processing of shapes.

*B-306*
*A+W Business Master data*

## Price Master Data

### How to enter a price as a shape surcharge

1.  Select menu Master data > Prices > Prices.
    Dialog Prices appears.
    ⇨ Software Reference, “Prices" on page B-770
2.  Go to the menu Start > New to switch to the input mode.
3.  Fill in the fields in section Identification as described in connection with the unit price.
    ⇨ "How to create a price table for a unit price" on page B-302
4.  Go to tab Shape.

*A screen capture of the 'Shape' tab in the 'Prices' window, showing fields for defining a shape surcharge.*

**A** Product group for which shape prices are calculated
**B** Limit type
**C** Price unit
**D** Surcharge per step
**E** Minimum values
**F** Currency
**G** General surcharge for shapes

*Fig. B-147: Price surcharge for shapes*

5.  In product group `<n.e.>/<n.e.>` (G), choose the price unit (C), e. g. Net-%.
    The selection of product groups and valid price units are listed in the combo box when you move the cursor to the corresponding field.

*A+W Business Master data*
*B-307*

## Price Master Data

6.  Enter the value in column (D), e. g. 18,00.
    Based on these entries, a surcharge of 18% of the net price will be added to all lites when a shape is produced. Since no graduation has been defined, a surcharge will be applied to all sizes.
    You can now enter other surcharges for certain product groups, e. g. for IG or tempered glass.
7.  Open the context menu by a right mouse click on the column header.

    *A screen capture of a context menu with options 'Insert' and 'Delete' > 'Above' / 'Below'.*

8.  Select the entry Insert > Below to release the next column.

    *A screen capture showing a new empty row added for another product class surcharge.*

9.  Select the product group and repeat the steps 5 and 6 for this product group.
    Position the cursor on the field to produce a combo box offering a selection of valid product groups.
10. Select in the menu Start > Save to save the data.
    The data will be saved. The price table can now be allocated to the products (shapes) in product definition.

## Definition of grill Prices

Grills are calculated either by linear meter or by field. Define how the price is composed, e.g. of grill, edge connection, and cross.

> **Knowing the input principles**
> Before entering a price for grills you should have entered at least a unit price. The following description is based on this knowledge.
>
> Grill prices can be graduated by a limit type. If you want to define a graduation please read the chapter on graduated prices. Grill prices can be graduated in the same way. These steps are not included in the following instructions.

Before entering the price you should consider which grill elements shall be calculated and which shall be included in the price. Individual settings can be made for the following elements:
-   General:
    This means that the grills per lite will be calculated, i. e. the entire grill pattern.
-   Price per horizontal and vertical grill

*B-308*
*A+W Business Master data*

## Price Master Data

-   Price per field
-   Price per edge connection, cross
-   Price per edge connection, cross Price per L-, T-, or X connection
-   Price per moon, sun, arc

Selection of the price unit refers to the corresponding grill element; only the following types are practical:
-   Proportional surcharge on the basic price, net or gross
-   per meter
-   per piece

**Examples**
-   Different prices per Lin.m. of horizontal and vertical grill
-   Price per edge connection, cross, moon, and sun - per piece.
-   Surcharge on the grill price for L-, T-. Y-, or X connections and arcs

### How to enter a price for grills

1.  Select menu Master data > Prices > Prices.
    Dialog Prices appears.
    ⇨ Software Reference, “Prices" on page B-770
2.  Go to the menu Start > New to switch to the input mode.
3.  Fill in the fields in section Identification.
    These steps are described in detail in connection with unit prices.
    ⇨ "How to create a price table for a unit price" on page B-302
4.  Go to tab grills.

*A+W Business Master data*
*B-309*

## Price Master Data

*A screen capture of the 'Georgian bars' (grills) tab in the 'Prices' window, showing a list of grill elements and fields for their pricing.*

**A** Grill element
**B** Price unit
**C** Limit type
**D** Price or surcharge per step
**E** Minimum values

*Fig. B-148: Prices for grill elements*

In this example, a price per linear meter is entered for the individual grills.
5.  In the line for horizontal grills (A), choose the price unit (B), e. g. Lin.m.
    Position the cursor on the field to produce a combo box offering a selection of valid price units.
6.  Enter a value in the next column (D), e.g. 18.00.
    Based on these entries, a price of 18 € will be calculated per meter of horizontal grill.
7.  Repeat steps 5 and 6 for the next grill element.
8.  Select in the menu Start > Save to save the data.
    The data will be saved. The price table can now be allocated to the products (grill) in product definition.

*B-310*
*A+W Business Master data*

## Price Master Data

## Copying and Changing Prices

This function can be used to copy a single price or entire price lists. When copying prices, you can allocate them to another customer or supplier and also change them. In the following examples, the processes will be described separately for easier understanding.

> **Prerequisite**
> Before copying prices you have to enter the target price lists, price keys, and rates.

There are the following instructions on this subject.
- "How to copy prices from one rate to another" on page B-311
- "How to change the prices in general" on page B-312

### How to copy prices from one rate to another

1.  Select menu Master data > Prices > Prices.
    Dialog Prices appears.
    ⇨ Software Reference, “Prices" on page B-770
2.  Go to menu Functions > group Prices > Copy.

*A screen capture of the 'Copy prices' window, showing source and target data fields for copying prices.*

**A** Price type
**B** Define the source data
**C** Select the table numbers
**D** Enter the target data
**E** Choose the price units

*Fig. B-149: Copy prices*

⇨ Software Reference, "Copy Prices" on page B-782

*A+W Business Master data*
*B-311*

## Price Master Data

3.  Select the price tables (C) to be copied.
    If you want to copy the complete rate you do not have to enter any table numbers. When you enter 1 to 999999, all tables will be transferred. Enter the price list and the key (rate).
    In this example, just a single table is copied to another price list.
4.  Choose the price type (A)
    If you have not chosen the option General you have to choose the corresponding codes, e. g. Customer group, Project, and Group. The input fields released depend on the selected option.
    In this example, the selection is not restricted any further.
5.  Repeat steps 3 and 4 in section target (D).
6.  Check the checkboxes (E) of the price units you want to adopt.
7.  Click on [OK] to save the data.
    The data will be saved. The price tables are copied from the source rate to the target rate as they are.

### How to change the prices in general

1.  Go to menu Master data > Prices > Prices.
    Dialog Prices appears.
2.  Go to menu Functions > group Prices > Change.

*A screen capture of the 'Change prices' window, showing fields for selecting price tables and defining the price change.*

**A** Selection of price tables
**B** Select the rate
**C** Type of change
**D** Calculation value and type

*Fig. B-150: Change Prices*

*B-312*
*A+W Business Master data*

## Price Master Data

3.  Choose the price tables (A) and the rate (B) to be changed.
4.  If required, choose the price type and the corresponding code, e. g. Customer group, Project, and Group.
    The input fields released depend on the selected option.
5.  Define how the prices are going to be changed.
    -   Value by which the new prices shall be increased or reduced, proportionally or absolutely (C).
        Without an entry, prices will be adopted as they are.
    -   Surcharge or Discount (D) if the prices of the new list shall be increased or reduced in general.

    If you enter e. g. 3.2 in field Per cent and select the option Surcharge, all prices will be raised by 3.2%.

    If you enter e. g. 5 in field Absolute then choose the option Surcharge, all prices will be raised by 5 €.

    Option Discount works the same way.
6.  Click on [OK] to save the data.
    The data will be saved. The prices will be changed as defined.

## Exercises

-   Enter a price list which shall be used by default for purchasing.
-   Enter a price key which shall be valid for purchased shapes.
-   Define a rate for calculating the purchase price for shapes.
-   Define an additional rate for the prices entered for training purposes (including year and key!).
-   Enter a unit price.
    Remember to enter the new price in the rate you have defined for your exercises.
-   Copy a complete rate to your training rate.
-   Enter a grill price for calculating the whole grill pattern.
-   Enter a shape price (surcharge) for toughened lites.

### Additional information

⇨ Software Reference, "Price List" on page B-725
⇨ Software Reference, "Price Keys" on page B-725
⇨ Software Reference, “Rates" on page B-726

*A+W Business Master data*
*B-313*

## Price Master Data

## Graduated Prices

**Objectives**
- Introducing limit types for the graduation of prices.
- Entering prices as a matrix, vector, or cube.
- Introducing the limit type 'external PGR key'.
- Introducing the processing index.

**Benefit**
- Graduated prices allow handling special cases without having to enter a price for every possible case, e. g. for the different work required for the drilling of thin or thick lites.

**Note**

| Term | Description |
| :--- | :--- |
| **Graduated prices** | Graduated prices can be used for merchandise as well as for lites with bills of material. |
| **Limit types** | Limit types define the object of the graduation, e. g. the width, the glass thickness, the surface. <br> Limit types are used to enter graduated prices in the following ways: <br> - Vector with one limit type <br> - Matrix with two limit types <br> - Cube with three limit types |
| **Limit** | The limit type defines the steps of the graduation. |
| **Triangular form** | The triangle means that the limits of a graduation can be interchanged. <br> The triangle must only be used for glass without a sense of pattern, i.e. glass where the direction of the cuts can be changed. |
| **PGR external key** | The limit types PGR external key and PGR external key exact can be used to control the pricing by means of product groups. This option can be used for all price types except unit prices. |
| **Processing index** | The limit types Processing index and Processing index exact can be used for rating the work required and the difficulty of processing products. |

*B-314*
*A+W Business Master data*

## Price Master Data

### Limit Types for Graduations

Prices can have up to three limit types: The vector format (1 limit type), matrix (2 limit types), or cube (3 limit types). Limit types serve to graduate prices by certain criteria, e. g. by length, surface, quantity, thickness.

Graduated prices can be used for merchandise as well as for IG units.

*A screen capture of the 'Matrix' tab in the 'Prices' window, showing a triangular matrix for price graduation based on width and height.*

**A** Triangular calculation
**B** Limit type 1
**C** Limits for limit type 1
**D** Limit type 2
**E** Limits for limit type 2
**F** Price per step

*Fig. B-151: Limit types in price management (triangular matrix)*

The limit type (B, D) defines the criteria for price graduation.
For the individual steps, different limits (C, E) are used per limit type. The price (F) is defined per combination of limit types. The triangle (A) should be selected if the limits can be exchanged at pricing.

Limits offer entries for exact sizes which are useful for individual prices if e.g. a customer always orders the same sizes.

A list of available limit types and their meanings can be found in Tutorial 2.
⇨ Tutorial 2, "Available limit types" on page B-593

Two special types of limit types are going to be explained in closer detail at this point, PGR external key and the Processing index.

*A+W Business Master data*
*B-315*

## Price Master Data

### PGR External Key

The limit types PGR external key and PGR external key exact can be used to control the pricing by means of product groups. This option can be used for all price types except unit prices.

> **Different PGR external keys**
> You can allocate a PGR external key to different product groups but you can only enter one PGR external key per product group. All products the price of which is calculated by the same PGR external key have to be allocated to the same price table. You can define different external keys with different prices.

**Example**

| Product | Price table | PGR | PGR external key | Price |
| :--- | :--- | :--- | :--- | :--- |
| 1004 | 1004 | 110 | 123 | 10 €/sqm |
| 1005 | 1004 | 110 | 123 | |
| 1006 | 1004 | 110 | 123 | |
| 1008 | 1004 | 111 | 123 | |
| 1010 | 1004 | 111 | 123 | |
| 1012 | 1004 | 111 | 123 | |
| 1015 | 1004 | 112 | 124 | 12 €/sqm |
| 1019 | 1004 | 113 | 124 | |

The use of this limit type is described in a separate section.
⇨ "Price Calculation by PGR" on page B-330

*B-316*
*A+W Business Master data*

## Price Master Data

### Processing Index

The limit types Processing index and Processing index exact can be used for rating the work required and the difficulty of processing products.

**Example**
- A float lite belongs to Index 1 because it is the easiest to process.
- A laminated lite belongs to index 2 because the heated film layer sticks to the grinding wheel at cutting and these have to be cleaned afterwards.
- Wired glass belongs to index 3 because the wear of the cutting wheel is highest here.

*Two screen captures showing A) a price vector graduated by 'Processing index' and B) the 'Processing index' field in product master data.*

**A** Price graduation by processing index
**B** Allocation in product master data

*Fig. B-152: Use of the limit type 'processing index'*

You can enter a price table (A) for every processing index of a product group. In product master data (B), define the processing index to which the product belongs.
⇨ Software Reference, "Processing Index" on page B-681

*A+W Business Master data*
*B-317*

## Price Master Data

### Parameterized macros

With the limit types Macro 1-10 and Macro 1-10 Dimension you can define the pricing according to the parameters of a macro.

*A screen capture of a dropdown menu showing various 'Macro' limit types.*

*Fig. B-153: Use of the limit types macros 1-10*

In the first step, define the limit quantity(s) according to the type of the dimension or numerical value parameter (e.g. angle). In case of a dimension parameter, the limit type Macro 1-10 (Dimension) must be used.

*A screen capture showing the 'Price Vector' tab with 'Macro 1 (Dim.)' as the limit type and defined limit quantities with prices per piece.*

*Fig. B-154: Defined limit quantities*

The prices can then be scaled in the price management according to these new limit quantities.

*B-318*
*A+W Business Master data*

## Price Master Data

*A detailed screen capture illustrating how macro parameters from an order item's Bill of Materials (BOM) are linked to the defined macro limit quantities for pricing. Arrows show the flow from the parameter value (e.g., 'W' = 200) to the corresponding price (20.00 Stk).*

*Fig. B-155: Limit quantities in the price management*

*A+W Business Master data*
*B-319*

## Price Master Data

### Vector

In case of vector, you enter the price based on a limit type, e.g. meter, piece, surface, liter. These prices can be graduated by quantity.

*A screen capture of the 'Vector' tab in the 'Prices' window.*

**A** Graduation values
**B** Limit type
**C** Price per limit type
**D** Price unit

*Fig. B-156: Vector*

This example shows that the price (C) is graduated by the length (A) of the longest edge (B). It does not matter whether the length is entered as width or height. The price will be calculated by surface (D).
Price unit and Limit type do not have the same.

**Example**

| Limit | Price |
| :--- | :--- |
| up to 0.25 sqm | 40.00 € per piece |
| up to 0.35 sqm | 35.00 € per piece |
| up to 10.00 sqm | 50.00 € per sqm |
| up to 25.00 sqm | 40.00 € per sqm |

In this example, the price for the limit type Surface (price units: pc. and surface) is graduated:

*B-320*
*A+W Business Master data*

## Price Master Data

-   For lites up to 0.25 sqm, 40 € per piece shall be calculated.
-   For lites from 0.26 sqm to 0.35 sqm, 35 € shall be calculated per piece.
-   For lites from 0.36 sqm to 10 sqm, 50 € shall be calculated per sqm.
-   For lites from 10.1 sqm to 25 sqm, 40 € shall be calculated per sqm.

For drilled hole for example, the combination of the limit type Diameter with limits in millimeters and the price unit Piece will be useful.

### Matrix

In a matrix, the price depends on two limits, e.g. width and height or surface and thickness.

*A screen capture of the 'Matrix' tab in the 'Prices' window, showing a price grid based on two limit types.*

**A** Limit type 1
**B** Limit type 2
**C** Graduation for limit type 2
**D** Graduation for limit type 1
**E** Triangular form

*Fig. B-157: Matrix*

*A+W Business Master data*
*B-321*

## Price Master Data

### Triangle

You can create a triangular matrix so that the limit types can be exchanged, e.g. height and width. You only have to enter one of the combinations. With triangular price tables, the cutting direction does not matter.
At order entry, sizes are turned so that the bigger size is the height, no matter in which sequence the sizes for width and height are entered.

> **Non-applicability of the triangle**
> A price table must not be entered as a triangle if the direction in which the glass is cut is important. If height and width of patterned glass must not be exchanged, you have to enter all prices for all possible combinations.

**Example**
*A table showing a triangular price matrix for different width and height combinations.*

In the triangle, the following sizes will have the same price, e.g. 67.19 €:
-   Width 840 mm x height 480 mm
-   Width 480 mm x height 840 mm

If the sizes must not be turned at order entry, you have to enter the price for all formats.
In this case, the sequence in which the sizes are entered will be taken into account; the price for a width of 1080 x height 480 mm would e.g. be 168.75 Euro.

*B-322*
*A+W Business Master data*

## Price Master Data

### Cube

Cubes are similarly structured as matrix tables but with three limits, e.g. width, height, and thickness.

*A screen capture of the 'Cube' tab in the 'Prices' window, showing a multi-level pricing structure with three limit types.*

**A** Limit type 3
**B** Graduation for limit type 3
**C** Prices on level 1
**D** Prices on level 2

*Fig. B-158: Cube*

As for a matrix, please remember: If you enter the prices as a triangle, you do not have to enter all prices for all combinations of limit types.

**Graduation limit**
If you want to enter graduations only up to a certain size you can define a 'next key'.
⇨ "Next key" on page B-282

*A+W Business Master data*
*B-323*

## Price Master Data

## Defining a Graduated Price with Limits

For some products, price graduation by one or more limit types is useful, e. g. drilling by thickness, IG units by size.

> **Knowing the input principles**
> Before entering a graduated price you should have entered at least a unit price. The following description is based on this knowledge.

The following steps show how to define a price graduation for IG units in the shape of a cube. This allows to show the application of three limit types. Similarly, these instructions can be used for defining prices in other graduation types.

After selecting the type, the sequence is the same for all:
-   Select limit types.
-   Enter the limits for the graduation.
-   Enter prices.

> **Prerequisite**
> Definition of prices is based on existing price years, price keys, and rates.
>
> ⇨Tutorial 1, "Editing rates" on page B-292

There are the following instructions for this session:
- "How to enter a graduated price" on page B-324
- "How to define the limits for limit type 1" on page B-326
- "How to define the limits for limit type 2" on page B-327
- "How to define the limits for limit type 3" on page B-328
- "How to copy the prices from one level to another" on page B-328

### How to enter a graduated price

1.  Select menu Master data > Prices > Prices.
    Dialog Prices appears.
    ⇨ Software Reference, “Prices" on page B-770
2.  Go to the menu Start > New to switch to the input mode.
3.  Fill in at least the fields in section Identification.
    These steps are described in detail in connection with unit prices.
    ⇨ "How to create a price table for a unit price" on page B-302
4.  Go to tab Cube.

*B-324*
*A+W Business Master data*

## Price Master Data

*A screen capture of the 'Cube' tab in the 'Prices' window, showing the empty structure for a cubic price graduation.*

**A** Column header
**B** Line header
**C** Enter the limit
**D** Limit type 1
**E** Enter the limit
**F** Limit type 2
**G** Enter the limit
**H** Limit type 3

*Fig. B-159: Price graduation, cubic shape*

⇨ Software Reference, “Prices" on page B-770
5.  Check the checkbox Triangle.
    If you do not check this checkbox you have to enter the prices for all combinations of the selected limit types, e.g. for all widths and heights as well as the thicknesses if required.
    ⇨ "Limit Types for Graduations" on page B-315
6.  Enter the minimum values for pricing.
    You can enter the value 300 mm as the smallest limit for the width and height although minimum sizes of 200 x 300 mm shall be valid for production. Pricing will only consider the limit sizes only for calculation but not for production.
    This way, the price for the minimum quantity will be calculated even for a smaller lite.
7.  Enter the Price unit and the Currency.

*A+W Business Master data*
*B-325*

## Price Master Data

The price unit is the reference size to which the graduation refers. The currency is essential if you are working with several currencies.
8. Choose the limit types (D, F, H), e. g. width, height, and thickness (BOM).
   By selecting these limit types you define that the price of the lite does not only depend on its size but also on the total thickness.
9. Select in the menu Start > Save to save the data.
   The data will be saved. Now enter the limits for the graduation. Start with limit type 1.

### How to define the limits for limit type 1

1.  Open the context menu by a right mouse click on the column header (A).

    *A screen capture showing a right-click context menu on a column header with options to Change, Insert, Delete.*

    **A** Column header
    **B** Context menu

    *Fig. B-160: Adding a step for the width*

2.  Select the entry Insert > Above from the context menu (B) .

    *A screen capture showing a new empty column added for entering a limit.*

    **A** New column
    **B** Enter the limit

    *Fig. B-161: Adding the limit for the width*

    The field for entering the limit (B) is accessible and a new column (A) is added.
3.  Enter the value for limit type 1 (B), e. g. 480 and confirm your entry by pressing the `<Tab>` key.
    The value appears in the new column header (A).
4.  Repeat the steps until all limits for the width have been set.
    Next, set the limits for limit type 2.

*B-326*
*A+W Business Master data*

## Price Master Data

### How to define the limits for limit type 2

1.  Open the context menu by a right mouse click on the line header.

    *A screen capture showing a right-click context menu on a line header with options to Change, Insert, Delete.*

    **A** Line header
    **B** Context menu

    *Fig. B-162: Adding a step for the height*

2.  Select Insert > Below (B) in the context menu.

    *A screen capture showing a new empty row added for entering a limit.*

    **A** Enter the limit
    **B** New line

    *Fig. B-163: Adding the limit for the height*

    The field for entering the limit (A) is accessible and a new column (B) is added.
3.  Enter the value, e. g. 900 and confirm your entry by pressing the `<Tab>` key.
    The value appears in the new line header.
4.  Repeat the steps until all limits for the height have been set.
    The first level of the cube has not been defined. Decide how you want to proceed:
    -   Set the limits for limit type 3.
    -   Enter prices on the first level.
        Position the cursor on the appropriate line and enter the price.

*A+W Business Master data*
*B-327*

## Price Master Data

### How to define the limits for limit type 3

1.  Open the context menu by a right mouse click on the combo box below the first column.

    *A screen capture showing a right-click context menu on the limit type 3 combo box with options Change, Insert, Delete, Copy.*

    **A** Enter the limit
    **B** Define a new level

    *Fig. B-164: Adding a step for the thickness*

2.  In the context menu, select Insert (B).
    The field for the thickness limit (A) is accessible; a new tab will be added.
3.  Enter the value, e. g. 24 and confirm your entry by pressing the `<Tab>` key.

    *A screen capture showing the new thickness level '24' added as a tab.*

    The value appears in the combo box. Repeat the steps until all thickness levels have been defined.
    If you had entered prices on the first level, these will be adopted for the new level. You can amend these prices as required. A copy function allows the automatic adjustment of prices.

### How to copy the prices from one level to another

1.  Choose the level with the prices to be copied.
    The prices are identical on all levels provided they had been defined before further levels were added.
2.  Open the context menu by a right mouse click on the combo box of the levels.

    *A screen capture showing a right-click context menu with the 'Copy' option highlighted.*

    **A** Change the limit
    **B** Copy level

    *Fig. B-165: Context menu*

3.  Select Copy (B) from the context menu

*B-328*
*A+W Business Master data*

## Price Master Data

*A screen capture of the 'Copy prices - Cube' dialog box.*

**A** Target level
**B** Proportional value of the change
**C** Absolute value of the change
**D** Price increase or reduction

*Fig. B-166: Context menu*

4.  Select the level (A) to which the prices shall be applied.
5.  Define how the prices are going to be changed.
    -   Proportional (B) or absolute (C) value by which the new prices shall be changed.
    -   Surcharge or reduction (D).
    If you enter e. g. 3.2 in field Per cent and select the option Surcharge, all prices will be raised by 3.2%.
    If you enter e. g. 5 in field Absolute then choose the option Surcharge, all prices will be raised by 5 €.
    Option Discount works the same way.
6.  Click on [OK] to copy the data.
    The prices are applied to the target level as defined. To transfer the prices to other levels please be careful to check the level from which the prices are copied.
7.  When you have entered the prices on all levels go to menu Start > Save to save the data.
    The data will be saved. They can be allocated to price tables in product definition.

*A+W Business Master data*
*B-329*

## Price Master Data

## Price Calculation by PGR

Normally, every product gets a price. Pricing can also be controlled by means of the product groups.

This is done in two steps:
-   First enter an external key in the product group.
-   This external key is entered as a limit in the price table.

You can select the limit type External PGR key for all price types except the unit prices.

There are the following instructions on this subject.
- "How to enter an external key in a product group" on page B-330
- "How to allocate the external keys as limits" on page B-331

### How to enter an external key in a product group

1.  Go to Master data > Products > General > PGR.

*A screen capture of the 'PGR' (Product groups) window.*

**A** Select the PGR
**B** Enter the external key

*Fig. B-167: Enter an external key for PGR*

⇨ Software Reference, "PGR" on page B-644
2.  Choose the product group (A).
3.  Enter the value of the External PGR key in field External key (B).

*B-330*
*A+W Business Master data*

## Price Master Data

You can choose this at random but you can only enter numerical values, e. g. 123. The same value can be entered as an external key for several product groups.

*A screen capture of the 'PGR' window with the 'External key' field filled in with the value '123'.*

*Fig. B-168: External key for PGR*

4.  Select in the menu Start > Save to save the data.
    The data will be saved. You can now enter this external key in the price table as a limit.

### How to allocate the external keys as limits

1.  Select menu Master data > Prices > Prices.
    Dialog Prices appears.
    ⇨ Software Reference, “Prices" on page B-770
2.  Search the price for which you want to enter an external key, or create it.
    ⇨ "How to enter a graduated price" on page B-324
3.  Go to the tab in which the limits shall be entered, i.e. Matrix, Vector or Cube.

*A+W Business Master data*
*B-331*

## Price Master Data

*A screen capture of the 'Price vector' tab, set up to use the 'PGR foreign key' limit type.*

**A** External key (number)
**B** Select the limit type
**C** Price
**D** Price unit

*Fig. B-169: External key for PGR*

4.  Choose the limit type PGR external key (B) and enter the value (A) you have defined in the product groups, which in this case is 123.
5.  If necessary, enter the price (C) if no price had been entered in the table as yet.
6.  Select in the menu Start > Save to save the data.
    The data will be saved. The price is now used for calculating all products allocated to the PGR in which the external key has been entered.
    If you want to work with several external PGR keys you can e.g. create a cube in which the external PGR key is used as a third limit type.
    You can e.g. define an external PGR key for tempered glass and another for laminated lites.

### Exercises

-   Consider for which products a simple price is practical and for which a graduated price is recommended.
-   Define a price with limits.

*B-332*
*A+W Business Master data*

## Price Master Data

-   Determine the way and graduation for entering prices. Based on these considerations you have to choose a matrix, a vector, or a cube.
    > **Graduation of limits**
    > There are no restrictions regarding the graduation of limits. The graduation should be logically connected to the selected limit type however.
-   Copy the new prices with a reduction of 2.5 % for your training customer. Attention. the reduction should only be valid for the training customer!

### Additional information

⇨ Software Reference, "Price Management" on page B-768
⇨ Software Reference, “Prices" on page B-724
⇨ Software Reference, "Price Groups" on page B-745
⇨ Software Reference, "Price and Quantity Unit" on page B-759
⇨ Software Reference, "Company Data > Price Calculation" on page B-970
⇨ Software Reference, "Calculate external PGR key as an inexact quantity limit" on page B-979

*A+W Business Master data*
*B-333*

# Surcharges

Surcharges are another means of adapting your price lists. Surcharges can be applied to certain products, processing steps, or in general.

This subject area will introduce the different surcharges and their functions.

This includes the following training sessions:
- "Einführung in das Thema Zuschläge" auf Seite B-374
- "Gruppenzuschläge" auf Seite B-377
- "Austauschzuschläge" auf Seite B-395
- "Modellbearbeitungszuschläge" auf Seite B-408
- "Sonstige Zuschläge" auf Seite B-413
- "Automatische Zuschläge" auf Seite B-432

*B-334*
*A+W Business Master data*

## Introduction of the Subject 'Surcharges'

Surcharges can be added for special services, e. g. for replacing one lite of an IG unit or for complex edgework for shapes.

### Surcharges for products and processing steps

The following surcharges are defined in direct connection with the prices for products and processing steps:
- Group Surcharges
- Replacement Surcharges
- Shape Processing Surcharges
- Miscellaneous Surcharges
- Automatic Surcharges

These surcharges are entered in Master data > Prices. Every surcharge can be defined for a customer or supplier group, for individual customers or suppliers.

Define the surcharge type and surcharge value to calculate these surcharges:
- The surcharge type defines the unit to which the surcharge refers, e. g. the surface, the price, the quantity.
- The surcharge value defines the amount of the surcharge.

Surcharges can be graduated in different ways. As for prices, limit types and limits are defined.

⇨ "Limit Types for Graduations" on page B-315

In an order, surcharges can be changed, removed, and others can be added. Shape-, grill-, or exchange surcharges will be included in pricing even if the price in the order is changed by hand. In contrast, Other surcharges will be taken into account in case of manual price changes only if they have been explicitly released for that.

*A+W Business Master data*
*B-335*

## Surcharges

### Product/surcharge allocation (automatic surcharges)

A special type are the so-called automatic surcharges, e.g. for toll, delivery fees, or energy surcharges. These surcharges are entered in Master data > Company > Product/surcharge allocation.

### Calculation sequence for surcharges

Surcharges for products and processing steps are calculated when the product is entered in an order. This is also the case if the product is a BOM element.

Since different surcharges can be defined it may happen that several surcharges are applied to an order item. This is relevant for pricing if the surcharge type Gross % is involved. The gross price to which a certain surcharge refers can already include another surcharge.

> **Sequence of sessions**
> The individual sessions in this set of topics are each based on the knowledge acquired in the previous session. This sequence does not match the sequence in which the dialogs appear in the Master data menu.

*B-336*
*A+W Business Master data*

## Surcharges

### Surcharge Settings (Company Data)

The standard calculation of surcharges can be changed in company data.

*A screen capture of the 'Company data > Pricing' settings window, showing numerous checkboxes for configuring price calculation parameters. Three specific checkboxes related to surcharge calculation are highlighted.*

*Fig. B-170: Company data > Pricing*

This tab is used for defining the options for the documents. Any changes on this tab will overrule the standard calculation in A+W Business.

For a detailed description of the checkboxes please refer to the software reference.

*A+W Business Master data*
*B-337*

## Group Surcharges

**Objectives**
- Introducing the group surcharge function.
- Price group allocation.
- Defining group surcharges.

**Benefit**
- A surcharge - based on the glass thickness - can be applied if lites in IG or laminated glass units are exchanged.
- Group surcharges refer to glass types united in price groups. The surcharge for exchanging a lite therefore does not have to be defined per glass (product).

**Note**

| Term | Description |
| :--- | :--- |
| **Price groups** | Price groups collect products in groups for which no separate price tables shall be created and maintained. Price groups are used for managing surcharges and discounts. |
| **Calculation parameters** | Surcharge calculation is based on different parameters, e. g.: <br> - Value, per cent or absolute <br> - Reference unit, e.g. surface, standard price, piece <br> - Quantity of the order item |
| **Surcharge type** | The rules for proportional surcharges are: <br> - Gross price = before deduction of discounts <br> - Net price = after deducting the discounts |
| **Group surcharges** | Group surcharges refer to products allocated to a price group. |
| **Surcharge calculation** | The surcharge is applied if lites belonging to these price groups are replaced. |
| **Property of group surcharges** | A decisive property of a group surcharge is the glass thickness defined in the bill of materials. Different surcharges can be defined for glass of the same thickness. |
| **Customer or supplier surcharges** | When defining the group surcharge, a surcharge can be allocated to customers, suppliers, groups of partners or objects. |

*B-338*
*A+W Business Master data*

## The Function of Group Surcharges

Group surcharges refer to products allocated to a price group. The surcharge is applied if lites belonging to these price groups are replaced. Decisive for a group surcharge is the glass thickness defined for the IG or laminated glass unit.

**Example**

| Glass thickness | Price group | Surcharge | Surcharge type | Minimum surface |
| :--- | :--- | :--- | :--- | :--- |
| 4 | A | 9.20 | sqm | 0.50 |
| 4 | B | 12.27 | sqm | 0.50 |
| 4 | C | 15.34 | sqm | 0.50 |
| 4 | D | 19.43 | sqm | 0.50 |
| 4 | E | 23.52 | sqm | 0.50 |
| 5 | A | 9.92 | sqm | 0.50 |
| 5 | B | 12.97 | sqm | 0.50 |
| 5 | C | 16.34 | sqm | 0.50 |
| 5 | D | 21.23 | sqm | 0.50 |
| 5 | E | 24.32 | sqm | 0.50 |

As you can see from these examples, different surcharges can be defined for glass of the same thickness. The glass thickness is specified because a price group can include glass of different thicknesses while the surcharge shall only be applied to glass of the specified thickness.

**Example**
Price group A shall include all colored single glass types, group B includes all patterned glass types, etc.
Group surcharges for the price groups A-E have been defined for a thickness of 4 mm and 5 mm of the exchanged lite.
For a 4 mm glass of price group A, a surcharge of 9.20 € per sqm would be applied. For a surface of up to 0.5 sqm, this is a surcharge of 4.60 €.
This surcharge will not be applied for colored lites of 3 mm thickness.

Group surcharges are defined in three steps:
- First define the price groups.
- Next, allocate the glass types to the price groups.
- Last, define the surcharges per thickness for the price groups.

> **Exchange of BOM elements**
> You can define an exchange surcharge for glass that cannot be allocated to any price group.
>
> ⇨ "Replacement Surcharges" on page B-356

*A+W Business Master data*
*B-339*

## Dialog 'Group Surcharges'

Dialog Group surcharges offers various tabs for surcharge allocation.
- **Price management:** These surcharges refer to generally applicable prices.
- **Customer selection:** These surcharges refer to the price lists for special customers.
- **Supplier selection:** These surcharges refer to the price lists for special suppliers.

The allocation to a customer or supplier price cannot be changed.

*A screen capture of the 'Group Surcharges' dialog, showing an overview of defined surcharges based on glass thickness and price group.*

**A** Surcharge on the sales or purchase price
**B** Combination of rates
**C** Product type for which the surcharge is valid.
**D** Validity of the surcharge
**E** Price group to which the surcharge applies.
**F** List of surcharges

*Fig. B-171: Dialog 'group surcharges'*

This example shows that there are different surcharges e.g. for lites of 4 mm thickness per price group (E).

Group surcharges apply to a certain rate (B). A combination of the price list `<n.e.>` and the key `<n.e.>` can also be used if prices have been entered for this combination.

*B-340*
*A+W Business Master data*

## Surcharges

Since group surcharges always refer to the exchange of a lite they can only be applied to IG or laminated glass lites (C).

### Price Groups and Price Group Allocation

For calculating surcharges and patterned glass you can define price groups to which the products are allocated. This simplifies the maintenance of price lists because you do not have to keep separate price lists for all these products.

As for products and partners, start by entering the (empty) groups as a basis. After that, allocate the products to the corresponding price group. Define the price group that is valid if the product is exchanged in an IG and/or laminated glass unit.

*A screen capture of the 'Price Group allocation' window, showing price groups and the allocation of products to these groups for IG and LG units.*

**A** Price groups
**B** Number of the allocated product
**C** Patterned glass
**D** Price group to be used when exchanging a lite in an IG unit
**E** Price group for exchanging a lite in a laminated glass unit

*Fig. B-172: Price groups and price group allocation*

*A+W Business Master data*
*B-341*

## Surcharges

These examples show that price groups A to N (A) have been defined. In dialog Price group allocation, the following allocation is defined for the first patterned glass (C):
-   If the glass is used for an IG unit (D) it is allocated to price group A.
-   If the glass is used for a laminated glass unit (E) it is allocated to price group B.

You can define any required number of price groups. You should however decide in advance which glass types can be united in a group so that the surcharges and/or prices can be maintained together.

### Price Group Allocation

By allocating products and price groups, you join glass types for which the same surcharge shall be calculated in case of an exchange. You should therefore first specify (on paper) which glass types are to get the same group surcharge.

If price group allocation is impossible, you can define an exchange surcharge to be added to the standard price. This surcharge will be introduced in the next session.

⇨ "Defining an Exchange Surcharge" on page B-360

> **Prerequisite**
> Price groups can be allocated only if price groups, products, and rates have been defined before.

*B-342*
*A+W Business Master data*

### How to allocate a product to a price group

1.  Go to menu Master data > Prices > Price group allocation.
    Dialog Price group allocation appears.
    ⇨ Software Reference, "Price Group Allocation" on page B-746

*A screen capture of the 'Price Group allocation' window, highlighting the Sales list and Purchase list options.*

**A** Sales list
**B** Purchase list

*Fig. B-173: Allocation to SP or PP*

2.  Choose one of the options in section Identification - rate, e. g. Sales list (A).
3.  Go to the menu Start > New to switch to the input mode.

*A+W Business Master data*
*B-343*

## Surcharges

*A screen capture of the 'Price Group allocation' window in input mode, with fields ready for new data entry.*

**A** Select the rate
**B** Select the product
**C** Select the price group

*Fig. B-174: Fields for the new allocation are accessible*

4.  In the fields Price list and Price key (A), select the rate for which the price group allocation shall be valid.
5.  Choose the product (B) to be allocated to the price group.
    You can enter either the product number or the matchcode. The selected product appears in section List of allocations.
6.  Click on the field in column PG IG (C) and select the price group, e. g. A.
    A selection of valid price groups appears in a combo box when you position the cursor on this field.

*B-344*
*A+W Business Master data*

## Surcharges

*A screen capture showing the product 'Orn. Gothik Bronze 4 mm' allocated to price group A for IG units.*

*Fig. B-175: Product allocated to the price group*

You have thus defined that the selected glass belongs to price group A if it is part of an IG unit.

7.  Allocate the price group in column PG LG if the glass is also used for laminated glass lites.
8.  Select in the menu Start > Save to save the data.
    The data will be saved.
9.  Repeat the steps 3 and 8 to allocate more glass types to the price groups.
    You can now enter the group surcharges for price groups.
    ⇨ "Defining a Group Surcharge" on page B-346

*A+W Business Master data*
*B-345*

## Surcharges

### Defining a Group Surcharge

This surcharge type is used for defining surcharges for glass of the same thickness. The surcharges can be valid for individual customers, suppliers, or partner groups. To define a partner-related group surcharge you have to allocate the partner or the partner group when you enter the surcharge. This allocation cannot be changed afterwards.

Special conditions for a building project can be handled by applying the group surcharge to a certain project.

> **Prerequisite**
> Rates, price groups, and their allocations have to be entered before you can define group surcharges.

There are the following instructions on this subject.
- "How to define a group surcharge" on page B-347
- "How to add a group surcharge" on page B-350
- "How to change a group surcharge" on page B-350
- "How to delete a single group surcharge" on page B-351
- "How to delete all group surcharges for a thickness" on page B-351

*B-346*
*A+W Business Master data*

### How to define a group surcharge

1.  Go to menu Master data > Prices > Group surcharges.

*A screen capture of the 'Group Surcharges' window, highlighting the 'Sales list' and 'Purchase list' radio buttons.*

**A** Sales list
**B** Purchase list

*Fig. B-176: Allocation to SP or PP*

2.  Choose one of the options (C) in section Identification - rate, e. g. Sales list
3.  Go to the menu Start > New to switch to the input mode.

*A+W Business Master data*
*B-347*

## Surcharges

*A screen capture of the 'Group Surcharges' window in input mode.*

**A** Rate
**B** Select the product type
**C** Validity of the group surcharge

*Fig. B-177: Fields for new group surcharge are accessible*

⇨ Software Reference, "Group Surcharges" on page B-747
4.  In the fields Year and Key, select the rate (A) to which the group surcharge shall be applied.
5.  Select the product type (B) for which the surcharge shall be valid, e.g. IG.

*B-348*
*A+W Business Master data*

## Surcharges

*A screen capture showing a new, empty line in the 'Group Surcharges' overview, ready for data entry.*

**A** Thickness of the lite to be replaced
**B** Select the price group
**C** Surcharge value
**D** Choose the calculation type

*Fig. B-178: Fields for new group surcharge are accessible*

6.  Enter the thickness (A) of the lite to be replaced, e. g. 5.
    Remember: this is the lite to be removed from the unit.
7.  Select the price group (B) to which the surcharge shall be applied, e.g. A.
8.  Enter the value (C) of the surcharge, e. g. 100.
    Depending on the surcharge type, this value will be interpreted as a percentage or an absolute value.
9.  Choose the type (D) of surcharge, e. g. Gross %.
    With this setting, a surcharge of 100 % on the gross price of the glass will be applied to this price group.
    The combo box for selecting the surcharge type appears when you position the cursor on the field.
    You have made the mandatory entries now. The details in the following fields can be added later.
    The next section explains how to add another surcharge for another price group.
10. Select in the menu Start > Save to save the data.
    The data will be saved. With that, you have created a surcharge table for a thickness of 5 mm.

*A+W Business Master data*
*B-349*

## Surcharges

### How to add a group surcharge

1.  Go to menu Master data > Prices > Group surcharges.
    Dialog Group surcharges appears.
2.  Select the group surcharge to be added.
    Restrict your search to the price list and key. The surcharges are listed in field Overview.
3.  Go to the menu Start > New to switch to the input mode.
4.  Repeat steps 7 to 9 from the previous process to specify a surcharge for another group of lites of the same thickness, e.g. for group C.
5.  Select in the menu Start > Save to save the data.
    The data will be saved. With this, you have defined a surcharge for price groups A, B, and C for lites of 5 mm thickness.

### How to change a group surcharge

1.  Go to menu Master data > Prices > Group surcharges.
    Dialog Group surcharges appears.
2.  Select the group surcharge to be added.
    Restrict your search to the price list, key, and thickness. The surcharges are listed in field Overview.
3.  Click on the table field you want to edit, and change the entry.
4.  Select in the menu Start > Save to save the data.
    The data will be saved.

> **Allocating a partner or changing the allocation**
> A group surcharge can only be allocated when it is defined. If a certain surcharge shall be applied later to another partner or a group of partners, you have to enter the surcharge again and delete the old surcharge.

*B-350*
*A+W Business Master data*

## Surcharges

### How to delete a single group surcharge

1.  Go to menu Master data > Prices > Group surcharges.
    Dialog Group surcharges appears.
2.  Select the required entry in field Overview.
3.  Press the `<Del>` key.
    The line will be deleted for good, without a security check.

> **Deleting a table**
> If you select the command from menu Start > Delete, all group surcharges for the current rate will be deleted.

### How to delete all group surcharges for a thickness

1.  Go to menu Master data > Prices > Group surcharges.
    Dialog Group surcharges appears.
2.  Go to menu Functions > Delete prices.

*A screen capture of the 'Delete prices by price group' dialog.*

**A** Thickness, from-to
**B** Rate

*Fig. B-179: Delete Group Surcharges*

3.  Enter the thickness (A) and the rate (B).
    Please make sure to enter the same thickness in both fields.
4.  Click on [OK] and confirm the security check by [Yes].
    All entries for the selected thickness will be deleted.

*A+W Business Master data*
*B-351*

## Surcharges

## Copying a Group Surcharge

Group surcharges can be copied from one rate to another, and can be changed at the same time. This function is the same as the function for copying prices.

The copy function offers the following options:
-   Define a new surcharge by copying.
-   Copy surcharges to a new table.
-   Copy surcharges from one rate to another.
-   Copy surcharges for a partner or a group of partners.

There are the following instructions on this subject.
- "How to define a group surcharge by copying" on page B-352
- "How to change group surcharges in general" on page B-353

### How to define a group surcharge by copying

1.  Go to menu Master data > Prices > Group surcharges.
    Dialog Prices by price groups appears.
2.  Select menu Functions > Copy prices.

*A screen capture of the 'Copy exchange prices' dialog, with tabs for Source, Target, and Price change.*

**A** Glass thickness to be copied
**B** Rate (source)
**C** Product type of the group surcharges
**D** Glass thickness to which the surcharge is copied
**E** Rate (target)

*Fig. B-180: Copy function for defining a group surcharge*

⇨ Software Reference, "Copy Group Surcharges" on page B-748

3.  Enter the glass thickness (A) the surcharges of which shall be copied.

*B-352*
*A+W Business Master data*

## Surcharges

If you enter the same number in both fields, just this table will be copied. In this example, the surcharges for a thickness of 5 mm will be copied.

4.  Select the rate (B) and the product type (C).
5.  Enter the thickness (D) to which the new surcharges shall be applied, e. g. thickness 8.
6.  Select the same rate (E) so that the new surcharge is defined there.
    In this example, PP is selected.
7.  Click on [OK] to copy the data.
    The new surcharge is created. A message will tell you how many records were copied. You can display the new group surcharges by reloading the data with the appropriate settings.

### How to change group surcharges in general

1.  Go to menu Master data > Prices > Group surcharges.
    Dialog Prices by price groups appears.
2.  Go to menu Functions > Copy prices.
3.  Go to tab Price change.

*A screen capture of the 'Change prices' dialog, showing fields for price selection and price change parameters.*

**A** Price increase or reduction
**B** Value of the change

*Fig. B-181: Copy function for changing the group surcharges*

4.  Select the thickness and the rate for which the surcharges shall be changed.
    To change all group surcharges for a rate please enter a thickness of 0 to 99.

*A+W Business Master data*
*B-353*

## Surcharges

5.  Define how the prices are going to be changed.
    -   Proportional (B) or absolute (C) value by which the new surcharges shall be changed.
    -   Surcharge or reduction (D).
    If you enter e. g. 3.2 in field Per cent and select the option Surcharge, all surcharges will be raised by 3.2%.
    If you enter e. g. 5 in field Absolute then choose the option Surcharge, all surcharges will be raised by 5 €.
    Option Discount works the same way.
6.  Click on [OK] to save the data.

*A screen capture showing the 'Group Surcharges' overview with new, amended values for a glass thickness of 8 mm.*

*Fig. B-182: New group surcharges with amended values*

This example shows that the group surcharges for a glass thickness of 8 mm were defined with higher values.

### Exercises

-   Decide which glass types can be united in a price group.
-   Create a price group for patterned glass. Call it P.
-   Allocate at least three patterned glass types to this price group.

*B-354*
*A+W Business Master data*

## Surcharges

-   Enter two new surcharges for this price group:
    -   A surcharge to be calculated by surface for lites of 5 mm thickness.
    -   For glass of a thickness of 8 mm a surcharge for your training customer which is applied by piece.
    -   Which values have to be entered to make sure that the surcharge is calculated only if the surface exceeds 1 sqm?

### Additional information

⇨ Software Reference, "Price Groups" on page B-745
⇨ Software Reference, "Price Group Allocation" on page B-746
⇨ Software Reference, "Group Surcharges" on page B-747

*A+W Business Master data*
*B-355*

## Replacement Surcharges

**Objectives**
- Introducing the function of exchange surcharges.
- Defining exchange surcharges.

**Benefit**
- Pricing for orders is done automatically even if a BOM element is exchanged. The additional work incurred by the exchange is charged by means of the exchange surcharge.

**Note**

| Term | Description |
| :--- | :--- |
| **Exchange of BOM elements** | An exchange refers to products in the BOM of which an element can be exchanged, e. g. glass, film layer, spacer. |
| **Exchange surcharges** | Exchange surcharges usually refer to glass (products) that cannot or shall not be combined in groups. |
| **Exchange lite** | This is the glass to be removed from an IG unit or laminated lite. This glass will be replaced by the exchange lite. |
| **Exchange - in** | This is the glass which is going to replace the original lite. |
| **Surcharge type** | Exchange surcharges are split into the following surcharge types: <br> - Independent surcharges <br> - Thickness-related surcharges <br> - Product-related surcharges |
| **Surcharge type rules** | The rules for proportional surcharges are: <br> - Gross price = before deduction of discounts <br> - Net price = after deducting the discounts |

*B-356*
*A+W Business Master data*

## The Function of Exchange Surcharges

Exchange surcharges refer to elements that are replaced in a BOM, e.g. glass, film layers, spacers. We distinguish the replaced lite (lite to be removed) and the exchange lite (lite replacing the original one).

Exchange surcharges usually refer to lites that cannot or shall not be combined in groups. Surcharges are defined for the products in which lites can be replaced, e.g. laminated or IG units.

**Example**

| Product | Price | Total |
| :--- | :--- | :--- |
| IG unit 2 x Float 4 mm, 1 sqm, 1000 x 1000 mm | 60.00 € | 60.00 € |
| Float 4 is replaced by tempered glass | 75.00 € | 75.00 € |
| **Total** | | **105.00 €** |

Exchange surcharges can be defined in different ways:
-   **Independent surcharge:**
    The surcharge is applied to the new lite. This is the lite to be fitted. The replaced lite will be ignored.
-   **Thickness-related surcharge:**
    The surcharge is applied to the lite to be removed. The program checks the thickness of the lite for this purpose. The surcharge will be applied only if a certain new lite is going to be fitted.
-   **Product-related surcharge:**
    The surcharge is applied to the lite removed if it is replaced by a certain new glass type.

*A+W Business Master data*
*B-357*

## Surcharges

**Example**

A surcharge shall be applied if a Float 6 mm lite in an IG unit is to be replaced by a heat protection glass. The amount of the surcharge shall depend on the width and height. If the minimum size of 0.3 sqm is not met, the surcharge for the minimum height x width will be applied automatically.

This surcharge is defined as follows:
-   Independent surcharge for IG
-   Exchange lite: TG 6 mm
-   Surcharge type: sqm
-   Limit type: width x height
-   Minimum size: 0.3 sqm

**Exchange prices**

| | Width | Height | Surcharge (amount) |
| :--- | :--- | :--- | :--- |
| up to | 2400 | 2000 | 35.00 € |
| up to | 3000 | 3000 | 45.00 € |
| over | 3000 | 3000 | 70.00 € |
| **Minimum surface 0.3 sqm** | | | |

For this surcharge, the glass to be removed from the IG unit is irrelevant. This surcharge will only be applied if a tempered glass lite of 6 mm thickness is fitted. If this surcharge shall be applied to other thicknesses, it has to be defined for them too.

*B-358*
*A+W Business Master data*

## The Exchange Surcharge Dialog

Dialog Exchange surcharges offers the tabs General, by thickness, and by product which can be selected when entering an exchange surcharge. This allocation cannot be changed afterwards.

*A screen capture of the 'Exchange Surcharges' dialog, showing the different tabs and fields for defining a surcharge.*

**A** Tab for the surcharge type and for surcharge allocation
**B** Table number of the surcharge
**C** Product type
**D** Lite to be fitted.
**E** Lite to be replaced
**F** Definition of the (graduated) surcharge
**G** List of exchange tables for the selected rate

*Fig. B-183: The exchange surcharge dialog*

Each surcharge table is allocated to a rate (price list, key). The validity of the exchange surcharge can be limited to products, customers, or suppliers. The allocation to a customer or supplier price cannot be changed afterwards. The surcharge can be graduated, e. g. by edge length or thickness.

You can also refer to a Miscellaneous surcharge, e. g. if the edges exceed a certain size.

*A+W Business Master data*
*B-359*

## Surcharges

## Defining an Exchange Surcharge

Exchange surcharges are defined for glass that shall be fitted into an IG unit instead of the original glass, and which cannot or shall not be collected in price groups. In this example, a general exchange surcharge is defined for the product type IG.

> **Allocating a partner or changing the allocation**
> Surcharges are defined as general surcharges by default so that they are valid for all partners. When an exchange surcharge is entered, it can be allocated to a certain partner or group of partners.
> The allocation can be changed only in menu Functions > Change prices.

There are the following instructions on this subject.
- "How to define an independent exchange surcharge" on page B-360
- "How to define a thickness-related exchange surcharge" on page B-363

### How to define an independent exchange surcharge

1.  Go to menu Master data > Prices > Exchange surcharges.
    Dialog Exchange prices appears.
2.  Go to menu Edit > New.

*A screen capture of the 'Define surch. type' selection dialog.*

*Fig. B-184: Surcharge type selection*

3.  Select the option Independent surcharge and click on [OK].
    The fields on tab General are accessible in dialog Exchange surcharges.

*B-360*
*A+W Business Master data*

## Surcharges

*A screen capture of the 'Exchange Surcharges | Standard' dialog, with the 'General' tab active and fields accessible for defining an independent surcharge.*

**A** Table number for the exchange surcharge
**B** Rate
**C** Select the product type
**D** Choose the product to be replaced.
**E** Fields for graduation of the exchange surcharge
**F** Choose the calculation type
**G** Choose the limit type

*Fig. B-185: Fields for independent exchange surcharge are accessible*

⇨ Software Reference, "Exchange Surcharges" on page B-729

4.  Enter the table number (A) for the surcharge.
    Exchange surcharges are usually entered in table 0. You have to enter another number only if you want to define different exchange surcharges.
5.  Select the rate (B).
    You should choose the rate in which the standard prices for IG products are defined so that the surcharge is applied to the standard prices. If the surcharge shall be applied to another rate as well you can use the copy function to transfer it.
    ⇨ "Copying and Changing Replacement Surcharges" on page B-365
6.  Check one of the options for the product type (C).
    In this example, IG is checked. You can e. g. replace the spacer too.
7.  Enter the product number (D) of the glass to be fitted.
    In this example, this is Float 6 mm. This means that the surcharge will be applied only if a Float 6 mm lite is fitted. For other glass types, no exchange surcharge will be applied.
8.  Select the Limit type (G).

*A+W Business Master data*
*B-361*

## Surcharges

In this example, this is Width x Height. The fields in section Exchange prices (E) depend on this setting.
9.  Enter the height, the width, and the surcharge (E).
    In this example, no surcharge shall be applied to 1200 x 1800 mm. For 2400 x 3600 mm, the surcharge shall be 2.00 and above that size, 5.00.
10. Enter the type (F), e. g. Gross %.
    Based on these settings, a surcharge of 2.00 or resp. 5.00 per cent shall be applied to the gross price of the lite to be added to the unit.

*A screen capture showing an example of a completed independent exchange surcharge with graduated values.*

*Fig. B-186: Example of an independent exchange surcharge*

All necessary entries have been made. The other fields can be filled in later.
11. Select in the menu Start > Save to save the data.
    The data will be saved. You can view the exchange surcharges defined for the selected price list and key on tab Table.

> **Miscellaneous surcharges**
> You can assign an additional surcharge to be added to the exchange surcharge, e.g. if the edges are overlong. These surcharge type will be introduced in a separate session.
>
> ⇨ "Miscellaneous Surcharges" on page B-374

*B-362*
*A+W Business Master data*

## Surcharges

### How to define a thickness-related exchange surcharge

1.  Go to menu Master data > Prices > Exchange surcharges.
    Dialog Exchange prices appears.
    ⇨ Software Reference, "Exchange Surcharges" on page B-729
2.  Go to menu Start > New to switch to the input mode.
    Dialog Select pops up.
3.  Choose the option Thickness-related surcharge and click on [OK].
    The fields on tab by thickness are accessible in dialog Exchange surcharges.

*A screen capture of the 'by Thickness' tab in the 'Exchange Surcharges' dialog.*

**A** Product type
**B** Product to be fitted
**C** Thickness of the product to be replaced

*Fig. B-187: Thickness-related exchange surcharge*

4.  Enter the table number and the rate.
5.  Check the option for the product type (A).
6.  Enter the number (B) of the product to be fitted, e. g. cast resin.
7.  Enter the thickness (C) of the product to be replaced, e. g. 8.
    With that you have defined that the surcharge shall be applied whenever a glass of 8 mm thickness is replaced by cast resin.

*A+W Business Master data*
*B-363*

## Surcharges

*A screen capture showing the fields for defining a thickness-related exchange surcharge.*

**A** Minimum surface
**B** Surcharge type
**C** Limit type
**D** Surcharge graduation

*Fig. B-188: Values for the thickness-related exchange surcharge*

8.  Define the limit type (C).
9.  Enter the values for the graduation (D), the surcharge type (B), and the minimum surface (A).
10. Select in the menu Start > Save to save the data.
    The data will be saved.
11. Repeat steps 2 to 10 to specify another exchange surcharge for another thickness.
    The fields will be preset by the data you have just entered.

*B-364*
*A+W Business Master data*

## Surcharges

## Copying and Changing Replacement Surcharges

Exchange surcharges can be copied from one rate to another. This function is the same as the function for copying prices.

The copy function offers the following options:
-   Copy the surcharges for a certain glass to be replaced or changed in to a new table.
-   Copy the surcharges for a certain glass to be replaced or exchanged from one rate to another.
-   Copy the surcharges for a certain glass to be replaced of exchanged for a partner or a group of partners.
-   Copy the surcharges for an exchange lite, at the same time entering them for another exchange glass.
-   Change the exchange glass in all surcharges for a certain glass type.
-   Copy the surcharges for a lite to be replaced, at the same time entering them for another glass to be replaced.
-   Change the glass to be replaced in all surcharges for a certain glass.

In the following session, all exchange surcharges for a certain product shall be copied to another.

**Examples**
-   Copy the surcharges for the exchange glass Float 4 and choose the target product Float 5. The surcharges for Float 5 will be copied to the same table, i. e. they are defined there. These surcharges can be changed now as required.
-   Copy the surcharges for the product combination Float 5/TG 3010 to a new table, e. g. number 3003. Now change surcharges for customer 3003. Allocate this table to customer 3003.

*A+W Business Master data*
*B-365*

## Surcharges

### How to define new exchange surcharges by copying

1.  Go to menu Master data > Prices > Exchange surcharges.
    Dialog Exchange prices appears.
2.  Go to menu Functions > Copy group > General.
    ⇨ Software Reference, "Copy Exchange Prices" on page B-736
    In this example, the surcharges for an exchange glass are copied. The steps are the same for lites to be replaced if you choose the command per complete exchange article.

*A screen capture of the 'Copy exchange prices in general' dialog.*

**A** Table number for the exchange surcharge (source)
**B** Product number of the exchange glass
**C** Rate
**D** Table number of the target
**E** Product number of the glass to which the data shall be transferred.

*Fig. B-189: Fields for copying are accessible*

3.  Enter the table number (A) for the surcharges to be copied.
4.  Select the rate (price list, key) from which the surcharges shall be copied.
5.  Enter the product number of the new glass (B), e.g. 1005.
6.  In section Copy to, enter the product number (E) to which the exchange surcharge shall be copied, e. g. 1008.
7.  Select the same rate in section Copy to.
8.  Click on [OK] to start copying.

*B-366*
*A+W Business Master data*

## Surcharges

*A screen capture showing the 'Copy exchange prices in general' dialog with source and target data filled in for copying a surcharge.*

*Fig. B-190: Settings for copying an exchange surcharge*

All exchange surcharges for product 1005 are copied for the exchange glass 1008 to the same table. A message will tell you how many records have been created.

*A screen capture of the 'Exchange Surcharges' dialog showing the newly copied exchange surcharges in the list.*

*Fig. B-191: Exchange surcharges copied*

The copied exchange surcharges appear on the list.

*A+W Business Master data*
*B-367*

## Surcharges

### Exercises

-   Enter an exchange surcharge for replacing a lite of your IG product.
-   Enter another exchange surcharge for your training customer. This exchange surcharge shall be applied if the customer orders a wider spacer.

### Additional information

⇨ Software Reference, "Exchange Surcharges" on page B-729

*B-368*
*A+W Business Master data*

## Shape Processing Surcharges

**Objectives**
- Introducing processing surcharges for shapes.
- Defining a shape processing surcharge.

**Benefit**
- The processing of shapes means additional work which usually has to be performed by hand. This additional work will be charged by means of a surcharge.

**Note**

| Term | Description |
| :--- | :--- |
| **Processing surcharge** | For the additional work in connection with the processing of shapes, a surcharge is defined which is based on the processing step and on the shape. |
| **Surcharge type** | The rules for proportional surcharges are: <br> - Gross price = before deduction of discounts <br> - Net price = after deducting the discounts |

*A+W Business Master data*
*B-369*

## Surcharges

### Function of Shape Surcharges for Processing Steps

For the additional work in connection with the processing of non-rectangular lites (shapes), a surcharge is defined which is applied to the original processing price.

This surcharge can be calculated based on the following surcharge types:
-   Edge length, e. g. for edgework
-   Surface, e. g. for screen printing, enamel
-   Piece, e. g. for corners, drill holes

*A screen capture of the 'Shape Surcharges' dialog, showing a list of processing surcharges and a sketch of a shape with numbered edges and corners.*

**A** Prices for shapes (glass of different product groups)
**B** Surcharge for processing the segments of a shape
**C** Shape number

*Fig. B-192: Processing surcharges for shapes*

In this example, calculation is based on the gross price of the processing (A).
The surcharge always applies to a certain shape (C) from the shape catalog. Since the surcharge is applied to the individual segments (B) of a shape, different surcharges can be entered per segment. Depending on the selected processing, the values in the segment fields refer to the corner or to the edges.
This example shows that the processing of edges 1 and 4 (red numbers outside the sketch) will incur no additional work. Edges 2 and 3 can only be processed manually. The numbers of the corners are green (inside the sketch).

### Defining a Shape Processing Surcharge

Shape processing surcharges are applied to non-rectangular lites. This surcharge is applied to the processing price.

*B-370*
*A+W Business Master data*

## Surcharges

### How to enter a processing surcharge for shapes

1.  Go to menu Master data > Prices > Shape surcharges.
    Dialog Shape processing surcharges appears.
    ⇨ Software Reference, "Shape Processing Surcharges" on page B-757
2.  Go to the menu Start > New to switch to the input mode.

*A screen capture of the 'Shape Surcharges' dialog in input mode.*

**A** Select the price table (processing)
**B** Rate
**C** Price or surcharge type
**D** Enter the shape number

*Fig. B-193: Fields for the new shape processing surcharge are accessible*

3.  Select the price table (A) for the processing to which a shape surcharge shall be applied.
4.  Select the rate (price list, key) (B).
    These surcharges must be entered in the same rate in which the processing prices have been entered. If you have got several rates for processing, you have to define the shape surcharge for every rate.
5.  Select the price type (C).
    Selection of the price type (surcharge type) is restricted to a proportional increase (Gross %), to the edge length (lin.m), and to the quantity (pcs.).
6.  Enter the shape number (D) and proceed by pressing the `<Tab>` key.
    The shape data are imported. The segment numbers of the edges and/or corners to be processed are marked on the shape sketch. The corresponding fields will be released.

*A+W Business Master data*
*B-371*

## Surcharges

*A screen capture of the 'Shape Surcharges' dialog with segment fields accessible after selecting a shape.*

**A** Minimum values for price and quantity
**B** Segment fields
**C** Numbering of edges and corners

*Fig. B-194: Segment fields per edge/corner accessible*

7.  Enter the surcharge for the individual segments (B).
    Edgework defined in the order refers to the edges. If rounded corners are entered, the corresponding values apply to the corners.
8.  Enter a minimum price and/or a minimum quantity (A).
    These are mandatory fields which must be filled in.
    If you do not want to define minimum values, enter 1 in both fields. This price and quantity will always be reached. Both values can be amended later.
9.  Select in the menu Start > Save to save the data.
    The data will be saved. The new surcharge appears on the list.

*B-372*
*A+W Business Master data*

## Surcharges

### Exercises

-   Decide which shape processing results in additional work:
    -   Drill holes?
    -   Coating?
    -   Edgework?
    -   Corner processing?
-   Enter a processing surcharge for the following shapes:
    -   Trapezium (5)
    -   Triangle (20)
    -   Hexagon (22)
    The shape numbers are shown in brackets. Define the segments which cause additional work in connection with certain processing steps. How does this affect the surcharge (amount)?

### Additional information

⇨ Software Reference, "Shape Processing Surcharges" on page B-757

*A+W Business Master data*
*B-373*

## Miscellaneous Surcharges

**Objectives**
- Introducing the function of the so-called miscellaneous surcharges.
- Introducing surcharge types and how they are calculated.
- Defining a miscellaneous surcharge.

**Benefit**
- Miscellaneous surcharges can be applied in addition to other surcharges. They refer either to a product or will be applied in general.
- Energy surcharge-, transport/toll-, spacer-, small/oversize-, minimum quantity-, thickness surcharges are defined as miscellaneous surcharges.

**Note**

| Term | Description |
| :--- | :--- |
| **Surcharge type** | The surcharge type defines how the surcharge is going to be calculated. |
| **Graduation** | The graduation of a miscellaneous surcharge is analysed in the sequence which appears in the dialog. A new limit will always be added at the end of the list even if it has been defined with smaller limits. |
| **Reference** | Miscellaneous surcharges always refer to the basic price. They can be transferred within a BOM. |
| **Surcharge type rules** | Apart from referring to the basic item, proportional values can be used. The rule is: <br> - Gross price = before deduction of discounts <br> - Net price = after deducting the discounts |
| **Other surcharges for BOM elements** | The calculation of other surcharges by surcharge type can be switched off in general in company data for BOM elements for which such a surcharge has been defined in product master data. |
| **Display in the order** | Other surcharges are implicit only, i.e. they do not appear on the order. |

*B-374*
*A+W Business Master data*

## The Function of Miscellaneous Surcharges

These surcharges are defined to be able to handle special cases, e. g. oversizes or especially small sizes. These surcharges are always applied to the standard price. They are always implicit, i.e. they are not stated in the order.

*A screen capture showing a list of miscellaneous surcharges.*

*Fig. B-195: Examples of miscellaneous surcharges*

Miscellaneous surcharges can be allocated in the following dialogs:
-   **Product management > tab Price/surcharge:**
    The surcharge will always be applied even if other prices are used for calculation.
-   **Prices > tab Price selection:**
    The surcharge will be applied only if this price is selected.
-   **Group surcharges:**
    The surcharge will be applied whenever a price is determined by means of the price group, with a group surcharge.
-   **Exchange surcharges > tab General, by thickness, by product:**
    The surcharge will be applied whenever an exchange surcharge is calculated.
-   **Customer-, supplier discounts > tab Differences:**
    The surcharge will be applied if different discounts have been agreed with the partner.

> **Miscellaneous surcharges will be applied twice**
> If A+W Business detects a miscellaneous surcharge both for the price and for the product, both will be applied.

*A+W Business Master data*
*B-375*

## Dialog Miscellaneous Surcharges

You can display a list of miscellaneous surcharges in dialog Miscellaneous surcharges.

*A screen capture of the 'Miscellaneous Surcharges' dialog, showing a table of graded allowances.*

**A** Surcharge table number
**B** Graded allowance
**C** Limit (1, 2)
**D** Limit type (1, 2)
**E** Take one or both limits into account
**F** Surcharge amount
**G** Unit to which the surcharge refers
**H** Surcharge type
**I** Validity in connection with manual price changes

*Fig. B-196: Dialog Miscellaneous surcharges*

If you are using two different limit types for graduation you have to define whether these shall be analysed together or alternatively (E):
-   If you check the checkbox, the surcharge will be applied to the limit that has been reached in the order. This can be limit 1 or limit 2.
-   If this checkbox is not checked, the surcharge will be applied only if both limits are reached.

Unlike shape-, grill- or exchange surcharges, miscellaneous surcharges will only be taken into account in case of manual price changes if they have been explicitly released (I).

*B-376*
*A+W Business Master data*

### Exmaple 1: Spacer surcharge

| up to limit 1 (mm) | Limit type 1 | or | up to limit 2 | Limit type 2 | Surcharge | Price unit |
| :--- | :--- | :- | :--- | :--- | :--- | :--- |
| 12 | AIR | | | | 0.00 | Net % |
| 16 | AIR | | | | 5.00 | Net % |
| 20 | AIR | | | | 10.00 | Net % |

Example 1 shows a simple graduation with one limit type which is applied to the spacer.
The following example shows one surcharge with two limit types.

### Example 2: Edge length surcharges

| up to limit 1 (mm) | Limit type 1 | or | up to limit 2 (mm) | Limit type 2 | Surcharge | Price unit |
| :--- | :--- | :- | :--- | :--- | :--- | :--- |
| 2000 | Width | | 2000 | Height | 0.00 | Net % |
| 9999 | Width | | 9999 | Height | 20.00 | Net % |
| 2000 | Width | ✔ | 3500 | Height | 0.00 | Basic item (n. add.) |
| 9999 | Width | ✔ | 9999 | Height | 20.00 | Basic item (n. add.) |

Example 2 shows two different surcharges for the edge length.
The first edge length surcharge is e. g. applied whenever the lite exceeds a certain size and cannot be handled by one person alone.
The OR connection in the second example means that the surcharge will be applied if either the defined width or the defined height is exceeded. The limit types can be exchanged in this case.

### Example 3: Thickness surcharge

| up to limit | Limit type | Surcharge | Unit | Surcharge type |
| :--- | :--- | :--- | :--- | :--- |
| 10 | Thickness | 0.00 | Gross % | Basic price (n. add.) |
| 9999 | Thickness | 35.00 | Gross % | Basic price (n. add.) |

In example 3, a surcharge is applied to the lite thickness which can be used e. g. for drilling. If the lite thickness is 10 mm or lower, no surcharge will be applied. A surcharge of 35.00 €/sqm will be applied to all thicker lites.

### Example 4: Small quantity surcharge

| up to limit | Limit type | Surcharge | Unit | Surcharge type |
| :--- | :--- | :--- | :--- | :--- |
| 0.1 | sqm | 100.00 | Gross % | Basic price |
| 0.15 | sqm | 50.00 | Gross % | Basic price |
| 0.5 | sqm | 30.00 | Gross % | Basic price |

*A+W Business Master data*
*B-377*

## Surcharges

Example 4 shows a graduated surcharge for lites smaller than 0.5 sqm. In a first step, a surcharge of 100 % will be applied if the lite surface is below 0.1 sqm. This surcharge is reduced in the next two steps to 50 % and 30 % for a surface of up to 0.15 sqm or up to 0.5 sqm respectively. No surcharge will be applied to lites larger than that.

The surcharge type defines how the surcharge is going to be calculated. Surcharge types and the calculation are described in detail - including examples - in the following chapters.
-   "Surcharge Types" on page B-378
-   "Calculation by surcharge type" on page B-380
-   "Calculating surcharges for processing" on page B-386
-   "Transfer of surcharge types" on page B-386

### Surcharge Types

Surcharge types define the basis on which the corresponding surcharge shall be calculated:
-   **Basic item:**
    For the top element (product) on the BOM to which a surcharge can be allocated as well
-   **Basic item + processing:**
    For the top element on the BOM and all corresponding processing steps.
-   **all previous processing steps:**
    For all processing steps executed before the selected BOM element.
-   **all previous items:**
    For all elements listed in the BOM before the selected element.
-   **Basic item + shape:**
    For the top element on the BOM and the corresponding shape.
-   **Basic price:**
    For the price of the top element of the BOM.
-   **previous processing:**
    All processing steps listed before the element for which the surcharge has been defined.
-   **Parent + its lites:**
    For the top element of an assembly (parent) and the lites of this assembly.
-   **Parent + its previous processing:**
    For the top element of an assembly (parent) and the processing attached to this element.
-   **previous BOM with same parent:**
    All elements of the assembly.
-   **Curr. processing:**
    For the selected BOM element only.

*B-378*
*A+W Business Master data*

## Surcharges

-   **Basic item without other surcharges:**
    For the top element on the BOM without the surcharge that may be allocated to the product.
-   **Complete item:**
    The surcharge is applied to the whole order item.

All surcharge types can be defined as additional or non-additional. The additional or non-additional calculation only refers to proportional surcharges however.
In case of non-additional calculation, the previous surcharge will not be taken into account for calculating the next surcharge.
In both cases, the resulting value serves as the basis for calculating the proportional surcharge.

**Example**

| | Basic price 100.00 € |
| :--- | :--- |
| | **additional** | **non-additional** |
| Shape surcharge + 20% | + 20.00 € | + 20.00 € |
| Subtotal | = 120.00 € | |
| Coating + 25% | + 30.00 € | + 25.00 € |
| **Total** | **= 150.00 €** | **= 145.00 €** |

*A+W Business Master data*
*B-379*

## Surcharges

### Calculation by surcharge type

The surcharge type is chosen in dialog Miscellaneous surcharges by means of the Surcharge type. The gross price is the price prior to deduction of discounts while the net price is the price after deduction of discounts.

The following examples show eight versions of calculating surcharges.

> **Fictitious prices**
> The prices in the examples are fictitious. They have been chosen to make the calculation examples easier to understand.

### Example 1: Basic price

Gross or net surcharge on the price of the main item

**Basic price - net surcharge**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 0.5 sqm | 50.00 | 25.00 | 50% | 25.00 |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 0.5 sqm | 50.00 | | 0% | 50.00 |
| Shape | Basic price (n.add.) Net % surcharge | | 100% | 25.00 | 100% of 25.00 | 0% | 25.00 |
| **Total** | | | | | | | **100.00** |

*Tab. B-4: Surcharge type Basic net price*

*B-380*
*A+W Business Master data*

## Surcharges

### Example 2: Basic item

Gross or net surcharge on the price of the main item including exchange surcharges

**Basic price - gross surcharge**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 0.5 sqm | 50.00 | 50.00 | 50% | 25.00 |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 0.5 sqm | 50.00 | 50.00 | 0% | 50.00 |
| Shape | Basic item (n.add.) Gross % surcharge | | 100% | 100.00 | 100% of 100.00 | 0% | 100.00 |
| **Total** | | | | | | | **175.00** |

*Tab. B-5: Surcharge type Basic gross price*

**Basic price - gross surcharge**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 0.5 sqm | 50.00 | 25.00 | 50% | 25.00 |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 0.5 sqm | 50.00 | 50.00 | 0% | 50.00 |
| Shape | Basic item (n.add.) Net % surcharge | | 100% | 75.00 | 100% of 75.00 | 0% | 75.00 |
| **Total** | | | | | | | **150.00** |

*Tab. B-6: Surcharge type Basic net price*

*A+W Business Master data*
*B-381*

## Surcharges

### Example 3: Basic item + processing

Shape surcharge on the basic item and all processing steps with surcharge type Basic item (additional).

**Basic item + processing**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 2 sqm | 200.00 | 100.00 | 50% | 100.00 |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 2 sqm | 200.00 | 200.00 | 0% | 200.00 |
| UV edge connection | Basic item | (add.) 1 lin.m at 4.00 | 6 lin.m. | 24.00 | 12.00 | 50% | 12.00 |
| Shape | Basic item + process. | Net % surcharge | 100% | 312.00 | 100% of 312.00 | 0% | 312.00 |
| **Total** | | | | | | | **624.00** |

*Tab. B-7: Surcharge type Basic item + Processing (added)*

**Basic item + processing**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 2 sqm | 200.00 | 100.00 | 50% | 100.00 |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 2 sqm | 200.00 | 200.00 | 0% | 200.00 |
| UV edge connection | Basic item | (n.add.) 1 lin.m at 4.00 | 6 lin.m. | 24.00 | 12.00 | 50% | 12.00 |
| Shape | Basic item + process. | Net % surcharge | 100% | 300.00 | 100% of 300.00 | 0% | 300.00 |
| **Total** | | | | | | | **612.00** |

*Tab. B-8: Surcharge type basic item + processing (not additional)*

*B-382*
*A+W Business Master data*

## Surcharges

### Example 4: Basic item + shape

If the surcharge Inside pattern shall be applied to the basic item and the shape, you have to chose an additional surcharge type for the shape.

**Basic item + shape - net surcharge**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 0.5 sqm | 50.00 | 25.00 | 50% | 25.00 |
| 1st lite = Float | | | | | | | |
| 2nd lite = patterned | | Exchange surcharge 1 sqm at 50.00 | 0.5 sqm | 25.00 | 25.00 | 0% | 25.00 |
| Grill | | 1 pc. at 50.00 | 1 pcs. | 50.00 | | 10% | 45.00 |
| Shape | Basic item + process. | (add.) Net % surcharge | 100% | 50.00 | 100% of 50.00 | 0% | 50.00 |
| Pattern inside | Basic item + shape | Net % surcharge | 10% | 10.00 | 100% of 100.00 | 0% | 10.00 |
| **Total** | | | | | | | **155.00** |

*Tab. B-9: Surcharge type Basic item + Shape*

### Example 5: Previous processing

Oversize surcharge for edgework, the input sequence is important. The surcharge will be applied only to the previous processing step.

**Previous processing**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Single annealed | | 1 sqm at 100.00 | 4 sqm | 400.00 | | 50% | 200.00 |
| Edgework | Basic item | (add.) 1 lin.m at 15.00 | 8 lin.m. | 120.00 | 120.00 | 5% | 114.00 |
| Oversize surcharge | Previous processing | (add.) Gross % surcharge | 10% | 12.00 | 10% of 120.00 | 0% | 12.00 |
| **Total** | | | | | | | **326.00** |

*Tab. B-10: Surcharge type Previous processing*

*A+W Business Master data*
*B-383*

## Surcharges

### Example 6: All previous items

Surcharge type in connection with work performed, e.g. surcharge Surcharge. Surcharge type in connection with work performed, e.g. surcharge Surcharge.

**All previous items - surcharge**

| Item/ product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 001/ IG | | 1 sqm at 100.00 | 0.5 sqm | 50.00 | 40.00 | 20% | 40.00 |
| 002/ TG | | 1 sqm at 90.00 | 1.2 sqm | 108.00 | 86.40 | 20% | 86.40 |
| 003/ LG | | 1 sqm at 80.00 | 2 sqm | 160.00 | 160.00 | 0% | 160.00 |
| 004/single annealed | | 1 sqm at 50.00 | 1.4 sqm | 70.00 | 42.00 | 40% | 42.00 |
| 005/ Surcharge | All previous items | (add.) Net % surcharge | 20% | 328.40 | 20% of 328.40 | 0% | 65.68 |
| **Total** | | | | | | | **394.08** |

*Tab. B-11: Surcharge type All previous items – surcharge*

If the surcharge is entered with a negative sign, it will be applied as a discount, e.g. special discount. If the surcharge is entered with a negative sign, it will be applied as a discount, e.g. special discount.

*B-384*
*A+W Business Master data*

## Surcharges

**All previous items - special discount**

| Item/ product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 001/ IG | | 1 sqm at 100.00 | 0.5 sqm | 50.00 | 40.00 | 20% | 40.00 |
| 002/ TG | | 1 sqm at 90.00 | 1.2 sqm | 108.00 | 86.40 | 20% | 86.40 |
| 003/ LG | | 1 sqm at 80.00 | 2 sqm | 160.00 | 160.00 | 0% | 160.00 |
| 004/single annealed | | 1 sqm at 50.00 | 1.4 sqm | 70.00 | 42.00 | 40% | 42.00 |
| 005/ Special discount | All previous items | (add.) Net % surcharge | -20% | 328.40 | 20% of 328.40 | 0% | -65.68 |
| **Total** | | | | | | | **262.72** |

*Tab. B-12: Surcharge type all previous items - Special discount*

### Example 7: Additional calculation

The surcharges for edgework and hole drilling are additional ones: Basis for calculating the proportional surcharge (shape) is the basic price plus the surcharges for edgework and drilling.

**Additional calculation**

| Item/ product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Single annealed | | 1 sqm at 100.00 | 1 sqm | 100.00 | 80.00 | 20% | 80.00 |
| Edgework | Basic item | (add.) 1 lin.m at 5.00 | 4 lin.m. | 20.00 | 20.00 | 0% | 20.00 |
| Drill hole | Basic item | (add.) 1 pc. at 30.00 | 1 pcs. | 30.00 | 30.00 | 0% | 30.00 |
| Shape | Basic item + process. | (n.add.) Net % surcharge | 50% | 65.00 | 50% of 130.00 | 0% | 65.00 |
| **Total** | | | | | | | **195.00** |

*Tab. B-13: Surcharge; additional calculation*

### Example 8: Non-additional calculation

The surcharges for edgework and hole drilling are non-additional ones: Basis for calculating the proportional surcharge (shape) is the basic item without edgework and drilling.

*A+W Business Master data*
*B-385*

## Surcharges

**Non-additional calculation**

| Product | Surcharge type | Price/price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Single annealed | | 1 sqm at 100.00 | 1 sqm | 100.00 | 80.00 | 20% | 80.00 |
| Shape | Basic item + process. | (n.add.) Net % surcharge | 50% | 50.00 | 50% of 80.00 | 0% | 40.00 |
| Edgework | Basic item | (n.add.) 1 lin.m at 5.00 | 4 lin.m. | 20.00 | | 0% | 20.00 |
| Drill hole | Basic item | (n.add.) 1 pc. at 30.00 | 1 pcs. | 30.00 | | 0% | 30.00 |
| **Total** | | | | | | | **170.00** |

*Tab. B-14: Surcharge; non-additional calculation*

If no length surcharge has been defined for a limit, all lites up to this limit will be calculated without a surcharge. Likewise, all airspaces up to 12 mm are calculated without a surcharge in example Limits for miscellaneous surcharges.

### Calculating surcharges for processing

**Calculation of additional surcharges:**

| | | |
| :--- | :--- | :--- |
| Edgework | 4 lin.m x 6.25 € | 25.00 € |
| Misc. surcharge Processing index 1 | 50% net on 25.00 € | 12.50 € |
| Misc. surcharge Thickness 9 mm | 10% net on 37.50 € | 3.75 € |
| **Total price of the processing** | | **41.25 €** |

**Calculation of non-additional surcharges:**

| | | |
| :--- | :--- | :--- |
| Edgework | 4 lin.m x 6.25 € | 25.00 € |
| Misc. surcharge Processing index 1 | 50% net on 25.00 € | 12.50 € |
| Misc. surcharge Thickness 9 mm | 10% net on 25.00 € | 2.50 € |
| **Total price of the processing** | | **40.00 €** |

### Transfer of surcharge types

Depending on the surcharge type chosen, the surcharge is calculated for the BOM elements:

*B-386*
*A+W Business Master data*

## Surcharges

*A diagram showing how different 'Surcharge type applies to' options (Parent + glass, Previous BOM same parent, Parent + previous processing, Previous processing) relate to different elements within a Bill of Materials (BOM) for an LG (laminated glass) parent item.*

*Fig. B-197: Transfer of surcharge type in the BOM*

The surcharge for processing 2 is applied to the laminated lite and the two single annealed lites for example if the surcharge type Parent + glass has been chosen. The surcharge for processing 2 is applied to the laminated lite and the single annealed lites if the surcharge type Parent + glass has been selected.

### Defining a Miscellaneous Surcharge

Two limit types can be taken into account per record; the limit types can change from record to record.

> **Calculation of miscellaneous surcharges**
> Pricing of orders takes into account the sequence in which the discount levels are defined. This sequence can influence the calculation considerably. If e.g. the unit surcharge appears last instead of first, the resulting sqm prices will differ.

**Example: 100 pcs. at 0.1 sqm / sqm at 100.00 (Euro)**

| Sequence | Amount | Sequence | Amount |
| :--- | :--- | :--- | :--- |
| Basic amount | 100.00 € | Basic amount | 100.00 € |
| Unit surcharge | + 35.00 € | Surface surcharge 100% | + 100.00 € |
| Total | 135.00 € | Total | 200.00 € |
| Surface surcharge 100% | + 135.00 € | Unit surcharge | + 35.00 € |
| **sqm price for calculation** | **270.00 €** | **sqm price for calculation** | **235.00 €** |

Therefore, please make sure to define new surcharge levels so that pricing meets your requirements.
To enter several steps for a surcharge you should first define the correct sequence on a piece of paper.

*A+W Business Master data*
*B-387*

## Surcharges

There are the following instructions on this subject.
- "How to define a new surcharge" on page B-389
- "How to enter more steps for grading the surcharge" on page B-391
- "How to delete a step of the graduation" on page B-392

*B-388*
*A+W Business Master data*

## Surcharges

### How to define a new surcharge

1.  Go to menu Master data > Prices > Misc. surcharges.

*A screen capture of the 'Misc. Surcharges' dialog, showing a previously defined surcharge.*

*Fig. B-198: View of a comparable surcharge*

⇨ Software Reference, "Miscellaneous Surcharges" on page B-728

If surcharges have been entered already, the values of the first surcharge (from tab Table) are shown. You can use the arrow keys to search for a surcharge that meets your expectations.
If no surcharges have been defined yet you have to fill in all fields by hand.

2.  Go to the menu Start > New to switch to the input mode.

*A screen capture showing the fields for a new surcharge being accessible.*

**A** (Table) number of the surcharge
**B** Name

*Fig. B-199: Release the fields for a new surcharge*

The fields are preset with the entries of the selected surcharge.
3.  Enter the number (A) and the name (B) of the new surcharge.

*A+W Business Master data*
*B-389*

## Surcharges

To do so, change the entries in the two fields if these are preset.

*A screen capture of the 'Misc. Surcharges' dialog with dropdowns and fields active for editing.*

**A** First value of limit type 1
**B** Limit type 1
**C** Surcharge amount
**D** Calculation unit
**E** Surcharge type
**F** Application of manual prices

*Fig. B-200: Amend preset values*

4.  Position the cursor on the first field (A) of the list and change the entry.
5.  Press the `<Tab>` key to proceed to the next field (B) and choose the limit type.
6.  Edit all fields for the first entry in this way.
7.  Check the checkbox Valid for price definition (F) if the surcharge shall also be applied if the price is changed manually.
8.  Select in the menu Start > Save to save the data.
    The data will be saved. You can now enter further steps for the graduation.

*B-390*
*A+W Business Master data*

## Surcharges

### How to enter more steps for grading the surcharge

1.  Select the surcharge you want to edit.
2.  Open the context menu by a right mouse click on the line header.

*A screen capture showing a right-click context menu on a surcharge line, with 'Insert' and 'Delete' options.*

**A** Table number of the surcharge
**B** Context menu

*Fig. B-201: Context menu for adding the next step of the graduation*

3.  Select the entry Insert (B).
    A new line is added at the end of the list. All fields except the first are preset by the entries from the previous line.

> **No sorting of entries**
> You cannot change the sequence of the surcharge levels. To put an entry before an existing one, you have to create all entries in the required sequence then delete the old ones.

*A screen capture showing a new line added to the surcharge list, ready for editing.*

*Fig. B-202: New line*

4.  Enter the new limit and amend the entries in the other fields if necessary.
5.  Enter the required surcharge levels, e.g. three levels for a surcharge for overlong edges.
6.  Select in the menu Start > Save to save the data.
    The data will be saved. To apply the surcharge automatically, allocate the table number to the product or the price. It can also be entered manually in the order.

*A+W Business Master data*
*B-391*

## Surcharges

### How to delete a step of the graduation

1.  Select the surcharge to be edited.
2.  Open the context menu by a right mouse click on the line header.
    The context menu appears.
3.  Select the entry Delete.

*A screen capture showing a line in the surcharge list marked for deletion with an 'X'.*

The line header is marked by an X.
4.  Go to menu Start > Save.
    A security query appears.
5.  Acknowledge the query by [Yes].
    The data will be deleted.

> **Deleting a table**
> If you select Start > Delete, the entire surcharge (the table) will be deleted.

*B-392*
*A+W Business Master data*

## Surcharges

### Exercises

-   Enter a simple surcharge for lites which shall be applied if the weight exceeds 30 kg.
-   Define a surcharge based on the edge length and the surface.
-   Enter at least two steps for the edge length surcharge.
-   Delete one of the graduations without deleting the whole table.

### Additional information

⇨ Tutorial 2, "Available limit types" on page B-593
⇨ Software Reference, "Miscellaneous Surcharges" on page B-728

*A+W Business Master data*
*B-393*

## Automatic Surcharges

**Objectives**
- Introducing the automatic surcharge/discount function.
- Enabling automatic surcharges in master data.
- Defining an automatic surcharge.

**Benefit**
- The so-called automatic surcharges are normally used for charging costs incurred e. g. through transport, waste disposal or similar things.
- These costs are defined as surcharges and entered in the document as a separate item, like any other product.

**Note**

| Term | Description |
| :--- | :--- |
| **Automatic surcharges** | Automatic surcharges are displayed in partner management, product management, and in the order in section Surcharges/discounts. They can be used as surcharges or special discounts. They will be automatically added to the documents only if they have been enabled in product and customer master data. Surcharges or special discounts are treated like products and are entered as separate order items. |
| **Product allocation** | An automatic surcharge is defined as a product with its own price table (unit price) and is allocated to one of the available surcharges/discounts. |
| **Surcharge or discount** | Based on the unit price, a surcharge or discount is applied. |
| **Application** | A+W Business adds the automatic surcharges as order items when the order is saved. |
| **Calculation in the document** | The automatic surcharge refers to a single order item or to the whole order. |
| **Position in document** | The item number in the document defines the point at which the automatic surcharge will be added. Based on the item number in the document and by means of the surcharge type selected at product definition, a discount/surcharge can be applied to another discount/surcharge. This means that a special discount can be applied to the entire order, including the automatic toll surcharge. |

### The Function of Automatic Surcharges

For every product and every customer you can define one or more automatic surcharges which will always be applied. These automatic surcharges can

*B-394*
*A+W Business Master data*

## Surcharges

e. g. be used as surcharges for transport-, toll fees, energy costs, or as special discounts. These surcharges can be defined for a customer or in general.

Surcharges or special discounts are treated like products and are entered as separate order items.

Surcharges/special discounts are defined acc. to the following rules:
-   They are entered as products.
-   They are always allocated to the product type and product group Services/surcharges.
-   Basically, they have their own price table.
-   They have to be allocated to the surcharges/special discounts in dialog Product allocation, surcharges.

Surcharges/special discounts can be allocated several times, either in general or for special customers only.

There are ten so-called special discounts available which can be applied as a discount (with a negative sign) or a surcharge (with a positive sign). This is e. g. useful for special promotions which are only valid for a certain time.

*A diagram illustrating the product allocation of surcharges/special discounts. It shows that a product (e.g., energy) with its own price table is allocated via 'Product allocation, surcharges'. This allocation can be enabled in Partner management or Product management, and is valid for a customer or in general.*

*Fig. B-203: Product allocation of surcharges/special discounts*

These surcharges are enabled in product or partner master data. Active surcharges/discounts are automatically entered as items in the document when the item entry dialog is closed. Automatic surcharges/discounts can be disabled in the order, or another one can be enabled.

*A+W Business Master data*
*B-395*

## Surcharges

*Two screen captures showing the 'Use surcharges/discounts' checklist in A) Product master data and B) Partner master data.*

*Fig. B-204: Automatic Surcharges*

The selection of surcharges/special discounts in partner product management (A) is limited. In partner management (B), all general discounts/surcharges are available. Customised discounts/surcharges will be shown for the customers in question.

### Product Surcharge Allocation

Automatic surcharges are entered in dialog Product surcharge allocation.

*A screen capture of the 'Surcharge allocation' window, showing a list of generally applicable automatic surcharges like 'Pattern inside', 'Edge stripping', 'Energy surcharge', etc.*

**A** Name of the surcharge
**B** Number and name of the allocated product
**C** Position in which the the surcharge is added in the document

*Fig. B-205: Product surcharge allocation*

This example shows a couple of generally applicable automatic surcharges. Each of these surcharges is based on a separate product (B), e. g. the product Inside pattern or Edge stripping.

The date 31.12.2099 indicates that this surcharge is valid indefinitely. Surcharges valid for a certain time only have an end date which appears in column Valid until. After the defined date, they will no longer be added or offered for selection.

*B-396*
*A+W Business Master data*

## Surcharges

By entering the item number (C) you can define the point at which the surcharge/discount shall appear in the document. Among other things, this item number determines the surcharge/discount calculation. 0 means that this surcharge shall be applied to an order item. The surcharge therefore has to be enabled in product management.

**Example**
If a surcharge/discount is entered with an item number of 900, it will appear at the end of the document. A surcharge/discount with item number 901 will be added as the next item.

If an energy surcharge is to be applied in general, it is enabled in product definition. As a surcharge, its item number is over 900, e. g. 970; it will be added as the last order item when the order is saved.

Through its position in the document and based on the Surcharge type chosen in product definition, a surcharge/discount can be applied to another surcharge/discount. This means that a special discount can be applied to the entire order, including the automatic toll surcharge.

⇨ "Surcharge Types" on page B-378

### Available Surcharges/Special Discounts

The following discounts/surcharges have been defined and can be edited:

| Surcharge/discount | Description |
| :--- | :--- |
| **Delivery fee** | This surcharge is calculated for delivery. It can be enabled in partner management. |
| **Down payment** | The down payment is entered as a down payment invoice, and is deducted from the order total. For further information, please refer to section Sales. ⇨ Sales, "Down payments" on page C-1395 |
| **Rush surcharge** | This surcharge will be applied if an order must be delivered sooner than is usual. It can be enabled in partner management. |
| **Energy surcharge** | The energy surcharge refers to the weight of the shipment. It can be enabled in product and partner management. In company data, it can be restricted to the glass weight. ⇨ Software Reference, "Company Data > Price Calculation" on page B-970 |
| **Rack 1, Rack 2** | Rack surcharges are applied in connection with rack management. It can be enabled in product and partner management. ⇨ Software Reference, "Company Data - Shipment" on page B-1017 |

*Tab. B-15: List of automatic surcharges (Section 1 of 2)*

*A+W Business Master data*
*B-397*

## Surcharges

| Surcharge/discount | Description |
| :--- | :--- |
| **Max. surface, Max. aspect ratio** | These surcharges are applied if the maximum surface and/or maximum aspect ratio is exceeded. They can be enabled in partner management. The values are checked against the sizes entered in product management. ⇨ Software Reference, "Price parameters" on page B-678 |
| **Shortfall** | This surcharge refers to the minimum quantity defined in product management. It can be enabled in partner management. ⇨ Software Reference, "Price parameters" on page B-678 |
| **Edge stripping** | This surcharge is automatically applied for edge stripping of coated lites. It always refers to an item. It can be enabled in partner management. |
| **Invoicing** | This surcharge is applied when the invoice is issued. It can be enabled in partner management. |
| **IG recycling** | This surcharge applied for the disposal of IG. It can be enabled in partner management. |
| **Special discount 1 - 10** | Special discounts can be defined individually. With a positive sign, they are applied as a surcharge and with a negative sign, as a discount. They can be enabled in product and partner management. |
| **Pattern inside** | This surcharge will be calculated for the fitting of a patterned lite with the patterned side facing inwards if, usually, this side is facing outwards. It can be enabled in partner management. |
| **IG transport** | This surcharge is calculated for the transport insurance of IG units. It can be enabled in partner management. |

*Tab. B-15: List of automatic surcharges (Section 2 of 2)*

All other surcharges which are not automatically applied based on product and partner master data, have to be entered by hand in the document.

### Defining an automatic surcharge

An automatic surcharge is defined in the following sequence:
-   Enter a product in product management (surcharge product):
    -   Go to tab Product and choose the entry Services/surcharges as Product type and Product group.
    -   On tab Production, enter the quantity unit and whether the discount/surcharge shall be printed on the BOM.
    -   On tab Price/surcharge, enter the corresponding Surcharge type, e.g. Basic item.

*B-398*
*A+W Business Master data*

## Surcharges

-   These steps are described in detail in chapter Product.
    ⇨ "Product Definition" on page B-245
-   Enter a unit price for this product in price management.
    A negative entry for the automatic surcharge will result in a reduction of the price. It is applied as a discount.
    ⇨ "Input of Unit Prices" on page B-301
-   In dialog Product surcharge allocation allocate the product to the corresponding automatic surcharge.
-   In customer master data, go to tab Order, section Apply surcharges/discounts and tick the checkbox for surcharges which shall always be applied to this customer.
    ⇨ Software Reference, "Surcharges/discounts" on page B-817
-   In product master data, go to tab Price/surcharges, section Apply surcharges/discounts and check the checkbox for the surcharges which shall always be applied to this product.
    ⇨ Software Reference, "Apply surcharges/discounts" on page B-678

The following guideline shows how to enter a special discounts for a customer. The product Special discount training and the corresponding price table have been created for this purpose.

> **Using automatic surcharges as discounts**
> You can use automatic surcharges as (special) discounts by entering a negative amount. This is why we will be talking about discount/surcharge in the following description.

*A+W Business Master data*
*B-399*

## Surcharges

### How to define an automatic surcharge for a customer

1.  Go to menu Master data > Company > Product surcharge allocation.
    Dialog Product surcharge allocation appears.
    ⇨ Software Reference, "Surcharge Product Assignment" on page B-1049
2.  Go to the menu Start > New to switch to the input mode.

*A screen capture of the 'Surcharge Product Assignment' dialog in input mode, with fields for Allocation, Surcharge, Product, and validity dates.*

**A** Customer
**B** Choose the surcharge
**C** Product for the surcharge
**D** Item

*Fig. B-206: Fields for automatic surcharge are accessible*

The fields are preset with the data of the surcharge selected from the list.
3.  Choose the option Customer (A) and the customer for which this surcharge/discount shall be entered.
4.  Select the automatic surcharge/discount (B) you want to define, e. g. the entry Special discount 3.
5.  Select the product (C) to be allocated to the surcharge, e. g. the product Special discount training.
    Product Special discount training has already been assigned a price (proportional surcharge).
6.  Choose a long period of time in field Valid to, e. g. 2099 if the surcharge/discount shall be applied always.
    In this example, the validity is limited to the 31.12. of the current year.
7.  Enter the Item in the document (D):

*B-400*
*A+W Business Master data*
