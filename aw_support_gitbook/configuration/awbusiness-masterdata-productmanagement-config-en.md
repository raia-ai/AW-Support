---
title: "EN_AWBusiness_Master_Data_9_6-4"
source: "EN_AWBusiness_Master_Data_9_6-4.pdf"
tags: ["A+W Business", "Master Data", "Product Management", "Software Reference", "Glass Manufacturing", "ERP", "Configuration", "Pattern", "Coating", "Glass Types"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for managing product-related master data within the A+W Business ERP system. It covers the configuration of patterns, coatings, glass types, and detailed product management settings."
long_description: "This comprehensive software reference guide details the procedures for configuring product master data in the A+W Business software, a specialized ERP for the glass manufacturing industry. The document provides step-by-step instructions and explanations for various master data dialogs, accessible through the 'Master Data > Products' path. Key sections include defining 'Pattern' and its properties like price key and short name; 'Pattern Side' and 'Coating Side' for configuring surfaces of IG or laminated units; and 'Coating Type' to specify coating characteristics. It also covers the setup of 'Glass Type Groups' for production analysis and reporting. The guide explains how to manage 'Quality Text' to be printed on spacers, including basic settings and restrictions. Furthermore, it details the management of 'Declaration of Performance' templates and the creation of 'Exchange Groups' to control which articles can be substituted in BOMs. The core of the document is the 'Product Management' section, which breaks down the numerous tabs available for defining every aspect of a product, from basic article information, production parameters, pricing, stock management, bill of materials (BOM), and more. It serves as an essential resource for administrators and power users responsible for setting up and maintaining the product catalog in A+W Business."
---

---
## Products

### Pattern

**Master Data > Products > General > Pattern**

This dialog shows the possible patterns of the lites. You can edit the entries but cannot add further patterns.

| Price key | Short de... | Name |
| :--- | :--- | :--- |
| 0 | | keiner/none |
| 1 | S | senkrecht/vertical |
| 2 | W | waagerecht/Horizontal |
| 3 | X | beliebig/any |

**Price key**
The key (ID) is preset by A+W Business and must not be changed.

**Short name**
One-digit, alpha-numerical short name that can be changed if required.

> **Example**
> V = vertical
> H = horizontal

**Name**
Unique name for the sense of pattern.

### Pattern Side

**Master Data > Products > General > Pattern Side**

This dialog shows the possible pattern sides of the lites. You can edit and complete the entries to define all pattern sides for multiple IG or laminated glass. Every lite of an IG or laminated unit has two sides, pointing inward and outward respectively.
*⇨ Tutorial 1, "Patterns and Coating" on page B-160*

| Level | Short descr. | Name |
| :--- | :--- | :--- |
| 0 | | Keine Strukturseite/No pattern side |
| 1 | | Ebene/Level 1 |
| 2 | A | Ebene/Level 2 |
| 3 | | Ebene/Level 3 |
| 4 | A | Ebene/Level 4 |
| 5 | | Ebene/Level 5 |
| 6 | A | Ebene/Level 6 |
| 7 | | Ebene/Level 7 |
| 8 | A | Ebene/Level 8 |
| 9 | | Ebene/Level 9 |

**Level**
The numbers of the levels (sides in an IG structure) must not be changed. If you enter more levels please select consecutive numbers, following the same principle.

**Short name**
One-character, alpha-numerical short name for the inside and outside. Can be changed if required.

**Name**
Unique name of the level.

### Coating Side

**Master Data > Products > General > Coating Side**

This dialog shows the possible coated sides. You can edit and complete the entries to define all levels for IG lites. Every lite of an IG unit has two sides, pointing inward and outward respectively.
*⇨ Tutorial 1, "Patterns and Coating" on page B-160*

| Level | Short de... | Name |
| :--- | :--- | :--- |
| 0 | | Keine Beschichtungsseite/No coating side |
| 1 | | Ebene/Level 1 |
| 2 | A | Ebene/Level 2 |
| 3 | | Ebene/Level 3 |
| 4 | A | Ebene/Level 4 |
| 5 | | Ebene/Level 5 |
| 6 | A | Ebene/Level 6 |
| 7 | | Ebene/Level 7 |
| 8 | A | Ebene/Level 8 |
| 9 | | Ebene/Level 9 |
| 10 | A | Ebene/Level 10 |

**Level**
The numbers of the levels must not be changed. If you define more levels please select consecutive numbers, following the same principle.

**Short name**
One-character, alpha-numerical short name for the inside and outside. Can be changed if required.

**Name**
Unique name of the level.

### Coating Type

**Master Data > Products > General > Coating Type**

This dialog shows the possible coating types. You can edit and complete the entries.
*⇨ Tutorial 1, "Patterns and Coating" on page B-160*

| Price key | Short de... | Name |
| :--- | :--- | :--- |
| 0 | N | nicht beschichtet/uncoated |
| 1 | B | beschichtet/coated |
| 2 | W | weich beschichtet/soft coated |
| 3 | H | hart beschichtet/hard coated |

**Price key**
The key is preset by A+W Business and must not be changed.

**Short name**
One-character, alpha-numerical short name.

> **Example**
> U = uncoated or W = without

**Name**
Unique name of the coating type.

### Glass Type Groups

**Master Data > Products > General > Glass Type Groups**

This dialog is used to define groups of glass types. You will need glass type groups when working in A+W Production. The glass type groups in A+W Production match the product types in A+W Business.

| Price key | Name |
| :--- | :--- |
| 1 | Floatglas/Float glass |
| 2 | Floatglas farbig / Float glass coloured |
| 3 | Beschichtete Gläser / Coated glass |
| 4 | VSG-Zuschnitt |
| 5 | Ornamentglas / Patterned glass |
| 6 | ESG/Tempered glass |
| 7 | test |
| 8 | VSG/Laminated glass |
| 9 | Folien / Films |
| 10 | Alu |
| 11 | Isolierglas / IG |
| 12 | Dreifach ISO/Triple IG |
| 13 | Füllung / Filling |
| 14 | Sonst. Glasartikel / Misc. glass product |
| 15 | Parsol |
| 16 | Drahtornament/Wired patterned glass |
| 17 | Kunststoff |
| 18 | Sprossen/Georgian bars |
| 19 | Thermix |
| 20 | Gas / Gas |
| 21 | TPS |
| 22 | Ganzglastüren / Glass doors |

> **Example**
> 1 = Float
> 2 = IG
> 3 =

Each glass product can be assigned a glass type and a glass type group in product management, tab A+W Production. The definition of glass type groups in A+W Production serves for analysis purposes in reports and statistics. The glass type groups are irrelevant for the production batches.
*⇨ "Glass Types" on page B-633*

**Name**
Name of the glass type group, e.g. Float, toughened glass, laminated glass.

**Key**
1- to 7-digit number of the glass type group.

### Quality Text

**Master Data > Products > General > Quality Text**

Quality text is printed on the spacer depending on the IG structure and on the destination's country code.

> **Prerequisite**
> This dialog is only accessible if the appropriate function has been selected in Company Data > tab Documents.
> *⇨ "Product ID" on page B-932*

Dialog Quality Text offers the following tabs:
- Quality Text - Basic Settings
- Quality Text - Restrictions

#### Quality Text - Basic Settings

**Master Data > Products > General > Quality Text > Basic Settings tab**

This tab is used to define the (country-specific) quality text to be printed on the spacers.
*⇨Tutorial 2, "Text Types" on page B-461*

**Product selection**

- **Glass**: Glass article for which quality text has been defined.
- **Gas**: Gas inside the IG lite.

**Values**

- **Priority**: The priority defines which quality text should be used if an IG unit consists of different lites for which different quality text has been entered.
- **Country**: Quality requirements can differ from country to country. The country code allows defining different text for a lite, depending on the country.
- **Text**: Quality text to be printed on the spacer.

#### Quality Text - Restrictions

**Master Data > Products > General > Quality Text > Restrictions tab**

This tab can be used to restrict the automatic application of quality text. By means of a rule you define the product types or classes for which the quality text should not be used.

The fields in section Product selection are described in connection with the tab Basic settings.
*⇨ "Quality Text - Basic Settings" on page B-581*

**Validity**

- **Rule**: Valid rules are preset by the program.
- **Parameters 1-4**: The number of parameters that can be changed depends on the selected rule.

**Restrictions**

The list shows all rules plus the corresponding parameters for the selected glass.

### Declaration of Performance, Management

**Master Data > Products > General > Declaration of Performance Management**

This dialog serves to manage the templates for the declarations of performance. By combining Number, Name, and Language you can register a declaration of performance under the same number in different languages.

To create declarations of performance, the technical text can be stored in all required languages.
*⇨ "Technical Values" on page B-1044*

The dispatch of declarations of performance can be enabled per customer and product.

#### Declaration of performance

- **Number**: Number of the declaration of performance.
- **Name**: Name of the declaration of performance. It should be unique and descriptive.

#### File attachment

- **Language**: Language in which the declaration of performance is issued.
- **Link**: Path for saving the declarations of performance. By default, the declarations of performance are saved together in a directory with the file attachments. This directory is defined in company data.
  *⇨ "File attachments" on page B-932*
- **[Add], [Delete]**: These buttons can be used for issuing a language version of the declarations of performance or for deleting it from the list.

#### Overview

The overview lists all declarations of performance that can be allocated to the products or customers.

### Exchange Groups

**Master Data > Products > General > Exchange groups**

On this dialog, you create the exchange groups. You must assign the products that are approved for the exchange to these groups.
*⇨ "Exchange Allocations" on page B-585*

With these definitions, you specify that in IG and/or LG, only glass, spacers, and that only articles that are assigned to these groups can be exchanged.

You must activate the function in the company data.
*⇨ "Apply product exchange rules for BOM exchange" on page B-943*

In the master data for the products with BOM, you must specify the valid group:
*⇨ "Product Management – BOM" on page B-614*

- **Number**: Number of the exchange group.
- **Name**: Name of the exchange group.

### Exchange Allocations

**Master Data > Products > General > Exchange allocation**

On this dialog you allocate the products to an exchange group. Thus you specify which products may be used for the exchange.

In the master data for the products with BOM, you can specify the group with the permissible products.
*⇨ "Product Management – BOM" on page B-614*

With these definitions, you specify that in IG and/or LG, only glass, spacers, and that only articles that are assigned to these groups can be exchanged.

You must activate the function in the company data.
*⇨ "Apply product exchange rules for BOM exchange" on page B-943*

#### New data generation

- **Group**: Name of the exchange group. This field is only enabled if you allocate a product to a group. You create new exchange groups on the Exchange groups dialog.
  *⇨ "Exchange Groups" on page B-584*
- **Product**: Product that is allocated to the exchange group.

#### Product allocations

The overview displays all allocations. To change an allocation, you must delete the invalid allocation and create a new one.

### Classifiers - Product

**Master Data > Products > General > Classifiers > Products**
**Master Data > Partners > General > Classifiers > Products**

This tab is used for entering the names of product classifiers. That dialog is described in detail in the Market Partner section.
*⇨ "Classifiers" on page B-752*

Apart from the name and a comment you have to define the value that can be allocated to each classifier.
*⇨ "Product Management - Attachments / Classifiers" on page B-623*

## Product Management

**Master Data > Products > Products/Articles > Product**

A+W Business can handle your individual product structure. You may define any product number (up to 8 digits), as well as alphanumerical codes (matchcode up to 15 digits).

This section provides information on the following subjects:
- "Product Management Menus" on page B-587
- "Product Management" on page B-590
- "Technical Parameters" on page B-626
- "Copy Technical Parameters" on page B-628
- "Product Change" on page B-629
- "Product Code Management" on page B-630
- "Glass Types" on page B-633

### Product Management Menus

**Master Data > Products > Products/Articles > Product**

The product management menus allow to define the default settings for the dialog and open other dialogs without closing product management.

This section provides information on the following subjects:
- "Options Menu" on page B-587
- "Functions Menu" on page B-588

#### Options Menu

**Master Data > Products > Products/Articles > Product > Options menu**

You can use this menu to enter the standard settings for the dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog. The following entries are displayed:

- **Show all A+W Production transfer error reports together**: Errors occurring during the transfer of production data will be shown as one message.

#### Functions Menu

**Master Data > Products > Products/Articles > Product > Functions menu**

This menu can be used to open other dialogs without closing the present one.

**Technical Parameters group**
- **Technical parameters in general**: Opens the dialog Technical parameters for reading or editing technical parameters.
  *⇨ "Technical Parameters" on page B-626*
- **Technical parameters - IG**: Opens the dialog Technical parameters for reading or editing technical parameters for the selected IG.
  *⇨ "Technical Parameters" on page B-626*
- **Copy technical parameters**: Opens the dialog Technical parameters for copying technical parameters for the selected IG.
  *⇨ "Copy Technical Parameters" on page B-628*

**Price management group, SLS relevance group, PCH relevance group**
- **Load sales/purchase price management**: Opens the price management where the sales or purchase price of the selected product can be changed.
  *⇨ "Price Management" on page B-710*
- **Set for all BOM elements**: Enables the corresponding price code for all BOM elements.
  *⇨ "Product Management – BOM" on page B-614*
- **Remove for all BOM elements**: Disables the corresponding price code for all BOM elements.

**Print flag group**
- **Set for all BOM elements**: Enables the print code for all BOM elements.
- **Remove for all BOM elements**: Disables the print code for all BOM elements.

**A + W Production group**
- **Transfer selected products to A+W Production**: Transfers the data of the selected product to A+W Production.
- **Transfer all master data to A+W Production**: Transfers all glass type groups, glass types, jumbos, tables, and table allocations to A+W Production.
- **Import A + W Production master data**: adopts the master data from A+W Production.

**Changing/Deleting group**
- **Change selected products**: Opens the dialog Product amendment where the automatic surcharges for the selected product can be enabled or disabled.
  *⇨ "Product Change" on page B-629*
- **Delete selected products**: Deletes all products from the list.

**CE group**
- **Import CE master data**: This function is available only if the appropriate files are ready for import. These data are usually imported when A+W Business is installed and configured.

## Product Management (Dialog)

**Master Data > Products > Products/Articles > Product**

This dialog serves for managing your products, e.g. single annealed, IG, laminated glass, toughened glass, shapes, grills, processing steps, single articles like handles, etc.

Dialog Product management offers the following tabs:
- Product Management - Product
- Product Management - Production
- Product Management – Price/Surcharge
- Product Management - Stock/Purchase
- Product Management - Shapes/Processing
- Product Management – BOM
- Product Management - Text
- Product Management - Languages
- Product Management - A+W Production
- Product Management - Attachments / Classifiers
- Product Management - Grills

*⇨Tutorial 1, "Product data" on page B-133*

### Product Management - Product

**Master Data > Products > Product > Products/Articles > Product tab**

This dialog is used for defining and editing your company's products. Article numbers (up to eight digits) and the alpha-numerical matchcode can be chosen at random. Once the new product data have been saved, the article number cannot be changed.
*⇨Tutorial 1, "Product Definition" on page B-182*

#### Articles

- **Number**: Shows the article number (product number). When you enter new product data you can use the zoom function to view the free numbers.
  *⇨ "Free Numbers / Areas" on page B-788*
- **Matchcode**: The matchcode is used as a search criterion. It can consist of up to 15 alpha-numerical characters.
- **EAN**: EAN code or GTIN code. In the USA, this field can be used for the UPC code.
- **Name (1 to 3)**: Name and a short description of the product. The name appears at item entry and is analyzed for the printing of forms.
    - For single lites that are to be assembled in an IG unit, only the first name is read.
    - You can use variables (wildcards) for name 1 to show the validity of special discounts or surcharges (product allocation surcharges).
      *⇨ Tutorial 2, "Variables" on page B-465*
    - Variables (including formulas) can be used for name 3 for product type Processing. In the document, the system will replace these variables by the actual values of the processing parameters.
      *⇨ Tutorial 2, "Available Variables (Wildcards)" on page B-523*
- **[Formula]**: Opens the dialog Parameter exchange where you can select the valid parameters. Please obey the spelling if this field is used for formulas to make sure that A+W Business can interpret the text correctly.

> **Examples**
> 
> | Name 3 in dialog Product management | Name in dialog Item entry |
> | :--- | :--- |
> | `<%> Edges *<§>* with miter 45 polished (<=> lin.m.)` | `2 Edges *2/3* with miter 45° polished (2,45 r.m.)` |
> | `Sawing of <%> edges *<>*` | `Sawing of 3 edges *2/3/4*` |
> | `<%> holes, d = <$> mm` | `2 drill holes of d = 20 mm` |
> | `<%> drilling(s) x/y/D in mm *<§>*` | `2 holes x/y/D in mm *100, 100, 25- 200,200,16*` |
> | `<%> x <$> mm rounded corner *<§>*` | `4 x 15 mm rounded corner *1/2/3/4*` |
> | `<$> Corner cut-outs/<%> Pieces/*<§>*` | `100 x 75 corner cut-outs/2 pcs./3/4*` |
> | `<%> Edge(s) *<$>* with <$> mm bevelling` | `2 edge(s) *1/4* with 20,0 mm bevelling` |
> 
> *⇨ Sales, "Parameter Replacement" on page C-587*

- **Short info**: Short information for the printing of labels (maximally 20 characters), e.g. IG 2 x FL4 for IG 2 x float 4 mm or FL4 for float 4 mm.
- **Article info**: Field for additional, product-related information (no character limitation). This information can be displayed at item entry.
- **Display**: The text from field Article info can be displayed at item entry.
    - The text will not be displayed automatically.
    - When the product is entered, dialog Article info opens automatically so that the BOM structure and prices can be checked.
- **Display in BOM**: The text from field Article info can be displayed in the bill of material, e.g. in case of an exchange.
    - The text will not be displayed if the product is used in a bill of material.
    - If the checkbox Display is checked, the text will be displayed at item entry only if the product is entered as the main product.
    - The text will be displayed even if the product is a BOM element.
- **[Info icon]**: Opens the dialog Article info where you can check the product details.
  *⇨ Sales, "Product Information" on page C-600*
- **[Variations icon]**: Opens the dialog Product variants for checking or entering product variants.
  *⇨ "Variants/Colors" on page B-571*

#### Properties

- **Product type, Product class**: Each product is allocated a product type and a product group. They serve as search criteria and can be used for analysis as well as for the pricing of shape surcharges.

> **Examples**
> 
> | Product type | Product class | Product |
> | :--- | :--- | :--- |
> | Single annealed | Single annealed<br>Patterned glass | Float 6 mm<br>Patt. Altd. straight 4 mm<br>Patt. Cathedral white 4 mm |
> | Processing | Rounded corners<br>Notches | Rounded corner, fine<br>Rounded corner, rough<br>Edge cut-out - 100 x 200 mm TG |
> | TG | Toughened glass<br>Glass door system | Toughened clear 12 mm<br>Toughened door white |
> | IG | IG | CLIMALIT Standard 2 x 4 mm float |

*⇨ "Product Types" on page B-564*
*⇨ "Product Classes" on page B-565*

- **PGR**: Any of the three product group levels can be allocated to the product. To distinguish e.g. IG and IG with shapes you have to allocate a PGR to the shape. Then define a PGR combination for every analysis for distinction. If you need no differentiating analysis please enter 0. The shape will be automatically allocated to the main product's product group, i.e. IG or single annealed glass.
  *⇨Tutorial 1, "PGR Combination" on page B-143*
  *⇨ Software Reference, "Combined PGR" on page B-568*
- **PGR Statistics**: Generally, the same PGR is entered here as in field PGR. PGR statistics allows defining different product group structures for discounts and statistics.

#### Units / Restrictions

The following sizes are used for the loading of racks and for technical or price restrictions.

- **Thickness / Grill thickness**: For glass, this is the glass thickness and for grills, the thickness of the grill in mm.
- **Weight**: Weight of the glass per quantity unit. In the order, the weight serves for surcharge calculation, e.g. for transporting very heavy items.
> **Example**
> 1 mm float glass weighs 2.5 kg per sqm
> 5 mm float weighs 5 x 2.5 kg = 12.5 kg per sqm

- **Width/height min.**: Minimum width and height for item entry. These values will be checked at item entry. If they are not met, a message to that effect will appear. In that case, the order can be rejected or produced with another product or an appropriate surcharge, e.g. for manual cutting.
- **Surf./Max. aspect ratio**: Maximum surface and aspect ratio for item entry. An aspect ratio of 1:6 means that e.g. with a width of 600 mm, the height must not exceed 3600 mm. These values will be checked at item entry. If they are exceeded, a message appears proposing an alternative article. It can be rejected or accepted. If the alternative article is rejected, the order cannot be produced.
  *⇨ "Alternative article" on page B-595*
  Tab Price/Surcharges allows entering a surcharge to be applied if the sizes are exceeded. The entries for surface and aspect ratio should correspond with the appropriate entries on tab Price/Surcharges.
  *⇨ "Product Management – Price/Surcharge" on page B-601*
- **Standard width / height**: The entries here will be suggested at order entry. They can be changed in the order.
- **Quantity unit**: The quantity unit (size unit) is the unit to be used for this product at order entry and pricing.
> **Examples**
> - **sqm**: Order entry by quantity, width, and height.
> - **pcs**: Order entry by quantity; the fields for Width and Height are locked.
> - **lin.m.**: Order entry by linear metres (quantity and metres). The length is entered in field Height in m (meters).

*⇨ "Price and Quantity Unit" on page B-700*

- **Lock code**: Options for the lock code are:
    - **Not locked**: The product can be entered in the order.
    - **Locked**: The product does not appear in the product search and cannot be entered in the order. A message appears if the product number is entered at item entry.
    - **Replicated**: If master data are only kept in the master database (DB), data can be updated by replication. Master data with the code replicated cannot be edited in the slave database.

#### Alternative Article/ External Key

- **Alternative article**: The alternative product is automatically suggested at order entry if certain restrictions have been violated for instance. A message to that effect is displayed.
- **External key**: External key for communicating with other programs, e.g. for transfer to production or financial accounting.
- **External statistics key**: External key for data exchange with an external software for statistical evaluation.

#### Article Sketch

- **File name**: File name of the sketch allocated to the product. This product sketch can be printed in the document only if the checkbox Print on form is checked. This sketch does not represent the shape or the fitted bars. It is therefore only useful for rare patterned glass types. The path is entered in Company data > System. tab
  *⇨ "Path for product images" on page B-975*
- **Print on form**: The article sketch can be printed on forms.
    - ☐ The sketch will not be printed on forms.
    - ☑ The sketch will be printed on forms.

### Product Management - Production

**Master Data > Products > Product > Products/Articles > Production tab**

This tab is used for defining the parameters for production, e.g. the patterned side or the use in a bill of materials. The fields in section Article are described in connection with tab Product:
*⇨ "Product Management - Product" on page B-591*

#### Shaping+Nesting - Parameters

- **Edge quality**: The edge quality has to be allocated to the product to make sure that the correct edgework will be performed. Apart from the standard qualities, further (individual) qualities can be selected that have to be known by the same number on the shop floor.

#### BOM Parameters

- **BOM irrelevant for production**: The BOM can be transferred to production.
    - ☐ The BOM is transferred to production. Choose this setting if the entire product structure is produced internally. In that case you can modify the BOM at order entry, e.g. exchange a lite.
    - ☑ The BOM will not be transferred to production. Choose this setting if you do not produce e.g. a laminated glass lite yourself. The laminated lite is a purchased article in this case. The supply type P.O. must be set on tab Stock/P.O. in that case.
      *⇨ "Procurement type" on page B-608*
- **Suitable for IG**: A product may be unsuited for an IG structure.
    - ☐ The product should not be used for IG.
    - ☑ The product can be used for IG.
- **Rotatable pattern level**: For patterned glass, you have to define whether the patterned side can be fitted pointing inward or outward. This setting does not apply to coated glass. If the lite is fitted on the inside or on the outside, the button Pattern level is enabled at item entry. This applies to patterned glass. There are special buttons for coated glass at item entry.
    - ☐ The pattern level cannot be changed. The glass must always be fitted on the standard level defined in section Pattern.
    - ☑ The lite can be fitted anywhere. At item entry, BOM tab shows the standard level that can be amended.
      *⇨Tutorial 1, "Sense of pattern" on page B-160*
      *⇨ "Pattern, Coating" on page B-599*
- **Print on BOM**: The BOM product can be printed on the form.
    - ☐ The product will not be printed in the BOM.
    - ☑ The product is identified as a BOM element on the printout.

#### Default Values for Different Quantities

If you are using commercial surplus you can define a percentage of the defined quantity that can be produced as surplus for every product. This applies to shortfall as well.
You have to specify in customer data whether the customer in question will accept different quantities.

- **Shortfall, surplus**: Percentage, e.g. 10%. The quantity produced may be 10% below or above the quantity entered in the order. These values can be adjusted per customer.
  *⇨ "Exceeds Amount" on page B-847*

#### Spacer code

You can define further codes for products of the product group Spacers. The spacer code in the variant overrides the code defined in product master data.
- **Free**: Currently not used.
- **Seal type**: Edge seal type, e.g. UV edge seal. The entry is preset by A+W Production.
- **Spacer type**: Number of the spacer type, e.g. for stainless steel, TPS, aluminium. The number is preset by A+W Production.
- **Color**: The color is preset by A+W Production.

#### Production Parameters

- **AW-Broke**: External key that is transferred to AWBroke and A+W CAD Designer (Shapes). There is a total of eleven external keys, some of which are preset. The following codes are defined for the known glass types:
    - G01: float
    - G02: toughened glass
    - G03: laminated glass
    - G04: patterned glass
    - G05: wired glass
    - G06: IG
    - G07: glass door system
    - G53: interlayer
    - G99: Meta element
> **Example**
> G028000
> This is a toughened lite with product number 8000.
The whole key consists of the letter (= code), the numerical part of the product number, and a dot. This permits e.g. to define processing steps for individual glass types apart from the standard processing. External keys for colors are set at the start of the external key for glass.
> **Examples**
> - GF10.028000: Toughened glass, the color belonging to F10, product number 8000.
> - KGF15.02111: Polishing of toughened glass with the color belonging to F15.

- **Optimization key**: The key is transferred to A+W Production for classification. You can enter an alternative product number (key) that is used for booking in the combined stock management mode.
  *⇨ "Optimization" on page B-868*
  *⇨ Inventory Management, "Stock bookings for combined stock control" on page G-38*
- **Pattern**: These fields are enabled only for Grills or leaded designs. You can select the required pattern. The entry is transferred to A+W Production. Enter the pattern in the first field and the Grill type in the second field.
  *⇨ Tutorial 1, "Grill construction types" on page B-162*
  *⇨ "Grill Types" on page B-572*
- **Width, height size allowance**: Code for processing allowances or deductions. Valid allowances and deductions are defined in dialog Size allowances.
  *⇨ "Size Surcharge" on page B-639*
  The size allowance compensates the loss of material resulting from the different processing steps. The size allowance is taken into account for cutting.
> **Example**
> By polishing all four edges, a float lite of 1000 x 1000 mm shrinks to a size of 998 x 998 mm.
> The size allowance is defined as 2 mm. The lite will be cut to a size of 1002 x 1002 mm.

#### Pattern, Coating

- **Side**: For patterned and coated lites, the patterned or coated side (level) is defined. This detail can be changed in the order.
> **Example**
> The pattern side of a patterned lite for example is on the outside by default. Should the pattern be required to be on the inside, an "inside pattern" surcharge will be applied in most cases.
> For coated glass, the pattern will have to be on the inside for reasons of production.

*⇨Tutorial 1, "Patterns and Coating" on page B-160*

- **Sense of pattern**: The sense (of pattern) is defined for patterned lites. This detail is required for cutting.
  *⇨ "Pattern" on page B-576*
- **Type**: The coating must be on top so as to avoid damages from the roller conveyors on the cutting table. This is especially important for soft and medium-hard coating. Hard-coated lites can also be loaded the other way.

#### Printing

- **Shape sketch, Grill sketch**: You can print schematic or true-to-scale sketches of shapes or Grill patterns on the forms. The settings for printing can be made in product management, at item entry, and in management of forms. In product management, printing can be permitted or prevented. The Tutorial describes the interaction of the settings.
  *⇨Tutorial 2, "Printing sketches" on page B-479*

#### Countersunk hole

You can enter several countersunk drillings with different values, e.g. as default settings for different glass types, or as a processing product.

- **Type**: The type defines whether the countersunk hole should be on the inside and/or on the outside.
- **Angle**: Drilling angle. It is defined at right angles to the glass surface. An angle of 0° represents a straight edge.

**Fig. B-31 Countersunk hole (both sides)**
- A: Edge
- B: Diameter
- C: Sinking depth

- **Input type**: The input type defines the size to be entered in the order for the countersunk hole.
