---
title: "EN_AWBusiness_Capacity_Planning_4_4"
source: "EN_AWBusiness_Capacity_Planning_4_4.pdf"
tags: ["capacity planning", "production reports", "A+W Business Pro", "software reference", "scheduling", "machine utilization", "production management", "ERP", "manufacturing software", "control station"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the Capacity Planning module of A+W Business Pro, version 4.02. It details functionalities for managing production reports, scheduling orders, and utilizing the Control Station to oversee and adjust production capacity."
long_description: "This software reference manual provides a comprehensive overview of the A+W Business Pro Capacity Planning module. It is intended for users responsible for production scheduling, reporting, and capacity management. The guide begins with instructions on handling Production Reports, including how to enter breakage reports and configure settings for manual completion reports. It then explains how to generate and customize Production Lists, detailing various print settings and data sorting options. A significant portion of the document is dedicated to the 'Production Level Orders' dialog, which allows users to check and report the completion status of individual machines, orders, and items down to the Bill of Materials (BOM) level. The manual provides a detailed walkthrough of the 'Control Station,' a central hub for checking and correcting the entire production schedule. It covers viewing machine utilization by area, machine, or order, and provides tools for manually rescheduling orders and items. This includes moving production times, changing machines, and managing capacity conflicts. The document also explains how to interpret graphical utilization displays, manage purchased elements, and configure various settings to tailor the view to specific user needs. The guide concludes with a detailed index for quick reference to specific topics and functionalities."
---

# Software Reference: Production Reports

> A breakage report can be entered only if the item has been reported completed before.
> This means that a sheet which is damaged at the station where it has been processed can be reported broken only after the completion report has been issued.
> A sheet that arrives damaged at the station, has already been reported completed by the previous station and can therefore be reported broken right away.

**Select machine**: In this field, the machines are displayed that are available in the selected production area. You have to mark one of the suggested machines so that you can enter the report. The program will offer only the machines that are eligible for the current user.
⇨ "Settings for Manual Completion Reports" on page H-301

---
## Settings for Manual Completion Reports

**Path**: `Production > Capacity planning > Completion report > Manually > Functions menu > Settings`

_Fig. H-196 Machine selection for manual report_

On this dialog, you specify for which production area and which machines the production employee can record reports.

### Select machines

**Production area**: Selection of the production area in which the respective employee shall record reports. The program then lists all machines belonging to the selected production area. You can choose only one production area at a time but you can choose as many of the listed machines as you like. You have to select at least one entry.

**Scanner**

**Separator**: Specification of the separator with which the barcodes are separated if several codes are scanned in succession. This specification must match the scanner setting. Please refer to the scanner's operating instructions for details.

## Production Lists

**Path**: `Production > Capacity planning > Production lists`

_Fig. H-197 Production lists_

On this dialog, you can evaluate which quantity of which order must be produced on a particular machine and when the order is required on which subsequent machine.

### Settings menu

Using this menu, you can specify the sorting of the data for printing.
⇨ "Settings for Production Lists" on page H-306

### Selection

**From date, to date**: Entry of the date or the time range for which you require the production papers.

**Machine**: Selection of the machine for which the production papers shall be printed. For selection, only the machines are offered for which processes are scheduled on the selected date or in the selected period.

### Print settings

The checkboxes in this group are only released in selection mode.

**Reprint**: You can print the production papers several times on a day. You can also specify whether only the new data shall be printed, or all data.
- By default, only the new data will be printed, i.e. the data which have not been printed before.
- All data for that day - up to the present point in time – will be printed.

**Print for all machines**: You can specify whether the production papers shall be printed for a single machine or for all machines.
- The data will only be printed for the machine defined in field Machine.
- The data of all machines will be printed.

**Incl. information on origin**: You can also print the production area from which the item came.
The checkbox is blocked if the output on the production papers is summarized by orders or items.
- The previous production area is not displayed.
- The previous production area is displayed.

**Orders summarized**: You can summarize the data by orders.
- The orders are printed individually.
- The data will be summarized per order. The checkbox for the items is automatically ticked and cannot be deactivated. With this setting, no origin information can be printed.

**Items summarized**: You can summarize the data by order.
- For each order item, one line per machine is printed.
- The items of an order are summarized and printed in one line. With this setting, no origin information can be printed.

**Show set up times as well**: Set-up times can be displayed only if they have been defined as basic times and allocated appropriately.
- Setup times are not printed.
- The setup time is printed.

### Table

In the overview, all data is displayed that match the selection criteria. Depending on the settings in the Print settings group, the following columns are displayed:

- **Date**: Production date.
- **Shift**: Shift in which the order or item was produced.
- **Order**: Order number.
- **Priority**: Priority from the order or from the scheduling.
- **Status**: Order status.
- **Item**: Number of the order item.
- **Item status**: Item status.
- **Product**: Product name.
- **Glass size**: Size of the item.
- **Shape**: Shape number.
- **Element**: Product name of the BOM component.
- **Processing**: Product name of the processing.
- **Work type**: Name of the work type.
- **Pcs**: Number of pieces of the item.
- **Quantity**: Number of sheets.
- **Sqm/pc**: Area per piece.
- **Lm/pc**: Linear meters of the edges per piece.
- **Next processing**: Next processing (process).
- **Following machine**: Machine.
- **Date**: Production date on the current machine.
- **Customer**: Customer name from the order.
- **BOM part**: Number of the BOM component.
- **Previous Machine, Previous work type, Production date**: Data for the previous process.

## Production Lists – Print

**Path**: `Production > Capacity planning > Production lists > Print menu > Printer`

_Fig. H-198 Production lists – Print_

In the printed lists, the order items are displayed with size, quantities, and next processings. The output is set with the checkboxes on the Production lists dialog.
⇨ "Print settings" on page H-303

## Settings for Production Lists

**Path**: `Production > Capacity planning > Production lists > Settings menu > Production lists`

_Fig. H-199 Settings for production lists_

On this dialog, you select the criteria for sorting the production list.

### Production list

**PRLIST Variables (0,1,2)**: The `PRLIST` variable setting depends on the report definition. By default, the following settings are available for printing the report:
- **0**: If the product texts of main product and BOM product are identical, the text is only printed for item 1.
- **1**: If the product texts of main product and BOM product are identical, the text is only printed for item 2.
- **2**: Both texts, both the text for the main product and the text for the BOM product are printed on the list.

**Example**

| | Text main product = Float 4 mm, Text BOM product = Float 4 mm | Text main product = IG, Text BOM product = Float 4 mm |
|---|---|---|
| **No.** | **Text item 1** | **Text item 2** | **Text item 1** | **Text item 2** |
| 0 | Float 4 mm | - | IG | Float 4 mm |
| 1 | - | Float 4 mm | IG | Float 4 mm |
| 2 | Float 4 mm | Float 4 mm | IG | Float 4 mm |

### Sorting by

With the selection of the option, you specify how the data shall be sorted in the production papers.

### Status

**From, to**: Status or status area of orders to be printed.

## Production Level Orders

**Path**: `Production > Capacity planning > Production level orders`

On this dialog, you can check and report completed individual machines, orders, and order items down to the BOM level.

There are the following tabs on the Order dialog:
- "Production Level Order – Selection" on page H-310
- "Production Level Orders – Overview" on page H-311
- "Production Level Orders – Items" on page H-312
- "Production Level Orders – Detail" on page H-314
- "Production Level Orders – P.O. Elements" on page H-315
⇨ Tutorial, "Check Production Status" on page H-148

### Navigation through the tabs and dialogs

The following overview shows you how to display the data.

| Tab | Action | Tab / dialog |
|---|---|---|
| Selection | Click on row header | -> Items |
| Items | Click on row header | -> Detail, P.O. elements |
| Detail | Click on row header | -> Production level orders |

### Functions Menu

**Path**: `Production > Capacity planning > Production level orders > Functions menu`

Using this menu, you can open other dialogs without closing the Completion report order dialog.

#### Document group
- **Display**: Opens the view of the document.
- **History**: Opens the History dialog on which you can check the course of the status changes. ⇨ Sales, "History" on page C-478
- **Status change**: Opens the dialog by the same name on which you can changes the status of the order. ⇨ Sales, "Status Change" on page C-479

#### Reports group
- **Overview**: Opens the Reports dialog to check the status of the individual items. ⇨ "Report List" on page H-318

#### Capacity planning group
- **Completion report by date**: Opens the Date dialog to report the order completed. ⇨ "Date" on page H-292
- **Move**: Opens the Change production times dialog to move the order. ⇨ "Change Production Times" on page H-319

#### Scheduling group
- **Scheduling**: Opens the Schedule order dialog to schedule the order. ⇨ "Book Order" on page H-275
- **Delete**: Deletes the selected order from capacity planning. After that, the order can be rescheduled. The right to delete can be limited in the rights management.

#### Status group
- **Show graphics**: Opens the graphical display of the completed and open work per item. The entry is only released on the Items tab. ⇨ "Graphic" on page H-295

#### Miscellaneous group
- **Update purchase prices**: Updates the purchase prices of the selected order. ⇨ "Report List" on page H-318
- **LG numbers**: This entry is only released customer-specifically.

## Production Level Order – Selection

**Path**: `Production > Capacity planning > Production level orders > Selection tab`

_Fig. H-200 Production level orders – Selection_

On this tab, you select an order for one customer or several orders for the delivery date. The orders found are listed in the Table group.

### Order, customer, date

In this group, you set the selection criteria.

**Number**: With the entry of the order number the order data are displayed.
**Number**: With the entry of the customer number, all orders for the customer are displayed.
**Customer**: The customer name is displayed automatically.
**Delivery date**: With the entry of the delivery date, all orders with this date are displayed.

### Completion report

**Enter date**: If you want to report an order completed, you can specify the date.
- The current date is entered as completion report date.
- You can change the date. The order is reported completed with the changed date.

**Production date**: Display of the production date for the order that is selected on the overview.

### Result

In the overview, all orders are displayed that correspond to the selection criteria.

## Production Level Orders – Overview

**Path**: `Select Production > Capacity planning > Production level orders > Overview tab`

_Fig. H-201 Production level orders - Overview_

On this tab, you can view details on the calculation of the selected order.

### Production

**Start, End**: Display of the respective dates for the order that is marked on the Selection tab.

### Quantity

- **Pcs**: Total quantity of the order.
- **Completed**: Quantity completed.

### Calculation

- **Material cost**: Material cost from the order.
- **Planned time costs**: Calculated time costs.
- **Total costs planned**: Total of material cost and planned time costs.
- **Order value**: Total order value.
- **Actual time costs**: Actual time costs. This value is calculated based on the report from A+W Production.
- **Actual total costs**: Total of material cost and actual time costs.

## Production Level Orders – Items

**Path**: `Select Production > Capacity planning > Production level orders > Items tab`

_Fig. H-202 Production level orders - Items_

On this tab, all items of a selected order are listed. You can report manually individual items completed.
The fields are described on the Selection tab.
⇨ "Production Level Order - Selection" on page H-310

### Table

In the overview, all items per order are displayed.
- **Item**: Items of the selected order.
- **Article**: Name of the article that is included in this item.
- **Date**: Production date of the first process on the main product of the item.
- **Pcs.**: Item quantity.
- **Size**: Size of the item.
- **Completed w/o processing**: Display of the quantity for which the cutting has already been done, but not yet the processing, e.g. drilling. However, this statement is very imprecise because the glass is usually subjected to a multitude of processings. A precise statement of the state of production can therefore only be made with the reports from the registration points in production. ⇨ "Report List" on page H-318
- **Completely finished**: Number of completely finished units of an item.
- **Ordered**: Display whether there are ordered articles.
- **Completion report**: Display whether the item was reported completed.

## Production Level Orders – Detail

**Path**: `Select Production > Capacity planning > Production level orders > Detail tab`

_Fig. H-203 Production level orders - Detail_

On this tab, the BOM components are displayed per item. The tab is released only if you have selected an order item with BOM on the Items tab.
With a click of the header row, you open the Production status > Date dialog.
⇨ "Date" on page H-292

### Table

In the overview, all BOM components of the current item are displayed.
- **Date**: Production date.
- **Shift**: Shift in which the item shall be produced.
- **BOM ID**: BOM ident number, that is the BOM level.
- **Product**: Product name.
- **Work type**: Work type.
- **Pcs.**: Item quantity.
- **Completed**: Quantity that was reported completed.
- **Machine**: Machine on which the item is or was produced.

## Production Level Orders – P.O. Elements

**Path**: `Select Production > Capacity planning > Production level orders > P.O. elements tab`

_Fig. H-204 Production level orders – P.O. elements_

On this tab, the P.O. elements are displayed that are included in the items of the current order.
With a click of the header row, you open the Schedule P.O. elements dialog.
⇨ "Scheduling of Purchased Elements" on page H-317

### Table

In the overview, all items are listed that contain P.O. elements.
- **Item**: Item number from the order.
- **Article**: Product name of the P.O. element.
- **Pcs.**: Quantity to be purchased.
- **Size**: Dimensions of the item.
- **Ordered for (date)**: Requested delivery date.
- **Quantity delivered**: Quantity already delivered.
- **Required on, Date, Shift**: These three columns display when the purchased elements are required where.

## Production Status – Graphic

**Path**: `Select Production > Capacity planning > Production level orders > Items tab > Functions menu > Status group > Show graphics`

_Fig. H-205 Production status of order items_

This display shows you the quantities of an order in graphical form.

## Scheduling of Purchased Elements

**Path**: `Select Production > Capacity planning > Production level orders > P.O. elements tab > Click in row header`

_Fig. H-206 Scheduling of purchased elements_

On this dialog, you schedule the purchased elements after the receipt of goods.

## Report List

**Path**: `Select Production > Capacity planning > Production level orders > Functions menu > Reports group > Overview`

_Fig. H-207 Completion report order – Production reports_

On this dialog, you check which positions were reported completed on which machines.

### Order information
- **Order**: Number of the order.
- **Address**: Name and address of the customer.
- **Status**: Status of the order.
- **Production**: Start and end date of production.

### Order information (colored display)
For each order item, a column with the current reports is displayed. The reported figures are displayed in different colors:
- **Black**: 0 indicates that no pieces of the item have been produced.
- **Green**: the reported quantity corresponds to the item quantity.
- **Blue**: the reported quantity is only a partial quantity of the item.
- **Red**: the reported quantity must be ordered again, e.g. due to breakage.

### Item overview

In this field, the BOM structure is displayed if you double-click in the Order information group on the column heading of an item.

## Change Production Times

**Path**: `Select Production > Capacity planning > Production level orders > Functions menu > Capacity planning group > Move`

You can change the dates and machines that were planned for an order. Thereby the capacities are not considered, however, so that you can move the process of an order item to a machine that is already fully utilized.

This dialog contains the following tabs:
- "Change Production Times – Selection" on page H-320
- "Change Production Times – Overview" on page H-321
- "Change Production Times – Overview 2" on page H-323

### Plant Menu

**Path**: `Select Production > Capacity planning > Production level orders > Functions menu > Capacity planning group > Move > Change production times > Plant menu`

Using this menu, you specify whether the capacity of an individual plant or all plants shall be considered.
- **All**: All defined production areas are displayed.
- **Plant 1**: Only the production areas with entry 0 and 1 are displayed.
- **Plant 2**: Only the production areas with entry 0 and 2 are displayed.
- **Plant 3**: Only the production areas with entry 0 and 3 are displayed.

The plant refers to the key that is entered in the company data for a site. The sites are then assigned on the Production areas dialog.

## Change Production Times – Selection

**Path**: `Select Production > Capacity planning > Production level orders > Functions menu > Capacity planning group > Move > Selection tab`

_Fig. H-208 Change production times – Selection_

On this tab, the machines for a selected date are displayed.

### Selection
**Production date**: Selection of the date on which the order shall be produced.

### Machines by product area
The following data is displayed in the overview:
- **Production areas/Machines**: All machines of the production area for which orders have been scheduled for the production date.
- **Pcs.**: Quantity to be produced by the corresponding machine.
- **Hours**: Utilization of the machine in hours.
- **Set-up time**: Set-up times can be scheduled in addition to the hours. Set-up times will be displayed only if they are allocated to the machine in question.

## Change Production Times – Overview

**Path**: `Production > Capacity planning > Production level orders > Functions menu > Capacity planning > Move > Overview tab`

_Fig. H-209 Change production times – Overview_

On this tab, all orders and/or items are displayed that shall be produced on the current machine on the production date. You can change the date, the shift, and the machine for an item or for an entire order.

### Order overview by machine
- **Machine**: Current machine. In selection mode, any machine can be chosen.
- **Suppress message**: Errors that occur during rescheduling for another date or another machine are displayed in a message.
    - The message is displayed.
    - ☑ Messages are not displayed.

### List
In the overview, all orders are listed that shall be produced on the machine on the current day.
- **Delivery date, Number, Customer**: Delivery date, order number, and customer name from the order.
- **Shift**: Shift in which the order in question shall be produced.
- **Pcs.**: Quantity to be produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Hours scheduled for this order.

### Allocation of elements
In the overview, all items of the selected order are listed that shall be produced on the machine on the current day.
- **Shift**: Shift in which the item shall be produced.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, i.e. the BOM level.
- **Sub item**: Sub-items resulting from the splitting of items at scheduling.
- **Process**: Work type for the BOM item.
- **Product/Processing**: Product name.
- **Pcs.**: Item quantity.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Hours planned for the order.

### Changed
The changes in these fields apply to the order or the item, based on the selection in the Move column.
- **New date**: Production date to which the order shall be moved.
- **Shift**: Shift to which the order shall be moved.
- **New machine**: Selection of an alternative machine.

## Change Production Times – Overview 2

**Path**: `Production > Capacity planning > Production level orders > Functions menu > Time management group > Move > Overview 2 tab`

_Fig. H-210 Change production times – Overview 2_

On this tab, detailed information per shift and machine is displayed.

### Work type overview by machine
In the overview, all work types are listed that are scheduled on the machine on the current day.
- **Number**: ID of the work type.
- **Process**: Work type on the machine.
- **Shift**: Shift in which the work in question shall be performed.
- **Quantity**: Quantity to be produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Utilization of the machine in hours.
- **Setup time**: Set-up times can be scheduled in addition to the hours. Set-up times will be displayed only if they are allocated to the machine in question.

### Order overview by work type/shift
In the overview, all orders with the same work type per shift are listed:
- **Order, Customer**: Order number and customer name from the order.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, i.e. the BOM level.
- **Sub item**: Sub-items created by splitting the item at scheduling.
- **Product/Processing**: Product name.
- **Quantity**: Quantity to be produced.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Hours planned for the item.

### Changed
The fields in the Changed group are described for the Overview tab.
⇨ "Change Production Times – Overview" on page H-321

## Control Station

**Path**: `Production > Capacity planning > Control station`

On this dialog, you can check and correct the entire scheduling.
This section provides information on the following subjects:
- "Control Station (Dialog)" on page H-326
- "Settings for Control Station" on page H-359
- "Control Station (Machine)" on page H-344
- "Utilisation (Date)" on page H-351
- "Utilisation - Print" on page H-358
- "Display Status" on page H-359
- "Settings for Control Station" on page H-359
- "Residue Qty." on page H-361
- "Control Station (Order)" on page H-362
- "Moving impossible" on page H-375
- "Change Production Times" on page H-319
⇨ Tutorial, "Control Station" on page H-161

### Functions Menu
**Path**: `Production > Capacity planning > Control station`

Using this menu, you can open other dialogs without closing the control station.

#### Additional displays group
- **Select order**: Opens the Control station (order) dialog on which you can edit the scheduling of the order. ⇨ "Control Station (Order)" on page H-362
- **Display residual quantities**: Opens the Residual quantities dialog to report these completed. ⇨ "Residue Qty." on page H-361

#### Display group
- **Graphic**: Opens a graphical display to compare the produced and remaining quantities. ⇨ "Graphic" on page H-295
- **Utilization**: Opens the Utilization on date dialog. The entry is only released on the Machines and Orders tab. ⇨ "Utilisation (Date)" on page H-351

#### Settings group
- **Settings**: Opens the Settings for control station dialog where you can define the data to be displayed by the control station. ⇨ "Settings for Control Station" on page H-359
- **No messages**: After scheduling, a message with various information about the scheduling is suppressed. The entry is only released if you are logged in with administrator rights.

## Control Station (Dialog)

**Path**: `Production > Capacity planning > Control station`

On this dialog, you check the utilization of the machines. On various tabs, you can reschedule manually entire orders or individual items.
The Control station dialog contains the following tabs:
- "Control Station – Areas" on page H-328
- "Control Station – Machines" on page H-329
- "Control Station – Orders" on page H-330
- "Control Station – Reschedule Order" on page H-332
- "Control Station – Reschedule Item" on page H-334
- "Control Station – Work Types" on page H-336
- "Control Station - Details" on page H-338
- "Control Station – Shifts" on page H-340
- "Control Station – Prev. Processes" on page H-341
- "Control Station - Purchased Elements" on page H-343
⇨ Tutorial, "Concept of the Control Station" on page H-162

### Navigation through the tabs and dialogs

The following overview shows you how to display the data.

| Tab | Action | Tab / dialog |
|---|---|---|
| Areas | Double-click on row header | -> Machines (all machines) |
| | Double-click on production area | -> Machines (only machines in the production area) |
| Machines | Double-click on machine | -> Orders |
| | Double-click on detail data | -> Reschedule order |
| | Double-click on row header | -> Control station (machine) |
| Orders | Double-click on number | -> Control station (order) |
| | Double-click on detail data | -> Reschedule item |
| Reschedule order | Click on row header | -> Reschedule item |
| | Click on [Elements] or [Prev.processes] | -> Prev. processes |
| Reschedule item | Context menu for process (right mouse key) | -> Delete setup time, Add setup time |
| Work types | Click on row header | -> Details |
| Details | Double-click on number | -> Control station (order) |
| Prev. processes | Click on [In Detail] | -> Production lists |

### Period displayed

When opening the dialog, the current and next week are displayed. With the navigation buttons, you can page forward and back across days or weeks.

## Control Station – Areas

**Path**: `Production > Capacity planning > Control station > Areas tab`

_Fig. H-211 Control station – Areas_

On this tab, you check the utilization of the production areas.

### Navigation through the tabs

| Action | Tab |
|---|---|
| Double-click on row header | -> Machines |
| Double-click on production area | -> Machines (only machines in the area) |
| Buttons for navigation | -> Page forward and back day by day |

### Overview
The following data is displayed in the overview:
- **Production area**: Production areas that are used in the period displayed.
- **Day of the week, Date**: The planned day per day of the week (all shifts) is displayed.

## Control Station – Machines

**Path**: `Production > Capacity planning > Control station > Machines tab`

_Fig. H-212 Control station - Machines_

On this tab, you check the utilization of per machine.

### Navigation through the tabs and dialogs

| Action | Tab / dialog |
|---|---|
| Double-click on machine | -> Orders |
| Double-click on details | -> Reschedule order |
| Double-click on row header | -> Control station (machine) dialog |

### Overview
The following data is displayed in the overview:
- **Machine**: Machines of the production area. If you have changed to the Machines tab from the Areas tab with a double-click, only the machines are displayed that belong to the appropriate production area.
- **Day of the week, Date**: The utilization with the following totals of all shifts per machine can be displayed per day of the week:
    - Scheduled and free time (all shifts)
    - Open and produced quantity of all sheets in pcs.
    - Total surface in sqm
    - Edge length of all sheets
    - Utilization in percent
All details except for the time can be selected or deselected in the control station settings.
⇨ "Settings for Control Station" on page H-359

## Control Station – Orders

**Path**: `Production > Capacity planning > Control station > Orders tab`

_Fig. H-213 Control station - Orders_

On this tab, you check the utilization of the machines per order.

### Navigation through the tabs and dialogs

| Action | Tab / dialog |
|---|---|
| Double-click on number | -> Control station (order) dialog |
| Double-click on quantity | -> Reschedule item |

### Overview
The following data is displayed in the overview:
- **Order, Status, Customer**: Order number, status, and name of the customer from the order.
- **Day of the week, Date**: The utilization with the following details per day of the week is displayed:
    - Scheduled and free time (all shifts)
    - Open and produced quantity of all sheets in pcs.
    - Total surface in sqm
    - Edge length of all sheets
    - Percentage of the utilization, e.g. 29% means that this order has a share 29% in the available 100% utilization.

## Control Station – Reschedule Order

**Path**: `Production > Capacity planning > Control station > Machines tab > Double-click on machine > Reschedule order tab`

_Fig. H-214 Control station - Reschedule order_

On this tab, you move an order on the machine in question, e.g. to another date, another shift or another machine.

### Navigation through the tabs
- Click on row header -> Reschedule item
- Click on [Elements] -> Prev. processes - Elements
- Click on [Prev. processes] -> Prev. processes
- **[Elements]**: Changes to the display of the items on the Prev. processes tab.
- **[Prev. processes]**: Changes to the display of previous processes on the Prev. processes tab.

### Overview
The following data is displayed in the overview:
- **Delivery date**: Delivery date from the order.
- **Order, Status, Customer**: Order number, status, and name of the customer stated in the order.
- **Shift**: Currently-scheduled shift.
- **Pcs.**: Quantity of the sheets or processings.
- **Finished**: Number of sheets produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Time reserved for this order.

### Move
- **New date**: Production date to which the order shall be moved.
- **Shift**: Shift to which the order shall be moved.
- **Machine**: Machine to which the order shall be moved. The field is released if you have ticked the Move checkbox on the Start > Execute menu.
- **[Load]**: Checks the utilization of the new machine. The value is displayed in hours. It includes the times for the order you have selected by clicking on the row header.
- **Without check**: You can force the moving of an order or an order item. Before moving, there is a check whether there are sufficient free capacities on the new date, on the new machine, and/or for the new shift. If the capacities are not sufficient, a message indicates that the moving is impossible. You will have to move the order elsewhere in that case. The move is accepted without a check even if this exceeds the capacity.

## Control Station – Reschedule Item

**Path**: `Production > Capacity planning > Control station > Machines tab > Double-click on detail data > Reschedule item tab`

_Fig. H-215 Control station - Reschedule item_

On this tab, you can move an order item to another date, another shift or another machine. The Process column displays the work type.

> **Edit set-up times**
> Use the context menu for a process (right mouse-button) to add or delete set-up times.

- **[Product]**: For long lists, you can highlight all entries in the display that contain a particular product. Tick the line that includes the required product. When you click on this button, all lines that include the same product will be selected.
- **[All], [None]**: You can use these buttons to tick or untick all checkboxes in the Move column.

### Overview
The following data is displayed in the overview:
- **Shift**: Shift in which the item shall be produced.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, that is the BOM level.
- **SI**: Sub-items resulting from the splitting of items at scheduling.
- **Process**: Work type.
- **Product/Processing**: Product name.
- **Pcs.**: Item quantity.
- **Finished**: Quantity of sheets produced.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Time reserved for this item.

### Move
The fields in this group are described for the Reschedule order tab.
⇨ "Control Station - Reschedule Order" on page H-332

## Control Station – Work Types

**Path**: `Production > Capacity planning > Control station > Work types tab`

_Fig. H-216 Control station – Work types_

On this tab, you check which work types are to be performed on a machine on a production date. The tab is only filled if you have displayed elements or previous processes.

### Navigation through the tabs
- Click on row header -> Details
- **[Elements]**: Changes to the display of the items on the Prev. processes tab.
- **[Prev. processes]**: Changes to the display of previous processes on the Prev. processes tab.

### Overview
The following data is displayed in the overview:
- **Number**: Number of the work type.
- **Process**: Name of the work type.
- **Articles**: Name of the product.
- **Shift**: Shift in which this work type shall be performed.
- **Pcs.**: Item quantity.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Time reserved for this item.

### Move
The fields in this group are described for the Reschedule order tab.
⇨ "Control Station - Reschedule Order" on page H-332

## Control Station – Details

**Path**: `Production > Capacity planning > Control station > Prev. processes tab > Click in row header > Details tab`

_Fig. H-217 Control station – Details_

On this tab, detailed information per shift and work type is displayed.

### Navigation
- Double-click on order number -> Control station (order) dialog

### Overview
The following data is displayed in the overview:
- **Order, Customer**: Order number and customer name from the order.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, i.e. the BOM level.
- **SI**: Sub-items resulting from the splitting of items at scheduling.
- **Product/Processing**: Product name.
- **Pcs.**: Item quantity.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Time reserved for this item.

### Move
The fields in this group are described for the Reschedule order tab.
⇨ "Control Station - Reschedule Order" on page H-332

## Control Station – Shifts

**Path**: `Production > Capacity planning > Control station > Shifts tab`

_Fig. H-218 Control station – Shifts_

On this tab, you see the machine utilization per shift.

### Overview
The following data is displayed in the overview:
- **Machine**: Machine name.
- **Shift**: One line is displayed per shift.
- **Day of the week, date**: Scheduled time and shift time in hours, per shift.

## Control Station – Prev. Processes

**Path**: `Production > Capacity planning > Control station > Reschedule order tab > [Elements], [Prev. processes] > Prev. processes tab`

_Fig. H-219 Control station – Prev.processes_

On this tab, you check from which production area the items come, for which the current data are displayed. You can display the data in the Elements and Prev. processes modes.

### Navigation
- Click on row header -> Order column is displayed
- **[In detail]**: Opens the Production list dialog to check for which orders the previous machines are utilized. ⇨ "Production Lists" on page H-302
- **[Elements]**: Changes to display of the items.
- **[Prev. processes]**: Changes to display of the previous processes.

### Selection
This group displays the number and area of the elements in total and per shift.

### Options
In Prev. processes mode, you can display additional information.
- **With name**: In the Elements column, the product name is displayed.
- **With work type**: In the Prev. work type column, the work type is shown that was performed previously.
- **By areas**: If there are several machines available for the previous processes, the display in the Comes from column can be toggled between production area and machine.
- **With order items**: The order items are also displayed.
- The additional information is not displayed.
- The additional information is shown in the overview in an additional column. The selection must be confirmed on the Start > Execute menu to update the display.

### Overview (Elements / Previous processes)
By default, the following columns are displayed in the overview:
- **Work type**: Name of the work type in the production area.
- **Order**: The order number is displayed if you click on the row header.
- **Customer**: The customer name is displayed if you click on the row header in Elements mode.
- **Quantity**: Number of sheets in the shift.
- **Element**: Product name (Elements mode).
- **Article no.**: Product number (Elements mode).
- **Sqm**: Total area in the shift (Prev. processes mode).
- **Comes from**: Previous production area (Prev. processes mode).

## Control Station – Purchased Elements

**Path**: `Production > Capacity planning > Control station > Purchased elements tab`

_Fig. H-220 Control station - Purchased elements_

On this tab, you check which orders (purchased articles) are included in the items.

### Overview
The following data is displayed in the overview:
- **Order, item**: Order and item number from the order.
- **Element**: Number of the BOM level.
- **(Blank column)**: Series, currently not used.
- **Article/processing**: Product name of the purchased element.
- **Quantity**: Quantity that must be purchased.
- **Size**: Dimensions of the item.
- **Ordered to**: Delivery date requested by the supplier.
- **Deliv.**: Quantity delivered.
- **Shift**: Shift in which the item is required.

## Control Station (Machine)

**Path**: `Production > Capacity planning > Control station > Machines tab > Double-click on row header`

On this dialog, you check the machine utilization per shift.
The Control station (machine) dialog contains the following tabs:
- "Control Station (Machine) – Shift" on page H-346
- "Control Station (Machine) – Load" on page H-348
- "Control Station (Machine) – Move II" on page H-350
⇨Tutorial, "Control Station – Machine" on page H-165

### Functions Menu
**Path**: `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Functions menu`

Using this menu, you can open other dialogs without closing the control station.

#### Fill shift group
- **Backwards**: Recalculates the shifts. The quantities are moved to one of the previous shifts if possible.
- **Forwards**: Recalculate the shifts. The quantities are moved to one of the next shifts if possible.

#### Compress group
You can have the machine utilization recalculated. This way you can fill gaps which occurred due to the settings regarding the proportional utilisation when an item was split or if e.g. an order was cancelled so that there is more free capacity.
- **Backwards**: Recalculates the utilization, starting backwards from the displayed date.
- **Forwards**: Recalculates the utilization, starting forward from the displayed date.
⇨ "Fill shift in case of item splitting" on page H-180
⇨ "Split Items" on page H-284

#### Graphic group
- **Graphic**: Opens a graphical daily overview of the production area. ⇨ "Graphic" on page H-295

### Options Menu
**Path**: `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Functions menu`

Using this menu, you can determine the default setting of the dialog. You can activate or deactivate options. The settings will not be reset when you close the dialog. The description of the following entries reflects the activated state:
- **Move setup time**: Enables the possibility to move the set-up times.
- **Suppress messages**: Errors that occur during rescheduling for another date or another machine are displayed in a message. You can suppress these messages.

## Control Station (Machine) – Shift

**Path**: `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Move I`

_Fig. H-221 Control station (machine) – Shift_

On this tab, you check which orders and quantities have to be produced per shift by this machine.

### Navigation through the tabs
- Double-click on order number -> Control station (order)

### Overview
The quantities for the selected machine are displayed in the overview.
- **Date**: Production date.
- **Shift**: Shift in which the orders are produced.
- **Order**: Order number.
- **Pcs.**: Pieces of the order on the current machine.
- **Finished**: Quantity of glass produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Time scheduled for the quantity.

### Move
- **New date**: Production date to which the order shall be moved.
- **Shift**: Shift to which the order shall be moved.
- **Machine**: Machine to which the order shall be moved.
- **[Load]**: Checks the utilization of the new machine. The utilisation is shown in hours. It includes the times for the order you have selected by clicking on the row header.
- **[Roll back]**: Sets the move back to the original values.

## Control Station (Machine) – Load

**Path**: `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Load`

_Fig. H-222 Control station (machine) – Load_

On this tab, all items are displayed that shall be produced in the selected period.
⇨Tutorial, "Control Station – Machine" on page H-165

### Selection
- **From date, to date**: Entry of the period to be checked.
- **Machine**: Selection of the machine for which you want to check the utilization.

### Overview
In the overview, all order items are listed that must be produced in the selected period.
- **Date**: Production date.
- **Shift**: Shift in which the item shall be produced.
- **Order, item**: Order and item number stated in the order.
- **Product**: Product name.
- **Glass size**: Size of the item.
- **Element**: Product name of the BOM component.
- **Work type**: Work type in the production area.
- **Pcs**: Number of pieces of the item.
- **Time**: Scheduled time.
- **Customer**: Customer name from the order.

## Control Station (Machine) – Move II

**Path**: `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Move II`

_Fig. H-223 Control station (machine) – Move II_

On this tab, all shifts are displayed in the selected period. Colored fields indicate a scheduling problem.

### Overview
In the overview, all shifts for the selected period are listed.
- **Date**: Production date.
- **Shift**: Shift in which the pieces are produced.
- **Hours**: Time required. If there are scheduling problems, the field is red.

### Move
The fields in this group are described for the Move I tab.
⇨ "Control Station (Machine) – Shift" on page H-346

## Utilisation (Date)

**Path**: `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilisation`

On this dialog, you display an overview of the quantities to be produced for a specified time period. The overview can optionally be output by production areas, machines or machine types.
The data is displayed if you have started the filtering in the Start > Execute menu.
This section provides information on the following subjects:
- "Plant Menu" on page H-352
- "Display Menu" on page H-352
- "Utilisation on (Date) (Display Period)" on page H-353
- "Utilisation on (Date) – Selection" on page H-355
- "Utilisation on (Date) - Details" on page H-356
- "Utilisation - Graphic" on page H-357
- "Utilisation - Print" on page H-358

### Plant Menu
**Path**: `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilisation`

Using this menu, you specify whether the capacity of an individual plant or all plants shall be considered.
- **All**: All defined production areas are displayed.
- **Plant 1**: Only the production areas with entry 0 and 1 are displayed.
- **Plant 2**: Only the production areas with entry 0 and 2 are displayed.
- **Plant 3**: Only the production areas with entry 0 and 3 are displayed.

The plant refers to the code entered in the client's company data. Clients can be allocated in the Production areas dialog.

### Display Menu
**Path**: `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilisation`

Using this menu, you can specify the order status up to which the orders shall be displayed.
⇨ "Display Status" on page H-359

## Utilisation on (Date) (Display Period)

**Path**: `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilisation`

_Fig. H-224 Utilisation on (date) - Select period_

On this dialog, you specify the criteria for the display of the utilization. You can display the result as a graphic or as a list.
⇨ "Utilisation - Graphic" on page H-357
⇨ "Utilisation - Print" on page H-358

### Evaluation period
- **From, to**: Period for which you would like to have an overview.

### Options
**Show turnover**: This checkbox is released only if you have selected the Machine option in the Overview of group.
- The turnover will not be displayed.
- The turnover will be displayed for the selected machine.

### Overview of
With the selection of the option, you filter the display.
- **Production area**: You can limit the overview to a particular production area (<n.e.> = all).
- **Machine types**: You can limit the overview to a particular machine type.
- **Machine**: You can limit the overview to a particular machine. With this option, you can release the Show turnover checkbox.
- **All machines by production area**: With this option, all machines are sorted by production areas.

### Overview
The following data is displayed in the overview:
- **Date, Production areas/machines**: The utilization is displayed per date and production area or machine.
- **Pcs.**: Total quantity.
- **Area**: Total area.
- **Circumference**: Total edge length.
- **Time**: Scheduled time.
- **Costs**: Time costs.
- **Turnover**: Turnover per machine. This column is displayed only if you have selected the Machine option and ticked the Show turnover checkbox.

## Utilisation on (Date) – Selection

**Path**: `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilisation > Display evaluation period > Click in row header`

_Fig. H-225 Utilization on date - Select production area/machine_

On this dialog, you check the utilization in a particular period.

### Evaluation date
- **From, to**: Period for which you would like to have an overview.
- **Only shift**: Specification of the shift whose utilization shall be displayed. The field is only released in selection mode.
- **Shift info**: The checkbox is only released in selection mode.
    - The selection is not limited to particular shifts. After filtering, all shifts are displayed in the overview.
    - The selection is limited to the shift that is specified in the Only shift field.

### Overview
With the selection of the option, you specify the filtering of the display:
- **All machines**: The utilization of all machines in the set period is displayed.
- **Only for production area**: The utilization for a particular production area is displayed. The field for selection of the production area is released.
- **Arrange detailed view**: With the selection of the option, you specify the grouping on the Details tab. The fields are released only if data is displayed.
    - **Order, customer**: The utilization is displayed per order and customer.
    - **Product**: The utilization is displayed per product.

### Utilization
The hit list is displayed in the overview.

## Utilisation on (Date) – Details

**Path**: `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilisation > Display evaluation period > Click in row header > Details tab`

_Fig. H-226 Utilization on date - Details on production area/machine_

On this dialog, you check the details of the utilization.

### Navigation through the tabs
- Click on row header -> Production level orders

### Details
The display of the columns and data is oriented according to the selection criteria. The lists are grouped by the option that is chosen on the Selection tab.
- **Production area**: Display of the production area in which the machines are or where the work will be performed.
- **Number manager**: Selection of the number manager in which the orders displayed shall be placed.
- **[Fill NM]**: Places all displayed orders in the specified number manager.

## Utilisation - Graphic

**Path**: `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilisation > Display evaluation period > Functions menu > Display group > Graphic`

_Fig. H-227 Utilisation on date - Graphic_

The graphical display shows the utilization based on the criteria selected on the Utilisation (date) dialog.
You can print the result from the Utilisation (date) dialog. The period to be printed can be limited to 8 or 12 days.
⇨ "Utilisation - Print" on page H-358

## Utilisation – Print

**Path**: `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilisation > Display evaluation period > Print menu`

_Fig. H-228 Print_

You can print the result shown in the Utilisation at a date dialog. The period to be printed can be limited to 8 or 12 days. With 12 days, make sure to print the list in landscape format.
The display shows a daily overview of the units to be produced per machine and production area. The nominal value is shown as well.

## Display Status

**Path**: `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilisation > Display menu > Status display`

_Fig. H-229 Specify display status_

On this dialog, you limit the display of the orders to a maximum status. Displayed are only the orders whose status is smaller than the status entered.

## Settings for Control Station

**Path**: `Production > Capacity planning > Completion report > Functions menu > Settings`

_Fig. H-230 Settings for the control station_

On this dialog, you specify which data shall be displayed in the Control station dialog. You must confirm the changed settings with [OK]. The Control station dialog must be re-opened so that the data can be reloaded.

### Only these production areas
You can restrict the display to a certain production area or several production areas. If no entry has been selected, all production areas will be displayed.

### Selection criteria
You can set that only the items not produced are displayed:
- **All entries**: With this setting, the produced and open items are displayed.
- **Only show entries which were not reported completed**: With this setting, only items are displayed that still have to be produced.

**Order area**: You can limit the display to a particular order area.

**From status, to status**: You can limit the display by order status. If you select the same status in both fields, only orders with this one status will be displayed.

### Display in addition to times
By default, only the hours available on the day per machine are displayed. You can expand these details to include the following details:
- **Pcs.**: Quantities for all shifts and orders.
- **Sqm**: Total area for all shifts and orders.
- **Linear m**: Total edge length for all shifts and orders.
- **In %**: Percentage utilization for all shifts.
- The information is not displayed.
- The information is displayed on the Machines and Orders tabs.

## Residue Qty.

**Path**: `Production > Capacity planning > Control station > Functions menu > Show residue quantities`

_Fig. H-231 Display residual quantities and report completed_

On this dialog, you check which orders have not yet been reported completed, and to report them as such if required.

**Display from status**: You can limit the display of the open orders to a minimum status, e.g. to exclude orders from the display the production of which has already begun.

### Overview
In the overview, all orders are displayed which have not been produced up to the current date. When you tick the checkbox, the corresponding order will be reported completed for the current date when you have confirmed with [OK].

## Control Station (Order)

**Path**: `Production > Capacity planning > Control station > Functions menu > Select order.`

On this dialog, you check the individual machines that an order runs through from production to shipping to move the scheduling on the "critical" machines.
The Control station (Order) dialog contains the following tabs:
- "Control Station (Order) – Machines” on page H-364
- "Control Station (Order) – Detail" on page H-366
- "Control Station (Order) – Work Types" on page H-368
- "Control Station (Order) – Purchased Elements" on page H-370
- "Control Station (Order) – Move I" on page H-371
- "Control Station (Order) – Move II” on page H-372
- "Control Station (Order) – Load" on page H-374
⇨ Tutorial, "Control Station - Order" on page H-164

### Navigation through the tabs and dialogs

| Tab | Action | Tab / dialog |
|---|---|---|
| Machines | Double-click on machine | -> Move II |
| | Double-click on date | Detail |
| Detail | Click on cell header | -> Work types |

### Functions Menu
**Path**: `Production > Capacity planning > Control station > Functions menu > Select order.`

Using this menu, you can open other dialogs without closing the control station.

#### Document group
- **Show document**: Opens the document view.
- **History**: Opens the History dialog where you can check the process of status changes. ⇨ Sales, "History" on page C-478
- **Status change**: Opens the dialog by the same name on which you can change the order status. ⇨ Sales, "Status Change" on page C-479

#### Graphic group
- **Production area**: Opens the graphical display Production areas/weekly overview to compare the completed and open quantities.
- **Order**: Opens the graphical display Order info/weekly overview to compare the completed and open quantities.
These graphics correspond to the Graphic areas display. ⇨ "Area Graphic" on page H-259

#### Production group
- **Reports list**: Opens the Reports overview dialog to check the current status of production per order item. ⇨ "Report List" on page H-318
- **Scheduling**: Opens the Schedule order dialog to change the scheduling of the current order. ⇨ "Book Order" on page H-275
- **Manual settings**: Opens the Order completion status dialog on which you can check the production status of the order. ⇨ "Production Level Orders" on page H-307

### Options Menu
**Path**: `Production > Capacity planning > Control station > Functions menu > Select order.`

Using this menu, you can determine the default setting of the dialog. You can activate or deactivate options. The settings will not be reset when you close the dialog. The description of the following entries reflects the activated state:
- **Check dwell time**: Before moving, it is checked whether the transition times permit a move. You should select this setting if you know that the transition requires longer transfer times, e.g. for TG production. You should only suppress this check if the transition from one production area to the next one does not require long transition times.
- **Ignore dwell days**: Ignores the dwell day when rescheduling.
- **Postpone setup time**: If this option is activated, the buttons on the Move II tab are locked.
- **Setup time check**: If the set-up time has been defined for several work types performed for an order item, this time shall be charged just once per item.
- **Suppress messages**: Errors that occur during rescheduling for another date or another machine are displayed in a message. You can suppress these messages.

## Control Station (Order) – Machines

**Path**: `Production > Capacity planning > Control station > Functions menu > Machines tab`

_Fig. H-232 Control station (order) – Machines_

On this tab, you check the utilization of the machines which are producing this order. If you have opened the dialog from the control station, the data for the current order is displayed. However, you can use the search mode to display another order or limit the display to a particular position.
If the order was reported completed manually, all previously not reported values are shifted to the day of the completion report. In this case, the production dates are shown in green.

### Order
- **Number, customer**: Number and customer name stated in the order.
- **Only item**: Number of the item to be changed. The field is released in selection mode. You can specify the item number if you want to display one order item only. If you enter a zero (0), all items are displayed.
- **Delivery date**: Delivery date stated in the order. You can change the date and confirm this by [Change]. ⇨Tutorial, "Postpone Scheduling for single Order" on page H-166
- **[Change]**: Confirms the new date.
- **Order area**: Order area from which the order comes.
- **Production of, to**: Display of the period in which the order is produced.

### Overview
In the overview, all machines are displayed on which the order is produced.
**Day of the week, date**: Per weekday, the utilization is displayed with the scheduled and free time (all shifts) per machine.
- Scheduled and free time (all shifts).
- Open and produced quantity of all sheets in pcs.
- Total surface in sqm.
- Edge length of all sheets.
- Utilization in percent.
All details except for the time can be selected or deselected in the control station settings.
⇨ "Settings for Control Station" on page H-359

## Control Station (Order) – Detail

**Path**: `Production > Capacity planning > Control station > Functions menu > Select order > Detail tab`

_Fig. H-233 Control station (order) – Detail_

On this tab, you can move quantities manually or report them completed. The machine to which these details refer is shown above the fields.
If you have moved a whole item, it is removed from the display.

### Overview
The quantities for the current order on the selected machine are displayed in the overview. The following columns are displayed:
- **Shift**: Current shift.
- **Pcs.**: Pieces of the order on the current machine.
- **Finished**: Quantity of glass produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Time scheduled for the quantity displayed.

**[Load / Day]**: Updates the display in the field below.

### Move
- **New date**: Production date to which the order shall be moved.
- **Shift**: Shift to which the order shall be moved.
- **Machine**: Machine to which the order shall be moved. The field is released if you have ticked the Move checkbox and confirmed with [OK].
- **[Load]**: Checks the utilization of the alternative machine. The value is displayed in hours. It includes the times of the order.
- **[Roll back]**: Sets the move back to the original values.

## Control Station (Order) – Work Types

**Path**: `Production > Capacity planning > Control station > Functions menu > Select order > Work types tab`

_Fig. H-234 Control station (order) – Work types_

On this tab, you check which work types are to be performed on a machine on a production date.
If you have moved a whole item to another date, it is removed from the display.

**[All], [None]**: Ticks or unticks all checkboxes in the Move column.

> **Edit setup times**
> Using the context menu (right mouse key) on an item, you can add or delete set-up times. For this, the set-up time must be created as work type with a basic time.

### Overview
The following data is displayed in the overview:
- **Shift**: Shift in which the item shall be produced.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, i.e. the BOM level.
- **SI**: Sub-items resulting from the splitting of items at scheduling.
- **Process**: Work type.
- **Product/Processing**: Product name.
- **Pcs.**: Item quantity.
- **Pcs**: Quantity of sheets produced.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved. These messages can be switched off using the Options menu.
- **Hours**: Time reserved for this item.

> **Move scheduling**
> The fields in the Move group are explained for the Detail tab.
> ⇨ "Control Station (Order) – Detail" on page H-366

## Control Station (Order) – Purchased Elements

**Path**: `Production > Capacity planning > Control station > Functions menu > Select order > Purchased elements tab`

_Fig. H-235 Control station (order) – Purchased elements_

On this tab, you check which purchased articles are required for production.

### Overview
The following data is displayed in the overview:
- **Item**: Item number from the order.
- **Article/processing**: Product name of the purchased element.
- **Quantity**: Quantity that to be purchased.
- **Size**: Dimensions of the item.
- **Ordered to**: Delivery date requested by the supplier.
- **Deliv.**: Quantity delivered.
- **Required on, date, shift**: These three columns display when the purchased elements are required where.

## Control Station (Order) – Move I

**Path**: `Production > Capacity planning > Control station > Functions menu > Select order > Move I tab`

_Fig. H-236 Control station (order) – Move I_

On this tab, you plan and edit the load of the machines with series. This function is not currently used.

### Order
This group displays the order number and name of the customer.

### Postpone for whole days
- **No. of days**: Number of days by which the production of the series shall be postponed.
- **Only from date**: Initial date from which the full days specified above shall be counted.

## Control Station (Order) – Move II

**Path**: `Production > Capacity planning > Control station > Functions menu > Select order > Move II tab`

_Fig. H-237 Control station (order) – Move II_

On this tab, you move the items or orders to other dates, shifts or machines.
If you have moved a whole item, it is deleted from the display.

### Overview
The quantities for the current order for the selected machine are displayed in the overview. The following columns are displayed:
- **Date**: Scheduled production date.
- **Shift**: Current shift.
- **Pcs.**: Pieces of the order on the current machine.
- **Finished**: Quantity of glass produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will indicate that this process cannot be moved.
- **Hours**: Time scheduled for the quantity displayed.

> **Areas locked**
> The Fill shift and Compress areas can be locked in the Options > Move set-up time menu.

### Fill shift
You can recheck the shift times to fill gaps in a shift using suitable quantities from the previous or the next shift.
- **[Backwards]**: Recalculates the shifts. The quantities are moved to an earlier shift if possible.
- **[Forward]**: Recalculates the shifts. The quantities are moved to the next shift if possible.

### Compress
You can recalculate the utilization of the machine. This way you can fill gaps which occurred due to the settings regarding the proportional utilisation when an item was split or if e.g. an order was cancelled so that there is more free capacity.
⇨ "Fill shift in case of item splitting" on page H-180
⇨ "Split Items" on page H-284
- **[Backwards]**: Recalculates the utilization, starting backwards from the displayed date.
- **[Forward]**: Recalculates the utilization, starting forward from the displayed date.

### Move
The fields in the Move group are explained for the Detail tab.
⇨ "Control Station (Order) – Detail" on page H-366

## Control Station (Order) – Load

**Path**: `Production > Capacity planning > Control station > Functions menu > Select order > Load tab`

_Fig. H-238 Control station (order) - Load_

On this tab, you check which order items are to be produced by the machine in addition to the current order items. The order items for which the display has been started are highlighted in green.

### Selection
- **From date, to date**: Period that you want to check.
- **Machine**: Machine for which you want to check the scheduled orders.

### Overview
In the overview, all order items are listed that must be produced in the selected period.
- **Date**: Production date.
- **Shift**: Shift in which the item is produced.
- **Order, item**: Order and item number.
- **Product**: Product name.
- **Glass size**: Size of the item.
- **Element**: Product name of the BOM component.
- **Work type**: Work type in the production area.
- **Pcs**: Number of pieces of the item.
- **Time**: Scheduled time.
- **Customer**: Customer name from the order.

## Moving impossible

**Path**: `Production > Capacity planning > Control station > Move`

_Fig. H-239 Move not possible_

On this dialog, you check why the intended move of an order is impossible. You can suppress the display of this message.

## Section Index
_This section provides an index of topics covered in the A+W Business Pro Capacity Planning documentation._

---

## Index

### A
- **Activity see work type**
- **Allocate**
  - next processing H-240
  - PGR - work type H-236
  - product H-238
  - product class - work type H-237
  - product type - work type H-234
- **Allocation**
  - BOM component H-105
  - combination product class H-247
  - combination product type H-239
  - combined product type, product class H-105
  - implicit, explicit H-102
  - machine H-102
  - overview of the dialogs H-103
  - special work type H-106
  - specifying H-107
  - specifying special allocation H-107
- **Alternative process** H-60, H-223
- **Alternative without BOM** H-223
- **Alternative work type** H-30
  - selection of the machine H-93
  - work types H-191
- **Assigned machines**
  - production areas H-194
  - work types H-191

### B
- **Backward scheduling** H-113
- **Basic time** H-61, H-223
  - creating graduation H-76
  - enter time value H-78
  - work process H-59
- **Batch**
  - report completed H-300
  - setting for manual completion report H-301
- **BOM**
  - allocation H-105
  - production status H-318
- **Bottleneck**
  - resolving H-130
  - selection of the delivery date H-123
- **Breakage**
  - manual report H-150
  - reporting H-140

### C
- **Calculation example**
  - machine hour H-46
  - man hour H-43
- **Calendar**
  - add shift times H-53
  - adjust H-49
  - closing time for shift H-187
  - create for capacity planning H-50
  - for unit, production area H-50
  - machine H-209
  - set up special shift H-54
  - shift times H-212
  - specify shift times H-49
- **Capa see capacity planning**
- **Capacity**
  - bottleneck H-285
  - item split H-288
  - per machine H-201
  - per workday H-41
  - specify utilization H-47
  - work unit H-43
- **Capacity planning**
  - basic ideas H-20
  - calculation example H-113
  - cost centres H-160, H-268
  - default settings in company data H-183
  - interplay of the master data H-20
  - menu overview H-16
  - org. overview H-219
  - possibilities for using H-21
  - production list H-306
  - resolve bottleneck H-130
  - scheduling according to route H-122
  - scheduling order H-123
  - series factor H-195
  - shift filling H-122
  - statistics H-262
  - time calculation H-39
- **Capacity planning module** H-16
- **Capacity problems** H-118
  - item split H-119
- **Change of the production area** H-68
- **Check**
  - specify in machine types H-189
- **Check value see restriction**
- **Checking**
  - fields for restrictions H-88
  - restrictions H-26
- **Closing time for scheduling** H-121
- **Combination product class**
  - time factor H-247
- **Combination product type**
  - allocating (capa) H-239
- **Company data**
  - settings for capacity planning H-99
- **Completion report**
  - catching up on H-154
  - graphic H-299
  - manual H-147
  - navigation through the tabs H-311
  - overview H-296
  - per item H-297
  - piece by piece H-297
  - production batch H-300
  - production date H-296
  - purchased elements H-298
  - report order completed manually H-302
  - reports H-136
  - reports overview H-322
  - residual quantities H-365
  - setting for batch H-301
- **Completion status**
  - order H-311
- **Control station**
  - check prev. processes H-345
  - machine (dialog) H-348
  - machine (tab) H-333
  - navigation through the tabs H-331
  - order (dialog) H-366
  - orders (tab) H-334
  - production areas H-332
  - purchased elements H-347
  - reschedule item H-338
  - reschedule order H-336
  - settings H-363
  - utilization per shift H-344
  - work types H-340
  - working with the control station H-166
- **Control station machine**
  - load H-352
  - utilization H-354
  - utilization of the shifts H-350
  - working with the control station H-169
- **Control station order**
  - machines H-368
  - move H-370, H-376
  - navigation through the tabs H-366
  - purchased elements H-374
  - utilization H-378
  - work types H-372
  - working with the control station H-168
- **Conversion**
  - default time in hours H-61
- **Cost calculation**
  - in order H-163
  - in quotation H-163
- **Cost centres**
  - analysis in capacity planning H-268
  - definition (capa) H-269
  - period for evaluation (capa) H-268
- **Costs**
  - machine H-201
  - per machine H-204
  - per order H-315
- **Create setup time** H-74
- **Cube**
  - default time H-228
  - limit types (capa) H-228

### D
- **Date**
  - calculation example H-113
  - change production date H-325, H-327
  - mode for date search H-276
- **Date calculation**
  - example dwell days H-114
- **Date search mode** H-276
- **Deduction for series** H-75
- **Default time** H-61
  - alternative process H-60
  - basic time H-59
  - change per work time, machine H-229
  - conversion to hours H-61
  - copy H-229
  - cube H-228
  - entering time value H-78
  - format H-61
  - graduated H-225, H-226, H-228
  - individual time per unit H-227
  - matrix H-225
  - priority H-60
  - setup time H-74
  - specifying H-76
  - specifying format H-76
  - time surcharge H-63
  - triangle H-61, H-225
  - type H-59
  - type basic time H-222
  - vector H-226
- **Default times**
  - other surcharges H-222
- **Defaults**
  - times H-57
- **Definition of cost centres (capa)** H-269
- **Delivery date**
  - for bottleneck H-123
  - move for scheduling H-278
  - schedule in capacity planning H-278
  - select manually H-278
- **Detail**
  - control station H-342
  - control station order H-370
- **Display conventions** H-15
- **Dwell days**
  - calculation example H-114
  - calculation example with transition times H-115
  - dwell matrix H-214
  - production area H-200

### E
- **Edge processing**
  - time factor H-243
- **Example**
  - calculation for transition and dwell times H-69
  - calculation of capacities H-113
  - plan time for IG H-64

### F
- **Factor**
  - calculation example for time planning H-67
  - default time H-67
  - series H-75
- **Factor for**
  - combination product class H-247
  - combination product type H-239
  - edge processing H-243
  - next processing H-240
  - next processing+shape H-245
  - PGR H-236
  - product H-238
  - product class H-237
  - shape H-241
  - special time H-75
  - work type H-234
- **Failure**
  - machine H-291
- **Formula**
  - for workflow task for scheduling H-118
- **Forward scheduling** H-113
- **Function enabled** H-13

### G
- **Gas**
  - technical restriction (capa) H-206
- **Graduation** H-61
  - cube for default time H-228
  - matrix for default time H-225
  - triangular shape for time H-61
  - vector for default time H-226
- **Graphic**
  - completion reports H-299
  - utilization H-361
  - weekly overview H-263

### H
- **Hours**
  - per shift H-39

### I
- **Ignore process** H-223
- **Individual time as default time** H-227
- **Item**
  - change production date H-327
  - check dimensions H-190
  - forbid split H-185
  - production status H-316
  - report completed manually H-302
  - schedule manually H-281
  - scheduling in capacity planning H-128
  - shift filling for split H-184
  - splitting H-131
- **Item split** H-288
- **Item splitting**
  - manual scheduling H-130

### L
- **Labor costs**
  - machines H-201
  - per unit H-204
- **Lock**
  - by PGR H-251
  - by product H-254
  - by product class H-252
  - customer-related (capa) H-256
  - production line H-258
- **Lock value see restrictions**
- **Locking**
  - lock formula H-87
  - machine H-94
  - overview of the dialogs H-95
  - shifts H-187

### M
- **Machine** H-25
  - assigned work types H-206
  - calendar H-210
  - changing after scheduling H-175
  - complete, locking temporarily H-96
  - costs per order H-163
  - create H-33
  - default time H-59
  - failure H-291
  - lock H-201
  - lock customer-related H-256
  - lock for PGR H-251
  - lock for product H-254
  - lock for product class H-252
  - lock on production line H-258
  - locking H-94
  - priority H-60
  - selection during scheduling H-89
  - selection for alternative work type H-93
  - selection for manual completion report H-305
  - selection in case of capacity bottleneck H-285
  - selection of work type H-191
  - skip next machine H-255
  - skip process H-259
  - skipping H-94
  - specifying default time H-76
  - specifying restrictions H-36
  - time costs H-158
  - times and costs H-28
- **Machine hour** H-46
- **Machine type** H-25, H-189
  - assigned machines H-194
  - restrictions H-26
- **Machines** H-200
  - calendar H-209
  - check production dimensions H-190
  - check spacer H-190
  - control station order H-368
  - in the production area H-219
  - per machine type H-194
  - per production area H-194
  - per work type H-194
  - priorities H-86
  - technical restriction H-206
  - type H-189
  - utilization control station order H-378
- **Man hour** H-43
- **Manual**
  - report order completed H-302
  - setting for completion report H-305
- **Manual scheduling**
  - order H-281
- **Master data (capa)**
  - calendar H-209
  - Components of capacity planning H-20
  - general H-189
  - machines H-200
  - production area H-199
  - recommended sequence H-23
  - special technical restrictions H-216
  - special times H-230
- **Matrix**
  - default times H-225
- **Menus**
  - capacity planning in the Production module H-18
  - master data for the capacity planning H-16
- **Move**
  - control station order H-376
  - not possible H-379

### N
- **Navigation**
  - control station dialog H-331
  - control station order dialog H-366
  - order completion status dialog H-311
- **Next machine**
  - skip H-255
- **Next processing** H-240, H-245
- **Number manager**
  - schedule in capacity planning H-272

### O
- **Order**
  - change production date H-325
  - completion status H-311
  - delete scheduling H-129
  - report completed manually H-302
  - reporting complete manually H-147
  - rescheduling H-170
  - resolve capacity bottleneck H-130
  - schedule manually H-279
  - scheduling in capacity planning H-123
  - time costs H-163
- **Order item**
  - scheduling individual H-128
  - split H-119
  - splitting H-131
- **Other surcharge**
  - editing graduation H-82
- **Overview**
  - area graphic H-263
  - completion reports H-296
  - current production status H-314
  - display residual quantities H-365
  - production list H-307
  - purchased elements (control station order) H-374
  - scheduled orders H-287
  - utilization on date H-355

### P
- **Personnel costs**
  - per order H-163
- **PGR**
  - allocate (capa) H-236
- **Priority**
  - alternative priority H-86
  - default times H-222
  - distinction from restriction H-88
  - for equivalent machine H-86
  - special priority H-231
- **Process**
  - alternative H-222
  - skip H-259
- **Process see work type**
- **Product**
  - allocating (capa) H-238
- **Product class**
  - allocating H-237
- **Production area** H-199
  - calendar H-210
  - create H-32
  - dwell days H-200, H-214
  - dwell time H-68
  - org. overview H-219
  - transition time H-68
  - transition type H-196
  - units H-199
- **Production areas** H-31
- **Production line** H-258
  - defining H-97
- **Production list**
  - capacity planning H-306
  - print format H-309
  - printing H-145
  - settings H-310
  - sorting H-310
  - production list H-310
- **Production module**
  - Capacity planning H-18
- **Production sequence** H-102
- **Production status**
  - BOM H-318
  - calculation H-315
  - checking H-152
  - items H-316
  - order H-315
  - purchased elements H-319
  - reports overview H-322
- **Production time**
  - change H-324
  - specify H-288
  - specify start date H-281
- **Purchased elements**
  - completion reports H-298
  - control station H-347
  - control station order H-374
  - order (production status) H-319

### Q
- **Quotation**
  - time costs H-163

### R
- **Reports** H-136
  - breakage H-144
  - completion report H-142
  - items H-322
  - production area H-200
  - registration points H-138
  - status assignment H-140
- **Reschedule**
  - control station order H-372, H-376
  - item (control station) H-338
  - not possible H-379
  - order (control station) H-336
- **Rescheduling**
  - item H-342
  - work type H-340
- **Residual quantities**
  - checking H-154
  - previous day H-365
  - report completed H-365
  - setting for transfer H-294
  - status setting H-143
- **Restrictions**
  - activate checks H-189
  - comparison with priorities H-88
  - per machine H-36
  - technical restrictions H-26
  - with lock formula H-87
- **Route**
  - date search H-122

### S
- **Schedule**
  - by number manager H-273
  - by order H-279
  - check result H-284
  - date search H-276
  - item split H-288
  - search for delivery date H-186
  - select machine automatically H-185
- **Schedule calculation**
  - backward scheduling H-113
  - example transition times H-116
  - example transition times + dwell days H-115
  - forward scheduling H-113
- **Schedule manually**
  - check times H-290
  - result H-284
  - select machine H-285
  - split item H-288
- **Scheduling**
  - automatic H-117
  - capacity bottleneck H-285
  - capacity problems H-118
  - changing machine H-175
  - Closing time H-121
  - in capacity planning H-117
  - individual item in capacity planning H-128
  - manual H-117
  - moving order H-170
  - order H-123
  - resolving bottleneck H-130
  - schedule calculation H-113
  - settings for automatic scheduling H-99
  - split item H-131
  - workflow task H-117
- **Sequence**
  - recommendation for master data for capacity planning H-23
- **Sequence of the work processes** H-102
- **Sequencing number** H-191
- **Series**
  - factor for time H-75
- **Series factor** H-195
- **Set up special shift** H-54
- **Settings**
  - automatic scheduling H-99
  - batch H-301
  - control station H-363
  - default settings in company data H-99
  - manual completion report H-305
  - production list H-310
  - reports H-137
- **Shape**
  - allocating H-241
  - technical restrictions H-206
  - time factor H-241
- **Shift**
  - add times H-53
  - closing time H-187
  - filling H-122
  - set up special shift H-54
  - shift change H-40
  - shift transition H-39
  - specify number H-49
  - specify quantity H-184
  - times for shift H-187
  - times in the calendar H-212
  - times per workday H-39
- **Shift change** H-40
- **SI see subitem**
- **Skip**
  - next machine H-255
  - process H-259
- **Sorting** H-310
- **Special allocation** H-240
  - edge processing H-243
  - next processing + shape H-245
  - shape H-241
  - specifying H-107
- **Special priority** H-86, H-231
- **Special times**
  - creating H-80
  - surcharge (capa) H-230
- **Special times (surcharge)** H-62, H-75
- **Splitting**
  - item H-288
  - item split H-119
  - locking of production times H-120
  - manual item splitting H-130
- **Statistics**
  - by order area H-264
  - capacity planning H-262
  - order area short H-267
- **Statistics by order area**
  - long H-264
  - short H-267
- **Status**
  - assignment in capacity planning H-140
  - assignment through report H-141
  - Manual allocation H-141
- **Status report** H-200
- **Stock articles**
  - allocate work type H-248

### T
- **Technical restriction**
  - machines H-206
  - work type H-216
  - work types H-206
- **Time**
  - graduation, limit types H-61
  - reduction H-67
  - reservation for item split H-120
  - value for basic time H-78
- **Time calculation** H-39
- **Time costs** H-158
  - per order H-163, H-315
  - per quotation H-163
- **Time factor**
  - combination product class H-247
  - edge processing H-243
  - next processing H-240
  - next processing+shape H-245
  - series H-75
  - shape H-241
- **Time management see capacity planning**
- **Time planning**
  - basic components H-57
  - calculation example H-67
  - example IG H-64
  - factor, surcharge H-67
- **Time surcharge** H-223
  - calculation example H-67
  - creating special time H-80
  - default time H-59
  - work type H-63
- **Transition time**
  - calculation example H-115
  - calculation example with shifts H-116
  - work type H-196
- **Triangle** H-61
  - default time H-225
- **Type**
  - default time H-59

### U
- **Utilisation**
  - machines (control station) H-333
  - per production area (control station) H-332
- **Utilization**
  - completion reports H-296
  - default settings H-47
  - graphic H-361
  - on date H-357
  - orders (control station) H-334
  - overview for date H-355
  - prev. processes (control station) H-345
  - print overview H-362
  - set status H-363
  - shifts H-344

### V
- **Vector**
  - default times H-226

### W
- **Work centers see production areas**
- **Work process**
  - skipping H-94
- **Work type**
  - allocate stock articles H-248
  - alternative work type H-30
  - assigned machines H-191, H-194
  - control station H-340
  - control station order H-372
  - factor for product type H-234
  - machines H-206
  - processes, activities H-29
  - skipping H-94
  - special for allocation H-106
  - specifying default time H-76, H-78
  - time surcharge H-63
- **Work unit**
  - machine hour H-46
  - man hour H-43
- **Workdays** H-39
  - capacity per production area H-41
