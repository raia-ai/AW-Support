---
description: "A+W Business Pro Capacity Planning"
---


# A+W Business Pro Capacity Planning Tutorial

---
## Master Data

### Special allocations:

- **Special allocation 1:** This allocation is made for the product type Processing which is followed by another processing step.
- **Special allocation 2:** This allocation is made for the processing of shapes.
- **Special allocation 3:** This allocation is made for edgework.
- **Special allocation 4:** This allocation is made for the processing and following processing steps for shapes.
- **Combined product group:** This allocation is made for individual products that can be part of the BOM of a product (in a product group), e.g. the product Float 6 mm as part of a LG unit (product class Laminated glass).
- **Stock article:** This allocation is made for stock articles (articles taken from stock) which are just packed and shipped. As a result, this product class is e.g. scheduled for dispatch, and the appropriate cost and time is calculated.

> **Description of allocation dialogs**
> For a detailed description of the dialogs please refer to the Software Reference.

### Combined Product Type, Combined Product Class

Products which are part of a bill of materials, or which influence a product group as a processing step, can be allocated differently. This means that the product can be allocated to different work types depending on the combined product type or combined product class in which it is used.

> **Example**
> Float glass is part of IG units, and part of LG. The cutting table for IG is located in the same hall as the IG line. The cutting table for LG is in the same hall as the LG production. This means that two different work types have to be defined, one each for the corresponding cutting type.
>
> You can therefore allocate the work type Laminated glass cutting to the float glass if it is part of the LG bill of material.

When you have defined two work types for cutting, you can allocate the corresponding cutting tables to the work types (in Default Times). If there is a bottleneck at one cutting table however, the other will not be used because it has not been allocated to the other work type.

**Example: Cutting control for product class LG**

This diagram illustrates how allocations direct production based on product context.

*   **Standard Path**:
    *   **Allocation**: Product type `Single glass`
    *   **Work type**: `Cutting`
    *   **Machine**: `Cutting table I` in `Hall A`

*   **Conditional Path**:
    *   **Allocation**: If `float 6 mm` is in product class `LG` (Combined product class)
    *   **Work type**: `Cutting LG`
    *   **Machine**: `Cutting table II` in `Hall B`

Cutting table I is used to capacity with this. If a float glass sheet shall be cut for a laminated sheet, cutting table I will be ignored, and cutting table II is chosen.

Both dialogs for allocation are structured analogously. The Combination product type dialog is used as an example here.

**Example for the allocation of work type to product**

This example shows that product `Float 4 mm` (A) has been allocated to work type `LG cutting` (C) if this is part of the product type `LG` (B).

*   **(A) Selected product**:
    *   **Identification**: `104`
    *   **Product**: `Float 4 mm A+W`
*   **(B) Selected product is part of**:
    *   **as part of/affects**: `VSG/Laminated glass`
*   **(C) Work types allocated to the selected product**:
    *   **Work type**: `10003 - VSG Zuschnitt / LG cutting`

### Define Allocation

In this example, a special allocation is made for the edge processings in shapes. It serves to explain nearly all steps that can occur in connection with allocations. The allocations in the other dialogs are made accordingly.

**How to specify a special allocation**

1.  Select in the module `Capacity planning > Allocation > Special allocation 4`. The dialog of the same name opens. This dialog is described in the Software Reference.
2.  Select in the menu `Start > New` to change to the recording mode. The fields for a new special allocation are released.
3.  Select the A+W Business Pro master data:
    *   Product, e.g. ornamental glass (A)
    *   Processing, e.g. seaming (B)
    *   Shape, e.g. shape with 2 rounded corners (C).
    The data are displayed in the overview.

**Specifying special allocation**

In the `Identification` group, a sketch of the shape (A) is displayed, from which you can see the numbering of the edges and corners.

*   **(A) Schematic sketch of the shape**
*   **(B) Insert fields**
*   **(C) Edges of the shape**

4.  Click in the `Work types with edge allocation` group on `[New]` (B) to enter the first work type.
5.  Place the cursor in the `Work type` field and select the first work type from the combo box, e.g. `Hand cutting`.
6.  Repeat step 4 and 5 to select the next work types, e.g. `Seaming`, `Washing`.
7.  Place the cursor in the `Factor` field and enter the factor by which this work type should be increased, e.g. `2.5`.
    This factor means that the time defined for seaming will be multiplied by 2.5 if a shape with two rounded corners is produced.
8.  Tick the checkboxes in columns 1 to 6 to select the edges to be processed, to which the factor shall be applied.
    If the factor is not to be applied to all edges, you have to define a second allocation for the remaining edges.
    
    *This example shows that edge 1 shall be processed first. No additional time will be charged for that. For edges 2 to 6, the required time will be increased by a factor.*
9.  Check the sequence of the steps.
    If you select a line you can use the arrow buttons to move the work step up or down until the right sequence is achieved.
10. Select in the menu `Start > Save` to save the data.
    The data will be saved. The sequence of work types has been fixed.

### Exercises

*   Specify the complete allocations for IG units with shape as shown in the examples.
    This exercise is quite complex. Therefore, feel free to adopt the examples.
    ⇨ "Case Study IG and Shape" on page H-60

**Additional information**
⇨ Software Reference, "Allocation" on page H-229

# Capacity Planning

Orders have to be scheduled in capacity planning so that the time costs are calculated and production times can be planned. The dates will be calculated based on the settings you have made in master data.

This session will show you how to determine dates, schedule orders, handle capacity problems, how to control automatic scheduling in general, and how to monitor the planning by means of the control unit.

This includes the following learning sections:

*   "Scheduling Orders" on page H-108
*   "Production” on page H-131
*   "Production Costs" on page H-153
*   "Control Station" on page H-161

## Scheduling Orders

**Objectives**
*   Get to know date calculation.
*   Recognize planning processes.
*   Get to know flow of scheduling.

**Benefits**
*   Orders are usually scheduled by a work flow task. You will only have to intervene in case of bottlenecks. It is therefore essential to know the scheduling process in detail.

**Note**

| Term | Description |
| :--- | :--- |
| **Scheduling** | Scheduling always starts from the delivery at the customer's and calculates the production dates so that the produced goods do not have to be stored. |
| **Bottleneck** | Bottlenecks usually occur only at machines performing complex work types. Cutting for example is generally unproblematic. |
| **Residual quantities** | Residue from the day before are items of which the production has not begun yet. Once the first sheet has been produced, the remaining quantities are no longer considered as residue. |
| **Closing time** | Closing time defines the point in time up to which orders can be scheduled for a shift. This makes sure that the scheduled orders can actually be produced, and no residue remains for the next day. |
| **Default settings** | **Company data:**<br>- Capacity planning tab |

### Date Calculation

Scheduling starts from the delivery date, from which the individual processes are counted back. The explicit and implicit work processes defined in the bills of materials are scheduled for the most cost-effective, valid machine according to their chronological sequence and their position on the bills of materials. If this is used to capacity, another machine will be selected (automatically or manually).

#### Backward scheduling

Scheduling is based on the delivery date. The check for free capacities always starts with the last work type in the last shift before the delivery date, e.g. packing in shift 2, then goes back to shift 1.

If all machines are used to capacity for a work process on a certain day, the program tries to move the process to the day before, etc.

#### Forward scheduling

If all backward scheduling is to no avail, the program searches for a new delivery date based on the next possible route day. Backward scheduling then starts again from that new date. This process can be repeated until scheduling is successful.

#### Times for date calculation

In addition to the production times of a machine, dwell and transition times are considered. These times were described in detail in the Default Times section. In summary, this concerns the following criteria:

*   Change of the production area, e.g. from cutting to washing.
*   Change of work type, e.g. from cutting a ticket window to fine polishing of the hole edge.
*   Rest time in the production area, e.g. cooling off after the TG furnace.

When the production area is changed, the definition in the `Transition matrix` dialog will override the entry in the `Production area` dialog.

If on both dialogs times are stored, the following must be observed:
*   `Produce LG` and `Saw LG` are e.g. two work types performed in the same production area, `Laminated glass`. In this case, only the transition time defined in the `Transition times` dialog will be considered.
*   `TG production` and `Picking` are two work types executed in different production areas. In this case, capacity planning will check the entries in the `Transition matrix` dialog and the `Transition times` dialog. The higher value will be used.

The following examples show how the definitions in the different dialogs influence the calculation of the start of production. Our example is based on a company working in three shifts as a standard. The production area `Heat soak test` only works one shift.

#### Example for dwell days

This example shows only entries in the Production area dialog. If one dwell day each is set for every production area, this will influence the calculation of the start of production as follows.

| | |
| :--- | :--- |
| **Work types** | `Cutting` -> `Heat-soak test` -> `Picking` |
| **Calculation of dates** | - Delivery date is Friday.<br>- Heat-soak test on Wednesday in the 1st shift.<br>- Picking on Thursday in the 1st shift<br>- Cutting (production start) on Tuesday in the 1st shift |

**Example with dwell days in the production area (Time scheme 1)**

This diagram shows backward scheduling from a Friday delivery date:
*   **Delivery**: Friday.
*   **Picking**: Occurs on Thursday (1 day dwell time before delivery). The production area has 3 shifts available.
*   **Heat-soak test**: Occurs on Wednesday (1 day dwell time before picking). The production area has only 1 shift available (shifts 2 and 3 are 0).
*   **Cutting**: Occurs on Tuesday (1 day dwell time before heat-soak test). The production area has 3 shifts available.

This example shows that the shifts will not be taken into account if one holding day has been defined per production area.

#### Example for different transition times

In this example, there are entries on the `Transition matrix` and `Transition times` dialogs. The start day of the production is calculated as follows.

| | |
| :--- | :--- |
| **Work types** | `Cutting` -> `Heat-soak test` -> `Picking` |
| **Calculation of dates** | - The delivery date is Friday.<br>- In the `Transition matrix` dialog, 0.1 days (= one shift) was entered for all production areas. Assuming that this route will be shipped in the second shift by default, picking can still be done in the first shift on Friday. Otherwise, picking takes place in the third shift on Thursday.<br>- In the `Transition time` dialog, the value 3 is entered. Starting from picking which is done in the first shift on Friday, three shifts are counted backwards. Even if 0 has been entered for the heat soak test in shifts 2 and 3, these will be included in the reckoning. The heat soak test therefore starts only in the first shift on Thursday. The entry in the `Transition matrix` dialog is ignored because the entry in the `Transition times` dialog is higher.<br>- Cutting (start production) is done in the third shift on Wednesday because the transition from production area Cutting to the heat soak test has been defined as 0.1 days (= one shift) in the `Transition matrix` dialog. |

**Example with transition times (Time scheme 2)**

This diagram shows backward scheduling incorporating transition times:
*   **Delivery**: Friday.
*   **Picking**: Occurs on Friday. There's a 0.1 day transition from the `Transition matrix` and a 0 shift transition between work types. Production area has 3 shifts.
*   **Heat-soak test**: Occurs on Thursday. There's a 0.1 day transition from the `Transition matrix` and a 3 shift transition between work types (Picking to Heat-soak). The production area has only 1 shift.
*   **Cutting**: Occurs on Wednesday. There's a 0.1 day transition from the `Transition matrix` and a 0 shift transition between work types (Heat-soak to Cutting). Production area has 3 shifts.

This example shows how the shifts are taken into account for calculation.

#### Example for transition times for several work processes in one shift

The start of production is determined as follows.

| | |
| :--- | :--- |
| **Work types** | `Cutting` -> `Grinding` -> `Screen printing` -> `Picking` |
| **Calculation of the dates** | - The delivery date is Friday.<br>- 0.1 days (= one shift) has been entered in the `Transition matrix` dialog. If this route is shipped in the second shift, picking can be done in the first shift on Friday. Otherwise, picking takes place in the third shift on Thursday.<br>- The entry in the `Transition time` dialog is 2. Starting from picking which is done in the first shift on Friday, two shifts are counted backwards. Silk screening therefore starts in the second shift on Thursday. The entry in the `Transition matrix` dialog is ignored because the entry in the `Transition times` dialog is higher.<br>- The entry in the `Transition matrix` dialog for the transition from production area `Grinding` to production area `Silk Screening` is 0.1 days (= one shift). `Grinding` starts in the first shift on Thursday.<br>- `Cutting` (start of production) is done in the same shift as `grinding` because the entry in the `Transition matrix` dialog is 0 (= same shift). |

**Example with different work types in the same shift (Time scheme 3)**

This diagram shows a more complex backward schedule:
*   **Delivery**: Friday.
*   **Picking**: Occurs on Friday. 0.1 day transition from matrix, 0 shift transition between work types.
*   **Screen printing**: Occurs on Thursday. 0.1 day transition from matrix, 2 shift transition between work types.
*   **Grinding**: Occurs on Thursday. 0.1 day transition from matrix, 0 shift transition between work types.
*   **Cutting**: Occurs on Thursday.

This example shows a calculation where several work types can be performed on the same day.

### Scheduling

There are three ways of scheduling orders in capacity planning:

*   Manually, per order
*   Manually, per number manager
*   Automatically, in batch operation.
    In this case, the orders are entered in capacity scheduling via work flow task. The program will automatically search for new orders in defined intervals.

#### Manual scheduling

For manual scheduling, the defaults can be set so that you can trace every single step by scheduling the order items individually to different machines. In general, you will want to set the default so that intervention is only required in case of bottlenecks.

Manual intervention is necessary if you are not satisfied with the scheduling results. Orders will have to be rescheduled in that case.

Rescheduling may also be necessary if a machine breaks down and needs to be repaired.

For manual scheduling, you can e.g. define the earliest start of production.

> **Example**
> If an order entered in September with a delivery date of 25.11. is to be produced so that the finished units do not have to be stored, you can enter a date for the earliest start of production.

#### Automatic scheduling

A work flow task (batch program) can be used to schedule orders automatically for production. The program will automatically search for free machines. Depending on the setting you will have to intervene only in case of bottlenecks, e.g. if machine A is used to capacity while machines B and C are not.

You can use the `Control unit` dialog to intervene in scheduling, and reschedule items to another machine or another date.

### Settings for the work flow task

> **Info**
> Work flow tasks serve to process orders automatically. If manual intervention between two successive work flow tasks is necessary, depends on how the processes in your company are organized. The necessary settings are made during the installation of A+W Business Pro and should not be changed afterwards. This paragraph therefore only explains the basic principles.

A work flow task consists of one or more customizing formulas. These formulas define the individual actions to be performed. The A+W Business Interface Service executes the task at a fixed time or in intervals.

Three steps are necessary for defining a work flow task:

*   Define the formulas in `Master data > Company > Formulas`. For capacity planning purposes, these can be e.g. formulas for searching for orders:
    *   to be scheduled
    *   left over from the day before (residue)
*   Allocate the formulas to a work flow task in `Master data > Company > Customizing > Work flow tasks` tab.
*   Set the starting time or interval for the work flow task in `Master data > Company > Customizing > Autom. process execution` tab.

If you want to define work flow tasks, please ask a member of the A+W Software GmbH team for support.

> **Transfer to production**
> Orders are not automatically transferred from capacity planning to production. The transfer to production is handled by a separate work flow task.

### Capacity Problems

Cutting usually causes no problems because it is done right at the start of the production chain. Capacity bottlenecks can occur easily however if a process is more complex, e.g. in connection with shapes or IG production.

If (automatic) scheduling encounters capacity bottlenecks, manual intervention should be possible. You can of course make the default settings so that any order can be scheduled by means of automatic postponement of delivery dates. Manual intervention permits however to move less complex orders in favour of others.

### Item split

Apart from postponing dates, large items can also be split if shift times and machine utilization require this. Production of an item will be split into several shifts and/or days this way.

Splitting items into sub-items offers the following options:

*   You can enter the quantity for every sub-item required.
*   You let the program create the necessary sub-items.

In the following example, 100 IG units with two rounded corners shall be produced. This is a total of 400 rounded corners for which a total time of 13.66 hours must be scheduled. The machine works 8 hours a shift. This means that the item must be split.

**Exceeding of the machine capacity - Splitting**

The UI shows a "Capacity bottleneck" on the `Forvet A+W` machine for an order of 100 `Rundecken/Rounded corner A` units. The required time is 11.6 hours, but the maximum time available is 8 hours. The user is presented with an option to split the item.

From 100 sheets in order item 3, two sub-items of 50 sheets each are created for cutting and processing. Splitting is not required for the cutting process. It is done however so that the cut sheets do not have to be stored before processing.

The production of 100 IG units is distributed as follows.
(SI = sub-item)

| SI | Glass / unit | Machine | Date |
| :-- | :--- | :--- | :--- |
| SI 1 | Glass 1 | Cutting 50 sheets | Shift 2 on 08/02 |
| | Glass 2 | Cutting 50 sheets | Shift 2 on 08/02 |
| | Glass 1 + Glass 2 | Rounded corners on 100 sheets | Shift 1 on 08/03 |
| | IG production | 50 pcs | Shift 1 on 08/04 |
| | Picking/shipping | 50 pcs | Shift 1 on 08/05 |
| SI 2 | Glass 1 | Cutting 50 sheets | Shift 1 on 08/03 |
| | Glass 2 | Cutting 50 sheets | Shift 1 on 08/03 |
| | Glass 1 + Glass 2 | Rounded corners on 100 sheets | Shift 1 on 08/04 |
| | IG production | 50 pcs | Shift 2 on 08/04 |
| | Picking/shipping | 50 pcs | Shift 1 on 08/05 |

### Reserving production times

In the splitting process, the remaining time of a shift can be locked for other orders. This prevents the machine from being set up again in the course of a shift.

You can also define the production date. This is especially useful if the production times for the different processes differ considerably.

> **Example**
> 10 oversized IG sheets have to be produced.
> All sheets can be cut on the same day. The IG line can only produce one unit of this size per day. This means that the cut sheets have to be stored up to 9 days.
>
> Splitting creates 10 sub-items (= one IG sheet per day) for which you define the production dates.
> Every sub-item will be cut separately and is produced on the IG line the same day.

### Closing Time

Obviously, items cannot be produced completely if they are scheduled at the end of a shift. Since unfinished items have to be produced the next day (as residue from the day before), you should define times for the last scheduling.

The closing time defines the point in time up to which orders can be scheduled for a shift. This makes sure that the scheduled orders can actually be produced, and no residue remains for the next day.

> **Example**
> You receive a new order on Friday 12 a.m. In manual scheduling you enter 2 p.m. although the shift ends at 4 p.m. This means that the order will not be scheduled because it cannot be produced that day.
>
> If the order cannot be scheduled because of the closing time, the dialog `Delivery date` issues a message to that effect. You will have to change the delivery date.

Closing times are generally defined in the dialog `Shift settings`. In case of bottlenecks, manual intervention can be used to check the times.
⇨ "Shift Settings" on page H-183

### Default Settings for Automatic Scheduling

The settings for the number of shifts and the degree of utilization in company data have been introduced in the section on `Shifts and working times`. This description is completed by the machine settings in the section on `Machine Selection`.

⇨ "Default Settings for Shift and Capacities" on page H-43
⇨ "Default Settings for Machine Selection" on page H-95

In addition to these settings, you have other setting possibilities for controlling automatic scheduling.

**Company data - Capacity planning**
The screenshot shows the capacity planning settings tab in the company data. Key settings are highlighted:

*   **(A) Autom. delivery date search by route**: Allows the system to find a new delivery date if needed.
*   **(B) Fill shift in case of item splitting**: Defines the percentage of a shift that can be filled by split items (e.g., 50%).
*   **(C) Schedule for delivery date**: Forces scheduling to adhere to the order's delivery date.
*   **(D) Do not split order**: Prevents the system from automatically splitting orders.

If you permit that orders are split at automatic scheduling you must also define how much of the machine capacity can be used (B). This is not necessary if you prevent automatic scheduling (D). Please consider however that an order item can be so big that its production exceeds the capacity of the machine. The order cannot be scheduled and manual intervention is required.

#### Choosing of the delivery date

The program can automatically search for a new delivery date in case of bottlenecks. A route day (A) should be chosen as the next delivery date. The suggested date can be changed manually for rush orders, e.g. if a special route is used for delivery. This setting only makes sense however if you have defined routes and allocated them to the customers.

You can also force the scheduling of an order to match the delivery date stated in the order (C). With this setting, orders will be scheduled without searching for an alternative delivery date, no matter if capacities are available or not. This can result in frequent residue from the previous day. Real scheduling will hardly be possible in this case.

> **Info: Change settings**
> If you have changed settings in the company data, you should restart A+W Business Pro.

## Schedule Order

Orders are usually capacity-scheduled by a work flow task. You can schedule all orders of a number manager or every single order manually.

The steps below describe the manual scheduling of a single order. The following session will tell you how to solve possibly occurring scheduling problems.
⇨ "Solve Capacity Problem" on page H-126

> **Info: Scheduling impossible**
> The order cannot be scheduled if it is being processed by another user and therefore open in Documents module at the time.
> To schedule capacities beyond the turn of the year, you have to enter the calendar for the new year including all shift times.

> **Info: Reschedule an order**
> To schedule an order once more, you have to delete the old scheduling first. This applies especially if the order has been manually reported complete by mistake, and therefore has to be rescheduled.

This includes the following training sessions:
*   "How to schedule an order” on page H-120
*   "How to schedule an individual order item" on page H-124
*   "How to delete an order from capacity planning" on page H-125

### How to schedule an order

1.  Select `Production > Capacity planning > Schedule > Schedule order`. The `Schedule order` dialog is described in the Software Reference.
2.  Enter the order number and press the `<Tab>` key. The order is loaded.
3.  Select on the menu `Functions > Group settings > Date search` to check the criteria for the scheduling. In the "Change criteria" dialog, you can set options like:
    *   Determine the production date (e.g., Automatically normal capacity)
    *   Mode for aligning the machines (e.g., Automatic, Manual)
    *   Other options (Closing time, Reduced control, Do not split orders)
4.  In this example, the following settings are selected so that the scheduling can be traced step by step:
    *   Automatic normal capacity for the determination of the production date.
    *   Manual for the selection of the machines.
5.  Click [OK] to apply the settings and close the dialog.
6.  **Schedule order manually**: In the `Book order` dialog, you can specify scheduling options:
    *   **(A) Also use priority -1**: Considers machines with priority -1 (manual selection) in the search for free capacities. This makes sense for urgent orders.
    *   **(B) Keep delivery date**: If ticked, the delivery date from the order must be adhered to. If unticked, the date may be changed according to free capacities.
    *   **(C) Earliest start of production**: Specify a date if the order should not be produced until later.
    *   **(D) Priority**: The priority from the order (e.g., Normal).
7.  Check whether the priority from the order (D) should be adopted or changed. If you change the setting, the new priority will only be adopted and written back to the order if you have confirmed the change in `Functions menu > Apply priority to order`. The change of the priority only makes sense if the appropriate transition times for all priorities are set up.
8.  Select in the menu `Start > Execute` to start the scheduling.
    If there are bottlenecks during scheduling, the following dialogs are displayed:
    *   Delivery date
    *   Machine selection in case of bottleneck
    The procedure for resolving bottlenecks will be described in the following sequences.
    During scheduling, it is displayed which item or sub-item is scheduled with which work type.
9.  For large quantities, the scheduling runs through several phases until an optimal result has been achieved. Thus the order is completely scheduled. You can have the result displayed by selecting `Functions > Scheduling result`.

**Result of the scheduling**

| It... | Machine | Work type | Time | Product/Processing | Pcs. | Date | Shift | Costs |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | Zuschnitt/Cutting | Zuschnitt / Cutting | 0.600000 | Float 5 mm A+W | 100 | 10.04.2014 | 1 | 54.00 |
| 1 | Zuschnitt/Cutting | Zuschnitt / Cutting | 0.600000 | Therm 6 mm A+W | 100 | 10.04.2014 | 1 | 54.00 |
| 1 | Forvet A+W | Kantenbearbeitungen/Edge processings | 11.600000 | Rundecken/Rounded corn... | 400 | 10.04.2014 | 1 | 1740.00 |
| 1 | Rahmenbieger/... | Rahmen biegen / Spacer bender | 0.100000 | Spacer 14 mm ALU A+W | 100 | 10.04.2014 | 1 | 10.00 |
| 1 | ISO Linie/IG Line | ISO-Fertigung/IG-Production | 2.500000 | IG 5/14/Th6 A+W | 100 | 10.04.2014 | 1 | 437.50 |
| 1 | Versand/Shipping | Versand/Shipping | 1.510000 | IG 5/14/Th6 A+W | 100 | 10.04.2014 | 1 | 151.00 |
| **Totals** | | | **16.91** | | | | | **2,446.50** |

### How to schedule an individual order item

If an order item has subsequently been changed, it can be scheduled separately. The other items of the order remain scheduled unchanged.

1.  Select `Production > Capacity planning > Book > Book order`.
2.  Enter the order number and press the `<Tab>` key. The order is loaded.
3.  Check the shipping date and correct it if necessary.
4.  Tick the `Schedule individual item` checkbox (A). The field for the number of the item is released.
5.  Enter the number of the item (B).
6.  Select in the menu `Start > Execute` to schedule the item.
    In case of bottlenecks please stick to the following instructions for the complete order.
    ⇨ "Capacity Problems" on page H-114

### How to delete an order from capacity planning

1.  Select `Production > Capacity planning > Book > Book order`.
2.  Enter the order number and press the `<Tab>` key. The order is loaded.
3.  Select from the menu `Functions > Delete scheduling`.
    The scheduling data will be deleted. You can schedule the order once more now.
    This function also serves to delete orders from capacity planning which have already been reported complete.

### Solve Capacity Problem

> **Info**
> If orders are scheduled automatically, intervention will be necessary only in case of capacity problems - and only provided that the appropriate settings were made in the company data.
> The following examples describe problems which can occur in connection with automatic scheduling or in connection with scheduling several orders from a number manager.

**Split item**
If you want to split an order item on all accounts, you have to schedule the order manually and choose the option `Manual` in the dialog `Search date`.

This includes the following training sessions:
*   "How to resolve bottlenecks when scheduling" on page H-126
*   "How to split an item" on page H-127

#### How to resolve bottlenecks when scheduling

The `Machine selection in case of bottleneck` dialog is displayed if the current item cannot be scheduled.

1.  Check which item (A) on which machine (B) cannot be scheduled.
    The dialog shows:
    *   **(A) Item to be scheduled**: `Rundecken/Rounded corner A`, Quantity `100`.
    *   **(B) Machines where the bottleneck occurs**: `Forvet A+W`. Machine with priority -1 is marked in color.
    *   **(C) Time required for the current item**: `11.6` hours.
    *   **(D) Schedule item**: Button to confirm scheduling.
    *   **(E) Shift time of the machine is exceeded**: `Time required` (11.6) > `Maximum time` (8).
2.  Check whether the scheduling for the date displayed is possible in another shift or on another machine. Using the arrow buttons, you can select another shift or another date. If no suitable capacities are found, you will have to split the item, i.e. divide it into several sub-items. This process is described below.
    ⇨ "How to split an item" on page H-127
3.  Click `[Schedule]` (D) to schedule the item with the changed defaults. The items are scheduled and the process is repeated for the previous machine.
4.  Repeat the steps until no more bottlenecks are displayed. The scheduling of the order is confirmed with a message.

#### How to split an item

The `Machine selection in case of bottleneck` dialog is displayed if the current item cannot be scheduled.

1.  Click `[Split item]` (C).
    The dialog shows:
    *   **(A) Item to be scheduled**
    *   **(B) Machine where the bottleneck occurs**
    *   **(C) Split item** button
    *   **(D) Time required for the current item**
    *   **(E) Shift time of the machine is exceeded**
    This indicates that the required time does not fit in one shift.
2.  The `Split items` dialog opens. On this dialog, you specify how the item is to be split. For this, you have the following possibilities:
    *   You specify the quantity that can be produced without a problem on all machines.
    *   You specify in how many shifts the total quantity should be produced. The quantities for appropriate sub-items are then calculated automatically. This version will be demonstrated in the following steps.
    *   You have the item split automatically by not specifying the quantity.
        *   With `[Qty = Shifts]` the quantity will be distributed evenly across the possible shifts.
        *   With `[Qty = units per shift]` the quantity will be divided up evenly so that the first shift is filled and the remaining quantity is produced in the following shift.
        For both variants, the split is only calculated for the machine on which the scheduling has come to a standstill.
    If you are not satisfied with the suggested split, you can delete the defaults and have the split calculated with new values.
3.  Click on the `[Overview]` button (D) to check where additional bottlenecks may occur. Based on this list you can determine the maximum size of the sub-items to prevent bottlenecks at all the machines. When you have closed the dialog you can enter the number of sub-items.
4.  Specify the quantity (B), e.g. 3. This value should relate to shifts.
5.  Click `[Quantity = Shifts]`.
6.  The dialog now shows the quantity and size of the sub-items. You can specify an individual production date (C) for each item.
    *   **(A) Enter quantity**
    *   **(B) Apply quantity for shifts**
    *   **(C) Specify production date** checkbox
    *   **(D) Enter production date, shift** for each sub-item
7.  Tick the checkbox (C) and enter the date and shift (D) for all sub-items.
8.  Click `[OK]` to confirm the splitting and close the dialog with `[End]`. The order item is split according to your instructions.
9.  The `Machine selection in case of bottleneck` dialog is displayed again. Then the scheduling for each of the sub-items begins again with shipping.
10. Click `[Schedule]` to schedule the sub-items. Scheduling continues and is interrupted when the next bottleneck is encountered. Please note that the sub-items will be scheduled now and that it may be necessary to split them again in case of further bottlenecks.
11. Repeat the steps 4 to 7 until no more bottlenecks are displayed. When you have split the sub-items so that no more bottlenecks occur, scheduling is completed.

### Exercises

Use the orders you have entered in this exercise to check the settings you have made in capacity planning master data. It will therefore be useful if you enter as many complex orders as possible.

*   **Enter several orders:**
    *   Cutting of large quantities of single glass.
    *   Several items with identical bills of materials but with different sizes.
    *   Items with complex work steps, e.g. a shape as part of a stepped IG unit.
*   **Schedule the orders manually**, using different modes (settings in the `Mode Search Dates` dialog):
    *   Automatically
    *   Manually
    *   Schedule w/o checking
    Check the differences based on the scheduling result.

> **Info: Schedule an order several times**
> You can schedule any order several times if no items have been produced yet. Delete the old scheduling result in this example before scheduling the order again but under different conditions.

**Additional information**
⇨ Software Reference, "Default Settings in Company Data" on page H-179
⇨ Software Reference, "Schedule Number Manager" on page H-269
⇨ Software Reference, "Change Criteria (Search Date)" on page H-272
⇨ Software Reference, "Delivery Date" on page H-274
⇨ Software Reference, "Book Order" on page H-275
⇨ Software Reference, "Machine Selection in Case of Bottleneck" on page H-281
⇨ Software Reference, "Split Items" on page H-284

## Production

**Objectives**
*   Set up reports from production.
*   Set up registration points.
*   Check status reports in the order.
*   Manually report orders completed.
*   Reschedule residual quantities from the previous day.

**Benefits**
*   The shop floor sends reports on the current status of the order items and thus, the order. The team in the sales department can check whether the delivery date of the order can be kept.
*   Delays due to breakage or production bottlenecks become evident based on the reports.

**Note**

| Term | Description |
| :--- | :--- |
| **Reports** | Production reports in A+W Business Pro serve to provide information on the production progress. The reports update the status of items and orders. |
| **Status reports from production** | The status of every single item changes during production. When all items of an order have reached the same status, the order status is changed too. |
| **Completion report** | To report an order complete, the registration point from which A+W Business Pro expects the report, must be defined and allocated in company data. |
| **Manual status allocation** | Every (omitted) status report can be manually made up for. If reports have been omitted at several machines, they will all be reported complete with the newest reported date. |
| **Default settings** | **Master data:**<br>- Registration points<br>**Company data:**<br>- Stock/EK/EDI tab<br>- Production tab<br>- Capacity planning tab |

### Reports about Production Status

Production reports in A+W Business Pro serve to provide information on the production progress. The reports update the status of items and orders.

If you are using the production software A+W Production, orders can be transferred to production after capacity planning. There is at least one registration point per production area on the shop floor. These registration points can report items or partial quantities to A+W Business Pro to change their status.

The order status can be changed in the following ways:

*   If you do not use A+W Production shop floor data collection (barcoding), you can manually report order items and orders complete.
*   If you are using A+W Production barcoding, completion reports are sent to capacity planning and will raise the status of the order items. When all items have the same status, the order status is raised in the order header. Status reports are shown in the `Report list` dialog. This gives you a constantly updated overview of an order's production progress or of the present day.

A process that is reported complete by A+W Production or manually, is fixed and cannot be changed in capacity planning. When the entire order has been reported complete, it appears in capacity statistics.

Reports are created by A+W Production and loaded by the A+W Business Pro interface service (AIS). This program runs centrally on the server and checks the defined directories periodically for new items.

> **Info: Reports from production**
> Reports from A+W Production can be received and edited by A+W Business Pro in different ways. This subject is described in detail in the section Production. In the tutorial on capacity planning, it will be explained only briefly.
> File-less reporting can only be processed with A+W Production Capacity Planner.

### Settings for reports

In the company data, you must check the settings for the production reporting.

The screenshot of the `Company Data -> Production` tab shows several settings:
*   **(A) Use production manager**: The program version A+W Business Pro works with the production manager (A) by default. Thus file-less reports are not possible.
*   **(B) Settings for production reports**: Specific settings for reporting.
*   **(C) File-less report and online production overview**: Enables file-less reporting.
*   **(D) URL for the PPS Webservice**: e.g., `http://localhost/Albwir.Alcim.DataService`
*   **(E) URL for the ERP Webservice**: e.g., `http://localhost/Albwir.Erp.Webservice.2012`. The URL of the ERP-Webservice is valid for transfer to production and for production reports in OrderXML format. These settings are described in detail in the Production tutorial.

⇨ Production: Tutorial, "Reports from Production" on page E-55

### Registration Points

Completion of work steps in a production area is reported through barcode registration points. One registration point per production area will usually do. You can however set up two registration points in a production area.

> **Example: TG dispatch**
> One registration point is set up where the finished sheets are loaded onto racks, and one in the fittings stock where the fittings are arranged.
>
> Only when all items (glass as well as fittings) have the same status, e.g. 540, the order is ready for dispatch and the order status is set to `Goods shipped`.

Production reports from barcoding are expected, e.g. from the following stations:

| Barcoding status | Meaning |
| :--- | :--- |
| 455 | Break in production |
| 460 | Cutting finished |
| 465 | Grinding finished |
| 470 | Drilling finished |
| 475 | Check |
| 480 | Screen printing finished |
| 485 | TG finished |
| 490 | LG finished |
| 495 | Bending finished |
| 500 | Heat-soak furnace finished |
| 510 | IG finished |
| 515 | Clear Shield finished |
| 540 | Ready for shipping |

Details on the current state of an order's and the items' production are provided in the `Report list` dialog. It shows the production areas every item has passed so far, and those it still needs to pass.

When an item has passed a production area and has been scanned at the registration point, its status is raised. When all work steps in a production area have been completed for all items of an order, the order status is raised automatically. Since the processing machines are not going to be changed at that point, the costs will be recalculated and saved in the order.

#### Registration point for reports

To analyze the reports from A+W Production in A+W Business Pro you have to allocate a registration point for the completion report. This allocation will be required for production reports and barcode reports.

In the `Master Data -> Stock/PCH/EDI` tab, under `Reg. point allocation` (A), you must set the registration point for when an order is considered produced (e.g., `0700 - produziert`).

If AWBar or A+W Production reports are sent to the files of the types STSP, STSL, STSD, STSB, STSG, you have to select a registration point that is allocated to a status point. If no such registration point has been allocated, the report will cause an error.

### Status Messages

In capacity planning, status reports have to be allocated to the production areas in which they are supposed to raise the item or order status. You can only allocate one status per production area.
⇨ Software Reference, "Production Area" on page H-195

#### Item and order status

The order status changes after an order has been scheduled in capacity planning. This change is recorded in the order history.

Status allocation is different for items and orders. When an item is complete, its status changes to `ready for dispatch`, the order itself however is not ready for dispatch yet.

In the `Report list` overview, you can see the status of the order (A) and the status of individual items (B). The order status is raised only when all order items have reached the status `ready for dispatch`.

#### Automatic status allocation in connection with different work types

Items of an order can be quite different so that they undergo different work types before reaching a common item status.

> **Example**
> Only one of five items has to pass the production area Toughening furnace. If this is the only item that needs to be reported complete in this production area for this order, the status in the order header would normally be raised automatically when this item is reported complete at the toughening furnace.
>
> This must not happen however, as long as the other order items have not reached the same production status. These may still be in the Cutting area, for example, and have to pass the production area Drilling before the order status can be raised to `Toughening furnace`.
>
> Capacity planning therefore checks which production area has to be passed by the four items before they reach the toughening furnace, in this case the production area Drilling. Only when the four items have been reported complete in the production area Drilling, the order status is raised to `Toughening furnace`.

#### Manual status allocation

It may happen that registration points do not register the completion reports for items so that the status is not raised for the time being. When the item is reported completed by one of the following production areas however, capacity planning (not A+W Production) automatically assumes that the previous production area has been passed. The status will be raised automatically.

> **Example**
> Let us assume that the items have been reported complete by production area Drilling. Cutting always precedes drilling. If the item has not been reported complete in the cutting area, capacity planning still assumes that it has been cut and automatically raises the status for production area Cutting.
>
> Registration point Drilling however has no data on the cutting table used. The data for the start of production are missing as well. In this case, the data and costs are only updated for production area Drilling, not for the Cutting area. This is why completion reports should be duly made at the registration points.

### Completion Report

Orders and items are reported complete by reports from the shop floor.

A completion report always assumes that the previous process has been completed. If the appropriate completion report has been omitted, it will be made automatically. The program adopts the date of the latest completion report for the last area for which this report is missing. Logically, this date does not match the date on which the item was actually produced in that area.

If you are not using the (automatic) reports from shop floor data collection (barcoding), you can issue manual completion reports for orders or items for the different production areas, e.g. by batch, by date, or by order.

When reporting `cutting` complete manually, the `Control station` dialog data will be updated accordingly. When an order is reported complete manually, all work steps that have not yet been reported will be moved to the day of the completion report. In this case, the production dates are shown in green on the Control Station.

The `Control station` dialog is covered in detail in a separate section.

### Remaining Quantities from Previous Day

When an order has been scheduled for the previous day but was not produced, this residue must be rescheduled for the present day. A batch program (work flow task) searches for orders that have not been started yet and reschedules them. Since this process requires quite a lot of processor capacity, the batch is defined as a work flow task and is automatically run outside working hours, e.g. after midnight. For details on the work flow task please see:
⇨ "Automatic scheduling" on page H-113

Using status settings, the program searches for orders that should have been produced the day before. It checks whether production has already begun. The resulting orders will be rescheduled without a capacity check.

> **Example workday 07/22**
>
> **Order A:** 100 pcs, production start 07/21,
> on 07/21 20 sheets are cut.
> These items will not be taken into account: Work has already begun and the worker will resume it today (07/22).
>
> **Order B:** 30 pcs, production start 07/21.
> No sheet has been cut.
> The batch runs at 4:00 a.m. and reschedules the order for 07/22 (today).

The status settings for the search for orders are usually made just once. In the `Residue transfer` dialog, you set the maximum order status for the transfer (e.g., `050-Übergabe ZW/Transfer to CAPA`).

As a minimum status, the order must have been (successfully) scheduled in capacity planning. You cannot reschedule orders that have not been scheduled yet.

The maximum status (lock status) depends on your production organisation. If you print delivery notes only after an order has been reported complete, this print status could be the upper limit for the search. If you are using barcode reports, the lock status could also be roughly scheduled.

> **Info: Catching up**
> If you realize that the scheduling of residue from the day before results in always new and ever increasing residue, you can aim at a lower use of capacity when planning the next shifts. This will create a buffer for the rescheduled orders. Alternative remedies could be overtime, special shifts, or spending an entire day just catching up on those old orders.

### Breakage Report

Production reports also include breakage reports. Examples of breakage reports are:

*   Sheets broken after passing a registration point.
*   Sheets with flaws that have to be reproduced.

A+W Business Pro can consider breakage reports for status allocation only if a registration point has been allocated in A+W Business Pro master data.
⇨ Master Data, "Registration Points Production" on page B-854

> **Info: Completion report before breakage report**
> When a unit reaches the next production area, it has usually been reported complete at the previous registration point. The breakage report can be entered right away in that case.
> Please note that before a manual breakage report is made, a completion report must be issued. If this is missing, the unit must be reported complete first before the breakage report can be entered.

### Print Production Papers

The program can analyze which quantity of an order has to be produced by a certain machine, and when the order is expected to reach the next machine.

#### How to print a list of the orders on a particular machine

1.  Select `Production > Capacity planning > Completion report > Manual`. The `Production lists` dialog opens.
2.  In the `from date` and `to date` fields (A), enter the period of time for which you want to generate the list. If you enter the same date in both fields, the list will be drawn up just for that day.
3.  Tick the checkbox for the `print settings` (B) to list all machines. To draw up the list for just one machine, select this machine (C). If you change the settings after drawing up the list, you have to tick the checkbox `Reprint`.
4.  Select in the menu `Start > Search` to start the search.

A detailed list is generated. For every work type, this list shows the sub-items of each item. If you send the data to a printer, choose horizontal format to make sure that all data are visible. An example printed report is shown below. One page is created per machine and day.

**Production documents: Zuschnitt / Cutting (01.04.2014 to 10.04.2014)**

| Date | Order | Item | Product | Mod. | Element | Processing | Quantity | Next processing |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **04.04.2014** | 20349 | 2 | Float 3 mm A+W+0.76 Vin | 1800 x 2200 | Float 3 mm A+W | Zuschnitt/Cutting | 800 | VSG-Fertigung/LG Vorverbund/Pre la 07.04.2014 |
| **07.04.2014** | 20349 | 2 | Float 3 mm A+W+0.76 Vin | 1800 x 2200 | Float 3 mm A+W | Zuschnitt/Cutting | 800 | VSG-Fertigung/LG Vorverbund/Pre la 07.04.2014 |
| **08.04.2014** | 20349 | 1 | Float 3 mm A+W+0.76 Vin | 1200 x 1800 | Float 3 mm A+W | Zuschnitt/Cutting | 800 | VSG-Fertigung/LG Vorverbund/Prela 08.04.2014 |
| **10.04.2014** | 20351 | 1 | Float 5 mm A+W+Spacer 1 | 1200 x 1800 | Float 5 mm A+W | Zuschnitt/Cutting | 100 | ISO-Fertigung/IG-P ISO Linie/IG Line 10.04.2014 |
| | 20351 | 1 | Float 5 mm A+W+Spacer 1 | 1200 x 1800 | Therm 6 mm A+W | Zuschnitt/Cutting | 100 | ISO-Fertigung/IG-P ISO Linie/IG Line 10.04.2014 |
| **07.04.2014** | 20352 | 1 | IG 5/12/Th6 A+W | 1200 x 1800 | Float 5 mm A+W | Zuschnitt/Cutting | 10 | ISO-Fertigung/IG-P ISO Linie/IG Line 07.04.2014 |

### Report manually Order completed

The options for manual completion reports are:
*   Complete orders
*   Individual order items
*   Sub-quantity of an order item

In the following example, a sub-quantity is reported complete.

> **Info: Scanning**
> If you are using a scanner please first go to menu `Options` and check whether barcode registration is active. If so, the cursor is automatically positioned in the barcode field.

#### How to report an order completed on a machine

1.  Select `Production > Capacity planning > Completion report > Manual`. The `Manual completion reports` dialog opens.
2.  Select in the menu `Functions > Settings`. Select the machines for which you want to record the completion reports and apply the selection with [OK]. You can select several machines.
3.  Check whether the `Completion report` option (A) is activated.
4.  Specify the order number (C) or record the barcode. The cursor goes to the next field.
5.  In the `from item` field (D), enter the item number and press the `<Tab>` key. The item is loaded and the quantity displayed.
6.  Tick the `With quantity` checkbox (F). If you have scanned the barcode, just one sheet will be reported complete. You have to tick the checkbox and enter the number of completed sheets. To report the entire item complete, tick the checkbox `Item complete`. You do not have to enter the quantity in that case.
7.  Go to the `Quantity` field (E) and enter the quantity to be reported completed.
8.  Go to the `Select machine` field (G) and choose the machine where the quantity was completed.
9.  If necessary, add the date and the shift.
10. Click `[Report items completed (F9)]`. The specified quantity is reported completed.

### Manual Breakage Report

Breakage reports can be made only for items which have already been reported complete. The options for manual breakage reports are:

*   **Breakage report - entry:** The defined quantities are reported broken at the machine entry. They have to be reproduced by the previous machine.
*   **Breakage report - exit:** The defined quantities are reported broken at the machine exit. They have to be reproduced by the same machine.

#### How to report breakage of an item

1.  Select `Production > Capacity planning > Completion report > Manual`. The `Manual completion reports` dialog opens.
2.  If necessary, select in the menu `Functions > Settings` the machine for which you want to record breakage reports.
3.  Enter the order number (B) or record the barcode.
4.  Enter the item number (C) and press the `<Tab>` key. The item is loaded and the quantity is displayed.
5.  Select the report type (A). This setting defines whether the defective sheets have to be reproduced by the previous or the same machine.
6.  In the `Quantity` field (D), enter the quantity that you want to report. If you have recorded the barcode via scanner, precisely 1 sheet is reported complete.
7.  In the `Select machine` field (F), mark the machine on which the breakage should be reported.
8.  If necessary, add the date and the shift.
9.  Click `[Report items completed (F9)]`.

The data are saved. The confirmation is displayed below the button. When the rejected sheets have been re-produced, the item status is increased.

> **Info: Breakage report cannot be confirmed**
> If the breakage report cannot be confirmed, you have to report the item complete first. After the completion report has been made, you can enter the breakage report.

### Check Production Status

You can check the production status of the orders in detail and add any omitted completion reports. To this end, you can view the orders for a customer or all orders for a certain delivery date.

#### How to check the production status of individual order items

1.  Select `Production > Capacity planning > Production status`.
2.  Enter the number of the order or the customer. You can enter the delivery date to restrict the selection even more. Alternatively, you can use this to view all orders for the defined date.
3.  Select in the menu `Start > Search` to load the data. The order data are loaded and displayed on the `Selection` tab.
4.  Change to the `Items` tab to check the production status of the individual order items.
5.  Check the date for which you want to report the item completed.
6.  Tick the `Report completed` checkbox (C) for the item that has already been completely produced. A security message is displayed. When you have confirmed the message, the quantity of the item is displayed in the `Completely finished` column.

### Catch up on Completion Reports

You can view the residue from the day before to check if completion reports have been omitted.

#### How to check if there is residue from the day before

1.  Select `Production > Capacity planning > Control station > Functions menu > Display residual quantities`.
2.  Select the minimum status (A). The orders have to be at least scheduled in capacity planning. Therefore, a lower status does not make sense.
3.  Tick the `Completion report` checkbox (B) for the orders to be marked as completed.
4.  Click `[OK]` to save the data. The status of the orders is increased. The orders reported completed are deleted from the overview.
5.  On the `Control station (order)` dialog, you can check if the data were amended correctly. All additional completion reports are set for the present date.

> **Info: Show completed orders**
> When making the settings for the control station you can define that orders which have been reported complete are not to be displayed. If you choose this option, you will not be able to check the status change as shown in this example.

### Exercises

*   Report completion of one of your orders manually.
*   Report an item completed in one of your orders.
*   Record breakage for one IG sheet. Consider thereby that the item or the order must be reported completed beforehand.
*   Report the residual quantities from the previous day completed. You can only do this exercise if there are residual quantities.

**Additional information**
*   Software Reference, "Production Area" on page H-195
*   Software Reference, "Residue Transfer" on page H-290
*   Software Reference, "Date" on page H-292
*   Software Reference, "Manual Completion Report" on page H-298
*   Software Reference, “Production Level Orders" on page H-307
*   Software Reference, "Report List" on page H-318
*   Software Reference, "Utilisation (Date)" on page H-351
*   Software Reference, "Residue Qty." on page H-361

## Production Costs

**Objectives**
*   Checking machine and time costs in the order or quotation.

**Benefits**
*   Even before an order is produced, you can check whether the time and machine costs are sufficiently taken into account for pricing.

**Note**

| Term | Description |
| :--- | :--- |
| **Production costs** | These are:<br>- Wage costs per unit<br>- Machine costs per hour<br>- Variable costs per hour, e.g. for insurances<br>These costs are stored per machine and checked during scheduling. |
| **Production in a quotation** | To determine the production costs for a quotation, a work flow task must be defined which transfers the quotations to capacity planning. |
| **Actual costs** | The actual costs are not determined until production, because only then it is decided which machines have actually been used. The actual costs are written back to the order with the reports. |

### Time Costs

The program calculates the time costs for orders and - if required - for quotations. This way you can check before production whether the order can still be produced at a profit considering the expected time costs.

Production cost calculation is based on the following details:
*   Machine costs per hour
*   Variable costs per hour, e.g. insurance costs
*   Costs per unit of default time, e.g. labour costs per unit

These costs are defined per machine and are checked at scheduling. The machine settings dialog shows the cost records (A) which compile to the total costs per unit produced (B).

The cost of an order item and for the entire order will be recalculated after the completion report. They can differ from the originally calculated costs, e.g. because the order or item was produced by another machine than the scheduled one.

On the `Order production status` dialog, you can display the current production costs, showing planned production costs for the whole order (A) and the production costs incurred so far (B).

### Cost Centres

You can define special cost centres for analyzing the production costs. This way, you can analyze the costs for a defined period.

The "Statistics by Order Area" dialog allows for evaluation of cost centres for production costs. You can sort by cost centre or order area, and list by product types, product classes, or products.

This analysis lists the cost centres for product types. You can sort this analysis by cost centre or by order area.

Cost centres and analysis can be defined according to your company's requirements.

> **Info: Cost centres in A+W Business Pro master data**
> Capacity planning cost centres are not connected with the cost centres defined in module `Master data`.

#### Principle of the evaluation columns

In the `Cost centre definition` dialog, you specify what the query shall evaluate in each column.

*   **(A) Main product type (MPT)**: number of the product type from the A+W Business Pro master data
*   **(B) No 1, No 2**: Number of the product class or product type in the Type field
*   **(C) Type 1, Type 2**:
    *   0 = Not specified
    *   1 = Product type
    *   2 = Product class
*   **(D) Priority**: Sequence of the query
*   **(E) Exclusion**: Products that are excluded from the evaluation

With the combination of the columns `No` and `Type` you set what shall be searched for in the BOM.

**Example: evaluation of processed TG**

| MPT | No 1 | No 2 | Type 1 | Type 2 | Priority |
| :-- | :--- | :--- | :--- | :--- | :--- |
| 2 (TG) | 20 (Processings) | 0 | 1 (Product type) | 0 | 19 |

This example shows that the main product of product type TG (2) shall be searched for Type1 (i.e. `Product type`) number 20 (`Processing`). This means that this cost centre shall include only TG with processings.

Before you start entering cost centres, you should decide in which sequence the cost centres are going to be checked. This sequence is defined in the column `Priority`.

> **Example TG**
> First you check whether this is a TG with processing (cost centre no. 7 with prio 19).
>
> If this is not the case, the next check is applied, that is prio 20.
>
> The TG that is not processed automatically goes into the cost centre TG (cost centre no. 6 with prio 20).

The column `Exclusion` can be used to exclude a product from this rule by entering the product number. The product number must be entered in brackets.

> **Example**
> All TG sheets are seamed. Therefore, you do not want seamed TG sheets to flow into the cost centre `TG with processing`.
> You can exclude this by entering the product number for seaming.

A detailed description on the definition of columns is found in the Production part. There, the definition of the preview columns is described, which follows the same principle.
⇨ Production, "The concept of preview columns" on page E-153

### Cost Calculation in Orders

A+W Business Pro calculates the material prices based on the purchase price. Apart from that, time and machine costs can be displayed in the order.

These costs are calculated per order in capacity planning at scheduling and shown in the order.

Material and time costs are shown in the order header on the `Totals` tab.

The costs are also displayed in the order header via the `Functions menu > Documents group > Cost and surcharge calculation`.

### Cost calculation for Quotations

Quotations can be transferred to capacity planning with a special work flow task for cost calculation. This function permits to display the costs in the order header and at item entry just like in the order. Quotations will not be scheduled in capacity planning, and are not transferred to production.

### Exercises

*   Check whether the machinery costs are shown in the orders you have transferred to capacity planning.
    If costs are missing: Check whether you have entered the costs for the machines. Add them if necessary and schedule the orders again. Then check if the costs are displayed.

**Additional information**
⇨ Software Reference, "Accounts" on page H-264
⇨ Software Reference, "Cost Centre Definitions" on page H-265

## Control Station

**Objectives**
*   Navigation on the Control station dialog.
*   Check utilization of the machines.
*   Reschedule orders or order items.

**Benefits**
*   On the Control station dialog, you get an overview of the utilization of the machines.
*   You can use this dialog to access all programs for checking and rescheduling the orders.

**Note**
*   **Control station**: From the Control station dialog you can load all dialogs for checking and rescheduling.

### Concept of the Control Station

The `Control station` dialog provides an overview of the hours scheduled per machine and allows to change dates if required.

The interface displays several layers of information:
*   **(A) Production Areas**: Shows the scheduled time for a whole production area (e.g., `Cutting`) for a given week.
*   **(B) Machines**: Drills down into the machines within a production area, showing their individual scheduled times.
*   **(C) Orders**: Drills down further to show the specific orders to be processed by a selected machine.

This example shows the utilization of production area `Cutting` (A) for one week. The detailed data for the individual machines in production area `Cutting` (B) and the orders (C) to be produced by a certain machine can be displayed in the Control station dialog.

### Navigation

The `Control station` dialog gives access to all programs for checking and rescheduling orders. These are the following dialogs:

*   **Using the Functions menu:**
    *   `Select order > Control station (order)`
    *   `Display residual quantities > Residual quantities`
    *   `Graphic display of the utilization`
    *   `Utilization > Utilization on date`
*   **Using `Control station > Prev.processes` tab:**
    *   `[In Detail] > Production lists`
*   **Using `Control station (order) > Functions` menu:**
    *   `Overview of reports`
    *   `Schedule > Schedule order`
    *   `Manual defaults (Production level orders)`

On the `Control station` dialog, you navigate as follows:

| Tab | Action | Tab / dialog |
| :--- | :--- | :--- |
| **Areas** | Double-click on row header | -> Machines (all machines) |
| | Double-click on production area | -> Machines (only machines in the production area) |
| **Machines** | Double-click on machine | -> Orders |
| | Double-click on detail data | -> Reschedule order |
| | Double-click on row header | -> Control station (machine) |
| **Orders** | Double-click on number | -> Control station (order) |
| | Double-click on detail data | -> Reschedule item |
| **Reschedule order** | Click on row header | -> Reschedule item |
| | Click on [Elements] or [Prev.processes] | -> Prev. processes |
| **Reschedule item** | Context menu for process (right mouse key) | -> Delete setup time, Add setup time |
| **Work types** | Click on row header | -> Details |
| **Details** | Double-click on number | -> Control station (order) |
| **Prev. processes** | Click on [In Detail] | -> Production lists |

### Control Station – Order

To check the scheduling of the individual order, the `Control station (order)` dialog is available. You reach the dialog via `Control station > Functions menu > Select order`.

This example shows the backdating process based on the delivery date (A): On the day before the scheduled shipping date (B), the order must reach the production area `Dispatch` to be packed. All other work is done before, taking into account the production and transition times.

Navigation in the `Control station – Order` dialog:

| Tab | Action | Tab / dialog |
| :--- | :--- | :--- |
| **Machines** | Double-click on machine | -> Move II |
| | Double-click on date | -> Detail |
| **Detail** | Click on cell header | -> Work types |

### Control Station – Machine

To check the utilization of an individual machine, the `Control station (machine)` dialog is available. You reach the dialog via `Control station > Machines tab > Double-click in row header`.

This example shows the orders including quantities and hours required (B) for the selected machine (A). The period shown matches the display in the `Control station` dialog from which you have accessed this dialog.

The next tab shows the detailed times. You can change the displayed period so that you see the utilization e.g. for just one day.

The sub-items generated by a splitting are listed individually. To move a scheduling, you can change with a double-click on the order number to the `Control station (order)` dialog.

### Postpone Scheduling for single Order

You want to check whether the shipping of an order can be postponed, e.g. due to a delay in the delivery of ordered elements. In this example, the shipping of an order shall be postponed by several days. This means that both the delivery date and the scheduling must be changed.

#### How to check the scheduling of an order

1.  Select in the module `Production > Capacity planning > Control station > Functions menu > Select order`. The `Control station – Order` dialog opens.
2.  Enter the order number.
3.  Select in the menu `Start > Search` to load the data. The dialog shows the current delivery date (A) and shipping completion date (B).
4.  Enter the new date in the `Delivery date` field (B).
5.  Click `[Change]`. The display will be updated the next time you open the dialog.
6.  Select in the menu `Functions > Schedule`. The `Book order` dialog opens, showing the new delivery date.
7.  Select in the menu `Start > Execute` to reschedule the order. Scheduling starts. Depending on the setting, you have to confirm the delivery date for the individual items. After successful scheduling you can view the `Scheduling result`.
8.  The result shows that shipping and all previous work steps have been rescheduled to the new dates.
9.  Change back to the `Control station (order)` dialog. To update the display, you must load the order again.
10. Select in the menu `Start > Filter` to change to the search mode.
11. Enter the order number again and start the search to load the order. The dialog now shows the changed plan data.

### Change Machine

You can move scheduled order items to another machine, e.g. from IG line I to IG line II.

#### How to reschedule an order item on another machine

1.  Select `Production > Capacity planning > Control station > Functions menu > Select order`.
2.  Enter the order number and start the search. The order data are loaded.
3.  Double-click on the machine to open the control station for the machine. The `Control station (machine)` dialog is displayed with the `Move II` tab.
4.  Tick the checkbox for the item that is to be moved to another machine.
5.  In the `Move` group, select another machine. In addition, you can enter a new date and/or another shift.
6.  With `[Load]` you can check whether the move makes sense.
7.  Select in the menu `Start > Execute` to start the action. The scheduling is moved. The change will be displayed after a restart of the dialog.

### Exercises

*   **Practice navigation on the control station:**
    *   Starting point for the following exercises is always the control station. Close the dialog to execute the next exercise.
    *   Have the machines for a production area displayed.
    *   Change to the `Control station (machine)` dialog.
    *   Change to the `Control station (order)` dialog.
    *   Have the data displayed on the `Detail` tab.

> **Info: Tip for practicing navigation**
> Print out the overview of the navigation. You will also find this in the software reference.
> ⇨ "Navigation through the tabs and dialogs" on page H-307

*   Change from the control station to an order and check the scheduling.
*   Move the delivery date of an order by one week. What else do you have to do? When are the new dates displayed?
*   Schedule an order with 10 large IG sheets so that only one unit per day is produced (item split and specification of production date).

**Additional information**
*   Software Reference, "Control Station (Dialog)" on page H-326
*   Software Reference, "Control Station (Machine)" on page H-344
*   Software Reference, "Control Station (Order)" on page H-362
*   Software Reference, “Production Level Orders" on page H-307
*   Software Reference, "Change Production Times" on page H-319

# A+W Business Pro Software Reference

## Overview

Capacity planning in A+W Business Pro is organized in two areas:
*   Management of capacity planning
*   Planning and monitoring of capacities

You will find the associated dialogs in the `Capacity planning` and `Production` modules.

In this software reference, the dialogs from both modules are described in the following sections:
*   "Administration" on page H-178
*   "Capacity Planning" on page H-267

## Administration

In order to work with capacity planning in A+W Business Pro, the master data must be set up. These data are the basis for all allocations, scheduling, and analyses.

This section provides information on the following master data:
*   "Default Settings in Company Data” on page H-179
*   "General" on page H-185
*   "Organisation" on page H-194
*   "Default Times" on page H-216

Apart from the description of master data, you will find information on the following subjects:
*   "Allocation" on page H-229
*   "Lock" on page H-246
*   "Overviews" on page H-257
*   "Scheduling" on page H-268
*   "Production Reports" on page H-291
*   "Control Station" on page H-325

### Default Settings in Company Data

`Master data > Company > Company data > Capacity planning` tab

In the `Master data` module, you specify the basic settings for A+W Business Pro Capacity Planning. These settings mainly refer to automatic scheduling. In case of manual scheduling, you can overwrite them.

> **Info: Changing settings**
> If settings were changed in company data and in capacity planning master data, you have to reboot A+W Business Pro to reload the data.

#### Capacity planning

**Version** For the selection of the program for capacity planning, you must pay attention to how you receive reports from production. If you want to work with Capacity Planning of A+W Business Pro, you must select the `A+W Business Capacity Planning` entry. This setting does not permit the use of online reports.

**Error message from automatic capacity planning**
With the selection of the option, you specify to whom error reports are sent.
*   **To operator:** With this setting, the error messages are sent to the employee who had entered the order in question. Such error messages usually refer to dates that cannot be adhered to because there are not enough capacities available. This is the default setting.
*   **To employee:** With this setting, the field for the selection of an employee is released. Select this option if only a single employee processes the orders that cannot be scheduled without problems.

**Schedule orders automatically**
Usually the orders are scheduled in capacity planning automatically at specified intervals by a workflow task. This function is described in the tutorial.

#### A+W Business capacity planning

**Number of shifts** Number of shifts in which you work. You specify the shift hours in the `Capacity planning` module on the `Calendar` dialog.
⇨ "Calendar" on page H-205

**Production scheduling mode** Specification whether you want to work with open or closed capacities.
*   **Autom. normal capacity:** The orders will be scheduled based on the available shift times. Overbooking is impossible. This is the default setting (closed capacities).
*   **Automatic full days:** This setting ignores the specifications for the number of shifts and hours in the calendar. Scheduling is based on a workday of 24 hours in this case (open capacities). This applies only to common workdays, not to holidays.
*   **Change machine only:** If capacities are fully utilized, the program will automatically search for another machine. If this is used to capacity as well, scheduling is interrupted and manual intervention is required.
*   **Schedule without check:** This setting represents an open shift. This means e.g. that despite a shift time of 8 h, 16 h can be scheduled as well. The program will issue no report if a day's capacity is fully utilized. This option should only be used in exceptional cases.

**Fill shift in case of item splitting** Large items can be split to several machines, shifts, or days. For this, you specify up to what percent the shift of a machine may be filled by splitting to keep capacity for other orders.

**Machine alignment** If you work with several machines that can perform the same work types, the planning can consider these machines in different ways:
*   **Automatic:** The program automatically searches for the most cost- and time-effective machine and schedules the orders on this machine. This is the default setting.
*   **Semi-automatic:** The program offers the alternative machines for selection. If the delivery date cannot be adhered to, you must intervene.
*   **Manual:** With this option, every possible change (machine, shift, etc.) requires manual intervention. Alternative machines can only be selected for manual scheduling or rescheduling.

**Scheduling priority** Priorities defined in the order can be taken into account for scheduling:
*   **Standard:** The capacities of the required machines are checked and the orders are scheduled based on the defined priority.
*   **Low priority:** All orders are scheduled with low priority by default.
*   **Adopt changed priority for the order:** If the priority is changed at scheduling, it will be automatically saved in the order.

**Product classes without status change**
You can suppress the increasing of the item status (order status) with completion reports for product classes. Just select the appropriate entries on the list.

**Order areas without scheduling**
You can define that certain order areas shall be excluded from automatic scheduling. This means that orders for the selected order areas can be scheduled manually only.

**Autom. delivery date search by route** In case of bottlenecks, it is possible to search for a new delivery date automatically.
*   The next possible date is selected as delivery date regardless of whether it is a route day or not. This is the default setting.
*   The new delivery date is searched for according to the customer's route days.

**Do not split order** Large orders must be split into smaller items if the work process cannot be performed completely in one day for an order.
*   The orders can be split in automatic scheduling. This is the default setting.
*   The orders can only be split manually. For the automatic scheduling of large orders, a message is displayed so that you can intervene.

**Reduced scheduling check if structure identical** An order may contain items with the same BOM structure, which differ only for the dimensions.
*   The entire BOM structure is checked for each item.
*   With the same BOM structure, the scheduling assumes the previous item without checking the BOM. This is the default setting.

**Schedule for delivery date** For automatic scheduling, orders are scheduled for the delivery date by default. Another delivery date is searched for only, if no capacities are free.
*   Orders are scheduled with delivery date search. This is the default setting.
*   The orders are scheduled without a search for an alternative delivery date, regardless whether or not there are free capacities.

**Autom. completion report for invoiced orders** Currently not used.

**Transfer to production (OrderXML) incl. planning data** For the transfer to production, the data determined from capacity planning can be written into an OrderXML file.
*   The data determined from capacity planning is not written into an OrderXML file.
*   The machine allocation, production date and shift, time costs are written to the transfer file.

**Use change of shifts table** If you work with more than one shift, you can specify when the scheduling changes from one shift to the next.
*   The change of shifts table is not used.
*   The change of shifts table is used. If no shift changes are specified, the `Shift settings` dialog opens.
    ⇨ "Shift Settings" on page H-183

### Shift Settings

`Master data > Company > Company data > Capacity planning` tab > `Use change of shifts table` checkbox

On this dialog, you specify the shift changes and the lock times in which no order can be scheduled.

> **Info: Requirements**
> You must have administrator rights to open the dialog. In addition, the `Use change of shift table` checkbox must be ticked on Company data dialog.
> ⇨ "Use change of shifts table" on page H-182

#### General

The settings in this group are taken over from the company data.
⇨ "A+W Business capacity planning" on page H-180

**Number of shifts** The number of shifts is loaded from company data.

**Alignment mode** Search mode for the machines:
*   **0 = Automatic:** The program automatically searches for the most cost- and time-effective machine and schedules the orders on this machine. This is the default setting.
*   **1 = Semi-automatic:** The program offers the alternative machines for selection. If the delivery date cannot be adhered to, you must intervene.
*   **3 = Manual:** With this option you must intervene manually for each possible change (machine, shift, etc.). Alternative machines can be selected only in manual scheduling or rescheduling.

#### Options

**Correct time tables when saving** If you have changed the values, the times for the scheduled orders can be revised.
*   The new times do not change the currently-scheduled orders.
*   The new times are taken over immediately. All scheduled orders are recalculated.

#### Shift changes

**Shift 1 > Shift 2, ...** Specification when the transition from one shift to the next shift takes place. This setting is important for the calculation of transition times. The number of fields displayed depends on the number of shifts that are specified in the company data.
⇨ "A+W Business capacity planning" on page H-180

#### Locked shift times

**1st, 2nd, ... shift** Specification from which time on the respective shift is locked for new orders.

> **Example: 2nd shift 10:00**
> Up to 17:00, orders can be scheduled in the second shift of the current day. Thus you keep the 2nd shift free so that all scheduled orders can actually be produced and there are no residual quantities.
>
> Orders that are scheduled after 17:00 will be planned for the 3rd shift or the following day.

### General

`Capacity planning > Master data > General`

On these dialogs, you store the data for work processes and machines that are available in production.

This section provides information on the following master data:
*   "Machine Types" on page H-185
*   "Work Types" on page H-187
*   "Allocated Machines" on page H-190
*   "Serial Factors" on page H-191
*   "Transition Times" on page H-192

#### Machine Types

`Capacity planning > Master data > General > Machine Types`

On this dialog, you define the machine types you are using on the shop floor, e.g. cutting tables, drills, edgers, toughening furnaces, etc. First, you have to define the machine types and the restrictions to be checked.

By activating the checkboxes, the appropriate fields on the `Machines` dialog are released.
⇨ "Machines" on page H-196

> **Info: Attention in case of subsequent activation**
> If you tick a checkbox later, you must check all machines that belong to the changed machine type. The newly-released fields are blank by default. This can cause errors during checking.

With a click of the row header, you open the `Allocated machines` dialog.
⇨ "Allocated Machines" on page H-190

*   **No.** User-defined number which serves as an ID for the individual machine types.
*   **Name** Name of the machine type.

**Settings**
The function of each checkbox is described below. A complete description of the function and the individual settings is available on the `Machines` dialog.
⇨ "Machines" on page H-196

*   **Machine type** The selection of the machine type is only available in A+W Business Pro. For this program version, the machine types are fixed. The machine type refers to the concrete machines and the drivers to be used. The specification defines which machine drivers are available on the `Machines > Additional options` dialog. A+W Business Pro can activate the machines with these drivers. In contrast to machine types above, these types cannot be configured.
*   **Dim. check** The dimension restrictions must be checked for this machine type.
*   **Spacer** The spacer restrictions must be checked.
*   **Total thickness** The total thickness of an IG or LG unit must be checked.
*   **Indiv. thickness** The thickness of an individual single glass must be checked.
*   **Weight** The weight of the sheet must be checked.
*   **No. of sheets** The number of sheets of a product (double, triple IG or LG) must be checked.
*   **Area** The area of the sheet must be checked.
*   **Gas** The item must be checked for gas filling.
*   **Edge prot.** The edge protection must be checked for insulated glass.
*   **Shape** The item must be checked for shapes.
*   **Georgian bars** The item must be checked for georgian bars.
*   **Quantity** In the item, the quantity or quantity range must be checked. The definition of the quantity is machine-dependent, e.g.:
    *   Drilling machine = number of drill holes
    *   Grinding machine = number of edges
*   **Aspect** The aspect of the sheet must be checked.
*   **Rotatable** For each glass it must be checked whether it may be rotated.
*   **Drilling diameter** The diameter of drill holes must be checked.
*   **Corner radius** The radius of rounded corners must be checked.
*   **Diagonal** Diagonal between the rollers, e.g. on the conveyor belt in front of the TG furnace must be checked.
*   **Mitre angle** Min. and max. mitre angle for facets must be checked.

#### Work Types

`Capacity planning > Master data > General > Work Types`

On this dialog, you store the work types. These are all activities that require time, e.g., cutting, manual cutting, seaming edges, polishing edges, sawing LG, packaging.

Within a process, several work types can be executed in succession, e.g. cutting and toughening as part of toughened glass production. You have to decide whether you are going to define these steps as individual work types, or if you are going to define the entire work process. Depending on how your production is organized, it may be useful to choose both types.
⇨ Tutorial, "Work Types" on page H-25

> **Info: Scan work types**
> If you are working with barcoding, you must create all work types that can be recorded with the scanner. Only then you can also evaluate the reports for the status.

**Functions menu**
With this menu, you can display an overview of the machines that are allocated to the selected work type.
⇨ "Allocated Machines" on page H-190

*   **No.** User-defined number which serves as an ID for the individual work types. We recommend to enter these numbers in steps of ten to leave space for inserting new work types. This permits to keep similar work types together. Work types should also be numbered in the sequence in which they appear in the production process.
*   **Name** Name of the work type. Even a surcharge which prolongs the cutting of shapes for instance, can be defined as a work type.
*   **Hierarchy** Sequence order number. This field specifies the priority (production sequence) of the individual work types within capacity planning.
    > **Example**
    > Edges have to be ground before holes are drilled.
    > TG pre-bonding after drilling.
    >
    > From this it follows that the hierarchy number for the grinding of edges must be smaller, and that for the laminating pre-compound bigger than the number for drilling.
    Numbers should be allocated in steps of at least 10, better in steps of 50 or 100 to leave enough space for defining new work types.
*   **Only main product** Some work types make sense only for the main product but not for the BOM elements.
    *   This work type can be applied to the main product as well as for the BOM elements.
    *   This work types only applies to the main product; BOM elements cannot be shipped for example.
*   **AWProd no.** Article number from A+W Production. Work types which are ordered from a glass producer but are not specified explicitly in the purchase order, will need an article number from A+W Production, e.g. cutting. In A+W Business Pro, you have to define a product of the product type/class Processing for this article; the article numbers must be the same.
*   **% Limit** By default, capacity planning will schedule an order so that it is produced shortly before the shipping date. This can cause problems in case of large orders. This percentage defines the maximum share of the order in the daily production. Large orders will be split onto several days.
    > **Example**
    > You receive a large order on July 17.
    > The delivery date is September 22.
    >
    > Capacity planning would schedule this order to be produced shortly before the delivery date. Production would be blocked by this order however for four whole days for example. No other order could be scheduled during that time.
    >
    > Since you have time to produce the order distributed across the entire period up to the delivery date, you can define that this work type must not use up more than e.g. 10% of the daily capacity per order item.
    This entry will be taken into account if you activate the `Pos. Control` option. You will find this option on the following dialogs:
    ⇨ "Schedule Number Manager" on page H-269
    ⇨ "Book Order" on page H-275
    ⇨ "Machine Failure" on page H-287
*   **Manual machine selection** If you have several machines that can perform the same work type, you specify a machine with priority 9 in the default times so that it is selected by default. If this machine is used to capacity on a certain date, the program can access one of the other machines.
    *   The order is automatically allocated to another machine. If, however, the production day is changed, you must intervene manually.
    *   If the capacity of a machine is exceeded, you must select another machine manually. The possible alternatives are displayed on a dialog.
*   **Alternative work type** You can allocate an alternative work type to any work type, e.g. for the drilling of special sizes.
    > **Example**
    > You have two work types `Drilling` and `Drill special sizes`.
    > For the work type `Drilling`, the alternative work type `Drilling special sizes` is specified.
    >
    > The standard drilling machine is assigned to the work type `Drilling`. However, it can only drill limited drill diameters. If these dimensions are exceeded, then capacity planning checks whether an alternative work type is entered.
    > If so, the program searches for the allocated machine.

#### Allocated Machines

`Capacity planning > Master data > General > Work Types > Functions menu > Allocated machines`

On this dialog, the machines are listed that are allocated to a machine type or a work type. The info section shows the dialog from which this list has been accessed.

*   **Machine** Name of the allocated machine.
*   **Comment** This column shows whether the work type is analyzed as basic time or as a time surcharge for the allocated machine.
*   **Prio** Priority for selecting this machine for scheduling.
    *   **9**: highest priority (standard machine). These machines are always selected first.
    *   **8 to 1**: decreasing priority. These machines are selected depending on utilization.
    *   **0**: lowest priorities. These machines are only selected if all other (equivalent) machines are used to capacity.
    *   **-1**: for manual scheduling. These machines are selected by automatic scheduling only in case of bottlenecks.
    *   **-2**: only for manual scheduling. These machines are never selected by automatic scheduling. The machine can only be selected manually.
    *   **-3**: is only selected with reporting from the production system when orders have been rescheduled there. In case of rescheduling in capacity planning, only machines with prio >-3 are displayed.

#### Serial Factors

`Capacity planning > Master data > General > Series Factors`

On this dialog, you specify the quantities for which the scheduled times shall be reduced, e.g. because no set-up time is required for grinding or drilling.

You assign the number of the series table to the machine on the `Machines` dialog.
⇨ "Serial tables" on page H-201

**Identification**
*   **Number** The number is assigned automatically when you create a new series table.
*   **Name** Name of the series table. Specify a meaningful name if you create several tables, e.g. for drilling and grinding.

**Serial tables**
*   **From ... qty.** Minimum quantity for applying this factor.
*   **Factor** Factor by which the basic time for the work process shall be multiplied.

> **Example**
>
> | From ... qty. | Factor | Time on the machine |
> | :--- | :--- | :--- |
> | 1 | 1 | 0.10 hr. |
> | 10 | 0.9 | 10 x 0.9 x 0.1 = 0.90 hr. |
> | 50 | 0.7 | 50 x 0.7 x 0.1 = 3.50 hr. |

**Table**
This list shows all serial tables you have defined.

#### Transition Times

`Capacity planning > Master data > General > Transition Times`

On this dialog, you specify the time in shifts that is required to change from one work type to another. For example, after the TG furnace, the sheets must cool off before the next work type can start.
⇨ Tutorial, "Transition Matrix and Transition Times" on page H-64

> **Info: Editing transition times**
> The combo boxes in the table fields are released only if you specify a new transition time. The work types allocated to the transition times cannot be changed once they were saved. If you want to change an assignment, you must recreate it and then delete the invalid assignment.

*   **Order priority** Order priority that is considered for the transition time. You can select one of these priorities:
    *   **Normal:** The transition time applies to all orders which have no special priority. This is the default setting.
    *   **Urgent:** The defined transition time applies to rush orders only. If transition times can be shortened for rush orders, a different transition time must be defined for this combination of work types.
    *   **Extra:** This priority means that the order shall be produced from residue (plates) left over from cutting other orders.
    *   **Release order:** The transition time applies only to orders that are produced on-call.

> **Info: Considering order priority**
> If in addition to the order priority Normal the priority Urgent shall be considered, then an individual transition time must be set up for the respective combination of work types. This applies to all transition times that can be shortened for urgent orders. If these have not been defined, the order will be scheduled with Normal priority.

*   **From work type** Initial work type, e.g. polishing.
*   **To work type** Next work type, e.g. drilling. If you select `<n.e.>`, the transition time applies to all subsequent work types.
*   **Time in shifts** In this field you enter the number of shifts that are required for the change from one work type to the next:
    *   `0` = the next process can take place in the same shift.
    *   `1` = the next process takes place at the earliest in the next shift.
    *   `2` = the next process takes place at the earliest in the shift after the next one.
    > **Example**
    > In your company, you regularly work in 3 shifts, in the heat-soak test, e.g. however only in one shift of 12 hours.
    >
    > If you want to achieve that the next work type always begins on the next day, then you must enter the value 3 in this field. Thus capacity planning calculates the date for the next work type automatically for the next day.
*   **Incl. days off** For the calculation, the days off are considered.
    *   Days off are not considered.
    *   Days off are considered. This means that a TG that comes out of the furnace on Friday can be processed further normally on Monday because the weekend is longer than the transition time.

### Organisation

`Capacity planning > Master data > Organisation`

On these dialogs you specify how capacity planning is organized, e.g. the production areas, machines, shift times.

This section provides information on the following subjects:
*   "Production Area" on page H-195
*   "Machines" on page H-196
*   "Calendar" on page H-205
*   "Transition Matrix" on page H-210
*   "Special Technical Restrictions" on page H-212
*   "Org. Overview" on page H-215

#### Production Area

`Capacity planning > Master data > Organisation > Production area`

On this dialog you define the production areas, e.g. cutting, grinding, drilling. At the same time you define which statuses shall be reported by the individual production areas when the item is reported completed.
⇨ Tutorial, “Production Areas (Work Centers)" on page H-27

*   **No.** Freely-definable number that serves as ID for the individual production areas. The numbering does not represent a hierarchy.
    > **Info: Production area <n.e.>**
    > The production area No. 0 (zero) with the description `<n.e.>` must be defined once as default production area. After this entry was saved, it is no longer displayed on this dialog. Enter this production area to see if it exists. An error report will indicate that it has already been entered.
*   **Production area** Name of the production area.
*   **Max. unit/h** Specification of how many units (pieces) can be processed in the production area per hour. If, for example, you have 6 grinding machines but only 3 workers who can work on these machines, you can only calculate the total capacity for three machines.
*   **Min. dwell days** Number of days that an element of an item dwells in the production area:
    *   0 = no dwell time
    *   0.1 = one shift
    *   1 = one day, e.g. entry into the production area today, exit tomorrow.
    Additional times are defined as transition times.
    ⇨ "Transition Times" on page H-192
    ⇨ "Transition Matrix" on page H-210
*   **Client** Client to whom the production area is assigned. The clients are stored in the company data.
    ⇨ Master Data, "Company Data – Client" on page B-900
*   **Status report** The status in capacity planning and in the order can be implemented automatically by the report from barcoding of A+W Production. With the setting you specify from which registration point the report is sent. The status of the items and of the order can be checked on the `Status reports` dialog.
    ⇨ Sales, "Status Message" on page C-498

#### Machines

`Capacity planning > Master data > Organisation > Machines`

All machines used are created with technical restrictions and operating costs required for planning and cost calculation.

This dialog contains the following tabs:
*   "Machines - General" on page H-197
*   "Machines - Restrictions" on page H-202

The fields for the definition of restrictions are released on the `Machine types` dialog.
⇨ "Machine Types" on page H-185

> **Info: Attention in case of subsequent activation of checks**
> If you tick a checkbox for a machine type later, you must check all machines that belong to the changed machine type. The newly-released fields are blank by default. This can cause errors during checking.

##### Machines – General

`Capacity planning > Master data > Organisation > Machines > General` tab

On this tab, you specify the machines that you use and that are relevant for capacity planning. You should also create a machine `Shipping` so that the times for that can be planned.
⇨ Tutorial, "Machine Types and Machines" on page H-21

**Machine**
*   **No./description** Number (ID) and description can be selected freely. We recommend grouping similar machines in number ranges, e.g. 100-199 for cutting tables, 400-499 for drills, etc.
*   **Type** Machine type to which the machine belongs. With the assignment, the fields for the restriction checks are released.
    ⇨ "Machine Types" on page H-185
*   **Production area** Production area in which the machine is installed.
    ⇨ "Production Area" on page H-195

**Options**
*   **Sheets rotatable** Defines whether the sheets can be rotated on the machine.
    *   The sheets cannot be rotated.
    *   The sheets can be rotated.
*   **Edge protection permitted** Defines whether this machine can apply edge protection.
    *   Edge protection cannot be put on.
    *   Edge protection can be put on.
*   **Auto break** Specification whether the cutting table has an automatic breaking device.
    *   The table has no automatic breaking device.
    *   The sheets can be broken automatically.
*   **Shapes possible** Specification whether shapes (non-rectangular sheets) can be produced on the machine.
    *   Shapes are not possible.
    *   Shapes are possible.
*   **Georg. bar permitted** Defines whether this machine can produce Georgian bars.
    *   Georgian bars are not possible.
    *   Georgian bars are possible.
*   **LG** Specification whether LG can also be cut on the cutting table.
    *   The table cannot cut any LG sheets.
    *   The table can cut LG sheets.
*   **Gas filling possible** Defines whether this machine can handle gas fillings.
    *   Gas fillings are not possible.
    *   Gas fillings are possible.
*   **Autosupport** Specification whether the cutting table has an automatic support.
    *   The table has no automatic support.
    *   The table has an automatic support. In this case, for each stock plate that is cut on this table, a support code must be assigned.
*   **Decoating** Specification whether the edges of sheets can be decorated on the machine.
    *   Edge decoatings are not possible.
    *   Edge decoatings are possible.
*   **Mitre-cut table**
    Selection of the number of mitre-cut tables. This setting is not displayed for A+W Business Pro.

**Additional options**
These settings apply only for A+W Business Pro.
*   **Output directory** Selection of the storage location for output file.
*   **Machine code** Selection of the machine code. The machine codes are stored on a dialog by the same name. If the code you are searching for is missing, you can create it in this dialog.
*   **IG driver, IG section** The fields are filled if the machine code for an IG line is selected.

**Keyword**
*   **Z-cut** Specification of the location of Z-cuts in cutting mode.
    *   **(<n.e.>):** Not applicable.
    *   **up:** Normally it is better to place the Z-cuts up, that is, to place them away from the working width so that individual cuts can first be broken across the whole width and then rotated. If overlying sheets have Z-cuts, then there is already space on the breaking table to break the sheets for the Z-cut.
    *   **bottom:** The starting point is at the top
    *   **anywhere:** The starting point can be selected at will.
*   **Cutting mode** Specification of the sequence in which the cuts will be made:
    *   **1 - XYZW:** The first cut runs parallel to the lower edge of the plate. After that come the Y-cut and the Z-cut. The further sequence is optional.
    *   **2 - XYZ\*:** Like 1. After the Z-cut comes any other cut.
    *   **3 - YXZW:** The first cut runs perpendicular to the lower edge of the plate. After that come the Y-cut and then the Z-cuts
    *   **4 - YXZZ:** Like 3. However only two Z-cuts are possible.

**Values**
*   **Units per hour** The value in this field depends on the work unit capacity planning shall use to calculate the capacity of this machine: man hours or machine hours. By default, a 1 is entered.
    ⇨ Tutorial, "Work Units" on page H-39
*   **Labour costs per unit** The entry in this field depends on the work unit capacity planning shall use to calculate the capacity of this machine, e.g. man hours or machine hours. You will find detailed information under:
    ⇨ Tutorial, "Work unit = man hour" on page H-39
*   **Machinery costs** Machine costs per hour, e.g. for maintenance, repair, consumables.
*   **Variable costs per hour** Miscellaneous costs which belong neither to labour costs nor to machinery costs, can be included in the production costs, e.g. insurance. The total insurance fee has to be converted in to costs per hour.
*   **Costs per unit** Total costs per unit for this machine. They are the basis for cost calculation. These costs are calculated from labour costs, machinery costs, variable costs, and the work unit per hour.
    > **Example**
    > Labor costs/hr
    > + machine costs/hour divided by units/hour
    > + variable costs/hour divided by units/hour
    > = costs/unit
