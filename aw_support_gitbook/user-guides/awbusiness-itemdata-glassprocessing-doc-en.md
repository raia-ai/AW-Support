---
description: "EN_AWBusiness_Sales_4_5-4"
---


# Item Data Software Reference

---
## Grooving

**Quantity**
The field is locked.

**All edges, (edge) 1 – 8**
Select the edges that are to receive grooves.
- No groove is ground on the edge.
- (At least) one groove is ground on the edge.

**Edge length**
The edge lengths of the lite are shown by default. Usually the length of the groove corresponds with the edge length.

**X / Y**
Distance to the edges. The sizes apply to all grooves.
To get an asymmetrical groove structure you have to create a separate processing step for each groove.

**Groove number**
The groove number defines the required type of groove.

**Width (b)**
Groove width.

**Side to be processed**
Specify the level on which processing will be carried out. Level 1 is selected by default. It is therefore imperative that you check this entry. The levels are counted from the outside to the inside.

## Regrinding, edge protection

**Quantity**
The field is locked.

**All edges, (edge) 1 – 8**
Selection of the edges to be reground or to be protected for transport.
- The edge is not processed.
- The edge is processed.

**Miter angle**
Angle in degrees for grinding. The field is only displayed for regrinding.

## Logo, stamp

For these processings, the fields Dimension type, Width (a) / Height (b), Angle, To edge and Reference are displayed. On this, see:
⇨ "Inside cut-outs, speech hole, handles" on page C-472

**Type**
Selection of the logo type.

**Number**
Number of the logo defined in the customer master data. It is transferred to production.

**Distance A/B**
Distance from the reference corner (A) and reference edge (B).

**Corner/edge**
Specifies the reference corner and reference edge.

**Level**
Level on which the logo will be applied. Level 1 is selected by default. It is therefore imperative that you check this entry. The levels are counted from the outside to the inside.

## Macro corner, macro edge, parameterizable macro (edge)

With this selection you can specify corner or edge notches that are saved as SN macro.

**Quantity**
Number of cut-outs that are to be applied. The field is only displayed if the Multi check box is marked, however it is locked. It is filled if in the area All corners/edges (corner/edge) 1 – 8 the number of corner or edge cut-outs is selected.

**All corners/edges, (corner/edge) 1 - 8**
Select the corners or edges that are to be processed. The fields are only enabled if the Multi checkbox is ticked. Specify in the fields how many processing steps are to be carried out.
- No processing is carried out.
- (At least) one processing step is carried out at the corner/edge.

**Distance**
This field is filled with the values from the macro if they have been entered in the product master data of the macro. This field is not shown for macro edge.

**Corner/edge**
Specify the corner and/or edge that is to be processed.

**Macro name**
File name of the selected SN macro.
- Use the directory icon to select a different file.
- Use the magnifier to open a dialog with the shape sketch.

**Multi**
Processing can be entered without parameters.
- All parameters are entered for the notch.
- Only the number of processing steps and the parameters required for pricing are entered for the notch. This setting only makes sense for quotations.

**(Parameter)**
The table shows the parameters for the selected macro. You can adjust the parameters in the table. The table is only displayed for parameterizable macro.

## Enamel

**Quantity**
The field is locked.

**All edges, (edge) 1 – 8**
Select the edges that are to be processed.
- The edge is not processed.
- The edge is processed.

**Depth (a)**
Depth of the enamel (strip). The depth is calculated from the cutback and the airspace width.

**Edge distance (x)**
Distance to the edges. The sizes are valid for all edges.

**Side to be processed**
Specify the level on which processing will be carried out. By default, Level 1 is selected as the side to be processed. The levels are counted from the outside to the inside.

## Alarm wire

**Wire exit corner**
The reference corner can be chosen freely. Input of additional dimensions is not required.

## Leaded designs
The leaded designs are described separately.
⇨ "Items - Leaded designs" on page C-485

## Curved glass
Curved glass is described separately.
⇨ "Items - Curved glass" on page C-483

## Masking

**Quantity**
The field is locked.

**All edges, (edge) 1 – 8**
Select the edges that are to receive edge coating.
- The edge coating is not executed.
- The edge coating is executed.

**Width**
Width of the edge coating in mm.

**Level**
The levels are counted from the outside to the inside. This option defines the side to be processed.

## Edge Deletion

**Quantity**
Number of cut-outs that are to be applied. This field is only enabled if the Multi checkbox is ticked.

**Dimension type**
With the dimension type you define how the entered values will be interpreted. A graphic is displayed underneath each field which shows how the values must be entered.
⇨ "Dimension type" on page C-467

**X / Y / corner / edge**
Dimensions and reference corners or reference edges of the pane from which measuring will be started. The fields for dimensioning are hidden if checkbox Multi is ticked.

**Width (a), height (b)**
Size of the cut-out in mm.

**Angle**
Cut-out angle (in degrees) in reference to the reference edge. The cut-out is rotated counter-clockwise.

**To edge**
Reference edge of the lite.

**Reference**
Select the cut-out corner in reference to the insertion point of the dimension type. With this specification, you define which edge of the cutout (or whether the center point) refers to the insertion point of the dimension type.

**Processing side**
Specify the level on which processing will be carried out. By default, Level 1 is selected as the side to be processed. The levels are counted from the outside to the inside.

**Multi**
Processing can be entered without parameters.
- All parameters are entered for the notch.
- Only the number of processing steps and the parameters required for pricing are entered for the notch. This setting only makes sense for quotations.

## Edge screen printing

**Quantity**
The field is locked.

**All edges, (edge) 1 – 8**
Selection of edges on which the edge screen printing should be executed.
- The edge screen printing is not executed.
- The edge coating is executed.

**Width**
Width of the edge screen printing in mm.

**Level**
The levels are counted from the outside to the inside. This option defines the side to be processed.

**Variant**
Selection of the variants (colors) if variants have been defined for the selected processing.

**Number**
Number that is transferred to production.

**Saturation**
The saturation specifies how intensively the edge screen printing should be applied.

## Macro inside, parameterizable macro (inside)

**Quantity**
Number of cut-outs that are to be applied. This field is only enabled if the Multi checkbox is ticked.

**Dimension type**
With the dimension type you define how the entered values will be interpreted. A graphic is displayed underneath each field which shows how the values must be entered.
⇨ "Dimension type" on page C-467

**X / Y / corner / edge**
Dimensions and reference corners or reference edges of the pane from which measuring will be started. The fields for dimensioning are hidden if checkbox Multi is ticked.

**Angle**
Cut-out angle (in degrees) in reference to the reference edge. The cut-out is rotated counter-clockwise.

**To edge**
Reference edge of the lite.

**Macro name**
File name of the selected SN macro.
- Use the directory icon to select a different file.
- Use the magnifier to open a dialog with the shape sketch.

**Multi**
Processing can be entered without parameters.
- All parameters are entered for the notch.
- Only the number of processing steps and the parameters required for pricing are entered for the notch. This setting only makes sense for quotations.

**(Parameters)**
The table shows the parameters for the selected macro. You can adjust the parameters in the table. The table is only displayed for parameterizable macro.

## Article

**Hardware parts**
The overview lists all hardware that is attached to the product. The following errors are displayed:
- **Area:** Affixing and/or type of hardware, e.g. handle, lock or hinge top, hinge middle, hinge bottom.
- **Prod No.:** Product number of the hardware.
- **Description:** Name of the hardware.
- **Variant:** Current variant (color) of the hardware.
- **Search:** Selection of the variant (color) if variants are stored for the selected hardware.
- **Special color:** Special color that is used for the hardware.

**Hinge side**
Side to which the hinge is affixed. You can choose from the options Left and Right. When changing the hinge side, the hardware is changed automatically if different items are stored in the master data for the hinge sides.

**Common variant**
Selection of the common variant (color) for all hardware in the overview. A common variant can only be selected if the same variant is stored for hardware in the overview. If a special color is selected as common variant, another text field is displayed next to the combo box in which the special color is specified.

## Items - Stepping
> Documents > Order > Select order > Items > Shapes/processing tab > Select stepping

Use this tab to enter the steps for IG unit. The areas BOM, Processing, and Sales Prices are explained for the Shapes/Processings tab.
⇨ "Items - Shapes/processing tab" on page C-461
⇨ Tutorial, "Enter Shape" on page C-110

### Processing
Use the buttons to select the processing Stepping.

### Parameters
The fields are shown for the selected item in accordance with the number of panes.
Specify in the checkboxes the panes to which the dimensions apply. Checkbox 1 defines the outside lite. If checkbox 2 is selected, positive entries are required in the fields, e.g. 15.

**S1 - Sn**
Size of the stepping for each lite in the unit.

## Items - Curved glass
> Documents > Order > Select order > Items > Shapes/processing tab > Select curved glass

Use this dialog to enter data for curved glass. The areas BOM, Processing, and Sales Prices are explained for the Shapes/Processings tab.
⇨ "Items - Shapes/processing tab" on page C-461

### Sketch printing, prices
The fields are described in detail in the description on the shapes.
⇨ "Items - Shapes/processing tab" on page C-461

### Processing
Use the buttons to select the processing Curved Glass.

### Parameters

**Chord size**
Length between the inside edges of the curved glass

**Segment height**
Height between edge and the apex of the curve

**Circumference**
Outside length of the curve between the edges

**Radius**
Radius of the curve

**Outside, neutral, inside**
Shows the calculated values if the sizes for the chord/segment height or circumference/radius have been entered.

**Shape**
The shape type if coating or patterns have to be considered.
- **Back:** The lite will be bent so that the curve points towards the back (inside) (of the room).
- **Outside:** The lite will be bent so that the curve points towards the outside.

**Degrees**
The degrees will be calculated automatically.

### Sketch printing, prices
These fields are described in detail in the description on the shapes.
⇨ "Items - Shapes/processing tab" on page C-461

## Items - Leaded designs
> Documents > Order > Select order > Items > Shapes/processing tab > Select Leaded design

Use this dialog to enter leaded designs for an item. After choosing the product and the pattern, the data will be transferred to the BOM.
The areas BOM, Processing, and Sales Prices are explained for the Shapes/Processings tab.
⇨ "Items - Shapes/processing tab" on page C-461

### Processing
Use the buttons to select the leaded design.

### Sketch printing, prices
These fields are described in detail in the description on the shapes.
⇨ "Items - Shapes/processing tab" on page C-461

## Items - Shape template
> Documents > Order > Select order > Items > Shapes/processing tab > Select S+N file

Use this tab to enter a shape by means of a template. These fields are only enabled if you have selected a template.
The areas BOM, Processing, and Sales Prices are explained for the Shapes/Processings tab.
⇨ "Items - Shapes/processing tab" on page C-461

Processings can also be entered for shape 99 and imported SN files. The processings are saved in the SN file.
The following requirements must be met for this:
- Company data – System tab: Edge processings and drillings on shape 99 checkbox has to be activated.
- A+W CAD Designer (Shapes) has to be installed.

On a free shape (shape 99), edge processings can be made only on all edges. The dimensions for drillings can only be specified with reference to the circumscribed rectangle.
For a standard shape from an SN file, edge processings can be entered on individual edges if the edges are numbered in the SN file.

### Shape parameters, Restrictions
For every template, the parameters and default values are shown. The entries can be changed. The new entries will not be saved with the template.
In the Restrictions section you can view the size restrictions for the selected shape. H stands for height and W for width.
⇨ Tutorial, "SN File and Template" on page C-167

**S+N file**
You can select the template by using the [Directory] button and assign it to the order item. In addition to S+N files, you can also load files in DFX and SHP format.
- You do not want to select a S+N file or save the details as a S+N file.
- You can select a template or save the current values in a S+N file. The buttons and input field will be enabled.
- You can select the required file either by means of the button or by entering the path and file name in the input field.

When you save the file, the system automatically creates a sub-directory with the present year and month as a name; the file is saved as a serial number.

**Surrounding rectangle**
The values are calculated automatically. They are used for pricing by default. In the company data you can define that the actual surface be used for pricing instead.
⇨ Master Data, "Use real shape size for price calculation" on page B-949

### Sketch printing, prices
These fields are described in detail in the description on the shapes.
⇨ "Items - Shapes/processing tab" on page C-461

## Items - Grills
> Documents > Order > Select order > Items > Grill tab

This tab offers additional tabs:
- "Grills - Standard" on page C-489
- "Grills - Prices" on page C-493
- "Grills - Omitted grills" on page C-495
- "Grills - Pattern" on page C-496

### Grills - Standard
> Documents > Order > Select order > Items > Grills tab > Standard tab

This tab is used to enter a grill pattern. The selected pattern is shown as a sketch when you select a grill from the sections horizontal, vertical grills.
⇨ Tutorial, "Enter Grills" on page C-105

**Selecting pattern**
Use the buttons to select the standard pattern for grills.

**Assembly position**
**Spacer** If you enter grills for multiple IG, you can define the gaps between the spacers. Use this button to transfer the settings to all spacers.

**Horizontal, Vertical grills**
The fields are enabled according to the selected grill pattern.

**Article**
Article number of the grills. The name is adopted from the product data.

**Continuous**
Specifies the continuous grill direction. If you do not mark any check box, all grills are fit together with miters.
- The grills in this direction will be cut.
- The grills in this direction are continuous.

**Variant**
Selection of a variant (color) for the grills.

**Width**
Grill width from the product data. You can change this value.

**Quantity**
The quantity is loaded from the selected pattern. You can add as many grills as you like. The sketch will be updated automatically.

**Thickness**
Grill thickness from the product data.

**Type**
Grill type from the product data.

**Drill sizes**
Drill sizes can be calculated automatically or entered manually. You must select an asymmetrical setting in the Calculation type field if you want to enter manual values.

> **Enter drill sizes last**
> If you enter the drill sizes manually, you should fill in all other fields first. Manual input will be changed by any other entry.

### Sales prices

**Year/key**
Price year and key from the product data. Both settings can be changed.

**Price / PU**
The grid price is calculated automatically. Changes in this field always refer to the total grid price. The total grid price is always shown as a unit price.

> **Change prices**
> You can view the grill prices underneath the graphics, in the Prices tab. There you can change the prices and price units for the horizontal and vertical bars. You can reset changed prices in the menu Functions > Delete settings.

Calculation of the grid price takes the settings for the minimum length into account.
⇨ Master Data, "Calculate min. grill length per pattern" on page B-947

**Discount**
Discount from the product data. It can be changed.

**Net**
The net price for the entire grill grid is automatically calculated based on the grid price and the discount. It cannot be changed.

### Construction / display

**Cutback**
The cutback will be taken into account for automatic calculation of the grill length. The entered value applies to all edges. It is adopted from the purchase price calculation. You can change it if required. Use this button to enter the cutback for each edge.
⇨ "Cutback" on page C-587
The values are transferred to the corresponding fields in Cutback in the Supplement tab.
⇨ "Items - Supplement" on page C-499

**Grill pads**
Grill pads can be fixed to the grill crosses if the grill thickness is considerably thinner than the spacer. Grill pads can be invoiced if required.
- No grill pads will be fitted.
- Grill pads will be fitted.
⇨ "Grillpads" on page C-427

**Printing sketches**
Define how the grill pattern will be printed:
- **No printout:** The grill sketch will not be printed on the forms.
- **Grill (true to scale):** True-to-scale grill sketches will be printed.
- **Grill (sketch):** Standard sketches will be printed. They only show the outline of the grills.
⇨ Tutorial, "Printing Sketches" on page C-192

**Calculation type**
Holes are drilled to fix the grills to the spacer bars. The sizes will be calculated automatically if you choose a symmetrical grill pattern. For asymmetrical patterns, the system will enable the fields in which you can enter the sizes.
The calculation type defines how the holes will be drilled. Please refer to the Master Data section for an example.
- **0 - Drilled hole-symmetrical:** Drilled holes will be calculated automatically. They will be arranged symmetrically in the spacer. If there are more than one grill per direction, the fields will have different sizes. The difference is plain to see if the grills are very wide.
- **1 - Field-symmetrical:** Drilled holes will be calculated automatically. The system will make sure that all fields are the same size. The distances of the drilled holes differ because they take the width of the grills into account.
- **2 - drilled hole-asymmetrical:** You can change the drill hole sizes manually. You have to choose this setting if certain requirements for the drilled holes have to be met.
- **3 - Field-asymmetrical:** You can change the drilled hole sizes manually. You have to choose this setting if certain requirements for the fields have to be met. You have to calculate the drilled hole positions yourself, based on the width of the bars.
- **4 - Identical length of bars:** The drilled hole positions are calculated so that all bars are of identical length.
- **5 - Drilled hole-sym. glass edge:** Drilled holes will be calculated automatically. They will be arranged symmetrically in the spacer. The glass edge is used as a reference value.
- **6 - Drilled hole-asym. glass edge:** You can change the drilled hole sizes manually. The glass edge is used as a reference value.

**Choose calculation type**
You can also choose the calculation type via the Calculation menu.
⇨ Master Data, "Calculation type for grill construction" on page B-163

**Dimensioning of drilling points**
Select an option to define how the entries for the drilling points will be calculated:
- **To reference point:** Every size is calculated starting from the reference point. The reference point is always the bottom left corner.
- **As a chain size:** The entries are calculated from one drilled hole to the next.

If you change the option, the sketch display will be amended accordingly. If you have already entered values for the drilled holes for an asymmetrical calculation type, these values will be amended as well.

### Grills - Prices
> Documents > Order > Select order > Items > Grills tab > Prices tab

This tab is used to edit the prices for the entire grill pattern.

**Grill article**
The prices for horizontal and vertical bars are shown separately underneath the sketch. The display refers to sales or purchase prices. This can be changed in the View menu.
- **Quantity:** Total length of fitted grills per direction.
- **Price, price unit:** The values are adopted from the price list selected in the Prices section.

The prices for the horizontal and vertical grills can be changed in Quantity as well as in the Price field.

**Grid**
Prices and price units are shown separately for the components of the pattern. The display refers to sales or purchase prices.
The calculation can be carried out per edge stopper, cross, field or T-grill. The total grid price is displayed in the Prices section.

**Grill article**
Define the display of the grill price elements by selecting an entry and setting in the Filter field:
- **All:** All components are listed.
- **Cut:** Cut grills are displayed.
- **Aluminum grill - vertical, horizontal:** Aluminum grills are displayed.

> **Reset price changes**
> If you do not want to adopt the changes, you can reset the standard prices using the Functions menu > Delete settings.

**Filter**
You can reduce the display of the grill price components as follows:
- **All:** All components are listed.
- **Quantity < > 0:** Displays the components that are found for a certain quantity.
- **Individual only:** Display of individual components.
- **Standard:** Standard mode of the previous version.

### Grills - Omitted grills
> Documents > Order > Select order > Items > Grills tab > Omitted grills

Use this tab to edit the grill pattern. Asymmetrical patterns and curved bars can be entered in the Pattern tab.

**Diagonal grills**
You can define the grill section which will be fitted diagonally. The checkboxes refer to the edge fields.
- This grill section will not be fitted.
- This grill section will be fitted.

> **Transferring diagonal grills to production**
> Documents including diagonal grills cannot be transferred to production directly. The concerned document and item numbers are shown in a notification.

**Horizontal, Vertical grills**
For every grill, you can define the bar sections to be omitted. All horizontal and vertical grills are marked by default.
- This grill section will not be fitted.
- This grill section will be fitted.

### Grills - Pattern
> Documents > Order > Select order > Items > Grills tab, Pattern tab

Use this tab to enter individual grill patterns.
The fields are described on the tabs Standard and Prices.

**Button [F12]**
Use this button to open the A+W CAD Designer application in order to design the grill pattern. The processing dialog offers specific online help functions.

## Items - Service
> Documents > Order > Select order > Items > Services tab

Use this tab to enter services that are to be added to the items. The services are saved in the items and listed in the BOM when the entries are saved.
⇨ Tutorial, "Enter a Surcharge for Special Services" on page C-127

### Item reference
This overview shows all order items, including quantities and prices. Service is only charged for items, the checkboxes of which have been ticked.
**[All], [None]** You can use these buttons to select all checkboxes or cancel the selection(s).

### Services
The list shows all services that have been entered. Tick the service to view the items for which a service will be charged. The checkboxes of the corresponding items are ticked in the Item reference section.
The following details are shown and can be edited:
- **Product, Selection, Name:** Selection, number and name of the selected service.
- **Service unit:** Reference value according to which the service will be charged. (Service unit = SU)
- **Service value:** Factor for the price calculation. For example, if you want to calculate the service costs for Disposal per piece for 3 order items of 12 lites each, the number of lites of these 3 items is displayed (36). The price/SU is multiplied by the service value. If the service is calculated in sqm, the service value represents the total surface of the corresponding order items.
- **Display:** The service can be displayed implicit, explicit and implicit in the price per QU. ⇨ Tutorial, "Price Printing" on page C-196
- **Printout:** Specify whether the service will be included in the printout.
- **Price list, Price key:** Price list year and price key from the master data. Can be changed if required.
- **Price / SU:** Price per service unit from the master data. Can be changed.
- **Discount:** Discount from the master data. Can be changed.
- **Net/pc:** The net price per unit is automatically calculated from the price/SU and the discount.
- **Item net:** The net price for the total item is calculated from the price/SU, the discount and the service value.
- **Min. quantity:** Minimum amount to be charged.

## Items - Supplement
> Documents > Order > Select order > Items > Supplement tab

Use this tab to enter and edit the data for mixed calculation and for complaints. The fields show the details of the selected item. All details apply to the main product.
The fields are enabled and/or updated as defined by you in the menus.
⇨ "Item Entry Menus" on page C-436

### Mixed calculation
This calculation type is only used in Austria.
Mixed calculation is used if the price are to be based on two or three IG price tables.

> **Master data: mixed calculation**
> The mixed calculation in this dialog is not related to the mixed calculation in the product master data.
> If the prices for your IG units are to be based on mixed calculation, you have to fill in the fields in the Supplement tab in item entry.

**IG 1, 2, 3**
Selection of the glass in the entered IG unit. The glass is not automatically displayed when you select an IG item. To calculate the total price, the corresponding prices are multiplied by the corresponding factor.

**Factor**
The factor defines how the price of the selected glass will be valued for mixed calculation. The factors are adopted from the company data. They can be changed in the order.
⇨ Master Data, "Mixed calculation factors" on page B-930

### Supplier/tax/surcharges

**Supplier**
You can enter a supplier if the selected product is to be ordered.
⇨ Master Data, "Supplier List" on page B-854

**KOMO no.**
Certificate number for Dutch building products. The defined value is transferred to production and is used for printing of labels and spacer text.

**Tax**
Selection of valid taxes. The setting applies to the item selected in the Items area.

**Surcharges**
Selection of valid surcharges. The setting applies to the item selected in the Items area.

### Product ID

**CE Code**
CE code from the product master data.

### CPIP data

**CPIP code**
Characteristic Performance Identification Paper (characteristics of features and of the performance). The CPIP code will be loaded from the product data.
