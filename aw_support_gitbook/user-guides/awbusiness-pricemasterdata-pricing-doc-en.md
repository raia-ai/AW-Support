---
description: "A+W Business Master Data - Price Master Data Tutorial"
---


# Tutorial 1: Price Master Data

---
## Processing Index

The limit types **Processing index** and **Processing index exact** can be used for rating the work required and the difficulty of processing products.

**Example**
- A float lite belongs to Index 1 because it is the easiest to process.
- A laminated lite belongs to index 2 because the heated film layer sticks to the grinding wheel at cutting and these have to be cleaned afterwards.
- Wired glass belongs to index 3 because the wear of the cutting wheel is highest here.

*Fig. B-150: Use of the limit type 'processing index'*

The document shows two interface snippets:
- **A: Price graduation by processing index:** A price vector table where different processing indices have different prices per piece (Stk).
- **B: Allocation in product master data:** A dropdown in the product master data to assign a specific "Processing index" (e.g., 3) to a product.

| Bearbeitungsindex / Processing index | Price | Price unit |
| :--- | :--- | :--- |
| 1 | 4.50 | Stk |
| 2 | 7.50 | Stk |
| 3 | 12.80 | Stk |
| 4 | 19.60 | Stk |
| 5 | 23.20 | Stk |

You can enter a price table (A) for every processing index of a product group. In product master data (B), define the processing index to which the product belongs.

## Vector

In case of vector, you enter the price based on a limit type, e.g. metre, piece, surface, litre. These prices can be graduated by quantity.

*Fig. B-151: Vector*

The interface shows a "Price vector" screen with the following labeled parts:
- **A:** Graduation values (e.g., up to 0.25 sqm)
- **B:** Limit type (e.g., qm/sqm)
- **C:** Price per limit type
- **D:** Price unit

This example shows that the price (C) is graduated by the limit (A) of the surface area (B). It does not matter whether the length is entered as width or height. The price will be calculated by surface (D).

**Price unit** and **Limit type** do not have the same.

**Example**

| Limit | Price |
| :--- | :--- |
| up to 0.25 sqm | 40.00 € per piece |
| up to 0.35 sqm | 35.00 € per piece |
| up to 10.00 sqm | 50.00 € per sqm |
| up to 25.00 sqm | 40.00 € per sqm |

In this example, the price for the limit type Surface (price units: pc. and surface) is graduated:
- For lites up to 0.25 sqm, 40 € per piece shall be calculated.
- For lites from 0.26 sqm to 0.35 sqm, 35 € shall be calculated per piece.
- For lites from 0.36 sqm to 10 sqm, 50 € shall be calculated per sqm.
- For lites from 10.1 sqm to 25 sqm, 40 € shall be calculated per sqm.

For a drilled hole for example, the combination of the limit type Diameter with limits in millimetres and the price unit Piece will be useful.

## Matrix

In a matrix, the price depends on two limits, e.g. width and height or surface and thickness.

*Fig. B-152: Matrix*

The interface shows a price matrix screen with the following labeled parts:
- **A:** Limit type 1 (e.g., Breite / Width)
- **B:** Limit type 2 (e.g., Höhe / Height)
- **C:** Graduation for limit type 2 (the rows of the matrix)
- **D:** Graduation for limit type 1 (the columns of the matrix)
- **E:** Triangular form checkbox

### Triangle

You can create a triangular matrix so that the limit types can be exchanged, e.g. height and width. You only have to enter one of the combinations. With triangular price tables, the cutting direction does not matter.

At order entry, sizes are turned so that the bigger size is the height, no matter in which sequence the sizes for width and height are entered.

> **Non-applicability of the triangle**
> A price table must not be entered as a triangle if the direction in which the glass is cut is important. If height and width of patterned glass must not be exchanged, you have to enter all prices for all possible combinations.

### Example

The following is an example of a triangular price matrix.

| | 300,00 | 360,00 | 420,00 | 480,00 | 540,00 | 600,00 | 720,00 | 840,00 | 960,00 | 1080,00 | 1200,00 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **300,00** | 181,370 | | | | | | | | | | |
| **360,00** | 168,230 | 155,600 | | | | | | | | | |
| **420,00** | 147,520 | 136,910 | 120,240 | | | | | | | | |
| **480,00** | 130,850 | 122,760 | 99,020 | 98,010 | | | | | | | |
| **540,00** | 123,270 | 108,110 | 95,990 | 85,880 | 79,820 | | | | | | |
| **600,00** | 112,660 | 97,000 | 87,400 | 79,320 | 72,750 | | | | | | |
| **720,00** | 101,040 | 89,930 | 79,320 | 72,750 | 66,690 | | | | | | |
| **840,00** | 91,440 | 79,820 | 71,740 | 67,190 | 66,690 | | | | | | |
| **960,00** | 83,360 | 75,780 | 70,220 | 65,680 | 64,160 | | | | | | |
| **1080,00** | 79,820 | 72,750 | 69,720 | 65,680 | 62,640 | | | | | | |
| **1200,00** | 75,780 | 70,730 | 69,210 | 65,170 | 60,120 | | | | | | |

In the triangle, the following sizes will have the same price, e.g. 67.19 €:
- Width 840 mm × height 480 mm
- Width 480 mm x height 840 mm

If the sizes must not be turned at order entry, you have to enter the price for all formats.
In this case, the sequence in which the sizes are entered will be taken into account; the price for a width of 1080 x height 480 mm would e.g. be 168.75 Euro.

## Cube

Cubes are similarly structured as matrix tables but with three limits, e.g. width, height, and thickness.

*Fig. B-153: Cube*

The interface shows a "Cube" pricing screen with three limit types. The labeled parts are:
- **A:** Limit type 3 (e.g., Durchmesser / Diameter), which acts as a level selector.
- **B:** Graduation for limit type 3, showing the different levels (e.g., 10, 20, 30).
- **C:** Prices on level 1 (the price matrix for the first value of limit type 3).
- **D:** Prices on level 2 (the price matrix for the second value of limit type 3).

As for a matrix, please remember: If you enter the prices as a triangle, you do not have to enter all prices for all combinations of limit types.

### Graduation limit

If you want to enter graduations only up to a certain size you can define a 'next key'.
⇨ "Next key" on page B-217

## Defining a Graduated Price with Limits

For some products, price graduation by one or more limit types is useful, e. g. drilling by thickness, IG units by size.

> **Knowing the input principles**
> Before entering a graduated price you should have entered at least a unit price. The following description is based on this knowledge.

The following steps show how to define a price graduation for IG units in the shape of a cube. This allows to show the application of three limit types. Similarly, these instructions can be used for defining prices in other graduation types.

After selecting the type, the sequence is the same for all:
- Select limit types.
- Enter the limits for the graduation.
- Enter prices.

There are the following instructions for this session:
- "How to enter a graduated price" on page B-256
- "How to define the limits for limit type 1" on page B-258
- "How to define the limits for limit type 2" on page B-259
- "How to define the limits for limit type 3" on page B-260
- "How to copy the prices from one level to another" on page B-260

### How to enter a graduated price

1.  Select menu **Master data > Prices > Prices**. Dialog `Prices` appears.
2.  Go to the menu **Start > New** to switch to the input mode.
3.  Fill in at least the fields in section **Identification**. These steps are described in detail in connection with unit prices. ⇨ "How to create a price table for a unit price" on page B-237
4.  Go to tab **Cube**.

*Fig. B-154: Price graduation, cubic shape*

The interface for a cubic price shape has the following labeled parts:
- **A:** Column header
- **B:** Line header
- **C, E, G:** Fields to enter the limits for each limit type.
- **D, F, H:** Dropdown menus to select Limit type 1, 2, and 3.

5.  Tick the checkbox **Triangle**. If you do not tick this checkbox you have to enter the prices for all combinations of the selected limit types, e.g. for all widths and heights as well as the thicknesses if required. ⇨ "Limit Types for Graduations" on page B-249
6.  Enter the minimum values for pricing. You can enter the value 300 mm as the smallest limit for the width and height although minimum sizes of 200 x 300 mm shall be valid for production. Pricing will only consider the limit sizes for calculation but not for production. This way, the price for the minimum quantity will be calculated even for a smaller lite.
7.  Enter the **Price unit** and the **Currency**. The price unit is the reference size to which the graduation refers. The currency is essential if you are working with several currencies.
8.  Choose the limit types (D, F, H), e. g. width, height, and thickness (BOM). By selecting these limit types you define that the price of the lite does not only depend on its size but also on the total thickness.
9.  Select in the menu **Start > Save** to save the data. The data will be saved. Now enter the limits for the graduation. Start with limit type 1.

### How to define the limits for limit type 1

1.  Open the context menu by a right mouse click on the column header (A).
    *Fig. B-155: Adding a step for the width*
2.  Select the entry **Insert > Above** from the context menu (B). A new column (A) is added and the field for entering the limit (B) is accessible.
    *Fig. B-156: Adding the limit for the width*
3.  Enter the value for limit type 1 (B), e. g. **480** and confirm your entry by pressing the `<Tab>` key. The value appears in the new column header (A).
4.  Repeat the steps until all limits for the width have been set. Next, set the limits for limit type 2.

### How to define the limits for limit type 2

1.  Open the context menu by a right mouse click on the line header.
    *Fig. B-157: Adding a step for the height*
2.  Select **Insert > Below** (B) in the context menu. The field for entering the limit (A) is accessible and a new line (B) is added.
    *Fig. B-158: Adding the limit for the height*
3.  Enter the value, e. g. **900** and confirm your entry by pressing the `<Tab>` key. The value appears in the new line header.
4.  Repeat the steps until all limits for the height have been set.

The first level of the cube has not been defined. Decide how you want to proceed:
- Set the limits for limit type 3.
- Enter prices on the first level. Position the cursor on the appropriate line and enter the price.

### How to define the limits for limit type 3

1.  Open the context menu by a right mouse click on the combo box below the first column.
    *Fig. B-159: Adding a step for the thickness*
2.  In the context menu, select **Insert** (B). The field for the thickness limit (A) is accessible; a new tab will be added.
3.  Enter the value, e. g. **24** and confirm your entry by pressing the `<Tab>` key.

The value appears in the combo box. Repeat the steps until all thickness levels have been defined.

If you had entered prices on the first level, these will be adopted for the new level. You can amend these prices as required. A copy function allows the automatic adjustment of prices.

### How to copy the prices from one level to another

1.  Choose the level with the prices to be copied. The prices are identical on all levels provided they had been defined before further levels were added.
2.  Open the context menu by a right mouse click on the combo box of the levels.
    *Fig. B-160: Context menu*
3.  Select **Copy** (B) from the context menu.

*Fig. B-161: Context menu*

The "Copy prices - Cube" dialog appears with the following options:
- **A: Target level:** Select the level to which prices will be copied.
- **B: Proportional value of the change:** A percentage value for the change.
- **C: Absolute value of the change:** A fixed currency value for the change.
- **D: Price increase or reduction:** Radio buttons for "Surcharge" or "Deduction".

4.  Select the level (A) to which the prices shall be applied.
5.  Define how the prices are going to be changed.
    - **Proportional (B)** or **absolute (C)** value by which the new prices shall be changed.
    - **Surcharge** or **reduction (D)**.
    If you enter e. g. 3.2 in field Per cent and select the option Surcharge, all prices will be raised by 3.2 %.
    If you enter e. g. 5 in field Absolute then choose the option Surcharge, all prices will be raised by 5 €. Option Discount works the same way.
6.  Click on **[OK]** to copy the data. The prices are applied to the target level as defined. To transfer the prices to other levels please be careful to check the level from which the prices are copied.
7.  When you have entered the prices on all levels go to menu **Start > Save** to save the data. The data will be saved. They can be allocated to price tables in product definition.

## Price Calculation by PGR

Normally, every product gets a price. Pricing can also be controlled by means of the product groups (PGR).

This is done in two steps:
1.  First enter an external key in the product group.
2.  This external key is entered as a limit in the price table.

You can select the limit type **External PGR key** for all price types except the unit prices.

There are the following instructions on this subject.
- "How to enter an external key in a product group" on page B-262
- "How to allocate the external keys as limits" on page B-263

### How to enter an external key in a product group

1.  Go to **Master data > Products > General > PGR**.
    *Fig. B-162: Enter an external key for PGR*
2.  Choose the product group (A).
3.  Enter the value of the **External PGR key** in field **External key** (B). You can choose this at random but you can only enter numerical values, e. g. 123. The same value can be entered as an external key for several product groups.
    *Fig. B-163: External key for PGR*
4.  Select in the menu **Start > Save** to save the data. The data will be saved. You can now enter this external key in the price table as a limit.

### How to allocate the external keys as limits

1.  Select menu **Master data > Prices > Prices**. Dialog `Prices` appears.
2.  Search the price for which you want to enter an external key, or create it. ⇨ "How to enter a graduated price" on page B-256
3.  Go to the tab in which the limits shall be entered, i.e. **Matrix, Vector** or **Cube**.

*Fig. B-164: External key for PGR*

The interface shows a price vector with the following labeled parts:
- **A:** External key (number)
- **B:** Select the limit type (PGR foreign key)
- **C:** Price
- **D:** Price unit

4.  Choose the limit type **PGR external key** (B) and enter the value (A) you have defined in the product groups, which in this case is **123**.
5.  If necessary, enter the price (C) if no price had been entered in the table as yet.
6.  Select in the menu **Start > Save** to save the data.

The data will be saved. The price is now used for calculating all products allocated to the PGR in which the external key has been entered.

If you want to work with several external PGR keys you can e.g. create a cube in which the external PGR key is used as a third limit type. You can e.g. define an external PGR key for toughened glass and another for laminated lites.

## Exercises

- Consider for which products a simple price is practical and for which a graduated price is recommended.
- Define a price with limits.
- Determine the way and graduation for entering prices. Based on these considerations you have to choose a matrix, a vector, or a cube.
- Copy the new prices with a reduction of 2.5 % for your training customer. Attention, the reduction should only be valid for the training customer!

> **Graduation of limits**
> There are no restrictions regarding the graduation of limits. The graduation should be logically connected to the selected limit type however.

**Additional information**
⇨ Software Reference, "Price Management" on page B-710
⇨ Software Reference, “Prices" on page B-659
⇨ Software Reference, "Price Groups" on page B-684
⇨ Software Reference, "Price and Quantity Unit" on page B-700
⇨ Software Reference, “Company Data > Price Calculation" on page B-944
⇨ Software Reference, "Calculate external PGR key as an inexact quantity limit" on page B-953

# Surcharges

Surcharges are another means of adapting your price lists. Surcharges can be applied to certain products, processing steps, or in general.
This subject area will introduce the different surcharges and their functions.

## Introduction of the Subject 'Surcharges'

Surcharges can be added for special services, e. g. for replacing one lite of an IG unit or for complex edgework for shapes.

### Surcharges for products and processing steps

The following surcharges are defined in direct connection with the prices for products and processing steps:
- Group Surcharges
- Replacement Surcharges
- Shape Processing Surcharges
- Miscellaneous Surcharges
- Automatic Surcharges

These surcharges are entered in **Master data > Prices**. Every surcharge can be defined for a customer or supplier group, for individual customers or suppliers.

Define the surcharge type and surcharge value to calculate these surcharges:
- The **surcharge type** defines the unit to which the surcharge refers, e. g. the surface, the price, the quantity.
- The **surcharge value** defines the amount of the surcharge.

Surcharges can be graduated in different ways. As for prices, limit types and limits are defined.
⇨ "Limit Types for Graduations" on page B-249

In an order, surcharges can be changed, removed, and others can be added. Shape-, grill-, or exchange surcharges will be included in pricing even if the price in the order is changed by hand. In contrast, Other surcharges will be taken into account in case of manual price changes only if they have been explicitly released for that.

### Product/surcharge allocation (automatic surcharges)

A special type are the so-called automatic surcharges, e.g. for toll, delivery fees, or energy surcharges. These surcharges are entered in **Master data > Company > Product/surcharge allocation**.

### Calculation sequence for surcharges

Surcharges for products and processing steps are calculated when the product is entered in an order. This is also the case if the product is a BOM element.

Since different surcharges can be defined it may happen that several surcharges are applied to an order item. This is relevant for pricing if the surcharge type **Gross %** is involved. The gross price to which a certain surcharge refers can already include another surcharge.

> **Sequence of sessions**
> The individual sessions in this set of topics are each based on the knowledge acquired in the previous session. This sequence does not match the sequence in which the dialogs appear in the Master data menu.

### Surcharge Settings (Company Data)

The standard calculation of surcharges can be changed in company data.

*Fig. B-165: Company data > Pricing*

The figure shows the "Price calc." tab in the company data settings, with many checkboxes (A) that control surcharge calculation.

This tab is used for defining the options for the documents. Any changes on this tab will overrule the standard calculation in A+W Business. For a detailed description of the checkboxes please refer to the software reference.

## Group Surcharges

**Objectives**
- Introducing the group surcharge function.
- Price group allocation.
- Defining group surcharges.

**Benefit**
- A surcharge - based on the glass thickness - can be applied if lites in IG or laminated glass units are exchanged.
- Group surcharges refer to glass types united in price groups. The surcharge for exchanging a lite therefore does not have to be defined per glass (product).

**Note**

- **Price groups**
  Price groups collect products in groups for which no separate price tables shall be created and maintained. Price groups are used for managing surcharges and discounts.
- **Calculation parameters**
  Surcharge calculation is based on different parameters, e. g.:
  - Value, per cent or absolute
  - Reference unit, e.g. surface, standard price, piece
  - Quantity of the order item
- **Surcharge type**
  The rules for proportional surcharges are:
  - **Gross price** = before deduction of discounts
  - **Net price** = after deducting the discounts
- **Group surcharges**
  Group surcharges refer to products allocated to a price group.
- **Surcharge calculation**
  The surcharge is applied if lites belonging to these price groups are replaced.
- **Property of group surcharges**
  A decisive property of a group surcharge is the glass thickness defined in the bill of materials. Different surcharges can be defined for glass of the same thickness.
- **Customer or supplier surcharges**
  When defining the group surcharge, a surcharge can be allocated to customers, suppliers, groups of partners or objects.

### The Function of Group Surcharges

Group surcharges refer to products allocated to a price group. The surcharge is applied if lites belonging to these price groups are replaced. Decisive for a group surcharge is the glass thickness defined for the IG or laminated glass unit.

**Example Table**

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

> **Example**
> Price group A shall include all colored single glass types, group B includes all patterned glass types, etc.
> Group surcharges for the price groups A-E have been defined for a thickness of 4 mm and 5 mm of the exchanged lite.
> For a 4 mm glass of price group A, a surcharge of 9.20 € per sqm would be applied. For a surface of up to 0.5 sqm, this is a surcharge of 4.60 €.
> This surcharge will not be applied for colored lites of 3 mm thickness.

Group surcharges are defined in three steps:
1.  First define the price groups.
2.  Next, allocate the glass types to the price groups.
3.  Last, define the surcharges per thickness for the price groups.

> **Exchange of BOM elements**
> You can define an exchange surcharge for glass that cannot be allocated to any price group.
> ⇨ "Replacement Surcharges" on page B-287

### Dialog 'Group Surcharges'

Dialog **Group surcharges** offers various tabs for surcharge allocation.
- **Price management:** These surcharges refer to generally applicable prices.
- **Customer selection:** These surcharges refer to the price lists for special customers.
- **Supplier selection:** These surcharges refer to the price lists for special suppliers.

The allocation to a customer or supplier price cannot be changed.

*Fig. B-166: Dialog 'group surcharges'*

The interface shows a screen with the following labeled parts:
- **A:** Surcharge on the sales or purchase price
- **B:** Combination of rates (Price list and key)
- **C:** Product type for which the surcharge is valid (e.g., IG, LG)
- **D:** Validity of the surcharge (General, Customer group, etc.)
- **E:** Price group to which the surcharge applies.
- **F:** List of surcharges

This example shows that there are different surcharges e.g. for lites of 4 mm thickness per price group (E).

Group surcharges apply to a certain rate (B). A combination of the price list `<n.e.>` and the key `<n.e.>` can also be used if prices have been entered for this combination.

Since group surcharges always refer to the exchange of a lite they can only be applied to IG or laminated glass lites (C).

### Price Groups and Price Group Allocation

For calculating surcharges and patterned glass you can define price groups to which the products are allocated. This simplifies the maintenance of price lists because you do not have to keep separate price lists for all these products.

As for products and partners, start by entering the (empty) groups as a basis. After that, allocate the products to the corresponding price group. Define the price group that is valid if the product is exchanged in an IG and/or laminated glass unit.

*Fig. B-167: Price groups and price group allocation*

The interface shows a screen with the following labeled parts:
- **A:** Price groups list
- **B:** Number of the allocated product
- **C:** Patterned glass product name
- **D:** Price group to be used when exchanging a lite in an IG unit
- **E:** Price group for exchanging a lite in a laminated glass unit

These examples show that price groups A to N (A) have been defined. In dialog **Price group allocation**, the following allocation is defined for the first patterned glass (C):
- If the glass is used for an IG unit (D) it is allocated to price group A.
- If the glass is used for a laminated glass unit (E) it is allocated to price group B.

You can define any required number of price groups. You should however decide in advance which glass types can be united in a group so that the surcharges and/or prices can be maintained together.

### Price Group Allocation

By allocating products and price groups, you join glass types for which the same surcharge shall be calculated in case of an exchange. You should therefore first specify (on paper) which glass types are to get the same group surcharge.

If price group allocation is impossible, you can define an exchange surcharge to be added to the standard price. This surcharge will be introduced in the next session.
⇨ "Defining an Exchange Surcharge" on page B-291

#### How to allocate a product to a price group

1.  Go to menu **Master data > Prices > Price group allocation**. Dialog `Price group allocation` appears.
    *Fig. B-168: Allocation to SP or PP*
    The screen shows options for **A: Sales list** and **B: Purchase list**.
2.  Choose one of the options in section **Identification - rate**, e. g. **Sales list (A)**.
3.  Go to the menu **Start > New** to switch to the input mode.

*Fig. B-169: Fields for the new allocation are accessible*

The input fields are now active:
- **A:** Select the rate (Price list and Price key)
- **B:** Select the product
- **C:** Select the price group

4.  In the fields **Price list** and **Price key** (A), select the rate for which the price group allocation shall be valid.
5.  Choose the product (B) to be allocated to the price group. You can enter either the product number or the matchcode. The selected product appears in section **List of allocations**.
6.  Click on the field in column **PG IG** (C) and select the price group, e. g. A. A selection of valid price groups appears in a combo box when you position the cursor on this field.
