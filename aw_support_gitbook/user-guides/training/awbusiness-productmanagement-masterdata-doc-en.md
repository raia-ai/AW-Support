---
title: "Product Management – Price/Surcharge"
category: "training"
product: "AWBusiness"
doc_type: "Documentation"
language: "EN"
tags: ["AWBusiness", "ProductManagement", "MasterData", "Doc"]
version: "1.0"
last_updated: "2025-12-10"
description: "title: "EN_AWBusiness_Master_Data_9_7-1" source: "EN_AWBusiness_Master_Data_9_7-1.pdf" tags: ["A+W Business", "Product Management", "Master Data", "ERP", "Software Reference", "Price Surcharge", "Stock Management", "BOM", "Shapes Processing"] version: "1.0" last_updated: "2025-10-03" short_description: "A technical reference guide for the Product Management module in A+W Business software. This document details the configuration of products, including pricing, surcharges, stock, purchasing, bill"
source_file: "AWBusiness-ProductManagement-MasterData-Doc-EN.md"
---


title: "EN_AWBusiness_Master_Data_9_7-1"
source: "EN_AWBusiness_Master_Data_9_7-1.pdf"
tags: ["A+W Business", "Product Management", "Master Data", "ERP", "Software Reference", "Price Surcharge", "Stock Management", "BOM", "Shapes Processing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical reference guide for the Product Management module in A+W Business software. This document details the configuration of products, including pricing, surcharges, stock, purchasing, bill of materials (BOM), shapes, processing, and integration with A+W Production."
long_description: "This document serves as a comprehensive software reference manual for the Product Management section of A+W Business Master Data. It provides detailed explanations for each tab and field within the product/articles master data interface. The guide covers critical areas such as setting up price and surcharge parameters, managing stock and purchasing data (including CPIP and P.O. parameters), defining complex shapes and processing steps, and configuring Bill of Materials (BOM) for IG or laminated lites. It also explains how to attach texts, manage multilingual product descriptions, handle attachments and classifiers, define grill patterns, and configure settings for A+W Production integration. This manual is intended for system administrators and power users responsible for maintaining product master data, ensuring accurate pricing, production planning, and order processing within the A+W software ecosystem."
---

# Product Management – Price/Surcharge

**Navigation**: Master Data > Products > Product > Products/Articles > Price/Surcharge tab

*Fig. B-32: Product management – Price/surcharge*

This tab is used for allocating the surcharges that should be automatically applied to the product.

The fields in section **Article** are described in connection with tab **Product**:
⇨ "Product Management - Product" on page B-591

### Apply Surcharges/Discounts

This field lists the automatic surcharges.
- The surcharge will not be charged.
- The surcharge will be charged.
  ⇨ Tutorial 1, "The Function of Automatic Surcharges" on page B-325
  ⇨ "Surcharge Product Assignment" on page B-1024

### Tax

Every product is assigned the tax code 1 by default. You can choose a different one if required. In some countries it is possible to assign several tax rates, e.g. in North America. If tax is not enabled, no tax will be applied to the product in question, e.g. for product down payment. The actual tax rates are maintained in dialog Tax.
⇨ "Tax" on page B-903

### Cost Accounting

**Cost type, cost center**: You can allocate a cost type and a cost center to every product for cost accounting purposes. The data can be analyzed by means of external reports.
The settings can be changed at order entry.
⇨ "Cost Mode" on page B-912
⇨ "Cost Centers" on page B-913

### Price Parameters

**Display of prices**: The product price can be shown in different ways on a form:
- **Implicit**: The main item's net price includes all prices of the BOM elements, i.e. shape and exchange surcharges as well as processing.
- **Explicit**: The prices of the BOM components are listed separately.
- **Implicit, price per quantity unit**: The prices of the BOM components are converted to the main product's price unit. This total price is shown in the document, but only if all BOM components of the item have been assigned with the same display type.

**Adopt main item**: If the product is included in a BOM, calculation and display of the prices and discounts can depend on the settings that have been made for the product of the main item. The following settings can be applied:
- **No adoption**: The price settings will not be adopted from the main item.
- **Discount + price key**: Discount and price key will be adopted from the main item.
- **Discount**: Only the discount will be adopted form the main item.
- **Price key**: Only the price key will be adopted from the main item.
- **No adoption (net for ind.pr.main itm)**: For customized net prices, the settings should not be adopted from the main item.
- **Discount + price key (net for ind.pr.main itm)**: For customized net prices, the discount and price key should be adopted.
- **Discount (net for Ind.pr.main itm)**: For customized net prices, only the discount will be adopted.
- **Price key (net for ind.pr.main itm)**: For customized net prices, only the price key should be adopted from the main item.
- **Discount + price key (even if discount exists)**: Discount and price key will be adopted from the main item even if a discount has been defined for the BOM product, e. g. when a lite is replaced.
- **Discount (even if discount exists)**: The discount should be adopted from the main item even if a discount has been defined for the BOM product, e. g. when a lite is replaced.
- **Price key (even if discount exists)**: The price key should be adopted from the main item even if a discount has been defined for the BOM product, e. g. when a lite is replaced.

For further information on adopting discounts also see:
⇨ "Discount Management - Exchange Discounts" on page B-809

> **Settings for pricing in company data**
> Dialog **Company data > Pricing** tab serves to make general settings that can partially override the settings in product master data.

**Sales / purchase price table**: Numbers of the price tables that will be used to calculate the sales price and the purchase price.
The products and the corresponding prices are defined separately. Product number and price table number are usually the same. A distinction makes sense only if lots of different products have the same price.
⇨ Tutorial 1, "Price Tables" on page B-230

**[Price table]**: Opens the dialog for editing prices.
⇨"Prices" on page B-713

**Basic product**: Number of the price table that is used as a basis for calculation if BOTH lites of an IG unit are replaced. If a price table has been defined, the system will automatically ask at order entry whether the basic table should actually be used.
If no lite or just one lite is replaced, the program will fall back on the entry in field **Price table**.

**Exchange surcharge table**: Number of the table for exchange surcharges. Every IG table can be allocated an individual exchange surcharge.
⇨ Tutorial 1, "The Function of Exchange Surcharges" on page B-288
⇨ "Exchange Surcharges" on page B-666

**Shortfall surcharge**: Number of the surcharge for shortfall.
You can define a surcharge on glass that is applied whenever the minimum quantity (surface) defined for the order is not met. The shortfall surcharge must be defined as a Product allocation surcharge.
⇨Tutorial 1, "The Function of Automatic Surcharges" on page B-325
⇨ "Surcharge Product Assignment" on page B-1024

**Miscellaneous surcharge**: Other surcharges can be applied for different reasons, e. g. a surcharge for an edge length over 3760 mm since this length is hard to handle.
⇨ Tutorial 1, "The Function of Miscellaneous Surcharges" on page B-306
⇨ "Miscellaneous Surcharges" on page B-664

**Surcharge type**: Surcharge types define the basis on which the corresponding surcharge should be calculated:
- **current processing**: For the selected BOM element.
- **all previous processing steps**: For all processing steps executed before the selected BOM element.
- **all previous items**: For all elements listed in the BOM before the selected element.
- **Basic item**: For the top element (product) on the BOM to which a surcharge can be allocated as well.
- **Basic item without other surcharges**: For the top element on the BOM without the surcharge that may be allocated to the product.
- **Basic item + processing**: For the top item on the BOM and all corresponding processing steps.
- **Basic item + shape**: For the top element on the BOM and the corresponding shape.
- **Basic price**: For the price of the top element of the BOM.
- **Parent + its lites**: For the top element of an assembly (parent) and the lites of this assembly.
- **Parent + its previous processing**: For the top element of an assembly (parent) and the processing attached to this element.
- **Previous BOM, same parent**: (previous BOM with same parent). All elements of the assembly.
- **previous processing**: All processing steps listed above the element for which the surcharge has been defined.

All surcharge types can be calculated additional or non-additional. The alternative **non-additional** only refers to proportional surcharges. Depending on the setting, a value is created that serves as a basis for calculating the proportional surcharge.
⇨Tutorial 1, "Calculation by surcharge type" on page B-311

**Size rounding width/height**: Pricing in Germany is based on rounding to thirty. This means that calculation is based on the next edge length that can be divided by 30. In France, calculation is based on rounding to 10 for example.

> **Example**
> Rounding 30:
> For a lite of 1000 x 1000 mm, a surface of 1.04 (= 1020 x 1020) will be calculated.

**Max. surface**: Maximum surface for which the regular price will be calculated. This value will be checked at item entry. If it is exceeded, the defined Other surcharge (oversize surcharge) will be applied.
The entries for the surface and the aspect ratio (in the next field) should match the respective entries on tab Product.
⇨ "Surf./Max. aspect ratio" on page B-594

**Max. aspect ratio**: Maximum aspect ratio. This value is entered as a ratio of 1: x. This means that with a width of 600 mm, the height must not exceed 3600 mm.
If this ratio is exceeded, the defined miscellaneous surcharge will be applied.

**Average waste**: This value will be considered for calculating the purchase price of glass, gas (loss), and the reserved stock.

> **Example: Waste = 5%, PP = 8.00 €/sqm**
> 
| Lite: | | PP: |
| :--- | :--- | :--- |
| 1000 x 1000 mm | | 8.00 € |
> 
| Lite: | Waste: | Calculated surface: | PP: |
| :--- | :--- | :--- | :--- |
| 1000 x 1000 mm | 0.05 sqm | 1.05 sqm | 8.40 € |

⇨ Inventory Management, "Purchase Price and Average PP" on page G-49

**Processing Index**: The processing index evaluates the work involved and the difficulty of processing the product. This field is only enabled for glass products.
The processing index can be entered as a limit type for the price.
⇨Tutorial 1, "Limit Types for Graduations" on page B-249

**Sales, purchase price relevant**: The product can be taken into account for calculating the sales and/or purchase price. For BOM products, this checkbox refers to the main item.
- The product will not be taken into account for calculating the sales and/or purchase price in the order. You can use this setting if the product will be used as a BOM element in which case the price is calculated for the main product, e. g. film layers as part of a laminated lite.
- Pricing will use the corresponding sales and/or purchasing price table.
This setting is irrelevant for lites in IG units that are exchanged in the order because pricing will be based on the defined exchange prices in this case.
⇨ Tutorial 1, "Pricing Codes" on page B-168

**Suited for discount, cash discount**: Defines whether a discount or cash discount can be applied to the price in the order. Both settings can be changed in the order.
- No discount or cash discount will be considered for price calculation. Even if a discount has been entered for a product group, you can define at this point that it should not be granted. The same applies to cash discounts.
- A discount and/or cash discount can be granted for the order.

---

# Product Management – Stock/Purchase

**Navigation**: Master Data > Products > Product > Products/Articles > Stock/Purchase tab

*Fig. B-33: Product management - Stock/purchasing*

This tab serves to define the parameters for purchasing and stockkeeping of the product.
The fields in sections **Articles** and **Properties** are described in connection with the **Product** tab.
⇨ "Product Management - Product" on page B-591

### CPIP data

The fields in this section are enabled only if CPIP creation is active in company data. To make sure that the data can be correctly entered and checked, the appropriate files must be imported when installing and configuring A+W Business.
⇨ "CPIP creation" on page B-951

**CE relevant**: Irrespective of the CE code, the CPIP data can be marked.
- The CPIP code is irrelevant for the CE code.
- The CPIP code is part of the CE code.

**Certification**: Certification valid for this product. The certificates have to be defined in the master data for CE codes. Valid options are:
- **Self-defined**:
    - **All product types**: The CPIP code can be created; the CE relevant elements must not be deleted.
    - **Single annealed, laminated glass**: The CPIP code is removed by replacing or adding CE relevant elements.
    - **IG**: When CE relevant elements are replaced, the search for the CPIP code begins again. If the replaced elements are not checked by the IG CPIP search, the CPIP code will be removed.
- **Certified, Certified with size restriction**:
    - **All product types**: The CPIP code has to be created; CE relevant elements must not be deleted.
    - **Single annealed, laminated glass**: CE relevant elements must neither be replaced nor added.
    - **IG**: The entries cannot be saved if no CPIP code is found.

⇨ "CE Code" on page B-1079

**Type**: Select the product type.

**CPIP code**: CPIP code for the product. The code is checked at entry against the setting in field **Certification**.
⇨ "CPIP Code" on page B-1079

### SAP Product Identification

**Material type**: Number of the material type specified in SAP for this product.

**Product code**: Product number specified in SAP for this product.

**Statistics code**: Number of the analysis SAP uses for this product.

### P.O. Parameters

**Maximum width, maximum height for the P.O.**: These values define the maximum size of the lite for purchasing.
If this size is exceeded in the order, the item can neither be produced in-house nor ordered from an external supplier.
The maximum size for stockkeeping may lie below these values. These sizes are entered in section **Parameters stock control**.

### Product Codes

**Procurement type**: The procurement type defines how the product is to be acquired for this order:
- **Production**: The order item will be produced in-house. If a main article has got this procurement type, its BOM elements can be defined as stock articles or purchased articles.
  ⇨Tutorial 1, "Procurement Type" on page B-171
- **Cutting**: The glass for this order item is cut from stockplates. The data will be transferred to production.
- **Stock withdrawal**: The product is kept on stock, with just this size or as a unit. The defined quantity will be reserved at order entry.
- **Processing**: The processing steps for an order item are transferred to production.
- **Customer's own glass**: The product is supplied by the customer and will be used to produce his orders.
- **P.O.**: Only the product in question will be ordered, irrespective of the contents of the BOM. If a laminated lite consists of a float lite, a film, and a toughened lite for instance and only the toughened lite is marked as P.O., only the toughened lite will be ordered from the supplier. The laminated unit will be produced in-house.
- **P.O. (complete)**: The product is ordered, including all processing steps defined in the BOM. If a laminated unit consists of single annealed 5 mm, an interlayer, and toughened glass 5 mm, the laminated unit will be ordered as a whole. Please note the difference from the code P.O.
- **Addition to stock through production**: The product should be used in work orders only to fill up the stock. The produced items will be added to stock.
  ⇨ Tutorial, "Production Orders" on page E-128

**Stock booking type**: The stock booking type defines how a product is kept as a stock article in stock management:
- **Size-dependent**: Choose this setting if stock sizes are to be kept as units. This setting only makes sense for glass. The quantity unit should still be set to sqm on tab Product to make sure that the surface is calculated.
- **Not size-dependent**: Choose this setting for all stock articles to be kept with their actual quantity unit, e.g. units, fittings. Use this setting also for glass that is to be kept in sqm.
- **Combined**: Choose this setting if you are using reports from the shop floor. This setting only makes sense for glass. Please remember to define a virtual stocksize without sizes for this purpose.

⇨Tutorial, "How should stock be managed" on page G-15
The setting w/o will not be used in this context.

**Automatic Cutting**: This code is transferred to A+W Production.
- A+W Production will add the lite to the list of special cuts. This lite will not be cut by a machine but by hand.
- A+W Production passes the lites on to the cutting line while optimising the cutting process.

**No availability check**: You can use the **Stock info** dialog to check for every product whether the current stock on hand is sufficient for the orders on hand. Restricting the availability check to the products actually kept on stock will increase the performance of your system.
- An availability check will be made for this product.
- The availability of this product will not be checked. The product does not appear in dialog **Stock info**. This setting is useful if you are storing this product but it is not kept as a stock article.

**Technical article number**: For the procurement type **Cutting**, you can enter an alpha-numerical article number per glass type/thickness combination. This number is usually preset by A+W Production.

**Different product codes**: Opens the dialog **Product code management** where you can choose another product code, e. g. from another order area.
⇨ "Product Code Management" on page B-630

### Stock Control Parameters

**Maximum width, maximum height on stock**: Maximum size for stockplates that can be kept on stock. All order items up to the defined maximum size can be produced from the stock on hand.
You have to distinguish the parameters for **Purchasing** and **Stock control**. Orders items the size of which lies between those defined in Stock control and those for Purchasing, can be ordered from a supplier. If the size exceeds the P.O. parameters however, the article in question can neither be produced nor ordered from a supplier.

### Product Code

**CE code**: You can enter a CE code for (the standard structure of) the product. The CE code is adopted for the order and can be printed on the forms. At transfer to production, it can be transferred to A+W Production.

> **CE code for glass supplied**
> When you order paid toughening, the CE code for the glass is loaded from master data. The buyer must pass on the CE code of the basic glass to his supplier (toughening company). This way, the supplier can confirm CE conformity too.

---

# Product Management - Shapes/Processing

**Navigation**: Master Data > Products > Product > Products/Articles > Shapes/Processing tab

*Fig. B-34: Product management - shapes/processing*

This tab serves for specifying the data for shapes and processing that is assigned to a lite by sales.

> **Product type and product class for shapes**
> A+W Business distinguishes standard shapes and the shape for stepped IG. Product group and shape number have to be defined accordingly. Standard shapes use shape numbers 1-99 and the shape number for stepped IG is 999.

The data that can be entered on this tab are described in detail on tab Sales:
⇨ Sales, "Items - Processing" on page C-466
⇨ Sales, "Items - Stepping" on page C-485
⇨ Sales, "Items - Curved glass" on page C-486
⇨ Sales, "Items - Leaded designs" on page C-488
⇨ Sales, "Items - Shape template" on page C-489

### BOM
Processing steps can be carried out on individual components of the BOM. Details about shapes always refer to the main product.
The view shows a sketch of the shape. The key defines the fields in which the sizes are entered.

### Processing
**Buttons**: Use the buttons to select a product group, e. g. shapes, processing, curved glass or leaded glass. If different products have been assigned to the product group, you can select and adopt the requested product in the Select dialog.

**Article**: Product number and name according to the master data.

**Formula**: Select and display the formula for the processing text.

### Shape
**Symbols**: Use these buttons to select a shape.

**Article**: The product number of the shape is adopted from the master data.

**Shape**: The shape number is adopted from the master data.

**Name**: The shape name is adopted from the master data.

### Parameters
**W, H**: Only the fields necessary to produce the shape will be enabled for each shape. The view shows the names of the edges.

**Restrictions**: This section provides details on the restrictions. Example: `H1>0` means that edge H must not be 0.

**S+N file**: If you frequently enter a certain shape with identical sizes, you can save it as an S+N file. In future orders, you can select this file using the [Directory] button and assign it to the order item without having to enter the details every time.
If you have selected shape 99, you can also load and assign an S+N template.

**Printing sketches**: You can define how the shape will be printed:
- **No printout**: The sketch will not be printed on the forms.
- **Shape (true to scale)**: True-to-scale shape sketches will be printed.
- **Shape (sketch)**: Standard sketches will be printed. They only show the outline of the shape.

### Prices
**Year/key**: Price year and key for the shape surcharge are adopted from the master data. It can be changed if required.

**Price / PU**: Price and price unit for the shape surcharge are adopted from the master data. It can be changed if required.

**Discount**: The discount for the shape surcharge is adopted from the master data. It can be changed.

**Net**: The net amount for the shape surcharge is displayed automatically.

---

# Product Management – BOM

**Navigation**: Master Data > Products > Product > Products/Articles > BOM tab

*Fig. B-35: Product Management – BOM*

This tab shows the BOM for IG or laminated lites. It also provides information on the BOM elements.
⇨ Tutorial 1, "Edit BOM Structure" on page B-185
⇨ Tutorial 1, "Define Production BOM Breakdown" on page B-189

### BOM

The list shows all BOM elements. The level defines the product to which the element has been added. When you select an element, its details appear in the appropriate fields. The fields for the top level (main product) remain blank.

### Production BOM Breakdown

The list shows all processing steps that can be performed for this product. By checking the checkboxes you define whether the processing should be applied to the main product or to the BOM element. If no checkboxes are checked for the BOM elements, the processing steps are performed for the main product.

> **Example**
> For a laminated lite you have checked edgework for the BOM elements. The edges will therefore be processed before the lite is assembled. If a logo is required as well, this will be applied to the main product, i.e. to the laminated lite.

This setting can be changed at order entry.
Please also refer to the settings in company data to be adopted for exchange lites.
⇨ “Maintain production BOM structure in case of changes" on page B-940

### BOM Articles

The fields in this section are accessible only if a BOM element has been selected. The fields will remain inaccessible if you select the top level (main product).

**Article number, name**: Every BOM element is defined as a product, with its own article number and name.

**Quantity/width/height**: The quantity refers to articles, e.g. including three fittings in the delivery.
The standard entry in the fields **Width** and **Height** is zero. You can enter the sizes e. g. for standard doors (toughened glass). These sizes can be changed in the order.

**Diff. PGR, PGR statistics**: The product group of a BOM element can differ from the main item's product group. You can select e. g. a product group combination in this case to analyse the elements together.
⇨ Tutorial 1, "PGR Combination" on page B-143

**Pattern level, sense of pattern, coated side**: The entries apply to the selected BOM element only. These fields are described in connection with tab **Production**.
⇨ "Product Management - Production" on page B-596

**Supplier, name**: The BOM element is ordered from the defined supplier by default. This setting can be changed for the order, the item, and in the P.O. pool.
⇨ "Supplier List" on page B-854
⇨ Purchasing, "Purchase orders" on page D-41

**Procurement type**: This setting refers to the selected BOM element. The procurement type is described in connection with the tab **Stock/Purchasing**.
⇨ "Product Management - Stock/Purchase" on page B-606

**Sales price, purchase price relevant**: The entries apply to the selected BOM element only. These two checkboxes are described in connection with the tab **Price/Surcharge**.
⇨ "Product Management - Price/Surcharge" on page B-601

**Print**: For every element you can define whether it should appear on the BOM when forms are printed.
- The element will not appear on the BOM on the form.
- The element will appear in the BOM on the form.
⇨Tutorial 2, "Form Management" on page B-472

**Group for BOM exchange**: Selection of valid exchange group. This selection defines that only those products can be installed that are assigned to the selected exchange group.
If no exchange group is selected, all products can be exchanged.
⇨ "Exchange Allocations" on page B-585

---

# Product Management - Text

**Navigation**: Master Data > Products > Product > Products/Articles > Text tab

*Fig. B-36: Product management - text*

This tab serves to allocate text that can be displayed in the order. Spacer text can be transferred to production.
⇨Tutorial 2, "Text Types" on page B-461
⇨ "Text" on page B-1040

The fields in section **Article** are described in connection with tab **Product**:
⇨ "Product Management - Product" on page B-591

### Standard texts

The allocated standard text must be product-related. It will be printed on the form only on item level, in connection with the corresponding product.
At item entry, an icon for allocated text appears in the line header of the item display.
This text code defines the documents/forms on which the text should appear.
⇨ Tutorial 2, "Text Codes and Standard Text" on page B-463
⇨ "Text Code" on page B-1039

### Spacer text

Spacer text is printed on the spacers of IG lites. The text must be entered in dialog **Text**.
⇨Tutorial 2, "Spacer Text" on page B-462
⇨ "Text" on page B-1040
You can enter a special spacer text for every IG unit. The text number can be freely assigned.

---

# Product Management - Languages

**Navigation**: Master Data > Products > Product > Products/Articles > Languages tab

*Fig. B-37: Product management - Languages*

If you are using the Multi-lingual operation module, enter the foreign-language names of all products on this tab. The appropriate name will be selected by means of the customer's language code and will be printed on the forms.
⇨ "Partner Management - Address" on page B-759

---

# Product Management - A+W Production

**Navigation**: Master Data > Products > Product > Products/Articles > A+W Production tab

*Fig. B-38: Product management - A+W Production*

This tab serves to define the master data that can be transferred to production. This tab is accessible only if you are using A+W Production and if the appropriate link has been set up in company data. The data from this tab will be transferred to A+W Production by master data adaptation.

> **Change A+W Production data**
> Master data are set up when A+W Business is installed, and is transferred to A+W Production. Please contact a member of the A+W Software GmbH service team if there are entries that need to be changed.

The fields in section **Article** are described in connection with tab **Product**:
⇨ "Product Management - Product" on page B-591

### A+W Production glass parameters

**Glass type**: The current glass product is allocated to a glass type. The file symbol is used to open the **Glass types** dialog where you can enter glass types.
⇨ "Glass Types" on page B-633

**Grinding group**: Grinding and processing requires a size allowance for the edges so that the lite can be processed to the required size. Grinding allowances depend on four factors:
- Glass type
- Machine
- Processing type
- Glass thickness
To avoid having to enter a separate surcharge for every single glass type, machine, and processing, these criteria are combined in groups in A+W Production. The following groups are available:
- Standard
- Article grinding groups
- Machine grinding groups
- Processing grinding groups

**Transition time**: For some products, a rest time must be kept before the product can be passed on to the next process, e. g. after toughening. This time is entered in whole days. This entry will be overruled by the values from capacity planning.

**[Glass type jumbo tables]**: Opens the dialog Glass type jumbo tables. This button is accessible only for single annealed that is to be cut.
⇨ "Glass Type - Jumbos - Tables" on page B-872

**Max. subplate width**: Input in mm. Limits the width of the resulting subplates. This entry depends on the width of the stockplate. For automatic breakout lines, the manufacturer's directions apply. This limitation is necessary to facilitate manual breakout on the one hand while on the other hand, automatic breakout lines can only handle subplates up to a certain width at the dynamic breakout station.

**Min. distance X-Y cuts**: Minimum distance between X and Z cuts. A Z cut runs between two Y cuts, parallel with the X cut. The minimum distance mainly depends on the glass thickness and is necessary for manual breakout.

**Optimization sequence**: Sequence in which detailed scheduling processes the optimizations. Depending on the master data settings, this is in ascending or descending order. High-priority glass types will be optimized first. The priority of expensive glass types is usually high.

**Min. surface autom. opti.**: Minimum surface to be optimized. This entry can be changed by detailed scheduling.

### Position on the cutting table

**Pattern position**: Position of the pattern when the lite is cut. This detail is essential if the patterned lite can be cut only on one side.

**Coating position**: The coating usually faces upwards so as to avoid damages from the roller conveyors on the cutting table.

### Machine center

The fields in this section will not be analyzed because machine allocation is controlled by A+W Production.

**Number / logical**: Currently not used.

**Time in seconds**: Currently not used.

### Trim

The trim defines the minimum trim that must be available on the lite so that the cut lite can be broken.

**Shape**: Trim for shapes. This entry depends on the glass thickness and the shape itself.

**Left, Right, Top, Bottom**: Trim for rectangular lites. The entries depend on the glass thickness.

### A+W Production processing parameters

The fields in this group are only accessible for processing.

**Process. sizes included**: Especially for stepped lites one needs to check whether processing sizes are included to make sure that the calculation of further processing sizes produces the correct results.

**Correct cutting dimensions**: Currently not used.

**Explicit planning**: The product can be scheduled separately. If a processing is marked as explicit, the corresponding product (glass) is marked as a so-called release element. In A+W Production, release elements can be removed from the BOM and can be planned separately. In case of an IG unit, the lites to be processed are release elements.

**In-house processing**: In-house processing creates a new (A+W Production) element, e.g. cutting, toughening.

**Purchase processing**: A processing step can be purchased if it cannot be performed in-house. This must be taken into account in production planning because this will interrupt the production process.

**Processing type**: Processing steps are joined in different processing types, e.g. cutting, arrissing, polishing. Choose the processing type to which the current processing step belongs.
Processing type 99999 - Pseudo processing must be selected for the step article (product type Shape, product class Step).

**Coating position**: On coated lites, some processing steps can be executed just on one side. Define the coated side.

**Plan text**: The planed text for lites appears in A+W Production. Plan text can be adopted several times, by priority (priority 1 being high and 10, low).

**Plan priority**: Priority for importing the plan text.

**Sequence**: Processing sequence. This number defines when the processing should be executed. Cutting is represented by 1 because this is always the first work step for glass.

**Surcharge group**: Size surcharge group for edgework that belongs to the processing step. Surcharge groups are entered and managed in A+W Production.

**Valid element type**: Currently not used.

---

# Product Management - Attachments / Classifiers

**Navigation**: Master Data > Products > Product > Products/Articles > Attachments/Classifiers tab

*Fig. B-39: Product management - attachments/classifiers*

This tab serves for attaching external files to provide further information on the product. You can edit the values.

The fields in section **Article** are described in connection with tab **Product**:
⇨ "Product Management - Product" on page B-591

In the product search and in the order search, it is possible to search for classifiers.
The classifiers are always created on the level of the main product. During entry, they are taken over into the BOM.

> **Example**
> That is, if for the float glass 104 the classifier Suitable for IG is entered with the value Yes, then all products that contain the product 104 in the BOM will take over this classifier if a corresponding item is entered in the order.
>
> ⇨ "Partner Management - Classifiers" on page B-772
> ⇨ Tutorial 1, "Enter a Classifier" on page B-74

### Classifiers

This list shows all classifiers that can be allocated to the product.
- **A (alpha-numerical)**: To make an entry here, open the dialog **Classifier value allocation** by double-clicking on the **Value** field.
  ⇨ "Classifier Value Allocation" on page B-798
- **N (numerical)**: You can make this entry right in the **Value** field.
- **D (date)**: You make this entry directly in the **Value** field.

### File Attachment

Drag the external file you have selected in Windows Explorer into this field. This establishes the link.
Linked files must not be moved to different directory.

**Comment**: You can enter or select a comment on the linked file in this column, e.g. regarding its contents.

### Declaration of performance

You can allocate a declaration of performance to the product, to be transferred by default. In the order, you can change this declaration of performance for the item, e.g. after a lite has been exchanged.

**Number (number)**: Number of the declaration of performance.

**Declaration of performance required**: Certain products may require a declaration of performance.
- The declaration of performance does not have to be transmitted.
- The declaration of performance has to be transmitted.

---

# Product Management - Grills

**Navigation**: Master Data > Products > Product > Products/Articles > Grills tab

*Fig. B-40: Grill pattern in an IG product*

This tab is used to enter a grill pattern. The selected pattern is shown as a sketch when you select a grill from the sections horizontal, vertical grills.

The data that can be entered on this tab are described in detail on tab Sales:
⇨ Sales, "Items - Muntins" on page C-491

