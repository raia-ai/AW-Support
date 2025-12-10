---
description: "EN_AWBusiness_Sales_4_5-3"
---


---
## Item Data

> **i**
>
> **Total order price**
> The total order price is shown in the title line of the dialog.

**Prop. surch. (PP, SP)**
Displays the proportionate redistributed footer surcharge, e. g. energy surcharge.
The footer surcharges are recalculated specific to the item. Footer surcharges in a P.O. are saved in the costs of the order.
Redistribution can be disabled in the Options menu.
*⇨ "Options menu" on page C-441*

**CM**
Contribution margin of the item. In this display, this means the proceeds minus the costs (including proportionate PP footer surcharges). The fields are completed after the item is saved.

**CM in %**
Percentage of the contribution margin. This is the ratio of the contribution margin and the proceeds.

**Unit costs**
The contribution margin is calculated from the master data for pricing (PP).

**PP**
The total purchase price for the selected item is calculated from the master data and the quantity.
Display of the purchase price (PP) depends on the option selected in company data, Trade or Producer.
*⇨ Master Data, "Customer version" on page B-971*

**Proceeds**
Sales price for the item plus proportionate footer surcharges (SP).

**Unit price**
Unit price for the selected item including all components. It is calculated based on the price unit, surcharges and discounts. Possible components include e. g. also processing, shapes, etc.

**SP**
Total sales price of the selected item. This can be changed. The changes are applied to the total sales price, the unit price, and the price(s) per price unit. This field is locked if the display is switched to Purchase prices.

**Price relevant SP, PP**
You can define whether the price of the selected item will be considered in the sales and/or purchase price calculation. The standard setting is adopted from the master data.
- [ ] The price will not be taken into account for sales and/or purchase price calculation.
- [x] The price will be taken into account for sales and/or purchase price calculation.

**Price code**
If distinctive features have been defined for the entered item in product definition, the corresponding icons will be shown in red. Click on the corresponding icons to disable the default settings.
- **M**: Minimum calculation
- **/**: Individual price
- **O**: Other surcharge
- **S**: Stock size
- **C**: Cost and surcharge calculation
- **F**: Formula price

**Net SA/PU**
Specification of the net prices for SA and PU per square meter. The entry applies to the current item.

**Customer item**
The item that has been defined by the customer. This usually refers to a consignment specified by the customer.

**Consignment**
Customer consignment defined by the customer. This information can be printed on the shipping list and stock list by product group.
*⇨ "First reference on dispatch list" on page C-722*
*⇨ "Print first reference of order" on page C-726*

## Items

You can select or disable the display of columns via the table properties. The most important columns in the standard order are described in the following.
*⇨ Tutorial, "Order Items" on page C-57*
*⇨ Tutorial, "Automatic Input" on page C-90*

If ordered articles have been provided to Purchasing, the corresponding text is displayed in the Note column. If you change the ordered item you must also change the referenced order.

If you have entered a down payment using the option Down payment invoice with items, the item values are displayed in blue.

If the line header shows a text icon, you can display and edit the stored text by means of the tab of the same name.
*⇨ "Items - Further details" on page C-503*

**Item**
The item number is automatically incremented at entry. New items will always be added; they cannot be inserted.

**Product**
The Product field can be used to enter the item in different ways:
- Enter the product number.
- Enter the matchcode.
- Enter the product via the product search [magnifier].
- Select an existing macro.

**Product search**
The product can be selected via the search.

**Macro search**
The product can be selected via the macro search.

**Thickness**
The total thickness of the individual lites, including film layers, spacers, etc. If you enter a different total thickness, A+W Business will check if a suitable spacer is available.

**Customer item**
The item that has been defined by the customer.

**Consignment**
Customer consignment defined by the customer.

**Description 1, 2, 3**
Product names for the main product.

**Unit**
The quantity may be preset from the previous item. This value should always be checked and amended if necessary.

> **i**
>
> **Enter shape sizes**
> If you want to enter a shape for this item, you should open the Shape/step input dialog once you have entered the quantity. This way you will not have to enter the width and height twice. The system will calculate the size of the surrounding rectangle from the entries in the Shape/step input dialog and use them to complete the Width and Height fields.
> *⇨ "Items - Shapes/processing tab" on page C-461*

**Width**
The value can be adopted from the previous item and should always be checked and/or changed if necessary. Enter the width of the lite in mm (or inches).

**Height**
The value can be adopted from the previous item and should always be checked and/or changed if necessary. Enter the height of the lite in mm (or inches).

**Quantity**
Surface per piece. It is calculated from the width and the height, considering the settings for size rounding defined in the master data.
*⇨ Master Data, "Rounding" on page B-880*
*⇨ Master Data, "Use real shape size for price calculation" on page B-949*
This value cannot be changed. If you have agreed with the customer to calculate the item price based on the exact surface rather than the rounded surface, select menu Options > Items > Enter quantity for the current item. The field will be released for entering a new value.
You have to save the new value in order to enter further items.

> **i**
>
> **Enter item as a box**
> If you have entered an item as a box by means of the stock search [F3], all fields starting from column Qty. will be locked and the item is displayed as a BOM.
> *⇨ "Items - BOM" on page C-457*
> *⇨ "Stock Search" on page C-736*

**Spacer**
The size for the airspace (spacer) is transferred from the product definition. If you change this entry, the new spacer will be displayed in the product fields. This change will also be adopted for the BOM structure on the BOM tab. You will not be able to select an airspace if certain settings have been made in the order:
*⇨ "Spacer settings" on page C-432*

**Year, key**
Price year and price key assigned to the product via the rate.

> **i**
>
> **Hide price**
> You can hide the item price (via user rights) to prevent other users from seeing the item prices.
> *⇨ Master Data, "Employee Rights" on page B-1010*
> *⇨ Master Data, "Identification, Program selection" on page B-1011*

**Price/PU**
If a price per unit has been assigned to the product, it will be shown at this point.

> **i**
>
> **Enter unit price**
> The unit price entered in this line only refers to the main product. Spacers and other components will be charged additionally. Define a unit price for the entered product as a whole in the unit price field. Define a fixed price for the entire item via the context menu.
> *⇨ "Item context menu" on page C-455*

**Unit**
Unit the price refers to.

**Discount**
Discount that has been defined for the customer. You can change the displayed value. The prices will be updated in this case.
*⇨ Master Data, "Customer" on page B-802*

> **i**
>
> **Show price and discount terms**
> Use the View menu> Terms to view the current terms for this customer.
> *⇨ "Terms" on page C-592*

**Net**
This is the net unit price for the glass only. It will be updated if you change the price, key, price unit and/or discount. It does not include the prices for shapes, processing, etc.

> **i**
>
> **Switch off real-time pricing**
> The menu Options menu > Pricing only upon saving can be used to disable the update after a price change. This is useful for entering products with very complex bills of material which include BOM components that are all are price-relevant.

In addition to the aforementioned columns, the following columns can be displayed: Thickness, Customer item, Consignment, Description 1, 2, 3, СМ (contribution margin), Sense of pattern, Patterned side, Coated side, Note.

**CM**
Contribution margin for one piece of the item.

**Sense of pattern**
How the patterned glass is to be fitted into the IG unit.

**Patterned side, Coated side**
The sides (levels) are viewed from the outside to the inside.

**Note**
Warning for items that have already been ordered.

### Item context menu

Right-click to open the context menu.

- **Create group:**
  The selected items are compiled in a group. Printouts will show a subtotal for each group. The groups are marked by colors.

| Item | Product | Pcs. | Width | Height | Qty. | AIR | Price List | Price Key | Price/PU | Unit | Discount | Net |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 1004 | 5 | 600 | 800 | 0,49 qm | | Price List 97 | Processings | 97,240 | qm | 0,00 | 47,6 |
| 2 | 1006 | 5 | 600 | 800 | 0,48 qm | | Price List 97 | Processings | 0,000 | qm | 0,00 | 0,00 |
| 3 | 1008 | 5 | 600 | 800 | 0,48 qm | | Price List 97 | Processings | 302,100 | qm | 0,00 | 145,0 |
| 4 | 150000 | 5 | 600 | 800 | 0,49 qm | 12 mmA... | Price List 97 | TEST | 214,160 | qm | 0,00 | 104,9 |
| 5 | 150108 | 5 | 1200 | 1200 | 1,44 qm | 10 mmA... | Price List 97 | TEST | 0,000 | qm | 0,00 | 0,00 |

- **Cancel group:**
  The group will be canceled.
- **Insert item before, insert item after:**
  The selected item is copied and inserted before/after.
- **Delete item and move up:**
  The selected item is deleted. The numbering of the subsequent items is updated.
- **Re-sort items:**
  Re-sorts the order items. If the order is already transferred to production, after a query, there is an attempt to cancel the order in production. After that, the order has to be transferred to the production system again. This also applies if items are added or deleted.
- **Import from clipboard:**
  Inserts one or several items from the clipboard, e.g. from Microsoft Excel. See the following note.
  This functionality requires the licensed module 156 Excel Line Item Import.
- **Enter fixed price:**
  Opens the Enter fixed price dialog to define a fixed price for several selected items. The fixed price will be applied to the selected items proportionally.
  *⇨ "Fixed Price Setting" on page C-589*
- **Delete fixed price:**
  Resets the manually entered fixed price to its original value. This can be the standard price or the manually defined price. Manual price changes can be reset to the standard price by using the Functions menu > Delete item settings.

- **Global changes:**
  Opens the Global item changes dialog where you can change the picking for the current item.
  *⇨ "Global Changes" on page C-590*
- **Content on clipboard:**
  Copies the selected item to the clipboard in order to use it in another program.

> **i**
>
> **Import from clipboard**
> Via this import, the quantity, dimension, commission, customer item, and article number can be imported. The columns on the clipboard have to be TAB-separated and can contain a title. The various columns can be assigned to one of the possible properties of an item and saved as template for later imports.
> If a title is imported, then the program tries using the title to assign the correct property itself. For this, the titles must have the same name as the property in the item table.
> For the article number, the B2B references for the partner in question can be used in order to import the product structures stored there including BOM. If no article number is imported, then the current item of the item entry is used including BOM as template.

## Items - BOM

Documents > Order > Select order > Items > BOM tab

[Image Description: Screenshot of the 'Items - BOM' tab in the A+W Business Sales software. The top section shows a BOM product structure (e.g., 725/IG 5/14/Th6 A+W). The middle section has fields for Display, Variation, Printout, Sales price details, and Supplier information. The bottom section is a grid of all items in the order, showing columns like Item, Product, Pcs, Width, Height, Qty, Price list, etc.]

Use this tab to edit details for calculating the prices of BOM components.
The fields are enabled and/or updated as defined by you in the menus.
*⇨ "Item Entry Menus" on page C-436*

> **i**
>
> **Services**
> If you have added services, the corresponding fields will remain locked. You can only change the services by using the Service tab.

**Product**
The data of the selected BOM component is shown in this area. These fields are locked if you have selected the main product.

**(Number)**
Product number of the selected component. Select another product by using the search.

**(Name)**
The name is adopted from the product master data.

**(Description)**
The description is adopted from the product master data and shows the processing text.

**Display**
Here, you can define how the prices should be printed on the document. The standard setting is adopted from the master data. You also need to tick checkbox Print. Prices can only be printed if the checkbox Price-relevant is ticked in product definition and a price has been entered.
*⇨ Master Data, "Sales price, purchase price relevant" on page B-616*
- **Implicit:**
  The main item's net price includes all prices of the BOM components; this includes shape and exchange surcharges as well as processing.
- **Explicit:**
  The prices of the BOM components are listed separately.
- **Implicit, price per quantity unit:**
  The prices of the BOM components are converted to the main product's price unit. This total price is shown in the document but only if all BOM elements of the item have been allocated the same display type.

**Variation**
The fields are only enabled if variants have been defined for the selected product. You can select a variant from the combo box.

**Autom. cutting**
The details for automatic cutting are adopted from the master data. These can be changed.
- [ ] The lite is cut manually.
- [x] The lite is automatically cut on the cutting table.

**Printout**
The BOM can be printed on the order form if required. This setting cannot override the settings from product management and management of forms.
- [ ] The BOM component will not be printed on the form.
- [x] The BOM component will be printed.

> **i**
>
> **Prerequisite**
> The BOM component can only be printed on the order if the print code is set for the BOM components or for the product.
> *⇨ Master Data, "Print" on page B-616*
> In the company data you can define the maximum number of BOM components that can be printed.
> *⇨ Master Data, "BOM" on page B-980*
> *⇨ Master Data, "Form Management - Options 1" on page B-1051*

**Changed**
This option is selected if a BOM component has been exchanged, e. g. Float 4 mm by patterned glass.
- [ ] The component has been adopted without changes.
- [x] The component has been changed for this order.

### Sales prices

This section shows for the selected BOM component the prices of all additional details, e.g. spacers, processing steps, shapes, stock sizes.

**Price list**
The price year is transferred from the product price master data. It can be changed for the selected component in the current order.

**Key**
The price key assigned to the product price is displayed. If several keys have been assigned, the setting for the selected component can be changed in the current order.

**Surcharge type**
The surcharge type is adopted from the product master data. It can be changed for the selected component in the current order.
*⇨ Master Data, "Calculation by surcharge type" on page B-311*

**Price / PU**
Price and price unit are adopted from the product master data. They provide the basis for price calculation.

**Discount**
Discounts are only displayed if they have been defined in the customer data. You can change this entry. The price will be updated automatically.

**Price relevant SP, PP**
You can define whether the price of the selected component should be considered in the sales and/or purchase price calculation. The standard setting is adopted from the master data.
- [ ] The price will not be taken into account for sales and/or purchase price calculation.
- [x] The price will be taken into account for sales and/or purchase price calculation.

**Net**
Updated net price for the selected component.

**Net total**
If the BOM includes identical components, their total price is displayed, e.g. the total price for two holes drilled.

**Min. qty.**
Shows the minimum quantity which is charged even if the quantity per unit remains below this minimum.
*⇨ Tutorial, “Prices and Price Calculation" on page C-137*
*⇨ Master Data, "Use real shape size for price calculation" on page B-949*
*⇨ Master Data, "Check min. qty. mainly by price unit" on page B-952*

**Measurement round.**
Size rounding for calculating the surface.
*⇨ Master Data, "Size calculation" on page B-150*

**PGR discount, statistics**
Shows the product groups that the product is assigned to.

### Details

**Supplier**
You can choose a (different) supplier if the selected element is to be ordered.
*⇨ Master Data, "Supplier List" on page B-854*

**Pce/Q/Wi/Hi**
Quantity and dimensions of the component.

> **i**
>
> **Amended sizes will not be adopted for the item line**
> If you change the sizes for a BOM component, the new sizes will not be adopted for the input fields of the item.

**Procurement type**
The procurement type is automatically checked and changed if necessary if you change the sizes of a component.

**Price code**
If distinctive features have been defined for a selected BOM component in product definition for pricing, the corresponding icons will be shown in red. Click on the icons to disable the default settings.
- **M**: Minimum calculation
- **/**: Individual price
- **O**: Other surcharge
- **F**: Formula price
- **P**: Production BOM explosion
*⇨Tutorial, "Icons for item entry" on page C-62*

**Items**
The fields are described in connection with the Item tab.
*⇨ "Items" on page C-452*

## Items – Shapes/processing tab

Documents > Order > Select order > Items > Shapes/processing tab > Select shape

[Image Description: Screenshot of the 'Shapes/processing' tab. On the left is a BOM component list and a large diagram of a shape with dimensions (W, H, H1). On the right are input fields for 'Processing', 'Shape parameters', 'Restrictions', 'Surrounding rectangle', and 'Sales price' details.]

Use this tab to enter the following data for an order item:
- "Shapes" on page C-462
- "Items - Processing" on page C-464
- "Items - Stepping" on page C-482
- "Items - Curved glass" on page C-483
- "Items - Leaded designs" on page C-485
- "Items - Shape template" on page C-486

**BOM**
Processing steps can be carried out on individual components of the BOM. Details about shapes always refer to the main product.
The view shows a sketch of the shape. The key defines the fields in which the sizes are entered.

### Processing

**Buttons**
Use the buttons to select a product group, e. g. shapes, processing, curved glass or leaded glass. If different products have been assigned to the product group, you can select and adopt the requested product in the Select dialog.

**Product**
Product number and name according to the master data.

**Formula**
Select and display the formula for the processing text.
*⇨ "Items - Processing" on page C-464*

### Shapes

**(Symbols)**
Use these buttons to select a shape.
*⇨ "Items - Processing" on page C-464*
*⇨ "Items - Shape template" on page C-486*

**Product**
The product number of the shape is adopted from the master data.

**Shape**
The shape number is adopted from the master data.

**(Name)**
The shape name is adopted from the master data.

**Shape parameter**
**W, H** Only the fields necessary to produce the shape will be enabled for each shape. The view shows the names of the edges.

**Restrictions**
This section provides details on the restrictions. Example: H1>0 means that edge H1 must not be 0.

**S+N file**
If you frequently enter a certain shape with identical sizes, you can save it as an S+N file. In future orders, you can select this file using the [Directory] button and assign it to the order item without having to enter the details every time.
In the master data, rules can be defined with which it is specified which processing article should be transferred to the BOM during the comparison.
*⇨ Master Data, "ITOE Rules" on page B-657*

In the processing entry, the comparison can be started either with a DXF file import or with the [iTOE] button on the ribbon. If in A+W CAD Designer (Shapes) the changes to the glass unit were taken over in a file, this change can be imported with the file.
For a detailed description of the function, see the documentation for A+W CAD Designer (Shapes).

If you have selected shape 99, you can also load and assign an S+N template.
*⇨ "SN File and Template" on page C-167*
*⇨ "Items - Shape template" on page C-486*

> **i**
>
> **Save as macro**
> As an alternative to saving the shape in an S+N file, you can save the entire product structure of the item as a macro.
> *⇨Tutorial, "Save Macro" on page C-158*
> *⇨ "Save Macro" on page C-618*

### Surrounding rectangle

The surrounding rectangle is used for pricing by default. In the company data you can define that the actual surface be used for pricing instead.
*⇨ Master Data, "Use real shape size for price calculation" on page B-949*

**(Printing of sketches)**
You can define how the shape will be printed:
- **No printout:**
  The sketch will not be printed on the forms.
- **Shape (true to scale):**
  True-to-scale shape sketches will be printed.
- **Shape (sketch):**
  Standard sketches will be printed. They only show the outline of the shape.

**Rotation by**
Angle by which the shape should be rotated. The function has to be activated in the company data.
*⇨ Master Data, "Company Data > Documents" on page B-928*
As angle, 90, 180 or 270 degrees can be specified. When printing on the papers, the rotated shape is depicted.
**Exceptions:**
- Shapes with the shape numbers 0, 24, 98, 99, 60, 61, and 81 cannot be rotated.
- No grills can be entered in rotated shapes, shapes with grills cannot be rotated.
- Patterned glass: If a shape is rotated by 90 or 270 degrees, the following applies:
  - For the production (OrderXML or production manager) and EDI export, the shapes are transferred turned. The identifier for the structure is switched in the process (horizontal -> vertical, vertical -> horizontal).
  - The check of the maximum dimensions refers to the turned dimension.

### Sales prices

**Year / key**
Price year and key for the shape surcharge are adopted from the master data. They can be changed if required.

**Price / PU**
Price and price unit for the shape surcharge are adopted from the master data. They can be changed if required.

**Discount**
The discount for the shape surcharge is adopted from the master data. It can be changed if required.

**Net**
The net amount for the shape surcharge is displayed automatically.

## Items - Processing

Documents > Order > Select order > Items > Shapes/processing tab > Select processing

[Image Description: Screenshot of the 'Items - Processing' tab. On the left is a BOM list and a diagram of a rectangular lite. On the right are controls for 'Processing' (e.g., Seaming), 'Parameters' (e.g., Qty, All edges), and 'Sales price' details.]

You can enter one or more processing steps for each order item.
The areas BOM, Processing, Sales Prices and Sketch Printing are explained for the Shapes/Processings tab.
*⇨ "Items - Shapes/processing tab" on page C-461*
*⇨ Tutorial, "Enter Processing Step" on page C-115*

### Processing

Use the buttons to select a product group. If different products have been assigned to the product group, you can select and adopt the requested product in the Select dialog.
The fields are displayed in the **Parameter** section according to the selected product.

> **i**
>
> **Processing steps for shapes**
> It is possible to apply processings to the shape 99 and imported SN files.
> *⇨ "Items - Shape template" on page C-486*

**[Formula]**
The processing text parameters can be edited. Use this button to open the **Replace parameters** dialog.
*⇨ "Parameter Replacement" on page C-584*

### Parameters

The entries are transferred to the price calculation formula and to production. The fields displayed may differ, depending on the selected processing.

- Edgework, glue
- Drill holes
- Countersunk Drillings
- Stepped drilling
- Rounded corners
- Notched corners
- Diagonal corners
- Edge notches, arch-shaped notch
- Inside cut-outs, speech hole, handles
- Coating, frosting, screen printing, area enameling, sandblasting, coloring
- Edge stripping
- Bending
- Grooving
- Regrinding, edge protection
- Logo, stamp
- Macro corner, macro edge, parameterizable macro (edge)
- Enamel
- Alarm wire
- Leaded designs
- Curved glass
- Masking
- Edge Deletion
- Edge screen printing
- Macro inside, parameterizable macro (inside)
- Article

### Edgework, glue

**Quantity**
The field is locked.

**All edges, (edge) 1 - 8**
Select the edges that are to receive edgework. The selected edges will be adopted for the description.
- [ ] Edge will not be processed.
- [x] Edge will be processed.

**Exact calculation**
This input is absolutely mandatory for shapes with more than four edges.
- [ ] Edgework will be calculated by default based on the surrounding rectangle dimensions. The fields **x Width** and **x Height** are available. If the shape has more than four edges, you can define how these edges should be calculated, e. g. 2 x width and 3 x height.
- [x] Edgework calculation is based on the exact sizes. The fields **Edgework processing size** are available.

Company data defines how edgework should be calculated in general.
*⇨ Master Data, "Calculate edgework with exact Im" on page B-934*
*⇨ Master Data, "Calculate min. edge length per edge" on page B-948*
*⇨ Master Data, "Commercial size rounding" on page B-948*

**x Width, x Height**
These fields are only available if exact calculation is disabled. The entries define the factor by which the width and height of the surrounding rectangle will be multiplied.
**Examples:**
- Input 2 x width and 2 x height produces the edge length of the surrounding rectangle.
- Input 2 x width and 3 x height is the edge length of a pentagon.

**Edgework size**
These fields are only available if exact calculation is enabled. These entries define how edgework should be calculated.

**Angle**
This field is used for beveling and miters. This value defines the beveling angle.

**Depth**
This field is displayed for beveling polishing. The entries define the polishing depth.

**(Bevel, miter) to outside**
This checkbox is displayed for beveling and miters.
- [ ] The polished bevel/miter will not be applied on the outside.
- [x] The polished bevel/miter will be applied on the outside.

### Drill holes

**Quantity**
Number of drilled holes. This field is filled if the drilling coordinates are entered in the **Parameters** section. If you enter the quantity, the fields for the drilling coordinates will be locked. The program assumes that only the price should be calculated, e. g. for a quotation.

**Diameter**
Diameter for all drilled holes in mm.

**Dimension type**
With the dimension type you define how the entered values will be interpreted. A graphic is displayed underneath each field which shows how the values must be entered.
- **Absolute coordinates:** With this setting you select the corner from which measuring will be started.
- **Distance from 2 edges:** With this setting you select the two edges from which measuring will be started.
- **Corner, edge, distance to edge:** With this setting you select the corner and edge from which measuring will be started.

[Image Description: Three icons representing different dimension types for drill holes: 'Absolute coordinates' from a corner, 'Distance from 2 edges', and 'Corner, edge, distance from edge'.]

**Drilled hole 1-4 [x/y]**
These entries define the drilled hole positions. The x and y values are interpreted according to the dimension type.

**Corner, edge**
The reference corner and edge can be selected for each drilled hole.

**Relief cut**
For drilled holes, counter-sinking and stepped drilling it is possible to make a relief cut, e. g. if the drilled hole is too close to the edge. The parameter can be transferred to production via the OrderXML interface.
- [ ] A relief cut is not carried out.
- [x] A relief cut is carried out.

### Countersunk Drillings

For these processing steps, the fields **Dimension type**, **Drilling 1 - 4 [x/y]** and **Relief cuts** are additionally shown. See also:
*⇨ "Drill holes" on page C-467*

**Quantity**
Number of drilled holes. This field is filled if the drilling coordinates are entered in the **Parameters** section. If you enter the quantity, the fields for the drilling coordinates will be locked. The program assumes that only the price should be calculated, e. g. for a quotation.

**(Type)**
Level of countersink. If you have selected Sink both sides, all fields will be enabled.

**Selection of entry**
Button to define the type of entry. This enables the corresponding fields:
- **D:** The diameter is retrieved. Fields D1, 2 are displayed.
- **T:** The sinking depth is retrieved. Fields T1, 2 are displayed.

The graphic display shows the interpretation of the respective values.

[Image Description: Two diagrams illustrating entry types for countersunk drilling. 'Diameter entries' shows diameters D1 and D2. 'Sinking depth entries' shows sinking depths T1 and T2.]

**D1, 2**
Sinking diameter in mm (inside, outside). These fields are only enabled if you have selected **Diameter**.

**T1, 2**
Sinking depth in mm (inside, outside). These fields are only enabled if you have selected **Depth**.

**D**
Drilled hole diameter in mm.

**<1, <2**
Degree of opening angle. By default, 60.00 is specified for the opening angle.
The fields D1, T1 and <1 are locked if you have selected Sink inside in the Type field. Fields D2, T2 and <2 are locked if you have selected Sink outside in the Type field.

### Stepped drilling

For these processing steps, the fields **Dimension type**, **Drilling [x/y]**, **Angle**, **To edge**, **Reference** and **Multi** are additionally shown. See also:
*⇨ "Drill holes" on page C-467*

**Quantity**
Number of drilled holes. This field is filled if the drilling coordinates are entered in the **Parameters** section. If you enter the quantity, the fields for the drilling coordinates will be locked. The program assumes that only the price should be calculated, e.g. for a quotation.

**Ø (Diameter)**
Diameter of the drilled hole per lite in the IG unit. The entries apply to all drilled holes.
The graphic display shows the interpretation of the values.

[Image Description: Two diagrams for stepped drilling. 'Diameter entries' shows a table with diameters for two glass lites. 'Graphic display' shows a cross-section of a stepped drill hole through two lites.]

### Rounded corners

**Quantity**
Number of rounded corners. The field is locked. It is filled if in the **All corners (corner) 1 - 8** area the number of rounded corners is selected.

**All corners, (corner) 1 - 8**
These checkboxes define the corners to be rounded.
- [ ] The round corner will not be cut.
- [x] The round corner will be cut.

**Radius**
The radius applies to all round corners. It is measured from the center of the lite.
If the round corners have different radiuses, you have to enter a separate processing step for every round corner.

### Notched corners

**Quantity**
Number of notched corners. The field is locked. It is filled if in the **All corners, (notched corner) 1 - 8** area the number of notched corners is selected.

**All corners, (notched corner) 1 - 8**
Select the corners that are to be made as notched corners.
- [ ] The notched corner will not be cut.
- [x] The notched corner will be cut.

**Distance A / B**
Distance A and B for all notched corners. By default, these distances are shown in a fixed connection A/B for the corners.
If you would like to enter different values for A and B, e.g. to produce oblong cut-outs, you have to define in the Cut-out edge A/B field how the cut-out should be measured.

**Cut-out edge A/B**
Vertical is set for A and B by default. This means that e.g. A defines both a vertical and a horizontal edge of a cut-out. You can define how the cut-out edges should be measured for this order here:
- **Vertical:** The edges of the cut-out will be measured vertically.
- **Parallel:** The edges of the cut-out will be measured parallel.
If you choose e.g. Vertical for A and Parallel for B, all cut-out edges A will be measured vertically and all cut-out edges B horizontally.
You can change the general parameters for corner cut-outs in the company data. This change will be applied to all orders!
*⇨ Master Data, "Enter rectangular cut-outs as width x height" on page B-938*

**Corner radius outside / inside**
The corner radius applies to the notch in mm.

### Diagonal corners

**Quantity**
Number of corner cut-offs. The field is locked. It is filled if in the **All corners, (diagonal corner) 1 - 8** the number of corner cut-offs is selected.

**All corners, (diagonal corner) 1 - 8**
Selection of the corners on which the corner cut-offs should be made.
- [ ] The slant will not be cut.
- [x] The slant will be cut.

**Distance A / B**
Distance A and B for all diagonal corners. By default, these distances are shown in a fixed connection A/B for the corners.
Please also refer to the description of notched corners.
*⇨ "Distance A / B" on page C-470*

### Edge notches, arch-shaped notch

**Distance / corner / edge, X / Y / corner**
Dimensions and reference corners or reference edges from which measuring will be started. The fields are hidden if checkbox **Multi** is ticked.

**Quantity**
Number of edge notches that are to be applied. This field is only enabled if the **Multi** checkbox is checked. The field is locked. It is filled if in the **All corners (edge) 1 - 8** area the number of notched corners is selected.

**All edges, (edge) 1 - 8**
Select the edges that are to receive edge notches. The fields are only enabled if the **Multi** checkbox is ticked. Enter in these fields the number of notches to be applied to the corresponding edge.
- [ ] No edge notch will be applied.
- [x] (At least) one edge notch will be applied.

**Dimension type**
With the dimension type you define how the entered values will be interpreted. A graphic is displayed underneath each field which shows how the values must be entered. The dimension type is only displayed for arch-shaped edge cutouts.
- **Absolute coordinates:** With this setting you select the corner from which measuring will be started.
- **Distance, corner, edge, distance to edge:** With this setting you select the corner and edge from which measuring will be started.

[Image Description: Two icons showing dimension types for edge notches: 'Absolute coordinates' from a corner, and 'Distance, corner, edge' from an edge.]

**Length (b), depth (a)**
Size of the edge cutout in mm. The field is only displayed for pointed edge cutouts.

**Chord (a)**
Size of the angled edge notch in mm. This field is only displayed for dimension type 2.

**Radius**
Size of the angled edge notch in mm. The radius is measured from the edge. The field is only displayed for arch-shaped edge cutouts.

**Corner radius outside/inside, corner radius outside**
The corner radius applies to the notch in mm.

**Multi**
Processing can be entered without parameters.
- [ ] All parameters are entered for the notch.
- [x] Only the number of processing steps and the parameters required for pricing are entered for the notch. This setting only makes sense for quotations.

### Inside cut-outs, speech hole, handles

**Quantity**
Number of cut-outs that are to be applied. This field is only enabled if the **Multi** checkbox is ticked.

**Dimension type**
With the dimension type you define how the entered values will be interpreted. A graphic is displayed underneath each field which shows how the values must be entered.
*⇨ "Dimension type" on page C-467*

**X / Y / corner / edge**
Dimensions and reference corners or reference edges of the pane from which measuring will be started. The fields for dimensioning are hidden if checkbox **Multi** is ticked.

**Width (a), height (b)**
Size of the cut-out in mm.

**Angle**
Cut-out angle (in degrees) in reference to the reference edge. The cut-out is rotated counter-clockwise.

**to edge**
Reference edge of the pane.

**Reference**
Select the cut-out corner in reference to the insertion point of the dimension type. Define with this entry which corner of the cut-out (or the center) the insertion point of the dimension type refers to.

**Examples**
- **Example 1:** Reference edge: 1, Reference point: (corner) 1, Angle of rotation: 0 °C
- **Example 2:** Reference edge: 3, Reference point: (corner) 3, Angle of rotation: 0 °C

[Image Description: Two diagrams showing examples of inside cut-outs. The first shows a rectangular cut-out positioned by coordinates X and Y from corner 1. The second shows a rotated rectangular cut-out positioned by coordinates X and Y from edge 3 and corner 3.]

**Key for Examples:**
- **A** Insertion point (depending on dimension type)
- **B** Reference point (corner of cut-out)
- **C** Reference edge (edge of the pane)
- **D** Numbering of reference points (corner 1 - 4)
- **E** Reference point (center = 9)

**Inside radius**
This field is only shown for inside cut-outs. The radius of the cut-out corners in mm.

**Processing side**
The field is only displayed for handles. By default, Level 1 is selected as processing side. The levels are counted from the outside to the inside.

**Multi**
Processing can be entered without parameters.
- [ ] All parameters are entered for the notch.
- [x] Only the number of processing steps and the parameters required for pricing are entered for the notch. This setting only makes sense for quotations.

### Coating, frosting, screen printing, area enameling, sandblasting, coloring

For these processings, the fields **Quantity**, **X / Y / Corner / Edge**, **Angle**, **To edge**, **Reference** and **Multi** are displayed. On this, see:
*⇨ "Inside cut-outs, speech hole, handles" on page C-472*

**Dimension type**
With the dimension type you define how the entered values will be interpreted. A graphic is displayed underneath each field which shows how the values must be entered.
- **Absolute coordinates:** With this setting you select the corner from which measuring will be started.
- **Distance from 2 edges:** With this setting you select the two edges from which measuring will be started.
- **Corner, edge, distance to edge:** With this setting you select the corner and edge from which measuring will be started.

[Image Description: Three icons representing different dimension types: 'Absolute coordinates', 'Distance from 2 edges', and 'Corner, edge, distance from edge'.]

**Width (a), height (b)**
Size of the surface to be processed. The dimensions of the lite are displayed by default.
- **Coating, matting, screen printing, area enameling, sandblasting, coloring:** If something other than the entire area should be processed, you can enter the dimensions freely.
- **Motif:** If you select a motif, you can change the dimensions as follows:
  - If in the **Number** you specify the screen number of a motif, the size of the motif is limited by the maximum dimensions in the master data. You cannot exceed the maximum width and height. If you specify dimensions within the dimensions of the screen, the motif will be cut.
  - If you insert a motif without screen number, you can specify the dimensions freely.
  - You can select the scaling mode of the motif in the Scaling combo box.
    *⇨ "(Scaling)" on page C-474*

**Variation**
Selection of the variants (colors) if variants have been defined for the selected processing.

**Number**
Number that is transferred to production. This specification is optional. If you specify the screen number, the motif file is displayed in the **Motif** field. The combo box for the scaling is locked.
*⇨ "Patterns" on page B-653*

**Saturation**
The saturation specifies how intensively the coating, matting, enameling, sandblasting or color of the screen or coloring is applied.

**Processing side**
By default, Level 1 is selected as processing side. The levels are counted from the outside to the inside.

The following fields only have to be filled if you would like to insert a motif.

**Motif**
Path and name of the motif file.
- If you enter a screen number in the **Number** field, a file path is displayed.
- If you do not enter a screen number, you can select a motif file with the [Folder] button.

**(Scaling)**
Scaling of the motif. You can only select a scaling if you insert the motif as file.
- **Freely scalable:** You can specify the height and width of the motif at will. The motif will not be scaled proportionally.
- **Proportional width:** You can specify the width of the motif. The height of the motif is adjusted proportionally to the width.
- **Proportional height:** You can specify the height of the motif. The width of the motif is adjusted proportionally to the height.
- **Not scaled:** This mode only makes sense with specification of a screen number. With specification of a screen number, this mode is pre-set. You can freely specify the height and width of the motif within the dimensions of the screen. The motif is cut.

> **i**
>
> **Cutting motifs**
> The following possibilities are available for cutting:
> - If you scale proportionally, the motif may under some circumstances be cut. Generally the motif is a cutout (center) from the entire motif.
> - If you insert the motif over the screen number, you can only scale the motif within the dimensions of the screen. If the specified dimensions in the fields Width (a) / Height (b) are smaller than the dimensions of the screen, the motif is cut. Generally the motif is a cutout (bottom left) from the entire motif.

**Mirroring**
You can mirror the motif.
- [ ] The motif is not mirrored.
- [x] The motif is mirrored horizontally.
A preview of the processing is displayed in the technical drawing in the bottom left corner of the dialog.

### Edge stripping

**Quantity**
The field is locked.

**All edges, (edge) 1 - 8**
Select the edges that are to receive edge stripping.
- [ ] Edges are not stripped.
- [x] Edges are stripped.

**Width**
Width of the edge stripping in mm.

**Level**
The levels are counted from the outside to the inside. This option defines the side to be processed.

### Bending

**Quantity**
Quantity of bending processes. By default, just one bending process is entered.

**Width**
Defines how far the lite will be bent (chord size).

**Height**
Defines the height up to which the edge will be bent compared with the level lite (sectional height).
To bend the edges differently, you have to create a separate processing step for every bend, and define the vertical and horizontal bend.
The edge stripping is displayed in the **Further details** tab.
*⇨ "Items - Further details" on page C-503*
