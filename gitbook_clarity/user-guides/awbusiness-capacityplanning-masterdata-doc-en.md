---
description: "EN_AWBusiness_Capacity_Planning_4_3"
---


# Software Reference

---
## Organisation

### Registration point
Number of the registration point (machine) in A+W Production this machine refers to. The numbers must be identical in A+W Business Pro and A+W Production. If you are using barcoding (scanners), you have to scan the registration point number.

### Output per hour
Average targets (based on experience or based on information from the machine manufacturer) in quantity units.
You can use this entry if you have e.g. defined all master data except the default times and want to schedule those in advance to estimate the capacity of your production. This allows to bridge the time until all standard times have been entered.

### Serial tables
Selection of the serial table in which the special times for series are defined.
⇨ "Serial Factors" on page H-191

### Lock

- **Locked**: The machine can be locked for scheduling.
- The machine is not locked.
- The machine is locked and cannot be included in scheduling. This setting is used for example if a new machine shall be tested first before it is actually used.

To lock a machine for maintenance purposes please go to the Machine downtime dialog:
⇨ "Machine Failure" on page H-287

### Locking formula
With a locking formula, you can store additional restrictions that cannot be reached with standard means.

> **Example**
> On a machine, only shapes, very small, and very large sheets shall be produced because this machine is very slow.
> All rectangular sheets with a width >200 and <2600 mm as well as a height >300 and <1600 mm shall not be cut on this machine.
> This restriction can only be specified with a formula. If you want to use formulas, contact your service employee at A+W Software GmbH.

### Add. work type for coupled machines
Currently not used.

### Table
In the overview, the machines that are available for capacity planning are listed depending on the selection criteria.

## Machines – Restrictions

**Path:** `Capacity planning > Master data > Organisation > Machines > Restrictions tab`

*Fig. H-137: Machines – Technical restrictions*

On this tab, you store minimum and maximum values for the restriction checks. Enter 0 to 9999 if all values are permitted.

The fields for the definition of restrictions are released on the Machine types dialog.
⇨ "Machine Types" on page H-185

If the technical restrictions are different for a machine with the same work types, define these restrictions on the Special technical restrictions dialog. Capacity planning checks the entry in Special technical restrictions dialog first.
⇨ "Special Technical Restrictions" on page H-212

The fields in the Machine group are described for the General tab.
⇨ "Machines - General" on page H-197

### Work types / time surcharges
In this group, all work types are listed for which default times on this machine are defined.
⇨ "Default Times (dialog)" on page H-217

### Technical restrictions
The fields for the definition of restrictions are released on the Machine types dialog.
⇨ "Machine Types" on page H-185

Enter 0 or 9999 if all values are permitted.

**Width, height**: Min. and max. sheet dimensions for this machine.

**Spacer**: Min. and max. spacer for this machine

**Total thickness**: Min. and max. total thickness for IG and LG.

**Glass thickness**: Min. and max. thickness of single glass.

**Surface in sqm**: Min. and max. surface for this machine.

**Mitre angle**: Min. and max. mitre angle for facets.

**Quantity**: Min. and max. quantity for the order item. In the item, the quantity or quantity range must be checked. The definition of the quantity is machine-dependent, e.g.
- Drilling machine = number of drill holes
- Grinding machine = number of edges

**Drilling diameter**: Min. and max. dimensions for this machine.

**Radius round. corner**: Min. and max. dimensions for this machine.

**Diagonal**: Diagonal between the rollers, e.g. on the conveyor belt in front of the TG furnace.

**Max. number of sheets**: Maximum quantity of sheets for a TG or IG unit, e.g. 3 on an IG line.

**Max. ratio**: Maximum ratio for this machine.

> **Example**
> You enter the value 5. This corresponds to a max. ratio of 1:5. If one side is 500 mm long, for example, then the other side can be max. 2500 mm.

**Weight up to kg**: Maximum weight of a unit.

### Distance between cuts
For cutting tables with an automatic breaking device, you must set the maximum and minimum distances between the cuts. These distances must be adhered to so that the system can still break the sheet.

**Min. Dist. X-X with Y**: Minimum distance between X-X cuts if Y-cuts are also made.

**Min. Dist. X-X without Y**: Minimum distance between X-X cuts if no Y-cuts are also made.

**Max. Dist. X-X cuts**: Maximum distance between X-X cuts.

**Min. Dist. Y-Y with Z**: Minimum distance between X-X cuts if Y-cuts are also made.
For cutting tables with several Y-cutting heads, the minimum distance corresponds to the distance of the cutting wheels of two immediately adjacent cutting heads, e.g. Bystronic XYZVA = 300 mm.

**Min. Dist. X-X without Z**: Minimum distance between X-X cuts if no Z-cuts are also made.

**Max. Dist. Y-Y cuts**: Maximum distance between Y-Y cuts.

**Min. residual width**: Minimum width at the edge of the plate.

**Min. Dist. X-Z cuts**: Minimum distance between X and Z-cuts.

**Min. Dist. Z-Z cuts**: Minimum distance between Z-cuts.

## Calendar

**Path:** `Capacity planning > Master data > Organisation > Calendar`

On this dialog, you specify the work days and shift times. The data can be saved only if at least one shift has been entered. The number of shifts is defined in company data
⇨ "Default Settings in Company Data" on page H-179

If no calendars are defined in capacity planning, the A+W Business Pro standard calendar will be used.

By default, capacity planning assumes one shift per day. If, however, you want to work in more than one shift, you have to enter the number of shifts first. After that you can define calendars for machines with different shifts and shift times.

> **Example**
> The calendar permits to enter a maximum of six shifts per day. If the hours are equally distributed, this is a maximum of four hours per shift. The distribution of the number of hours per shift varies however, e.g. 5, 3, 5, 3, 5, 3 or 4, 2, 6, 6, 3, 3.
> These examples show that you do not have to stick to an even distribution of hours.
> In case of 4 shifts and uniform distribution per shift, a maximum of 6 hours can be entered.
> The total hours x shifts per day must not exceed 24 hours of course.

> **Changing the calendar**
> When you have edited a calendar or entered a new one, you have to reboot A+W Business Pro to make sure that the data are available for scheduling.

This dialog contains the following tabs:
- "Calendar - Selection" on page H-206
- "Calendar - Calendar" on page H-208

### Functions Menu

**Path:** `Capacity planning > Master data > Organisation > Calendar`

Using this menu, you can open other dialogs without closing the calendar.

The following entries are displayed:

- **Copy:**
Opens the Copy calendar dialog to transfer a calendar, e.g. into a new year.
⇨ "Copy Calendar" on page H-209
- **Shift times:**
Opens the Shift settings dialog on which you can specify the shift transition and closing times.
⇨ "Shift Settings" on page H-183
You must have administrator rights to open the dialog. In addition, the Use change of shift table checkbox must be ticked on the Company data dialog.
⇨ "Use change of shifts table" on page H-182

### Calendar – Selection

**Path:** `Capacity planning > Master data > Organisation > Calendar > Selection tab`

*Fig. H-138: Calendar - Selection*

On this tab, you specify calendar for work types, machines, production area, and clients.

If no special calendar is defined for a production area or a machine, the common calendar will be used.
⇨ Tutorial, "Adjust Calendar" on page H-45

#### Identification
The labeling of the two selection fields depends on the mode selected.

**Work type, machine**: Work type and machine to which the calendar applies.

**Production area, client**: Production area and client to whom the calendar applies.

**Year**: Year to which the calendar is edited or created.

#### Mode
With the selection of the option, you specify for what you want to create the calendar. The fields are only released in selection mode.

- **Work type, machine:**
With this setting, you specify a calendar for a work type and/or a machine.
- **Production area/client:**
With this setting you specify a new calendar for a production area and/or a client.
In order to create a general calendar, select this option and enter the production area `<n.e.>` and for the clients `all`.

**Calendar tables**: In the overview, all calendars are displayed that correspond to the selection criteria. If you have limited the selection only according to the Work type mode or Production area, all calendars are displayed.

### Calendar – Calendar

**Path:** `Capacity planning > Master data > Organisation > Calendar > Calendar tab`

*Fig. H-139: Calendar - Calendar*

On this tab, you specify the work time per shift. The number of shifts is specified in the company data.
⇨ "Default Settings in Company Data" on page H-179

#### Working week

**Monday - Sunday**: If you want to change the shift time of a weekday, you must tick the appropriate checkbox and enter the new number of hours. The change applies only to the date displayed. If necessary, you must transfer the new shift time to the year or the calendar week.

**Hours per shift**: Number of available hours per week day and shift.

> **Set up additional shift**
> If you want to set up an additional shift for a machine or a production area, you must re-enter all shift times.
> It is not sufficient to specify only the hours for the new shift, because during transfer to the year (or the week), the blank fields are also taken over. This deletes the old shift times.

#### Adopting shifts for calendar

**[Apply to year]**: Transfers the changes to all appropriate weekdays of the year.
Only the shift times of the weekdays are transferred for which the checkbox is ticked.

**[Apply to week]**: Transfer the change to all days of the calendar week.

#### Calendar week

**Go to**: Selection of the calendar week.

**[Current calendar week]**: Changes the display in the Working week group to edit the shift times for the current calendar week.

## Copy Calendar

**Path:** `Capacity planning > Master data > Organisation > Calendar > Functions menu > Copy`

*Fig. H-140: Copy calendar*

On this dialog, you copy the calendar for a machine or a production area, e.g. by transferring it to another machine.

### Calendar source selection
The labeling of the two selection fields depends on the mode selected.

**Work type, machine**: Work type and machine for which the calendar is created.

**Production area, client**: Production area and client to whom the calendar applies.

**Year**: Year for which the calendar is created.

### Calendar destination selection

**Work type, machine**: Work type and machine to which the calendar shall be transferred.

**Production area, client**: Production area and client to whom the calendar shall be transferred.

## Transition Matrix

**Path:** `Capacity planning > Master data > Organisation > Transition matrix`

*Fig. H-141: Transition matrix*

On this dialog, you enter how long it takes until the item moves from one production area to the next one. The times can be designed differently depending on the order priority.

> **Example**
> The transition from the Cutting production area to the Processing production area can normally be done in the same shift.
> The transfer from the TG production area to the IG production area takes several shifts or 1 day.

⇨ Tutorial, "Transition Matrix and Transition Times" on page H-64

**Order priority**: Selection with which order priority the transition time shall be considered. You can select one of these priorities:
- **Normal:**
The transition time applies to all orders which have no special priority. This is the default setting.
- **Urgent:**
The defined transition time applies to rush orders only. If transition times can be shortened for rush orders, a different transition time must be defined for this combination of work types.
- **Extra:**
This priority means that the order shall be produced from residue (plates) left over from cutting other orders.
- **Release order:**
The transition time applies only to orders that are produced on-call.

> **Consider order priority**
> If in addition to the order priority `Normal` the priority `Urgent` shall be considered, a special transition time must be defined for the corresponding combination of production areas. This applies to all times that can be shortened for rush orders if required. If these have not been defined, the order will be scheduled with `Normal` priority.

**From production area**: Production area the item comes from.

**To production area**: Next production area to which the item changes.

**Transition time**: Time that a glass requires to change to the next production area. The values are entered in days:
- 0 = same day or same shift
- 0.01 to 0.99 = next shifts
- 1 = next day

### Examples for the calculation of the transition

*Tab. H-4: Transition times in days*

| No. shifts | 1/no. hours | Same shift | Next s. | e.g. | S. after the next one | e.g. | S. two shifts after the next one | e.g. | S. three shifts after the next one | e.g. |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **4** | 1/4=0.25 | 0<br>Transition: S1-Mo<br>Transition: S2-Mo | 0.1-0.24<br>S2-Mo<br>S3-Mo | 0.2 | 0.26-0.49<br>S3-Mo<br>S4-Mo | 0.4 | 0.51-0.74<br>S4-Mo<br>S1-Tu | 0.6 | 0.76-1<br>S1-Tu<br>S2-Tu | 1 |
| **3** | 1/3=0.33 | 0<br>Transition: S1-Mo<br>Transition: S2-Mo | 0.1-0.3<br>S2-Mo<br>S3-Mo | 0.2 | 0.4-0.6<br>S3-Mo<br>S1-Tu | 0.5 | 0.7-1<br>S1-Tu<br>S2-Tu | 1 | - | - |
| **2** | 1/2=0.5 | 0<br>Transition: S1-Mo<br>Transition: S2-Mo | 0.1-0.49<br>S2-Mo<br>S1-Tu | 0.3 | 0.51-0.1<br>S1-Tu<br>S2-Tu | 1 | - | - | - | - |

> **Flexible transition time**
> Instead of a fixed value, you can also enter a formula if the transition time depends on different parameters, e.g. thickness. With a right-click in the field, the Formula search dialog opens.
> If you want to work with formulas, call your service employee at A+W Software GmbH for assistance.

## Special Technical Restrictions

**Path:** `Capacity planning > Master data > Organisation > Special technical restrictions tab`

*Fig. H-142: Special technical restrictions*

On this dialog, you specify restrictions for machines that refer to particular work types.

If a machine can execute different work types, e.g. Drilling and Corner cut-out, you can define different check values per work type. If capacity planning finds no definition for the work type, the general technical restrictions of the machine will be checked.
⇨ "Machines - Restrictions" on page H-202

The available parameters depend on the settings on the Machine types dialog.
⇨ "Machine Types" on page H-185

### Functions menu
Using this menu, you can copy the values from the standard machine. Already-entered values are overwritten without a query.
⇨ "Machines – Restrictions" on page H-202

### Identification
**Work type**: Work type to which the restrictions apply.

**Machine**: Machine to which the restrictions apply when the appropriate work type is performed.

### Technical restrictions (minimum/maximum)
Enter 0 or 9999 if all values are permitted.

**Width, height**: Min. and max. dimensions for this machine.

**Spacer**: Min. and max. spacer for this machine.

**Total thickness**: Min. and max. total thickness for IG and LG for this machine.

**Glass thickness**: Min. and max. thickness of single glass.

**Quantity**: Min. and max. quantity for the order item. In the item, the quantity or quantity range must be checked. The definition of the quantity is machine-dependent, e.g.
- Drilling machine = number of drill holes
- Grinding machine = number of edges

**Drilling diameter**: Min. and max. size for this machine.

**Radius round. corner**: Min. and max. size for this machine.

**Surface in sqm**: Min. and max. surface for this machine.

**Diagonal**: Diagonal between the rollers, e.g. on the conveyor belt in front of the TG furnace.

**Mitre angle**: Min. and max. mitre angle for bevelling.

### Other technical restrictions
Enter 9999 if all values are permitted.

**Serial table**: Number of the serial table that shall be used for serial production.
⇨ Software Reference, "Serial Factors" on page H-191

**Max. number of sheets**: Maximal number of sheets permitted for a laminated glass or IG unit on this machine.

**Weight up to kg**: Maximum weight.

**Max. ratio**: Maximum ratio for this machine.

> **Example**
> The value 5 corresponds to a max. ratio of 1:5.
> If one edge of the sheet is 500 mm, for example, then the other edge can be max. 2500 mm long.

### Technical restrictions (options)

**Shapes possible**: Defines whether this machine can produce shapes.
- Shapes are not possible.
- Shapes are possible.

**Georg. bar permitted**: Defines whether this machine can produce Georgian bars.
- Georgian bars are not possible.
- ☑ Georgian bars are possible.

**Gas filling possible**: Defines whether this machine can handle gas fillings.
- Gas fillings are not possible.
- Gas fillings are possible.

**Sheets rotatable**: Defines whether the sheets can be rotated on the machine.
- The sheets cannot be rotated.
- Sheets can be rotated

**Edge protection permitted**: Defines whether this machine can apply edge protection.
- Edge protection cannot be put on.
- Edge protection can be put on.

### Overview of special restrictions
On the overview, the work types and machines are listed for which special restrictions are stored.

## Org. Overview

**Path:** `Capacity planning > Master data > Organisation > Org. overview`

*Fig. H-143: Org. overview*

On this dialog, you check which machines and work types are allocated to the production areas.

### Selection
**Client**: Client to whom the production area is assigned.

**Production area**: Production area to which the machines are assigned.

**Breakdown level**: With the selection of the option, you filter the display in the overview.

### View
The columns in the overview depend on the breakdown level.

- **Production area:**
Production area to which the machine is assigned.
- **Machine:**
Machines that are assigned to the production area in question.
- **Work type:**
Work types that are assigned to the machine in question.
- **Surcharges:**
Type of default time that is consulted for the work type in question for calculation.

## Default Times

**Path:** `Capacity planning > Master data > Default Times`

In this program group, you will find the dialogs on which the defaults for the time calculation are stored.

This section provides information on the following subjects:
- "Default Times (dialog)" on page H-217
- "Change Default Times" on page H-225
- "Copy Default Times" on page H-225
- "Special Times" on page H-226
- "Special Priorities" on page H-227

### Default Times (dialog)

**Path:** `Capacity planning > Master data > Default Times > Default Times`

On this dialog, you enter the time values determined for your machines per work type and machine. It depends on the machine whether the calculation of times is based on linear metres, square metres, pieces, etc.

On this dialog, you will find the following tabs:
- "Default Times – Time Selection" on page H-218
- "Default Times – Matrix" on page H-221
- "Default Times - Vector" on page H-222
- "Default Times – Individual Time" on page H-223
- "Default Times – Cube" on page H-224

#### Entry of time values in hours
Times are not entered in minutes but in hours. This means that the measured minutes must be converted into hours:

| Minutes | Time entry in hr. |
| :--- | :--- |
| 60 | 1 |
| 30 | 0.5 |
| 15 | 0.25 |
| 7.5 | 0.125 |
| 3.75 | 0.0625 |
| 1.875 | 0.03125 |

### Functions menu

**Path:** `Capacity planning > Master data > Default Times > Default Times`

Using this menu, you can open other dialogs without closing the default times. The following entries are displayed:

- **Change:**
Opens the dialog by the same name to increase or reduce the default times by a factor.
⇨ "Change Default Times" on page H-225
- **Copy:**
Opens the dialog by the same name to copy the default times from the standard machine.
⇨ "Copy Default Times" on page H-225

### Default Times – Time Selection

**Path:** `Capacity planning > Master data > Default Times > Default Times > Choose time tab`

*Fig. H-144: Default Times - Table selection*

On this tab, you specify the type of calculation and the priority.
⇨ Tutorial, "Default Times" on page H-55

#### Identification
**Work type**: Work type to which the default time applies.
**Machine**: Machine on which the work time requires the default time.

**Type**: Type of the default time:
- **0 - Basic time:**
Stopped time for a work process.
⇨ "Entry of time values in hours" on page H-217
- **1 - Time surcharge:**
A time surcharge is required for work types that require more effort, e.g. for cutting shapes.
- **2 - Alternative procedure:**
This default time is only considered if an alternative work type exists for the work type. In this case, in the `Alternative A+W Prod. no.` field you must enter the alternative machine number.
- **3 - Alternative without BOM:**
Laminated glass producers usually enter all LG articles with bills of materials. When a LG sheet is not going to be produced but directly cut from a LG stockplate, the bill of material must be ignored. For the work type `LG cutting`, the `Alternative w/o BOM` would be selected. In this case, enter the alternative machine number in field `altern. A+W Prod. no.`
- **4 - Ignore process:**
A corner cut-out for example requires three processes: 1. Drilling (of corner hole), 2. Cutting, and 3. Grinding.
The CNC machine can do everything on one, so that just the drilling will be taken into account. The other two work types will be ignored. You only have to assign the default time for the work type `Drilling` which covers the whole process. The other two work types are allocated the entry `Ignore process` for this machine.

**Priority**: If several machines are available for one work type, you must specify which machine is queried first during the search for free capacities and which, for example, can only be selected manually.
If two machines have the same priority, then capacity planning checks the costs that are defined per machine. In this case, the cheaper machine is selected automatically.
If no costs per machine are stored, the program can find the cheapest machine. In this case, the priority must be clear for the same machines.
- **9:** highest priority (standard machine). These machines are always selected first.
- **8 to 1:** decreasing priority. These machines are selected depending on utilization.
- **0:** lowest priorities. These machines are only selected if all other (equivalent) machines are used to capacity.
- **-1:** for manual scheduling. These machines are selected by automatic scheduling only in case of bottlenecks.
- **-2:** only for manual scheduling. These machines are never selected by automatic scheduling. The machine can only be selected manually.
- **-3:** is only selected with reporting from the production system when orders have been rescheduled there. In case of rescheduling in capacity planning, only machines with prio >-3 are displayed.

**Alternative A+W Prod. no.**: In this field, you must enter the machine number from A+W Production if in the `Type` field the value `Alternative process` or `Alternative without BOM` is selected.

#### Grouped by
With the selection of the option, you specify how the display in the overview shall be grouped. The fields are only released in selection mode.
- **Work type:**
For each work type, the assigned machines are displayed.
- **Machine:**
The work types with defined times are displayed per machine.

#### Other surcharges
**Table**: Reference to surcharge table, e.g. for oversizes. These surcharge tables are created on the Special times dialog.
⇨ "Special Times" on page H-226

#### Overview
All default times with the assigned work types are listed in the overview. With a double-click on allocations, the allocated products, product types, product classes, and/or product groups are displayed.
You select the grouping in the selection mode.

### Default Times – Matrix

**Path:** `Capacity planning > Master data > Default Times > Default Times > Matrix tab`

*Fig. H-145: Default Times – Matrix*

On this tab, you specify the default times, which are graduated according to two limit types.
⇨ Tutorial, "Default Times" on page H-55

**Limit type 1, limit type 2**: Default times can be graduated by means of limit types. The limit type defines the measure for the graduation. You can select thickness and area, for example.
The input field for the limit value is released if you insert a new column/row. The limit value refers to the limit type.
⇨ Master Data, "Quantity Limits" on page B-872

#### Specification

**Time unit**: The unit refers to the limit type. The limit value can refer to pieces, square meters, linear meters, etc.

**Triangle**: You can record times in a matrix or in a cube so that the specified limit values can be switched, e.g. height and width.
- The limit types must not be switched. In this case, you must enter a time per column/row in all fields. Select this setting for glass for which it is important in which direction it is cut.
- The limit types may be switched. Thus you only have to record the time in one of the combinations of limit types.

#### Min. values
The min. values are checked at scheduling. If values are under-run, a message is displayed and/or a surcharge is charged.

**Minimum time**: You can specify how much minimum time is calculated for an item.

#### Overview
In the overview, you specify in each field per row and column the time that is required for this combination of limit types for the work type.

### Default Times – Vector

**Path:** `Capacity planning > Master data > Default Times > Default Times > Vector tab`

*Fig. H-146: Default Times - Vector*

On this tab, you specify default times, which are graduated according to one limit type, e.g. by thickness.
The fields are described on the Matrix tab.
⇨ "Default Times – Matrix" on page H-221

### Default Times – Individual Time

**Path:** `Capacity planning > Master data > Default Times > Default Times > Indiv. time tab`

*Fig. H-147: Default Times – Individual time*

On this tab, you store individual times. Generally you store individual times for the work processes. There is a row displayed for each combination of machine and work type. Entries in red indicate that no times are defined.

#### Overview
- **Machine:**
Machine that is selected on the `Choose time` tab.
- **Work type:**
Work type for which a time is specified on the selected machine.
- **Time:**
Measured time.
- **Time unit:**
Unit to which the measured time refers, e.g. to piece, square meter, linear meter, etc.
- **Minimum time:**
Minimum time that is calculated for an item if the required time is here.
- **Type:**
Type of the time. The type specifies how the time shall be calculated, e.g. as basic time or surcharge.
⇨ "Default Times - Time Selection" on page H-218

### Default Times – Cube

**Path:** `Capacity planning > Master data > Default Times > Default Times > Cube tab`

*Fig. H-148: Default Times – Cube*

On this tab, you store default times that are graduated according to three limit types, e.g. by height, width, and thickness.
The fields are described on the Matrix tab.
⇨ "Default Times – Matrix" on page H-221

### Change Default Times

**Path:** `Capacity planning > Master data > Default Times > Default Times > Functions menu > Change`

*Fig. H-149: Change default times*

On this dialog, you can change the default times for a machine or work type. If, for example, you enter the factor 1.5, all times of the selected combination of machine and work time are increased by half. The factor 0.5 would reduce the times by half.

### Copy Default Times

**Path:** `Capacity planning > Master data > Default Times > Default Times > Functions menu > Copy`

*Fig. H-150: Copy default times*

On this dialog, you can copy default times from a machine and work type to transfer them to another machine and work type. You can also reduce or increase the values by a factor.

## Special Times

**Path:** `Capacity planning > Master data > Default Times > Special Times`

*Fig. H-151: Special times*

On this dialog, you define the time surcharges for especially time-consuming processings, e.g. for special sizes. You can assign the time surcharges on the `Default Times` dialog in the `Other surcharges` group. Special times which have been defined with the same criteria, can be collected in groups (tables).

⇨ Tutorial, "Special Times" on page H-58

Another possibility for defining time surcharges in the form of factors is using the allocation dialog boxes.
⇨ "Default Times (dialog)" on page H-217
⇨ "Allocation" on page H-229

### Time surcharge for
**Number**: Use-defined number (ID) of the table.
**Name**: Name of the table, e.g. oversizes.

### Surcharges (overview)
In the overview, all defined surcharges are listed.

### Surcharges
In the overview, the graduation of the time surcharge is shown that is selected on the Table tab.

- **Up to limit 1, 2:**
Value per limit type up to which the surcharge shall be calculated.
- **Limit type 1, 2:**
Limit type to which the limit value refers, e.g. the edge length for the calculation of oversizes.
⇨ Master Data, "Quantity Limits" on page B-872
- **Surcharge:**
Amount of the surcharge. The value refers to the surcharge unit.
- **Surcharge unit:**
Unit with which the surcharge shall be calculated.
- **Surcharge type:**
Basis on which the surcharge is assessed.

## Special Priorities

**Path:** `Capacity planning > Master data > Default Times > Special priorities`

*Fig. H-152: Special priorities*

On this dialog, you enter the priorities per machine and work type based on additional criteria, e.g. by product class, thickness, customer. If there is a zero (0) in the fields, the special priority applies overall, e.g. to the selected customer or to the specified quantity.

This can be useful in the following cases:
- If several machines of the same type are available for a work type.
- If customers require special processing steps, which can only be executed on special machines.

**Work type**: Work type for which an exception has been defined.

**Machine**: Machine on which the work type is performed.

**Customer**: Customer to whom the priority applies.

**Company**: Company to whom the priority applies.

**PGR**: Product group to which the priority applies.

**Edge length**: Edge length in mm, to which the priority applies.

**Thickness >=**: Glass thickness in mm, to which the priority applies. 0 = all thicknesses.

**Quantity >**: Quantity starting from which the priority applies, e.g. number of holes, of corner cut-outs.

**Drilling diameter >=**: Diameter of a hole in mm from which on the priority is applied.

**Priority**: The digits have the following meaning:
- **9:** highest priority (standard machine). These machines are always selected first.
- **8 to 1:** decreasing priority. These machines are selected depending on utilization.
- **0:** lowest priorities. These machines are only selected if all other (equivalent) machines are used to capacity.
- **-1:** for manual scheduling. These machines are selected by automatic scheduling only in case of bottlenecks.
- **-2:** only for manual scheduling. These machines are never selected by automatic scheduling. The machine can only be selected manually.
- **-3:** is only selected with reporting from the production system when orders have been rescheduled there. In case of rescheduling in capacity planning, only machines with prio >-3 are displayed.

## Allocation

**Path:** `Capacity planning > Master data > Allocation`

On these dialogs, you allocate the basic products of A+W Business Pro (single glass, TG, LG, processings, shapes, muntions, etc.) to the work types.

This section provides information on the following subjects:
- "Product Types" on page H-230
- "PGR" on page H-232
- "Product Class" on page H-233
- "Products" on page H-234
- "Combined Product Type" on page H-235
- "Special Allocation 1" on page H-236
- "Special Allocation 2" on page H-237
- "Special Allocation 3" on page H-239
- "Special Allocation 4" on page H-241
- "Combined Product Class" on page H-243
- "Stock Articles" on page H-244

### Product Types

**Path:** `Capacity planning > Master data > Product Types`

*Fig. H-153: Product Types*

On this dialog, you allocate the work types to the A+W Business Pro product types in the sequence in which they will be performed in production or in shipping. For each work type, you can specify a time factor that shall be calculated for planning.
⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

**Product type**: Product type to which work types are allocated.

#### Work types
In the overview, the allocated work types are displayed.

**#**: Number of the sequence.

**Work type**: Product number and name of the work type. If you enter `<n.e.>` the product type is ignored. This makes sense for the product type Surcharges, for example.

**Factor**: The time calculated at scheduling is multiplied by this factor.
- 0 or 1: the time is not increased or reduced.
- 1: A factor of 1.5 corresponds to a time increase of 50%.

#### Buttons
**[New], [Delete]**: With these buttons you enable a new row or delete a marked entry.

**Arrow buttons**: Use this buttons to change the sequence of work types. For the product type TG, for example, the allocation could look as follows:
- Wash glass
- Check
- Produce TG
- Package processed TG
- Loading

#### List of allocations
In the list, the product types are displayed to which work types are assigned.

### PGR

**Path:** `Capacity planning > Master data > PGR`

*Fig. H-154: Product groups*

On this dialog, you allocate the product types to the A+W Business Pro product groups in the sequence in which they will be performed in production or in shipping. For each work type, you can specify a time factor that shall be calculated for planning.
⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Product group**: Product group to which the work types are allocated.

#### Work types
The fields and buttons in this group are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

#### List of allocations
In the list, the product groups are displayed to which work types are assigned.

### Product Class

**Path:** `Capacity planning > Master data > Product Class`

*Fig. H-155: Product Class*

On this dialog, you allocate the work types to the A+W Business Pro product classes in the sequence in which they will be performed in production or in shipping. For each work type, you can specify a time factor that shall be calculated for planning.
⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Product class**: Product class to which work types are allocated.

#### Work types
The fields and buttons in this group are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

#### List of allocations
In the list, the product classes are displayed to which work types are assigned.

### Products

**Path:** `Capacity planning > Allocation > Products`

*Fig. H-156: Products*

On this dialog, you allocate the work types to the A+W Business Pro products in the sequence in which they will be performed in production or in shipping. For each work type, you can specify a time factor that shall be calculated for planning.
⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Product**: Product to which work types are allocated.

#### Work types
The fields and buttons are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

#### List of allocations
In the list, the products are displayed to which work types are assigned.

### Combined Product Type

**Path:** `Capacity planning > Master data > Combined product type`

*Fig. H-157: Combined product types*

On this dialog, you allocate the work types to the A+W Business Pro products that are a component of a BOM or affect a product group as a processing. You allocate the work types in the sequence in which they are performed in production or in shipping. For each work type, you can specify a time factor that shall be calculated for planning.
⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Product**: Product which – as a BOM element e.g. of TG, LG, etc. – has been assigned a work type other than the work type defined by default for the main product.

**As part of, affects**: If the float sheet is part of a BOM, the production sequence or the work type can change. Enter the appropriate product type, e.g. TG.

#### Work types
The fields and buttons in this group are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

#### List of allocations
In the list, the combination product types are displayed to which work types are assigned.

### Special Allocation 1

**Path:** `Capacity planning > Allocation > Special Allocation 1`

*Fig. H-158: Special Allocation 1 – Processings*

On this dialog, you allocate the work types to a A+W Business Pro processing product and the subsequent processing. You allocate the work types in the sequence in which they are performed in production or in shipping. For each work type, you can specify a time factor that shall be calculated for planning.
⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Processing**: Processing to which work types are allocated.

**Next processing**: Next processing to which work types are allocated.

#### Work types
The fields and buttons in this group are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

#### List of allocations
In the list, the processings and next processings are displayed to which work types are assigned.

### Special Allocation 2

**Path:** `Capacity planning > Allocation > Special Allocation 2`

*Fig. H-159: Special Allocation 2 - Processings to shapes*

On this dialog, you allocate the work types to a processing on shapes and the subsequent processing. You allocate the worktypes in the sequence in which they are performed in production or in shipping. For each work type per edge, you can specify a time factor that shall be calculated for planning.

> **Example**
> On a sheet with round edges, the edge processing on straight edges can be performed on the standard grinding machine, the edge processing for the round edges must be done on another machine.

⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Processing**: Processing to which work types are allocated.
**Shape**: Shape to which work types are allocated.
**Up to qty.**: Quantity if the assignment of the work types depends on the number of sheets, e.g. large quantities on CNC machines. Enter `9999` if the quantity shall not be checked.

*Fig. H-160: Identification of corners and edges of the selected shape*

#### Work types
In the overview, the allocated work types are displayed. The number of edges depends on the shape selected.
The buttons are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

**#**: Number of the sequence.

**Work type**: Number and name of the work type. If you enter `<n.e.>` the processing is ignored.

**Factor**: The time calculated during scheduling is multiplied by this factor.
- 0 or 1: the time is not increased or reduced.
- 1: A factor of 1.5 corresponds to a time increase of 50%.

**1 - n (edge)**: Specification to which edge the factor applies. The number of fields available depends on the number of edges and corners of the shape. In the shape sketch, the edges are marked with red numbers.
- The factor is not calculated for this edge.
- The factor is calculated.

#### List of allocations
In the list, the processings on shapes are displayed to which work types are assigned.

### Special Allocation 3

**Path:** `Capacity planning > Allocation > Special Allocation 3`

*Fig. H-161: Special Allocation 3 – Edge processing (rectangular sheets)*

On this dialog, you allocate the sequence of edge processing for rectangular sheets.

> **Example**
> If for a rectangular sheet all edges shall be polished, by default the edges 1 and 3 are polished simultaneously and after that 2 and 4 (or vice-versa).
> If on a machine 2 edges across from one another can be polished, seamed, etc. simultaneously, then you must assign the work type per edges 1 + 3 and 2 + 4.

⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Processing**: Processing to which work types are allocated.

**Edges 1 - 4**: Specification to which edges the allocation applies.
- This edge is not processed.
- This edge is processed.

*Fig. H-162: Identification of corners and edges for the calculation of the factor*

#### Work types
In the overview, the allocated work types are displayed. A factor can be specified per edge.
The buttons are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

**#**: Number of the sequence.

**Work type**: Number and name of the work type. If you enter `<n.e.>` the processing is ignored.

**Factor**: The time calculated during scheduling is multiplied by this factor.
- 0 or 1: the time is not increased or reduced.
- >1: A factor of 1.5 corresponds to a time increase of 50%.

**1 - 4 (edges)**: Specification to which edges the factor applies. In the shape sketch, the edges are marked with red numbers.
- The factor is not calculated for this edge.
- The factor is calculated.

#### List of allocations
In the list, the processings are displayed to which work types are assigned.

### Special Allocation 4

**Path:** `Capacity planning > Allocation > Special Allocation 4`

*Fig. H-163: Special Allocation 4*

On this dialog, you allocate different work types to a product, depending on the next processing and a shape. For each work type, you can specify a time factor that shall be calculated for planning.
⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Product**: Product to which work types are allocated.
**Next processing**: Next processing to which work types are allocated.
**Shape**: Shape to which the allocation applies.

*Fig. H-164: Identification of corners and edges for the calculation of the factor*

#### Work types
In the overview, the allocated work types are displayed. The number of fields for the edges depends on the selection of the shape.
The buttons are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

**#**: Number of the sequence.

**Work type**: Number and name of the work type. If you enter `<n.e.>` the processing is ignored.

**Factor**: The time calculated during scheduling is multiplied by this factor.
- 0 or 1: the time is not increased or reduced.
- >1: A factor of 1.5 corresponds to a time increase of 50%.

**1 - n (edges)**: Specification to which edges the factor applies. The number of fields available depends on the number of edges of the shape. In the shape sketch, the edges are marked with red numbers.
- The factor is not calculated for this edge.
- ☑ The factor is calculated.

#### List of allocations
In the list, the processings are displayed to which work types are allocated.

### Combined Product Class

**Path:** `Capacity planning > Master data > Combined product class`

*Fig. H-165: Combined product classes*

On this dialog, you allocate the work types and a time factor to the products that are a component of a BOM or affect a product class as a processing. For each work type, you can specify a time factor that shall be calculated for planning.
⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Product**: Product to which, as BOM of e.g. TG, LG, etc., is assigned to another work type than the one that normally applies to the main product.

**As part of, affects**: If the float sheet is part of a BOM, the production sequence or the work type can change. Enter the appropriate product type, e.g. LG

#### Work types
The fields and buttons in this group are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

#### List of allocations
List of the products to which work types are allocated.

### Stock Articles

**Path:** `Capacity planning > Allocation > Stock articles`

*Fig. H-166: Stock articles*

On this dialog, you allocate the work type `Shipping` to stock articles. This allocation is used because stock articles (supply type `Stock withdrawal`) will not be processed, e.g. handles which are just packed and shipped. As a result, this product class is, e.g., scheduled for dispatch, and the appropriate cost and time is calculated. For each stock article, you can specify a time factor that shall be calculated for planning.
⇨ Tutorial, "Allocate the A+W Business Pro Master Data" on page H-97

#### Identification
**Product class**: Stock articles to which work type is allocated.

#### Work types
The fields and buttons in this group are described for the `Product types` dialog.
⇨ "Product Types" on page H-230

#### List of allocations
In the list, the product classes are displayed to which work type is assigned.

## Lock

You must define locks to prevent, for example, that particular work is performed twice or that a machine is planned that cannot provide a service for a particular product.
The procedure for locking products, product classes or product groups on particular machines is similar in all dialogs.

This section provides information on the following subjects:
- "Lock by PGR" on page H-247
- "Lock by Product Classes" on page H-248
- "Lock Machines by Products" on page H-250
- "Skip next Machine" on page H-251
- "Customer-related Locks" on page H-252
- "Define Production Line" on page H-254
- "Skip Processes" on page H-255

### Lock by PGR

**Path:** `Capacity planning > Lock > Lock by PGR`

*Fig. H-167: Lock by PGR*

On this dialog, you lock particular product groups for one or more machines.
⇨ Tutorial, "Locks" on page H-90

#### Identification
**Product group**: Product group for which the machine is locked.

#### Machines
In the overview, the allocated machines are displayed.
**#**: Number of the sequence.
**Machine**: Number and name of the machine.

#### Buttons
**[New], [Delete]**: With these buttons you enable a new row or delete a marked entry.

**Arrow buttons**: With these buttons you can change the sequence of the work types.

#### Lock overview
In the list, the PGRs are displayed for which the locks were defined.

### Lock by Product Classes

**Path:** `Capacity planning > Lock > Lock by product types`

*Fig. H-168: Lock by product classes*

On this dialog, you lock a product class depending on the work type for one or more machines.
⇨ Tutorial, "Locks" on page H-90

> **Example**
> Two IG lines are available for IG production. Steel spacers can be fitted into the IG unit only on IG line no. 2 however.
> This is why product class IG must be locked for IG line no. 1 for the work type Fit steel spacer.

#### Identification
**Product class**: Product class for which the machine is locked.

#### Machines
The buttons are described for the `Lock by PGR` dialog.
⇨ "Lock by PGR" on page H-247

**#**: Number of the sequence.
**Work type**: Number and name of the work type.
**Machine**: Number and name of the machine.

**Total**: In the combination of product class and work type, the machine can be locked completely or partially.
- This machine is locked only for this product class (main product) and this work type.
- If the product class including the work type is component of a BOM, then the machine is locked completely, i.e. also for all other work types that affect the main product and its BOM components.

#### Lock overview
In the overview, the product classes are displayed for which the locks were defined.

### Lock Machines by Products

**Path:** `Capacity planning > Lock > Lock by products`

*Fig. H-169: Lock machines by products*

On this dialog, you lock a product depending on the work type for one or more machines.
⇨ Tutorial, "Locks" on page H-90

#### Identification
**Product**: Product for which the machine is locked.

#### Machines
The fields and buttons are described for the `Lock machines by products` dialog.
⇨ "Lock by Product Classes" on page H-248

#### Lock overview
In the overview, the products are displayed for which the locks were defined.

### Skip next Machine

**Path:** `Capacity planning > Lock > Skip next machines`

*Fig. H-170: Skip next machines*

On this dialog, you lock a machine depending on the next machine.

> **Example**
> If the drilling line automatically includes washing, then you can lock the next machine Washing or skip it to prevent doubled washing.

⇨ Tutorial, "Locks" on page H-90

#### Identification
**Machine**: Machine for which the next machine is locked.

#### Machine
The fields and buttons are described for the `Lock machines by products` dialog.
⇨ "Lock by Product Classes" on page H-248

#### Lock overview
In the overview, the machines are displayed for which the locks were defined.

### Customer-related Locks

**Path:** `Capacity planning > Lock > Customer-related locks`

*Fig. H-171: Customer-related locks*

On this dialog, you lock machines depending on the customer number, product or processing.

> **Example**
> If a customer insists that a particular drilling machine not be used for his orders, this drilling machine must be locked for him.

⇨ Tutorial, "Locks" on page H-90

#### Functions menu
Using this menu, you can extend the lock of a customer to the entire customer group or lift the lock.
The following entries are displayed:
- **Set lock:**
The lock is expanded to all customers of the customer group to which the customer displayed belongs. All affected customers will be listed in the overview.
- **Lift lock:**
The lock is deleted for all customers of the customer group. The customers are all removed from the overview.

#### Identification
**Customer**: Customer for whom the lock has been set.
**Product/processing**: Product or processing for which the machine is locked.
**Locked machine**: Machine that is locked.

#### Table
In the overview, all customers are displayed for whom locks are defined.
- **Customer no., Customer:**
Number and name of the customer.
- **Customer group:**
Customer group to which the customer belongs.
- **Place:**
Customer's headquarters.
- **Product no., Product:**
Number and name of the product for which the lock is defined.
- **Locked machine:**
Machine that is locked for the combination of customer and product.

### Define Production Line

**Path:** `Capacity planning > Lock > Define production line`

*Fig. H-172: Define production line*

On this dialog, you lock a machine depending on the previous machine.
⇨ Tutorial, "Define Production Line" on page H-93
The buttons are described for the `Lock by PGR` dialog.
⇨ "Lock by PGR" on page H-247

#### Identification
**Machine**: Machine for which the next machine is locked. This next machine is specified in the `Machines` group.

#### Machines
In the overview, the work types and allocated machines are displayed.
**#**: Number of the sequence.
**Work type**: Number and name of the work type.
**Machine**: Number and name of the machine.

**Total**: The machine can be locked partially or completely.
- The machine can be selected manually.
- This machine is completely locked for this work type.

#### Lock overview
In the overview, the machines are displayed for which the locks were defined.

### Skip Processes

**Path:** `Capacity planning > Lock > Skip processes`

*Fig. H-173: Skip processes*

On this dialog, you lock next processings depending on the machine.

> **Example**
> If the drilling line includes washing, then you can lock the next process Wash glass to prevent doubled washing.

⇨ Tutorial, "Locks" on page H-90

#### Identification
**Machine**: Machine on which the work type is locked.

#### Work types
In the overview, the allocated work types are displayed.
The buttons are described for the `Lock by PGR` dialog.
⇨ "Lock by PGR" on page H-247

**#**: Number of the sequence.
**Work type**: Number and name of the work type for which the machine is locked.

#### Lock overview
In the overview, the machines are displayed for which the locks were defined.

## Overviews

With various tables and graphics, you get an overview of the utilization on a particular date or in a period of time.

This section provides information on the following subjects:
- "Statistics" on page H-258
- "Area Graphic" on page H-259
- "Statistics by Order Area" on page H-260
- "Statistics by Order Area (short)" on page H-263
- "Accounts" on page H-264
- "Cost Centre Definitions" on page H-265

### Statistics

**Path:** `Capacity planning > Overview > Statistics`

*Fig. H-174: Statistics*

In this overview, you can display all orders that have been reported completed by a machine within a period of time.
The screen display applies only to the selected machine. The printout, however, shows all machines and the time costs.

#### Selection
**From, to**: Evaluation period. If you enter the same date in both fields, a daily evaluation is created.
**Machine**: Machine whose utilization is displayed.

#### Utilisation times
In the overview, the values for all quantities reported completed, by machine, are listed.
- **... Work type**
- **Pcs.**: Quantity reported completed.
- **Area**: Square meters reported completed.
- **Circumference**: Edge length in total.
- **Time**: Time required in total.
- **Machine**: Machine that reported the values.
- **Total time**: Total of the times for the selected machine.

### Area Graphic

**Path:** `Capacity planning > Overview > Graphic Areas > Legend`

*Fig. H-175: Area graphic - Weekly overview*

In this overview, you display a graphic overview of the utilization either by machine types or by production areas.
You can limit the display with the `Plant` menu to a particular plant or a customer.
The graphic can be opened from various dialogs. The display of the data is then filtered according to the initial dialog, e.g. per daily shift.

#### Period
**Date**: Date for which the graphic shall be created.
**Week**: You can only evaluate the day entered or the whole week.
- Only the selected day is evaluated.
- The evaluation considers the whole week (Monday through Sunday).

**Machine type, production area**: With the selection of the option, you specify to what the evaluation shall refer.

**[Legend]**: Shows/hides the legend with the significance of the colors in the graphic. The setting applies to all graphics.

#### Graphic
**Red lines**: The red line indicates the end of a shift.
**Left column**: The left column changes depending on the day or week view.
- Day view: shifts
- Week view: day's date.

### Statistics by Order Area

**Path:** `Capacity planning > Overview > Statistics by Order Area`

Order area statistics is product-based and includes all work types reported completed.
This dialog contains the following tabs:
- "Statistics by Order Area – Selection" on page H-261
- "Statistics by Order Area – Table" on page H-262

#### Statistics by Order Area – Selection

**Path:** `Capacity planning > Overview > Statistics by Order Area > Selection tab`

*Fig. H-176: Statistics by order area - Selection*

On this tab, you select the criteria according to which the overview of completion reports shall be created. If you want to display all details for a period, you must not limit the search with restrictions.

##### Evaluation period
**From, to**: Evaluation period. If you enter the same date in both fields, a daily evaluation is created.

##### Restrictions
In this group you can limit the selection.

> **Entry <n.e.>**
> If one of the fields shall not be taken into account, you have to delete the complete entry. `<n. e.>` means for example that the product type `<n. e.>` shall be excluded.
> To view information on all products, product classes, order areas, and production areas, leave all four fields empty.

**Product type**: The selected product type shall not be displayed.
**Product class**: The selected product class shall not be displayed.
**Order area**: The selected order area shall not be displayed.
**Production area**: The selected production area shall not be displayed.

##### Output / sorting
The left field displays the output options. The right field shows the sorting criterion. This setting determines the display of the results on the `Table` tab.
You move a selected entry into the right field or back into the left field with the arrow buttons.

##### List by
With the selection of the option, you specify which data shall be displayed:
- **Product type:** The evaluation shall refer to the product type.
- **Product class:** The evaluation shall refer to the product class.
- **Product:** The evaluation shall refer to the products.

#### Statistics by Order Area – Table

**Path:** `Capacity planning > Overview > Statistics by Order Area > Table tab`

*Fig. H-177: Statistics by order area - Table*

On this tab, the results of the evaluation is displayed. Based on the selection criteria you can determine, for example in which order area the glass is consumed.

##### Overview
The second column is filled in only if the sorting is made by production area and order area, no matter in which sequence this is done.

- **Production area, Order area:** Display depending on the sorting criterion.
- **Product, Product class, Product type:** Display depending on the selection of the sorting criterion.
- **Process:** This field displays the work types.
- **Quantity:** Quantities produced.
- **Sqm:** Area produced.
- **Lm:** Linear meters produced (edges)
- **Time costs:** Time costs determined.
- **Material costs:** Material costs determined.

### Statistics by Order Area (short)

**Path:** `Capacity planning > Overview > Statistics by Order Area (short)`

On this dialog, you can display an abbreviated list of the evaluation by order areas, which is automatically sorted according to the two criteria `Order area` and `Production areas`.
The fields are described for the `Order area statistics` dialog.
⇨ "Statistics by Order Area" on page H-260

### Accounts

**Path:** `Capacity planning > Overview > Accounts`

*Fig. H-178: Accounts - Selection*

On this dialog, you can display to which cost centres or order areas particular products, product classes or product types were booked. The data is read out of the orders. Archived orders are not taken into consideration.

#### Cost centres menu
Using this menu, you can open the Cost centre definition dialog to create or edit the cost centres.
⇨ "Cost Centre Definitions" on page H-265

#### Evaluation period delivery date
**From, to**: Evaluation period. If you enter the same date in both fields, a daily evaluation is created.

#### Sorted by
With the selection of the option, you specify how the display shall be sorted:
- **Cost centres:** These are the cost centres that you have created for capacity planning.
⇨ "Cost Centre Definitions" on page H-265
- **Order areas:** Order areas from the A+W Business Pro master data.

> **Define cost centres**
> You define new cost centres the same way as the preview columns in the Production module.

#### List by
With the selection of the option, you specify whether the evaluation is displayed by product type, product class or according to the individual products.

#### Overview
The following data is displayed in the overview:
- **Cost centre:** Name of the cost centre. The names are specified on the Cost centre definition dialog.
⇨ "Cost Centre Definitions" on page H-265
- **Order area:** Order area to which the cost centre is assigned.
- **Product type, product class, product:** The display of the appropriate data depends on the option that was selected on the Selection tab.
- **Qty:** Quantity of sheets produced.
- **Area:** Total area of the sheets produced.
- **Material costs:** Material costs of the sheets produced.

### Cost Centre Definitions

**Path:** `Capacity planning > Overview > Accounts > Cost centres menu`

*Fig. H-179: Cost centre definition*

On this dialog, you specify the cost centres for the evaluation of production data and costs.

> Before you create cost centres, you should consider in which sequence the cost centres should be queried.
>
> **Example TG**
> First you query whether this is a TG with processing (cost centre no. 7 with prio 19).
> If this is not the case, the follow-up query starts.
> The TG that is not processed flows automatically into the cost centre TG (cost centre no. 6 with prio 20).

> **Define cost centres**
> You define new cost centres the same way as the preview columns in the Production module.

**No.**: Number of the cost centre.
**Name**: Name of the cost centre.
**MPT**: Main product type. In this field you enter the product type for which the evaluation shall be done.
**No 1, No 2**: These entries refer to the fields `Type 1` and `Type 2`. Here you enter the number for the product type or product class of Type 1 or Type 2 or 0 for no specification.
**Type 1, type 2**: Product type or product class that is BOM element of the main product type.
- 0 = no specification
- 1 = product type
- 2 = product class
Example: You search for the Product class (Type 1 = 1) Processings (No 1 = 20), which is a component of TG (MPT = 2).
**Priority**: Number of the sequence in which the query of the cost centres shall be done.
**Exclusion**: You can exclude a product from the rule. The product number must be in brackets.

> **Example**
> All TG sheets are seamed. Therefore, seamed TG sheets shall not flow into the cost centre 'Processed TG'.
> You exclude this by entering the appropriate product number (in brackets).

### Lisec Interface
This dialog is only released if you are working with an appropriate interface.

## Capacity Planning

**Path:** `Production > Capacity planning`

The Production module offers various dialogs for capacity planning purposes. Apart from transferring data to production, you can use this module to monitor the production progress by means of reports.

This section provides information on the following subjects:
- "Scheduling" on page H-268
- "Production Reports" on page H-291
- "Control Station" on page H-325

### Scheduling

Time and material costs can only be calculated for orders that are scheduled in capacity planning. Orders can be scheduled automatically at defined intervals or manually.

This section provides information on the following subjects:
- "Number Manager" on page H-268
- "Schedule Number Manager" on page H-269
- "Change Criteria (Search Date)" on page H-272
- "Delivery Date" on page H-274
- "Book Order" on page H-275
- "Scheduling Result" on page H-280
- "Machine Selection in Case of Bottleneck" on page H-281
- "Order Numbers" on page H-283
- "Split Items" on page H-284
- "Item Times" on page H-286
- "Machine Failure" on page H-287
- "Residue Transfer" on page H-290
- "Shift Settings" on page H-183

#### Number Manager
**Path:** `Production > Capacity planning > Booking > Number manager`

You have the possibility to schedule several orders manually at once in capacity planning. For this, the orders are collected in a number manager.

On the `Schedule orders` dialog, you can select the number manager and schedule the orders. The program shows all number managers created for documents.
⇨ "Schedule Number Manager" on page H-269

On the `Number manager` dialog, you can open the `Production overview` dialog for the order you have selected in the overview. That dialog is described in detail in the Sales section.
⇨ Sales, "Status Message" on page C-498

The `Number manager` dialog and the associated menus are the same for all modules. It is described in detail in the Sales section.
⇨ Sales, "Number Manager" on page C-543

#### Schedule Number Manager
**Path:** `Production > Capacity planning > Booking > Book NM`

Using a number manager, you schedule all orders manually that match the minimum status.

This section provides information on the following subjects:
- "Functions Menu” on page H-269
- "Options Menu" on page H-269
- "Schedule Orders (Dialog)" on page H-270

##### Functions Menu
**Path:** `Production > Capacity planning > Booking > Book NM > Functions menu`

Using this menu, you can display the history of the selected order. The history is described in detail in the Sales section.
⇨ Sales, "History" on page C-478

##### Options Menu
**Path:** `Production > Capacity planning > Booking > Book NM > Options menu`

Using this menu, you can determine the default setting of the dialog and open other dialogs without leaving the current dialog. You can activate or deactivate options. The setting will not be reset when you close the dialog. The following entries are displayed:
- **Mode date search:**
Opens the Change criteria dialog on which you can specify the criteria for the schedule search.
⇨ "Change Criteria (Search Date)" on page H-272
- **Item check:**
When the order is scheduled, the program checks its share in the daily capacity. The percentage is defined on the Work types dialog.
⇨ "% Limit" on page H-189
- **Old dwell day mode:**
This setting is only required if you want to retain the old mode for dwell days (= Transition matrix).
- **Check for ST:**
If the set-up time has been defined for several work types performed for an order item, this time shall be charged just once per item.

#### Schedule Orders (Dialog)
**Path:** `Production > Capacity planning > Booking > Book order`

*Fig. H-180: Schedule by number manager*

On this dialog, you transfer the orders from a number manager to capacity planning. You start the transfer with the menu `Start > Execute`.
⇨ Tutorial, "Scheduling Orders" on page H-108

##### Identification
**Client**: Selection of the client whose orders shall be scheduled.
**Area**: Selection of the order area whose orders shall be scheduled.
⇨ Master Data, "Order Areas" on page B-983
**Employee**: Employee logged in.
**Number Manager**: If you have selected a number manager, all orders are transferred that are in this number manager and have achieved the minimum status.

**Order priority**: The field is only released if you have selected the `Take over changed priority in order setting` on `Company data > Capacity planning tab > Scheduling priority` field.
Orders are usually scheduled with Normal priority. Only e.g. for rush orders which have to have shorter through times, you will have to select the appropriate priority.
- **Normal:** The order is scheduled according to the default settings.
- **Urgent:** The order must be scheduled with top priority.
- **Release order:** The order is only produced if the customer calls the items.
- **Extra:** This priority means that the order shall be produced from residue (plates) left over from cutting other orders.

> **Consider order priority**
> If in addition to the order priority `Normal` the priority `Urgent` shall be considered, a special transition time must be defined for the corresponding combination of production areas. This applies to all times that can be shortened for rush orders if required.
> ⇨ "Transition Times" on page H-192
> ⇨ "Transition Matrix" on page H-210

**Behavior in case of delivery date problems**: With the selection of the option, you specify how the program shall react to problems during scheduling:
- **No automatism:** The order shall not be automatically scheduled for the next possible production date. If this option is chosen, Delivery date dialog opens on which you can specify the settings for scheduling.
⇨ "Delivery Date" on page H-274
- **Next delivery date:** The order shall be scheduled on the next possible delivery date. The new delivery date is written back to the order.
- **Schedule for delivery date:** The order shall be scheduled for the original delivery date, even if this exceeds the machine capacities. You can select this option if you are sure that you can postpone other, already scheduled orders.
- **Infinite capacities:** The order will be scheduled regardless of the actual capacities.

#### Change Criteria (Search Date)
**Path:**
- `Production > Capacity planning > Booking > Book NA > Options menu > Search date`
- `Production > Capacity planning > Booking > Book order > Functions menu > Mode date search`

*Fig. H-181: Settings for schedule search*

On this dialog, you specify the criteria for manual scheduling or in case of capacity problems. The settings are valid only for the current scheduling.

##### Determine the production date
With these settings you override the default settings from the company data. The overridden settings apply only to the current session:
- **Autom. normal capacity:** The orders will be scheduled based on the available shift times. Overbooking is impossible. This is the default setting (closed capacities).
- **Automatic full days:** This setting ignores the specifications for the number of shifts and hours in the calendar. Scheduling is based on a workday of 24 hours in this case (open capacities). This applies only to common workdays, not to holidays.
- **Change machine only:** If capacities are fully utilized, the program will automatically search for another machine. If this is used to capacity as well, scheduling is interrupted and manual intervention is required.
- **Schedule without check:** This setting represents an open shift. This means e.g. that despite a shift time of 8 h, 16 h can be scheduled as well. The program will issue no report if a day's capacity is fully utilized. This option should only be used in exceptional cases.

##### Mode for aligning the machines
If you work with several machines that can perform the same work types, scheduling can consider these machines in different ways:
- **Automatic:** The program automatically searches for the most cost- and time-effective machine and schedules the orders on this machine. This is the default setting.
- **Semi-automatic:** The program offers the alternative machines for selection. If the delivery date cannot be adhered to, you must intervene.
- **Manual:** With this option you must intervene manually for each possible change (machine, shift, etc.). Alternative machines can only be selected for the manual scheduling or rescheduling.

##### Options
**Closing time**: For manual scheduling, you can specify the point in time up to which orders can be scheduled. This setting will be kept until the next change is made.

> **Example**
> You get a new order on Friday at 12 a.m. For manual scheduling, you enter 14 h although the shift goes to 16 h. This ensures that the order will not be scheduled if it cannot be produced on this day. You thus prevent residual quantities of not-yet-begun orders from arising, which must then be rescheduled on the following day.
> If the order cannot be scheduled due to the closing time, an appropriate message will be displayed on the Delivery date dialog. You then have to change the delivery date.

Closing times are generally defined on the Shift settings dialog.
⇨ "Shift Settings" on page H-183

**Reduced control**: Scheduling usually searches for each item for free capacities to schedule the order items. However, an order may contain items with the same BOM structure, where only the sizes are different.
- The entire BOM structure is checked for each item.
- If the BOM structure is the same, scheduling is based on the previous item without checking the BOM again. This is the default setting.

The program notes the start date of production of the first item, e.g. on the grinding machine. The next item starts from that date, starts the capacity of this machine and if it this already running to capacity, goes to the previous shift or the previous day. The next item starts from that new date with its capacity check, etc.

**Do not split orders**: If an order cannot be produced on one day, the order has to be split.
- The order can be split so that production is distributed across several days.
- The order shall not be split. The search for a suitable date must continue until all capacities needed for this order are free.

#### Delivery Date
**Path:** `Production > Capacity planning > Booking > Book order, Book NM > Schedule`

*Fig. H-182: Delivery date for scheduling*

On this dialog, you specify manually when or how the order shall be scheduled.
The dialog is displayed if the delivery date from the order cannot be kept because the capacity check did not come up with a suitable free date. These manual settings will be recorded in the order history.

The following options are available for selection:
- **Define automatically:** With this option, the next possible delivery date is determined and saved in the order. The customer's route days will be taken into account. This option is based on forward scheduling.
- **Choose delivery date:** With this option, you select another delivery date. The program then checks again whether sufficient capacities are available on that date. This process continues until the order can be scheduled. When scheduling is successful, the new date is saved in the order.
- **Schedule for delivery date:** With this option, the default times are ignored and the program tries to schedule the order for the delivery date. The search for free capacities goes one day back at a time until the current date. If by then no capacities are found, the order is scheduled on this day regardless of whether or not capacities are free.
- **Infinite capacities:** With this option, the order is scheduled for the delivery date regardless of whether or not capacities are free.
- **Individual setting:** With this option, it is first possible to determine the delivery date manually. After that, the program stops for each work type included in the order. You have to specify the appropriate machines, the production day, and the shift manually.

**[End]**: With this button, you abort the scheduling of the current order. After you have answered a security query with [Yes], the program proceeds with the next order in the number manager. The unscheduled order has to be scheduled separately afterwards.

#### Book Order
**Path:** `Production > Capacity planning > Booking > Book order`

On this dialog, you schedule an individual order or an individual item of an order manually in capacity planning.

This section provides information on the following subjects:
- "Functions menu" on page H-276
- "Options menu" on page H-277
- "Settings group" on page H-276
- "Book Order (Dialog)" on page H-277

##### Functions menu
**Path:** `Production > Capacity planning > Booking > Book order`

Using this menu, you can open other dialogs without closing the Schedule order dialog.

###### Current order group
- **Scheduling result:** Opens the Scheduling result dialog on which you can check the results of the scheduling.
⇨ "Scheduling Result" on page H-280
- **Apply priority:** Applies the changed priority and writes it back to the order. Only if you write back the change to the order is it considered during the scheduling.
- **Delete scheduling:** Deletes the scheduled order from capacity planning, e.g. to scheduled it again using changed criteria or in case of cancellations. The order is deleted from capacity planning, the reserved capacities are released again.
- **Transfer to production:** Transfers the order directly to production.
- **Display messages:** After scheduling, displays a message with various information about the scheduling. The entry is only released if you are logged in with administrator rights.

###### Settings group
- **Search date:** Opens the dialog by the same name on which you can specify the criteria for the schedule search.
⇨ "Change Criteria (Search Date)" on page H-272
- **Shift times:** Opens Shift time settings dialog where you can define the shift transition and the closing time.
⇨ "Shift Settings" on page H-183
You must have administrator rights to open the dialog. In addition, the `Use change of shift table` checkbox must be ticked on the Company data dialog.
⇨ "Use change of shifts table" on page H-182
- **Select shift:** Enables the `Shift` field to enter the requested shift.
- **Residue transfer:** Opens Residue transfer dialog where you can define the status up to which orders shall be checked for residue.
⇨ "Residue Transfer" on page H-290

##### Options menu
**Path:** `Production > Capacity planning > Booking > Book order`

Using this menu, you can determine the default setting of the dialog. You can activate or deactivate options. The settings will not be reset when you close the dialog. The following entries are displayed:
- **Old dwell day mode:** This setting is only required if you want to retain the old mode for dwell days (= Transition matrix).
- **Check for ST:** If the set-up time has been defined for several work types performed for an order item, this time shall be charged just once per item.
- **Item check:** When the order is scheduled, the program checks its share in the daily capacity. The percentage is defined on the `Work types` dialog.
⇨ "% Limit" on page H-189
- **Consider closing time for scheduling:** The program shall check until when orders can be scheduled for a shift.
⇨ "Shift Settings" on page H-183

#### Book Order (Dialog)
**Path:** `Production > Capacity planning > Booking > Book order`

*Fig. H-183: Book order manually*

On this dialog, you schedule an individual order or an individual order item manually in capacity planning.
⇨ Tutorial, "Scheduling Orders" on page H-108

##### Order information
**Order**: Entry of the order number.
**Customer**: Display of the customer name.
**Shipping date**: Shipping date from the order. You can overwrite the date. The change is written back to the order. If you have ticked the checkbox `Keep delivery date`, you cannot choose another date.

> **Pushing up production**
> In order to push up the scheduling of production, you have to change the shipping date first before ticking the checkbox `Keep delivery date`.

**Shift**: Specification of the shift number in which the order shall be produced. The field is released in menu `Functions > Settings group > Select shift`.
**Status**: Current order status.
**Priority**: By default, the orders are scheduled with the priority `Normal`. You can select another priority and use the `Functions menu > Settings group > Apply priority` to write it back to the order. Only after that is the new priority considered for scheduling. The following entries are available for selection:
- **Normal:** The order is scheduled according to the default settings.
- **Urgent:** The order must be scheduled with top priority.
- **Release order:** The order is only produced if the customer calls the items.
- **Extra:** This priority means that the order shall be produced from residue (plates) left over from cutting other orders.

> **Consider order priority**
> If in addition to the order priority `Normal` the priority `Urgent` shall be considered, a special transition time must be defined for the corresponding combination of production areas. If these have not been defined, the order will be scheduled with `Normal` priority.
> ⇨ "Transition Times" on page H-192
> ⇨ "Transition Matrix" on page H-210

##### Options
**Schedule individual item**: You can schedule individual items from an order.
- All items of the order are scheduled.
- The field for entry of the item number is released. Only the defined item will be scheduled.

**Item number**: Entry of the item that shall be scheduled. The field is only released if the `Schedule individual item` checkbox is ticked.

**Also use priority -1**: Machine selection takes the machine priorities into account. By default, the program checks the availability of the machine with the highest priority. Priority -1 is usually assigned to the machines for manual selection, e.g. manual cutting.
- Machines with priority -1 can only be scheduled manually.
- ☑ Machines with priority -1 are included in the scheduling process.

**Keep delivery date**: If the utilization of the machines makes the delivery date impossible, it can be postponed.
- Order scheduling permits postponing the delivery date.
- The order shall be scheduled so that the delivery date stated in the order is kept. With this setting, you will not be able to choose another date in field `Shipping date`.

**Earliest production start**: If you have a delivery date that is far in the future, you can specify the earliest date for production start.

##### Current scheduling
In this group is displayed which item is currently being scheduled.

##### Item/processings
In the overview, the product names and processings of the individual items are displayed.

#### Scheduling Result
**Path:** `Production > Capacity planning > Booking > Book orders > Functions menu > Scheduling result`

*Fig. H-184: Result of the scheduling*

On this dialog, you check how the order was scheduled.

##### Processes
In the overview, the items are displayed per work type.
- **Item:** Item number from the order.
- **Machine:** Name of the machine.
- **Work type:** Work type that is performed on the machine.
- **Time:** Time scheduled per item and work type. The totals line shows the total time scheduled for this order.
- **Pcs.:** Number of process steps, e.g. 10 sheets to be cut but 4 x 10 units for rounded corners.
- **Date:** Production date.
- **Shift:** Shift in which the item is scheduled.
- **Costs:** Costs per work type and item. In the total line, the total costs for the order are displayed.

##### Sort result
With the selection of the option, you specify how the display shall be sorted:
- **By item:** The work types are listed per item.
- **By production date:** The items are listed according to the date of the work type in question.

##### Totals
In this group, the totals for the times and costs are displayed, which were calculated for the scheduled order.

#### Machine Selection in Case of Bottleneck
**Path:** `Production > Capacity planning > Booking > Book order > Scheduling > (bottleneck)`

*Fig. H-185: Bottleneck during scheduling - Select machine*

On this dialog, you select another machine manually. The dialog is displayed automatically at scheduling if the default machine with the priority 9 is fully utilized.
⇨ Tutorial, "Capacity Problems" on page H-114

##### Capacity bottleneck
**Order, customer, shipping date**: Display of the order number, the customer name, and the shipping date stated in the order.
**Item/element/sub-item**: Display of item number, level of the BOM and for split items, the number of the sub-item where the capacity bottleneck occurs.
**Quantity**: Quantity of the item or sub-item.
**Product, dimensions**: Product name and dimensions of the order item.
**Work type**: Work type for which the bottleneck occurs.

##### Production
**Date**: Scheduled production date. With the arrow buttons, you can move the date forward or backward.
**Shift**: Scheduled shift. With the arrow buttons, you can move the shift forward or backward on the same day. If you are working with just one shift, the date is shifted.

##### Valid machines
In the overview, all machines are displayed which can also perform this work type.
- **Machine:** Alternate machines.
- **Time required:** Time required for the process, for the item and quantity displayed.
- **Time reserved:** Time that is already reserved for other orders on that machine.
- **Set-up time:** Time that is required to set up the machine if the items displayed shall be produced.
- **Maximum time:** Shift time of the machine on the selected date.

##### Buttons
**[Overview]**: Opens the `Order numbers` dialog to check which orders are already scheduled on the machine for the current settings.
⇨ "Order Numbers" on page H-283
**[Alignment]**: Currently not used.
**[Split item]**: Opens the `Split item` dialog to split the item into sub-items.
⇨ "Split Items" on page H-284
**[Criteria]**: Opens the `Change criteria` dialog.
⇨ "Change Criteria (Search Date)" on page H-272
**[Schedule]**: Schedules the item based on the set conditions. Depending on the setting, you have to schedule each work type per item individually. If all items are scheduled, a message with the changes is displayed.
**[Schedule previous day]**: Schedules the item based on the set conditions on the previous day. For this, you first have to select the last shift of the previous day in the `Shift` field.

#### Order Numbers
**Path:** `Production > Capacity planning > Booking > Book order > Schedule machine in case of bottleneck > [Overview]`

*Fig. H-186: Bottleneck during scheduling – Overview of the scheduled orders*

On this dialog, you check which orders are already scheduled on the machine at the set conditions.

#### Split Items
**Path:** `Production > Capacity planning > Booking > Book order > Scheduling > Machine selection in case of bottleneck > [Split items]`

*Fig. H-187: Bottleneck during scheduling – Split item*

On this dialog, you split an order item into several sub-items.
⇨ Tutorial, "Capacity Problems" on page H-114

##### Item information
**Order, item**: Order number and number and product name for the order item.
**Product, quantity**: Product number and quantity of the order item.

##### Split
In this group, you specify how the item shall be split. The splitting of the item into sub-items is displayed in the overview.
If you have ticked the `Preset production date` checkbox in the `Options` group, in addition to the quantity, the date and shift are also displayed. You can enter the requested values directly in those fields.

**Quantity**: Specification of the quantity. Using the buttons below, you specify whether the quantity shall be interpreted as shift or as quantity.
**[Reset splitting]**: Resets the splitting of the item. Then you can try other possibilities for splitting the item.
**[Quantity = Shifts]**: The value in the `Quantity` field shall refer to shifts, e.g. 2 shifts. The quantity of the item is split evenly across the number of shifts. In the overview, you can overwrite the values.
**[Quantity = units per shift]**: The value in the `Quantity` field shall refer to the units per shift, e.g. 50 units per shift.
If you have not made any specifications about the quantity, as many sub-items are generated as the settings from the company data permit, e.g. 50% of the shift. In the overview, you can overwrite the values.
⇨ "Fill shift in case of item splitting" on page H-180

##### Options
**Maximum work types for preset date**: The field is only released if the `Preset production date` checkbox is ticked. The field must not be empty.
You can specify production dates for the item split. In this case, you can also specify starting with which work type these dates shall not apply. This setting makes sense, e.g., because the sub-items are not packaged and shipped separately.

**Reduced control**: Normally the scheduling checks for each item on which day there are still capacities available to schedule the item there.
An order can however include items with the same BOM structure where only the sizes are different.
- The entire BOM structure is checked for each item.
- With the same BOM structure, the scheduling assumes the previous item without checking the BOM. This is the default setting.
The program notes the start date of production of the first item, e.g. for the grinding machine. The next item starts precisely on this date in order to check the capacity for this machine and goes, if the machine is fully utilized on this day, to the previous shift or the previous day. The next item, in turn, relies on this new date for the checking of the capacity, etc.

**With locks**: When splitting, the remaining shift time for other orders can be locked, e.g. so that the machine does not have to be set up again.
- Remaining time of the shift or the day in question is not locked for other orders.
- Only sub-items created by splitting the order will be produced. The remaining time will not be scheduled otherwise.

**Preset production date**: You can specify a date per sub-item.
- The date cannot be preset.
- In the overview, the columns `Date` and `Shift` are displayed, and in the `Options` group the field `Max. work type for preset date`.

**[OK]**: Applies the data. Scheduling is continued with the new sub-items.
**[End]**: Interrupts the splitting. The `Machine selection in case of bottleneck` dialog is displayed again in the foreground.
**[Overview]**: Opens the `Item times` dialog.
⇨ "Item Times" on page H-286

#### Item Times
**Path:** `Production > Capacity planning > Booking > Book order > Scheduling > Machine selection in case of bottleneck > [Split items] > [Overview]`

*Fig. H-188: Bottleneck during scheduling – Overview of the item split*

On this dialog, you check the times that are required for the current item. The times are displayed in red for which no capacities are available.

#### Machine Failure
**Path:** `Production > Capacity planning > Booking > Machine Failure`

Machines can be locked temporarily or completely. Scheduled orders have to be rescheduled in this case. The query regarding rescheduling appears when you lock a machine for which orders have already been scheduled. You should therefore set the search mode first.
⇨ "Change Criteria (Search Date)" on page H-272

This section provides information on the following subjects:
- "Functions Menu" on page H-287
- "Options Menu" on page H-288
- "Machine Failure (Dialog)" on page H-289

##### Functions Menu
**Path:** `Production > Capacity planning > Booking > Machine Failure`

Using this menu, you can open other dialogs without closing the Machine Failure dialog.

###### Date search group
- **Change criteria:** Opens the dialog by the same name on which you can specify the criteria for the date search.
⇨ "Change Criteria (Search Date)" on page H-272

###### Residual quantities group
- **Transfer:** Opens the `Residual quantity transfer` dialog on which you can specify up to which status orders shall be checked for residual quantities.
⇨ "Residue Transfer" on page H-290

###### Scheduling group
- **Schedule selection:** Opens the `Schedule order` dialog to reschedule the selected orders on other machines.
⇨ "Book Order" on page H-275

###### Capacity planning group
- **Shifts:** Opens the `Shift settings` dialog on which you can specify the shift transition and closing times.
⇨ "Shift Settings" on page H-183
You must have administrator rights to open the dialog. In addition, the `Use change of shift table` checkbox must be ticked on Company data dialog.
⇨ "Use change of shifts table" on page H-182

##### Options Menu
**Path:** `Production > Capacity planning > Booking > Machine Failure`

Using this menu, you can determine the default setting of the dialog. You can activate or deactivate options. The settings will not be reset when you close the dialog.

###### Dwell days group
- **Use old mode:** This setting is only required if you want to retain the old mode for dwell days (= Transition matrix).

###### Set-up time group
- **Check:** If the set-up time has been defined for several work types performed for an order item, this time shall be charged just once per item.

###### Scheduling group
- **Check item:** When the order is scheduled, the program checks its share in the daily capacity. The percentage is defined on the `Work types` dialog.
⇨ "% Limit" on page H-189
- **Obey closing time:** The program shall check until when orders can be scheduled for a shift.
⇨ "Shift Settings" on page H-183

#### Machine Failure (Dialog)
**Path:** `Production > Capacity planning > Booking > Machine Failure`

*Fig. H-189: Machine Failure*

On this dialog, you store downtimes for your machines, so that capacity planning can consider this during the planning. Such downtimes arise, e.g. due to maintenance work or repairs.
⇨ Tutorial, "Locks" on page H-90

##### Selection
**Machine**: Selection of the machine to which the downtimes shall be assigned. Downtimes are entered in days, not in shifts.
**Downtime from, to**: Period during which the machine is probably unavailable. If you save the entered times, the affected orders are displayed in the overview. These orders can automatically scheduled for other machines. A query appears in which you can confirm or reject the rescheduling.

##### Data
In the overview, all machines are listed for which downtimes are defined.

##### Affected orders
In the overview, all orders are listed that are scheduled on the selected machine. The `Hours` column shows the time reserved for the order on the locked machine.

#### Residue Transfer
**Path:** `Production > Capacity planning > Booking > Book order > Functions menu > Settings group > Residue transfer`

*Fig. H-190: Transfer of residual quantities*

On this dialog, you specify the status up to which the workflow task searches for non-produced residual quantities from the previous day. This includes only orders and items which should have been produced the day before, but have not been started yet.
⇨ Tutorial, "Remaining Quantities from Previous Day" on page H-139

### Production Reports

The current production status can be included in capacity planning so that in addition to the order status, other lists can be drawn up, e.g. production lists and diagrams on the production status.

If you are not working with reports from barcoding, on the dialogs for manual completion reporting at the various production stations, you can report batches, orders, or order items complete.

On the dialogs, you can display all orders or only orders that have not been reported completed yet. You can enter completion reports or breakage reports.
The rights to report completed can be limited by the administrator on special dialogs.

This section provides information on the following subjects:
- "Date" on page H-292
- "Graphic" on page H-295
- "Batch" on page H-296
- "Settings for Batch Completion Report" on page H-297
- "Manual Completion Report" on page H-298
- "Settings for Manual Completion Reports" on page H-301
- "Production Lists" on page H-302
- "Settings for Production Lists" on page H-306
- "Production Level Orders" on page H-307
- "Report List" on page H-318
- "Change Production Times" on page H-319

#### Date
**Path:** `Production > Capacity planning > Completion reports > Date`

*Fig. H-191: Completion report by date*

On this dialog, you report the production of an order, order item or sub-item completed at a certain machine. Once the first element of an item has been reported completed, the corresponding process cannot be changed.
⇨ Tutorial, "Report manually Order completed" on page H-143

##### Functions menu
Using this menu, you open a graphical display of the orders produced in the production area in question.
⇨ "Graphic" on page H-295

##### Selection
**Production date**: Date of production.
**Show items reported complete**: You can display per order which items were reported completed.
- Only the items are displayed that are not yet reported completed.
- All items are displayed.

**Production area**: You can limit the display to the machines of a particular production area.
- All production areas are displayed.
- Only the machines of the selected production area are displayed. The field for selection of the production area is released.

##### Machines
In the overview, all machines are displayed that correspond to the selection criteria.

##### Details
In this list, the totals reported for the quantities and times are displayed.
- **Completed:** Quantity produced on the current day.
- **Pcs.**: Total pieces that are to be produced on this machine on this day.
- **Time:** Time (in hours) that is required to produce the total quantity on this machine.
- **Remaining time:** Remaining time for the not yet produced quantities.

##### By unit
In the overview, all items are displayed that are produced on the machine on the selected date. You can report an item partially or entirely completed.
- **Item:** Item number from the order.
- **BOM ID:** BOM ident number, i.e. the BOM level.
- **Sub item(s):** Sub-items created at scheduling by the splitting of the item.
- **Process:** Work type.
- **Product/Processing:** Product name.
- **Pcs.:** Item quantity.
- **Size:** Dimensions of the item.
- **Already completed:** Quantity produced on the current day.
- **Completion report:** Entry of the quantity to be reported completed.
- **Fixed:** As soon as the first piece of an item is reported the checkbox is ticked. The process cannot be changed any more. If you tick this checkbox (manually) while no completion report has been made yet, you will force the production of the item on the set date, on the defined machine.

##### P.O. elements
In the overview, all order items with purchased elements are displayed.
- **Order, Item:** Order and item number from the order.
- **Element:** If the purchased element is a processing, the component is displayed that will be processed.
- **Article/processing:** Product name of the purchased element.
- **Pcs.:** P.O. quantity.
- **Size:** Dimensions of the item.
- **Ordered for:** Requested delivery date.
- **Delivered quantity:** Quantity already delivered.
- **Required on, shift:** These two columns show where and when the purchased elements will be needed.

#### Graphic
**Path:** `Production > Capacity planning > Completion reports > Date > Functions menu > Graphic`

*Fig. H-192: Graphical display of the quantities produced*

This display presents the quantities of a production area, a machine or an order item in graphical form.
- **Blue graphic:** Quantities that have not yet been reported completed.
- **Green graphic:** Quantities that have been reported completed.

#### Batch
**Path:** `Select Production > Capacity planning > Completion report > Batch`

*Fig. H-193: Report batch completed*

On this dialog, you report a production batch completed manually if you are not working with the status reports from barcoding.

##### Functions menu
Using this menu, you open the `Settings for batch completion report` dialog to select the production area for the completion report.
⇨ "Settings for Batch Completion Report" on page H-297

##### Selection
With the option, you specify the selection of the orders for the completion report:
- **By batch number from, to:** An entire batch is reported completed. With the selection of this option, the fields from and to are released, where you can enter a batch number of a range of batch numbers. The batch numbers are assigned in A+W Production.
- **By number manager:** The orders of a whole number manager are reported completed. With the selection of this option, the field for selecting the number manager is released.

**Enter date**: By default, the current date is taken over for the completion report.
- The current date is taken over for the completion report.
- The field for the specification of the date is released. The batch is reported completed with the changed date.

##### Production areas / machines
In this field, the production areas or machines are displayed for which the batch is reported completed. The required areas or machines are selected in the Selection menu on the `Settings for batch completion report` dialog.
⇨ "Settings for Batch Completion Report" on page H-297

##### Table
In the overview, all orders are listed that match the criteria in the `Selection` group.

#### Settings for Batch Completion Report
**Path:** `Select Production > Capacity planning > Completion report > Batch > Functions menu > Production areas/machines`

*Fig. H-194: Select areas or machines for completion report*

On this dialog, you specify for which production area or which machines the batch is reported completed.

##### Completion report
With the selection of the option, you specify to what the completion report applies:
- **Whole order:** With this option, all items and thus the entire order is reported completed. For the completion report, the current date or the specified date is taken over.
- **Selected production areas:** With this option, the production areas are listed in the `Selection` field. You can select one or more entries. The selected production areas are displayed on the `Batch` dialog. The batch numbers can be reported completed for the selected production areas.
- **Selected machines:** With this option, the machines are listed in the `Selection` field. You can mark one or more entries. The selected machines are displayed on the `Batch` dialog. The batch numbers can be reported complete for the selected machines.

#### Manual Completion Report
**Path:** `Select Production > Capacity planning > Completion report > Manually`

With this dialog, you can report individual orders or order items complete.

This section provides information on the following subjects:
- "Functions Menu" on page H-298
- "Options Menu" on page H-299
- "Manually (Completion Report)" on page H-299

##### Functions Menu
**Path:** `Select Production > Capacity planning > Completion report > Manually`

Using this menu, you can open the dialog for the settings to limit completion reports to particular production areas.
⇨ "Settings for Manual Completion Reports" on page H-301

##### Options Menu
**Path:** `Select Production > Capacity planning > Completion report > Manually`

Using this menu, you can determine the default setting of the dialog. You can activate or deactivate options. The settings will not be reset when you close the dialog. The following entries are displayed:
- **Scanning:** Enables the field for entering the barcode (next to the order number).
- **Adjust prod. date:** By default, the date of the completion report is entered as production date. You can specify another date, e.g. that of the previous day.

##### Manually (Completion Report)
**Path:** `Select Production > Capacity planning > Completion report > Manually`

*Fig. H-195: Manual completion report*

On this dialog, you report orders partially or entirely completed. In addition to the completion reports, you can also record breakage reports. The dialog can be used by employees in production. The completion reports can be set here so that the employee can report completed only own production area and certain machines.
⇨ Tutorial, "Report manually Order completed" on page H-143

###### Completion report
**Order**: You can enter the order number or record by scanner. The field for the barcode is released in the `Options` menu.

**From item, to item**: You can report an individual item or several items of an order. If you enter several items, only the whole items can be reported.
**Total qty.**: Display of the total quantity of processings for the items you have entered.

> **Example**
>
> | | Cutting | Shipping |
> | :--- | :--- | :--- |
> | Item 1: 12 x IG | 24 pcs. | 12 pcs. |
> | Item 2: 6 x single glass | 6 pcs. | 6 pcs. |
> | Item 1 - 2: | 30 pcs. | 18 pcs. |

**Quantity**: Quantity to be reported. The field is released only if you have entered a single item number, e.g. 2.

**Item complete**: Scanning will report one unit completed for every scanned order item.
- Every item will be scanned until the required quantity is reached.
- The scanned item is reported completed as a whole.

**With quantity**: You can also report a partial quantity of the scanned item completed.
- One piece is reported completed for the scanned item.
- The quantity entered in `Quantity` field will be reported completed for the scanned item.

**[Report items completed (F9)]**: Only the selected items are reported completed.

**[Report order completed (F12)]**: The entire order is reported completed.

###### Preset date
**Enter date**: By default, the current date is taken over for the completion report. You can change the date.
- The present date will be used for the completion report.
- The fields for the date and the shift are released.

**Shift**: The field is released only if the `Enter date` checkbox is ticked. You can then enter the shift to which the report applies.

###### Report type
With the selection of the option, you specify the type of report:
- **Completion report:** The specified quantity is reported completed.
- **Breakage report - entry:** The specified quantities are reported as broken at the machine entry. They must be reproduced by the previous machine.
- **Breakage report - exit:** The specified quantities are reported as broken at the machine exit. They must be reproduced by the same machine.
