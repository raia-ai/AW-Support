---
description: "EN_AWBusiness_Master_Data_9_7-2"
---


# Product Management

---
## Technical Parameters

> Master Data > Products > Product > Products/Articles > Functions menu > group: Technical Parameters > Technical parameters in general, technical parameters for IG

*Fig. B-41 Technical Parameters*

Enter the technical parameters for glass products in this dialog.

### Different glass structure

**1st glass, 2nd glass, 3rd glass**
These fields remain blank for single annealed products. For IG products, the appropriate lites are entered.

**Spacer, gas**
Technical values per IG table and spacer.

**Name**
Name of the glass structure.

### Technical values

The following field names can be adapted to your company's requirements in dialog System text (system text no. 111–118). The descriptions are valid for the technical parameters in product management and product search.
⇨ "System Text" on page B-1041

**Ug value in W/sqm**
Heat transmission coefficient (system text 110). The Ug value is the central measure for determining the heat loss in a construction element. The unit of measure is W/sqm K. The smaller the Ug value, the higher the thermal insulation.

**Ug value according to DIN 4108-4**
Thermal resistance

**Light transmission in %**
Light transmission. The light transmission ratio expresses the directly transmitted, visible radiation in a wave length from 280 to 380 nm, referring to the light sensitivity of the human eye. The reference unit of 100% refers to an unglazed hole in the wall.

**g value in %**
Total energy transmission ratio %. This value consists of the direct solar energy transmission and of the secondary heat emission towards the inside due to long-wave radiation and convection. The g value is the secondary parameter after the k value.

**b factor**
Average transmission factor. It represents the average transmission factor for solar energy referring to the total energy transmission ratio of a 4 mm lite. It is necessary for calculating the cooling load of a building.

**Sound insulation factor in dB**
The sound insulation factor is the main effect of sound insulation.

**Thickness tolerance in mm**
The thickness of insulated glass can vary by a few mm. Enter the tolerance in mm.

**Size tolerance mm (<200 cm), (>=200 cm)**
The size of insulating glass can vary by a couple of centimeters. Enter the corresponding tolerance in cm.

**(Combo box)**
You can define a surcharge on the Ug value if grills are fitted in the IG unit. The following settings are available:
- **No grills in airspace**: There will be no surcharge on the Ug value.
- **Grills in airspace, single (+0.1)**: For a common IG unit with grills, the Ug value will be raised by 0.1.
- **Grills in airspace, multiple (+0.2)**: For multiple IG with grills, the Ug value is raised by 0.2.

At order entry, the Ug value is automatically adapted to the number of grills.

## Copy Technical Parameters

> Master Data > Products > Product > Products/Articles > Functions menu > group: Tech-nical parameters > Copy technical parameters

*Fig. B-42 Copy Technical Parameters*

This dialog is used for copying the technical values and applying them to another product.

### Options

The options define how existing parameters in the target product should be treated:
- **Update existing parameters in the target**: Parameters existing in the target product will be changed. Additional parameters from the source product will be adopted.
- **Delete all parameters in target**: The parameters in the target product will be deleted first. After that, the parameters from the source product will be entered.

## Product Change

> Master Data > Products > Product > Products/Articles > Functions menu > Change selected products

*Fig. B-43 Change allocation of automatic surcharges*

This dialog serves to change the allocation of automatic surcharges. The allocations always apply to all products displayed on tab Table.

### Surcharges/discounts

This section shows the surcharges and (special) discounts defined in dialog Product allocation.
⇨ "Surcharge Product Assignment" on page B-1024

Choose an option to specify how the selected surcharges/discounts should be handled:
- **Set**: The selected surcharges or discounts will be enabled for all products selected in product management.
- **Delete**: The selected surcharges or discounts will be disabled for all products selected in product management.

## Product Code Management

> Master Data > Products > Product > Products/Articles > Stock/Purchase tab [different product codes]

This dialog is used to define different supply types if you are using internal orders and internal invoicing. The corresponding clients and/or order areas must be defined.
⇨ "Company Data - Client" on page B-918
⇨ "Order Areas" on page B-1014

This dialog offers the following tabs:
- Product Code Management - Editing
- Product Code Management – Copy

### Product Code Management – Editing

> Master Data > Products > Product > Products/Articles > Stock/Purchase tab [different product codes] > Edit

*Fig. B-44 Product code management – editing*

This tab allows to define and edit the product codes.

**Product**
This group shows the product number and the name of the current product.

**Area, code**
You can define the supply type for different clients and/or order areas.

> **Example**
>
> The order areas IG, toughened glass, and laminated glass user internal orders. All order areas use the same database, the same master data, etc.
> An order is entered in the IG area; the IG unit consists of a laminated lite with toughened glass, a spacer, and a float lite.
>
> - For order area IG, the IG unit is Production, the laminated lite is Purchased while the float lite is Cut.
> - For order area laminated glass, the laminated lite is Production, the toughened lite is Purchased, and the float lite is also Cut.
> - For order area toughened glass, the toughened lite is Production, and the float lite is Cut.
>
> The different supply types for laminated glass and toughened glass thus have to be defined by different product codes.

**Client**
Client for whom the different codes should be valid.

**Order area**
Order area for which the different codes should be valid.

**Procurement type**
Different procurement type for the defined client or order area.

**Stock booking type**
Different stock booking type for the defined client or order area.

**Valid for**
Choose an option to define where the settings should be valid:
- **Other**: The allocation is not restricted to one of the two other options.
- **Order entry**: The settings are valid for order entry. See the example.
- **Profit center**: The search for the code is restricted to a client or an order area. Profit center invoicing must be enabled in Company data > tab Production for this purpose.
- **Search all**: The option is enabled only in selection mode. This option does not restrict the search any further.

**Overview**
The list shows all products for which different codes have been entered.

### Product Code Management – Copy

> Master Data > Products > Products/Articles > Article > Stock/Purchase tab [different product codes] > Copy

*Fig. B-45 Product code management - copy*

This tab is used for copying the settings for a product to a product group and/or a sequence of products.

**Source**
This section shows the data for the selected product. The fields are described in connection with the tab Edit.
⇨ "Product Code Management - Editing" on page B-630

**Target**
This section is used to define where the product code should be copied to. You have to enter at least one product group or product type.

**Product group**
You can choose a PGR, MPG or PSG.

**Product type, product class**
After choosing a product type you can also define a product class.

**from product no. - to**
You can choose a single product by entering the same product number in both fields. If you enter different product numbers, the product code will be applied to all products between the first and the second number defined.

**Client**
Client to whose products the different code should be copied.

**Order area**
Order area the products of which should get the different code. You can also choose the allocation:
- **Other**: The allocation is not restricted to one of the two other options.
- **Order entry**: The settings are valid for order entry.
- **Profit center**: The settings apply to a client or an order area. Profit center invoicing must be enabled in Company data > tab Production for this purpose.

## Glass Types

> Master Data > Products > Product > Products/Articles > A+W Production tab > field [Glass type]

*Fig. B-46 Glass types*

Enter all relevant data for the current glass type in this dialog. The glass types can be allocated in the following dialogs:
- **Product management**: If you allocate a glass type to a glass product, the fields Product type and Product class are disabled and cannot be changed any more.
⇨ "Product Management - A+W Production" on page B-619
- **Glass type jumbo tables**: Every glass type can be allocated to a cutting table to make sure that the cuts are made correctly. Laminated glass e.g. must be allocated to the table capable of cutting this glass type.
⇨ "Glass Type - Jumbos - Tables" on page B-872

### Values

**Glass type**
Number of the glass type. The glass type number usually matches the A+W Business article number.

**Name**
Name of the glass type.

**Product class**
Product class and product type to which the glass type belongs.

**Glass type group**
Glass type group to which this glass type belongs.

**Pattern**
Sense of pattern for this glass type.

**Coating**
Coating type for this glass type.

**Table**
The table lists all glass types defined (in A+W Enterprise).

## Products

> Master Data > Products > Product

A+W Business allows defining your company's own products as well as data for production.

In addition to product management, menu Articles offers the following entries:
- "Stock Sizes" on page B-635
- "Size Surcharge" on page B-639
- "Product Variants" on page B-641
- "Cost Calculation" on page B-645
- "Spacer Restrictions" on page B-647
- "Template Editor" on page B-649
- "IG Structure" on page B-650
- "Processing Restrictions" on page B-652
- "Patterns" on page B-653
- "Shape Edge Qualities" on page B-654
- "Fitting Allocation" on page B-655
- "¡TOE Rules" on page B-657

## Stock Sizes

> Master Data > Products > Product > Stock sizes

You can enter the stock sizes for pricing purposes. These stock sizes are not identical with the stock articles kept in stock management.

This section provides information on the following subjects:
- Functions Menu
- Stock Sizes - Product
- Stock Sizes - Table

### Functions Menu

This menu gives access to the Stock management dialog where you can enter the selected product as a stock size (stock article) for stock management.
⇨ Inventory Management, "Stock Management" on page G-185

### Stock Sizes - Product

> Master Data > Products > Products> Stock sizes > Product tab

*Fig. B-47 Product management: stock sizes - products*

This tab serves to enter the stock sizes for pricing purposes. You can also enter stock sizes that are not actually stored. Each stock size can be allocated a sales and a purchase price code as well as a product group.

> **Stock management**
> The stock sizes for stock management are entered in dialog Stock management (module Stock management). A detailed description of stock sizes can be found in section Stock Management:
> ⇨ Inventory Management, “Stock Sizes" on page G-39
> ⇨ Inventory Management, "Stock Management" on page G-65

**Articles**
This section shows the article number (product number) and the name of the product in question.

**Units / Restrictions**

**Cont./width/height**
For boxes, enter the number of lites; the width and height is defined in mm.

**PGR, PGR statistics**
Every stock size or box can be allocated to different product groups.
⇨ Tutorial 1, "Product Groups" on page B-142

**Price**

**Price key SP, PP**
All price codes for sales (SP) and purchasing (PP) entered in price master data are offered for selection. A separate price key should be defined for boxes.

**PU search stock**
A product can be taken into account for calculating the average purchase price.
- The product will not be taken into account for calculating the average price.
- The product will be taken into account for calculating the average price.
⇨ Inventory Management, "Purchase Price and Average PP" on page G-49

**Name**

**Name, Short descr.**
Name and short description for a (better) distinction from the cut size. The names appear at order entry, e. g. Box Float 4 LM. This product name will be printed on the forms.

**Flag**

**Procurement type**
The procurement type defines how the product is to be acquired for this order.
- **Production**: The stock size will be produced. If a main article has got this procurement type, its BOM elements can be defined as stock articles or purchased articles.
⇨Tutorial 1, "Procurement Type" on page B-171
- **Cutting**: The glass is cut from stockplates.
- **Stock withdrawal**: The product is kept on stock, with just this size or as a unit.
- **Processing**: The processing steps for an order item are transferred to production.
- **Customer's own glass**: The product is supplied by the customer and will be used to produce his orders.
- **Ρ.Ο.**: Only the product in question will be ordered, irrespective of the contents of the BOM.
- **P.O. (complete)**: The product is ordered, including all processing steps.
- **Addition to stock through production**: The product should be used in work orders only to fill up the stock. The produced items will be added to stock.
⇨ Tutorial, "Production Orders" on page E-128

The procurement types are described in detail in connection with product master data.
⇨ "Product Management - Stock/Purchase" on page B-606

**External statistics key**

**External key**
External key for communicating with other programs, e.g. for statistical analysis.

**Available stock sizes**
The list shows all stock sizes for the current product number. These stock sizes are used for pricing.

### Stock Sizes - Table

> Master Data > Products > Product > Stock sizes > Table tab

*Fig. B-48 Product management: stock sizes - table*

This tab lists all products matching the search criteria in selection mode. The field descriptions apply to both tabs.
The fields are described in detail in connection with the Product tab.
⇨ "Stock Sizes - Product" on page B-636

## Size Surcharge

> Master Data > Products > Product > Size Allowance

You can draw up tables for size-related allowances and enter different levels per table.
Dialog Size allowances offers the following tabs:
- Size Surcharge - Size Allowances
- Size Surcharge - Table

### Size Surcharge - Size Allowances

> Master Data > Products > Product > Size Surcharge > Size Allowances tab

*Fig. B-49 Size Surcharge - Size Allowances*

This tab is used for entering the steps for size-related allowances and reductions.
Choose an option to define how the table should be analyzed.
- **Allowance table**: A size allowance compensates the loss of material resulting from processing. This size will be taken into account for cutting.
- **Reduction table**: A size reduction is e.g. needed for picture frames.

> **Example**
> By polishing all four edges, a float lite of 1000 x 1000 mm shrinks to a size of 998 x 998 mm.
> You have to enter a size allowance of 2 mm. This value is taken from the allocated table, taking into account the glass thickness.

Size allowances are allocated in Product management to the products of product type Processing (not to glass).
⇨ "Product Management - Production" on page B-596

**Table (overview)**

**Up to thickn.**
You can define for every table - step by step - up to which thickness a certain value should be added.

**Value**
The value defines the size in mm that has to be added or deducted for the thickness in question.

### Size Surcharge – Table

> Master Data > Products > Product > Size Surcharge > Table tab

*Fig. B-50 Size Surcharge – table*

This tab serves to draw up new tables for size-related allowances or reductions.

## Product Variants

> Master Data > Products > Product > Variants

You can enter product variants for the products, e.g. for spacers, grills, and units. Colors are not allocated to the lites. Different glass colors are represented by different products.
This section provides information on the following subjects:
- "Functions Menu" on page B-641
- "Product variants – Variants" on page B-641
- "Product Variants – Table" on page B-643

### Functions Menu

This menu gives access to dialog Copy variants where you can transfer the product variants from one product to another.
⇨ "Copy Variants" on page B-644

### Product variants – Variants

> Master Data > Products > Product > Variants > Variants tab

*Fig. B-51 Product variants - variants*

This tab is used to define variants for the products entered in product management, e.g. other colors, different polishing or frosting, etc. Every product variant can be allocated to a price table.
⇨ Tutorial 1, "Definition of Product Variants" on page B-207

**Product**

**Number**
Product number or range of product numbers for which this color is valid.

**EAN**
The EAN code appears only if a single product has been selected.

**Name**
Shows the product name and description.

**Product type, product class**
Shows the product type and the product class allocated to the product.
⇨ "Product Management - Product" on page B-591

**Variant**

**No./Variant**
Variant number and name defined in dialog Variants.
⇨ "Variants/Colors" on page B-571

**Price table**
You can define different price tables for every product and variant.
⇨"Prices" on page B-713

**Weight**
Specific weight of the variant if the weight of this variant differs from the weight of the product. The weight is usually irrelevant for products with variants, which is why it is set to zero by default.

**Default**
If a certain product variant is frequently required, it can be generally displayed first at order entry.
- The product variant will not be shown first by default.
- The product variant will be automatically suggested for input. This setting can be changed at order entry.

**Locked**
A variant can be locked for input in product management and in documents if it is no longer needed.
- The variant can be allocated.
- The variant is locked and cannot be allocated. If it has been allocated to products and in documents, it will still be shown however.
⇨Tutorial 1, "Locks" on page B-34

**PGR, PGR statistics**
Each product variant can be assigned different product groups.
⇨ Tutorial 1, "Product Groups" on page B-142

**Code, procurement type**
The procurement type of the product variant can differ from that of the product.
⇨Tutorial 1, "Procurement Type" on page B-171

**Spacer code**
You can define further codes for products of the product group Spacers. The spacer code in the variant overrides the code defined in product master data.

**Free**
Currently not used.

**Color**
The color is preset by A+W Production.

**Avail. product variants**
The list shows all variants for the individual products, and the allocated price tables.

### Product Variants – Table

> Master Data > Products > Product > Variants > Table tab

*Fig. B-52 Product variants - table*

This tab shows all product variants matching the search criteria in selection mode.
The fields are described in connection with tab Variants.
⇨ "Product variants - Variants" on page B-641

## Copy Variants

> Master Data > Products > Product > Variants > Functions menu > Copy variants

*Fig. B-53 Copying of product variants*

This dialog is used for transferring the variants from one product to another.

**Source, target**
Enter the product from which the variants should be copied, and the product to which they should be copied.

**Overwrite existing records**
If variants have already been defined for the target product you have to decide whether these should be kept or changed.
- The existing variants will be kept and completed by the new variants from the source product. Identical variant numbers will not be changed.
- The variants of the target product will be overwritten by those from the source product. Additional variants will be added. Existing variants will not be deleted.

## Cost Calculation

> Master Data > Products > Product > Cost calculation

*Fig. B-54 Settings for cost calculation - BOM*

This dialog is used for the settings for calculating the primary costs for insulated glass (IG). Define the average consumption of butyl, Thiokol, etc. by airspace (AIR).
Tab BOM serves to enter the values for primary cost calculation.

### Spacer Product

**Article/MCode, Name**
Number, matchcode, and name of the spacer the primary costs of which should be calculated.

**Cutback (single)**
Cutback for the spacer.

**Expanded volume for gas**
Expanded volume of sound protection gas as per manufacturer's specification.

### BOM product

This section provides details of the products that are used in connection with the spacer.

**Product**
Number of the product.

**Name, Quantity unit**
Shows the name and the quantity unit, e.g. for Butyl.

**Consumption per - Reference unit**
Quantity and unit the consumption refers to.

> **Example**
> Quantity unit (Butyl): kg
> Consumption: 0.0055
> Reference unit: lin.m.
> Calculation: 0.0055 kg Butyl is used per meter of spacer.

⇨ Tutorial 2, "Complex Example: IG Calculation" on page B-545

**BOM**
The list shows all products that were added as elements to the spacer. Data will be displayed only if a spacer has been selected on tab Table.

**Table (overview)**
List of products matching the search criteria or for which a certain consumption of Butyl, drying agent, edge seal, etc. has been defined.

## Spacer Restrictions

> Master Data > Products > Product > Spacer Restrictions

*Fig. B-55 Spacer restrictions*

This dialog is used for defining restrictions for certain spacers. Not all of the structures used for common IG can be used with TPS IG (Thermo Plastic Spacer).
If restrictions are not met at order entry, you have to use another product.

### Identification

**Product class**
Spacer restrictions are generally necessary for TPS IG. You can also choose other product groups however.

**Password**
If a password has been entered, the restriction can be changed in the order. In this case, the password is checked at order entry. If no password has been entered, the system automatically uses the alternative product defined in the group If validity is violated go to.

**Rule**
The rules have been defined with variables the values of which are loaded from the parameter fields. [N1], [N2], and [N3] apply to parameters 1 to 3. The rules are fixed. Please contact a member of the A+W Software GmbH service team in case you need additional rules.

### Validity

**Parameters 1-3**
Fields for the values that are inserted to the rule by means of variables. The fields are released according to the selected rule. If a rule without variables has been chosen, no fields are released, e. g. for rule 3114 – Shapes must not include grills.
For certain rules, there is a combo box for parameter 1 from which the corresponding restriction can be selected.

**If validity is violated go to**
An alternative product can be used if the defined parameters are violated.

**Product class**
Selection for the product class that can be used if the restriction is violated.

**Variant**
In addition to the product group you can define a variant for the alternative product.

**Restrictions**
List of defined restrictions and parameters.

## Template Editor

> Master Data > Products > Product > Template Editor

*Fig. B-56 Template Editor*

You can select a template for shape input from this dialog. The editor can be used to edit the A+W CAD Designer (Shapes) templates or draw up new templates for processing.

**Directory**
Templates can be kept in various directories. The last used directory will be shown automatically.

**Templates**
Offers a list of templates saved in the selected directory.

> **A+W CAD Designer manual**
> There is a special online help as well as a special manual for working with A+W CAD Designer.

## IG Structure

> Master Data > Products > Product > IG Structure

*Fig. B-57 IG structure*

Use this dialog to enter the key numbers for a clearly defined structure of IG units.
The numbers can be printed on the spacers. Based on this key number, the structure of a completely produced IG unit can be determined based on the corresponding order.
This dialog is released only if the Quality code function is enabled in Company data > tab Documents.
⇨ "Product ID" on page B-932

**Key number**
Key number to be assigned to the corresponding IG structure.

### Glass Structure

**1st glass, 2nd glass, 3rd glass**
Product numbers of the lites that form the double or triple IG unit.

**Spacer thickness**
Width of the spacer.

**Gas**
Gas type (if the airspace of the IG unit is filled with gas).
