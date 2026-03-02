---
description: "EN_AWBusiness_Production_3-3"
---


# Software Reference

---
## Racks

- **Date of issue:** Date at which the rack was booked.
- **Days off site:** Number of days since date of issue.
- **Bars, wheels, carts:** Number of bars, wheels and carts belonging to the rack.
- **Blocked:** The rack is blocked for further bookings.
- **Lost:** The rack is not in the inventory; its whereabouts cannot be clarified.
- **Stationary:** The rack is only used stationary.

## Rack Management
*Production > Rack Management*

You can plan and control the packaging of produced orders on racks. The following dialogs are available in the **Rack management** menu:
- Rack types
- Racks
- Customer consignments

This chapter provides information on the following dialogs in this part of the program:
- "Rack Types" on page E-253
- "Racks" on page E-237
- "Rack Overview" on page E-255
- "Overview Partners" on page E-256
- "Reset Reminder Status" on page E-258
- "Reallocate Rack" on page E-257
- "Customer Reference" on page E-263

### Rack Types
*Production > Rack Management > Rack types*

*Fig. E-122 Rack types*

You can create different rack types in this dialog. The rack types are allocated to the racks. They serve to organize racks of the same design.

**Rack base type**
- **Designation:** Name of rack type.
- **Remark:** Comment to rack type, e.g. no usage off site.
- **Max. width/ max. height:** Largest admissible width and height of the lites to be accommodated on the rack.
- **Net weight / max. weight:** Net weight of the rack type and maximum loaded weight. The difference amounts to the admissible load.
- **Rack value:** The rack value can be e.g. the purchase price or the rental value.
- **Rack type:** Type of the rack, e.g. A rack or harp rack.

**Default when created anew**
- **Number of tension slats:** The specification of the tension slats serves to check completeness upon return.
- **Number of wheels:** The number of wheels serves to check completeness upon return.
- **Number of carts:** The number of carts serves to check completeness upon return.
- **Stationary:** Racks can be used to transport glass and as a storage place.
    - The rack can be used freely, e.g. also for off-site deliveries.
    - The rack has a fixed location. It cannot be used for deliveries.

**Table**
The overview shows all rack types matching the search criteria.
- **Description:** Name of rack type.
- **Remark:** Remark regarding special usage, size, etc.
- **Maximum width, maximum height:** Maximum admissible size of lites.
- **Net weight:** Weight without load.
- **Maximum weight:** Maximum loaded weight.
- **Value:** Purchase or rental value.
- **Bars, wheels, carts:** Number of tension slats, wheels and carts.
- **Stat.:** Specification whether the rack is used stationary.

### Rack Overview
*Production > Rack Management > Racks > Racks tab > Button at field number*

*Fig. E-123 Rack overview*

You can check the rack numbers in this dialog when you want to create a new rack.

**Racks**
- **Total:** Quantity of created rack numbers.
- **Available:** Quantity of available racks.

**Selection**
- **Number:** Rack number.
- **Type:** Rack type.
- **Customer number, name:** Customer number and name.
- **Output:** Date at which the rack was moved off site.

### Overview Partners
*Production > Rack Management > Racks > History tab > [Directory]*

*Fig. E-124 Racks - Overview partners*

In this dialog you can check which racks are or were with a certain market partner.

**Off-site**
The following sums are shown in these fields:
- **Racks:** Number of racks currently with this partner.
- **Bars:** Number of bars currently with this partner.
- **Wheels:** Number of wheels currently with this partner.
- **Carts:** Number of carts currently with this partner.

**Racks**
- **Rack no.:** Number of created rack.
- **Type:** Rack type.
- **Output:** Date at which the rack was moved off site.
- **Return:** Date at which the rack was booked in again.
- **Bars, wheels, carts:** Number of bars, wheels or carts belonging to the rack.

### Reallocate Rack
*Production > Rack Management > Racks > Functions menu > Reallocate rack*

*Fig. E-125 Reallocate rack*

In this dialog, you reallocate a rack from one partner to another.

**Off-site racks**
The list shows all racks which are currently off site.
- **Number:** Number of selected rack.
- **Type:** Rack type.
- **Customer:** Customer number.
- **Output:** Date at which the rack was moved off site.

**Rack**
- **Number:** Number of selected rack.
- **Type:** Type of selected rack.

**Reallocation**
- **From:** Number and name of partner to which the off-site rack is booked.
- **To:** You can enter the number of the new partner or select him by way of a search.

### Reset Reminder Status
*Production > Rack Management > Racks > Functions menu > Reset reminder status*

*Fig. E-126 Reset reminder status*

In this dialog you can reset the reminder status for individual racks.

### Rack Load
*Production > Rack Management > Racks > Racks tab > Functions menu > Execute group > Rack Load*

On this dialog, you can specify the assignment of order items to racks.

> **Prerequisite**
> You can only specify an assignment if you have created racks and the racks are available. You can create racks in the rack management on the Racks tab.

This dialog offers the following tabs:
- "Rack load - by order" on page E-259
- "Rack load - by rack" on page E-261

### Rack load – by order
*Production > Rack management > Racks > Functions menu > Execute group > Rack load > By order tab*

*Fig. E-127 Rack load - by order*

On this tab, you can assign the rack to individual items of an order. You can also specify what quantity of an item should be stored on the rack. You can assign several items to the same rack.

**Selection**
- **Order:** Number of the order.
- **Cust.:** Customer number and name. The fields are filled if you enter the order number.
- **[Clear assignments]:** Deletes all assignments of the order items to the racks from the overview. If you want to delete only one order item from the assignment, you must click on [Delete] on the Start menu.

**Overview**
In the overview, all items of the selected order are displayed with the assignments to the racks. You can create assignments for one rack or new assignments. Only the fields Rack, Search, and Lites on rack can be edited; the other fields are filled automatically.
- **Item:** Order item number.
- **Description:** Name of the glass.
- **Width, Height:** Dimensions of the item.
- **Item quantity:** Quantity of the item.
- **Weight per piece:** Weight of a piece of the item.
- **Not yet stored:** Quantity of items that is not yet assigned to a rack.
- **Rack:** Number of the rack to which the item should be assigned.
- **Max. height, Max width:** Largest permissible size of lites. The fields are filled automatically if a rack number is entered.
- **Maximum weight:** Maximum loaded weight. The field is filled automatically if a rack number is entered.
- **Search:** Opens the Rack overview dialog where you can select a rack. The size and weight of the rack selected are taken over into the table. The Lites on rack field is filled by default with the quantity from the Item quantity field.
- **Lites on rack:** Quantity of lites that should be assigned to the selected rack. If you assign the rack fewer lites than the total quantity of the item, a new line with the difference for the item is displayed automatically. You can assign this quantity to another rack.

- **Total:** Total quantity of the order items.
- **Rest:** Total quantity of the items that are not assigned to a rack.
- **On rack:** Total quantity of the items that are assigned to a rack.

### Rack load – by rack
*Production > Rack management > Racks > Functions menu > Execute group > Rack load > By rack tab*

*Fig. E-128 Rack load - by rack*

On this tab, you assign individual items of an order to a rack. You can also specify what quantity of an item should be stored on the rack.

**Selection**
- **Rack/rack type:** Number and type of the rack. You can only specify the number of the rack to which the items should be assigned. The Rack type field is filled.
- **Max. Width/Height/Weight:** Largest permissible size of the lites and greatest weight of the rack loaded. The fields are filled if you enter a rack number.

- **[Empty rack]:** Deletes all assignments of the order items to the marked rack from the overview. If you want to delete only one order item from the assignment, you must click [Delete] on the Start menu.

**Overview**
In the overview, all items are displayed that are assigned to the selected rack. You can edit the assignments or re-assign items. Only the fields Order, Pos, and Lites on rack can be edited; the other fields are filled automatically.
- **Order:** Order number.
- **Item:** Order item number.
- **Description:** Name of the glass.
- **Size:** Item size.
- **Customer:** Customer number.
- **Maximum storable:** Quantity of the item that is not yet assigned to a rack.
- **Weight:** Weight of the quantity of an item that is assigned to a rack.
- **Lites on rack:** Quantity of lites that should be assigned to the selected rack.

- **Total:** Total quantity of the order items.
- **(Weight) on rack:** Total weight of the items that are assigned to the rack.
- **On rack:** Total quantity of the items that are assigned to the rack.

### Customer Reference
*Production > Rack Management > Customer Reference*

Further details for shipping are specified with the customer reference. This dialog offers the following tabs:
- "Customer Reference – Reference" on page E-263
- "Customer Reference - Unload Address" on page E-264
- "Customer Reference – Allocation" on page E-265

#### Customer Reference - Reference
*Production > Rack Management > Customer Reference > Reference tab*

*Fig. E-129 Customer reference - reference*

Under this tab, you can specify the location consignment of the customer. This allows you to select the desired consignment in the order during the item entry.
⇨ Software Reference, "Consignment" on page C-454

#### Customer Reference - Unload Address
*Production > Rack Management > Reference > Unload Address tab*

*Fig. E-130 Customer reference - Unload address*

Under this tab, you can specify the unloading sites usually approached at the customer's site.

#### Customer Reference – Allocation
*Production > Rack Management > Customer Reference > Allocation tab*

*Fig. E-131 Customer Commissions - Allocation*

Under this tab, you allocate the consignments to the unloading sites.

## Date Overview
*Production > Date Overview > Date Overview*

You can use the Date Overview to check what needs to be produced within a certain space of time, and which material is required for this purpose.

This chapter provides information on the following subjects:
- "Date Overview – Menus" on page E-266
- "Date Overview (Dialog)" on page E-267
- "Export" on page E-274

### Date Overview - Menus
The menus in the Date Overview dialog serve to define the default setting for the dialog and open other dialogs without closing the schedule.

This chapter provides information on the following subjects:
- "Functions menu" on page E-266
- "Options menu" on page E-266

#### Functions menu
*Production > Date Overview > Date Overview > Functions menu*

The Table tab can be used to open other dialogs without closing the schedule.

**Documents group**
- **History:** Opens a list of processing steps and status changes for the selected document. For a detailed description, please see the chapter Sales.
⇨ Sales, "History" on page C-550
- **Display:** Opens the Document dialog and provides a document preview.
⇨ Sales, "Complaints" on page C-589

**Selection group**
- **Export:** Opens the Export dialog where you can define which data should be saved in an export file.
⇨ "Export" on page E-274

#### Options menu
*Production > Date Overview > Date Overview > Menu Options*

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog. The following entries are displayed:
- **Automatic paging enabled:** A new page will be started for every date and order.
- **Archives:** Archives are used to analyze reference periods of the previous year, for example.

### Date Overview (Dialog)
*Production > Date Overview > Date Overview*

The Date Overview dialog can be used to check which quantities have to be produced within a certain space of time, and the material required for this purpose. The analyses can be printed or exported.

This dialog offers the following tabs:
- "Date Overview – Selection" on page E-268
- "Date Overview – Table” on page E-273

#### Date Overview - Selection
*Production > Date Overview > Date Overview > Selection tab*

*Fig. E-132 Date Overview - Selection*

On this tab, you create the criteria for the orders that should be displayed on the Table tab.
⇨ "Date Overview - Table" on page E-273

**Source**
This option defines the way in which you are going to search for orders:
- **Number:** You can view a single order. The fields for entering the order number and the evaluation period are activated.
- **Number Manager:** You can view the orders of a number manager. The field for selecting the number manager is activated.

> **Material per order**
> When you select a single order, you can use the evaluation mode and the breakdown level to compile a list of all material that is going to be used for the selected order.

**Client:** If you are using clients, the selection can be restricted to a certain client.

**Production preparation:** If you are using production preparations, you can restrict the selection to a certain preparation.

**Evaluation mode**
This option defines how the orders are going to be evaluated:
- **Production area:** The fields in section Production area are activated so that you can select the desired area.
- **Product groups:** The fields in the section Select product group are activated so that you can choose a product group.
- **Product:** The fields in section Select product are activated so that you can choose a product.

**Evaluation period**
The fields in this section are only accessible if you have chosen the option Number in the Source section and leave this field blank. You can display all orders for a certain period in this case.
- **By delivery date:** The defined period refers to the delivery date.
- **By production date:** The defined period refers to the production date.
- **From, to:** Period to be evaluated.

**Production areas**
Choose an option to define the production area you want to assess. The fields are only accessible if you have selected the evaluation mode By production area.
- **IG:** Only shows orders with IG items.
- **LG:** Only shows orders with laminated glass items.
- **TG:** Only shows orders with toughened glass items.
- **Annealed glass:** Only shows orders with annealed glass. This also applies for single glass processed in ISO.
- **Cutting:** Shows all orders that include the cutting of glass.
- **IG auxiliary material:** Shows all orders which include auxiliary material for IG production.
- **All:** Shows all orders.

**Restrictions**
You can also restrict the evaluation to one of the following supplementary conditions. The checkboxes Shape cutting to Processing steps are only accessible if you have selected the evaluation mode By production area.

- **Shape cutting:** You can restrict the evaluation to shapes.
    - Evaluation will not be restricted to shapes.
    - The evaluation only refers to items which include shapes.
- **Grill production:** Evaluation can be limited to Georgian bar patterns.
    - Evaluation will not be restricted to Georgian bars.
    - The evaluation only refers to items which include Georgian bar patterns.
- **Stepped:** You can restrict the evaluation to steps.
    - Evaluation will not be restricted to steps.
    - The evaluation only refers to items which include steps.
- **Processing:** You can restrict the evaluation to processing steps.
    - Evaluation will not be restricted to processing steps.
    - The evaluation only refers to items which include processing steps.
- **In-house production:** Evaluation can be restricted to in-house production. In-house production includes orders of the supply types Cutting, Production, Processing.
    - Evaluation will not be restricted to in-house production.
    - The evaluation only refers to items which include in-house production.
- **Stock:** You can restrict the evaluation to stock articles.
    - Evaluation will not be limited to stock articles.
    - Evaluation only refers to items with stock articles.
- **Purchasing:** You can restrict the evaluation to purchased articles.
    - Evaluation will not be restricted to purchased articles.
    - The evaluation only refers to items which include purchased articles.

**Select status range**
By restricting the list to a status you can e.g. select quotations or orders which have not been transferred to production yet.
- **From, to:** The combo boxes show all status points defined in the master data.

**Select product group**
This option defines the product group to be evaluated. The fields are only accessible if you have selected the evaluation mode By product group.
- **PGR:** All orders containing products from a certain product group will be assessed. The field for selecting the product group is activated. You can select the PGR from any of the three product group levels. If this field is left blank, all product groups will be displayed.
- **PGR statistics:** The field for selecting the statistics product group is accessible.

You can select a product group (PGR), super product group (PSG), or main product group (MPG). The evaluation always shows the main product group (MPG), however.
If you also need product groups (PGR) or super product groups (PSG) for your evaluation you can switch to the Capacity overview dialog.
⇨ "Capacity Overview" on page E-275

**Combined PGR:** Evaluation can also include combined product groups (combined PGR).
- The product's original PGR will be displayed.
- The combined PGR will be displayed.

> **Example:**
> Float 4 = PGR 100
> Drilled hole = PGR 801
> Float 4 with drilled hole (combination of 100 and 801) = Combined PGR 860
>
> Evaluation on PGR level shows PGR 100 and 801.
> PGR 860 is displayed.

**Select product**
You can restrict the evaluation to orders which include a certain product. These fields are only accessible if you have selected the evaluation mode By product.
- **Product type:** Evaluation can be limited to a product type, e.g. to product type Article to check which accessories have to be ordered for production.
- **Product class:** You can only choose a product group after selecting a product type.
- **Product:** Evaluation can be restricted to a certain product.

**Breakdown level**
The breakdown level defines how detailed the orders are going to be displayed. You can check several checkboxes.
- **Per date:** The orders can be displayed by delivery date. This setting is useful if you want to get an overview of the products to be produced in the coming week, for example.
    - The delivery date will not be used as a criterion.
    - Orders will be grouped by delivery date.
- **Per order:** Every order will be evaluated separately. This setting is useful if you have selected a production area, for example.
    - Individual orders will not be displayed.
    - The list will be grouped by orders.
- **Per item:** Every single order item will be evaluated. The checkbox is only activated if the checkbox by order is checked. This setting is useful for evaluating orders with very many items and large quantities, for example.
    - Individual items will not be shown.
    - The individual order items will be listed.
- **Per customer:** The orders can be displayed by customer. This setting is useful for evaluating orders of a customer, for example.
    - Individual customers will not be displayed.
    - Orders will be grouped by customers.
- **Subtotal per QU:** A subtotal can be displayed.
    - No subtotal will be displayed.
    - The subtotal for the quantity units entered in the items will be shown per order.

**Gas calculation**
- **Individual gas calculation:** You can change the display of the quantity unit for gas. If, for example, the product gas has been defined in product master data in the quantity unit kg, the quantity consumed can be displayed in liters.
    - Gas calculation is not converted.
    - Gas calculation is converted to new quantity unit.
- **Quantity unit:** Specification of new quantity unit. The quantity is only converted if checkbox Indiv. gas calculation is enabled.

#### Date Overview - Table
*Production > Date Overview > Date Overview > Table tab*

*Fig. E-133 Date Overview - Table*

This tab displays all orders that correspond to the criteria that you have specified on the Selection tab.
⇨ "Date Overview - Selection" on page E-268

**Result**
The evaluation appears on the list. The display of the columns depends on the selected criteria. You can view each order in the menu Functions > Show document in the document view.

**Totals**
The overview displays the totals of all orders in the Result area.

### Export
*Production > Date Overview > Date Overview > Functions menu > Selection Group > Export*

*Fig. E-134 Exporting the schedule*

The Export function can be used to export the data to an ASCII file for further analysis.

**Path/File name**
Enter the path and the file name of the transfer file. Use ASC or TXT as a format.
After the export, the field Export shows the number of records that were saved in the file.

**Export fields**
This section shows the fields from which data can be exported. The corresponding code for the display format is shown for information.

## Capacity Overview
*Production - Date Overview - Capacity Overview*

*Fig. E-135 Capacity overview*

In this dialog you can display a preview of the capacities you will be needing to produce certain product groups.

> **No connection with capacity planning**
> Capacity planning is not connected with A+W Business capacity planning and does not process any reports from the shop floor.

**Break down by**
This option defines the breakdown level. You can also select individual product groups.
- **Main product group:** Only main product groups (MPG) will be evaluated.
- **Super product group:** Within the MPG, there is a differentiation by super product groups (PSG).
- **Product group:** Within the PSG, there is a differentiation by product groups (PGR).
