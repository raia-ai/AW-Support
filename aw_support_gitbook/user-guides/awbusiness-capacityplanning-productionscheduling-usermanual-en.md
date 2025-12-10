---
description: "EN-UM-AWBusiness_32"
---


# Software Reference: Scheduling

---
## Order scheduling (dialog)
**Path:** `Production > Capacity planning > Scheduling > Order scheduling`

On this dialog, you schedule an individual order or an individual item of an order manually in the capacity planning.
-> Tutorial, "Scheduling Orders" on page H-2760

### Order information

- **Order**: Entry of the order number.
- **Customer**: Display of the customer name.
- **Shipping date**: Shipping date from the order. You can overwrite the date. The change is written back to the order. If you have ticked the checkbox **Keep delivery date**, you cannot choose another date.
    > **Pushing up production**
    > In order to push up the scheduling of production, you have to change the shipping date first before ticking the checkbox **Keep delivery date**.
- **Shift**: Specification of the shift number in which the order should be produced. The field is enabled via the `Functions menu > Group settings > Select a shift`.
- **Status**: Current order status.
- **Priority**: By default, the orders are scheduled with the priority **Normal**. You can select another priority and use the `Functions menu > Group settings > Apply priority` to write back to the order. Only after that is the new priority considered during scheduling. The following entries are available for selection:
    - **Call**: The order is only produced if the customer calls the items.
    - **Urgent**: The order must be scheduled with top priority.
    - **Normal**: The order is scheduled according to the default settings.
    - **Extra**: This priority means that the order shall be produced from residue (plates) left over from cutting other orders.
    > **Consider order priority**
    > If except for the order priority **Normal** the priority **Urgent** should be considered, then individual values must be defined for the transition times. If these have not yet been set up, scheduling is done with the priority **Normal**.
    > -> "Transition times" on page H-2846
    > -> "Transition matrix" on page H-2863
- **Keep delivery date**: If the utilization of the machines makes the delivery date impossible, it can be postponed.
    - [ ] Order scheduling permits postponing the delivery date.
    - [x] Order scheduling permits postponing the delivery date. With this setting, you will not be able to choose another date in field Shipping date.
- **Earliest production start**: If you have a delivery date that is far in the future, you can specify the earliest date on which the production should be started.
- **Current scheduling**: This area displayed which item is currently being scheduled.
- **Item/processings**: In the overview, the product names and processings of the individual items are displayed.

### Options

- **Schedule individual item**: You can schedule individual items from an order.
    - [x] All items of the order are scheduled.
    - [ ] The field for entry of the item number is enabled. Only this one item is then scheduled.
- **Item number**: Entry of the item that should be scheduled. The field is only enabled if the **Schedule individual item** checkbox is ticked.
- **Also use priority -1**: For the selection of the machine, the priorities of the machines are considered. By default, the availability of the machine with the highest priority is checked. The priority -1 is generally assigned the machines for manual selection, e.g. hand cutting.
    - [ ] Machines with priority -1 can only be scheduled manually.
    - [x] Machines with priority -1 are included in the scheduling process.

## Scheduling result
**Path:** `Production > Capacity planning > Scheduling > Order Scheduling > Functions menu > Current order group > Scheduling result`

On this dialog, you check how the order was scheduled.

| Item | Machine | Work type | Product/Processing | Pcs. | Date | Shift |
| --- | --- | --- | --- | --- | --- | --- |
| 1 | Zuschnitt / Cutting | Zuschnitt / Cutting | Therm 6 mm A+W | 10 | 04.08.2017 | 3 |
| 1 | Rahmenbieger / Spacer bender | Rahmen biegen / Spacer bender | 12 mm ALU spacer A+W | 10 | 07.08.2017 | 1 |
| 1 | ISO Linie / IG Line | ISO-Fertigung/IG-Production | IG 5/12/Th6 A+W | 10 | 07.08.2017 | 1 |
| 1 | Versand / Dispatch | Verpacken / Packing | IG 5/12/Th6 A+W | 10 | 07.08.2017 | 3 |
| 1 | LKW/Truck | Versenden / Shipping | IG 5/12/Th6 A+W | 10 | 08.08.2017 | 1 |
| 2 | Zuschnitt / Cutting | Zuschnitt / Cutting | Therm 6 mm A+W | 10 | 04.08.2017 | 3 |
| 2 | Rahmenbieger / Spacer bender | Rahmen biegen / Spacer bender | 12 mm ALU spacer A+W | 10 | 07.08.2017 | 1 |
| 2 | ISO Linie / IG Line | ISO-Fertigung/IG-Production | IG 5/12/Th6 A+W | 10 | 07.08.2017 | 1 |
| 2 | Versand / Dispatch | Verpacken / Packing | IG 5/12/Th6 A+W | 10 | 07.08.2017 | 3 |
| 2 | LKW/Truck | Versenden / Shipping | IG 5/12/Th6 A+W | 10 | 08.08.2017 | 1 |

### Work processes
In the overview, the items per work type are displayed.
- **Item**: Item number from the order.
- **Machine**: Name of the machine.
- **Work type**: Work type that is performed on the machine.
- **Time**: Time scheduled per item and work type. The totals line shows the total time scheduled for this order.
- **Product/Processing**: Product name.
- **Pcs.**: Number of work steps, that would be e.g. 10 sheets for cutting, but 4 x 10 pieces for rounded corners.
- **Date**: Production date.
- **Shift**: Shift in which the item is scheduled.
- **Costs**: Costs per work type and item. In the total line, the total costs for the order are displayed.

### Sort result
With the selection of the option, you specify how the display should be sorted:
- **By item**: The work types are listed per item.
- **By production date**: The items are listed according to the date of the work type in question.

### Totals
In this area, the totals for the times and costs are displayed, which were calculated for the scheduled order.

## Residue transfer
**Path:** `Production > Capacity planning > Scheduling > Order Scheduling > Functions menu > Group settings > Transfer remaining quantities`

On this dialog, you specify the status up to which the workflow task searches for non-produced residual quantities from the previous day. Considered are only orders and items that should have been produced on the previous day, but were not yet begun.
-> Tutorial, "Remaining Quantities from Previous Day" on page H-2792

**Settings:**
- **Maximum order status**: e.g., `050 - Ready for transfer to PPS`
- **Transfer only complete items**: Checkbox

## Machine selection in case of bottleneck
**Path:** `Production > Capacity planning > Scheduling > Order Scheduling > Scheduling > (bottleneck)`

On this dialog, you select another machine manually. The dialog is displayed automatically during scheduling if the default machine with the priority 9 is fully utilized.
-> Tutorial, "Capacity Problems" on page H-2766

### Capacity bottleneck
- **Order, customer, shipping date**: Display of the order number, the customer name, and the shipping date from the order.
- **Item/element/sub-item**: Display of item number, level of the BOM and for split items the number of the sub-item to which the capacity bottleneck applies.
- **Quantity**: Quantity of the item.
- **Product, dimensions**: Product name and dimensions of the order item
- **Work type**: Work type for which the bottleneck occurs.

### Production
- **Date**: Scheduled production date. With the arrow buttons, you can move the date forward or backward.
- **Shift**: Planned shift. With the arrow buttons, you can move the shift forward or backward on the same day. If you are working with just one shift, the date is shifted.

### Valid machines
In the overview, all machines are displayed on which the work type can also be performed.
- **Machine**: Alternate machines.
- **Time required**: Time required for the process for the item and quantity displayed.
- **Time reserved**: Time reserved for other orders on that machine.
- **Set-up time**: Time required for setting up the machine if the defined items shall be produced.
- **Maximum time**: Shift time of the machine on the selected date.

### Buttons
- **[Overview]**: Opens the **Order numbers** dialog to check which orders are already scheduled on the machine for the current settings. -> "Order numbers" on page H-2924
- **[Alignment]**: Currently not used.
- **[Split item]**: Opens the **Split item** dialog to split the item into packages. -> "Split items" on page H-2925
- **[Criteria]**: Opens the **Change criteria** dialog. -> "Change criteria (schedule search mode)" on page H-2913
- **[Schedule]**: Schedules the item for the set conditions. Depending on the setting, you must schedule each work type per item individually. If all items are scheduled, a message with the changes is displayed.
- **[Schedule previous day]**: Schedules the item for the set conditions on the previous day. For this, you should first select the last shift of the previous day in the **Shift** field.

## Order numbers
**Path:** `Production > Capacity planning > Scheduling > Order scheduling > Schedule machine in case of bottleneck > [Overview]`

On this dialog you check which orders are already scheduled on the machine at the set conditions.

| Order | Customer | Date | Status | Hours | Priority |
| --- | --- | --- | --- | --- | --- |
| 700053 | Maier Fensterbau | 21.03.2014 | 90 | 3.73 | Normal |

## Split items
**Path:** `Production > Capacity planning > Scheduling > Order scheduling > Scheduling > Machine selection in case of bottleneck > [Split items]`

On this dialog, you split an order item into several packages.
-> Tutorial, "Capacity Problems" on page H-2766

### Item information
- **Order, item**: Order number and number and product name for the order item.
- **Product, quantity**: Product number and quantity of the order item.

### Split
In this area, you specify how the item should be split. The splitting of the item into packages is displayed in the overview.
If you have ticked the checkbox **Set production date** in section **Options**, the quantity is displayed as well as the date and the shift. You can enter the desired values directly in these fields.

- **Quantity**: Specification of the quantity. Using the buttons below, you specify whether the quantity should be interpreted as package or quantity.
- **[Reset splitting]**: Resets the splitting of the item. You can also try out other possibilities for splitting the item.
- **[Quantity = packages]**: The value in the **Quantity** field refers to packages, e.g. 2 packages. The quantity of the item is evenly distributed across the number of packages. In the overview, you can overwrite the values.
- **[Quantity = units per package]**: The value in the **Quantity** field refers to the units per package, e.g. 50 units per package.
If you have not made any specifications about the quantity, as many packages are generated as the specifications from the company data permit, e.g. 50% of the shift. In the overview, you can overwrite the values. -> "Fill shift in case of item splitting" on page H-2835

### Options
- **Maximum work type**: This field appears only if the checkbox **Preset production date** has been ticked. It may not be empty. You can specify production dates for the item split. In this case, you can also specify starting with which work type these dates should not apply. This setting makes sense, e.g. because the sub-items are not packaged and shipped separately.
- **Reduced control**: Normally the scheduling checks for each item on which day there are still capacities available to schedule the item there. However, an order may contain items with the same BOM structure, which differ only according to the dimensions.
    - [ ] The entire BOM structure is checked for each item.
    - [x] With the same BOM structure, the scheduling assumes the previous item without checking the BOM. This is the default setting. The program notes the start date of production of the first item, e.g. for the grinding machine. The next item starts precisely on this date in order to check the capacity for this machine and goes, if the machine is fully utilized on this day, to the previous shift or the previous day. The next item, in turn, relies on this new date for the checking of the capacity, etc.
- **With locks**: When splitting, the remaining shift time for other orders can be locked, e.g. so that the machine does not have to be changed over.
    - [x] Remaining time of the shift or the day in question is not locked for other orders.
    - [ ] Only sub-items created by splitting the order will be produced. The remaining time will not be scheduled otherwise.
- **Preset production date**: You can specify a date per package.
    - [x] The date cannot be preset.
    - [ ] In the overview, the columns **Date** and **Shift** are displayed, in the **Options** area the field **Max. work type** for preset date.

- **[OK]**: Applies the data. Scheduling is continued with the new packages.
- **[End]**: Interrupts the splitting. The **Machine selection in case of bottleneck** dialog is displayed again in the foreground.
- **[Overview]**: Opens the **Item times** dialog. -> "Item times" on page H-2926

## Item times
**Path:** `Production > Capacity planning > Scheduling > Order scheduling > Scheduling > Machine selection in case of bottleneck > [Split items] > [Overview]`

On this dialog, you check the times that are required for the current item. The times are displayed in red for which no capacities are available.

| SL | Work type | Hours | Machine |
| --- | --- | --- | --- |
| 0 | Zuschnitt Float BM | 0.0 | Test |
| 0 | Zuschnitt Float LM | 1.0 | Bystronic |

## Machine downtime
**Path:** `Production > Capacity planning > Scheduling > Machine downtime`

Machines can be locked temporarily or completely. The already-scheduled orders must then be rescheduled. The query regarding rescheduling appears when you lock a machine for which orders have already been scheduled. Therefore, you should set the mode in advance.
-> "Change criteria (schedule search mode)" on page H-2913

This section provides information on the following subjects:
- "Functions menu" on page H-2927
- "Options menu" on page H-2928
- "Machine downtime (dialog)" on page H-2929

### Functions menu
**Path:** `Production > Capacity planning > Scheduling > Machine downtime`

Using this menu, you can open other dialogs without closing the **Machine downtime** dialog.
The menu is organized in the following groups:
- "Date search group" on page H-2927
- "Residual quantities group" on page H-2927
- "Scheduling group" on page H-2927
- "Time management group" on page H-2928

#### Date search group
- **Change criteria**: Opens the dialog by the same name on which you can specify the criteria for the date search. -> "Change criteria (schedule search mode)" on page H-2913

#### Residual quantities group
- **Transfer**: Opens the **Residual quantity transfer** dialog on which you can specify up to which status orders should be checked for residual quantities. -> "Residue transfer" on page H-2922

#### Scheduling group
- **Schedule selection**: Opens the **Schedule order** dialog in order to reschedule the marked orders on other machines. -> "Schedule order" on page H-2915

#### Time management group
- **Shifts**: Opens the **Shift settings** dialog on which you can specify the shift transfer and lock times. -> "Shift settings" on page H-2837. You must have administrator rights in order to open the dialog. In addition, a checkmark must be placed in the **Use change of shift table** checkbox. -> "Use change of shifts table" on page H-2837

### Options menu
**Path:** `Production > Capacity planning > Scheduling > Machine downtime`

Using this menu, you can determine the default setting of the dialog. You can activate or deactivate options. The setting is not reset when you close the dialog.
The menu is organized in the following groups:
- "Dwell days group" on page H-2928
- "Set-up time group" on page H-2928
- "Scheduling group" on page H-2928

#### Dwell days group
- **Use old mode**: This setting is only required if you want to retain the old mode for dwell days (= transition matrix)

#### Set-up time group
- **Check**: If the set-up time has been defined for several work types performed for an order item, this time shall be charged just once per item.

#### Scheduling group
- **Item check**: When the order is scheduled, the program checks its share in the daily capacity. The percentage is defined in dialog **Work types**. -> "% Limit" on page H-2844
- **Consider closing time**: The program shall check until when orders can be scheduled for a shift. -> "Shift settings" on page H-2837

### Machine downtime (dialog)
**Path:** `Production > Capacity planning > Scheduling > Machine downtime`

On this dialog, you store downtimes for your machines, so that the capacity planning can consider these during the planning. Such downtimes arise, e.g. due to maintenance work or repairs.
-> Tutorial, "Locks" on page H-2742

#### Selection
- **Machine**: Selection of the machine to which the downtimes should be assigned. The downtimes are only specified in days, not in shifts.
- **Downtime from/to**: Period during which the machine is probably unavailable. If you save the specified times, the affected orders are displayed in the overview. The orders can automatically be rescheduled on other machines. For this, a query is displayed with which you can confirm or decline the shift.

#### Data
In the overview, all machines are listed for which downtimes are entered.

#### Affected orders
In the overview, all orders are listed that are scheduled on the marked machine. Column **Hours** shows the time reserved for the order on the locked machine.

# Production Reports
The current production status can be included in capacity planning so that in addition to the order status, other lists can be drawn up, e.g. production lists and diagrams on the production status.

If you do not use shop floor data collection (barcoding) reports, you can report batches, orders, or order items complete at various points on the shop floor by means of the manual completion report dialogs.

On the dialogs, you can display all orders or only the orders that were not yet reported completed. You can enter completion reports or breakage reports.

The rights to report completed can be limited by the administrator on special dialogs.

This section provides information on the following subjects:
- "Date" on page H-2931
- "Graphic" on page H-2934
- "Batch" on page H-2935
- "Settings for batch completion report" on page H-2935
- "Manual completion report" on page H-2936
- "Settings for manual completion reports" on page H-2939
- "Production lists" on page H-2939
- "Settings for production lists" on page H-2943
- "Production status - order" on page H-2943
- "Scheduling of purchased elements" on page H-2952
- "Report list" on page H-2953
- "Change production times" on page H-2954

## Completion report by date
**Path:** `Select Production > Capacity planning > Completion report > Date`

On this dialog, you report the production of an order, order item or sub-item completed at a certain machine. Once the first element of an item has been reported completed, the corresponding process cannot be changed.
-> Tutorial, "Report manually Order completed" on page H-2796

### Functions menu
Using this menu, you open a graphic display of the orders produced in the production area in question.
-> "Graphic" on page H-2934

### Selection
- **Production date**: Date of production.
- **Batch number**: Number of production batch. The batch number is assigned by the system in ascending order. You cannot change the batch number.
- **Display completed items**: You can display per order which items were reported completed.
    - [ ] Only the items are displayed that are not yet reported completed.
    - [x] All items are displayed.
- **Production area**: You can limit the display to the machines of a particular production area.
    - [x] All production areas are displayed.
    - [ ] Only the machines of the selected production area are displayed. The field for selection of the production area is enabled.

### Overview
In the overview, all machines are displayed that correspond to the selection criteria.

### Details
In this area, the totals reported for the quantities and times are displayed.
- **Completed**: Quantity produced on the current day.
- **Pcs**: Total pieces that are to be produced on this machine on this day.
- **Time**: Time (in hours) that is required or was required in order to produce the total quantity on this machine.
- **Remaining time**: Remaining time for the not yet produced quantities.

### P.O. elements
In the overview, all items are displayed that are produced on the machine on the selected date. You can report an item partially or entirely completed.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, that is the BOM level.
- **Sub item**: Subitems (packages) that arose during scheduling through splitting of the item.
- **Process**: Work type.
- **Product/processing**: Product name.
- **Pcs.**: Item quantity.
- **Size**: Dimensions of the item.
- **Already completed**: Quantity produced on the current day.
- **Completion report**: Entry of the quantity to be reported completed.
- **Fixed**: As soon as the first piece of an item is reported completed, a checkmark is placed in the checkbox. The process can then no longer be changed. If you place a checkmark in the checkbox (manual) although no completion report is present, you force the production of the item on the set date on a particular machine.
- **Batch**: Number of production batch.
- **Production date**: Date of production.

### Purchased parts
In the overview, all order items with purchased parts are displayed.
- **Order, Item**: Order and item number from the order.
- **Part**: If the purchased part is a processing, the component is displayed that should be processed.
- **Article/processing**: Product name of the P.O. element.
- **Pcs**: Quantity of the purchased part.
- **Size**: Dimensions of the item.
- **Ordered for**: Desired delivery date.
- **Quantity delivered**: Quantity already delivered.
- **Required on, shift**: These two columns display when the purchased parts are required where.
- **Batch**: Number of production batch.

## Graphic display of quantities produced
**Path:** `Production > Capacity planning > Completion reports > Date > Functions menu > Graphic`

This display presents the quantities of a production area, a machine or an order item in graphic form.
- **Blue graphic**: Quantities that have not yet been reported completed.
- **Red graphic**: Quantities that have been reported completed.

## Report batch completed
**Path:** `Select Production > Capacity planning > Completion report > Batch`

On this dialog, you report a production batch completed manually if you are not working with the status reports from barcoding.

### Functions menu
Via this menu, you open the **Settings for batch completion report** dialog in order to select the production area for the completion report.
-> "Settings for batch completion report" on page H-2935

### Selection
With the option, you specify the selection of the orders for the completion report:
- **By batch number from, to**: An entire batch is reported completed. With the selection of this option, the fields **from** and **to** are enabled, where you can enter a batch number of a range of batch numbers. The batch numbers are assigned in A+W Production.
- **By number manager**: The orders of a whole number manager are reported completed. With the selection of this option, the field for selecting the number manager is enabled.

- **Enter date**: By default, the current date is taken over for the completion report.
    - [x] The current date is taken over for the completion report.
    - [ ] The field for the specification of the date is enabled. The batch is reported completed with the changed date.

### Production areas / machines
In this field, the production areas or machines are displayed for which the batch is reported completed. The desired areas or machines are selected using the **Selection** menu on the **Settings for batch completion report** dialog.
-> "Settings for batch completion report" on page H-2935

### Table
In the overview, all orders are listed that correspond to the criteria in the Selection area.

## Settings for batch completion report
**Path:** `Select Production > Capacity planning > Completion report > Batch > Functions menu > Production areas / machines`

On this dialog, you specify for which production area or which machines the batch is reported completed.

### Completion report
With the selection of the option, you specify for what the completion report applies:
- **Whole order**: With this option, all items and thus the entire order is reported completed. For the completion report, the current date or the specified date is taken over.
- **Selected production areas**: With this option, the production areas are listed in the **Selection** field. You can select one or more entries. The selected production areas are displayed on the **Batch** dialog. The batch numbers can be reported completed for the selected production areas.
- **Selected machines**: With this option, the machines are listed in the **Selection** field. You can select one or more entries. The selected machines are displayed on the **Batch** dialog. The batch numbers can be reported complete for the selected machines.

## Manual completion report
**Path:** `Select Production > Capacity planning > Completion report > Manually`

With this dialog, you can report individual orders or order items complete.
This section provides information on the following subjects:
- "Functions menu" on page H-2936
- "Options menu" on page H-2937
- "Manually (completion report)" on page H-2937

### Functions menu
**Path:** `Select Production > Capacity planning > Completion report > Manually`

With this menu, you can open the dialog for the settings to limit completion reports to particular production areas.
-> "Settings for manual completion reports" on page H-2939

### Options menu
**Path:** `Select Production > Capacity planning > Completion report > Manually`

Using this menu, you can determine the default setting of the dialog. You can activate or deactivate options. The setting is not reset when you close the dialog. The following entries are displayed:
- **Scan**: Enables the field for recording the barcode (next to the order number).
- **Adjust prod. date**: By default, the date of the completion report is entered as production date. You can specify another date, e.g. from the previous day.

### Manually (completion report)
**Path:** `Select Production > Capacity planning > Completion report > Manually`

On this dialog, you report orders partially or entirely completed. In addition to the completion reports, you can also record breakage reports. The dialog can be used by employees in production. Completion reports can be set there so that the users can issue completion reports only for their own production area and certain machines.
-> Tutorial, "Report manually Order completed" on page H-2796

#### Completion report
- **Order**: You can enter the order number or record via scanner. The field for the barcode is enabled with the **Options** menu.
- **From item, to item**: You can report an individual item or several items of an order. If you enter several items, you can only report the complete items.
- **Total qty.**: Display of the total quantity of processings for the items you have entered.
    **Example**
    | | Cutting | Dispatch |
    | :--- | :--- | :--- |
    | Item 1: 12 x ISO | 24 pcs | 12 pcs |
    | Item 2: 6 x single annealed | 6 pcs | 6 pcs |
    | **Item 1-2:** | **30 pcs** | **18 pcs** |
- **Quantity**: Quantity to be reported. This field is accessible only if you have entered a single item number, e.g. 2.
- **Item complete**: Scanning will report one unit completed for every scanned order item.
    - [ ] Every item will be scanned until the required quantity is reached.
    - [x] The scanned item is reported completed.
- **With quantity**: You can also report a partial quantity of the scanned item completed.
    - [ ] One piece is reported completed for the scanned item.
    - [x] The quantity entered in field **Qty.** will be reported completed for the scanned item.

- **[Report items completed (F9)]**: Only the selected items are reported completed.
- **[Report order completed (F12)]**: The entire order is reported completed.

#### Preset date
- **Enter date**: By default, the current date is taken over for the completion report. You can change the date.
    - [x] The current date is taken over for the completion report.
    - [ ] The fields for the date and the shift are enabled.
- **Shift**: This field is accessible only if checkbox **Enter date** is ticked. You can then enter the shift for which the report applies.

#### Report type
With the selection of the option, you specify the type of report:
- **Completion report**: The specified quantities are reported completed.
- **Breakage report - entry**: The specified quantities are reported as broken at the machine entry. They must be produced again on the previous machine.
- **Breakage report - exit**: The specified quantities are reported as broken at the machine exit. They must be produced again on the same machine.

> **Breakage report**
> A breakage report can be entered only if the item has been reported completed before. This means that a sheet which is damaged at the station where it has been processed can be reported broken only after the completion report has been issued. A sheet that is already damaged when it arrives at a station, has already been reported completed by the previous station and can therefore be reported broken right away.

- **Select machine**: In this field, the machines are displayed that are available in the selected production area. You must mark one of the suggested machines so that you can enter the report. The program will offer only the machines that are eligible for the current user. -> "Settings for manual completion reports" on page H-2939

## Settings for manual completion reports
**Path:** `Production > Capacity planning > Completion report > Manually > Functions menu > Settings`

On this dialog, you specify for which production area and which machines the production employee can record reports.

### Select machines
- **Production area**: Selection of the production area in which the respective employee should record reports. The program then lists all machines belonging to the selected production area. You can choose only one production area at a time but you can choose as many of the listed machines as you like. You have to select at least one entry.
- **Scanner Separator**: Specification of the separator with which the barcodes are separated if several codes are scanned one after another. This specification must match the scanner setting. Please refer to the scanner's operating instructions for details.

## Production lists
**Path:** `Production > Capacity planning > Production lists`

On this dialog, you can evaluate which quantity of which order must be produced on a particular machine and when the order is required on which subsequent machine.

### Options menu
With this menu, you can specify the sorting of the data for printing.
-> "Settings for production lists" on page H-2943

### Selection
- **From date, to date**: Entry of the date or the time range for which you require the production papers.
- **Machine**: Selection of the machine for which the production papers shall be printed. For selection, only the machines are offered for which processes are scheduled on the day set or in the time selected.

### Print settings
The checkboxes in this area are only enabled in selection mode.
- **Reprint**: You can print the production papers several times on a day and specify whether each time only the new or all data shall be printed.
    - [x] By default, only the new data is printed that was not yet printed.
    - [ ] All data for that day - up to the present point in time - will be printed.
- **Print for all machines**: You can specify whether the production papers for a single machine or for all machines shall be printed.
    - [x] The data is only printed for the machine specified in the **Machine** field.
    - [ ] The data is printed for all machines.
- **Incl. information on origin**: You can also print the production area from which the item came. The checkbox is blocked if the output on the production papers is summarized by orders or items.
    - [x] The previous production area is not displayed.
    - [ ] The previous production area is displayed.
- **Orders summarized**: You can summarize the data by orders.
    - [x] The orders are printed individually.
    - [ ] The data is summarized per order. The checkbox for the items is automatically ticked and cannot be deactivated. With this setting, no origin information can be printed.
- **Items summarized**: You can summarize the data by order.
    - [x] For each order item, one line per machine is printed.
    - [ ] The items of an order are summarized and output on one line. With this setting, no origin information can be printed.
- **Show set-up times as well**: Set-up times can be displayed only if they have been defined as basic times and allocated appropriately.
    - [x] Set-up times are not listed.
    - [ ] Set-up time is listed.

### Table
In the overview, all data is displayed that corresponds to the selection criteria. Depending on the settings in the **Print settings** area, the following columns are displayed:
- **Date**: Production date.
- **Shift**: Shift in which the order or item was produced.
- **Order**: Order number
- **Priority**: Priority from the order or from the scheduling.
- **Status**: Order status.
- **Item**: Number of the order item.
- **Item status**: Item status.
- **Product**: Product name.
- **Glass size**: Size of the item.
- **Shape**: Shape number.
- **Element**: Product name of the BOM component.
- **Processing**: Product name of the processing.
- **Work type**: Name of the work type
- **Pcs**: Number of pieces of the item.
- **Quantity**: Number of sheets.
- **Sqm/pc**: Area per piece.
- **Lm/pc**: Linear meters of the edges per piece.
- **Next processing**: Next processing (process).
- **Next machine**: Machine.
- **Date 2**: Production date on the current machine.
- **Customer**: Customer name from the order.
- **BOM part**: Number of the BOM component.
- **Previous machine, previous work type, production date**: Data for the previous process.

### Production lists – printing
**Path:** `Production > Capacity planning > Production lists > Print menu > Printer`

In the printed lists, the order items are displayed with size, quantities, and next processings. The output is set via the checkboxes on the **Production lists** dialog.
-> "Print settings" on page H-2939

## Settings for production lists
**Path:** `Production > Capacity planning > Production lists > Options menu > Production lists`

On this dialog, you select the criteria for sorting the production list.

### Production list
- **PRLIST Variable (0,1,2)**: The PRLIST variable setting depends on the report definition. By default, the following settings are available for printing the report:
    - **0**: If the product texts of main product and BOM product are identical, then the text is only printed for item 1.
    - **1**: If the product texts of main product and BOM product are identical, then the text is only printed for item 2.
    - **2**: Both texts, both the text for the main product and the text for the BOM product are printed on the list.

    **Example**
    | No. | Text item 1 (if Text main = Float 4 mm, Text BOM = Float 4 mm) | Text item 2 (if Text main = Float 4 mm, Text BOM = Float 4 mm) | Text item 1 (if Text main = IG, Text BOM = Float 4 mm) | Text item 2 (if Text main = IG, Text BOM = Float 4 mm) |
    | --- | --- | --- | --- | --- |
    | 0 | Float 4 mm | - | IG | Float 4 mm |
    | 1 | - | Float 4 mm | IG | Float 4 mm |
    | 2 | Float 4 mm | Float 4 mm | IG | Float 4 mm |

### Sorting by
With the selection of the option, you specify how the data shall be sorted on the production papers.

### Status
- **From, to**: Status or status area of orders to be printed.

## Production status - order
**Path:** `Production > Capacity planning > Production status - Order`

On this dialog, you can check and report complete individual machines, orders, and order items up to BOM level.
-> "Scheduling of purchased elements" on page H-2952
-> Tutorial, "Check Production Status" on page H-2801

There are the following tabs on the **Order** dialog:
- "Production status - order – selection" on page H-2946
- "Production status - order – overview" on page H-2948
- "Production status - order - items" on page H-2948
- "Production status - order - detail" on page H-2949
- "Production status - order - P.O. elements" on page H-2951

### Navigation through the tabs and dialogs
The following overview shows you how to display the data.

| Tab | Action | Tab / dialog |
| --- | --- | --- |
| Selection | Click on row header | -> Items |
| Items | Click on row header | -> Detail, Purchased part |
| Detail | Click on row header | -> Production status order |

### Functions menu
**Path:** `Production > Capacity planning > Production status order > Functions menu`

Using this menu, you can open other dialogs without closing the **Completion report order** dialog.
The menu is organized in the following groups:
- Document group
- Reports group
- Time management group
- Scheduling group
- Status group
- Miscellaneous group

#### Document group
- **Display**: Opens the view of the document.
- **History**: Opens the **History** dialog on which you can check the course of the status conversions. -> Sales, "History" on page C-1662
- **Status change**: Opens the dialog by the same name on which you can convert the status of the order. -> Sales, "Status change" on page C-1664

#### Reports group
- **Overview**: Opens the **Reports** dialog to check the status of the individual items. -> "Report list" on page H-2953

#### Time management group
- **Completion report by date**: Opens the **Date** dialog to report the order completed. -> "Date" on page H-2931
- **Move**: Opens the **Change production time** dialog to move the order. -> "Change production times" on page H-2954

#### Scheduling group
- **Scheduling**: Opens the **Schedule order** dialog to schedule the order. -> "Schedule order" on page H-2915
- **Delete**: Deletes the selected order from the capacity planning. After that, the order can be rescheduled. The right to delete can be limited via the rights management.

#### Status group
- **Show graphics**: Opens the graphic display of the completed and open work per item. The entry is only enabled on the **Items** tab. -> "Graphic" on page H-2934

#### Miscellaneous group
- **Update purchase prices**: Updates the purchase prices of the selected order. -> "Report list" on page H-2953
- **LG numbers**: This entry is only enabled customer-specifically.

### Production status - order – selection tab
**Path:** `Production > Capacity planning > Production status - order > Selection tab`

On this tab you select an order via the customer number or several orders via the delivery date. The orders found are listed in the **Table** area. In the following areas, you set the selection criteria.

#### Order
- **Nummer (number)**: Enter the order number to display the details on this order.

#### Customer
- **Nummer (number)**: Enter the customer number to view all orders of this customer.
- **Name**: The customer name is displayed automatically.

#### Date
- **Delivery date**: Enter the delivery date to view all orders for this date.

#### Completion report
- **Enter date**: If you want to report an order completed, you can specify the date.
    - [x] The current date is entered as completion report date.
    - [ ] You can change the date. The order is reported completed with the changed date.
- **Production date**: Display of the production date for the order that is marked on the overview.

#### Result
In the overview, all orders are displayed that correspond to the selection criteria.

### Production status - order – overview tab
**Path:** `Production > Capacity planning > Production status - order > Overview tab`

On this tab, you can view details on the calculation of the selected order.

#### Production
- **Start, End**: Display of the respective dates for the order that is marked on the **Selection** tab.

#### Quantity
- **Qty.**: Total quantity of the order.
- **Completed**: Quantity completed.

#### Calculations
- **Material costs**: Material cost from the order.
- **Planned time costs**: Calculated time costs.
- **Total costs planned**: Total of material cost and planned time costs.
- **Order value**: Total order value.
- **Actual time costs**: Actual time costs. This value is calculated based on the report from A+W Production.
- **Actual total costs**: Total of material cost and actual time costs.

### Production status - order – items tab
**Path:** `Production > Capacity planning > Production status - order > Items tab`

On this tab, all items of a selected order are listed. You can report individual items completed manually. The fields are described on the **Selection** tab.
-> "Production status - order - selection" on page H-2946

#### Table
In the overview, all items per order are displayed.
- **Item**: Items of the selected order.
- **Article**: Name of the article that is included in this item.
- **Date**: Production date of the first process on the main product of the item.
- **Pcs.**: Item quantity.
- **Size**: Size of the item.
- **Completed w/o processing**: Display of the quantity for which the cutting has already been done, but not yet the processing, e.g. drilling. However, this statement is very imprecise since the glass is generally subjected to a multitude of processings. A precise statement about the state of production can therefore only be made via the reports from registration points in production. -> "Report list" on page H-2953
- **Completely finished**: Number of completely finished units of an item.
- **Ordered**: Display whether there are ordered articles.
- **Completion report**: Display whether the item was reported completed.

### Production status - order – detail tab
**Path:** `Production > Capacity planning > Production status - order > Detail tab`

On this tab, the BOM components are displayed per item. The tab is only enabled if you have selected an order item with BOM on the **Items** tab.
With a click of the header row, you open the **Completion report > Date** dialog.
-> "Date" on page H-2931

#### Table
In the overview, all BOM components of the current item are displayed.
- **Date**: Production date.
- **Shift**: Shift in which the item shall be produced.
- **BOM ID**: BOM ident number, that is the BOM level.
- **Product**: Product name.
- **Work type**: Work type.
- **Pcs.**: Item quantity.
- **Completed**: Quantity that was reported completed.
- **Machine**: Machine on which the item is or was produced.

### Production status - order – P.O. elements tab
**Path:** `Production > Capacity planning > Production status - order > P.O. elements tab`

On this tab the P.O. elements are displayed that are included in the items of the current order.
With a click of the header row, you open the **Schedule P.O. elements** dialog.
-> "Scheduling of purchased elements" on page H-2952

#### Table
In the overview, all items are listed that contain P.O. elements.
- **Item**: Item number from the order.
- **Article**: Product name of the purchased element.
- **Pcs**: Quantity to be purchased.
- **Size**: Dimensions of the item.
- **Ordered for**: Desired delivery date.
- **Quantity delivered**: Quantity already delivered.
- **Required on, date, shift**: These three columns display when the purchased parts are required where.

### Production status – graphic
**Path:** `Production > Capacity planning > Production status - order > Items tab > Functions menu > Status group > Show graphics`

This display shows you the quantities of an order in graphic form.

### Scheduling of purchased elements
**Path:** `Production > Capacity planning > Production status - order > P.O. elements tab > Click in row header`

On this dialog, you schedule the purchased elements after the receipt of goods.

### Report list
**Path:** `Production > Capacity planning > Production status - order > Functions menu > Reports group > Overview`

On this dialog, you check which positions were reported completed on which machines.

#### Order information
- **Order**: Number of the order.
- **Address**: Name and address of the customer.
- **Status**: Status of the order.
- **Production**: Start and end date of production.

#### Order information (Item Details)
For every order item there is a column showing the current reports. The reported figures are displayed in different colors:
- **Black**: 0 indicates that no pieces of the item have been produced.
- **Green**: the reported quantity corresponds to the item quantity.
- **Blue**: the reported quantity is only a partial quantity of the item.
- **Red**: the reported quantity must be ordered again, e.g. due to breakage.

#### Item overview
In this area, the BOM structure is displayed if you double-click in the **Order information** area on the column of an item.

## Change production times
**Path:** `Production > Capacity planning > Production status - order > Functions menu > Capacity planning group > Move`

You can change the dates and machines that were planned for an order. Here the capacities are not considered, however, so that you can move the process of an order item to a machine that is already fully utilized.

This dialog contains the following tabs:
- "Change production times – selection" on page H-2955
- "Change production times – overview" on page H-2955
- "Change production times – overview 2" on page H-2957

### Plant menu
**Path:** `Production > Capacity planning > Production status - order > Functions menu > Capacity planning group > Move > Change production times > Plant menu`

With this menu you specify whether the capacity of an individual plant or all plants shall be considered.
- **All**: All defined production areas are displayed.
- **Plant 1**: Only the production areas with entry 0 and 1 are displayed.
- **Plant 2**: Only the production areas with entry 0 and 2 are displayed.
- **Plant 3**: Only the production areas with entry 0 and 3 are displayed.

The plant refers to the key that is entered in the company data for a site. The sites are then assigned on the **Production areas** dialog.

### Change production times – selection tab
**Path:** `Production > Capacity planning > Production status - order > Functions menu > Capacity planning group > Move > Selection tab`

On this tab, the machines for a selected date are displayed.

#### Selection
- **Production date**: Selection of the date on which the order shall be produced.

#### Machines by product area
The following data is displayed in the overview:
- **Production areas/Machines**: All machines of the production area for which orders have been scheduled for the production date.
- **Pcs.**: Quantity to be produced by the corresponding machine.
- **Hours**: Utilization of the machine in hours.
- **Setup time**: Set-up times can be scheduled in addition to the hours. Set-up times will be displayed only if they are allocated to the machine in question.

### Change production times – overview tab
**Path:** `Production > Capacity planning > Production status - order > Functions menu > Capacity planning group > Move > Overview tab`

On this tab, all orders/items are displayed that shall be produced on the current machine on the production date. You can change the date, the shift, and the machine for an item or for an entire order.

#### Order overview by machine
- **Machine**: Current machine. In selection mode, any machine can be selected.
- **Suppress messages**: Errors that occur during rescheduling for another date or another machine are displayed in a message.
    - [ ] The message is displayed.
    - [x] Messages are not displayed.

#### List
In the overview, all orders are listed that shall be produced on the machine on the current day.
- **Delivery date, Number, Customer**: Delivery date, order number, and customer name from the order.
- **Shift**: Shift in which the order in question shall be produced.
- **Pcs.**: Quantity to be produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. The entire order shall be moved. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Time scheduled for the order.

#### Parts allocation
In the overview, all items of the marked order are listed that should be produced on the machine on the current day.
- **Shift**: Shift in which the item shall be produced.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, that is the BOM level.
- **SI**: Sub-items resulting from the splitting of items at scheduling.
- **Process**: Work type for the BOM item.
- **Product/Processing**: Product name.
- **Pcs.**: Item quantity.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Hours planned for the order.

#### Changed
The changes in these fields apply to the order or the item, based on the selection in column **Move**.
- **New date**: Production date to which the order shall be moved.
- **Shift**: Shift to which the order shall be moved.
- **New machine**: Selection of an alternative machine.

### Change production times – overview 2 tab
**Path:** `Production > Capacity planning > Production status order > Functions menu > Capacity planning group > Move > Overview 2 tab`

On this tab, detailed information per shift and machine is displayed.

#### Work type overview by machine
- **Machine**: Current machine. In selection mode, any machine can be selected.

#### List
In the overview, all work types are listed that are scheduled on the machine on the current day.
- **Number**: ID of the work type.
- **Process**: Work type on the machine.
- **Shift**: Shift in which the work in question shall be performed.
- **Quantity**: Quantity to be produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. The entire process will be moved. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Utilization of the machine in hours.
- **Setup time**: Set-up times can be scheduled in addition to the hours. Set-up times will be displayed only if they are allocated to the machine in question.

#### Order overview by work type/shift
In the overview, all orders with the same work type per shift are listed:
- **Order, Customer**: Order number and customer name from the order.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, that is the BOM level.
- **Sub item**: Sub-items (packages) created by splitting the item at scheduling.
- **Product/Processing**: Product name.
- **Quantity**: Quantity to be produced.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. The entire order will be moved. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Hours planned for the item.

#### Changed
The fields in the **Changed** group are described for the **Overview** tab.
-> "Change production times – overview" on page H-2955

# Control Station
**Path:** `Production > Capacity planning > Control station`

On this dialog you can check and correct the entire scheduling.
-> Tutorial, "Control Station" on page H-2814

This section provides information on the following subjects:
- "Control station (dialog)" on page H-2960
- "Control station (machine)" on page H-2975
- "Utilization (date)" on page H-2981
- "Display status" on page H-2985
- "Settings for control Station" on page H-2986
- "Residue qty.” on page H-2987
- "Control station (order)" on page H-2988
- "Moving impossible" on page H-2999

## Functions menu
**Path:** `Production > Capacity planning > Control station`

Using this menu, you can open other dialogs without closing the control station. The menu is organized in the following groups:
- Additional displays group
- Display group
- Settings group

### Additional displays group
- **Select order**: Opens the **Control station (order)** dialog on which you can edit the scheduling of the order. -> "Control station (order)" on page H-2988
- **Display residual quantities**: Opens the **Residual quantities** dialog to report these completed. -> "Residue qty." on page H-2987

### Display group
- **Graphic**: Opens a graphic display to compare the produced and remaining quantities. -> "Graphic" on page H-2934
- **Utilization**: Opens the **Utilization on date** dialog. The entry is only enabled on the **Machines** and **Orders** tab. -> "Utilization (date)" on page H-2981

### Settings group
- **Settings**: Opens the **Settings for control station** dialog where you can define the data to be displayed by the control station. -> "Settings for control Station" on page H-2986
- **No messages**: After scheduling, a message is displayed with various information about the scheduling. The entry is only released if you are logged in with administrator rights.

## Control station (dialog)
**Path:** `Production > Capacity planning > Control station`

On this dialog, you check the utilization of the machines. Various tabs allow the manual rescheduling of entire orders, or of individual items.
-> Tutorial, "Concept of the Control Station" on page H-2815

The **Control station** dialog contains the following tabs:
- Control station - areas
- Control station – machines
- Control station – orders
- Control station - reschedule order
- Control station - reschedule item
- Control station – work types
- Control station – details
- Control station – shifts
- Control station – prev. processes
- Control station - purchased elements

### Navigation through the tabs and dialogs
The following overview shows you how to display the data.

| Tab | Action | Tab / dialog |
| --- | --- | --- |
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

### Control station - areas tab
**Path:** `Production > Capacity planning > Control station > Areas tab`

On this tab, you check the utilization of the production areas.

#### Navigation through the tabs
- Double-click on row header -> Machines
- Double-click on production area -> Machines (only machines in the area)
- Buttons for navigation -> Page forward and back day by day

#### Overview
- **Production area**: Production areas that are used in the period displayed.
- **Day of the week, Date**: The planned day per day of the week (all shifts) is displayed.

### Control station – machines tab
**Path:** `Production > Capacity planning > Control station > Machines tab`

On this tab, you check the utilization of per machine.

#### Navigation through the tabs and dialogs
- Double-click on machine -> Orders
- Double-click on details -> Reschedule order
- Double-click on row header -> Control station (machine) dialog

#### Overview
- **Machine**: Machines of the production area. If you have changed to the **Machines** tab from the **Areas** tab with a double-click, only the machines are displayed that belong to the appropriate production area.
- **Day of the week, Date**: The utilization with the following totals of all shifts per machine can be displayed per day of the week:
    - Scheduled and free time (all shifts)
    - Open and produced quantity of all sheets in pcs.
    - Total surface in sqm
    - Edge length of all sheets
    - Utilization in percent
    All details except for the time can be selected or deselected in the settings for the control station. -> "Settings for control Station" on page H-2986

### Control station – orders tab
**Path:** `Production > Capacity planning > Control station > Orders tab`

On this tab, you check the utilization of the machines per order.

#### Navigation through the tabs and dialogs
- Double-click on number -> Control station (order) dialog
- Double-click on quantity -> Reschedule item

#### Overview
- **Order, Status, Customer**: Order number, status, and name of the customer from the order.
- **Day of the week, Date**: The utilization with the following details per day of the week is displayed:
    - Scheduled and free time (all shifts)
    - Open and produced quantity of all sheets in pcs.
    - Total surface in sqm
    - Edge length of all sheets
    - Share in the utilization, e.g. 29% means that this order has a share 29% in the available 100% utilization.

### Control station – reschedule order tab
**Path:** `Production > Capacity planning > Control station > Machines tab > Double-click on machine > Reschedule order tab`

On this tab, you move an order on the machine in question, e.g. to another date, another shift or another machine.

#### Navigation through the tabs
- Click on row header -> Reschedule item
- Click on [Elements] -> Prev. processes - elements
- Click on [Prev. processes] -> Prev. processes
- **[Elements]**: Changes to the display of the items on the **Prev. processes** tab.
- **[Prev. processes]**: Changes to the display of previous processes on the **Prev. processes** tab.

#### Overview
- **Delivery date**: Delivery date from the order.
- **Order, Status, Customer**: Order number, status, and name of the customer stated in the order.
- **Shift**: Currently scheduled shift.
- **Pcs.**: Quantity of the sheets or processings.
- **Finished**: Number of sheets produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Time reserved for this order.

#### Move
- **New date**: Production date to which the order shall be moved.
- **Shift**: Shift to which the order shall be moved.
- **Machine**: Machine to which the order shall be moved. The field is enabled if you ticked the **Move** checkbox on the **Start > Execute** menu.
- **[Load]**: Checks the utilization of the new machine. The value is displayed in hours. It includes the times for the order you have selected by clicking the row header.
- **Without check**: You can force the moving of an order or an order item.
    - [x] Before moving, there is a check whether there are sufficient free capacities on the new date, on the new machine, and/or for the new shift. If the capacities are not sufficient, a message indicates that the moving is impossible. You will have to move the order/item elsewhere in that case.
    - [ ] Rescheduling is accepted without a check even if this exceeds the capacity.

### Control station – reschedule item tab
**Path:** `Production > Capacity planning > Control station > Machines tab > Double-click on detail data > Reschedule item tab`

On this tab, you can move an order item to another date, another shift or another machine. The **Process** column displays the work type.
> **Edit set-up times**
> Use the context menu for a process (right mouse-button) to add or delete set-up times.

- **[Product]**: For long lists, you can highlight all entries in the display that contain a particular product. Tick the line that includes the required product. When you click on this button, all lines that include the same product will be selected.
- **[All]**, **[None]**: You can use these buttons to tick or untick all checkboxes in column **Move**.

#### Overview
- **Shift**: Shift in which the item shall be produced.
- **Item**: Item number from the order.
- **Date**: Production date.
- **BOM ID**: BOM ident number, that is the BOM level.
- **SI**: Sub-items (packages) resulting from the splitting of items at scheduling.
- **Process**: Work type.
- **Product/Processing**: Product name.
- **Pcs.**: Item quantity.
- **Finished**: Quantity of sheets produced.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Time reserved for this item.

#### Move
The fields in this area are described for the **Reschedule order** tab.
-> "Control station - reschedule order" on page H-2964

### Control station – work types tab
**Path:** `Production > Capacity planning > Control station > Work types tab`

On this tab you check which work types are to be performed on a machine on a production date. The tab is only filled if you have displayed elements or previous processes.

#### Navigation through the tabs
- Click on row header -> Details
- **[Elements]**: Changes to the display of the items on the **Prev. processes** tab.
- **[Prev. processes]**: Changes to the display of previous processes on the **Prev. processes** tab.

#### Overview
- **Number**: Number of the work type.
- **Process**: Name of the work type.
- **Articles**: Name of the product.
- **Shift**: Shift in which this work type shall be performed.
- **Pcs.**: Item quantity.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Time reserved for this item.

#### Move
The fields in this area are described for the **Reschedule order** tab.
-> "Control station - reschedule order" on page H-2964

### Control station – details tab
**Path:** `Production > Capacity planning > Control station > Prev. processes tab > Click in row header > Details tab`

On this tab, detailed information per shift and work type is displayed.

#### Navigation
- Double-click on order number -> Control station (order) dialog

#### Overview
- **Order, Customer**: Order number and customer name from the order.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, that is the BOM level.
- **SI**: Sub-items (packages) resulting from the splitting of items at scheduling.
- **Product/Processing**: Product name.
- **Pcs.**: Item quantity.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Time reserved for this item.

#### Move
The fields in this area are described for the **Reschedule order** tab.
-> "Control station - reschedule order" on page H-2964

### Control station – shifts tab
**Path:** `Production > Capacity planning > Control station > Shifts tab`

This tab serves to check the machine utilization per shift.

#### Overview
- **Machine**: Machine.
- **Shift**: One line is displayed per shift.
- **Day of the week, date**: Scheduled time and shift time in hours per shift.

### Control station – prev. processes tab
**Path:** `Production > Capacity planning > Control station > Reschedule order tab > [Elements], [Prev. processes] > Prev. processes tab`

This tab allows to check the origin of the items for which data are currently being displayed. You can display the data in the **Elements** and **Prev. processes** modes.

#### Navigation
- Click on row header -> Order column is displayed
- **[In detail]**: Opens the **Production list** dialog to check for which orders the previous machines are utilized. -> "Production lists" on page H-2939
- **[Elements]**: Changes to display of the items.
- **[Prev. processes]**: Changes to display of the previous processes

#### Selection
This area displays the number and area of the elements in total and per shift.

#### Options
In **Prev. processes** mode, you can display additional information.
- **With name**: In the **Elements** column, the product name is displayed.
- **With work type**: In the **Prev. work type** column, the work type is shown that was performed previously.
- **By areas**: If there are several machines available for the previous processes, the display in the **Comes from** column can be switched between production area and machine.
- **With order items**: The order items are also displayed.
- [x] The additional information is not displayed.
- [ ] The additional information is shown in the overview in an additional column. The selection must be confirmed on the **Start > Execute** menu in order to update the display.

#### Overview (elements / previous processes)
- **Work type**: Name of the work type in the production area.
- **Order**: The order number is displayed if you click on the row header.
- **Customer**: The customer name is displayed if you click on the row header in **Elements** mode.
- **Quantity**: Number of sheets in the shift.
- **Sqm**: Total area in the shift (Prev. processes mode).
- **Elements**: Product name (Elements mode).
- **Article no.**: Product number (Elements mode).
- **Comes from**: Previous production area (Prev. processes mode).

### Control station – purchased elements tab
**Path:** `Production > Capacity planning > Control station > Purchased elements tab`

On this tab you check which orders (purchased articles) are included in the items.

#### Overview
- **Order, Item**: Order and item number from the order.
- **Element**: Number of the BOM level.
- **(empty column)**: Series, currently not used.
- **Article/processing**: Product name of the purchased element.
- **Quantity**: Quantity that must be purchased.
- **Size**: Dimensions of the item.
- **Ordered to**: Delivery date requested by the supplier.
- **Deliv.**: Quantity delivered.
- **Shift**: Shift in which the item is required.

## Control station (machine)
**Path:** `Production > Capacity planning > Control station > Machines tab > Double-click on row header`

On this dialog, you check the utilization of the machines per shift.
-> Tutorial, "Control Station – Machine" on page H-2818

The **Control station (machine)** dialog contains the following tabs:
- "Control station (machine) – shift" on page H-2977
- "Control station (machine) – load" on page H-2979
- "Control station (machine) – move II" on page H-2981

### Functions menu
**Path:** `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Functions menu`

Using this menu, you can open other dialogs without closing the control station.
The menu is organized in the following groups:
- Fill shift group
- Compress group
- Graphic group

#### Fill shift group
- **Backwards**: Rechecks the shifts. The quantities are moved to an earlier shift if this is possible.
- **Forwards**: Rechecks the shifts. The quantities are moved to the next shift if this is possible.

#### Compress group
You can fill gaps that occurred due to the settings regarding the percentage utilization when an item was split or if e.g. an order was cancelled so that there is more free capacity.
- **Backwards**: Rechecks the utilization, starting backwards from the displayed date.
- **Forwards**: Rechecks the utilization, starting forward from the displayed date.
-> "Fill shift in case of item splitting" on page H-2835
-> "Split items" on page H-2925

#### Graphic group
- **Production area**: Opens a graphic daily overview of the production area. -> "Graphic" on page H-2934

### Options menu
**Path:** `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Options menu`

Using this menu, you can determine the default setting of the dialog. You can activate or deactivate options. The setting is not reset when you close the dialog. The description of the following entries reflects the activated state:
- **Move setup time**: Enables the possibility to move the set-up times.
- **Suppress messages**: Errors that occur during rescheduling for another date or another machine are displayed in a message. You can suppress these messages.

### Control station (machine) – shift tab (Move I)
**Path:** `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Move I tab`

On this tab you check which orders and quantities have to be produced per shift by this machine.

#### Navigation through the tabs
- Double-click on order number -> Control station (order)

#### Overview
The quantities for the selected machine are displayed in the overview.
- **Date**: Production date.
- **Shift**: Shift in which the orders are produced.
- **Order**: Order number.
- **Pcs.**: Pieces of the order on the current machine.
- **Finished**: Quantity of glass produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Time scheduled for the quantity.

#### Move
- **New date**: Production date to which the order shall be moved.
- **Shift**: Shift to which the order shall be moved.
- **Machine**: Machine to which the order shall be moved.
- **[Load]**: Checks the utilization of the alternative machine. The value is displayed in hours. It includes the times for the order you have selected by clicking the row header.
- **[Roll back]**: Sets the move back to the original values.

### Control station (machine) – load tab
**Path:** `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Load tab`

On this tab, all items are displayed that must be produced in the selected period.
-> Tutorial, "Control Station – Machine" on page H-2818

#### Selection
- **From date, to date**: Entry of the period whose load you want to check.
- **Machine**: Selection of the machine for which you want to check the utilization.

#### Overview
In the overview, all order items are listed that must be produced in the selected period.
- **Date**: Production date.
- **Shift**: Shift in which the item is produced.
- **Order, item**: Order and item number from the order.
- **Product**: Product name.
- **Glass size**: Size of the item.
- **Element**: Product name of the BOM component.
- **Work type**: Work type in the production area.
- **Pcs**: Number of pieces of the item.
- **Time**: Planned time
- **Customer**: Customer name from the order.

### Control station (machine) – move II tab
**Path:** `Production > Capacity planning > Control station > Machines tab > Double-click on row header > Control station (machine) > Move II tab`

On this tab, all shifts are displayed in the selected period. A cell is highlighted in color if there is a problem during scheduling.

#### [Overview]
In the overview, all shifts for the selected period are listed.
- **Date**: Production date.
- **Shift**: Shift in which the pieces are produced.
- **Pcs**: Number of pieces of the item.
- **Hours**: Time required. If problems arise during scheduling, the field is highlighted red.

#### Move
The fields in this area are described for the **Move I** tab.
-> "Control station (machine) - shift" on page H-2977

## Utilization (date)
**Path:** `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization`

On this dialog, you display an overview of the quantities to be produced for a specified time period. The overview can optionally be output by production areas, machines or machine types. The data is displayed if you have started the filtering in the **Start > Execute** menu.

This section provides information on the following subjects:
- "Plant menu" on page H-2981
- "Display menu" on page H-2982
- "Utilization (date) (display period)" on page H-2982
- "Utilization (date) – selection" on page H-2984
- "Utilization on (date) – details" on page H-2984
- "Utilization - graphic" on page H-2985
- "Utilization - print" on page H-2985

### Plant menu
**Path:** `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization > Plant menu`

With this menu you specify whether the capacity of an individual plant or all plants shall be considered.
- **All**: All defined production areas are displayed.
- **Plant 1**: Only the production areas with entry 0 and 1 are displayed.
- **Plant 2**: Only the production areas with entry 0 and 2 are displayed.
- **Plant 3**: Only the production areas with entry 0 and 3 are displayed.

The plant refers to the code that is entered in the client's company data. Clients can be allocated in the **Production areas** dialog.

### Display menu
**Path:** `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization > Display menu`
- **Display status**: With this menu you can specify the order status up to which the orders shall be displayed. -> "Display status" on page H-2985

### Utilization (date) (display period)
**Path:** `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization`

On this dialog, you check the criteria for the display of the utilization. You can display the result as a graphic or as a list.
-> "Utilization - graphic" on page H-2985
-> "Utilization - print" on page H-2985

#### Evaluation period
- **From, to**: Period for which you would like to have an overview.

#### Options
- **Show turnover**: This checkbox is only enabled if you have selected the **Machine** option in the **Overview of** area.
    - [x] The turnover is not displayed.
    - [ ] The turnover for the selected machine is displayed.

#### Overview of
With the selection of the options, you filter the display.
- **Production area**: You can limit the overview to a particular production area (<n.e.> = all).
- **Machine types**: You can limit the overview to a particular machine type.
- **Machine**: You can limit the overview to a particular machine. With this option, you can activate the **Show turnover** checkbox.
- **All machines by production area**: With this option, all machines are sorted by production areas.

#### Overview
The following data is displayed in the overview:
- **Date, Production areas/machines**: The utilization is displayed per date and production area or machine.
- **Pcs.**: Total quantity.
- **Area**: Total area.
- **Circumference**: Total edge length.
- **Time**: Scheduled time.
- **Costs**: Time costs.
- **Turnover**: Turnover per machine. This column is only displayed if you have selected the **Machine** option and ticked the **Show turnover** checkbox.

### Utilization (date) – selection
**Path:** `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization > Display evaluation period > Click in row header > Details tab Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization > Display evaluation period > Click in row header > Selection tab`

On this dialog, you check the utilization in a particular period.

#### Evaluation - date
- **From, to**: Period for which you would like to have an overview. Period to be evaluated.
- **Only shift**: Specification of the shift whose utilization shall be displayed. The field is only enabled in selection mode.
- **Shift info**: The checkbox is only enabled in selection mode.
    - [x] The selection is not limited to particular shifts. After filtering, all shifts are displayed in the overview.
    - [ ] The selection is limited to the shift that is specified in the **Only shift** field.

#### Overview
With the selection of the option, you specify the filtering of the display:
- **All production areas**: The utilization of all production areas in the set period is displayed.
- **All machines**: The utilization of all machines in the set period is displayed.
- **Only for production area**: The utilization for a particular production area is displayed. The field for selection of the production area is enabled.

- **Arrange detailed view**: With the selection of the option, you specify the grouping on the **Details** tab. The fields are only enabled if data is displayed.
    - **Order, customer**: The utilization is displayed per order and customer.
    - **Product**: The utilization is displayed per product.

#### Utilization
The hit list is displayed in the overview.

### Utilization on (date) – details
**Path:** `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization > Display evaluation period > Click in row header > Details tab`

On this dialog, you check the details of the utilization.

#### Navigation through the tabs
- Click on row header -> Production status - order

#### Details
The display of the columns and data is oriented according to the selection criteria. The lists are grouped by the option that is marked on the **Selection** tab.
- **Production area**: Display of the production area in which the machines are or where the work will be performed.
- **Number manager**: Selection of the number manager in which the orders displayed shall be placed.
- **[Fill NM]**: Places all displayed orders in the specified number manager.

### Utilization – graphic
**Path:** `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization > Display evaluation period > Click in row header > Utilization (date) - Selection > Functions menu > Utilization group > Display graphic`

The graphic display shows the utilization based on the criteria selected on the **Utilization (date)** dialog.
You can print the result from the **Utilization (date)** dialog. The period to be printed can be limited to 8 or 12 days.
-> "Utilization - print" on page H-2985

### Utilization – print
**Path:** `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization > Display evaluation period > Print menu`

You can print the result shown in the dialog **Utilization at a date**. The period to be printed can be limited to 8 or 12 days. If you choose 12 days please make sure to print the list in horizontal format.
The display shows a daily overview of the units to be produced per machine and production area. In addition, the target value is specified.

## Display status
**Path:** `Production > Capacity planning > Control station > Machines tab > Functions menu > Display group > Utilization > Display menu > Options group > Status display`

On this dialog, you limit the display of the orders to a maximum status. Displayed are only the orders whose status is smaller than the status entered.

## Settings for control Station
**Path:** `Production > Capacity planning > Completion report > Functions menu > Settings`

On this dialog, you specify which data shall be displayed in the **Control station** dialog.
You must confirm the changed settings with **[OK]**. The **Control station** dialog must be re-opened so that the data can be reloaded.

### Only these production areas
You can limit the display to a particular production area or several production areas. If no entry has been selected, all production areas will be displayed.

### Selection criteria
- **Display only the items not produced**: You can set that only the items not produced are displayed:
    - [ ] With this setting, completed and not yet completed items are displayed.
    - [x] With this setting, only the items are displayed that must still be produced.
- **Order area**: You can limit the display to a particular order area. The combo box for selecting the order area is accessible.
- **From status, to status**: You can limit the display by order status. If you select the same status in both fields, only orders with this one status will be displayed.

### Display in addition to times
By default, only the hours available on the day per machine are displayed. You can expand these details to include the following details:
- **Pcs.**: Quantities for all shifts and orders.
- **Sqm**: Total area for all shifts and orders.
- **Linear m**: Total edge length for all shifts and orders.
- **In %**: Percentage utilization for all shifts.
- [x] The information is not displayed.
- [ ] The information is displayed on the **Machines** and **Orders** tabs.

## Residue qty.
**Path:** `Production > Capacity planning > Control station > Functions menu > Residue qty.`

On this dialog, you check which orders still need to be reported completed, and to report them as such if required.

- **Display from status**: You can limit the display of the open orders to a minimum status, e.g. to exclude orders from the display the production of which has already begun.

### Overview
In the overview, all orders are displayed that were not produced up to the current date. When you tick the checkbox, the corresponding order will be reported completed for the current date when you press **[OK]**.

## Control station (order)
**Path:** `Production > Capacity planning > Control station > Functions menu > Select order.`

On this dialog you check the individual machines that an order runs through from production to shipping to move the scheduling on the "critical" machines.
-> Tutorial, "Control Station (Order)" on page H-2817

The **Control station (order)** dialog contains the following tabs:
- Control station (order) – machines
- Control station (order) – detail
- Control station (order) – work types
- Control station (order) – purchased elements
- Control station (order) – move I
- Control station (order) – move II
- Control station (order) – load

### Navigation through the tabs and dialogs
| Tab | Action | Tab / dialog |
| --- | --- | --- |
| Machines | Double-click on machine | -> Move II |
| | Double-click on date | -> Detail |
| Detail | Click on cell header | -> Work types |

### Functions menu
**Path:** `Production > Capacity planning > Control station > Functions menu > Select order > Functions menu`

Using this menu, you can open other dialogs without closing the control station.
The menu is organized in the following groups:
- Document group
- Graphic group
- Production group

#### Document group
- **Show document**: Opens the document view.
- **History**: Opens the **History** dialog where you can check the process of status changes. -> Sales, "History" on page C-1662
- **Status change**: Opens the dialog by the same name where you can change the order status. -> Sales, "Status change" on page C-1664

#### Graphic group
- **Production area**: Opens the graphic display **Production areas/weekly overview** to compare the completed and open quantities.
- **Order**: Opens the graphic display **Order info/weekly overview** to compare the completed and open quantities.
These graphics correspond to the Graphic areas display. -> "Area graphic" on page H-2901

#### Production group
- **Reports list**: Opens the **Reports overview** dialog to check the current status of production per order item. -> "Report list" on page H-2953
- **Scheduling**: Opens the **Schedule order** dialog to change the scheduling of the current order. -> "Schedule order" on page H-2915
- **Manual settings**: Opens the **Order completion status** dialog on which you can check the production status of the order. -> "Production status - order" on page H-2943

### Options menu
**Path:** `Production > Capacity planning > Control station > Functions menu > Select order > Options menu`

Using this menu, you can determine the default setting of the dialog. You can activate or deactivate options. The setting is not reset when you close the dialog. The description of the following entries reflects the activated state:
- **Check dwell time**: Before moving, it is checked whether the transfer times permit a move. You should select this setting if you know that the transfer requires longer transfer times, e.g. for TG production. You should only suppress this check if the transfer from one production area to the next one does not require long transfer times.
- **Ignore dwell days**: Ignores the dwell day when rescheduling.
- **Postpone setup time**: If this option is activated, the buttons on the **Move II** tab are locked.
- **Setup time check**: If the set-up time has been defined for several work types performed for an order item, this time shall be charged just once per item.
- **Suppress messages**: Errors that occur during rescheduling for another date or another machine are displayed in a message. You can suppress these messages.

### Control station (order) – machines tab
**Path:** `Production > Capacity planning > Control station > Functions menu > Machines tab`

On this tab you check the utilization of the machines which are producing this order. If you have opened the dialog from the control station, the data for the current order is displayed. However, you can use the search mode to display another order or limit the display to a particular position.
If the order was reported completed manually, all previously not reported values are shifted to the day of the completion report. In this case, the production dates are shown in green.

#### Order
- **Number, customer**: Number and customer name stated in the order.
- **Only item**: Number of the item to be changed. The field is enabled in selection mode. You can specify the item number if you want to display one order item only. If you enter a zero (0), all items are displayed.
- **Delivery date**: Delivery date stated in the order. You can change the date and confirm with **[Change]**. -> Tutorial, "Postpone Scheduling for Single Order" on page H-2819
- **[Change]**: Confirms the new date.
- **Order area**: Order area from which the order comes.
- **Production from - to**: Display of the period in which the order is produced.

#### Overview
- **Machine**: Machines on which the order is produced.
- **Day of the week, date**: Per weekday, the utilization is displayed with the scheduled and free time (all shifts) per machine.
    - Scheduled and free time (all shifts).
    - Open and produced quantity of all sheets in pcs.
    - Total surface in sqm.
    - Edge length of all sheets.
    - Utilization in percent.
All details except for the time can be selected or deselected in the control station settings.
-> "Settings for control Station" on page H-2986

### Control station (order) – detail tab
**Path:** `Production > Capacity planning > Control station > Functions menu > Select order > Detail tab`

On this tab, you can move quantities manually or report them completed. The machine to which these details refer is shown above the fields. If you have moved one item completely, it is deleted from the display.

#### Overview
The quantities for the current order for the selected machine are displayed in the overview. The following columns are displayed:
- **Shift**: Current shift.
- **Pcs.**: Pieces of the order on the current machine.
- **Finished**: Quantity of glass produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Time scheduled for the quantity.

- **[Load / day]**: Updates the display in the fields below.

#### Move
- **New date**: Production date to which the order shall be moved.
- **Shift**: Shift to which the order shall be moved.
- **Machine**: Machine to which the order shall be moved. The field is enabled if you have ticked the **Move** checkbox and confirmed with **[OK]**.
- **[Load]**: Checks the utilization of the alternative machine. The value is displayed in hours. It includes the times of the order.
- **[Roll back]**: Sets the move back to the original values.

### Control station (order) – work types tab
**Path:** `Production > Capacity planning > Control station > Functions menu > Select order > Work types tab`

On this tab you check which work types are to be performed on a machine on a production date. If you have moved one item completely to another date, it is deleted from the display.

- **[All]**, **[None]**: Ticks all checkboxes in the **Move** column or removes the ticking.

> **Edit setup times**
> Using the context menu (right mouse key) on an item, you can add or delete set-up times. For this, the set-up time must be created as work type with a basic time.

#### Overview
- **Shift**: Shift in which the item shall be produced.
- **Item**: Item number from the order.
- **BOM ID**: BOM ident number, that is the BOM level.
- **SI**: Sub-items (packages) resulting from the splitting of items at scheduling.
- **Process**: Work type.
- **Product/Processing**: Product name.
- **Pcs.**: Item quantity.
- **Finished**: Quantity of sheets produced.
- **Size**: Dimensions of the item.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved. This message can be switched off using the **Options** menu.
- **Hours**: Time reserved for this item.

#### Move scheduling
The fields in the **Move** area are explained for the **Detail** tab.
-> "Control station (order) – detail" on page H-2992

### Control station (order) – purchased elements tab
**Path:** `Production > Capacity planning > Control station > Functions menu > Select order > Purchased elements tab`

On this tab you check which purchased articles are required for production.

#### Overview
- **Item**: Item number from the order.
- **Article**: Product name of the purchased element.
- **Quantity**: Quantity to be purchased.
- **Size**: Dimensions of the item.
- **Ordered to**: Delivery date requested by the supplier.
- **Deliv.**: Quantity delivered.
- **Required on, date, shift**: These three columns display when the purchased elements are required where.

### Control station (order) – move I tab
**Path:** `Production > Capacity planning > Control station > Functions menu > Select order > Move II tab`

On this tab, you plan and edit the load of the machines with series. This function is not currently used.

#### Order
This area displays the order number and name of the customer.

#### Postpone for whole days
- **No. of days**: Number of days by which the production of the series shall be postponed.
- **Only from date**: Initial date from which the full days specified above shall be counted.

### Control station (order) – move II tab
**Path:** `Production > Capacity planning > Control station > Functions menu > Select order > Move II tab`

On this tab, you move the items or orders to other dates, shifts or machines. If you have moved one item completely, it is deleted from the display.

#### Overview
The quantities for the current order for the selected machine are displayed in the overview. The following columns are displayed:
- **Date**: Scheduled production date.
- **Shift**: Current shift.
- **Pcs.**: Pieces of the order on the current machine.
- **Finished**: Quantity of glass produced.
- **Move**: Changes can be adopted only if this checkbox is ticked. If the changes clash with other processes for this order, an error message will tell you that this process cannot be moved.
- **Hours**: Time scheduled for the quantity.

> **Areas locked**
> The **Fill shift** and **Compress** areas can be locked via the **Options > Move setup time** menu.

#### Fill shift
You can recheck the shift times using suitable quantities from the previous or the next shift.
- **[Backwards]**: Recalculates the shifts. The quantities are moved to an earlier shift if possible.
- **[Forward]**: Recalculates the shifts. The quantities are moved to the next shift if this is possible.

#### Compress
You can recalculate the utilization of the machine. This way you can fill gaps which occurred due to the settings regarding the proportional utilization when an item was split or if e.g. an order was cancelled so that there is more free capacity.
-> "Fill shift in case of item splitting" on page H-2835
-> "Split items" on page H-2925
- **[Backwards]**: Recalculates the utilization starting backwards from the displayed date.
- **[Forward]**: Recalculates the utilization, starting forward from the displayed date.

#### Move
The fields in the **Move** area are explained for the **Detail** tab.
-> "Control station (order) – detail" on page H-2992

### Control station (order) – load tab
**Path:** `Production > Capacity planning > Control station > Functions menu > Select order > Load tab`

On this tab, you check which order items are to be produced by the machine in addition to the current order items. The order items for which the display has been started are highlighted in green.

#### Selection
- **From date, to date**: Period that you want to check.
- **Machine**: Machine for which you want to check the scheduled orders.

#### Overview
In the overview, all order items are listed that must be produced in the selected period.
- **Date**: Production date.
- **Shift**: Shift in which the item is produced.
- **Order, item**: Order and item number.
- **Product**: Product name.
- **Glass size**: Size of the item.
- **Element**: Product name of the BOM component.
- **Work type**: Work type in the production area.
- **Pcs**: Number of pieces of the item.
- **Time**: Scheduled time
- **Customer**: Customer name from the order.

## Moving impossible
**Path:** `Production > Capacity planning > Control station > Move`

On this dialog you check why the intended move of an order is impossible. You can suppress the display of this message.

# A+W Business Box Management
## Revision overview of the module:

| Date | Description |
| --- | --- |
| 12-2019 | Updating the settings in the master data. Transfer of box purchase orders from Purchase part and stock bookings from Production part. |
| 12-2018 | Original version box management: Separation from Stock, Purchase and Production parts. |

This section provides information on the following subjects:
- Tutorial
- Software Reference
