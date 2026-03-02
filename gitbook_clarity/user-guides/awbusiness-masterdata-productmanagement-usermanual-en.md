---
description: "EN-UM-AWBusiness_3"
---


# Tutorial 1: Product data

---
## Product

### Objectives
- Knowing the use of products.
- Introducing product types, product groups.
- Introducing the product organization in product groups.
- Introducing the function of combined and top product groups.

### Benefit
- Products are the basis for order and P.O. items and for sales and purchase price calculation.
- The entire product structure can be described by means of product master data.

### Note

**Product**
Products are the basis for price and cost calculation, purchasing, materials and time management, technical checks, etc.

**Product Types**
Product types are the basis for products. Product types are not only glass or glass types, but also shapes, processing steps, surcharges, etc. which are entered like products in the order.

**Product groups**
Product types are split into product groups. Product types and groups unite the products for transfer to production and for internal program purposes.

**Product groups**
All products are allocated to product groups. Product groups and the combinations thereof are the core of pricing, e.g. for calculating discounts and surcharges. The product group hierarchy is:
- MPG: main product group
- SPG: product super group
- PGR: product group

**PGR combination**
Product groups can be combined. These product group combinations serve for discount calculation and analysis.

**Top product groups**
Top product groups are analyzed in connection with the creation of sales statistics.

**Quantity unit**
The necessary sizes for describing a product have to be defined per product. This is usually done by means of the quantity unit.

### Product Types and Product Groups

Product types are the basis for products. Product types are not only glass or glass types, but also shapes, processing steps, surcharges, etc. which are entered like products in the order.

Product types are split into product groups. Product types and groups collect the products for transfer to production and for program-internal purposes, e.g. the preselection at order item input.

| Product type | Product groups | Product |
| :--- | :--- | :--- |
| Single annealed | Single annealed, Patterned glass | Float 6 mm, Patt. Ald. Glastt 4 mm, Patt. Cathed. white 4 mm |
| IG | IG, Triple IG | CLIMALIT Standard 2x4, CLIMASOL silver 53/39 |
| Tempered glass | Tempered glass, Glass door system | Toughened clear 12 mm, Toughened door white |
| Shapes | Shapes, Steps | Standard shape 1 - 135, Shape 999 |
| Spacer | Alu, Steel, TPS | 12 mm, 16 mm |
| Services | Down payment, Surcharges, UV edge connection | Down payment, Rush surcharge |
| Processing steps | Rounded corners, Edge cut-out | Rounded corner, fine, Rounded corner, rough, Edge cut-out - 100 x 200 mm |

Each product is allocated to a product group and thus, to a product type.

**(Fig. B-76 Product organisation, example: spacer)**

This example shows that various product groups have been allocated to product type Spacer. Product group Alu unites the spacers with different sizes.
- **A Product Types**: Shows a list of product types, including "Abstandhalter / Spacer".
- **B Product groups of the product type spacer**: Shows product groups for the "Spacer" type, including "Alu", "Stahl / Steel", etc.
- **C Products of the product group ALU**: Shows specific products within the "Alu" group, such as "Spacer 6 mm ALU A+W", "Spacer 8 mm ALU A+W", etc., with different sizes.

> **New product types or product groups**
> Product types are preset in A+W Business. You can define or change product groups but without any effect within the system. Should you need more product groups or types please contact A+W Software GmbH.

## Product Groups

All products are generally allocated to product groups. Product groups and the combinations thereof are the core of pricing, e.g. for calculating discounts and surcharges. Top product groups can be defined for sales statistics.

### Product groups 0xx

Each product group is marked by a three-digit, alpha-numerical code which represents the hierarchy level:

**(Fig. B-77 Hierarchic product group structure)**
- **A MPG: main product group**: Top-level group, e.g., `1** Iso/IG`.
- **B SPG: product super group**: Mid-level group, e.g., `20* Float klar / clear`.
- **C PGR: product group**: Lowest-level group where products are allocated, e.g., `200 Float 2-10 mm FM/CTS`.
- **D MPG with alpha-numerical number**: Example of an alphanumeric main product group, e.g., `B** Bearbeitung / Processings`.

The main product group 0**, super product group 00*, and product group 000 are fixed. All other product groups can be numbered according to your own rules.

- The main product group (MPG) serves for discount allocation and statistical analysis. Example MPG 1**.
- If more than 10 MPG (0** to 9**) are required you can also use letters for numbering, e.g. A**.
- The super product group (SPG) serves for discount allocation and statistical analysis. Example SPG 10*.
- The product group (PGR) serves for discount allocation, product organisation, and statistics. Products can be allocated only to this level. Example PGR 105.

> **Hint for product group allocation**
> Product group 000 usually only includes shapes. This way, the shape sales can be automatically allocated to the sales of the main product in statistics for example.
> Grills and processing steps usually have their own product groups.

### Product group hierarchy for analysis

For more sophisticated sales statistics, you can define your own product group combinations, e.g. for the different IG units including shapes. Shapes are allocated to single annealed or to IG, to be analysed together.
- **Top product group (top PGG)**, e.g. grills.
  Relevant for statistics.
- **Main product group (MPG)**, e.g. 1**.
  Relevant for discounts and statistics.
- **Super product group (SPG)**, e. g. 10*.
  Relevant for discounts and statistics.
- **Product group (PGR)**, e.g. 105.
  Relevant for discounts. Only the product group can be allocated to a product.

Section Statistics describes how product groups are analysed for statistics.

### PGR Combination

Product groups can be combined. Product group combinations (PGR combinations) serve for discount calculation and analysis, e.g. to show the sales for IG units in different structures.

> **Examples**
> PGR combinations for sales statistics are useful for the following analyses:
> - IG (without anything)
> - IG with shape
> - IG with grills
> - IG with shape and grills
> - LG with processing
> - LG with shape and processing

Every combination of product groups results in a so-called PGR combination. This is not automatically created by combining the product groups but, like any other PGR, has to be specially defined.

Every combination can be created just once even if you choose another number for the PGR combination.

**(Fig. B-78 Definition of PGR combinations)**
The image displays a user interface for defining PGR combinations.
- **A Product groups which have been combined**: Shows the original product groups being combined, e.g., Product group 1 `1**` and Product group 2 `95*`.
- **B Number of the PGR combination**: Shows the resulting combination number, e.g., `19>`.
- **C Details on the use**: Checkboxes to define the purpose of the combination, such as "Valid for discount determ." and "Valid for statistics".

When defining PGR combinations you can define whether the combination shall be used for discount calculation or for statistics. You can also define e.g. whether only the main product shall be analysed when searching for a discount, or all products of the BOM.

### Rules for PGR Combinations

You have to stick to certain rules when creating PGR combinations. The following rules are explained by means of examples:
- Combination rules for number allocation
- Combination rules for follow-up processing
- Create PGR combinations with full BOM

#### Combination rules for number allocation
Generally, a PGR combination gets a unique number. Allocation of numbers can also be controlled by wildcards so that products are allocated automatically. The symbols `<` for left and `>` for right are used as wildcards.

**(Fig. B-79 Example of a PGR combination)**
This example shows a combination of PGR `1**` and PGR `9*` to form PGR combination `19>` (A). The symbol `>` means that the third position of PGR `19*` shall be addressed.
When an IG unit (PGR `1**`) is combined with Breakage (D), a discount (B) shall be applied. Since no discount will have been defined for breakage, the discount will only be calculated for the IG unit. This is why the checkbox for the main item does not have to be checked. The combination (IG and breakage) shall be analysed statistically as part of the statistics for IG (C).

#### Examples of different combinations

| Definition | Example | PGR | Description |
| :--- | :--- | :--- | :--- |
| **PGR 1:** 10\*, **PGR 2:** 81\* | **PGR 1:** 101, **PGR 2:** 814 | **PGR comb.:** 1G<, **Result:** 1G1 | The last number of PGR 1 is allocated. The last number of PGR 1 is 1, hence 1G1. The valid product group combinations 1G0-1G9 have to be defined as PGRs. |
| **PGR 1:** 10\*, **PGR 2:** 81\* | **PGR 1:** 101, **PGR 2:** 814 | **PGR comb.:** 1G>, **Result:** 1G4 | The last number of PGR 2 is allocated. The last number of PGR 2 is 4, hence 1G4. The valid product group combinations 1G0-1G5 have to be defined as PGRs. |
| **PGR 1:** 22\*, **PGR 2:** 766 | **PGR 1:** 224, **PGR 2:** 766 | **PGR comb.:** 966, **Result:** 966 | Fixed setting. The PGR combination is always 966. The product group combination 966 has to be defined as PGR. |
| **PGR 1:** 3\*\*, **PGR 2:** 19\* | **PGR 1:** 376, **PGR 2:** 195 | **PGR comb.:** 4<<, **Result:** 476 | The second and third number of PGR 1 are allocated. The last numbers of PGR 1 are 7 and 6, hence 476. The valid product group combinations 400-487 have to be defined as PGRs. |
| **PGR 1:** 3\*\*, **PGR 2:** 19\* | **PGR 1:** 376, **PGR 2:** 195 | **PGR comb.:** 4>>, **Result:** 495 | The last two numbers of PGR 2 are allocated. The last numbers of PGR 2 are 9 and 5, hence 495. The valid product group combinations 400-499 have to be defined as PGRs. |

#### Explanations of the examples

For the first of the above examples:
- PGR 10* includes PGR 100-109, 10A-10Z, 10a-10z, e.g. for IG units.
- PGR 81* includes PGR 810-815, e.g. for grills.

To be able to analyse IG units with grills in statistics, PGR 10 and PGR 81 shall be combined. The result is the PGR combination number 1G<.

Symbol `<` represents product group 1. It stands in third place and therefore refers to the third digit of PGR 1.

For PGR combinations 101 and 814, 1G< is 1G1. This means that the analysis of the combination is part of PGR 1G1.

The other examples are constructed in the same way.

This rule can also be applied to the second and even the first digit. This will result in a large number of combinations and is therefore prone to errors.

It is essential to define all product groups that can be created by a PGR combination. For the first example, these are PGR 1G0 to 1G9.

#### Combination rules for follow-up processing
The production of an order item can include several steps, e.g. an IG unit with grills and a shape.
If all elements of such a BOM shall be included in a PGR combination, the following combination rules apply:

| PGR 1 | PGR 2 | PGR combination | Description |
| :--- | :--- | :--- | :--- |
| **Definition:** 12\* | **Definition:** 5\*\* | A2A | PGR A2A applies in general. |
| **Example:** 121 IG | **Example:** 502 Grills | A2A | IG + grill becomes A2A. |
| **Definition:** A2A | **Definition:** 5\*\* | A2A | PGR A2A applies in general. |
| **Example:** A2A (IG + grill) | **Example:** 540 Shape | A2A | IG + grill + shape becomes A2A. |

If no appropriate follow-up combination (A2A + 5** = A2A) has been defined, the original PGR defined for the processing step will be used (540).

#### Create PGR combinations with full BOM
To describe PGR combinations with a complete BOM you have to define in company data whether the entire BOM shall be checked for discounts for a PGR combination. This setting applies to all PGR combinations.
⇨ Software Reference, "Create PGR combinations using complete BOM" on page B-972

### Combination examples for product groups with BOM

| PGR | Name (examples) |
| :-- | :--- |
| 100 | Float 4 mm |
| 101 | Float 4 mm, edges polished |
| 102 | Float 4 mm, drill hole |
| 103 | Float 4 mm, edges polished and drill hole |
| 400 | Bevelling |
| 600 | Edge polishing |
| 800 | Drilled hole |

| PGR 1 | + PGR 2 | PGR combination | Name |
| :-- | :--- | :--- | :--- |
| 100 | 600 | 101 | Float 4 mm, edges polished |
| 100 | 800 | 102 | Float 4 mm, drill hole |
| 101 | 800 | 103 | Float 4 mm, edges polished and drill hole |
| 102 | 600 | 103 | Float 4 mm, edges polished and drill hole |

Depending on the settings in *Company data*, the product group combination for this product will be used, or all BOM elements are booked to the last combination found in this item.

| Product | PGR 1 | + PGR 2 | Checkbox Create PGR combination with complete BOM (unchecked) | Checkbox Create PGR combination with complete BOM (checked ☑) |
| :--- | :--- | :--- | :--- | :--- |
| Float 4 mm | 100 | 600 | 101 | 103 |
| + edges polished | | | | |
| + bevelling | 400 | - | 400 | 103 |
| + drill hole | 800 | 101 | 103 | 103 |

This example shows the product groups which are booked if checkbox *Create PGR combination with complete BOM* is checked or unticked in company data.

### Top PGR

Any product group (PGR) can be allocated to a top PGR. These are used for special analysis in sales statistics.

> **Example**
> A top PGR for grills makes sense if in statistics, all grills are allocated to the various IG structures by means of PGR combinations. This tells you how many grills have been produced per standard IG or per heat protection IG. Grills or IG units alone can only be analysed by means of the top PGR. This tells you how many grills have been produced per standard IG or per heat protection IG.
> If you allocate the top PGR grills to all product groups which include grills, sales statistics provides a general overview of all grills produced.

Top PGRs are not defined like product groups but in a basic table.

> **Allocate top PGR**
> Only third level product groups can be allocated to a top product group.

### Size and Quantity Units

Apart from the structural description of a product (BOM), pricing requires quantity units to which the price refers. Units have to be defined for every product. The units are fixed.

The necessary sizes for describing a product have to be defined in master data for every product. This is usually done by means of the quantity unit:
- **Piece:** The quantity unit Piece is e.g. used for products like handles, felt pads, etc.
- **Volume:** The quantity unit Liter is used for gas. The quantity (= liters) is checked in the order.
- **Time:** The quantity unit Hours is used for special services or processing steps. The quantity (= number of hours) per item is checked in the order.
- **Linear meters:** The quantity unit Linear meters is used for the length (per meter) of grills, edgework, etc. The quantity and the length per item are checked in the order.
- **Surface:** The quantity unit Surface defines the total surface in sqm (width x height) of plates or lites. Quantity, width, and height of an item are checked at order entry.

#### Size calculation
Formulas and variables can be used for calculating sizes. The following variables have a fixed meaning and cannot be changed:
- `$1` = width
- `$2` = height
- `$3` = AIR1 (airspace 1) or depth
- `$4` = AIR2 (airspace 2, for triple IG)

> **Available variables**
> Tutorial 2 offers a list of available variables and wildcards that can be used in formulas.
> ⇨ Tutorial 2, "Available variables (wildcards)" on page B-597

The sizes are rounded for pricing. German pricing is based on rounding to thirty. This means that calculation is based on the next edge length that can be divided by 30.

> **Example**
> Rounding 30:
> For a lite of 1000 x 1000 mm, a surface of 1.04 (= 1020 x 1020) will be calculated.
> The lite will be cut to a size of 1000 x 1000 mm however.

Other countries use other rounded sizes; France for example uses a rounding of 10.

Rounded sizes are used in the following areas:
- **Product**
  ⇨ Software Reference, "Product Management – Price/Surcharge" on page B-678
- **Price list**
  ⇨ Software Reference, "Price Management" on page B-768
- **Customer and supplier master data**
  ⇨ Software Reference, "Partner Management - Order" on page B-813

If A+W Business finds details on rounded sizes in several areas, the following hierarchy applies: Partners > Products > Prices > Discounts > Unit prices. The entry for unit prices overrides all others.

## Product Group Definition

Product groups (PGR) are used for the clear structuring of products, for quick input of articles, allocation of discounts and surcharges, and for statistical analysis. Budgets, commissions, and proceeds accounts are calculated on the basis of product groups.

Product groups only defined for statistical purposes are useful too.

> **Define MPG, PSG, or PGR**
> Main product groups (X**), product super groups (XX*), and product groups (XXX) are defined in the same way.

### How to define a product group
1. Go to **Master data > Products > General > PGR**.
   Dialog *Product groups* pops up.
   ⇨ Software Reference, "PGR" on page B-644
2. Go to the menu **Start > New** to switch to the input mode.
   **(Fig. B-80 Fields for the new product group are accessible)**
   The screen shows the product group tree on the left (A) and input fields on the right for the new product group number (B) and name (C).
3. Enter the number (B) and name (C) of the product group.
4. Leave the fields **Prep. days** and **Special surcharge** blank. You can fill them in later.
5. Select in the menu **Start > Save** to save the data.
   The new product group will be saved.
6. If necessary, select an icon (A) if the new product group shall not keep the bitmap of the superior product group.
7. Select in the menu **Start > Save** to save the data.
   The data will be saved.

### Combine Product Groups

You can use wildcards instead of numbers when you define combination product groups. Please read the examples for combination rules carefully before entering a PGR combination.
⇨ "Rules for PGR Combinations" on page B-206

> **Sequence for defining product group combinations**
> Every combination of product groups results in a so-called PGR combination. This is not automatically created by combining the product groups, but has to be specially defined. First define the product groups which can result from PGR combinations. Only then can you select the PGR combination in the following steps.

#### How to combine product groups
1. Go to menu **Master data > Products > General > PGR combinations**.
   Dialog *PGR combinations* appears.
2. Go to the menu **Start > New** to switch to the input mode.
   **(Fig. B-81 Fields for the PGR combination are accessible)**
   The screen shows fields for defining a combination.
   - **A PGR 1 (main product)**
   - **B PGR 2 (BOM element)**
   - **C Number of the PGR combination**
   - **D Settings for the application**
   ⇨ Software Reference, "Combined PGR" on page B-647
   The released fields are preset by the values of the selected PGR combination.
3. Select product groups 1 (A) and 2 (B).
4. Enter the number of the PGR combination (C).
   Please obey the rules for wildcards should you want to use them. PGR combinations will not be created automatically when you enter a new number. You will have to create these new PGR combinations later in dialog PGR.
5. Check the required checkboxes (D) for the validity of the PGR combination.
   The checkboxes for editing discount combinations are accessible after you have checked the checkboxes for the validity.
6. Select in the menu **Start > Save** to save the data.
   The data will be saved.

> **Check the settings for PGR combinations**
> Please take into account the settings for product group combinations in company data.
> ⇨ Software Reference, "PGR combination for discounts valid only if discount exists" on page B-972
> ⇨ Software Reference, "Create PGR combinations using complete BOM" on page B-972

### Definition and allocation of Top PGR
To allocate a Top PGR, perform the following steps:
- Create the Top PGR.
- Allocate the PGR.

#### How to set up a Top PGR for analysis
1. Go to **Master data > Products > General > Top PGR**.
   Dialog *Top PGR* appears.
2. Go to the menu **Start > New** to switch to the input mode.
   The next line is accessible now.
3. Enter the name.
   **(Fig. B-82 Create the Top PGR)**
   ⇨ Software Reference, "Top PGR" on page B-649
4. Select in the menu **Start > Save** to save the data.
   The data will be saved.
5. Close the dialog *Top PGR*.
6. Go to menu **Master data > Products > General > PGR**.
   Dialog *Product groups* pops up.
   ⇨ Software Reference, "PGR" on page B-644
7. Go to the menu **Start > New** to switch to the input mode.
8. Select the PGR (A) you want to allocate to the Top PGR.
9. Check the checkbox of the Top product group (B) you want to allocate.
10. Select in the menu **Start > Save** to save the data.
    The data will be saved.
    **(Fig. B-83 Allocate top PGR)**
    The image shows the Product Group (A) `S11 Wiener Srosse...` being allocated to the Top PGR (B) `TOP 01 - Sprossen / Bars`.

## Exercises

- Define a product group for training purposes.
- Enter a PGR combination which is valid for all processing steps for laminated glass. Please remember:
  - You have to define the PGR combination as a product group.
  - You have to define the rule for the PGR combination.

## ITOE

With the iTOE module, there is a synchronization of the processings between the A+W CAD Designer (Shapes) and the A+W Business.

During the import of the DXF files from the A+W CAD Designer (Shapes), there is an immediate takeover of the processings into the order entry. The advantage of the iTOE is that this way, no more doubled entries of the processings are required.

> **Prerequisite**
> The iTOE module, which requires a license, assumes the database system Microsoft SQL Server 2016. Contact A+W Software GmbH if you want to use the module.

In the beginning, master data is not absolutely required since the module works with self-learning. The master data consists of rules with which it is specified which article should be transferred to the BOM during the comparison. After each import, the articles that correspond to no rules are displayed and they can be created there during the comparison and also changed.

### Creating rules
The rules can either be created at the beginning in the iTOE rules dialog (Master Data > Products > Articles > ITOE rules) or defined during the import. The rules are processed in the sequence of the specified priority.

### iTOE rules
You can reach the dialog for creating the rules via:
**Master Data > Products > Product > ITOE Rules**

**(Fig. B-84 iTOE rules)**
The dialog shows fields for defining iTOE rules, including Priority, SN Processing type, Product Type, Diameter range, and a list of existing rules.
For a detailed description of the fields of this dialog, see:
⇨ Software Reference, “ITOE Rules" on page B-722

### Product comparison
In the processing entry, the product comparison can be started either with a DXF file import or with the [iTOE] button on the ribbon. If you have made the changes to the glass unit in the A+W CAD Designer (Shapes), you take over the changed data with the **File > Save with file** or **File > Save without file** menu element.

**Save with file** means that an SN file (iTOE file) should be created in the BOM. With **Save without file**, no file is created.

If a iTOE file is created, the product comparison independently inserts a shape set (if it does not exist yet) and links the iTOE file created. You can recognize the iTOE files from their file names in the form XXXX_TOE.SN. Whereby the number at the front is determined by the number ranges of the SN files.

As soon as the changes have been applied, A+W Business displays the result of the rule check on a dialog.

**(Fig. B-85 Result of the product comparison)**
If a product was found for each processing, it will be displayed as in the example above. If for a processing no rules applies, you can see this from the line with the dark background and from the fact that the article number (field Product) is missing. Now, using the [...] button in the **Edit rule/Insert rule** field, you can change directly to the iTOE Rules dialog and create the appropriate rule. You can also change already-created rules with this button. After you exit the iTOE rules, there is always a new comparison and the changes you just made to the rules display their effects immediately.

If you confirm the result of the product comparison, the complete BOM is generated in the processing entry and provided with the appropriate prices. The system compares changes that are now made in the processing entry with the TOE file.

> **Property of CAD processing**
> Changes to properties that are not a component of the A+W processing type catalog are lost during comparison; that is, a drilling hole sequence with series dimensioning: The series dimensioning is deleted as soon as one of the participating drillings is changed in the processing entry. Such changes have to be made in A+W CAD Designer.

### Restrictions and configuration
For processings that have an edge quality (drillings, cut-outs), during the DXF import, the edge quality must always be defined on the import dialog; the iTOE rule must consider the edge quality and then select the product that corresponds to the edge quality. In A+W Business, the edge quality is not saved in the order; instead, it always comes from the base product. If no quality is defined, the one from the master data processing is always used.

## Production

### Objectives
- Allocating the procurement type.
- Allocating product-specific standard settings for production

### Benefit
- Products are adopted for an order with their production-related settings. These details can be changed in the actual document.

### Note

**Procurement type**
This code tells A+W Business how an order item shall be provided.
- All products which cannot be taken from stock have to be transferred to production so that they can be produced.
- Products which are neither going to be produced nor taken from stock have to be purchased.

**Size allowance**
The size allowance compensates the loss of material resulting from the different processing steps.

**Size reduction**
A size reduction is called for if the lite is going to be cut to fit into a picture frame.

**Pattern**
Patterns can have a sense of pattern which has to be taken into account for cutting. The possible directions are entered in a basic table and have to be allocated to the patterned lites.

**Levels for patterns and coating**
For the production of IG units you have to define how the lites are to be fitted into the unit. Triple IG for example has six levels. These are always counted from the outside to the inside.

**Grill patterns**
Referring to the fields or drill positions, symmetrical or asymmetrical grills can entered.

**Grill types**
Grills are united in types which different criteria, e.g. the consecutive grill of a grid.

### Production Settings
Depending on the product type and the product group, different entries are required for the transfer to production. The appropriate fields are accessible.

**(Fig. B-86 Product management - Production)**
The image shows the production settings tab for a product. Key fields are:
- **A Edge quality**: Defines the quality for edgework.
- **B BOM settings**: Options like "BOM not relevant for production" and "Suitable for IG".
- **C Different quantities for stock articles**: Settings for sub/excess quantity.
- **D Spacer code**: Code for spacer type.
- **E Printing shape or grill sketches**: Options for printing sketches.
- **F Details on patterns and coatings**: Defines pattern sense and coating type.
- **G Size allowances**: Width and height allowances.

For complex products, the BOM can also be transferred to production (B). If the complete product is purchased however, the BOM will not be relevant for production. For simple (glass) products you have to define whether or not they can be used in the BOM. If a product includes edgework, the edge quality (A) must be allocated so that the right processing steps will be executed.

If the product includes grills or shapes, printing of the sketch (E) can be prevented. Printing of sketches is described in detail in a separate session.
⇨ Tutorial 2, "Printing sketches" on page B-552

### Size Allowances and Reductions
In some cases, size allowances or reductions have to be taken into account for cutting.

- The size allowance compensates the loss of material resulting from the different processing steps.
- A size reduction is called for if the lite is going to be cut to fit into a picture frame.

> **Example**
> By polishing all four edges, a float lite of 1000 x 1000 mm shrinks to a size of 998 x 998 mm.
> You have to enter a size surcharge of 2 mm. This value is taken from the allocated table, taking into account the glass thickness.

Size allowances and reductions are summed up in allowance or reduction tables. For every table, different values can be entered for the allowance or reduction, taking the glass thickness into account. Size allowances are allocated to the products of product type Processing.

**(Fig. B-87 Size allowances and reductions)**
- **A Surcharge table**: Master data and product management for surcharge tables.
- **B Entries per glass thickness**: A table showing different surcharge values based on glass thickness.
- **C Product edge processing**: The product setting where the surcharge table is applied.

### Patterns and Coating
Pattern, sense of pattern, coating types and levels are defined for production purposes. These can be selected in product management as well as in the order.

#### Sense of pattern
For patterned lites, the sense (of pattern) has to be defined for cutting and assembly. The entry is allocated to the lite in product management.

**(Fig. B-88 Sense of pattern)**
- **A**: Vertical pattern
- **B**: Horizontal pattern

The sense of pattern can be:
- **None:** This applies to all float glass lites.
- **Vertical, horizontal:** The pattern runs vertically (A) or horizontally (B).
- **Random:** If a pattern has no specific sense, both directions can be used.

#### Coating type
Coating layers are applied in different degrees of hardness. The hardness is defined so that the appropriate cutting and processing tools - e.g. drills - can be used. The name can be chosen at random, e. g. soft, hard, without.

### Levels for the patterned and coated side
To define exactly how a lite shall be fitted into an IG unit, the different levels of an IG unit are defined. The unit is always seen from the outside (level 1) inwards (level 2).

**(Fig. B-89 Assembly levels for the patterned and coated side)**
The image shows a quadruple IG unit with 8 assembly levels, counted from the outside in.

### Cuts
You also need to define the direction of the cuts. If the sense of pattern does not matter, this task can be omitted to keep the waste at a minimum.

**(Fig. B-90 XYZ cuts on the stockplate)**
The image shows a stockplate with X, Y, and Z cuts, illustrating different cutting directions.

## Grills

There are different types of grills, e. g. glass-dividing grills, fitted grills, grills inside the airspace (AIR). In A+W Business, grills are usually entered for the airspace, and are distinguished by pattern type.

All grills, connections, and edge connections have to be defined as products so that they can be entered in an order.

### Grill construction types
For the processing of lites with several fields, the type of the grill connection is defined in addition to the edge connections. The following patterns are defined by default:

- **+**: Grill with double mitre at the intersection
- **Cross grills**: horizontal and vertical grills have blunt connections with the crosspieces.
- Vertical grill continuous, horizontal grill with overreaching mitre.
- Horizontal continuous grill, Vertical grill with overreaching mitre.
- Vertical grill continuous, horizontal grills with blunt connections to the vertical grills.
- Horizontal grill continuous, vertical grills have blunt connections to the horizontal ones.
- Horizontal and vertical grills continuous.

> **Define new grill types only if agreed**
> If you are using A+W Production, new grill types have to be agreed with A+W Software GmbH.

### Calculation type for grill construction Prices and Surcharges
Referring to the fields or drill positions, symmetrical or asymmetrical grills can be entered.
- You can enter individual sizes for grill construction so that drill holes or fields are arranged asymmetrically.
- In case of automatic calculation you can define whether the symmetry shall be related to the drill holes or to the fields.

> **Example: Symmetrical calculation of grill pattern**
> An edge length of 1000 mm and a grill width of 26 mm will produce the following values (without cutback):
> - **Drill-hole symmetrical**: The drill holes are each 333.3 mm away from the edges. The edge length of the outer fields is 307.3 mm while the central field has an edge length of 320.2 mm.
> - **Field-symmetrical**: The drill holes are 329.0 mm away from the edges, with a central distance of 342.0 mm. The edge length of the three fields is 316.0 mm.

### Spacer code
The spacer codes are passed on at transfer to production. The codes have to be agreed with A+W Production.
The spacer code in the variant can overrule the code defined in product master data.

## Prices and Surcharges

### Objectives
- Defining the price-relevance of products.

### Benefit
- Price and tax codes serve to calculate order items.

### Note

**Price view**
- **Implicit:** The main item's net price includes all prices of the BOM elements; i.e. shape and exchange surcharges as well as processing. Other surcharges are implicit only, i.e. they do not appear on the order.
- **Explicit:** The prices of the BOM elements are listed separately.
- **Implicit, price per quantity unit:** The price of the BOM elements are converted to the main product's price unit. This total price is shown in the document but only if all BOM elements of the item have been allocated the same display type.

**Adopt main item**
Calculation and display of prices depends on the details entered for the main item. There are various ways of adopting discounts and prices.

**Pricing codes**
Prices, discounts, and cash discounts can only be calculated if permitted for the product.

### Price Parameters
This tab serves to allocate price tables and surcharges and to define how the prices are to be displayed.

**(Fig. B-93 Product management - Price/Surcharge)**
The image shows the price/surcharge tab in product management.
- **A Tax rate**: Fields for setting tax rates.
- **B Automatic Surcharges**: Fields for special discounts.
- **C Cost accounting details**: Fields for cost type and cost center.
- **D Price view**: Defines how prices are displayed (e.g., explicit).
- **E Price tables**: Allocation of sales and purchase price tables.
- **F Surcharges**: Allocation of surcharge tables.
- **G Rounding for pricing purposes**: Defines size rounding for width/height.
- **H Price code**: Checkboxes for price relevance (SP/PP), discountable, and cash discountable.

You have to enter the tax rate (A) for every product. If you are using cost accounting, you can also enter the cost type and the cost center.

You can also calculate automatic surcharges (B), e.g. an energy surcharge or surcharges for the exchange of BOM elements (F).

A product can be calculated for sales and purchasing only if the appropriate codes (H) have been set and if the corresponding price tables (E) have been defined.

Surcharges and prices are described in detail in separate sessions.
⇨ "Surcharges" on page B-334
⇨ "Price Master Data" on page B-276

### Price View
For every product you can define the way in which prices are displayed. Product management offers the following options for this purpose:
- **Price view:**
  - **Implicit:** The main item's net price includes all prices of the BOM elements; i.e. shape and exchange surcharges as well as processing. Other surcharges are implicit only, i.e. they do not appear on the order.
  - **Explicit:** The prices of the BOM elements are listed separately.
  - **Implicit, price per quantity unit:** The price of the BOM elements are converted to the main product's price unit. This total price is shown in the document but only if all BOM elements of the item have been allocated the same display type.

> **Price view - an example**
> The section Prices offers a detailed example of the display of prices.
> ⇨ "Example of how Prices are Shown in the Document" on page B-283

### Adopt Main Item
If the product is included in a bill of material, calculation and display of the prices and discounts can depend on the settings which have been made for the product of the main item. The following settings are possible:
- **No adoption:** The price settings will not be adopted from the main item.
- **Discount + price key:** Discount and price key will be adopted from the main item.
- **Discount:** Only the discount will be adopted form the main item.
- **Price key:** Only the price key will be adopted from the main item.
- **No adoption (net for ind.pr.main itm):** For customised net prices, the settings shall not be adopted from the main item.
- **Discount + price key (net for ind.pr.main itm):** For customised net prices, the discount and price key shall be adopted.
- **Discount (net for Ind.pr.main itm):** For customised net prices, only the discount will be adopted.
- **Price key (net for ind.pr.main itm):** For customized net prices, only the price key shall be adopted from the main item.
- **Discount + price key (even if discount exists):** Discount and price key will be adopted from the main item even if a discount has been defined for the BOM product, e.g. when a lite is replaced.
- **Discount (even if discount exists):** The discount shall be adopted from the main item even if a discount has been defined for the BOM product, e. g. when a lite is replaced.
- **Price key (even if discount exists):** The price key shall be adopted from the main item even if a discount has been defined for the BOM product, e. g. when a lite is replaced.

Prices and discounts are described in detail in separate sessions.

> **Settings for pricing in company data**
> Dialog Company data > tab Pricing serves to make general settings which can partially override the settings in product master data.

### Pricing Codes
Prices, surcharges, and discounts are calculated only for products of BOM elements for which the corresponding codes have been set:
- Price-relevant for sales (SP)
- Price-relevant for purchasing (PP)
- Discountable
- Cash discountable

A product is price-relevant if it has its own sales price which is used for pricing. For products with a BOM, this can refer to the main product or to the individual elements.

This means that you either enter a price for the product, or calculate it in connection with an order, based on the BOM elements.

> **Example**
> A door consists of a toughened lite with fittings at the bottom corners, and a brass bearing. A price table has been created for this product according to which the door shall cost 200.00 €. It is therefore price-relevant. This code is disabled for the individual BOM elements however.
> The BOM would be price-relevant if the individual BOM elements were price-relevant. The price would be calculated in the order.
> If all BOM elements were price-relevant in addition to the main product, the price would be calculated as follows:
> Price for the complete door
> + price for a toughened lite
> + price for bottom fittings
> + price for brass bearing

If the code is not set, A+W Business considers the product irrelevant for pricing even if a price table has been allocated. If a product is irrelevant for pricing, no price will be shown at order entry, and no price can be entered by hand either.

If the prices for exchange lites in IG units are calculated by means of exchange surcharges, the code price-relevant has no effect. The price setting for the main item has to be obeyed however. This setting will be dealt with in the session on exchange discounts.

## Stock and Purchasing

### Objectives
- Distinguishing procurement types.
- Introducing the settings for stock management.
- Introducing the settings for purchasing.

### Benefit
- Settings for stock management and purchasing serve the provision or replacement of products. The settings will be adopted for the documents and can be amended if necessary.

### Note

**Procurement type**
The procurement type defines how the product is to be acquired for this order, e.g. production, stock withdrawal, purchasing.

**Maximum sizes for purchasing**
The sizes will be checked at document entry.

**Stock booking type**
The stock booking type defines how a product is kept as a stock article in stock management.

**Alternative product codes (for the procurement type)**
The supply type for different clients and/or order areas can differ from the supply type defined in product master data.

### Stock Settings
This tab serves to define the parameters for purchasing and stockkeeping of the product.

**(Fig. B-95 Product management - Stock / Purchasing)**
- **A Purchase sizes**: Max. width and height for purchasing.
- **B Procurement type**: Defines how the product is procured (e.g., Production).
- **C Different product code**: Allows for different codes for specific clients/areas.

Products can be produced or purchased. The procurement type (B) defines how the product has to be procured for the order in question.

### Procurement Type
Product master data define how the product is going to be procured for the order:
- **Production:** The order item will be produced in-house. If a main article has got this procurement type, its BOM elements can be defined as stock articles or as purchased articles.
- **Cutting:** The glass for this order item is cut from stock sizes. The sizes are then transferred to production.
- **Stock withdrawal:** The product is kept in the stock as a stock article in sqm or as a stock dimension with its dimensions in the case of glass articles. Other products are kept in stock in their quantity unit. The defined quantity will be reserved at order entry. This procurement type is a prerequisite for stock management in the stock module.
- **Processing:** The processing steps for an order item are transferred to production.
- **Customer's own glass:** The product is supplied by the customer and will be used to produce his orders.
- **P.O.:** Only the product in question will be ordered, irrespective of the contents of the BOM acc. to the order. If a laminated lite consists of a float lite, a film, and a toughened lite for instance and only the toughened lite is marked as P.O., only the toughened lite will be ordered from the supplier. The laminated lite will be produced in-house.
- **P.O. (complete):** The product is ordered, including all processing steps defined in the BOM of this order. If a laminated lite consists of a float lite of 5 mm, a film layer, and a 5 mm toughened lite, the entire laminated lite will be ordered. Please note the difference from the code P.O.
- **Addition to stock through production:** The product shall be used in work orders only to fill up the stock. The produced items will be added to stock.

The code Procurement type is adopted from product master data for the order item. In the order, every single item can be allocated a different procurement code.

### Stock Booking Type
The stock booking type defines how a product is kept as a stock article in stock management:
- **Size-dependent:** Choose this setting if stock sizes are to be kept as units. This setting makes sense only for glass. The quantity unit should still be set to sqm on tab Product to make sure that the surface is calculated.
- **Not size-dependent:** Choose this setting for all stock articles to be kept with their actual quantity unit, e.g. units, fittings. Use this setting also for glass which is to be kept in sqm.
- **Combined:** Choose this setting if you are using reports from the shop floor. This setting makes sense only for glass. Please remember to define a virtual stocksize without sizes for this purpose.

The setting w/o will not be used in this context.
Stock bookings are described in detail in section Stock management.

### Different Product Codes
If you are using clients and order areas, you can define procurement types for the individual products or product groups which differ from the entries made in product master data.

> **Example**
> The order areas IG, tempered glass, and laminated glass user internal orders. All order areas use the same database, the same master data, etc.
> An order is entered in the IG area; the IG unit consists of a laminated lite with tempered glass, a spacer, and a float lite.
> - For order area IG, the IG unit is Production, the laminated lite is Purchased while the float lite is Cut.
> - For order area laminated glass, the laminated lite is Production, the toughened lite is Purchased, and the float lite is also Cut.
> - For order area tempered glass, the toughened lite is Production, and the float lite is Cut.
> The different supply types for laminated glass and tempered glass thus have to be defined by different product codes.

**(Fig. B-96 Product code management)**
The image shows a dialog to manage different procurement types for a product based on client or order area.

## Shapes and Bills of Material

### Objectives
- Introducing the display of shapes.
- Creating bills of materials for complex products.

### Benefit
- Standard product structures are described by bills of materials and can be saved in master data.
- Pricing and production are based on bills of materials.

### Note

**Shape**
Shapes are usually standard shapes with a non-rectangular geometry.

**Shape catalog**
The shape catalog is predefined. Products are entered based on these settings.

**Bill of Material (BOM)**
A bill of materials describes the product structure. It consists of individual elements.

**BOM element**
Every BOM element is a product itself. BOM elements can be individual products as well as processing steps or further bills of material, so-called assemblies.

**Price- or production relevant**
A+W Business distinguishes price-relevant and production-relevant BOM elements.
- A price-relevant element is directly linked with the main product.
- A production-relevant element (the processing step) is linked with the glass.

**Main product**
The main product is the basis of a bill of materials. A bill of material is always attached to a main product. It can be linked with properties which apply to the whole (complex) product.

**Production BOM breakdown**
The production BOM breakdown defines the processings which shall or must not be applied to the main product but to the corresponding BOM element.

**Transmission**
Modifications of BOM elements can be passed on to other elements.
- Sizes are passed on to the various BOM elements (size transfer).
- In case of surcharges, either the basic item or the so-called parent product will be taken into account.

**Parent product**
A parent product is the basic product of an assembly, e.g. the laminated glass lite which is fitted as an assembly into an IG unit.

**Basic item**
The basic item is the top level of the bill of material.

### Shape
Shapes are entered in the catalog without sizes and glass as a product. In an order item, these non-rectangular shapes from the shape catalog can be assigned to a glass product and completed by the required sizes.

**(Fig. B-97 Schematic layout of the shape)**
This example shows that shape 2 (C) appears without sizes at first (A). The display is updated after the item sizes have been entered (B).

Working with shapes is described in detail in section Sales.

### Display of Shapes in A+W Business
The way in which shapes are to be displayed in product management and at order entry is defined in company data.

**(Fig. B-98 Company data - System)**
- **A Color setting for displaying shapes**: Defines the appearance of shape sketches (e.g., filled).
- **B Path for shape templates**: Defines the file path for S+N (Shape and Nesting) files.

The color setting (A) and the sizes refer to the display of the sketch in the dialog.

**(Fig. B-99 Unfilled sketch, filled-sketch)**
The image shows the same octagonal shape displayed as an unfilled outline and as a filled-in shape.

### Bill of Material (BOM)
A product can consist of several other products, e. g. an IG unit can consist of two lites, a spacer, and a round shape. All elements of the BOM have to be entered as products.

**(Fig. B-100 Structure of the product IG)**
The diagram shows a main product "IG 150100" breaking down into its BOM products: Float 4, Spacer, Grills, Float 4, Coating.

The following functions are based on the bill of material:
- Pricing
- Product names in documents, e.g. on the order confirmation.
- Stock management planning
- Production control
- Production time calculation

You can define your products in such a way that input is largely automated. The bills of material and their elements are available at order entry and can be adapted to the order in question.

### Production BOM Breakdown
The so-called production BOM breakdown is entered in product management for every production with a BOM if the processing step shall or must not be applied to the main product.

> **Example**
> Hinges and door handles have to be added to a glass door before the glass is toughened.
> When you enter the structure of a glass door you have to check the checkboxes for Drilling and Handles. These processing steps will be performed by default and do not have to be entered in the order.

### BOM Concept in A+W Business
In A+W Business, products are described by product master data. These include details such as name, type, product group, variants, colors, supply types.

Bills of material describe the product structure.

**(Fig. B-101 BOM elements of an IG product (order))**
- **A Main product: IG** (150070/Wärmeschutz-ISO)
- **B 1st element: single annealed glass** (1006/Float 6 mm)
- **C 2nd element: spacer with gas** (12012/12 mm ALU Profil, 12510/Wärmedämmgas 100% Argon)
- **D 3rd element: heat-protection glass** (1106/Wärmeschutz 6 mm Neutral)
- **E 4th element: shape** (8002 / Schräge Kante links)
- **F 5th element: step** (8000/Stufung Außenansicht)

BOM elements can be individual products as well as processing steps or further bills of material, so-called assemblies. All BOM elements have to be entered as products in master data.

> **Examples**
> - The product 'spacer' can be entered with the gas firmly allocated. The gas will always be added to the spacer as an element in this case.
> - When you replace a spacer you can define whether the corresponding gas shall be replaced too.
> - Film layers in laminated units can be added before or after the single annealed lite.

Every main product and every element is marked by the supply type which triggers the necessary action, e.g. purchase order, stock withdrawal, production.

Individual conditions for pricing can be defined for every BOM element.

Exchange/addition rules allow replacing certain articles or processing steps on the product BOM.

The BOM structure has no limits. The processing speed of the data in the program will however be reduced considerably if the BOM gets too bulky.

> **Restrict the BOM structure**
> In company data you have to define the maximum number of BOM elements that can be printed. Excess components will not be printed on the order.
> ⇨ Software Reference, "BOM" on page B-1005

### Passing on BOM Details
Modifications of BOM elements can be passed on to other elements. This means that the changes will be applied to other elements. Whether or not changes will be passed on depends on if they apply to sizes, or to the replacement of elements.
- Sizes are passed on to the various BOM elements (size transfer). The sizes of the main product 'triple IG' for instance will be passed on to all lites of the BOM.
- As to the transfer of surcharges, there is a selection of definitions which either consider the basic item or the so-called parent product. The basic item is the top level of the bill of material. A parent product is the basic product of an assembly, e.g. the laminated glass lite which is fitted as an assembly into an IG unit.

**(Fig. B-102 Distinction: Basic item - parent product)**
- **Product: Laminated glass (A Basic item)**: `701 / A+W VSG DEMO`
- **Product: IG with a laminated glass lite (B Parent product)**: The laminated glass `701 / A+W VSG DEMO` is now a child component (parent product) within the larger `700 / A+W VSG ISO` assembly.

The transfer of surcharges is described in detail in connection with Surcharges.
⇨ "Transfer of surcharge types" on page B-386

> **BOM of the parent product**
> The BOM of the parent product will not be displayed if the parent product itself is not produced but taken from stock.

### Price- and/or Production-Relevant
At order entry, A+W Business distinguishes BOM elements which are relevant for pricing and those that are relevant for production.

> **Example**
> - The price-relevant element is directly linked with the main product, e.g. tempered glass.
> - The production-relevant element (the processing) is connected to the float glass because this will be processed.

Production-relevant BOM elements can already be entered in product master data if they are to be applied as a standard.

Production-relevant BOM elements are shown in blue at order entry.

**(Fig. B-103 BOM elements in product master data and in the order)**
- **Display of the BOM of the product**: Shows a main product (A) and a production-relevant element (B).
- **BOM at order entry**: Shows the same structure, but now with an additional price-relevant element (C) for the same processing step.

The code is set in dialog Product management which is going to be introduced in the next session.
⇨ "Define Production BOM Breakdown" on page B-254

> **Restrictions**
> If restrictions have been defined for a product in dialog *Processing restrictions*, you can enter an alternative product. The assigned alternative product is available at order entry if the restrictions of the selected product are not met by the order data (item data).
>
> Spacer text for IG products can be automatically created from the defined text, and printed.

> **Additional information**
> ⇨ Software Reference, "Product Management" on page B-667
> ⇨ Software Reference, "BOM transmission of variants" on page B-962

### Product Definition
When you define a product you have to enter at least the number, the name, and the product type. All other data can be added later.

There are the following instructions on this subject.
- "How to enter a product" on page B-246
- "How to complete the product data" on page B-248

> **The product type influences the fields displayed**
> Please make sure to select the right product type because this will determine which fields are accessible in the Product Management dialog.

When setting up your product master data you should first decide how to arrange the products so that the first digit of the product number identifies the product type.

| Example | from number | to number |
| :--- | :--- | :--- |
| Single annealed | 1000 | 1999 |
| IG | 2000 | 2999 |
| Tempered glass | 3000 | 3999 |
| Laminated glass | 4000 | 4999 |
| Grills | 5000 | 5999 |
| Shapes | 6000 | 6999 |
| Processing | 7000 | 7999 |
| Articles | 10 000 | - |

> **Individual products**
> You can define individual products for recurring orders. These product structures are usually defined as macros and saved for a certain customer. Moreover, you can enter a customised fixed price.

> **Free numbers**
> You can view the free numbers in dialog Product management by clicking on the [Zoom] icon next to the input field for the number. This view is described in section Partners.
> "Input of Partner Master Data" on page B-110

#### How to enter a product
1. Go to menu **Master data > Products > Articles > Articles**.
   Dialog *Product management* appears.
2. Go to menu **Edit > New**.
   **(Fig. B-104 Fields for new product are accessible)**
   The product management window opens with all fields cleared for new entry.
   - **A Product number**: Field to enter the unique product number.
   - **B Product type**: Dropdown to select the product type.
   - **C Lock codes**: Option to lock the product from use.
   ⇨ Software Reference, "Product Management" on page B-667
3. Enter a number (A).
   The article number can consist of up to eight digits. You can choose the product numbers random; every number must however be assigned just once. You can view the free numbers by clicking on the [Zoom] icon.
4. Enter the appropriate terms in fields **Matchcode** and **Description**.
   The alpha-numerical matchcode may consists of up to fifteen digits.
5. Choose the product type (B).
   The product group appears automatically. It can be changed if required.
6. Check the setting in field **Lock code** (C).
   If the new product shall not be available for orders yet please select the lock code **locked**.
7. Select in the menu **Start > Save** to save the data.

With that, you have entered a new product. The product can be displayed in other modules only if the lock code is set to **not locked**.
Enter the necessary data in the tabs **Product, Production, Price/surcharges, Inventory/purchasing** and - if applicable - **BOM**. Leave the fields blank for which entries cannot be made at this stage, e.g. prices.

> **Product data for transfer to A+W Production.**
> Data which shall be transferred to A+W Production for production purposes, have to be entered in A+W Production tab. This tab is accessible only if the A+W Production connection has been enabled in company data.
> ⇨ Software Reference, "Company Data - Production" on page B-1009

#### How to complete the product data
1. In the new product, go to tab **Production** and check the settings in section **BOM parameters**.
   - `BOM not relevant for production`
   - `Suitable for IG`
   - `Rotatable pattern level`
   - `Print on BOM`
   If the product can be used as part of a BOM, check the checkboxes **suitable for IG** and **Pattern level rotatable** if applicable.
   If the product shall be purchased (ordered), check the checkbox **BOM irrelevant for production**. Please also choose this setting if the product must not be included in any BOM.
2. Go to tab **Price/surcharge** and select the price tables for sales and purchasing in section **Price parameters**.
   - `Price table SP/PP`
   Skip this step if no suitable prices have been entered yet. You can allocate the unit to the prices later.
3. Go to tab **Stock/purchasing** and check the settings in section **Product code**.
   - `Procurement type`
   - `Stock booking type`
   The following settings are available:
   - **Production:** The product will be produced in-house.
   - **Cutting:** The glass for this order item is cut from stockplates.
   - **Stock withdrawal:** The product is kept on stock, with just this size or as a unit.
   - **Processing:** The product is a processing step which is transferred to production by means of the order item.
   - **P.O. (complete):** The product will not be produced in-house but ordered from a supplier.
4. Select in the menu **Start > Save** to save the data.
   The data will be saved. Tab BOM will be introduced in the following session.

### Edit BOM Structure
Carefully consider which elements you are going to enter in product master data and which can be added at order entry. Product definition must include all production-relevant BOM elements.

| Product management | Order |
| :--- | :--- |
| Glass | Sizes |
| Spacer | Grills |
| Prices | Shape |
| Procurement type | Processing |
| Steps | Steps |

This example shows which BOM elements are rather entered in product master data, and which are mostly added at order entry. At the end of the day, all elements can be changed in the order.

Details on steps may be useful even in master data. This subject is handled in a separate session.
⇨ "Adding Steps to an IG Product" on page B-251

Details on grills, shapes, and processing steps are rather expected in connection with order items. These BOM elements are described in detail in section Sales.
⇨ Sales, "Order items" on page C-1175

#### How to edit a BOM
1. Go to menu **Master data > Products > Articles > Articles**.
   Dialog *Product management* appears.
   ⇨ Software Reference, "Product Management" on page B-667
2. Search the product the BOM of which you want to edit.
   Restrict the search to a product type the products of which are part of the BOM, e. g. IG or laminated glass.
3. Go to tab **BOM**.
4. In section **BOM** tag the element above or below which you want to add an element.
5. Open the context menu and enter the required command.
   - `Insert element (before)`
   - `Insert component (after)`
   - `Add element`
   - `Delete element`
   This commands have the following effects:
   - **Insert element (before, after):** The cursor automatically switches to field *Article number*. When you select the element, it will be added to the BOM on the same level.
   - **Add element:** The cursor automatically switches to field *Article number*. When you select the element, it is automatically added to the BOM on the level below.
6. Go to the menu **Start > Save** to save the changes.
   The data will be saved.

> **Changing BOM elements**
> BOM elements can be replaced by other elements. When an element has been selected it can be replaced in field *Article number*.

### Adding Steps to an IG Product
Steps can be useful for IG products which are usually entered with steps in the orders.

#### How to enter a step
1. Go to menu **Master data > Products > Articles > Articles**.
   Dialog *Product management* appears.
2. Search the IG product the BOM of which you want to edit.
3. Go to the **Shapes/processing** tab.
4. Select the step by entering the product number, or by means of the corresponding icon.
   The fields to enter the values are displayed.
   **(Fig. B-107 Define step)**
   - **A Select the lite for which the step shall be defined**: Checkboxes for `1 = Outside lite` and `2 = Inside lite`.
   - **B Enter the values per edge**: Positive entries will scale down the selected lite. Negative entries will enlarge the lite.
   ⇨ Software Reference, "Items - stepping" on page C-1611
   The fields for the sizes are now enabled. If no shape has been entered, a rectangular lite will appear automatically.
   In section **Parameters**, a checkbox (A) pops up for every glass element. In this example, this is an IG unit consisting of two lites. For triple IG, three checkboxes will appear. Checkbox 1 is the outside lite.
5. Enter the size of the step per side (B).
   Please make sure to check checkbox 2. You will have to enter positive values for this lite in the fields, e. g. 15.
   When you enter a negative size (-15), a larger lite will be cut. This would mean that lite 2 (inside) would be bigger than the outside lite.
   The sketch shows for which sides steps have been defined.
6. Select in the menu **Start > Save** to save the data.
   The step is shown as a BOM element.
   **(Fig. B-109 BOM with steps)**
7. Select in the menu **Start > Save** to save the data.
   The data will be saved.

Grills, shapes, and processing steps are added in the same way. These steps are described in detail in section Sales as these elements will mostly be added at item input.

### Define Production BOM Breakdown
This session will show you how to define the BOM element to be processed.

#### How to edit the production BOM breakdown
1. Go to menu **Master data > Products > Articles > Articles**.
   Dialog *Product management* appears.
2. Search the product the BOM of which you want to edit.
3. Go to tab **BOM**.
4. In section **BOM**, select the element the production BOM breakdown of which you want to edit.
   The fields in section **Production BOM breakdown** are accessible.
   **(Fig. B-110 Valid processing steps for the transfer to production)**
   The screen shows a list of processing classes (e.g., Processings, Coating, Drilling) with an "Active" checkbox for each.
5. Check the checkboxes of the processing steps to be applied to the selected element, e. g. drilling.
6. Select in the menu **Start > Save** to save the data.
   The data will be saved. Production-relevant elements are shown in blue at order entry.

### Grill Input
Grills and grill patterns can be defined for an IG unit if this kind of product frequently occurs in orders. The details can be amended in the actual document.

There are the following instructions for this session:
- "How to enter a common grill pattern" on page B-255
- "How to enter an uneven grill pattern" on page B-257

> **Prerequisite**
> A grill pattern can be defined in product management only if minimum and standard sizes have been entered for the IG product on tab Product.

#### How to enter a common grill pattern
1. Go to menu **Master data > Products > Articles > Articles**.
   Dialog *Product management* appears.
2. Search the IG product the BOM of which you want to edit.
3. Go to tab **grills**.
4. Choose the grill pattern by means of the corresponding icon.
   The fields for the vertical and horizontal grills are released.
   **(Fig. B-111 Fields for grills are enabled)**
   - **A Grill pattern selection**
   - **B In the case of multiple IG**: Select the spacer
   - **C Selection of grills**
   - **D Number of grills**
   - **E Cutback**
   - **F Calcul. type**
   ⇨ Software Reference, "Items - grills" on page C-1614
5. Choose the grills (C) and enter the quantity (D).
   If you have entered a multiple IG unit, you must select the spacer (B) to which the grills shall be attached.
   The graphics and the fields will be updated. You can choose different products and/or variants for the horizontal and vertical grills.
   Use this button to adopt the grills for the second spacer.
   However, you can also design the grill grids differently in the gaps, e. g. position the horizontal grills in the first gap and the vertical ones in the second.
6. Define the calculation type (F) and enter the drilling sizes if necessary.
   The fields for the drilling positions are only released for asymmetrical calculation types.
   ⇨ "Grills" on page B-227
7. Check the size of the cutback (E) and define whether or not felt pads shall be fitted.
8. Select in the menu **Start > Save** to save the data.
   The grills appear on the BOM.
9. Select in the menu **Start > Save** to save the data.
   The data will be saved.

#### How to enter an uneven grill pattern
1. Enter the grills as described in steps 1 to 7 of the previous process.
   Please make sure that the number of grills permits an asymmetrical pattern.
2. To fit V grills, go to tab **Auxiliary grills**.
   **(Fig. B-112 Uneven grill pattern)**
   - **A Diagonal grills**
   - **B Vertical grills**
   - **C Horizontal grills**
3. Disable the checkboxes for all grid sections that are not required, e.g. the vertical grills in the top third (B).
4. Enable the checkboxes for diagonal grills (A).
5. Select in the menu **Start > Save** to save the data.
   The data will be saved.

Special grill patterns such as sun or moon are also possible. These are the subject of a separate training session on A+W CAD Designer.

### Define Shapes
Shapes can be defined for an IG unit if this kind of product frequently occurs in orders. The details can be amended in the actual document.

> **Prerequisite**
> You can define a shape for a glass only if shapes have been specified as a product.

#### How to enter a glass with a shape
1. Go to menu **Master data > Products > Articles > Articles**.
   Dialog *Product management* appears.
2. Search the product the BOM of which you want to edit, or enter a new product.
3. Go to tab **Shapes/processings**.
4. Select by using the icon **Shapes**.
   The fields to enter the values are displayed.
   **(Fig. B-113 Shape input)**
   - **A Enter sizes**
   - **B Select a shape**
   - **C Dimensions for price calculation**
   ⇨ Software Reference, "Items - shapes/processing tab" on page C-1590
5. Select the shape by entering the shape or product number, or by means of the corresponding icon (B).
   Section **Display** shows a sketch of the shape; the fields for the corresponding sizes are released.
6. Enter the sizes for the edges (A).
   Please obey the appropriate notes, W1+W2<=W for example means that the total of the entries for edges W1 and W2 must not exceed the size of edge W.
   When you have made all entries, the size of the surrounding rectangle is shown which is used for price calculation by default.
7. Go to the menu **Start > Save** to adopt the shape data.
   The data will be saved. The shape appears on the BOM.
8. Go to the menu **Start > Save** to save the data.
   The data will be saved.

### Define Processings
Processing steps can be defined for a glass if this kind of product frequently occurs in orders. The details can be amended in the actual document.

> **Prerequisite**
> Processing steps have to be defined as products.

#### How to enter a processing step for a lite
1. Go to menu **Master data > Products > Articles > Articles**.
   Dialog *Product management* appears.
2. Search the product the BOM of which you want to edit, or enter a new product.
3. Go to the **Shapes/processing** tab.
4. Select the processing step by entering the product number, or by means of the corresponding icon, e. g. edgework.
   **(Fig. B-115 Processing: Example: Edge sawing)**
   - **A Select the processing step**
   - **B Selection of the edges to be processed**
   - **C Reference corners, reference edges**
   - **D Mitre angle**
   Product data for this processing step are loaded now. The fields for the corresponding parameters are displayed and enabled.
   The parameters are described in detail in chapter Sales.
   ⇨ Software Reference, "Items - processing" on page C-1592
5. Enter the parameters by ticking or unticking the checkboxes (B) for the edges, and enter the sizes.
   Please obey the reference corners or reference edges (C) and convert the sizes if necessary.
   ⇨ Software Reference, "Parameters" on page C-1593
6. Go to the menu **Start > Save** to adopt the data.
   The data will be saved; price fields will be updated. The BOM shows the processing and the corresponding price.
7. Go to Menu **Start > Save** to save the product.
   The data will be saved.

> **Wrong or missing processing parameters**
> If incorrect parameters are displayed for a processing step, you have to check if the proper product type and group have been allocated to this product in product management.

### Exercises
Enter the following products:
- Grills
- Single annealed, e.g. wired ornaments which must not be part of an IG unit.
- Tempered glass to be purchased.
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

**Products**
The products defined in master data serve for the input and pricing of documents. They will not be automatically kept as stock on hand.

**Stock size**
A+W Business distinguishes stock sizes for pricing (in the order) and stock sizes for stock management.

**Stock code (stock booking type)**
The stock code defines whether the stock on hand for an article is evaluated as a surface (sqm) or a quantity (pieces).

**Procurement type**
The code defines how a product is to be provided by default, e. g.:
- Cutting
- Stock withdrawal
- Production
- Purchasing

**Variants**
Products with identical properties can be kept in different colors. The product is defined just once and is distinguished further by allocating the colors (variants).

### Product Data and Stock
All products entered in the sales area are allocated a code to identify the procurement type. Apart from the code (procurement type) Stock withdrawal, glass kept on stock has a code (stock booking type) defining how the stock on hand is calculated.

Products kept on stock with their quantities have to be defined as so-called stock sizes.
A+W Business distinguishes stock sizes for pricing (in the order) and stock sizes for stock management.
- **Stock sizes** are used at order entry and for pricing. You can enter several stock sizes per (glass) product, with different widths and heights. If these sizes are kept on stock they do not have to be cut. This is why these prices can be calculated differently.
- **Stock sizes** for stock management serve for stockkeeping. Lites can be defined in different sizes for stock management.

**(Fig. B-116 Relations between product, stock size, and price)**
The diagram shows the flow from Master Data (Product, Sales price list) to Price (Fixed size cutting, Stock size), to an Order in Sales, and finally to Stock (on hand), either by cutting from a stockplate (consumption = surface) or taking a pre-cut stock article (consumption = pieces).

You can enter several stock sizes for a product, with different sizes.

The procurement type for lites of defined sizes is usually Stock withdrawal. You can also define stock sizes (for pricing) which are not kept on stock.

**(Fig. B-117 Product management – stock sizes)**
- **A Product for which stock sizes have been defined**
- **B List of stock sizes with different sizes**
- **C Allocated price list**
- **D Procurement type**

The stock sizes for pricing are entered in dialog **Product management - stock sizes**.
Stock sizes for stockkeeping are entered in dialog **Stock management**. These stock sizes are described in detail in section Stock management.

### Variants
Products can be kept in different colors, e. g. spacers or grills in white, silver, and brown. This means that all color variants of a product can be entered in an order by means of the same product number.

> **Color variants of lites**
> Colored lites are defined as independent products, e. g. Float 3 mm in bronze and Float 4 mm in bronze.

Defining product variants requires the following steps:
- Enter all colors of your products as basic data in dialog Variants.
- Enter the product master data.
- Define the product variants by allocating a color to the product.

**(Fig. B-118 Variants which can be allocated)**
- **A Color number can be chosen at random**
- **B External key for transfer to production software**
- **C Display of color in the order**
- **D Adopt the color definition from the order**

The color (=variant) is transferred to production by means of the external key (B).
The color display (C) defines how e.g. grills shall be displayed at item entry. This color is not transferred to production.
The code **Special color (D)** can be used to enter special colors in an order, e. g. for screen printing.

> **Example**
> For a customer order you want to enter screen printing with a certain pattern, e. g. a formula 1 racecar.
> For such a case, a variant with the code **Special color** must be defined for the product *Screen printing*. At item entry, select this product variant for the processing step *Screen printing*. Another field appears in which you can enter the name of the pattern. This name will be transferred to production.

Colors are allocated to the product in dialog **Product variants**.

**(Fig. B-119 Product variants in master data)**
- **A Product for which variants have been defined**
- **B (Color) number of the variant**
- **C Variants of the product**

This example shows that several colors have been allocated to product grills. When you enter an order item, first enter the product then select the variant. Colors which have not been allocated to the product cannot be selected at order entry.

**(Fig. B-120 Product variants in the order (tab BOM))**
The image shows an order's BOM where a product (A), `Wiener Sprosse 18 mm`, has a specific color variant (B), `BLAU A1`, selected.

### Definition of stock sizes
This session shows you how to define stock sizes for the products which can be used to differentiate pricing.

> **Prerequisite**
> Stock sizes can be entered only if price keys have been defined before.

#### How to define stock sizes in master data
1. Select menu **Master data > Product > Products > stock sizes**.
   Dialog *Product management - stock sizes* appears.
2. Go to the menu **Start > New** to switch to the input mode.
   **(Fig. B-121 Fields for new stock size are accessible)**
   - **A Product number to which the stock size belongs**
   - **B Lite size (contents only for boxes)**
3. Enter the product number (A) for which stock sizes shall be defined.
   You can also use the search function for selecting the product.
4. Enter the width and the height (B).
   If the stock size is managed as a box, enter the number of lites in the box in field **Contents**.
5. Select the price keys for sales and purchasing (B).
6. You can make the following, different settings:
   - Product groups (A) used for managing the stock size.
   - Name and short name (matchcode), e.g. for better identification of stock sizes.
   - Procurement type (C), e.g. Stock withdrawal for stock articles.
7. Select in the menu **Start > Save** to save the data.
   The data will be saved. Next, the system will want to know whether you want to define this stock size as a stock product as well. Stock articles are described in detail in section Stock management.

### Definition of Product Variants
This session will show you how to enter different variants of a product, e. g. colored grills of the same width.

> **Prerequisite**
> Product variants can be entered and saved only if the product and the basic data for the variants (colors) must be defined first.

#### How to define a product variant
1. Go to menu **Master data > Products > Articles > Product variants**.
2. Search the product for which you want to define variants.
3. Click on the icon [Variants] on tab **Product**.
   Dialog *Product variants* appears. The system will come up with a message should no variants have been defined for a product yet. Acknowledge this to go to dialog *Product variants*.
4. Go to menu **Edit > New**.
   **(Fig. B-123 Fields for the new product variant are accessible)**
   - **A Product number**
   - **B Variant (color) number**
5. Enter the number of the product (A) for which variants shall be defined.
   You can also use the search function for selecting the product.
6. Choose the variant (B).
7. Fill in the fields **Price table (A)**, **Product group (B)**, and **Procurement type (C)**.
   You can use a single price table for all variants, e. g. with a proportional surcharge (unit price).
8. Select in the menu **Start > Save** to save the data.
   The data will be saved. The new product variant appears in section **Available product variants**.
   You can add further product variants and other colors to the same product.

#### How to add another product variant
1. Go to menu **Master data > Products > Articles > Articles**.
2. Search the product for which variants shall be defined, e. g. grills with a width of 20 mm.
3. Click on the icon [Variants] on tab **Product**.
   Section **Available product variants** lists all variants which have already been defined for this product.
4. Go to the menu **Start > New** to switch to the input mode.
   The fields will be released.
5. Choose the variant in section **Variant**.
6. Check the entries for the price table, the product groups, and the procurement type.
7. Select in the menu **Start > Save** to save the data.
   The data will be saved. The product variant is now available at order entry.

### Exercises
Enter the following data:
- Stock sizes for your training products
- Colors (variant)
- Enter several product variants for your (training) products.
- Enter two variants of the product 'grills'. If you have not got any price tables yet, you can do this exercise later, after dealing with the subject of **Prices**.

> **Additional information**
> ⇨ Software Reference, "Variants/Colors" on page B-650
> ⇨ Software Reference, "Stock Sizes" on page B-707
> ⇨ Sales, "Order items" on page C-1175
> ⇨ Stock management, "Products as Stock Articles" on page G-2463

## Price Master Data

Pricing in A+W Business consists of modules covering all pricing options. These modules include prices, surcharges, and discounts.

This session will show you how prices are handled and calculated in A+W Business.

This includes the following training sessions:
- "Stammdatendialoge für Preise" auf Seite B-321
- "Preisdefinition" auf Seite B-324
- "Preistabellen" auf Seite B-333
- "Gestaffelte Preise" auf Seite B-353

## Price Management

### Objectives
- Introducing the structure of price lists.
- Distinguishing different pricing methods.

### Benefit
- Prices can be handled flexibly. You can also use different currencies.
- Settings made in master data can be changed in the actual order.

### Note

**Price definition**
Various elements are used for pricing, e.g.
- Rates
- Price per quantity unit
- Surcharges and discounts

**Pricing methods**
A+W Business offers the following pricing methods:
- Unit price calculation
- IG prices + exchange surcharges
- VEGLA pricing
- Mixed calculation (Austria)
- French pricing

**Pricing based on minimum values**
The minimum value will be applied whenever the actual order or item quantity falls below the minimum defined. The minimum value can be a quantity or a price.

**Currencies**
Prices can be kept in different currencies.

**Price table**
The price table shows the price of the product. The price table usually has the same number as the product.

**Price list**
All price tables of a rate form the price list.

### Introduction of the Subject 'Prices'
This simple chart shows a price list with a price table and its different elements, e.g. price lists, price keys, surcharges.

**(Fig. B-126 Price list elements)**
The diagram shows how `Price year`, `Price key`, `Shape surcharge`, and `Exchange surcharge` all feed into a `Rate`. The rate, along with `Price/quantities` and `Price groups`, determines the final `Price table`.

Price years, keys, and rates form the framework of the price lists. Prices can be defined in standard price lists or in price lists for certain customer or supplier groups, for individual customers or for individual suppliers.

Settings made in master data can be changed in the actual order. The following hierarchy is used for price calculation:
- **Manual entry of prices in an order or quotation (top priority):** This subject is dealt with in detail in section Sales.
- **Project-related agreements:** These terms only apply to a certain building project.
- **Customer/supplier-related agreements:** These terms apply to a certain partner.
- **Group-specific agreements:** These terms apply only to a certain group.
- **General agreements:** These price lists will be introduced in this session.

Within these hierarchy levels you can enter general prices, special conditions for product groups and individual products, alternative prices and surcharges for shapes and grills.

By defining different terms you can accept divergences from the generally valid prices.

> **Currencies**
> Prices can be kept in different currencies. You can access several price lists at once to compare calculations. The currencies are described in Tutorial 2.

### Pricing methods
**Unit price calculation:**
Pricing is based on the elements of the product. This method is described in detail below.

| Price examples: | |
| :--- | :--- |
| Float 4: 30.00 €/sqm | - price table 1004 |
| Float 5: 35.00 €/sqm | - price table 1005 |
| AIR: 12.00 €/m | - price table 1 |
| Abstracto: 40.00 €/sqm | - price table 0 |

| Product examples: | |
| :--- | :--- |
| **IG 1 (1000 x 1000 mm)** | **IG 2 (1000 x 1000 mm)** |
| Float 4: 30.00 €/sqm - price table 1004 | Float 4: 30.00 €/sqm - price table 1004 |
| AIR: 12.00 €/m - price table 1 | AIR: 12.00 €/m - price table 1 |
| Float 4: 30.00 €/sqm - price table 1004 | Abstracto: 40.00 €/sqm - price table 0 |

| Unit price calculation | |
| :--- | :--- |
| **IG 1:** | 2 x 30.00 € + 4 x 12.00 € = 108.00 € |
| **IG 2:** | 30.00 € + 40.00 € + 4 x 12.00 € = 118.00 € |

**IG prices + exchange surcharges:**
Prices for standard IG structures and exchange surcharges (EXS). This method is described in detail in section Exchange surcharges.

| Price examples: | |
| :--- | :--- |
| ISO 4-12-4: 100.00 €/sqm | - price table 4 |
| IG 5-12-5: 110.00 €/sqm | - price table 5 |
| Exchange surcharge: Abstracto: 40.00 €/sqm | - price table 1 |
| Exchange surcharge: Group A: 30.00 €/sqm | - price table 1 |

| Example orders: | |
| :--- | :--- |
| **IG 1 (1000 x 1000 mm)** | **IG 2 (1000 x 1000 mm)** |
| Float 4 | Float 4 |
| AIR 12 | AIR 12 |
| Float 4 | Abstracto |

| IG + EXS | |
| :--- | :--- |
| **IG 1:** | Price table 4 = 108.00 € |
| **IG 2:** | 100.00 € + 40.00 € = 140.00 € |

- **VEGLA pricing:** Pricing is based on a single matrix which includes surcharges and discounts for the individual thicknesses and exchange lites. A short overview of this method will be given in a separate session. ⇨ "Basic IG table" on page B-290
- **Mixed calculation (Austria):** The price is calculated from two or three IG price tables. A short overview of this method will be given in Tutorial 2. ⇨ Tutorial 2, "Mixed calculation" on page B-607
- **French pricing:** Pricing based on surface and unit price. A short overview of this method will be given in Tutorial 2. ⇨ Tutorial 2, "French pricing" on page B-608

### Pricing based on minimum values
You can enter the minimum order value for every price table. The minimum value will be applied whenever the actual order or item quantity falls below the minimum defined. You can define a minimum quantity or a minimum price.

These values can be entered at the following points:
- Gross price, net price, and quantity
- Small quantity surcharge and surface (automatic surcharge)
- Replacement surcharges
- Shape processing as a processing surcharge
- Emergency glazing for insurance prices
- Partner master data

Price calculation for orders is described in section Sales.

### Unit prices
For the definition of unit prices for customers you can use all the reference values that apply to the general price lists and surcharges. You can either enter price tables for individual customers or amend the prices in the order as necessary and agreed.

> **Example**
> There is a standard price for IG which has been defined as a matrix. Apart from that, an unit price can be defined for a customer which is entered as an unit price because an appropriate agreement has been made with that customer for IG, e. g. because of defined order quantities.

This price is automatically used when the corresponding order is entered for the customer in an order.

### Dialog Prices
Price data are entered in A+W Business as price master data in dialog **Prices**. These master data are used in documents and can be changed there if required. Amendments made in the documents will not be saved in master data.

**(Fig. B-129 Dialog Prices)**
The dialog header shows the main price definitions in brief. This way you can check on all tabs which price you are currently editing.
- **A Number of the price table**
- **B Remarks, e.g. product name**
- **C Price year**
- **D Price key**
- **E Key text**
- **F List of price tables**
- **G Diversion to a rate for shapes**
- **H Diversion to another rate**
- **I List of assigned products**

For every product, a price table will be created the number of which matches the product number. Every price table is allocated to a year and a key. The price for every price table can be entered in different ways, e. g. as unit price or graduated price.

**Next key**
If the price shall be valid only up to a certain size you can define a so-called 'next key'. The next key refers to another price table which will be automatically used for pricing if there is no price in the standard price table for the size entered in the order.

### Master Data Dialogs for Prices
Apart from the data entered in dialog **Prices**, other data from the following dialogs are used for defining prices:
- Year, key, rate
- Other surcharges, exchange surcharges, shape surcharges, group surcharges
- Price and quantity units, limit types, grill price elements

These dialogs will be described in the following sessions in connection with the corresponding prices.
Surcharges are described in a separate session.
Glazing prices are a speciality in that special prices and surcharges can be defined for repairs and emergency glazing.

### Example of how Prices are Shown in the Document
Prices and discounts will be used for calculation only if the appropriate codes are set in the order. This setting has been introduced in section **Product management**.

For every product you can also define the way in which prices are displayed.
- Implicit
- Explicit
- Implicit in price per quantity unit

#### Price view Implicit in price per QU
In this example, a float lite of 5 mm, with a size of 1000 x 2000 mm has been entered, with two drill holes. The glass price is 10 €/sqm. The drill holes will be charged at 5 €/pc.; the price code is set to implicit. Calculation is done in the following way:

| | | |
| :--- | :-: | :-- |
| **Total price per sqm** | **=** | **15 €** |
| Glass price (2 sqm) | = | 20 € |
| Price for the drill hole (2 pcs.) | = | 10 € |
| Total | = | 30 € |
| ÷ total sqm | ÷ 2 | |
| **Price/sqm** | **=** | **15 €** |

The price for drilling is included (implicitly) in the price/price unit of the main product (in this case, glass -> sqm).
This price appears in the info section of the dialog as net sales price (A).

**(Fig. B-130 Price as shown in the order - item entry)**
- **A Sales price and purchase price for the selected item**: Shows the calculated prices.
- **B Implicit per quantity unit**: The price display type is set to "Included in price per QU".

The price for hole drilling is 5 €/pc.

**(Fig. B-131 Price of the processing step 'drill hole')**
- **A Name of the processing step (product)**: `Lochbohrungen A+W`
- **B Price per piece**: `5.00 Stk`

## Definition of Prices

### Objectives
- Knowing the connection of price lists, price keys, and rates.
- Checking global settings for pricing.
- Editing rates.

### Benefit
- Prices for sales and purchasing can be kept in different lists.
- Price lists are used for calculating orders and purchase orders.
- Based on different settings for price allocations and surcharges, price lists can be created quite flexibly.

### Note

**Price table**
The price table shows the price of the product. The price table usually has the same number as the product.

**Price year**
Every price table is allocated to a year and a key (rate). Prices are always defined for a certain year. A price year is a collection of price tables.

**Price key**
Price keys arrange prices in different areas. A price key groups identical prices.

**Rate**
A rate is a combination of price year and key. In the application, e. g. in documents, the key defined as the standard key (allocated in the rate) will be used for a price year/list.

**Price list**
All price tables of a rate form the price list.

### Price List
Price lists are usually arranged in so-called years and for a certain area, e. g. standard for IG.

**(Fig. B-132 Price years)**
- **A Years**: The names of the price lists (e.g., Standard, Training Demo).
- **B Code**: Standard price tables for sales and purchase prices.
- **C Validity of the year**: The date range for which the price list is valid.
- **D Example**: Standard code for calculating sales prices.

A year (A) is a collection of price tables which are applied by default (B) for:
- **Sales prices (SP) for:**
  - IG
  - Single annealed
  - Processing
  - Shapes
- **Purchase prices (PP) for:**
  - Purchase prices (glass, articles)
  - Processing steps
  - Shapes

The defined validity is for information only.

### Price key
The price keys in A+W Business can be compared with the chapters of printed price lists. Keys are therefore used for grouping similar prices, e.g. single annealed, IG, purchase prices, sales price fixed sizes, sales price for boxes, processing prices, insurance prices.

### Definition of Rates
Rates are the combination of price years and keys. Even the year `<n.e.>` and the key `<n.e.>` can be combined to form a rate. Prices can only be entered for one of the defined rates (combinations).

**(Fig. B-133 Combinations of rates)**
This illustration shows that the price list SP 2012 is combined with various keys (Processing keys, Stock size keys, Standard keys) to form different rates (Rate A, Rate B, Rate C). These rates then link to specific price tables.

This illustration shows that the price list SP 2012 is combined with various keys to form different rates. Price tables in which the prices are defined, are allocated to the rates. If an item is entered in an order which includes the product IG, the price table from the corresponding rate will be used automatically, proposing the defined price.

In practice, allocation to a rate means that the standard key will always be applied when you choose a certain price list. You have to define a rate for every price list/key combination if this combination is going to be used for pricing. It does not matter whether this rate shall be used by default, or is only valid for a single customer.

**(Fig. B-134 Rates)**
- **A List of price years**
- **B Code for the standard year**
- **C List of price keys**
- **D Year for PP**
- **E Standard year**
- **F Standard rates**
- **G Rates**: Combinations of the year and different keys
- **H Number of the basic IG table**
- **I Cost calculation code**

This example shows that the price list **Standard (E)** and the price key **SP1 (C)** are linked to form a rate (G). When working with A+W Business this means that you can enter price tables and prices for this combination which will be used whenever this combination (rate) is selected.

Due to various rates being allocated, the **Standard** price list in this example includes several price lists (G).

Price list **PP (D)** is only allocated to the key **PP** in this example. This means that you cannot enter prices for the combination of price list **PP** and the key **Standard**.

You can also see that a price year each is marked as the standard (B) for sales or purchase price calculation. This means that these price lists will be suggested by default. These codes are adopted from dialog **Price list**.

#### Standard
The rate (the combination) is also marked as a standard (F). In the document or when entering discounts it can be replaced by another rate.
You can enter customer- or supplier-related rates.

#### Basic IG table
A+W Business calculates the IG prices by default based on an IG matrix for each of the standard structures, e. g. for IG with 2 x float 4 mm, 2 x float 6 mm, 2 x float 8 mm.

If you base the prices on a single matrix, using proportional surcharges and discounts for the different thicknesses and exchange lites, you have to create a new, so-called basic IG table.

The basic IG table is used for entering a matrix e.g. for 2 x float 4 mm and price unit sqm *without surcharge*. The (selected) number of this new basic IG table has to be entered in rate allocation, column **Basic IG table (H)** so that this is used for pricing. All other structures will be calculated using surcharges and discounts on the individual elements.

#### Production cost calculation
If you are using the supplement Production cost calculation you can also define the rate to be used for production cost calculation. The settings for production cost calculation are described in the software reference.
⇨ Software Reference, "Company Data > Calculation" on page B-1004

### Price Settings (Company Data)
Standard price calculation can be changed in company data.

**(Fig. B-135 Company data > Pricing)**
This tab shows numerous checkboxes (A) for defining the options for documents. Any changes on this tab will overrule the standard calculation in A+W Business.
For a detailed description of the checkboxes please refer to the software reference.

### Editing rates
Every price list/price key combination forms a rate. Definition of rates determines the standard rate to be used for pricing.
In documents, different rates can be defined by means of discounts or manual selection.

There are the following instructions on this subject.
- "How to define a rate" on page B-292
- "How to delete a rate" on page B-293

> **Prerequisite**
> Rates can only be defined if price lists and price keys have been entered before. Please note that even the price list `<n.e.>` and the key `<n.e.>` can be combined to form a rate.

#### How to define a rate
1. Go to **Master data > Prices > Rates**.
   The defined price lists and price keys are listed.
   **(Fig. B-136 Defining a new rate)**
   - **A Select price list**
   - **B Select price key**
2. Select the price list (A) and the price key (B) to be combined in a rate.
   A rate for purchase prices is defined in this example.
3. Go to the menu **Start > New** to switch to the input mode.
   **(Fig. B-137 Standard codes for the new rate)**
   - **A New rate**
   - **B Standard checkboxes**
   The new combination appears as a rate (A) in section **Rate allocation**.
4. Define the product types for which the new rate shall be used by default, by ticking the corresponding checkboxes (B), e.g. Stn. PP.
   With that, the standard rate for purchase prices has been defined.
5. Select in the menu **Start > Save** to save the data.
   The data will be saved. You can now enter prices for this rate.

#### How to delete a rate
> **Prerequisite**
> Rates can be deleted only if the corresponding prices have been deleted before. This does not include the prices used in documents.

1. Go to **Master data > Prices > Rates**.
   Dialog **Rates** appears with the defined price lists, price keys, and rates.
2. Choose the rate to be deleted.
3. Go to menu **Start > Delete**.
   The allocated rate is marked by an X.
4. Go to menu **Start > Save** and acknowledge the security check.
   The data will be saved. The rate has been deleted.

## Price Tables

### Objectives
- Introducing price tables for unit prices, shapes, and grills.
- Introducing price and quantity units.
- Defining prices.
- Copying and changing prices, completely or in part.

### Benefit
- Pricing consists of flexible modules which cover all calculation options. Price matrixes can be used for merchandise as well as for IG.
- The different pricing types can be allocated to the products at random.

### Note

**Price**
Prices are entered in price tables as unit prices or graduated prices.
- Unit prices e.g. valid for single items.
- Graduated prices are mainly used for glass, e. g. depending on the size.

**Price unit**
For every price you have to define the quantity to which the value refers, e.g. 5.80 € per sqm.
Price and quantity units (price/QU) are preset in A+W Business.

**Pricing**
Prices and discounts will be used for calculation only if the appropriate codes are set in the order.

**Grills**
Prices for grills are kept in special price tables where the price can be entered per grill element.

**Shapes**
Prices for non-rectangular lites are usually defined as surcharges for the product groups.

### Unit Price
Unit prices are entered on tab **Unit price** without a graduation, e. g. Float 4 mm per square meter, hinges per piece. In the actual order, the value from the price table is multiplied by the quantity of the allocated price unit and the item quantity.

**(Fig. B-139 Unit price (example))**
- **K Price type (here: unit price)**
- **L Defined prices**
- **M Undefined prices**
- **A Price table**
- **B Price list (year)**
- **C Price key**
- **D Price**
- **E Price unit to which the price refers.**
- **F Minimum price gross, net**
- **G Minimum quantity**
- **H Rounding (different from product definition)**
- **I Currency in which the price is kept**
- **J Minimum sizes**

This example shows the elements forming the unit price. Most of these details are also used for other price types.
Price definition can be extended by the following details (columns): Key text, next key, remark, other surcharges, different product group.

#### Price and quantity units
Price and quantity units are preset by A+W Business. These units cannot be deleted or extended. These units are allocated to prices, surcharges, reminder fees, and products.

**(Fig. B-140 Price and quantity units)**
- **A Quantity units for defining the price (price units)**
- **B Quantity units for defining the product**

This example shows fixed price and quantity units. In sections A and B you can see that the selection in the combo boxes is restricted to the price and quantity units valid for defining a price or product.
- Price units (A) are allocated to the corresponding prices in price management. The simplest price unit is the price per piece, e.g. for fittings. Other price units are based e.g. on the surface, the volume, or the working time.
- Quantity units (B) are allocated to the corresponding products in product management.

If you are using the Multi-lingual operation module, the units must exist on all languages tabs. They should be translated into the individual languages.
Quantity units can be added but will be ignored by the system.

### Shape Price
Shapes with all their necessary sizes are usually only entered in the order. It is therefore not necessary to draw up and maintain a price list for every possible shape.

Shape prices are usually defined as surcharges (C) on the glass price of a product group (A). These surcharges can be defined for all glass types of which shapes are produced. The general shape surcharge for single annealed glass is entered for the product group `<n.e.>`. For all other product types, different shape surcharges are entered, e.g. for tempered glass lites with shapes.

Shape surcharges can also be graduated by means of limit types (B). The price in this example is not graduated. The limit of 0.000 (D) defines that the surcharge is applied to all sizes.

**(Fig. B-141 Shape price)**
- **A Product group to which the price applies**
- **B Limit type**
- **C Unit: Proportional surcharge**
- **D Quantity limit**

### Grill Price
Grills are calculated either by linear meter or by field. Define how the price is composed, e.g. of grill, edge connection, and cross. Grill prices can also be graduated by means of limits, e.g. by linear meter.

**(Fig. B-142 Grill price)**
- **A Grill price element for which is valid**
- **B Price unit**
- **C Limit type**
- **D Price**

This example shows that the grills are calculated with a fixed price (D) per meter (B) for horizontal and vertical grills (A).

### The Copy Function
Dialog **Price management** allows copying and changing price lists, completely or partially. If you want to introduce new prices next year you can use the copy function to make the necessary preparations. Copy all price lists to a new year and change the prices. The rate is activated only from the day on which the new prices become effective.

> **Prerequisite**
> Please note that you have to enter price lists and price keys before you can copy prices to a new year.

The options for copying are:
- Transfer price tables to another price list or price key.
- Increase or reduction by a fixed amount.
- Increase or reduction by a percentage.
- Change a single or several price tables.
- Change the rounding.
- Transfer price lists, e.g. to a project or a customer.

**(Fig. B-143 Copy function for prices)**
The diagram shows three copy options:
1.  **Copy to partner/group**: Copies prices to a specific customer/group with a value adjustment (e.g., +2%).
2.  **Change within same rate**: Modifies prices within the existing rate.
3.  **Copy + change to new rate**: Copies prices to a new year and/or key.

This example shows three of the options provided by the copy function.
