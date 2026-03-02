---
description: "EN_AWBusiness_Master_Data_9_2-3"
---


# Tutorial 1: Product data

---
## Product Group Definition

Product groups (PGR) are used for the clear structuring of products, for quick input of articles, allocation of discounts and surcharges, and for statistical analysis. Budgets, commissions, and proceeds accounts are calculated on the basis of product groups.

Product groups only defined for statistical purposes are useful too.

> **Define MPG, PSG, or PGR**
> Main product groups (X**), product super groups (XX*), and product groups (XXX) are defined in the same way.

### How to define a product group

1.  Go to **Master data > Products > General > PGR**.
    Dialog **Product groups** pops up.

2.  Go to the menu **Start > New** to switch to the input mode.

    *(Fig. B-80: Shows the "Product groups" dialog. A tree view on the left (A) displays the PGR hierarchy. The fields on the right allow for entering a new product group's Number (B) and Name (C).)*

    The fields for the new product group are accessible.

3.  Enter the number (B) and name (C) of the product group.

4.  Leave the fields **Prep. days** and **Special surcharge** blank. You can fill them in later.

5.  Select in the menu **Start > Save** to save the data. The new product group will be saved.

6.  If necessary, select an icon (A) if the new product group shall not keep the bitmap of the superior product group.

7.  Select in the menu **Start > Save** to save the data. The data will be saved.

## Combine Product Groups

You can use wildcards instead of numbers when you define combination product groups. Please read the examples for combination rules carefully before entering a PGR combination.

⇨ "Rules for PGR Combinations" on page B-144

> **Sequence for defining product group combinations**
> Every combination of product groups results in a so-called PGR combination. This is not automatically created by combining the product groups, but has to be specially defined. First define the product groups which can result from PGR combinations. Only then can you select the PGR combination in the following steps.

### How to combine product groups

1.  Go to menu **Master data > Products > General > PGR combinations**.
    Dialog **PGR combinations** appears.

2.  Go to the menu **Start > New** to switch to the input mode.

    *(Fig. B-81: Shows the "Combo-PGR" dialog. The fields for the PGR combination are accessible.)*

    The released fields are preset by the values of the selected PGR combination.

3.  Select product groups 1 (A) and 2 (B).

4.  Enter the number of the PGR combination (C).
    Please obey the rules for wildcards should you want to use them. PGR combinations will not be created automatically when you enter a new number. You will have to create these new PGR combinations later in dialog PGR.

5.  Tick the required checkboxes (D) for the validity of the PGR combination.
    The checkboxes for editing discount combinations are accessible after you have ticked the checkboxes for the validity.

6.  Select in the menu **Start > Save** to save the data.
    The data will be saved.

> **Check the settings for PGR combinations**
> Please take into account the settings for product group combinations in company data.
>
> ⇨ Software Reference, "PGR combination for discounts valid only if discount exists" on page B-946
> ⇨ Software Reference, "Create PGR combinations using complete BOM" on page B-946

## Definition and allocation of Top PGR

To allocate a Top PGR, perform the following steps:
*   Create the Top PGR.
*   Allocate the PGR.

### How to set up a Top PGR for analysis

1.  Go to **Master data > Products > General > Top PGR**.
    Dialog **Top PGR** appears.

2.  Go to the menu **Start > New** to switch to the input mode.
    The next line is accessible now.

3.  Enter the name.

    *(Fig. B-82: Shows the "Top-PGR" dialog to create the Top PGR.)*

4.  Select in the menu **Start > Save** to save the data.
    The data will be saved.

5.  Close the dialog **Top PGR**.

6.  Go to menu **Master data > Products > General > PGR**.
    Dialog **Product groups** pops up.
    ⇨ Software Reference, "PGR" on page B-566

7.  Go to the menu **Start > New** to switch to the input mode.

    *(Fig. B-83: Shows the "Product groups" dialog to allocate a Top PGR. A Product Group (A) is selected, and a checkbox for a Top product group (B) is ticked.)*

8.  Select the PGR (A) you want to allocate to the Top PGR.

9.  Tick the checkbox of the Top product group (B) you want to allocate.

10. Select in the menu **Start > Save** to save the data.
    The data will be saved.

## Exercises

*   Define a product group for training purposes.
*   Enter a PGR combination which is valid for all processing steps for laminated glass. Please remember:
    *   You have to define the PGR combination as a product group.
    *   You have to define the rule for the PGR combination.

## Production

### Objectives

*   Allocating the procurement type.
*   Allocating product-specific standard settings for production

### Benefit

*   Products are adopted for an order with their production-related settings. These details can be changed in the actual document.

### Note

| Term | Description |
| :--- | :--- |
| **Procurement type** | This code tells A+W Business how an order item shall be provided. <ul><li>All products which cannot be taken from stock have to be transferred to production so that they can be produced.</li><li>Products which are neither going to be produced nor taken from stock have to be purchased.</li></ul> |
| **Size allowance** | The size allowance compensates the loss of material resulting from the different processing steps. |
| **Size reduction** | A size reduction is called for if the lite is going to be cut to fit into a picture frame. |
| **Pattern** | Patterns can have a sense of pattern which has to be taken into account for cutting. The possible directions are entered in a basic table and have to be allocated to the patterned lites. |
| **Levels for patterns and coating** | For the production of IG units you have to define how the lites are to be fitted into the unit. Triple IG for example has six levels. These are always counted from the outside to the inside. |
| **Grill patterns** | Referring to the fields or drill positions, symmetrical or asymmetrical grills can entered. |
| **Grill types** | Grills are united in types which different criteria, e. g. the consecutive grill of a grid. |

## Production Settings

Depending on the product type and the product group, different entries are required for the transfer to production. The appropriate fields are accessible.

*(Fig. B-84: Product management - Production tab. The screen shows various settings including: (A) Edge quality, (B) BOM settings, (C) Different quantities for stock articles, (D) Spacer code, (E) Printing shape or grill sketches, (F) Details on patterns and coatings, and (G) Size allowances.)*

For complex products, the BOM can also be transferred to production (B). If the complete product is purchased however, the BOM will not be relevant for production. For simple (glass) products you have to define whether or not they can be used in the BOM. If a product includes edgework, the edge quality (A) must be allocated so that the right processing steps will be executed.

If the product includes grills or shapes, printing of the sketch (E) can be prevented. Printing of sketches is described in detail in a separate session.

⇨ Tutorial 2, "Printing sketches" on page B-479

## Size Allowances and Reductions

In some cases, size allowances or reductions have to be taken into account for cutting.
*   The size allowance compensates the loss of material resulting from the different processing steps.
*   A size reduction is called for if the lite is going to be cut to fit into a picture frame.

> **Example**
> By polishing all four edges, a float lite of 1000 x 1000 mm shrinks to a size of 998 x 998 mm.
> You have to enter a size surcharge of 2 mm. This value is taken from the allocated table, taking into account the glass thickness.

Size allowances and reductions are summed up in allowance or reduction tables. For every table, different values can be entered for the allowance or reduction, taking the glass thickness into account. Size allowances are allocated to the products of product type Processing.

*(Fig. B-85: Size allowances and reductions dialog. This screen shows the (A) Surcharge table: Master data and product management, with (B) Entries per glass thickness, and a reference to (C) Product edge processing.)*

## Patterns and Coating

Pattern, sense of pattern, coating types and levels are defined for production purposes. These can be selected in product management as well as in the order.

### Sense of pattern

For patterned lites, the sense (of pattern) has to be defined for cutting and assembly. The entry is allocated to the lite in product management.

*(Fig. B-86: Shows two images illustrating the sense of pattern. (A) shows a vertical pattern, (B) shows a horizontal pattern.)*

The sense of pattern can be:
*   **None:** This applies to all float glass lites.
*   **Vertical, horizontal:** The pattern runs vertically (A) or horizontally (B).
*   **Random:** If a pattern has no specific sense, both directions can be used.

### Coating type

Coating layers are applied in different degrees of hardness. The hardness is defined so that the appropriate cutting and processing tools - e.g. drills - can be used. The name can be chosen at random, e. g. soft, hard, without.

### Levels for the patterned and coated side

To define exactly how a lite shall be fitted into an IG unit, the different levels of an IG unit are defined. The unit is always seen from the outside (level 1) inwards (level 2).

*(Fig. B-87: A diagram showing the assembly levels for a quadruple IG unit, numbered 1 through 8.)*

### Cuts

You also need to define the direction of the cuts. If the sense of pattern does not matter, this task can be omitted to keep the waste at a minimum.

*(Fig. B-88: A diagram showing XYZ cuts on a stockplate.)*

## Grills

There are different types of grills, e. g. glass-dividing grills, fitted grills, grills inside the airspace (AIR). In A+W Business, grills are usually entered for the airspace, and are distinguished by pattern type.

All grills, connections, and edge connections have to be defined as products so that they can be entered in an order.

### Grill construction types

For the processing of lites with several fields, the type of the grill connection is defined in addition to the edge connections. The following patterns are defined by default:

| Pattern | Description |
| :---: | :--- |
| `+` (mitred) | Grill with double mitre at the intersection |
| `+` (blunt) | Cross grills, horizontal and vertical grills have blunt connections with the crosspieces. |
| `+` (vertical continuous) | Vertical grill continuous, horizontal grill with overreaching mitre. |
| `+` (horizontal continuous) | Horizontal continuous grill Vertical grill with overreaching mitre |
| `+` (vertical continuous, blunt) | Vertical grill continuous, horizontal grills with blunt connections to the vertical grills. |
| `+` (horizontal continuous, blunt) | Horizontal grill continuous, vertical grills have blunt connections to the horizontal ones. |
| (lines) | Horizontal and vertical grills continuous. |

*(Fig. B-89: Grill patterns)*

> **Define new grill types only if agreed**
> If you are using A+W Production, new grill types have to be agreed with A+W Software GmbH.

### Calculation type for grill construction

Referring to the fields or drill positions, symmetrical or asymmetrical grills can entered.
*   You can enter individual sizes for grill construction so that drill holes or fields are arranged asymmetrically.
*   In case of automatic calculation you can define whether the symmetry shall be related to the drill holes or to the fields.

> **Example**
> An edge length of 1000 mm and a grill width of 26 mm will produce the following values (without cutback):
> *   **Drill-hole symmetrical:** The drill holes are each 333.3 mm away from the edges. The edge length of the outer fields is 307.3 mm while the central field has an edge length of 320.2 mm.
> *   **Field-symmetrical:** The drill holes are 329.0 mm away from the edges, with a central distance of 342.0 mm. The edge length of the three fields is 316.0 mm.
>
> *(Fig. B-90: Symmetrical calculation of grill pattern. Two diagrams show "Drill hole-symmetrical" and "Field-symmetrical" layouts.)*

### Spacer code

The spacer codes are passed on at transfer to production. The codes have to be agreed with A+W Production.
The spacer code in the variant can overrule the code defined in product master data.

## Prices and Surcharges

### Objectives

*   Defining the price-relevance of products.

### Benefit

*   Price and tax codes serve to calculate order items.

### Note

| Term | Description |
| :--- | :--- |
| **Price view** | <ul><li>**Implicit:** The main item's net price includes all prices of the BOM elements; i.e. shape and exchange surcharges as well as processing. Other surcharges are implicit only, i.e. they do not appear on the order.</li><li>**Explicit:** The prices of the BOM elements are listed separately.</li><li>**Implicit, price per quantity unit:** The price of the BOM elements are converted to the main product's price unit. This total price is shown in the document but only if all BOM elements of the item have been allocated the same display type.</li></ul> |
| **Adopt main item** | Calculation and display of prices depends on the details entered for the main item. There are various ways of adopting discounts and prices. |
| **Pricing codes** | Prices, discounts, and cash discounts can only be calculated if permitted for the product. |

## Price Parameters

This tab serves to allocate price tables and surcharges and to define how the prices are to be displayed.

*(Fig. B-91: Product management - Price/Surcharge tab. This screen shows various settings, including (A) Tax rate, (B) Automatic Surcharges, (C) Cost accounting details, (D) Price view, (E) Price tables, (F) Surcharges, (G) Rounding for pricing purposes, and (H) Price code.)*

You have to enter the tax rate (A) for every product. If you are using cost accounting, you can also enter the cost type and the cost center.

You can also calculate automatic surcharges (B), e.g. an energy surcharge or surcharges for the exchange of BOM elements (F).

A product can be calculated for sales and purchasing only if the appropriate codes (H) have been set and if the corresponding price tables (E) have been defined.

Surcharges and prices are described in detail in separate sessions.

### Price View

For every product you can define the way in which prices are displayed. Product management offers the following options for this purpose:

*   **Price view:**
    *   **Implicit:** The main item's net price includes all prices of the BOM elements; i.e. shape and exchange surcharges as well as processing. Other surcharges are implicit only, i.e. they do not appear on the order.
    *   **Explicit:** The prices of the BOM elements are listed separately.
    *   **Implicit, price per quantity unit:** The price of the BOM elements are converted to the main product's price unit. This total price is shown in the document but only if all BOM elements of the item have been allocated the same display type.

> **Price view - an example**
> The section Prices offers a detailed example of the display of prices.
>
> ⇨ "Example of how Prices are Shown in the Document" on page B-218

### Adopt Main Item

If the product is included in a bill of material, calculation and display of the prices and discounts can depend on the settings which have been made for the product of the main item. The following settings are possible:

*   **No adoption:** The price settings will not be adopted from the main item.
*   **Discount + price key:** Discount and price key will be adopted from the main item.
*   **Discount:** Only the discount will be adopted from the main item.
*   **Price key:** Only the price key will be adopted from the main item.
*   **No adoption (net for ind.pr.main itm):** For customised net prices, the settings shall not be adopted from the main item.
*   **Discount + price key (net for ind.pr.main itm):** For customised net prices, the discount and price key shall be adopted.
*   **Discount (net for Ind.pr.main itm):** For customised net prices, only the discount will be adopted.
*   **Price key (net for ind.pr.main itm):** For customized net prices, only the price key shall be adopted from the main item.
*   **Discount + price key (even if discount exists):** Discount and price key will be adopted from the main item even if a discount has been defined for the BOM product, e. g. when a lite is replaced.
*   **Discount (even if discount exists):** The discount shall be adopted from the main item even if a discount has been defined for the BOM product, e. g. when a lite is replaced.
*   **Price key (even if discount exists):** The price key shall be adopted from the main item even if a discount has been defined for the BOM product, e. g. when a lite is replaced.

Prices and discounts are described in detail in separate sessions.

> **Settings for pricing in company data**
> Dialog **Company data > tab Pricing** serves to make general settings which can partially override the settings in product master data.

### Pricing Codes

Prices, surcharges, and discounts are calculated only for products of BOM elements for which the corresponding codes have been set:
*   Price-relevant for sales (SP)
*   Price-relevant for purchasing (PP)
*   Discountable
*   Cash discountable

*(Fig. B-92: Shows checkboxes for `Price relevant SP`, `Price relevant PP`, `Discountable`, and `Cash discountable`.)*

A product is price-relevant if it has its own sales price which is used for pricing. For products with a BOM, this can refer to the main product or to the individual elements.

This means that you either enter a price for the product, or calculate it in connection with an order, based on the BOM elements.

> **Example**
> A door consists of a toughened lite with fittings at the bottom corners, and a brass bearing. A price table has been created for this product according to which the door shall cost 200.00 €. It is therefore price-relevant. This code is disabled for the individual BOM elements however.
>
> The BOM would be price-relevant if the individual BOM elements were price-relevant. The price would be calculated in the order.
>
> If all BOM elements were price-relevant in addition to the main product, the price would be calculated as follows:
>
> *   Price for the complete door
> *   + price for a toughened lite
> *   + price for bottom fittings
> *   + price for brass bearing

If the code is not set, A+W Business considers the product irrelevant for pricing even if a price table has been allocated. If a product is irrelevant for pricing, no price will be shown at order entry, and no price can be entered by hand either.

If the prices for exchange lites in IG units are calculated by means of exchange surcharges, the code price-relevant has no effect. The price setting for the main item has to be obeyed however. This setting will be dealt with in the session on exchange discounts.

## Stock and Purchasing

### Objectives

*   Distinguishing procurement types.
*   Introducing the settings for stock management
*   Introducing the settings for purchasing

### Benefit

Settings for stock management and purchasing serve the provision or replacement of products. The settings will be adopted for the documents and can be amended if necessary.

### Note

| Term | Description |
| :--- | :--- |
| **Procurement type** | The procurement type defines how the product is to be acquired for this order, e.g. production, stock withdrawal, purchasing. |
| **Maximum sizes for purchasing** | The sizes will be checked at document entry. |
| **Stock booking type** | The stock booking type defines how a product is kept as a stock article in stock management: |
| **Alternative product codes (for the procurement type)** | The supply type for different clients and/or order areas can differ from the supply type defined in product master data. |

## Stock Settings

This tab serves to define the parameters for purchasing and stockkeeping of the product.

*(Fig. B-93: Product management - Stock / Purchasing tab. This screen shows (A) Purchase sizes, (B) Procurement type, and (C) an area for Different product codes.)*

Products can be produced or purchased. The procurement type (B) defines how the product has to be procured for the order in question.

### Procurement Type

Product master data define how the product is going to be procured for the order:
*   **Production:** The order item will be produced in-house. If a main article has got this procurement type, its BOM elements can be defined as stock articles or as purchased articles.
*   **Cutting:** The glass for this order item is cut from stock sizes. The sizes are then transferred to production.
*   **Stock withdrawal:** The product is kept in the stock as a stock article in sqm or as a stock dimension with its dimensions in the case of glass articles. Other products are kept in stock in their quantity unit. The defined quantity will be reserved at order entry. This procurement type is a prerequisite for stock management in the stock module.
*   **Processing:** The processing steps for an order item are transferred to production.
*   **Customer's own glass:** The product is supplied by the customer and will be used to produce his orders.
*   **P.O.:** Only the product in question will be ordered, irrespective of the contents of the BOM acc. to the order. If a laminated lite consists of a float lite, a film, and a toughened lite for instance and only the toughened lite is marked as P.O., only the toughened lite will be ordered from the supplier. The laminated lite will be produced in-house.
*   **P.O. (complete):** The product is ordered, including all processing steps defined in the BOM of this order. If a laminated lite consists of a float lite of 5 mm, a film layer, and a 5 mm toughened lite, the entire laminated lite will be ordered. Please note the difference from the code P.O.
*   **Addition to stock through production:** The product shall be used in work orders only to fill up the stock. The produced items will be added to stock.

The code Procurement type is adopted from product master data for the order item. In the order, every single item can be allocated a different procurement code.

### Stock Booking Type

The stock booking type defines how a product is kept as a stock article in stock management:
*   **Size-dependent:** Choose this setting if stock sizes are to be kept as units. This setting makes sense only for glass. The quantity unit should still be set to sqm on tab Product to make sure that the surface is calculated.
*   **Not size-dependent:** Choose this setting for all stock articles to be kept with their actual quantity unit, e.g. units, fittings. Use this setting also for glass which is to be kept in sqm.
*   **Combined:** Choose this setting if you are using reports from the shop floor. This setting makes sense only for glass. Please remember to define a virtual stocksize without sizes for this purpose.

The setting w/o will not be used in this context.
Stock bookings are described in detail in section Stock management.

### Different Product Codes

If you are using clients and order areas, you can define procurement types for the individual products or product groups which differ from the entries made in product master data.

> **Example**
> The order areas IG, toughened glass, and laminated glass user internal orders. All order areas use the same database, the same master data, etc.
> An order is entered in the IG area; the IG unit consists of a laminated lite with toughened glass, a spacer, and a float lite.
> *   For order area IG, the IG unit is Production, the laminated lite is Purchased while the float lite is Cut.
> *   For order area laminated glass, the laminated lite is Production, the toughened lite is Purchased, and the float lite is also Cut.
> *   For order area toughened glass, the toughened lite is Production, and the float lite is Cut.
>
> The different supply types for laminated glass and toughened glass thus have to be defined by different product codes.

*(Fig. B-94: Product code management dialog. This screen allows setting different procurement types based on Area, Client, or Order area.)*

## Shapes and Bills of Material

### Objectives

*   Introducing the display of shapes.
*   Creating bills of materials for complex products.

### Benefit

*   Standard product structures are described by bills of materials and can be saved in master data.
*   Pricing and production are based on bills of materials.

### Note

| Term | Description |
| :--- | :--- |
| **Shape** | Shapes are usually standard shapes with a non-rectangular geometry. |
| **Shape catalog** | The shape catalog is predefined. Products are entered based on these settings. |
| **Bill of Material (BOM)** | A bill of materials describes the product structure. It consists of individual elements. |
| **BOM element** | Every BOM element is a product itself. BOM elements can be individual products as well as processing steps or further bills of material, so-called assemblies. |
| **Price- or production relevant** | A+W Business distinguishes price-relevant and production-relevant BOM elements. <ul><li>A price-relevant element is directly linked with the main product.</li><li>A production-relevant element (the processing step) is linked with the glass.</li></ul> |
| **Main product** | The main product is the basis of a bill of materials. A bill of material is always attached to a main product. It can be linked with properties which apply to the whole (complex) product. |
| **Production BOM breakdown** | The production BOM breakdown defines the processings which shall or must not be applied to the main product but to the corresponding BOM element. |
| **Transmission** | Modifications of BOM elements can be passed on to other elements. <ul><li>Sizes are passed on to the various BOM elements (size transfer)</li><li>In case of surcharges, either the basic item or the so-called parent product will be taken into account.</li></ul> |
| **Parent product** | A parent product is the basic product of an assembly, e.g. the laminated glass lite which is fitted as an assembly into an IG unit. |
| **Basic item** | The basic item is the top level of the bill of material. |
