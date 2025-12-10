---
description: "EN_AWBusiness_Master_Data_9_2-4"
---


# Product data - Tutorial 1

---
## Shape

Shapes are entered in the catalog without sizes and glass as a product. In an order item, these non-rectangular shapes from the shape catalog can be assigned to a glass product and completed by the required sizes.

*   **Fig. B-95: Schematic layout of the shape**
    *   **A**: Shape with wildcard sizes
    *   **B**: Shape sizes in the order
    *   **C**: Shape number

This example shows that shape 2 (C) appears without sizes at first (A). The display is updated after the item sizes have been entered (B).

Working with shapes is described in detail in section Sales.

## Display of Shapes in A+W Business

The way in which shapes are to be displayed in product management and at order entry is defined in company data.

*   **Fig. B-96: Company data - System**
    *   **A**: Color setting for displaying shapes
    *   **B**: Path for shape templates

The color setting (A) and the sizes refer to the display of the sketch in the dialog.

*   **Fig. B-97: Unfilled sketch, filled-sketch**
    *   The image shows two octagonal shapes, one as an outline (unfilled) and one with a solid color (filled), demonstrating the display options.

## Bill of Material (BOM)

A product can consist of several other products, e. g. an IG unit can consist of two lites, a spacer, and a round shape. All elements of the BOM have to be entered as products.

*   **Fig. B-98: Structure of the product IG**
    *   This diagram shows a product `IG 150100` being broken down into its BOM components: `Float 4`, `Spacer`, `Grills`, `Float 4`, `Coating`.

The following functions are based on the bill of material:
- Pricing
- Product names in documents, e.g. on the order confirmation.
- Stock management planning
- Production control
- Production time calculation

You can define your products in such a way that input is largely automated. The bills of material and their elements are available at order entry and can be adapted to the order in question.

### Production BOM Breakdown

The so-called production BOM breakdown is entered in product management for every production with a BOM if the processing step shall or must not be applied to the main product.

**Example**

Hinges and door handles have to be added to a glass door before the glass is toughened.

When you enter the structure of a glass door you have to tick the checkboxes for Drilling and Handles. These processing steps will be performed by default and do not have to be entered in the order.

## BOM Concept in A+W Business

In A+W Business, products are described by product master data. These include details such as name, type, product group, variants, colors, supply types.

Bills of material describe the product structure.

*   **Fig. B-99: BOM elements of an IG product (order)**
    *   **A**: Main product: IG
    *   **B**: 1st element: single annealed glass
    *   **C**: 2nd element: spacer with gas
    *   **D**: 3rd element: heat-protection glass
    *   **E**: 4th element: shape
    *   **F**: 5th element: step

BOM elements can be individual products as well as processing steps or further bills of material, so-called assemblies. All BOM elements have to be entered as products in master data.

**Examples**
- The product 'spacer' can be entered with the gas firmly allocated.
- The gas will always be added to the spacer as an element in this case.
- When you replace a spacer you can define whether the corresponding gas shall be replaced too.
- Film layers in laminated units can be added before or after the single annealed lite.

Every main product and every element is marked by the supply type which triggers the necessary action, e.g. purchase order, stock withdrawal, production.

Individual conditions for pricing can be defined for every BOM element.

Exchange/addition rules allow replacing certain articles or processing steps on the product BOM.

The BOM structure has no limits. The processing speed of the data in the program will however be reduced considerably if the BOM gets too bulky.

> **Restrict the BOM structure**
> In company data you have to define the maximum number of BOM elements that can be printed. Excess components will not be printed on the order. This will have no influence on production.
> ⇨ Software Reference, "BOM" on page B-980

## Passing on BOM Details

Modifications of BOM elements can be passed on to other elements. This means that the changes will be applied to other elements. Whether or not changes will be passed on depends on if they apply to sizes, or to the replacement of elements.

- **Sizes** are passed on to the various BOM elements (size transfer). The sizes of the main product 'triple IG' for instance will be passed on to all lites of the BOM.
- As to the **transfer of surcharges**, there is a selection of definitions which either consider the basic item or the so-called parent product. The basic item is the top level of the bill of material. A parent product is the basic product of an assembly, e.g. the laminated glass lite which is fitted as an assembly into an IG unit.

*   **Fig. B-100: Distinction: Basic item - parent product**
    *   **Product: Laminated glass**
        *   **A**: Basic item
    *   **Product: IG with a laminated glass lite**
        *   **B**: Parent product

The transfer of surcharges is described in detail in connection with Surcharges.
⇨ "Transfer of surcharge types" on page B-317

> **BOM of the parent product**
> The BOM of the parent product will not be displayed if the parent product itself is not produced but taken from stock.

## Price- and/or Production-Relevant

At order entry, A+W Business distinguishes BOM elements which are relevant for pricing and those that are relevant for production.

**Example**
- The **price-relevant element** is directly linked with the main product, e.g. toughened glass.
- The **production-relevant element** (the processing) is connected to the float glass because this will be processed.

Production-relevant BOM elements can already be entered in product master data if they are to be applied as a standard.
Production-relevant BOM elements are shown in blue at order entry.

*   **Fig. B-101: BOM elements in product master data and in the order**
    *   **A**: Main product
    *   **B**: Production-relevant element
    *   **C**: Price-relevant element (processing)

The code is set in dialog Product management which is going to be introduced in the next session.
⇨ "Define Production BOM Breakdown" on page B-189

> **Restrictions**
> If restrictions have been defined for a product in dialog Processing restrictions, you can enter an alternative product. The assigned alternative product is available at order entry if the restrictions of the selected product are not met by the order data (item data).
> Spacer text for IG products can be automatically created from the defined text, and printed.

**Additional information**
⇨ Software Reference, "Product Management" on page B-590
⇨ Software Reference, "BOM transmission of variants" on page B-938

## Product Definition

When you define a product you have to enter at least the number, the name, and the product type. All other data can be added later.

There are the following instructions on this subject.
- "How to enter a product" on page B-182
- "How to complete the product data" on page B-184

> **The product type influences the fields displayed**
> Please make sure to select the right product type because this will determine which fields are accessible in the Product Management dialog.

When setting up your product master data you should first decide how to arrange the products so that the first digit of the product number identifies the product type.

| Example | from number | to number |
| :--- | :--- | :--- |
| Single annealed | 1000 | 1999 |
| IG | 2000 | 2999 |
| Toughened glass | 3000 | 3999 |
| Laminated glass | 4000 | 4999 |
| Grills | 5000 | 5999 |
| Shapes | 6000 | 6999 |
| Processing | 7000 | 7999 |
| Articles | 10 000 | |

> **Individual products**
> You can define individual products for recurring orders. These product structures are usually defined as macros and saved for a certain customer. Moreover, you can enter a customised fixed price.

### Free numbers

You can view the free numbers in dialog Product management by clicking on the [Zoom] icon next to the input field for the number. This view is described in section Partners.
⇨ "Input of Partner Master Data" on page B-50

### How to enter a product

1.  Go to menu **Master data > Products > Articles > Articles**.
    Dialog Product management appears.
2.  Go to menu **Edit > New**.

*   **Fig. B-102: Fields for new product are accessible**
    *   **A**: Product number
    *   **B**: Product type
    *   **C**: Lock codes

3.  Enter a number (A).
    The article number can consist of up to eight digits. You can choose the product numbers random; every number must however be assigned just once. You can view the free numbers by clicking on the [Zoom] icon.
4.  Enter the appropriate terms in fields **Matchcode** and **Description**.
    The alpha-numerical matchcode may consist of up to fifteen digits.
5.  Choose the product type (B).
    The product group appears automatically. It can be changed if required.
6.  Check the setting in field **Lock code (C)**.
    If the new product shall not be available for orders yet please select the lock code locked.
7.  Select in the menu **Start > Save** to save the data.

With that, you have entered a new product. The product can be displayed in other modules only if the lock code is set to **not locked**.

Enter the necessary data in the tabs **Product, Production, Price/surcharges, Inventory/purchasing** and - if applicable - **BOM**. Leave the fields blank for which entries cannot be made at this stage, e.g. prices.

## Product data for transfer to A+W Production

> Data which shall be transferred to A+W Production for production purposes, have to be entered in A+W Production tab. This tab is accessible only if the A+W Production connection has been enabled in company data.
> ⇨ Software Reference, "Company Data - Production" on page B-983

### How to complete the product data

1.  In the new product, go to tab **Production** and check the settings in section **BOM parameters**.
    If the product can be used as part of a BOM, tick the checkboxes **suitable for IG** and **Pattern level rotatable** if applicable.
    If the product shall be purchased (ordered), tick the checkbox **BOM irrelevant for production**. Please also choose this setting if the product must not be included in any BOM.

2.  Go to tab **Price/surcharge** and select the price tables for sales and purchasing in section **Price parameters**.
    Skip this step if no suitable prices have been entered yet. You can allocate the unit to the prices later.

3.  Go to tab **Stock/purchasing** and check the settings in section **Product code**.

    The following settings are available:
    - **Production:** The product will be produced in-house.
    - **Cutting:** The glass for this order item is cut from stockplates.
    - **Stock withdrawal:** The product is kept on stock, with just this size or as a unit.
    - **Processing:** The product is a processing step which is transferred to production by means of the order item.
    - **P.O., P.O. (complete):** The product will not be produced in-house but ordered from a supplier.

4.  Select in the menu **Start > Save** to save the data.
    The data will be saved. Tab **BOM** will be introduced in the following session.

## Edit BOM Structure

Carefully consider which elements you are going to be enter in product master data and which can be added at order entry. Product definition must include all production-relevant BOM elements.

*   **Fig. B-103: BOM elements**
    This table shows which BOM elements are typically entered in product management versus at order entry.

| Product management | Order |
| :--- | :--- |
| Glass | Sizes |
| Spacer | Grills |
| Prices | Shape |
| Procurement type | Processing |
| Steps | Steps |

This example shows which BOM elements are rather entered in product master data, and which are mostly added at order entry. At the end of the day, all elements can be changed in the order.

Details on steps may be useful even in master data. This subject is handled in a separate session.
⇨ "Adding Steps to an IG Product" on page B-186

Details on grills, shapes, and processing steps are rather expected in connection with order items. These BOM elements are described in detail in section Sales.

## How to edit a BOM

1.  Go to menu **Master data > Products > Articles > Articles**.
    Dialog **Product management** appears.
    ⇨ Software Reference, "Product Management" on page B-590
2.  Search the product the BOM of which you want to edit.
    Restrict the search to a product type the products of which are part of the BOM, e. g. IG or laminated glass.
3.  Go to tab **BOM**.
4.  In section BOM tag the element above or below which you want to add an element.
5.  Open the context menu and enter the required command.

    *   **Fig. B-104: Context menu for editing the BOM**
        The menu shows options like `Insert element (before)`, `Insert component (after)`, `Add element`, `Delete element`.

    This commands have the following effects:
    - **Insert element (before, after):** The cursor automatically switches to field **Article number**. When you select the element, it will be added to the BOM on the same level.
    - **Add element:** The cursor automatically switches to field **Article number**. When you select the element, it is automatically added to the BOM on the level below.

6.  Go to the menu **Start > Save** to save the changes.
    The data will be saved.

> **Changing BOM elements**
> BOM elements can be replaced by other elements. When an element has been selected it can be replaced in field **Article number**.

## Adding Steps to an IG Product

Steps can be useful for IG products which are usually entered with steps in the orders.

### How to enter a step

1.  Go to menu **Master data > Products > Articles > Articles**.
    Dialog **Product management** appears.
2.  Search the IG product the BOM of which you want to edit.
3.  Go to the **Shapes/processing** tab.
4.  Select the step by entering the product number, or by means of the corresponding icon.
    The fields to enter the values are displayed.

    *   **Fig. B-105: Define step**
        *   **A**: Select the lite for which the step shall be defined:
            1 = Outside lite
            2 = Inside lite
        *   **B**: Enter the values per edge:
            Positive entries will scale down the selected lite
            Negative entries will enlarge the lite

    The fields for the sizes are now enabled. If no shape has been entered, a rectangular lite will appear automatically.
    In section **Parameters**, a checkbox (A) pops up for every glass element. In this example, this is an IG unit consisting of two lites. For triple IG, three checkboxes will appear. Checkbox 1 is the outside lite.
5.  Enter the size of the step per side (B).
    Please make sure to tick checkbox 2. You will have to enter positive values for this lite in the fields, e. g. 15.
    When you enter a negative size (-15), a larger lite will be cut. This would mean that lite 2 (inside) would be bigger than the outside lite.
    The sketch shows for which sides steps have been defined.

    *   **Fig. B-106: Sketch with steps on four sides**

6.  Select in the menu **Start > Save** to save the data.
    The step is shown as a BOM element.

    *   **Fig. B-107: BOM with steps**

7.  Select in the menu **Start > Save** to save the data.
    The data will be saved.

Grills, shapes, and processing steps are added in the same way. These steps are described in detail in section Sales as these elements will mostly be added at item input.

## Define Production BOM Breakdown

This session will show you how to define the BOM element to be processed.

### How to edit the production BOM breakdown

1.  Go to menu **Master data > Products > Articles > Articles**.
    Dialog **Product management** appears.
2.  Search the product the BOM of which you want to edit.
3.  Go to tab **BOM**.
4.  In section **BOM**, select the element the production BOM breakdown of which you want to edit.
    The fields in section **Production BOM breakdown** are accessible.

    *   **Fig. B-108: Valid processing steps for the transfer to production**
        This UI shows a list of processing types with checkboxes to mark them as `Active`.

5.  Tick the checkboxes of the processing steps to be applied to the selected element, e. g. **drilling**.
6.  Select in the menu **Start > Save** to save the data.
    The data will be saved. Production-relevant elements are shown in blue at order entry.

## Grill Input

Grills and grill patterns can be defined for an IG unit if this kind of product frequently occurs in orders. The details can be amended in the actual document.
There are the following instructions for this session:
- "How to enter a common grill pattern" on page B-190
- "How to enter an uneven grill pattern" on page B-192

> **Prerequisite**
> A grill pattern can be defined in product management only if minimum and standard sizes have been entered for the IG product on tab **Product**.

### How to enter a common grill pattern

1.  Go to menu **Master data > Products > Articles > Articles**.
    Dialog **Product management** appears.
2.  Search the IG product the BOM of which you want to edit.
3.  Go to tab **grills**.
4.  Choose the grill pattern by means of the corresponding icon.
    The fields for the vertical and horizontal grills are released.

    *   **Fig. B-109: Fields for grills are enabled**
        *   **A**: Grill pattern selection
        *   **B**: In the case of multiple IG: Select the spacer
        *   **C**: Selection of grills
        *   **D**: Number of grills
        *   **E**: Cutback
        *   **F**: Calcul. type

5.  Choose the grills (C) and enter the quantity (D).
    If you have entered a multiple IG unit, you must select the spacer (B) to which the grills shall be attached.
    The graphics and the fields will be updated. You can choose different products and/or variants for the horizontal and vertical grills.
    Use this button to adopt the grills for the second spacer.
    However, you can also design the grill grids differently in the gaps, e. g. position the horizontal grills in the first gap and the vertical ones in the second.

6.  Define the calculation type (F) and enter the drilling sizes if necessary.
    The fields for the drilling positions are only released for asymmetrical calculation types.
    ⇨ "Grills" on page B-162

7.  Check the size of the cutback (E) and define whether or not felt pads shall be fitted.
8.  Select in the menu **Start > Save** to save the data.
    The grills appear on the BOM.
9.  Select in the menu **Start > Save** to save the data.
    The data will be saved.

### How to enter an uneven grill pattern

1.  Enter the grills as described in steps 1 to 7 of the previous process.
    Please make sure that the number of grills permits an asymmetrical pattern.
2.  To fit V grills, go to tab **Auxiliary grills**.

    *   **Fig. B-110: Uneven grill pattern**
        *   **A**: Diagonal grills
        *   **B**: Vertical grills
        *   **C**: Horizontal grills

3.  Disable the checkboxes for all grid section that are not required, e.g. the vertical grills in the top third (B).
4.  Enable the checkboxes for diagonal grills (A).
5.  Select in the menu **Start > Save** to save the data.
    The data will be saved.

Special grill patterns such as sun or moon are also possible. These are the subject of a separate training session on A+W CAD Designer.

## Define Shapes

Shapes can be defined for an IG unit if this kind of product frequently occurs in orders. The details can be amended in the actual document.

> **Prerequisite**
> You can define a shape for a glass only if shapes have been specified as a product.

### How to enter a glass with a shape

1.  Go to menu **Master data > Products > Articles > Articles**.
    Dialog **Product management** appears.
2.  Search the product the BOM of which you want to edit, or enter a new product.
3.  Go to tab **Shapes/processings**.
4.  Select by using the icon **Shapes**.
    The fields to enter the values are displayed.

    *   **Fig. B-111: Shape input**
        *   **A**: Enter sizes
        *   **B**: Select a shape
        *   **C**: Dimensions for price calculation

5.  Select the shape by entering the shape or product number, or by means of the corresponding icon (B).
    Section **Display** shows a sketch of the shape; the fields for the corresponding sizes are released.
6.  Enter the sizes for the edges (A).
    Please obey the appropriate notes, W1+W2<=W for example means that the total of the entries for edges W1 and W2 must not exceed the size of edge W.
    When you have made all entries, the size of the surrounding rectangle is shown which is used for price calculation by default.

    *   **Fig. B-112: Shape entered**
        This image shows the shape input screen after the dimensions have been entered.

7.  Go to the menu **Start > Save** to adopt the shape data.
    The data will be saved. The shape appears on the BOM.
8.  Go to the menu **Start > Save** to save the data.
    The data will be saved.

## Define Processings

Processing steps can be defined for a glass if this kind of product frequently occurs in orders. The details can be amended in the actual document.

### How to enter a processing step for a lite

> **Prerequisite**
> Processing steps have to be defined as products.

1.  Go to menu **Master data > Products > Articles > Articles**.
    Dialog **Product management** appears.
2.  Search the product the BOM of which you want to edit, or enter a new product.
3.  Go to the **Shapes/processing** tab.
4.  Select the processing step by entering the product number, or by means of the corresponding icon, e. g. edgework.

*   **Fig. B-113: Processing: Example: Edge sawing**
    *   **A**: Select the processing step
    *   **B**: Selection of the edges to be processed
    *   **C**: Reference corners, reference edges
    *   **D**: Mitre angle

Product data for this processing step are loaded now. The fields for the corresponding parameters are displayed and enabled.
The parameters are described in detail in chapter Sales.

5.  Enter the parameters by ticking or unticking the checkboxes (B) for the edges, and enter the sizes.
    Please obey the reference corners or reference edges (C) and convert the sizes if necessary.
6.  Go to the menu **Start > Save** to adopt the data.
    The data will be saved; price fields will be updated. The BOM shows the processing and the corresponding price.
7.  Go to Menu **Start > Save** to save the product.
    The data will be saved.

> **Wrong or missing processing parameters**
> If incorrect parameters are displayed for a processing step, you have to check if the proper product type and group have been allocated to this product in product management.

## Exercises

Enter the following products:
- Grills
- Single annealed, e.g. wired ornaments which must not be part of an IG unit.
- Toughened glass to be purchased.
- Laminated glass to be produced in-house. Please consider the production BOM structure.
- Complex IG product with two different lites, all edges stepped.

## Stock Sizes and Variants

### Objectives

- Knowing the difference between stock size and stock article
- Knowing the interaction of product, stock article, and stock size
- Introducing the function of variants
- Defining product variants

### Benefit

- If the products are defined correctly, pieces and surfaces can be calculated and reserved.
- The display of the actual stock on hand including reservations makes purchasing easier.
- All color variants of a product can be managed by the same product number.

### Note

- **Products**: The products defined in master data serve for the input and pricing of documents. They will not be automatically kept as stock on hand.
- **Stock size**: A+W Business distinguishes stock sizes for pricing (in the order) and stock sizes for stock management.
- **Stock code (stock booking type)**: The stock code defines whether the stock on hand for an article is evaluated as a surface (sqm) or a quantity (pieces).
- **Procurement type**: The code defines how a product is to be provided by default, e. g.:
    - Cutting
    - Stock withdrawal
    - Production
    - Purchasing
- **Variants**: Products with identical properties can be kept in different colors. The product is defined just once and is distinguished further by allocating the colors (variants).

## Product Data and Stock

All products entered in the sales area are allocated a code to identify the procurement type. Apart from the code (procurement type) **Stock withdrawal**, glass kept on stock has a code (stock booking type) defining how the stock on hand is calculated.

Products kept on stock with their quantities have to be defined as so-called **stock sizes**.

A+W Business distinguishes stock sizes for pricing (in the order) and stock sizes for stock management.
- **Stock sizes are used at order entry and for pricing.** You can enter several stock sizes per (glass) product, with different widths and heights. If these sizes are kept on stock they do not have to be cut. This is why these prices can be calculated differently.
- **Stock sizes for stock management serve for stockkeeping.** Lites can be defined in different sizes for stock management.

*   **Fig. B-114: Relations between product, stock size, and price**
    This flowchart illustrates the relationship between Master Data (Product, Sales price list), Sales (Order item), and Stock (on hand). An order for a specific size can be fulfilled either by cutting a larger stockplate (consumption by surface) or by taking a pre-cut stock size (consumption by pieces). This is driven by pricing which can be per sqm for cutting or per piece for a fixed size.

You can enter several stock sizes for a product, with different sizes.
