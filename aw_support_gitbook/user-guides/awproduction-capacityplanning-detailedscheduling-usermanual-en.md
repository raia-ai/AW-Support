---
description: "EN_UM_AWProduction_5"
---


# Lots

---
## Behavior in detailed scheduling

> **i**
> Except for **Use sub-element**, this setting is currently used only for processing, not for the elements themselves. Valid options:

*   **Standard**: Lots and racks will be created and allocated to this processing.
*   **Use child part**: There is no direct lot creation or rack allocation for this processing or element. Instead, the same batch number, rack numbers and sequences will be used as for the child element. Please note that this process is not valid for all elements. The element must not be cutting; there must be just one sub-element, and it must not belong to a rack optimization. Also, sub-element and element must belong to the same batch.
*   **Properties only**: In this case, there will be no lot creation or rack allocation for the processing. The processing and all its properties are available for rack allocation in connection with the organization. In this case, racks can be allocated after the first processing, after cutting.
    **Processing will be removed from the element tree**
    The processing will be removed from the element tree right after rack allocation. Grouping and sorting on the racks can no longer refer to this. This can be avoided by using a trick. The required processing property can be allocated to the lite by assigning an otherwise not required property.
*   **Not used**: This processing will not be added to the element tree, and is thus not available for rack allocation. Naturally, there is no lot creation or rack allocation in this case.

Please note that lots for related processing which are arranged below the original processing do not only use their own group key but also depend on the lot creation for the elements.

**Technical info:** database field: `FEINPLANUNG_KZ`

### More information on lot types

*   ⇨ Tutorial, "Lots" on page D-262
*   ⇨ Overview, "Buttons" on page A-90

# Processings Tab

**Master data > Detailed scheduling > Processings**

**(Fig. D-61 Lot types and processing, Processing tab)**

Use this dialog to define new processings, or change existing ones. The processing is specified by its name, its element or processing type, its supply type, and the allocated lot type. When detailed scheduling is started and the system finds no master data entry for a combination of processing type/procurement, this dialog will automatically be loaded so that you can enter the missing processing. Detailed scheduling can be recommenced immediately.

**Technical info:** database table: `FEIN_BEARBTYP`

## Description of fields

**Name**
This field shows the processing name. This name will be used only in the other tabs of this dialog, and does not reappear in detailed scheduling.
**Technical info:** database field: `NAME`

**Type**
Combo box Type shows all existing processing types. The processing types are loaded from master data.
**Technical info:** database field: `BEARBTYP`

**Procurement**
Select the appropriate procurement type for the processing from the combo box. Valid options:
*   0 = Production
*   1 = Cutting
*   2 = Stock withdrawal
*   9 = Ordered
**Technical info:** database field: `BESCHAFFUNGSART`

**Lot Type**
The combo box refers to the lot types defined on tab Lot type. Select the required lot type from the combo box. Please note that only processing steps of the procurement type Cutting must be allocated to lot type number 100.
**Technical info:** database field: `LOSTYP`

**Product number for missing processing**
Import will use this product number for processing whenever this is needed, and exists nowhere else in the system.
**Technical info:** database field: `ARTIKEL`

### More information on processing steps

*   ⇨ Overview, "Buttons" on page A-90

# Implicit Processing Tab

**Master data > Detailed scheduling > Processing > Implicit processing tab**

**(Fig. D-62 Lot types and processing, Implicit processing tab)**

Implicit processing tab can be used to automatically define further processing steps, to be added to the element tree. These implicit processings are specified by the attributes Name (only for display in this dialog), Type (processing type as per table BEARB_TYP), the allocated Lot type, and the code Creation.

## Description of fields

**Name**
This field shows the name of the implicit processing.
**Technical info:** database field: `NAME`

**Type**
The (processing) type must be defined so that the processing is not unnecessarily created should it be transferred from order entry to A+W Production so that the processing step would exist twice.
**Technical info:** database field: `BEARBTYP`

**Lot type**
Select the existing lot types from this combo box. The lot types are loaded from tab Lot types.
**Technical info:** database field: `LOSTYP`

**Definition**
This field defines under which circumstances the processing is created. Valid options:
*   Always
*   Header parts
*   Non-header parts

The processing step can be created always, only for main elements, or for elements other than main elements. The implicit processing Despatch for example could be created for all elements; this would make sense only for main elements of course so that you will need to select Header parts.
**Technical info:** database field: `ERZEUGUNG`

**The selected processing creates the following, implicit processing**
This table lists the existing implicit processing steps for the selected processing.

### More information on implicit processings

*   ⇨ Tutorial, "Lots" on page D-262
*   ⇨ Overview, "Buttons" on page A-90

# Detailed Scheduling of Batches

For batches shown in the batch view as *roughly scheduled*, detailed scheduling can be started by means of the context menu. Detailed scheduling runs in the background which means that you can go on working meanwhile. When detailed scheduling is terminated, a dialog appears *Detailed scheduling for batch...*.

## Detailed Scheduling for Batch...

The dialog is split into the following tabs:

*   "Glass Types Tab" on page D-407
*   "Rack Load Tab" on page D-410
*   "Results Tab" on page D-415
*   "Specials Tab" on page D-417
    *   "Nested Shapes Tab" on page D-417
    *   "Filler Orders Tab" on page D-419
    *   "Residue Plates Tab" on page D-421
    *   "Rejects Tab” on page D-422
    *   "Rush orders tab" on page D-424
    *   "Thickness Tab" on page D-425
*   "Free Optimization Tab" on page D-427
*   "Organization Tab" on page D-430
*   "Organization Options Tab" on page D-432
*   "Options Tab” on page D-434
*   "Stockplate Selection Tab" on page D-436

The individual tabs give a complete overview of all parameters used for detailed scheduling (cutting type, racks, stock sizes, etc.). The displayed parameters can be changed in the corresponding tabs. Detailed scheduling has to be run once more. This should be done carefully, however!

## Glass Types Tab

**View > Batch view > Select batch > Context menu detailed scheduling > Glass types tab**

**(Fig. D-63 Detailed scheduling for one batch, Glass types tab)**

The **Glass types tab** refers to the glass types in this batch. It provides information on the thickness, the optimization, the surface to be produced, and the quantity to be produced. Select an item from the top section to view information on the counterpane in the bottom section. This applies only to lites which have counterpanes in the same batch.

The symbols give a quick overview of the cutting type.
The symbols in the two sections have the following meanings:

**Top section:**
*   **Automatic cutting**
*   **Manual cutting**
*   **Manual cutting and cutting plan**

**Counterpane section:**
*   **Automatic cutting**
*   **Manual cutting**

**(Fig. D-64 Explanation of the detailed scheduling symbols for the individual batches)**

### Description of the fields in the top section

The fields in the top section provide information on:
*   **Glass type:** Shows the article number of the glass type. Glass types are defined in master data.
*   **Thickness:** This field shows the thickness of the glass type. The thickness is defined in master data.
*   **Optimization:** This field shows the optimization type. The optimizations are fixed in the system and cannot be changed.
*   **Surface (B):** This field shows the optimization surface in sqm.
*   **Qty (B):** This field shows the quantity. * after the quantity means that you can use filler orders for this optimization.

### Description of buttons

**Up**
This button allows to define the optimization priority, i.e. the sequence in which the optimization shall be run. Use this button to move the selected record one position up on the list.

**Down**
This button allows to define the optimization priority, i.e. the sequence in which the optimization shall be run. Use this button to move the selected record one position down on the list.

**Manual cutting**
Use this button to change the cutting type for the selected record from automatic to manual, or vice versa. This means that if the record is set to automatic cutting, it will be set to manual cutting; if it was set to manual cutting, it will be changed to automatic cutting.

**XOPT**
This button will appear if the selected lite is to be cut automatically. It will not appear if the tagged lite shall be cut manually. Use these buttons to force or delete an XOPT optimization for parts that are not stacked on harp racks.

**Cutting plan**
This button will appear if the selected lite is to be cut manually. It will not appear if the selected lite will be cut automatically. This means that an optimization will be started for this lite although it will be cut manually. A cutting plan will be created for this optimization.

### Description of the fields in section Counterpane Information

This section contains information on the counterpane of the lite selected in the upper section:
*   **Glass type:** Shows the article number of the glass type. Glass types are defined in master data.
*   **Thickness:** This field shows the thickness of the glass type. The thickness is defined in master data.
*   **Optimization:** This field shows the optimization type. The optimizations are fixed in the system and cannot be changed.
*   **Surface (B):** This field shows the optimization surface in sqm. The system will automatically calculate the surface.
*   **Qty (B):** This field shows the quantity to be optimized. The quantity will be imported from the order processing system.

### Description of buttons

**Double optimization**
Use this button to create a double optimization for the item selected in the counterpane section.

**Remove**
This button is valid only for items for which a double optimization was created. In this case, the button allows to remove the double optimization.

**Repeat**
This button is active only if you have changed the detailed scheduling results. Whenever you have made changes, you have to repeat detailed scheduling to apply these changes.

**Optimization**
If the detailed scheduling for this batch is acceptable, use this button to start the optimization. When the optimization is completed, tab Results will open automatically.

**PlanEdit**
After optimization you can use this button to view the cutting plan. Program Plan Editor is started.

## Rack Load Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Rack load tab**

**(Fig. D-65 Detailed scheduling for one batch, Rack load tab)**

This tab provides a detailed list of the racks required for this batch. This is the result of the rack settings you have made in tab Production sequence in the organization dialog.

The left section shows the individual racks in a tree structure. Click on the plus sign in front of a rack to open it so that you can see which rack numbers are used.

The meaning of the symbols:

| Icon | Description |
| --- | --- |
| Rack | Rack load |
| A | A Racks |
| Harp | Harp racks |
*Tab. D-8 Explanation of the systems in Rack load tab*

### Description of fields

**List on the left**
The list on the left side provides information on:
*   **Glass type:** This field shows all glass type/thickness combinations for this batch. Example: `1306/6.0` means that the glass type has the product number 1306, and a thickness of 6.0 mm. Glass types are defined in master data.
*   **Min. stack#:** This field shows the minimum number of stacks. You can edit this number by double-clicking on it. The dialog *Change minimum number of A racks* opens.
    > Should you have made any changes, you will need to repeat detailed scheduling!
*   **Stack#:** This field shows the actually required number of stacks.
*   **Harp rack#:** This field shows the actually required number of harp racks.

The display in the right section of the dialog is based on what has been selected in the left section. When you select the top entry (rack load), the right section shows all glass type/thickness combinations of this batch.

When you select the condition for the lites on an A rack on the left, the display looks as follows:

**(Fig. D-66 Detailed scheduling for one batch, tab Rack load, A rack)**

You will see the rack number, the stack number containing the lites, and the depth and width of the stack in mm.

#### Description of fields (A Rack View)

*   **Rack no.** Shows the rack number. The rack number area is loaded from master data.
*   **Stack#** This field is active only for A racks. This field shows the stack number containing the lites.
*   **Depth** Shows the depth of the stack (in mm).
*   **Width** Shows the width of the stack (in mm).

When you open in the left section the name of an A rack in the tree structure by clicking on the plus sign, you will see the rack number below. When you select the rack number, the display looks as follows:

**(Fig. D-67 Detailed scheduling for one batch, Rack load tab, A rack)**

You can see how many lites of a glass type/thickness combination are stacked on a rack, and how deep and wide the stack is.

#### Description of fields (A Rack - Detailed View)

*   **Glass type** This field shows all glass type/thickness combinations on this rack. Example: `1306/6.0` means that the glass type on this rack has the product number 1306, and a thickness of 6.0 mm. Glass types are defined in master data.
*   **Lites** How many lites of this glass type/thickness combination does this rack hold.
*   **Depth** How deep (in mm) have the lites of this glass type/thickness combination been stacked on this rack.
*   **Width** How wide (in mm) have the lites of this glass type/thickness combination been stacked on this rack.

When you select the name for the lites of a harp rack on the left, the display looks as follows:

**(Fig. D-68 Detailed scheduling for one batch, tab Rack load, Harp rack)**

You will see the rack number, the stack number containing the lites, and the depth and width of the stack in mm.

#### Description of fields (Harp Rack View)

*   **Rack no.** Shows the rack number. The rack number area is loaded from master data.
*   **Occupied slots** This field shows the number of occupied slots on this rack.
*   **Number of glass types** This field shows the number of different glass types on the harp rack.

When you open in the left section the name of a harp rack in the tree structure by clicking on the plus sign, you will see the rack number below. When you select the rack number, the display looks as follows:

**(Fig. D-69 Detailed scheduling for one batch, Rack load tab, Harp rack)**

You can see how many lites of a glass type/thickness combination are stacked on a rack.

#### Description of fields (Harp Rack - Detailed View)

*   **List on the left**: The list on the left side shows the racks used for this batch, and the valid conditions.
*   **List on the right**: The list on the right provides information on:
    *   **Glass type:** This field shows all glass type/thickness combinations on this rack. Example: `1306/6.0` means that the glass type on this rack has the product number 1306, and a thickness of 6.0 mm. Glass types are defined in master data.
    *   **Thickness:** This field shows the lite thickness. The thickness is defined in master data.
    *   **Lites:** You can see how many lites of a glass type/thickness combination have been loaded onto the rack.

## Results Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Results tab**

**(Fig. D-70 Detailed scheduling for one batch, Results tab)**

This tab shows the processes involved in producing this batch (spacers, IG line, etc.) and which quantities will be produced on the individual machines (bender, IG line, etc.). The bottom section shows the glass types, thicknesses, surfaces, and quantities. The fields stockplates, waste, and residue plate will be filled after optimization. These fields will be empty until an optimization has been run.

### Description of fields

**List on the right**
The list on the right provides the following information:
*   **Machines:** Shows the machine that shall perform the process selected in the left section.
*   **Value:** This column is available - and filled - only if the production lot type has been allocated to a grouping (e.g. spacer). In this case, this column shows the valid entry for each property/formula.
*   **Quantity:** Shows the quantity to be produced in the corresponding lot.

**Bottom list**
The list at the bottom provides the following information:
*   **Glass type.** This field shows all glass type/thickness combinations on this rack. Example: `1306/6.0` means that the glass type on this rack has the product number 1306, and a thickness of 6.0 mm. Glass types are defined in master data.
*   **Thickness:** This field shows the lite thickness. The thickness is defined in master data.
*   **Surface (B):** Shows the optimized surface in sqm.
*   **Quantity (B):** This field shows the number of lites to be optimized for this glass type. The following positive figures in the brackets (e.g. 10) show the number of fillers to be cut. (10) means that 10 fillers will have to be cut. Negative (e.g. -4) figures show the number of lites that were removed from this batch, and will have to be cut with a different thickness. (-4) means that four lites were removed from the batch, and have to be cut with a different thickness. Both values can be combined, of course: (10/-4).
*   **Stockplates:** This field shows the number of stockplates required for optimization. Stock sizes are defined in master data.
*   **Waste:** This field shows the waste for this optimization in %.
*   **Residue plate:** This field shows the length of the residue plate.

### Description of buttons

**PlanEdit**
This button will be active after an optimization has been run. Use this button to open the program PlanEditor. For more information on PlanEdit please refer to the documentation on the program PlanEditor.

**Save**
This button will be active after an optimization has been run. Use this button to adopt the detailed scheduling results. If you do not want to adopt the results, close the dialog by clicking on X in the top right corner. Answer the ensuing security check as required.

## Specials Tab

This tab provides information on existing special elements such as filler orders, residue plates, and breakage.

This tab consists of five sub-tabs:
*   Nested Shapes Tab
*   Filler Orders Tab
*   Residue Plates Tab
*   Rejects Tab
*   Rush orders tab
*   Thickness Tab

### Nested Shapes Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Special tab > Nested Shapes tab**

**(Fig. D-71 Detailed scheduling for one batch, Specials tab, Nested Shapes tab)**

Nested shapes tab refers to the joining of shapes. Shapes can be joined in an optimization item even if they belong to different lites. Prerequisite is that the shapes belong to the same pseudo series. Double-click on the Shape icon to edit this option (join yes/no) on this tab.

> **i Define the standard behavior**
> Whether or not shapes shall be nested by default can be set in A+W Production master data as follows: **Master data > Parameters> Module Detailed Scheduling > Special > Nested shapes**.

This function is based on the A+W standard shape catalog. Certain shapes can be nested (e.g. two triangles are joined in a rectangle). This works only for a few shapes - not for all.

In addition to this simple type of nesting shapes, A+W offers an extended module - **A+W Shape Optimizer**. This module allows the nesting of two shapes of the same shape within a surrounding rectangle which helps to improve the optimization results considerably.

The symbols in front of the shape number are:

| Icon | Description |
| --- | --- |
| ⬚ | Shapes will not be joined, but can be. |
| ☑ | Shapes will be joined. |
*Tab. D-9 Explanation of the systems in tab Join*

**Fields**
*   **Shape**: This field shows the shape number. The shape number is imported from the ERP system.
*   **WxH**: This field shows the sizes of the surrounding rectangle.
*   **Qty**: Shows how many of these shapes are included in the detailed scheduling for this batch.
*   **Order**: This field shows the number of the order which includes shapes. The shape number is imported from the ERP system.
*   **Item**: Shows the item number of the order which includes shapes.

### Filler Orders Tab

**View > Batch view > Select batch > Context menu Detailed Scheduling > Special tab > Filler Orders tab**

**(Fig. D-72 Detailed scheduling for one batch, Special tab, Filler orders tab)**

This tab shows the filler orders available for this glass type.

> **i Show filler orders**
> Tick the appropriate checkbox in the Organization dialog to use and display filler orders. If this checkbox is inactive, the table header shows the message *Filler orders will not be used!*

The symbols in front of the date are:

| Icon | Description |
| :---: | --- |
| 🟨 | The optimization defines whether the lite will be produced. |
| 🟩 | The lite will be produced with this batch in any case. |
| 🟥 | The lite will not be cut with this batch. |
| X | The order has already been scheduled in detail. It has not been completed yet, or detailed scheduling could not be completed successfully. |
*Tab. D-10 Explanation of the systems in tab Filler orders*

Select a record on the list and use the context menu to change the attributes.

#### Description of fields

*   **Date**: This field shows the production date calculated by the system.
*   **Qty**: Shows the quantity. The quantity in brackets is the order quantity. The quantity in front of the brackets is the quantity that can be produced in this batch.
*   **Order**: Shows the number of the order which includes filler orders.
*   **Item**: This field shows the item number of the order which includes filler orders. The shape number is imported from the ERP system.
*   **Modify individually/all**: Double-click on the table header to switch between *Modify individually* and *Modify all*. Depending on the mode (individual or all), the complete item will (or will not) be used as a filler. Accordingly, the symbol in front is changed either individually, or for all lites of an item.
*   **Priority**: This field shows the priority number. Valid entries are:
    *   **3**: lites will be scheduled together with the optimization to improve the overall yield. More stockplates can be used.
    *   **4**: lites will be scheduled with the optimization to improve the overall yield. No additional stockplates will be used.

### Residue Plates Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Special tab > Residue plates tab**

**(Fig. D-73 Detailed scheduling for one batch, Special tab, Residue plates tab)**

This tab shows the residue plates available for this glass type.

> **i Show residue plates**
> Tick the appropriate checkbox in the Organization dialog to use and display residue plates. If this checkbox is inactive, the table header contains the message *Residue plates will not be used!*

The symbols in front of the date are:

| Icon | Description |
| :---: | --- |
| 🟩 | The elements can always be used. |
| 🟥 | The elements cannot be used at present. |
*Tab. D-11 Explanation of the systems in tab Filler orders*

Select a record on the list and use the context menu to change the attributes.

#### Description of fields

*   **Date**: This field shows the production date.
*   **Qty**: Shows the quantity.
*   **Order**: This field shows the number of the order which includes filler orders. The order number is imported from the ERP system.
*   **Item**: Shows the item number of the order which includes filler orders.

### Rejects Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Special tab > Rejects tab**

**(Fig. D-74 Detailed scheduling for one batch, Special tab, Rejects tab)**

This tab shows the breakage available for this glass type.

> **i Show reject**
> Tick the appropriate checkbox in the Organization dialog to use and display rejects. If this checkbox is inactive, the table header contains the message *Rejects will not be used!*

The symbols in front of the date are:

| Icon | Description |
| :---: | --- |
| 🟩 | The parts can always be used. |
| 🟥 | The parts cannot be used at present. |
*Tab. D-12 Explanation of the systems in Rejects tab*

Select a record on the list and use the context menu to change the attributes.

#### Description of fields

*   **Date**: This field shows the production date calculated by the system.
*   **Qty**: Shows the quantity.
*   **Order**: This field shows the number of the order which includes filler orders. The order number is imported from the ERP system.
*   **Item**: Shows the item number of the order which includes filler orders.
*   **Last field**: This field shows the glass type and thickness, as well as the machines on which the broken lite can be produced.

### Rush orders tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Special tab > Rush orders tab**

**(Fig. D-75 Detailed scheduling for one batch, Special tab, Rush orders tab)**

This tab shows the rush orders available for this glass type. Rush orders can be displayed only if they have been entered in dialog Rush orders.

> **i Show rush orders**
> Tick the appropriate checkbox in the Organization dialog to use and display rush orders. If this checkbox is inactive, the table header contains the message *Rush orders will not be used!*

The symbols in front of the date are:

| Icon | Description |
| :---: | --- |
| 🟩 | The rush order will be produced with this batch in any case. |
| 🟥 | The rush order will not be cut with this batch. |
*Tab. D-13 Explanation of the systems in Rush order lites tab*

Select a record on the list and use the context menu to change the attributes.

#### Description of fields

*   **Date**: This field shows the production date calculated by the system.
*   **Qty**: Shows the quantity.
*   **Order**: Shows the number of the order which includes rush orders. -1 means that the rush order was entered manually, in dialog *Enter rush orders*.
*   **Item**: Shows the item number of the order which includes rush orders.
*   **Last field**: This field shows the glass type and thickness, as well as the machines on which the broken lite can be produced.

### Thickness Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Special tab > Glass thickness tab**

**(Fig. D-76 Detailed scheduling for one batch, Special tab, Glass thickness tab)**

You can use this dialog to change the optimization (cutting) thickness of lites to be fit into an IG unit. This will reduce the waste. You can define the lites to be cut with a thicker glass. This allocation defines the maximum change. Use tab Glass thickness to enter the lites that shall be actually cut with a different thickness. There are the following restrictions for the tab Glass thickness:

> **i Change thickness**
> **Glass thickness tab** is available only if the property (Formula editor) *Difference in thickness* has been allocated.
> There are the following restrictions for the Glass thickness tab:
> *   The thickness can be changed only for lites that are to be fit into an IG unit; this IG unit must not contain a sub-element with more than one direct sub-element.
> *   Cut element and IG must belong to the same batch.

The symbols in front of the order are:

| Icon | Description |
| :---: | --- |
| 🟩 | The lite will be cut from thicker glass. |
| 🟥 | The lite will not be cut from thicker glass. |
*Tab. D-14 Explanation of the systems in Thickness tab*

Select a record on the list and use the context menu to change the attributes.

#### Description of fields

*   **Order**: This field shows the number of the order which contains lites that can be cut from thicker glass
*   **Item**: Shows the item number of the order which includes the lites.
*   **Qty**: Shows the quantity.
*   **Unnamed field**: This field shows the current thickness and the cutting table on which the lite will be cut.
*   **New thickness**: Shows the new thickness of the lite to be cut.

## Free Optimization Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Free Optimization tab**

**(Fig. D-77 Detailed scheduling for one batch, Free optimization tab)**

This tab shows the optimization types used for the individual glass types. For glass types optimized in sequence, double-click on the item to change the optimization from sequenced optimization to free optimization. An [X] will appear in front of XOPTS. Only a sequenced optimization can be changed into a free optimization; this is impossible for manual cutting.

The bottom section of the dialog allows to change the optimization for individual racks, instead of glass types.

### Description of fields

*   **Glass type**: This field shows the article number of the glass type. The glass type is loaded from master data.
*   **Thickness**: This field shows the lite thickness. The thickness is loaded from master data.
*   **Optimization**: This field shows the optimization mode used for detailed scheduling.
*   **Surface (B)**: Shows the optimized surface in sqm.
*   **Quantity (B)**: This field shows the optimized number of lites for this glass type. * behind the quantity means that fillers are included.

### Bottom section

*   **Rack**: Shows the number of the rack containing the lites.
*   **Stack**: Shows the stack containing the lites.
*   **Qty**: This field shows the number of lites on the stack.
*   **Width**: Shows the width of the stack in mm.

## Partial Quantities Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Partial quantities tab**

**(Fig. D-78 Detailed scheduling for one batch, Partial quantities tab)**

This tab can be used to remove part of the lites from the optimization. In case of too much waste for instance, individual lites can be transferred to manual cutting, or optimized with one of the following batches. The dialog consists of two sections. The top section shows the glass types to be optimized with this batch. Tag a glass type to view information on the order in the bottom section.

> **i Partial quantities**
> Tab **Partial quantities** is available only if this has been activated in parameter settings.

### Description of the fields in the top section

*   **Glass type**: This field shows the glass type/thickness combinations. Example: `1306/6.0` means that this glass type's product number is 1306, and its thickness 6.0 mm. Glass types are defined in master data.
*   **Thickness**: This field shows the lite thickness. The thickness is defined in master data.
*   **Sqft. (B)**: Shows the optimized surface in sqm.
*   **Quantity (B)**: This field shows the number of lites optimized for this glass type. The following positive figures in the brackets (e.g. 10) show the number of fillers to be cut. (10) means that 10 fillers will have to be cut. Negative (e.g. -4) figures show the number of lites that were removed from this batch, and will have to be cut with a different thickness. (-4) means that four lites were removed from the batch, and have to be cut with a different thickness. Both values can be combined, of course: (10/-4).
*   **Stockplates**: This field shows the number of stockplates required for optimization. Stock sizes are defined in master data.
*   **Waste**: This field shows the waste of this optimization in %.
*   **Residue plate**: This field shows the length of the residue plate.

### Description of the fields in the bottom section

*   **Order**: Shows the number of the order which includes the glass type.
*   **Item**: Shows the item number of the order which includes the glass type.
*   **Rack**: Shows the rack number containing the item.
*   **Field without name**: Shows the lite dimensions.
*   **Quantity**: Shows the quantity.
*   **Partial quantity**: This field shows the partial quantities. If this is 0, no partial quantities were defined for this item. To enter a partial quantity, double-click on the order number in the bottom section of the dialog. The input dialog *Partial quantity* appears in which you can enter the required quantity.

## Organization Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Organization tab**

**(Fig. D-79 Detailed scheduling for one batch, Organization tab)**

This tab gives an overview of the organization settings for this batch used in detailed scheduling. You can use other settings. Settings should be changed only with the utmost care.

### Description of fields

*   **Processing sequence**: The combo box shows the selected processing sequence.
*   **Master organization**: The combo box shows the selected master organization.
*   **Organizations**: This section shows all defined organizations.
*   **Organization groups**: This section shows all defined organization groups.
*   **Sort groups**: The checkbox is related to field Organization groups and defines whether the selected group shall be sorted.
    *   ☑ The groups will be sorted.
    *   ☐ The groups will not be sorted.
    The two combo boxes below refer to the checkbox *Sort groups*. If this checkbox is ticked, select from the top combo box the required group and from the bottom combo box, the sorting (if applicable).
*   **Group formation**: This combo box shows the Group formation selected for this organization group.
*   **Sorting within groups**: The combo box shows the Sorting within the groups selected for the organization group.
*   **Racks**: Section Racks shows the racks that can be used for the batch in question. The entries are loaded from dialog *Rack settings*.
*   **disable**: Use this button to disable the rack selected in section Racks. It will not be available for detailed scheduling, and will be marked `***`. To activate the rack, use again the button `disable`.
*   **Rack mode**: The radio button defines the rack mode for detailed scheduling. The values are loaded from dialog *Rack settings*.
*   **Stacking mode groups**: This section shows the rack mode selected for groups. The values are loaded from dialog *Rack settings*.
*   **Sort groups**: The checkbox is related to field *Stacking Mode Groups* and defines how the selected group shall be sorted.
    *   ☑ The groups will be sorted.
    *   ☐ The groups will not be sorted.
    The two combo boxes below refer to the checkbox *Sort groups*. If this checkbox is ticked, select from the top combo box the required group and from the bottom combo box, the sorting (if applicable).
*   **Max. number of groups**: This field shows the maximum number of groups that can be put on a rack. The entries are loaded from dialog *Rack settings*.

### Description of buttons

**Save**
This button is active only if you have changed the settings in Organization tab. Use the Save button to adopt the changes. Only then will the changes be adopted.

**Repeat**
If changes have been made, detailed scheduling can be repeated so that the effects of the changes or the changed rack load become evident. After that, you can press the [Save] button.

## Organization Options Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Organization Options tab**

**(Fig. D-80 Detailed scheduling for one batch, Organization options tab)**

This tab shows the organization applied to this batch.

### Description of the fields in section Master Organization

**Stack XOPT together**
If certain lites are removed from detailed scheduling to be optimized by XOPT, this field defines how these lites shall be stacked. The entries are loaded from dialog *Master organization*.

### Fields in section Organization

*   **Left section**: The left section shows the organization used for this batch. The entries are loaded from dialog *Organization*.
*   **Stacking mode**: The radio button defines the stacking mode for detailed scheduling. The values are loaded from dialog *Rack settings*.
*   **Field Stacking mode** is related to the field on its right side. The picture in the right field is based on the property selected in field *Stacking mode*. It helps to visualize the selected property.
*   **Maximum load of A racks**: This field shows the percentage of the A rack surface that can be loaded.
*   **No group splitting if occupied by**: The value in this field defines the point from which on groups will not be split. The entries are loaded from dialog *Organization*.
*   **No item splitting if occupied by**: The entry in this field defines the point from which on items will not be split. The entries are loaded from dialog *Organization*.

### Description of buttons

**Save**
This button is active only if you have changed the settings in Organization options tab. Use the [Adopt] button to accept the changes. Only then will the changes be adopted.

**Repeat**
If changes have been made, detailed scheduling can be repeated so that the effects of the changes or the changed rack load become evident. After that, you can press the [Save] button.

## Options Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Options tab**

**(Fig. D-81 Detailed scheduling for one batch, Options tab)**

This tab contains only optimization options which serve to improve the optimization results.

### Description of fields

*   **Glass type**: This field shows the article number of the glass type. The glass type is loaded from master data.
*   **Thickness**: This field shows the lite thickness. The thickness is loaded from master data.
*   **Table allocation**: Shows the cutting tables valid for this glass type.
*   **Pair**: Shows the percentage of pairs in this optimization.
*   **Pair optimization**: Ticking this checkbox means that free optimizations will be automatically run as pair optimizations is possible.
*   **A+W Shape Optimizer**: If you are working with A+W Shape Optimizer, please enable this checkbox.
*   **Runtime factor**: The runtime factor defines the number of optimization runs to be computed by two different methods. Valid entries are 1 to 9. The runtime factor should always be set to 9. Nine optimization runs each will be calculated by two different methods; the best result will be selected automatically. If you enter 9, computing will of course take longer than for an entry of 2. The optimization result will very probably be much better, however.
*   **Cutting mode**: The radio button shows the cutting mode used for detailed scheduling. The entries are loaded from dialog *Master organization*. This field defines the cutting mode for the XOPT(S) optimizations. The radio button shows the cutting mode used for detailed scheduling. Selection of the appropriate cutting mode depends on the cutting table and the company's requirements. Generally, cutting mode 1 will produce the best yield while cutting mode 4 shows the worst results. Higher waste might be compensated by quicker breakout and stacking (due to the simpler cutting mode). The cutting mode determines the position of the lites on the subplate between two adjacent Y cuts. Possible values:
    1.  Between two Y cuts, lites of different width and height can lie next to another. Hence, W cuts may be made.
    2.  Between two Y cuts, only lites of different width and the same height can lie next to another.
    3.  Between two Y cuts, only lites of the same item can lie next to another.
    4.  Between two Y cuts, only up to two lites of the same item can lie next to another.
    5.  -7: Special mode for Coopmes tables. This mode is identical to the mode 2-4. For Z cuts: Z cuts up to the plate edge do not cut any lites.
*   **Trim**: The fields *left trim*, *right trim*, *top trim* and *bottom trim* show the trim entered for this glass product. The grey fields refer to the values taken from the glass product master data. The values in the white fields can be overridden. This is just a temporary change of trim for the batch on hand.
*   **Max. subplate**: This entry shows the maximum width of the subplate. The gray field refers to the values taken from the glass product master data. This entry can be changed in the white field. This is just a temporary change of trim for the lot on hand.
*   **Z costs**: This entry defines the costs per Z cut. The gray field refers to the values taken from the glass product master data. This entry can be changed in the white field. This is just a temporary change of the costs for the lot on hand.

## Stockplate Selection Tab

**View > Batch view > Select batch > Context menu Detailed scheduling > Stockplate selection tab**

**(Fig. D-82 Detailed scheduling for one batch, Stockplate Selection tab)**

This tab provides an overview of the stocksizes used in this batch.

### Description of fields

*   **Table allocation**: Shows the cutting tables valid for this glass type.
*   **Glass type**: This field shows the article number of the glass type. The glass type is loaded from master data.
*   **Thickness**: This field shows the lite thickness. The thickness is loaded from master data.
*   **Width x Height**: Shows the width and height of the stocksize in mm. This entry is loaded from master data.
*   **Quantity**: Shows the number of existing stocksizes. `9999` means an infinite number. Double-click on the field to change the number of stocksizes.
*   **Modify quantity**: Press this button to open the dialog *Number of stockplates*. In this dialog you can change the number of available stockplates.

### Description of the fields in section Residue Use

*   **Width**: If a residue plate was left over from a previous optimization that can be used for this batch, enter the width of this residue plate.
*   **Height**: If a residue plate was left over from a previous optimization that can be used for this batch, enter the height of this residue plate.

## Change minimum number of A racks

**View > Batch view > Select batch > Context menu Detailed scheduling > Rack load tab > select Rack Load from the left window > in the right window, double-click on the glass type for which the minimum number of A racks shall be changed.**

**(Fig. D-83 Change minimum number of A racks)**

This dialog allows to change the minimum number of A racks required for a batch.
Override the existing value, and leave the dialog by [Ok].

## Sequence of Tables

**Master data > Detailed scheduling > Tables**

**(Fig. D-84 Sequence of tables)**

Detailed scheduling allows to allocate a table, independent of the machine allocation. This requires that the tables are available in a defined checking sequence. This sequence can be defined for the tables in master data (only by means of a text field, without relation of the tables), or by means of this dialog.

This dialog will sort all existing tables by the field `XOPT_TISCH::RANG`. Use the buttons [Up] and [Down] to shift the tables and adapt the checking sequence. If you quit this dialog via button [OK], the above-mentioned field `Rank` will automatically be adapted in the database.

For the internal allocation of tables, all tables will be feasibility-checked for a certain lite, in the defined sequence. The first table found will be allocated to the lite.

Internal table allocation will only be used if explicitly set by the user, or if machinery allocation did not create a table allocation.

### Description of fields

*   **Display**: The view shows all defined cutting tables. Cutting tables are defined in master data.

### Description of buttons

*   **Up**: Use this button to change the checking sequence of the cutting tables. To change the checking sequence, select the cutting table to be moved one position up in the checking sequence. Now press the button [Up] until the cutting table has reached the required position.
*   **Down**: Use this button to change the checking sequence of the cutting tables. To change the checking sequence, select the cutting table to be moved one position down in the checking sequence. Now press the button [Down] until the cutting table has reached the required position.

# A+W Production Capacity Planning

## Revision overview of the module

| Date | Change |
| :--- | :--- |
| 01-2023 | Export work plan added. |
| 11-2017 | Complete revision. |
| 01-2017 | Product and company names adjusted. |
| 08-2013 | Initial creation of Tutorial and complete revision of Software Reference. |
| 04-2008 | Revision. |
| 11-2007 | Change of name (AWCapacity/Capacity Planning), change of chapter Work plan. |

This module provides information on the following subjects:
*   ⇨ Tutorial
*   ⇨ Software Reference

# Tutorial

This section provides information on the following subjects:
*   ⇨ Overview
*   ⇨ Basic Principles
*   ⇨ Planning and Scheduling
*   ⇨ Master Data of Capacity Planning

## Overview

The tutorial on the **Capacity planning** module deals with the planning of your production process and the optimum use of your machine capacity. The main goals of capacity planning are the adherence to delivery dates, using the machinery to the best effect, and being able to react flexibly to unforeseeable events. Optimal capacity planning is always a balancing act between the greatest possible efficiency and greatest possible flexibility.

This tutorial describes how you can intervene manually in the planning and how the master data for capacity planning is set up.

### Prerequisite knowledge

This tutorial is meant for persons in charge of production scheduling in **A+W Production** who are responsible for organizing the optimum production process. Participants must be familiar with the master data concept in A+W Production. Knowledge of rough and detailed scheduling are also useful.

> **i Protecting master data against access**
> The master data of AWP and especially of **A+W Capacity Planner** are highly sensitive data. Uncontrolled or unintentional interventions and changes can bring production to a complete standstill. Therefore, set up the workstations so that only the administrators or employees with appropriate functions have access to the master data.

> **i Data back-up**
> Create a full back-up of the master data before beginning any processing of the master data. The backup tool is located under: `C:\Programs (x86)\A+W\Techsoft\Tools\AWSplicer\AWSplicer.exe`.
> Shift the saved back-up out of your user directory into a directory to which support also has access. Discuss the upcoming changes in advance with your planner at A+W Software GmbH.

## Tutorial Structure

This tutorial consists of subjects with several training modules each. Each unit consists of the following elements:

*   **Overview**: Each training unit starts with an overview of the major topics.
    *   Objectives: What shall be conveyed?
    *   Benefit: What can this knowledge be used for?
    *   Maxims: Which correlations are to be remembered?
*   **Concepts**: Concepts and terms of the corresponding training session will be explained first. This is followed by examples and operating instructions.
*   **Exercises**: There are exercises featuring special tasks for some of the training units.

### Reading instructions

The contents of a training unit are based on the knowledge conveyed in the previous unit. We therefore recommend not to skip any unit.
If you are already familiar with a subject you should at least read the summary at the beginning of the unit in order to bring the main details to mind.

# Basic Principles

**A+W Capacity Planner** is designed so that even for products with unusually deep BOMs, usually several secure paths from the start technology to dispatch are found. The capacity planning accesses the work processes that the lites run through from cutting to delivery.

### Master data for machine allocation

The machine allocation (MA) establishes the connection between work processes and machines and maps the assessment according to preferred machines. So that the machines valid for the lites to be produced are found, the machines must be described precisely. In the machine allocation, there is a distinction between physical restrictions and logical machines with additional restrictions, cost rates and transition times.

Since the steps for setting up the capacity planning rely on the logical machines, the machine park must be described completely. The information for this is in the Machine Allocation section.

### Master data for capacity planning

For the date determination, shift plans, transition times, and times for the processing duration are required.

*   So that a simple picture for the utilization arises for testing the data, it is recommended that you specify the processing durations across the board in seconds per piece, e.g. 1 - 5 minutes per lite depending on the machine.
*   For the transition times, the optimal and realistic production throughput should be described. The specification of the times in whole shifts ensures a simple, predictable date determination. On machines that can also work unattended, the transition time (storage time) in hours can be specified, e.g. heat soak, autoclave, or hardening of silicon seals. In the exercises, ensure that you have the needed space in the operation in order to store the glass quantity of a shift.
*   The scheduling bottlenecks can be determined from the times for the processing duration.

### Scheduling rules

The scheduling rules are specified as configuration parameters for **A+W Capacity Planner**. They influence the program behavior, the message culture, and the possible user reactions. This affects, for example:

*   May delivery dates be shifted.
*   When is the earliest production start for a scheduled order.
*   How are quotations scheduled and do they have to be canceled again.
*   How are rush orders put through.
*   Starting with what quantity do items need to be split.

## Date optimization

The date optimization begins with the last machine on or before the delivery date: the loading. With a view to the Production Monitor, the date optimization can be depicted as follows.

**(Fig. E-1 Scheduling paths with and without conflicts)**

*   **A**: Vehicle fleet - loading
*   **B**: Calculation with optimal transition time
*   **C**: Calculation path 2
*   **D**: Transition time in shifts
*   **E**: Conflict
*   **F**: Production beginning cutting

Starting from the drive date, after deducting the customer handling time (in working days), the production end is specified. From the end of the last possible work shift (A), the scheduling searches backwards for the latest possible production beginning.

The transition times from one processing to the next are counted in shifts (D), whereby 0 is the immediately following processing in the same shift. Locked shifts, which are marked with an X, are counted too.

The calculation always checks all possible cost-effective paths. In case of date conflicts, transition times are kept and there is a buffer at the end of production. If in the process storage times that are too long result, the buffer times must be distributed manually. The solutions arising this way are much more expensive, however.

The Production Monitor is described in detail in a separate unit.
⇨ "Production Monitor" on page E-454

Scheduling is described in detail in a separate unit.
⇨ "Scheduling" on page E-448

## Scheduling

This section summarizes the technical background information for the scheduling.
Scheduling and interactive rescheduling uses the **A+W Capacity Planner** functions for allocating valid processing dates and machines to the bills of material.
Scheduling runs through five phases:

*   Analysis of the BOM.
*   Definition of machine paths.
*   Definition of feasible production dates.
*   Evaluation of feasible production dates.
*   Selection of the most favorable solution.

### BOM analysis

The BOM is broken down into element chains; those are the BOM sections whose first processing has no preceding processing or that unites several BOM parts. The individual element chains are calculated independently and in parallel. The individual results are matched to the final BOM at the conclusion of the calculation.

**(Fig. E-2 Formation of element chains from the BOM)**

While the BOM for the scheduling is being constructed, it is checked for plausibility at the same time. Here, errors in the BOM are detected and reported:
*   Abandoned BOM elements and processing steps will be detected and skipped. A warning is written in the log files.
*   Processing sequences are checked and adjusted. Defining processings receive the sequence 100; processings with smaller sequence are arranged according to the defining processing.
*   Any missing defining processings will be detected and reported.
*   Any missing logical machines will be detected and reported.
*   Inconsistencies between the processing data and machine allocation master data will be detected.

### Definition of machine paths

For the calculation of the machine paths, there are two features available in **A+W Capacity Planner**: best technology and automatic machine rescheduling.

If only best technology is used, there is precisely one machinery path. Alternative machines are not used.

**(Fig. E-3 Machinery path with best technology)**
*   **A** Processing
*   **B** Defined machines
*   **C** No machine change
*   **D** Informative processing
*   **E** No machine change
*   **F** Screen printing + subsequent screen printing

By forming processing chains on a machine, subsequent processings can be summarized insofar as the machine alternatives are the same. Subsequent processings (C, E) without machine change are done on the same date. To prevent this, e.g. with two screen printings one after another (F), a transition time must be defined so that the first printing can dry before the second is applied. Informative processings (D) are assigned to the preceding processing.

> **i Processing chains and automatic rescheduling**
> The settings for processing chains and automatic rescheduling are specified in the machine properties. The machines are described in the Machine Allocation (MA) part.

For automatic machine rescheduling, all machine alternatives are determined and connected to one another for each processing in the element chain. The number of machine paths can thus get so large that no solution is possible. Therefore, the number of alternative machines must be limited.

**(Fig. E-4 Automatic machine rescheduling)**
*   **A** Preferred machines
*   **B** Alternative machines
*   **C** Manual production

In this example, you see that the alternative machines are limited: all machines where manual work is done are not included in the determination of the machine paths.

For each processing in an element chain, the quantity of valid alternative machines is loaded and transition times are assigned.

*   For each processing, the machine specified by rescheduling determined by the MA or by earlier rescheduling applies. If automatic reallocation is active and processing has not yet begun, machines with the property *Automatic rescheduling* are also added to the list of possible alternatives.
*   Subsequent processings without machine change are done on the same date.
*   Machines that form processing chains can combine successive processings provided that their processing alternatives are identical.
*   Machines that are not assigned to any registration point process only informative processings, e.g. Shape corners. These processings are assigned to the preceding processing and planned with it. The first processing of an element chain may therefore not be an informative processing.

All machines found are associated with their preceding machines insofar as the transitions are permitted. Thus the set of all machine paths with start points and end points will be created for an element chain. All processing steps of the element chain must not be included more than once in every path of the set.

> **i Keep the number of alternative machines small**
> For each processing in the element chain, all machine alternatives are determined and connected to one another. The number of machine paths can thus get so large that no solution is possible. Therefore, limit the number of machine alternatives. Also form processing chains. This increases performance significantly.

### Definition of feasible production dates

Using the machine paths, the shift plans, and the transitions between the participating logical machines, the possible production dates for the individual processings steps are determined. For this, their (virtual) costs are calculated and the scheduling rights determined, which are required for the use of the transitions.
Random transitions are permitted below the last processing step in the BOM, below each joining processing steps, and below campaigns, rescheduling targets, and date locks.
This makes sure that valid production dates are available even if the scheduling variance has been extremely restricted.
The result is a set of all scheduled machine paths from which the following evaluation can determine the most favorable paths.

### Evaluation of feasible production dates

The set of all production dates found will be checked and evaluated. This results in solution sets for start and end dates of the machine paths and their (virtual) costs. This supports:

*   A production flow that is as fast as possible.
*   Priority use of the transition type *Normal*.
*   Scheduling for the preferred machine.
*   Buffer times at the end of production.
*   Use of the transition type *Rush* at the start of production.

If the production needs to be brought forward because of date conflicts, overload, locked shifts or for other reasons, this is done by moving the entire processing chain forward.
The result of this step is for every element chain a set of the most favorable solutions for every completion date of the next step.

### Finding the optimal solution

The individual solutions for the element chains are linked with the transition costs to the next steps to achieve the optimal result for the entire BOM.
For every start date of a laminated sheet or IG unit, the most favorable solutions for all sub-elements are combined and passed on to the next step for every completion date.

### Reporting to the ERP system

The calculated time and personnel costs and material consumption are reported in the order and the storage management of the ERP system. In connection with the ERP integration, the following data is transmitted:

*   Scheduling state.
*   Machine and personnel cost determination.
*   Calculation of earliest possible delivery date.
*   Query of the driving dates for route planning.
*   Query of the receipt of goods dates.
*   Fileless completion reporting via Webservices.
*   Online progress display from ERP via Webservices.

# Planning and Scheduling

In this section, you will find information about how the scheduled orders are displayed and edited in the Production Monitor. In addition, you can correct incorrect schedulings and reserve production times.

This section provides information on the following subjects:

*   "Production Monitor" on page E-454
*   "Scheduling and Rescheduling" on page E-467
*   "Campaign Planning" on page E-476
*   "Reservations" on page E-486
*   "Creating Processings" on page E-495

## Production Monitor

The Production Monitor is the central capacity and order control desk and entry point for work preparation, e.g. batch formation, rescheduling.
On the Production Monitor dialog, you check and edit production planning. Here, the capacity utilization of the machines is displayed per work shift.

**(Fig. E-5 Production Monitor)**

*   **A** Displayed machines
*   **B** Work shift per date
*   **C** Scheduling
*   **D** Work shift shortened
*   **E** Bottleneck
*   **F** Disabled
*   **G** Reserved for rush orders
*   **H** Undefined processings

In this example, you see that for most machines, there are 2 work shifts available. For some machines, 3 work shifts are displayed and can be booked. These work shifts are set up and generated via the master data for the capacity planning.
⇨ "Master Data of Capacity Planning" on page E-500

The orders are scheduled from the point of view of date optimization. Here, the rules of **A+W Capacity Planner**, the times of the work shifts, the locking of shifts, the defined bottlenecks, and the (virtual) costs are considered.

The details of how the scheduling is calculated is described in a separate unit.
⇨ "Date optimization" on page E-447

Generally, the orders from the ERP system are scheduled automatically. The work processes (processings) are scheduled accordingly on the machines' work shifts so that the delivery date promised in the order is adhered to. In special situations, you must intervene in this planning:

*   Shift orders to other machines or dates.
    *   ⇨ "Rescheduling" on page E-469
    *   ⇨ "Rescheduling Processings" on page E-471
*   Eliminate missing information from the orders.
    *   ⇨ "Incorrect Scheduling" on page E-473
    *   ⇨ "Post-Processing of Scheduled Orders" on page E-474
    *   ⇨ "Creation of Processings" on page E-497
*   Lock, reserve or set up additional work shifts.
    *   ⇨ "Campaign Planning" on page E-476
    *   ⇨ "Reservations" on page E-486
*   Eliminate missing information from the orders.
    *   ⇨ "Creating Processings" on page E-495
*   Adjust utilization on a daily basis
    *   ⇨ "Daily adjustments of the work shifts" on page E-456
*   Furthermore, you can set up the colored display of the work shifts as you wish.
    *   ⇨ "Setting up Production Monitor" on page E-463

### Detail view

**(Fig. E-6 Production Monitor - detailed view)**

In the detailed view, you can check the scheduling for individual days. In order to edit the schedulings, you must change back to the main view.

### Daily adjustments of the work shifts

The work shifts in the Production Monitor are generated from the capacity planning master data. They apply for the assigned machines on particular days of the week and in a defined period of time. Changes to the master data therefore apply regardless of the current planning.

You can control the planning day by day by adding individual work shifts for a machine, for example; by disabling machines to exclude them from the scheduling; equalizing the planning by defining machines or work shifts as bottlenecks.

In order to adjust individual work shifts to current needs for ongoing orders, you have the following possibilities:

*   "Here's how to create an additional work shift" on page E-457
*   "Here's how to lock a work shift completely" on page E-458
*   "Here's how to reserve a work shift" on page E-459
*   "Here's how to edit the working hours for a work shift" on page E-459
*   "Here's how to define a work shift as bottleneck" on page E-459
*   "Here's how to set up the work shifts for a machine" on page E-461
*   "Here's how to define a machine as bottleneck machine" on page E-462

#### Here's how to create an additional work shift

> **i No automatic rescheduling**
> If you set up an additional shift in the Production Monitor, already scheduled orders are not rescheduled automatically.

1.  Select **A+W Production > Production Monitor**.
2.  Open the context menu for the machine and the day on which you need an additional work shift.
3.  Select the **Enter new shift** menu.
    *   **A** Date of the work shift
    *   **B** Time of the work shift
4.  Select the start and end time (B).
5.  Select the date (A) of the start and end times.
    The end date of a night shift must be on the following day.
6.  Save the setting with [OK].

The new work shift is displayed in the Production Monitor.

#### Here's how to lock a work shift completely

1.  Select **A+W Production > Production Monitor**.
2.  Mark the work shift (A) that you want to lock.
3.  Select **Shift properties** from the context menu (B).
    *   **A** Status of the work shift
    *   **B** Selection of the status
4.  Set the status to **Disabled**.
5.  Save the setting with [OK].

The locked shift is marked in the Production Monitor with an X.

#### Here's how to reserve a work shift

1.  Open the Shift Properties dialog as shown in the previous action sequence.
2.  Set the status to **Active for rush orders**.
3.  Save the setting with [OK].

The reserved work shift is marked in the Production Monitor with a !.

#### Here's how to edit the working hours for a work shift

1.  Open the Shift Properties dialog as shown in the previous action sequence.
    *   **A** Capacity of the work shift
    *   **B** Specification of the duration
2.  Enter the duration of the time in hours and minutes.
3.  Save the setting with [OK].

Shortening of the work shift is indicated with cross-hatching in the Production Monitor.

#### Here's how to define a work shift as bottleneck

1.  Open the Shift Properties dialog as shown in the previous action sequence.
2.  Change the setting for the Bottleneck entry (A) to Yes (B).
3.  Save the setting with [OK].
    The setting applies only for the current work shift. It prevents the work shift from being booked beyond its capacity.

> **i Setting several work shifts to bottleneck**
> You can mark several work shifts by pressing `<Ctrl>` and marking the shift. When you're holding the `<Ctrl>` key down, you can also drag a rectangle across all shifts that should be marked. Then you can mark all highlighted shifts together as **Bottleneck**.

#### Here's how to set up the work shifts for a machine

1.  In the Production Monitor, open the context menu for the desired machine and select **Shift properties**.
    *   **A** Shift number
    *   **B** Duration of the work shift
    *   **C** Days of the week
2.  Mark the days of the week (C) on which the machine is available in the work shift.
3.  Enter the number (A) of the shift to which the changes refer.
4.  Enter the duration (B) in which the machine is available on the marked days of the week.
5.  Save the setting with [OK].
6.  If necessary, update the Production Monitor so that the changes to the machine shifts are displayed.

#### Here's how to define a machine as bottleneck machine

1.  In the Production Monitor, open the context menu for the desired machine and select **Properties**.
    *   **A** Bottleneck
    *   **B** Change setting
2.  Change the setting for the **Bottleneck** entry (A) to **Yes** (B).
    The setting only applies for the current machine and only until it is reset again manually. This way, the machine cannot be booked beyond its capacity.

> **i Defining bottleneck machines at the very start of the process**
> To equalize production, bottleneck machines must be defined as far toward the beginning of the production process as possible. This setting should be specified at the beginning of the start-up of the Production Monitor via the setting of the machines displayed.
> ⇨ "Here's how to display the machines in the Production Monitor" on page E-463

### Setting up Production Monitor

In order to adjust the display to your planning needs, you have the following possibilities:
*   "Here's how to display the machines in the Production Monitor" on page E-463
*   "Here's how to set the display of the colors" on page E-464
*   "Here's how to set the display type for all machines" on page E-465
*   "Here's how to set the display type for one machine" on page E-465

#### Here's how to display the machines in the Production Monitor

1.  Select **A+W Production > Production Monitor**.
2.  Click [Selected machines].
    *   **A** Displayed Machines
    *   **B** Machines are not displayed

    On this dialog, all machines from the MA are listed. The red font marks machines that are defined as bottleneck machines. These machines cannot be booked beyond their capacity.
3.  Check whether the settings as bottleneck machines are correct.
    Via the context menu for a machine, you can change the setting.
4.  Mark the machines that should be displayed in the Production Monitor.
5.  Save the setting with [OK].
    The dialog closes.
6.  If necessary, update the Production Monitor so that the changes to the machines are displayed.

#### Here's how to set the display of the colors

1.  Click [Settings].
    *   **A** Days before start date
    *   **B** Selection of the color
    *   **C** Specification of the color values (RGB)
    *   **D** Selection from combo box
2.  Specify the settings with which the work shifts and scheduling should be displayed in the Production Monitor, e.g.:
    *   Number of days (A) that are displayed before the start date.
    *   Color (B, C) in which the times are displayed, e.g. assigned times, reservations.
    *   Specification (D) whether particular information is displayed, e.g. the time, planned work processes.
3.  Save the settings with [OK].
    The dialog closes.
4.  If necessary, update the Production Monitor so that the changes to the machines are displayed.

#### Here's how to set the display type for all machines

1.  Click [Change display type for all machines].
2.  Select with which values the scheduling in the Production Monitor should be displayed.
3.  Save the setting with [OK].
    The dialog closes.
4.  If necessary, update the Production Monitor so that the changes to the machines are displayed.

#### Here's how to set the display type for one machine

1.  In the Production Monitor, open the context menu for the desired machine.
    *   **A** Logical machine
    *   **B** Display type of the machine
2.  Specify whether the assigned logical machines (A) should also be displayed for the machine.
3.  Select with which values (B) the scheduling of the machine in the Production Monitor should be displayed.
4.  Save the setting with [OK].
    The dialog closes.
5.  If necessary, update the Production Monitor so that the changes to the machines are displayed.

### Export Work Plan

**(Fig. E-7 Export work plan)**

If you have opened the work plan in the Production Monitor via the context menu, you can export the data to a CSV file. Select the requested entries and open the **Display** menu. There you select **Export**. The dialog *Save as ...* opens... Enter an appropriate name and click on [Save].

## Scheduling and Rescheduling

**Objectives**
*   What is scheduling and how are orders scheduled?
*   How can you react to problems which occur during scheduling?
*   What is rescheduling and how is it done?

**Benefit**
*   During scheduling, order and quotation data transferred by the ERP system are processed and calculated. Based on these data, dates are calculated and restrictions relevant for production are checked to make sure that your order is produced efficiently.
*   Rescheduling can be used to allocate processing steps to other dates and machines.

**Note**

*   **Scheduling**: Scheduling means the processing and calculation of data after an order or a quotation has been transferred by the ERP system. The orders or quotations are generally scheduled automatically. You can re-work a failed scheduling.
*   **Bottleneck machine**: A bottleneck machine cannot be booked beyond its capacity.
*   **Scheduling**: Scheduling start with the selection of processings.The target dates are binding. They are treated like processings with a single campaign date. Delivery dates are protected - exception: The processing Shipping can be shifted.
*   **Processing sequences**: Processing sequences in ascending order define the sequence of processing steps.
*   **Rescheduling mode**: Possibilities for rescheduling: Complete BOM, Only predecessor processing, Only successor processing, Individual processing. Rescheduling mode and direction are independent. Processings that do not participate are excepted from the scheduling.
*   **Rescheduling of orders**: Date rescheduling: Orders are shifted to other dates. Machine rescheduling: Orders are produced on other machines than originally planned.

### Scheduling of Orders

Generally, automatic scheduling of orders is set up in A+W Production. The data import runs as background process. You can trace the process of scheduling in the A+W ServiceMonitor. Manual interventions are only required if individual orders or order items could not be scheduled. The processing of these orders is described in a separate unit.
⇨ "Incorrect Scheduling" on page E-473

You can check and edit the scheduled orders that cannot be processed further on the Orders dialog. This topic is discussed in the Rough Scheduling section.
⇨ Rough Scheduling: Software Reference, "Orders in Rough Scheduling" on page C-153

If manual scheduling has been configured in A+W Production you will have to use the Scheduling dialog. When scheduling has been successful, field Status will show the actual time.

**(Fig. E-8 Scheduling)**

The scheduling is calculated in A+W Production until a solution is found that corresponds to the scheduling rules. If no acceptable solution was found, you must control the scheduling manually. For this, for example, large items can be split. The position split is described in detail in the Rough Planning section.
⇨ Rough Scheduling: Tutorial, "How to split an item" on page C-146

> **i Settings for the data transfer**
> Please check the settings for the data transfer from the ERP system to AWP with the A+W Software GmbH customer service team.

### Rescheduling

You can reschedule orders if they cannot be put through production as originally planned. Here, you can either select another machine or shift the processing to another date.

*   Scheduling begins with the selection of processings.
*   With the various rescheduling modes, you have the following possibilities for rescheduling: Complete BOM, only predecessor, only successor, individual processing.
*   The target dates are binding: The target dates are assigned and locked. They are handled like processings with a single campaign date.
*   Delivery dates are protected: This does not apply for the processing Shipping.
*   Rescheduling mode and direction are independent. Processings that do not participate are excepted from the scheduling. If due to the rescheduling an invalid processing sequence would arise, all successors are rescheduled if this achieves a valid result. An invalid rescheduling would be, for example, the rescheduling *Only predecessors* in the direction later than the successors.

#### Machine reallocation

With a machine reallocation, the production of an order is shifted to other machines. This can be necessary, for example, if a machine is not available due to repairs.

**(Fig. E-9 Machine reallocation)**
*   **A** Currently scheduled machines
*   **B** Available machines

#### Processing rescheduling

For the rescheduling of a production date, a processing is shifted to another date so that the order is completed earlier or later. This can be necessary, for example, if the priority of an order changes.

**(Fig. E-10 Rescheduling)**
*   **A** Processings
*   **B** Date and machine selection
*   **C** Rescheduling mode
*   **D** Specifications for the scheduling

You can reschedule a processing (A) for another date (B) or another machine. For this, you can specify how the transition times (D) should be considered. The dates recalculated by a rescheduling can then be locked. Thus, they are protected against further rescheduling.

The following modes are available for rescheduling (C):
*   **Reschedule complete BOM**: The complete parts list to which the processing belongs is rescheduled.
*   **Only marked processing**: Only the marked processing is rescheduled.
*   **Selected processing and all following processings**: The selected processing and all following processing steps for the lite will be rescheduled.
*   **Marked and all previous processings**: The marked and all previous processings of the lite are rescheduled.
*   **Unconditional allocation of dates for selected processing**: Scheduling of the selected processing will be forced on the selected date irrespective of the machine capacities.

With all these options, shipping and delivery date will be kept unless they are explicitly rescheduled. If you permit the shifting of the delivery date (D, you should also send the new delivery date back to the ERP system.

### Rescheduling Processings

This unit will teach you how you can shift the processings to another date.

#### Here's how to reschedule a processing

1.  Go to **Display > Orders > Context menu for selected orders > Processings > Context menu for selected processings > Work schedule > Rescheduling**.
    **(Fig. E-11 Reschedule date)**
    *   **A** Processings
    *   **B** Available machines for the selected processing
    *   **C** Reservation
    *   **D** Mode
    *   **E** Time pattern
2.  Choose the processings (A) to be rescheduled.
    If you select several processings, you can only shift the date.
3.  Select the setting for the scheduling (E):
    *   **Force rescheduling**: With this setting, the capacity limits of bottleneck machines are not considered. Therefore, it is possible to overbook the work shifts.
    *   **Allow Express Grid**: For rescheduling, the transition times of the type *Rush* are used.
    *   **Reschedule as High-Priority Order**: The processing is rescheduled with the minimum transition times. Caution: Here, the times for campaigns can also be used. Use this setting only in emergencies.
4.  Mark the shift in which the processing should be rescheduled.
5.  Choose the rescheduling mode (D).
    The button to start the rescheduling is enabled.
6.  Click [Reschedule] to start the rescheduling.
    The times are recalculated. The result is displayed on a dialog. If the rescheduling was not successful, you must change the conditions and try rescheduling again.

### Incorrect Scheduling

The scheduling of orders can fail for various reasons, e.g. in the following cases:
*   Undefined articles in orders.
*   Undefined production articles in orders.
*   Undefined processing steps in orders.
*   Invalid order data.
*   Shift restrictions cannot be met.
*   Shifts do not exist, e.g. because the shift plans have expired.

You can rework these orders and then repeat the scheduling.

**(Fig. E-12 Incorrect scheduling)**
*   **A** Defective Orders
*   **B** Selection criteria for the display

To filter the orders, you can select one of the possible error causes (B). The display of the corresponding orders (A) is updated automatically. You can select per order how the orders are handled. For this, you have the following options:

*   **Take over data again**: The order data is scheduled again and unchanged. For this, you must correct the master data, e.g. extend shift plans, and then schedule without renewed transfer of the data from the ERP system.
*   **Force scheduling**: The scheduling is forced. Here, the capacity of bottleneck machines is not considered. Therefore, the work shifts can be overbooked.
*   **Ignore scheduling**: The production dates are determined without consideration of transfer times, capacity limits, and campaign dates. All other orders and their delivery dates are pushed back.
*   **Delete invalid orders**: The corresponding orders are deleted. Speak to your colleagues in order entry so that the orders will be corrected and re-entered into A+W Production.
*   **Confirm determined delivery date**: The delivery date proposed by A+W Production is accepted. The new delivery date is reported back to the ERP system.

### Post-Processing of Scheduled Orders

This unit will teach you how you can manually re-work the orders that could not be scheduled.

#### Here's how to re-work a scheduling

1.  Go to **Master data > Post-processing of scheduling**.
    **(Fig. E-13 Post-processing of invalid scheduling)**
    *   **A** List of orders
    *   **B** Selection criteria
    *   **C** Display by
2.  Select the filter criterion (B) for the display of the orders and sorting (C). The list of orders is filtered.
3.  Select the order (A) to be edited.
4.  Click [Edit].
5.  Select the option with which you can eliminate the error. There is a description of the options in the Software Reference.
    *   ⇨ Software Reference, "Defective Orders" on page E-614
    *   ⇨ Software Reference, "Asynchronous Processing" on page E-615
    *   ⇨ Software Reference, "Changes to Scheduled Orders" on page E-616
6.  Click [OK] to adopt the changes. The order is treated according to the options selected.

### Campaign Planning

**Objectives**
*   What is a campaign?
*   How are campaigns defined, edited, and deleted?
*   What are Individual dates?
*   What are Weekly dates?

**Benefit**
*   Campaigns are processes that are executed only on certain days, in certain shifts, and on certain machines, e.g. blue screen printing every Friday in shift 2.

**Note**
*   **Campaigns**: Campaigns will help you process specific orders for customers or projects and plan them in due time. Campaigns are fixed, repeating dates for particular processes, which are largely untouchable. However, they can be overridden by "High-priority orders" or in the rescheduling editor with date assignments.
*   **Individual dates**: Individual dates are campaigns which are executed just once.
*   **Weekly dates**: Weekly dates are campaigns which are run on a regular basis.

> **i Prerequisite**
> Campaigns can be defined only if the appropriate work processes and shifts have been defined and if the corresponding shift plan is active.
> ⇨ "Shifts" on page E-501

#### Definition of the campaigns

Campaigns serve especially to set up a machine correctly, e.g. for coatings that require long set-up times. This means that the machine is used in different modes.

With campaigns, you can plan capacities for particular work processes, e.g. for screen printing in a different color for each day of the week. From this, e.g. campaigns *Blue on Monday* or *Green on Tuesday* are created. The advantage of reserving the screen printing capacities in this way is that the cleaning and set-up work can be minimized.

Campaigns can also be set up so that particular work processes are done in a particular shift, e.g. all the cutting of special glass types in the first shift.

The time reserved for a campaign can only be overridden by high-priority orders.

**(Fig. E-14 Campaigns)**
*   **A** Work process of the campaign
*   **B** Day of the campaign
*   **C** Available shifts
*   **D** Day of the planned campaign
*   **E** Activated campaign

A campaign always applies for a particular work process (A). It is either specified as individual date or as weekly date on a particular day of the week (B). If on the day there are several shifts available (C), the respective shifts must be specified.

Campaigns are used exclusively for work processes. The machine on which the processing is done plays no role here. For this, the work processes may not be bound to a particular machine.

**Example**
If two different screen printings are defined, during scheduling it must be detected which of the screen printings is the one in question. Here it plays no role on which machine the screen printing is done.
A work process Screen printing for campaign X must be set up in the MA so that it is only used for campaigns. This work process must be assigned to the logical machine to which the campaigns are allocated.

#### Campaigns in scheduling

For the scheduling for campaigns, all dates are hidden for which the work process does not apply.

**(Fig. E-15 Scheduling for campaigns)**
*   **A** Hidden work shifts
*   **B** Flexible transition time
*   **C** Second campaign of the BOM
*   **D** Flexible transition time
*   **E** Optimal solution

In this example, you see that the optimal solution (E) has a transition from one shift apiece. If the scheduling finds no result, it is checked whether there is a solution if campaign dates are ignored. If necessary, a corresponding message indicates that campaign dates are missing.

Work processes with campaigns automatically receive a flexible transition time at entry. If in the BOM there are several campaigns (C), then the system searches for earlier start dates (B, D) in order to avoid conflicts.

### Definition and Management of Campaigns

This unit will show you how to define, edit, or delete campaigns.

For instructions on this subject, please see:
*   "Here's how to define a campaign as an Individual date” on page E-480
*   "Here's how to define a campaign as a weekly date" on page E-482
*   "Here's how to edit a campaign" on page E-484
*   "Here's how to delete a campaign" on page E-485

> **i Prerequisite**
> Campaigns can be defined only if the appropriate work processes and shifts have been defined and if the corresponding shift plan is active.
> ⇨ "Here's how to draw up a shift plan" on page E-508

#### Here's how to define a campaign as an Individual date

> **i Prerequisite**
> On the Individual dates tab, only activated shift plans are displayed. If necessary, activate the shift plans that are required for the campaign.

1.  Go to **Master data > Capacity planning > Campaign planning**.
    *   **A** Work process
    *   **B** Date of the campaign
    *   **C** Duration of the campaign
2.  Mark the work process (A) for the campaign. The buttons are enabled.
3.  Click the arrow to the right. The work process is displayed in the Campaigns field.
4.  Check the checkbox of this work process in the Campaigns field. The **Individual dates** tab is active now.
5.  Mark the date for the campaign (B) on the calendar. The **Available shifts** field lists the shifts that are available for this date.
6.  Choose the shift in which the campaign shall be run.
    If the shifts are not displayed, you must check in the corresponding shift rule whether the days of the week are marked on which the shift is available.
    ⇨ "Here's how to define a shift rule" on page E-511
7.  Specify how many days or weeks (B) the campaign should last.
8.  Click [+].
    The new campaign is displayed in the Individual dates field. If the campaign should run through several shifts, repeat the steps 6 - 8 for each individual shift.
9.  Click [OK] to save the campaign. The campaign is saved, the dialog closed.

#### Here's how to define a campaign as a weekly date

> **i Prerequisite**
> On the Weekly dates tab, only activated shift plans are displayed. If necessary, activate the shift plans that are required for the campaign.

1.  Go to **Master data > Capacity planning > Campaign planning**.
    *   **A** Work process
    *   **B** Date of the campaign
    *   **C** Duration of the campaign
2.  Mark the work process for the campaign. The buttons are enabled.
3.  Click the arrow to the right. The work process is displayed in the Campaigns field.
4.  Check the checkbox of this work process in the Campaigns field. The **Weekly dates** tab is enabled.
5.  Change to the **Weekly dates** tab.
    *   **A** Campaign days
    *   **B** Shifts
6.  Mark the day of the week for the campaign (A) on the calendar. The **Available shifts** field lists the shifts that are available for this day of the week.
7.  Choose the shift in which the campaign shall be run.
8.  Click [+].
    The new campaign appears in the **Weekly dates** field. If the campaign should run through several shifts, repeat the steps 6 - 8 for each individual shift.
9.  Click [OK] to save the campaign. The campaign is saved, the dialog closed.

#### Here's how to edit a campaign

1.  Go to **Master data > Capacity planning > Campaign planning**.
2.  In the Campaigns field, mark the campaign that you want to change. The tabs Individual dates and Weekly dates show the dates for which campaigns have been defined.
3.  Mark the date that you want to change.
4.  Click [Delete]. The date is deleted.
5.  Select a new date or day of the week and the shift.
6.  Click [+]. The new date is displayed.
7.  Click [OK] to save the changes. The change is saved; the dialog closed.

#### Here's how to disable a campaign

1.  Go to **Master data > Capacity planning > Campaign planning**.
2.  In the Campaigns field, mark the campaign that you want to disable. The fields are locked.
3.  Click [OK] to save the changes. The change is saved, the dialog closed.
    The campaign is not included in the capacity planning. The campaign retains all of its properties. This way, you can switch campaigns on and off on short notice.

#### Here's how to delete a campaign

1.  Go to **Master data > Capacity planning > Campaign planning**.
2.  Mark the campaign that you want to delete.
3.  Click the arrow to the left. The campaign including all its dates is deleted.
4.  Click [OK] to save the changes. The change is saved, the dialog closed.

### Exercises on Campaigns

Create the data so that it is available in all subsequent exercises. If the data for the capacity planning is thus complete, you can test the planning for your own orders in the Production Monitor.

*   Decide which work processes on your shop floor should be organized in campaigns.
*   What is best for these work processes: A campaign as an individual date or a campaign as a weekly date?
*   Create the appropriate campaigns.
*   Edit the individual campaigns.
*   Delete dates from campaigns.
*   Delete campaigns.

**Additional information**
⇨ Software Reference, "Campaigns" on page E-620

### Reservations

**Objectives**
*   What are reservations?
*   How are reservations defined, edited, and deleted?

**Benefit**
*   Reservations can be used to keep capacities free for certain customers or projects.

**Note**
*   Reservations can be made only for bottleneck machines.
*   Reservations are made for customers and projects.

> **i Prerequisite**
> Reservations can be made only for machines defined as bottleneck machines.

> **i Reservations in shifts, days or weeks**
> Generally, capacities are reserved by the week. Depending on the setting under **Master Data > Configuration > A+W Production > Capacity Planning > Type of Reservation**, the reservation can also be specified for days or work shifts. If you change the setting, the old reservations are lost.

#### Reservation of capacities

For individual customers or projects, you can reserve capacities on a particular machine. Generally, you reserve the capacity across the entire week, so that you are not dependent on when the order arrives.

This way, capacities are held free so that the orders can be channeled through the bottlenecks without delay. Therefore, capacities can only be reserved for the work processes and machines for which bottlenecks can arise and which therefore are defined as bottleneck machines.
⇨ "Here's how to define a machine as bottleneck machine" on page E-462.

> **i Reservations for individual orders**
> Reservations for times for individual orders must be entered by the ERP system and transferred. The orders marked as *Reserved order* and released for production reserve appropriate times on all machines required for the production.

**(Abb. E-16 Reservations)**
*   **A** Machine for which the capacities are displayed
*   **B** Detailed information
*   **C** Information about the reservation

The capacities of the machines (A) are depicted graphically. Per day, all shifts are displayed that correspond to the selected period. For this, detailed information (B) is available.
The reservations are displayed in a list (C) if a day is marked.
The daily capacity of a machine is defined by the shifts entered for this machine.

When an order is transferred to A+W Production, the software checks whether there is a reservation for the customer or project in question.

*   If so, A+W Production will allocate the order to the reserved capacity provided there is enough free capacity left.
*   If no reservation has been made for the customer or project yet, or if there is nothing left of the reserved capacity, the order will be allocated to non-reserved capacities.

**Expired reservations**
If there are expired reservations, the dialog *Expired reservations* will open when you open the Reservations dialog. You can delete expired reservations or take over future reservations by changing the expiration date.

### Definition and Management of Reservations

This part of the tutorial will show you how to enter, edit, and delete reservations.

For instructions on this subject, please see:
*   "Here's how to delete an expired reservation" on page E-493
*   "How to enter a reservation" on page E-489
*   "Here's how to edit a reservation" on page E-491
*   "Here's how to delete a reservation" on page E-492

> **i Condition**
> Reservations can only be made for machines defined as bottleneck machines.

#### How to enter a reservation

1.  Go to **Master data > Capacity planning > Reservations**.
    If necessary, close the Expired Reservations dialog to open the Reservations dialog.
    ⇨ "Here's how to delete an expired reservation" on page E-493.
    *   **A** Machine
    *   **B** Start date
    *   **C** Number of days displayed
2.  Select the machine (A) on which you want to enter the reservation, e.g. *Grinding*.
3.  Select the start date (B) from which the reservation should apply.
4.  Specify the number of days (C) that should be displayed, e.g. 5.
    In the **Shift reservations** area, the shifts for the days are displayed on which the selected machine is available.
5.  Click [New].
    *   **A** Customer
    *   **B** Start date
    *   **C** Shift
    *   **D** Percentage reservation
6.  Select a customer (A) or a project.
7.  Select the start date (B) and the shift (C) for the reservation.
8.  Specify the reservation in % (D).
    You can also click in the field above to specify the reservation visually.
9.  Click [OK] to save the reservation.
    The dialog closes. The data appears on the **Reservations** dialog.
10. In the **Shift reservations** field, select the day with the reservation.
    The reservations for the shift are listed in the List of reservations.
11. Click [OK] to adopt the changes.
    The changes are saved and the dialog closed.

#### Here's how to edit a reservation

1.  Go to **Master data > Capacity planning > Reservations**.
2.  Choose the machine for which you want to edit a reservation, e.g. *Grinding*.
3.  Select the start date from which the reservations should apply.
4.  Specify the number of days that should be displayed, e.g. 5.
    In the **Shift reservations** area, the shifts for the selected days are displayed on which the selected machine is available.
5.  Select the field to be edited from the List of reservations.
6.  Change the percentage value of the reservation.
7.  Click [OK] to adopt the changes.
    The changes are saved and the dialog closed.

#### Here's how to delete a reservation

1.  Go to **Master data > Capacity planning > Reservations**.
2.  Choose the machine for which you want to edit a reservation, e.g. *Grinding*.
3.  Select the start date from which the reservations should apply.
4.  Specify the number of days that should be displayed, e.g. 5.
    In the **Shift reservations** area, the shifts for the selected days are displayed on which the selected machine is available.
5.  Select the line with the reservation that should be deleted.
6.  Click [Delete].
    The selected reservation is deleted from the list.
7.  Click [OK] to adopt the changes.
    The changes are saved and the dialog closed.

#### Here's how to delete an expired reservation

1.  Go to **Master data > Capacity planning > Reservations**.
2.  Select the reservations to be deleted from the list.
3.  Click [Delete].
    The reservations are deleted.
4.  Click [OK] to save the changes.
    The *Expired Reservations* dialog closes and the *Reservations* dialog opens.

### Exercises on Reservations

*   Enter a reservation for several days and shifts for a customer or a project.
*   Enter a test order for a customer or a project with a delivery date at the end of the two weeks.
*   Schedule the order.
*   Check the results.
*   Make a new reservation and enter a new order which exceeds the reserved capacities.
*   Schedule the order and check the results.
*   Edit the reservations.

**Additional information**
⇨ Software Reference, "Reservations" on page E-626

### Creating Processings

**Objectives**
*   What does creation of processings mean?
*   How are processing steps created and added to the BOM?

**Benefit**
*   The PPS system needs a more detailed BOM that includes all work steps in order to calculate the individual production dates and production costs. This is created by creating processings within the course of scheduling.

**Note**
*   **Processings**: Processing steps define the product's need to be processed, e.g. arrissing.
*   **Work processes**: Work processes define the way in which the need for processing shall be served, e.g. a special type of arrissing.

> **i Prerequisite**
> Processing steps can be created only by allocating processing articles to element types. The definition of processing types, processing articles, and element types is described in the Master Data section.
> Please agree any changes in the creation of processings with the A+W Software GmbH customer service because these are relevant for production.

#### Creation of Processings for Scheduling

The BOM of the ERP system includes the end product to be produced with its sub-elements and price-relevant processings, e.g. arrissing of the edges. Other production steps are only included implicitly in this BOM, e.g. cutting.

For the calculation of the individual production dates and costs, A+W Capacity Planner needs a more detailed BOM with all steps for which expenditures of time and costs are required. Therefore, in the course of scheduling, production-relevant steps are added to the production BOM. The creation of processings thus ensures that for each BOM element it is described how it arises in production.

**(Fig. E-17 Creation of processings)**
*   **A** Processings with the assigned processing articles
*   **B** Element types with assigned processings

So that the processings can be created for the elements of the BOM, these processings must be permitted on the corresponding element types. By assigning the processing (A) to an element type (B), the production BOM can be created so that all time and cost-relevant calculations can be made.

Therefore, for the capacity planning, processing must be defined at least for all stock removals, purchased and cut elements and for the assembly of LAMI and IG.

#### Creation of Processings

This unit will show you how to complete the BOM by processing steps which are relevant for production.

For instructions on this subject, please see:
*   "Here's how to add a processing" on page E-497
*   "Here's how to remove a processing step from the creation of processings" on page E-498

##### Here's how to add a processing

> **i Adding processings**
> When processings are added, changes will be applied as soon as they are made in the dialog. They cannot be undone.
> Please contact the A+W Software GmbH customer service if you want to change processings.

1.  Go to **Master data > Capacity planning > Creation of processings**.
2.  Go to field **Processings** and select the processing article you want to assign to an element type.
3.  Go to the **Element types** field and select the processing article you want to assign to the processing article.
4.  Click the arrow to the right.
    The processing article is assigned to this article type.
5.  Click [OK] to save the data.
    The assignment will be saved.

##### Here's how to remove a processing step from the creation of processings

> **i Add processings**
> When processings are added, changes will be applied as soon as they are made in the dialog. They cannot be undone.
> Please contact the A+W Software GmbH customer service if you want to change processings.

1.  Go to **Master data > Capacity planning > Creation of processings**.
2.  In field **Part types**, select the processing article to be removed.
3.  Click the arrow to the left.
    The assignment will be removed from the article type.
4.  Click [OK] to save the data.
    The change is saved.

# Master Data of Capacity Planning

In order to be able to work with **A+W Capacity Planner**, the master data for the capacity planning must be set up. This master data forms, together with the master data for the machine allocation (MA) and the master data for the article, the basis for the scheduling of orders and planning by **A+W Capacity Planner**.

Before you set up or edit the master data for capacity planning, the machines and work processes must be described completely. Information about this topic is in the Machine Allocation section.

> **i Protecting master data against access**
> The master data of AWP and especially of **A+W Capacity Planner** are highly sensitive data. Uncontrolled or unintentional interventions and changes can bring production to a complete standstill. Therefore, set up the workstations so that only the administrators or employees with appropriate functions have access to the master data.

This section provides information on the following subjects:
*   "Shifts" on page E-501
*   "Cost Calculation" on page E-520
*   "Transition Times" on page E-525
*   "Default Times" on page E-538
*   "Machinery Groups" on page E-563
*   "Load Distribution" on page E-569

> **i Data back-up**
> Before you begin editing the master data, create a complete data back-up of the master data. The back-up tool is under `C:\Programs (x86)\A+W\Techsoft\Tools\AWSplicer\AWSplicer.exe`. Move the saved back-up from your user directory into a directory to which support also has access. Discuss the upcoming change in advance with your planner at A+W Software GmbH.
