---
title: "EN_UM_AWProduction_6"
source: "EN_UM_AWProduction_6.pdf"
tags: ["capacity planning", "production scheduling", "A+W Production", "shift management", "cost calculation", "master data", "transition times", "default times", "machinery groups", "load distribution"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial and software reference for A+W Production Capacity Planning. It details the configuration of master data, including shifts, calendars, cost calculations, transition times, default times, machinery groups, and load distribution to enable effective production scheduling."
long_description: "This document serves as a comprehensive guide for the A+W Production Capacity Planning software. It is structured into two main parts: a tutorial and a software reference. The tutorial section provides step-by-step instructions on how to set up and manage the essential master data required for capacity planning. Key topics covered include defining shifts, work calendars, and non-working days; creating and managing shift plans, rules, and groups; performing cost calculations by defining labor, machine, and other costs for logical machines; setting up transition times between different production processes, including normal, rush, and minimal transitions; and configuring default processing times using a powerful formula editor with elements, vectors, and conditions. The tutorial also explains how to organize machines into machinery groups to manage capacity collectively and how to implement load distribution for bottleneck machines. The second part of the document is a detailed software reference, providing an organized overview of the application's dialogs, functions, and settings related to scheduling, such as the Production Monitor, filter options, machine properties, and more."
---

# Tutorial: Master Data of Capacity Planning

---
## Shifts

### Objectives
- What's the calendar for?
- What is a shift?
- What details are required for a shift?
- How are shifts defined, edited, and deleted?

### Benefit
- With shifts, you define in which period work is done on particular machines.

### Note

**Calendar**
With the calendar, you define non-working days, e.g. legal holidays or company holidays.

**Work shift**
Work shifts are displayed in the Production Monitor. A work shift is defined as a shift plan with shift rules and shift groups.

**Shift plan**
In the shift plan, you define with shift rules and shift groups:
- In how many shifts work is done.
- On which days the shift is available.
- For which machines the rules apply.

**Shift rule**
A shift rule defines the details of a shift, e.g. the shift duration.
For each shift rule, only one shift group can be defined. All shift rules of a shift plan must have this same shift group.

**Shift group**
In a shift group, the machines are specified that work in this shift. All shift rules of a shift must have the same machine groups.

## Shift plans
With shift plans, you define work shifts that are displayed in the Production Monitor. In the shift plan, you specify in which period the machine works in your production. An individual work shift can be changed or deleted in the Production Monitor without having the change taken over in the shift plan.

[Image of the Shift editor interface, showing a calendar, a list of shift plans and rules, and details for a selected shift plan.]
*Fig. E-18 Shifts*

- **A** Calendar
- **B** Shift plan
- **C** Shift rule
- **D** Shift rule with assigned machines
- **E** Shift plan is available
- **F** Generate data for the Production Monitor

The calendar (A) forms a general basis, on which you specify the non-working days, e.g. the public holidays or company holidays.

You define the shifts in A+W Production with the shift plan (B) with shift rules (C) and shift groups (D).

- The shift plan (B) defines the general conditions. You can e.g. create a shift plan called Two-shift which specifies two-shift operation. The Two-shift shift plan specifies whether this shift plan is active, when it comes into effect and for how long, and whether you will be using an individual shift calendar or if the shift calendar will be imported from the ERP system.
- For each shift plan, there is at least one shift rule (C) with which you specify on which days and at what times work is done, e.g. in two-shift operation from Monday to Friday, from 6AM to 2PM for the early shift and from 2PM to 10PM for the late shift.
- The shift rule applies for a shift group (D) in which you define which machines work in which shifts. Thus, for example, you can specify that one of your cutting tables is always only active in the early shift or that the CNC center is also in operation on Saturdays. Only one shift group can be added to each shift rule. If you are using several shift rules, all of them must include the same shift group.

With the shift rules, you can set up the planning so that, e.g. the machines on which bottlenecks can arise work in several shifts, but all others work in only one shift.

Each shift plan can initially be defined regardless of the capacity planning. This way, you can create shift plans that you activate only at particular times (E), e.g. for special shifts.

Furthermore, each shift plan can only be valid to a limited extent. Thus, for example, you can create a shift plan for a planned construction project that is only valid for the time in which the lites must be delivered. This way, these times are not included in the planning outside the validity period.

When you create or change a shift plan, the shift is only taken over as work shift into the Production Monitor if it is generated explicitly with (F). The new work shifts are consider for the scheduling in A+W Capacity Planner for the new orders; already scheduled orders are unaffected by this.

You can display an overview of the work shifts and their utilization on the Production Monitor dialog.
⇨ Software Reference, "Scheduling" on page E-579

## Definition of non-working days
This unit will show you how to define, edit, or delete non-working days.

> **Setting up the calendar**
> You must set up the calendar before you define shift plans. Non-working days are only considered for new shifts.

For instructions on this subject, please see:
- "Here's how to define non-working days" on page E-504
- "Here's how to edit non-working days" on page E-505
- "Here's how to delete non-working days" on page E-506

### Here's how to define non-working days
1. Go to **Master data > Capacity planning > Shifts**.

[Image of the Shifts editor with the Calendar selected, showing a list of non-working days.]
- **A** Select calendar
- **B** Non-working days

2. In the **Shift editor** field, select the **Calendar** entry (A).
3. Click **[New]**.
A new line is added in the **Shift calendar** area.
4. In the **Day** and **Comment** fields, enter the data, e.g. a national holiday.
5. Click **[Accept]**.
The data is saved. When creating new shifts, the non-working days are skipped.

### Here's how to edit non-working days
1. Go to **Master data > Capacity planning > Shifts**.
2. In the **Shift editor** field, select the **Calendar** entry.

[Image showing the Shift Calendar with a date selected for editing.]

3. In the **Shift calendar** field, select the date that you want to edit.
4. Change the values.
5. Click **[Accept]**.
The data is saved.

### Here's how to delete non-working days
1. Go to **Master data > Capacity planning > Shifts**.
2. In the **Shift editor** field, select the **Calendar** entry.
3. In the **Calendar** area, in the first column, select the day that you want to delete.

[Image showing the Shift Calendar with a row selected for deletion.]
- **A** Calendar
- **B** Selection

4. Click **[Delete]**.
The day with the arrow in the first column is deleted.
5. Click **[Accept]**.
The data is saved.

## Create a Shift Plan
This unit will show you how to define, edit, or delete shift plans.
A new work shift can only be created if you have created at least one shift rule and a shift group with machines for the new shift plan.

For instructions on this subject, please see:
- "Here's how to draw up a shift plan" on page E-508
- "Here's how to edit a shift plan" on page E-509
- "Here's how to delete a shift plan" on page E-510

> **Import data**
> When you create or change a shift plan, a shift rule or a shift group, you must click [New] so that the changed shift data is created in the Production Monitor. If the changed shift is not created, A+W Production plans production with the old shift data.

### Here's how to draw up a shift plan
1. Go to **Master data > Capacity planning > Shifts**.
2. In the **Shift editor** field, select the **Calendar** entry.

[Image showing the context menu on the Calendar entry, with 'New shift plan' highlighted.]
- **A** Select context menu
- **B** Select button

3. With a right-Click the calendar, open the context menu (A) and select the **New shift plan** entry.
Alternatively, you can open the selection list (B) on the [New] button and select **New shift plan**.

[Image showing the Shift Plan detail area for a new plan.]

4. In the **Shift plan** area, in the **Name** field, enter a name, e.g. *Two-shift normal*.
5. Click **[Accept]**.
The data is saved. The new shift plan is displayed in the shift editor.
Next, you must set up the shift rules and assign the machines. Only after that is the [Create] button enabled.
⇨ "Defining a Shift Rule" on page E-510

### Here's how to edit a shift plan
1. Go to **Master data > Capacity planning > Shifts**.
2. Select the shift plan to be edited in the **Shift editor** area.

[Image of the Shift Plan details area ready for editing.]

3. Edit the values for the shift plan.
A typical application case is the extension of a shift plan.
4. Check whether the **Active** checkbox is checked so that the shift plan can be used in the capacity planning.
5. Click **[Accept]**.
The data is saved.
6. Click **[Create]** to create the changed data in the Production Monitor.

### Here's how to delete a shift plan
> **Deleting a shift plan**
> If you delete a shift plan, the corresponding shift rule and shift group will be deleted as well! The deleted shift will still be displayed in the Production Monitor. To delete it from the Production Monitor, you must first reschedule the scheduled processings.

1. Go to **Master data > Capacity planning > Shifts**.
2. Select the shift plan to be deleted in the **Shift editor** area.
3. Click **[Delete]**.
The shift plan is deleted from the shift editor.
4. Click **[Accept]**.
The data is saved.

## Defining a Shift Rule
This unit will show you how to define, edit, or delete shift rules.

For instructions on this subject, please see:
- "Here's how to define a shift rule" on page E-511
- "Here's how to edit a shift rule" on page E-513
- "Here's how to delete a shift rule" on page E-514

> **Import data**
> When you create or change a shift plan, a shift rule or a shift group, you must click [New] so that the changed shift data is created in the Production Monitor. If the changed shift is not created, A+W Production plans production with the old shift data.

### Here's how to define a shift rule
1. Go to **Master data > Capacity planning > Shifts**.
2. Select the shift plan to which the shift rule will be assigned.

[Image showing the context menu on a shift plan, with 'New shift rule' highlighted.]
- **A** Select context menu
- **B** Select button

3. Open the context menu for the shift plan (A) and select the **New shift plan** entry.
Alternatively, you can open the selection list (B) on the [New] button and select **New shift plan**.

[Image of the Shift Rule detail editing screen.]
- **A** Name of the shift rule
- **B** Start and end date
- **C** Shift number
- **D** Calendar - selection

4. Enter a name (A) and a shift number (C), e.g. *Early shift* and number 1.
5. Select the time for shift beginning and shift end (B), e.g. beginning at 6AM and end at 2PM.
6. Select the weekdays on which this shift shall be run, e.g. **Mon-Fri** for a five-day working week.
7. Select whether you want to use your own calendar (D) or if the calendar shall be imported from the ERP system, e.g. from A+W Enterprise.
You must only specify the validity period if you are setting up a special shift.
8. Click **[Accept]**.
The data is saved. The new shift plan is displayed in the shift editor.
Next, you must set up the shift groups and assign the machines. Only after that will the [Create] button be enabled.
⇨ "Creating a Shift Group" on page E-515

### Here's how to edit a shift rule
1. Go to **Master data > Capacity planning > Shifts**.
2. Select the shift rule you want to edit.

[Image of the Shift Rule editing screen with elements for changing validity and saving.]
- **A** Changing the validity period
- **B** Saving shift data
- **C** Creating data for planning

3. Change the entries in the **Shift rule** section.
A typical change is to extend a shift plan. For this, change the time period (A). The fields for the period are only enabled if at least one shift group is assigned.
4. Click **[Accept]** (B).
The data is saved.
5. Click **[Create]** (C) to create the shift with the changed data in the Production Monitor.
The shift is displayed with the changed data in the Production Monitor.

### Here's how to delete a shift rule
Before you delete a shift rule, you should restrict the validity. This way, the shifts are no longer displayed in the Production Monitor and they can no longer be booked.
1. Go to **Master data > Capacity planning > Shifts**.
2. Select the shift rule that you want to delete.

[Image showing the delete buttons for a shift rule.]
- **A** Deleting a shift rule
- **B** Deleting a shift rule for shift plan

3. Click **[Delete]** (A).
The shift rule is deleted from the editor.
4. Click **[Delete]** (B).
The shift is deleted from the Production Monitor.

> **Deleting a shift**
> You can delete a work shift in the Production Monitor. Here, only the individual shift is deleted. If you want to delete shifts by deleting the shift rules, you should first check the shifts in the Production Monitor. Under some circumstances, you must shift orders that are still scheduled.

## Creating a Shift Group
This unit will show you how to define, edit, or delete shift groups.

For instructions on this subject, please see:
- "How to create a shift group" on page E-515
- "Here's how to edit a shift group" on page E-518
- "How to delete a shift group" on page E-519

> **Import data**
> When you create or change a shift plan, a shift rule or a shift group, you must click [New] so that the changed shift data is created in the Production Monitor.
> If the changed shift is not created, A+W Production plans the production with the old shift data.

### How to create a shift group
1. Go to **Master data > Capacity planning > Shifts**.
2. Go to section **Shift editor** and select the shift rule to which the shift group will be allocated.

[Image showing the context menu on a shift rule with 'New shift group' highlighted.]
- **A** Select context menu
- **B** Select button

3. Open the context menu for the shift rule (A) and select the **New shift group** entry.
Alternatively, you can open the selection list (B) on the [New] button and select **New shift group**.

[Image of the Edit Shift Group dialog showing a list of machines.]
- **A** Name of Shift Group
- **B** Assigning the shift group

4. Select a shift group in the **Name** field (A) or enter a name.
Section **Edit shift group** lists the available machines.
5. Click **[Accept]** to save the data.
6. For all machines you want to assign the new shift group, select the name of this shift group (B) in the **Shift group** column.

[Image showing a machine being assigned to a new shift group.]

7. Assign every machine to a shift group this way.
8. Click **[Accept]**.
The data is saved. The new shift group is displayed in the shift editor with all assigned machines.

[Image showing the new shift group in the main shift editor tree view.]

After you have completely defined the shift plan, you can create the shift in the Production Monitor. To do this, proceed as follows:
9. Select the new shift plan in the shift editor.
The **Shift plan** area is displayed.
10. Check the **Active** checkbox and enter the date starting on which the shift plan is valid.
11. Click **[Create]**.
This creates the shift and so the shift is available for capacity planning starting on the validity date and if necessary for the specified time period.

### Here's how to edit a shift group
1. Go to **Master data > Capacity planning > Shifts**.
2. Select the shift group to be edited from section **Shift editor**.

[Image of the Edit Shift Group dialog, ready for editing machine assignments.]

3. In the **Edit shift group** area, change the dates, e.g.:
    - Assign machines to other shift groups. The change of the assignment of a machine to a machinery group is a typical application case for moving a machine to a different shift operation.
    - Changing the name of a shift group.
4. Click **[Accept]** to save the data.
The data is saved.
5. Select the current shift rule.
The **Shift rule** area is displayed with the current data.
6. Check the data and if necessary, adjust the settings, e.g. the validity period.
After you have edited the shift plan, you can create the changed shift in the Production Monitor. To do this, proceed as follows:
7. Click **[Create]**.
This needs to be done for all shifts.

### How to delete a shift group
1. Go to **Master data > Capacity planning > Shifts**.
2. Select the shift group to be deleted from section **Shift editor**.
3. Click **[Delete]**.
The shift group is deleted.
4. Click **[Accept]** to save the data.
The data is saved.

### Exercises
Create the data so that it is available in all subsequent exercises. If the data for the capacity planning is thus complete, you can test the planning for your own orders in the Production Monitor.
- Plan your production on paper. Which shifts will be worked on which days, and which machines will be used for the individual shifts?
- Transfer your results to A+W Production by defining the shifts.
- Check your results in the Production Monitor.
  ⇨ Software Reference, "Scheduling" on page E-579
- Change the shift plan for a machine, e.g. from two-shift to three-shift operation.
- Extend an existing shift plan.

**Additional information**
⇨ Software Reference, "Shifts" on page E-663

## Cost Calculation

### Objectives
- What is cost calculation in capacity scheduling?
- How are the costs for logical machines entered, edited, or deleted?
- Which data are exchanged between A+W Production and the ERP system in connection with cost calculation?

### Benefit
- With cost calculation, a cost optimization can be achieved. Together with the transition times, first the more economical machines are utilized for the scheduling.
- The exact breakdown and reporting of costs offers the following advantages:
  - Exact cost calculation for quotation and order entry in the ERP system.
  - Scheduling on more economical machines.
  - Cost-based statistical analysis.

### Note
With the cost calculation, you can determine personnel costs, machine costs, and other costs.
Labor and machine costs are stored in A+W Capacity Planner per machine.
Material costs are stored and calculated in the ERP system.

### Definition of the cost calculation
For logical machines, you can specify the costs that arise for production. If an order or a quotation is scheduled, A+W Production reports the costs back to the ERP system. This way, the person entering the order can query the production costs that arise for production. The material costs are stored and calculated in the ERP system.

[Image of the Cost Calculation screen showing a table of machines and their associated costs.]
- **A** Physical machine
- **B** Assigned logical machine

Enter the costs per hour and logical machine. This way, you can weight the costs of a physical machine differently, depending on which logical machine is addressed. You specify machine costs, labor costs, and other costs separately per logical machine.

**Example**
Various edge processings can be executed on your single-sided grinding machine, e.g. grinding, polishing, and mitering.
The various work processes are created not just as different processings, but also as different logical machines.
The machine tools for possible processings have different costs for the tool downtime and reprocurement. You map these differences via the costs of the logical machine that are defined for the physical machine.
At the same time, you can consider the different speeds for the processing in different specified times.

### Definition and Management of Costs
This unit will tell you how to enter, edit, and delete the costs for logical machines.

For instructions on this subject, please see:
- "How to define the costs for a logical machine" on page E-522
- "How to edit the costs for a logical machine" on page E-523
- "How to delete the costs for a logical machine" on page E-524

#### How to define the costs for a logical machine
1. Go to **Master data > Capacity planning > Cost calculation**. The **Cost Calculation** dialog opens.
2. Click **[New]**. A line with the machine -1 is inserted into the list.

[Image of the Cost Calculation dialog with a new line inserted.]
- **A** Machine
- **B** Costs

3. Double-Click the -1 field (A). The **Please select a machine** dialog appears.
4. Select the desired machine with a double-click.
5. Double-Click the empty field **Log. Machine**. The **Please select a machine** dialog appears. It lists all logical machines defined for the selected machine.
6. Select the desired logical machine with a double-click.
7. Enter the labor costs per hour for a worker. If two people are required for the work process, you must enter twice the costs.
8. Repeat step 7 for the fields **Machine costs** and **Other costs** (B). You can enter a comment, e.g. in order to explain the labor costs.
9. Click **[OK]**. The data is saved and the dialog closed.

#### How to edit the costs for a logical machine
1. Go to **Master data > Capacity planning > Cost calculation**.

[Image of the Cost Calculation dialog with costs ready for editing.]

2. Change the value of the field in question, e.g. **Other Costs**.
3. Repeat step 2 for all costs whose entries are outdated.
4. Click **[OK]**. The data is saved and the dialog closed.

#### How to delete the costs for a logical machine
1. Go to **Master data > Capacity planning > Cost calculation**.
2. Mark the line that you want to delete.
3. Click **[Delete]**. The entry will be deleted from the list. If you have deleted the entry by accident, cancel the process with **[End]**.
4. Click **[OK]**. The data is saved and the dialog closed.

### Exercises
Create the data so that it is available in all subsequent exercises. If the data for the capacity planning is thus complete, you can test the planning for your own orders in the Production Monitor.
- Select your machine and formulate the costs for the associated logical machines: Which labor costs, machinery costs, and other costs are incurred for the logical machine.
- Enter the costs for the logical machine on the **Cost calculation** dialog.
- Enter a test order or test quotation and schedule it for this machine. Check the reported prices.
- Edit the costs for the logical machines in dialog **Cost calculation**.

**Additional information**
⇨ Software Reference, "Cost Calculation" on page E-675

## Transition Times

### Objectives
- What are transition times?
- How are transition times defined, edited, and deleted?

### Benefit
- Transition times shape the time movement of the lites through production.

### Note

| Term | Definition |
| :--- | :--- |
| **Transition Time** | A transition time describes the span between the end points of sequential processings. If two sequential work processes are done on the same machine, there are no transition times, e.g. drilling and washing. Transition times are defined exclusively for logical machines. |
| **Transition type** | Transition times are defined as three different types: normal, rush transition, minimal transition. |
| **Normal transition**| Normal transitions describe the optimal production process, e.g. without absences of personnel or machine breakdowns, breakage, etc. |
| **Rush transition** | Rush transitions describe accelerated processing, e.g. in that the dwell times are shortened. However, these transition times increase the costs. |
| **Minimal transition**| Minimal transitions are the most expensive transition times. |
| **Transition time 0**| Processings that follow one another directly have no transition times, e.g. spacer bending - IG line - IG edge sealing. For these processings, all three types of transition times are identical. |
| **Explicit transition**| You define the transition from machine x to machine y as an explicit transition. |
| **Hierarchical evaluation**| The stored transition times are evaluated in the following sequence:<br>- Machine x -> Machine y.<br>- Machine x -> All machines.<br>- All machines -> machine x.<br>- All machines -> all machines. |
| **Dwell times** | Dwell times refer to times that pass without any processing, e.g. for lite sorting, wait time for remakes, drying times. Required dwell times cannot be sped up, e.g. the times for heat soak. Dwell times are calculated into the transition times. |
| **Set-up time** | Set-up times are calculated into the transition times. |
| **Customer handling time**| This refers to the time that is required to load the packaged goods. Generally one working day is set for this. For loading a container, however, several days may be required. This time is not calculated into the date optimization and it is therefore not defined as transition time. It is stored in the ERP in the customer's master data. |

### Transition times in shifts or hours
With transition times, you define the time between two processings or two (logical) machines. These time vary depending on from which machine a lite comes and to which machine it is going.
The simplest form of the transition time is the time for the path that a lite requires from one (logical) machine to the next one, e.g. the transition from cutting to the next processing. These times are defined as optimal transitions with the type **Normal**. If the transition can be sped up, times with the type **Rush** and/or **Minimal** are created.
⇨ "Transition types" on page E-532

[Diagram showing backwards calculation of production steps across shifts and days.]
*Fig. E-19 Backwards calculation with normal transition times*
- **A** Alternative - with or without coating
- **B** Transition time within a shift
- **C** Transition of 2 shifts

In this example, you see the optimal flow with the normal transition times for an IG lite with a coated lite. If in the IG only one lite is coated (A), the cutting is divided across two shifts so that the lite to be coated is cut earlier. Since Spacer bender - IG line - Seal IG (B) must always be done one after another, these processings are done in the same shift.
The transition is regarded in each case from the end of a shift. The transition from packing to sealing (C) is specified with 2 shifts, for example. This way, there is enough room for play within the shift in which the processing is scheduled.

### Transition times in shifts
Maximum transition times are only evaluated for **Normal** transitions. The other transitions are filled out automatically as minimal. If there is an entry of the type **Minimal**, faster transitions are forbidden. For **Rush** transitions, it is enough to specify the minimum number of shifts.

[Diagram illustrating normal, rush, and minimal transition times in shifts.]
*Fig. E-20 Transitions in shifts*
- **A** Optimal and maximal transition time
- **B** Rush transition time
- **C** Minimum transition time

In this example, the normal transition time (A) is specified across five shifts, which can be extended to a maximum of seven. The rush transition (B) is defined with three shifts. The program can thus automatically also calculate four shifts.
With the minimum transition time of precisely one shift (C), the transition in the same shift is forbidden automatically. The transition of two shifts is calculated automatically.
This means that you must only make four specifications: *Normal* with 5 + 2, *Rush* with 3 shifts, and *Minimal* with 1 shift. This way, seven possible shift transitions can be calculated.

### Transition times in hours
The transition time in hours does not refer to work time, but to the calendar time and is also evaluated with the virtual costs. The program specifies the transition times in hours in general in the work time.
Processing dates always refer to the shift end. With a transition time of 00:00 hours, the lites are automatically passed to the next machine, that is, they are processed further in the same shift.
If you specify the transition time in hours, you must specify a maximum time. The selection of the maximum time determines whether weekends are included in the planning.

> **Each time specification means a change of the shift**
> With the first minute, which you specify as transition time in hours, there is a change to the next shift.

[Diagram showing transitions in hours, including next shift, next day, and over a weekend.]
*Fig. E-21 Transitions in hours*
- **A** Transition time = 0
- **B** Transition time to the next shift
- **C** Transition time to the next day
- **D** Transition time to the weekend

The shift times of the various machines can vary in their length; that is, the TG furnace can be specified with a shift time of 6 hours, the IG line, by contrast, has 8 hours.
If you are working with such changeable shift ends, the time may not be specified with more than 8 hours. To avoid this problem, you can simply specify 6 hrs. (B).
From Friday at 10PM to Monday at 2PM, you need a transition time of at least 64 hours (D) for the optimal transition. Only with this transition time is it worth letting the glass stand over the weekend.
From this example, you can see that the definition of transition times in shifts is much easier than the transition in hours.

### Shift change - special case
The grinding machine in the following example works in a single shift. Furthermore, it works very slowly. If it is fitted in the morning, the lites can be transferred to the subsequent machine at the shift end.
The transition times are therefore defined with the following details:
- Normal = 0 shift
- Max. = 1 shift
- Rush = 1 shift
- Min. = 0 shift

[Diagram showing a transition of 1 shift.]
*Fig. E-22 Shift change with regard to machine*

The transition time of 1 shift refers to the shifts of the grinding machine. From this, it follows that the transition to the next shift is always calculated for the following day regardless of the transition type.
In this case, it is necessary to define the transition times for the grinding machine in hours:
- Normal = 0 hrs.
- Max. = 8 hrs.
- Rush = 4 hrs.
- Min. = 4 hrs.

[Diagram showing transitions in hours.]
*Fig. E-23 Transition in hours*

As a result of these settings, the maximum transition leads to the end of the subsequent shift on the subsequent machine. The times for the rush transition and the minimal transition lead to the middle of the following shift.

### Definition of transition times
For the individual logical machines, you specify transition times of all types with the corresponding time specifications in shifts. In exceptional cases, you can also use times with the specification in hours, e.g. for drying times.
In addition, there are a series of production-conditioned transition times that cannot be sped up, e.g. for heat soak or drying times after screen printing.
For the case that a transition does not result in a change of machine and if no explicit transition between two logical machines has been defined, an automatic transition with a transition time of 0 will be used. This guarantees that unnecessary transitions between machines will be avoided even if no explicit transitions have been defined.
⇨ "Definition of machine paths" on page E-449

[Image of the Transition Times editor, showing a table of transitions between machines.]
*Fig. E-24 Transition times*
- **A** Station from which the lite comes
- **B** Station to which the lite is going
- **C** Type of transition
- **D** Normal transition times in hours
- **E** Normal transition time in shifts
- **F** Maximum transition time in hours, shifts

Transition times are generally defined in shift (E); in exceptional cases they can also be specified in hours (D). Handling and set-up times must be considered in the transition times.

- Transition times in shifts are defined in whole shifts.
- Transition times in hours are defined in blocks of four or eight hours. This is adjusted to the shifts in your production and is clear. The transition times also include the non-working time, e.g. for the hardening of silicone sealing over the weekend.

The transition times are processed hierarchically. Here, it applies that:
- **Machine x -> Machine y** describes the explicit transition between two machines.
- **Machine x -> All machines** describes the transition at the end of machine x.
- **All machines -> Machine x** describes the transition at the entry to machine x.
- **All machines -> All machines** describes the general transition and is evaluated last if no other transition time was found.

### Transition types
In order to specify the transition times correctly, you must know the optimal throughput of your production. This means that you need to know exactly how long it takes until the next processing can be done. Starting from the normal (optimal) transition, you can then determine by how much time a transition can be shortened.

The various types of transition times are used as follows:
- **Normal type:** the lites go through production in the regular, scheduled time. These times apply for the optimal production process, e.g. without absences of personnel or machine breakdowns, breakage, etc.
- **Rush type:** the production of individual lites is sped up, e.g. by shortening the dwell time. However, these transition times increase the costs.
- **Minimal type:** the so-called high-priority orders are pushed through production. Here, only the transition times are considered that are indispensable for production, e.g. dwell times in the LAMI autoclave, drying of adhesions. Minimal transition times are the most expensive transition times.
- **Illegal type:** a transition from or to a machine is locked, e.g. because internal transport paths are required.

**Example**
With a grinding drilling line with the setting **Illegal**, you can specify that only such lites will reach the drilling station that were previously at the grinding station. For this, you would set up the following transitions:
- Illegal: All machines -> drilling station
- Normal: Grinding station -> drilling station

### Preparation for defining transition times
In order to determine the transition times for your production, you can create a matrix. The matrix helps to visualize the transition times between the logical machines.

Distinguish the time between departure and the time for arrival:
- The departure after the work process can mean, e.g. that a lite is waiting to be repacked after a processing.
- The arrival at the start can refer to preliminary work.

[Image of a sample matrix for transition times between different workstations.]
*Fig. E-25 Sample matrix for transition times*

In this example, you see, for example, that the glass in heat soak always dwells for eight hours. Therefore, the transition time from heat soak to all other workstations is always 16 hours. The times determined this way for your production must be converted into shifts.
Such a matrix shows that you must only define a few transition times between the workstations. All others can be defined with the setting **From all machines -> machine x** or **From machine x -> All other machines**.
We recommend creating the matrix and entering it in the dialog together with the A+W Software GmbH service team.

### Definition and Management of Transition Times
This unit will show you how to define, edit, or delete transition times. Consider that set-up and handling times must also be considered in the transition times.

For instructions on this subject, please see:
- "How to enter a transition time" on page E-534
- "How to edit a transition time" on page E-536
- "How to delete a transition time" on page E-536

> **Prerequisite**
> Before entering transition times you have to define the corresponding logical machines in machine allocation.

#### How to enter a transition time
1. Go to **Master data > Capacity planning > Transition times**.
2. Click **[New]**.

[Image of the Transition Times editor with a new line added at the top.]
- **A** New line
- **B** Machine from which the part is departing
- **C** Machine at which the part is arriving
- **D** Type of transition time
- **E** Normal transition time in hours or shifts
- **F** Maximum transition time in hours or shifts

A new line is added at the top of the list of machines.

3. Double-click in the field (B) in order to open the dialog for selecting the machine.

[Image of the 'Please select a machine' dialog.]

4. Select the desired machine with a double-click.
5. Repeat the step for the machine (C) for which you are specifying the transition. Also use the options **All machines to machine X** and **Machine X to all machines**.
6. Select the type (D) for the transition time and enter the appropriate time (E). Use shifts if possible. In exceptional cases, you can also use time periods, e.g. drying times.
7. Enter the maximum transition time (F). This way, you allow the system to extend the transition time. Here, you can also use hours or shifts.
> **Tip**
> For the transition to the last process, e.g. Packing or Dispatch, specify the longest transition time possible. This will give you greater flexibility in critical situations.
8. Repeat steps 2 and 7 for the next transition type (D) of the same machine combination.
9. Click **[OK]** to save the data. You have thus created the transition times in the various transition types for a transition.

#### How to edit a transition time
1. Go to **Master data > Capacity planning > Transition times**.
2. Correct the transition times for the desired machines. Activate the fields with a double-click.
3. If necessary, add a machine combination by creating data for another transition type. To do this, follow the description in the action sequence for creating transition times.
4. Click **[OK]** to save the changes. With that, you have changed the transition time.

#### How to delete a transition time
1. Go to **Master data > Capacity planning > Transition times**.
2. In the first column, select the transition time to be deleted. The whole line for this transition time is highlighted.

[Image of the Transition Times editor with a row selected for deletion.]

3. Click **[Delete]**. The transition time is deleted from the list. In case you have deleted a transition time from the list by mistake: Click the **[End]** button. If you confirm the message with [No], the dialog closes without saving the changes. The transition time is displayed in the list again when you open the dialog.
4. Click **[OK]** to close the dialog. The changes will be taken over in the database.

### Exercises
Create the data so that it is available in all subsequent exercises. If the data for the capacity planning is thus complete, you can test the planning for your own orders in the Production Monitor.
- Work with your trainer to create a new machine in the machine allocation completely, which you mark clearly as test machine for the capacity planning.
- Define the transition times for this machine in the rush and common grid.
- Create transition times between two machines for all types of transition times that are required for the transitions.
- Change the transition times.
- Check the results in the production monitor by means of a test order.

**Additional Information**
⇨ Software Reference, "Transition Times" on page E-659

## Default Times

### Objectives
- What are default times?
- How are default times defined, edited, and deleted?
- Which elements do the default times consist of?
- How are elements included in default times?
- How does the formula test work?

### Benefits
- You can use default times to define the duration of a work step on a machine for a lite. Together with the transition times, the times through the production stations are calculated this way.

### Note

| Term | Definition |
| :--- | :--- |
| **Default time = processing time** | Default times define how long a certain work process takes on a certain machine. The processing time is calculated using formulas. Default times are called processing times in machine allocation (MA). |
| **Logical machines** | Default times are created for the logical machines. |
| **Default Times** | The default times are used for capacity planning and cost calculation. |
| **Formula** | Default times can be calculated with formulas in order to consider various influencing variables, e.g. area, linear meters, quantity, thickness. Complex default times are entered as formulas in machine allocation. |
| **Element** | A line in a default time formula, e.g. a thickness dependency, the time for the production of a cut-out on a machining center or a time surcharge for heavy lites. Elements can be entered separately and tested. There are fixed elements, conditioned expressions, threshold values, weighted expressions (so-called free elements), and vectors. Tables and three-dimensional dependencies (so-called cubes) can also be processed as user-defined elements. |

### Definition of the default times
With a default time, you define how the duration of a work process is calculated on a logical machine. The basis of the calculation is the respective area or edge length of the individual order item.

[Image of the Default Times dialog listing logical machines and their formula settings.]
*Fig. E-26 Default Times*

This dialog lists the logical machines via which processings are controlled. Default times are specified in A+W Production with default time formulas. You define the default time formulas on the **Formula for Default Time** dialog.

> **Default Times**
> The default times are called processing times in machine allocation (MA). Since the default times are assigned to logical machines you can also enter formulas for default times in machinery allocation. This is done by means of the machine allocation editor, Logical machine tab in the Processing time field. These formulas from the A cannot be changed on the Default Times dialog.
> ⇨ "Structure of default time formulas" on page E-540

### Structure of default time formulas
Each default time formula is based on a basis time that is specified in seconds. Default time formulas can be defined with specified elements. In addition, you can also create your own elements and use them in the formula.

[Image of the Formula for Default Time dialog.]
*Fig. E-27 Default Time Formula*
- **A** Elements of the default time formula
- **B** Basis time in seconds
- **C** Selection of the calculation operation
- **D** Sorting sequence of the elements
- **E** Multiplier for the processing quantity

With each line, a time surcharge is specified, which is either calculated as a formula or determined as value of a table.
You can use several different elements (A) in a default time formula. For this, select the desired element, specify a value in seconds, and specify how the value should be used in the calculation operation (C). Important here is that the sequence (D) is sorted correctly. This is especially true if the next calculation operation builds on the intermediate result of the previous operation.
The basis time counts as start value. All other elements of the formula are therefore surcharges on the start value. If you do not enter a basis time, all calculations build on the result of the first entry (A).
By default, various elements are offered for selection, to which you can add with your own definitions:
⇨ "Editor for formula elements" on page E-545

**Example gas and shape**
| | |
| :--- | :--- |
| Basis time | 23 s |
| Factor for size | 23 * size factor |
| Factor for gas | Intermediate result * gas factor |
| Constants for shape | Intermediate result + shape constant |

With this default formula, you can calculate times for lites with gas filling and for shapes. If, however, you want to calculate LAMI, the formula must be structured as follows:

**Example LAMI, size and gas**
| | |
| :--- | :--- |
| Basis time | 23 s |
| Factor LAMI | + LAMI factor |
| Factor for size | Intermediate result 1 * size factor |
| Factor for gas | Intermediate result 2 + (23 * gas factor) |

⇨ "Possible settings for the default time formula" on page E-544

#### Fixed elements
Fixed elements are not assigned a value; instead, it is only specified how the elements affect the default formula. For calculation, the actual values of the glass are used. Thus, for example, for the Fixed element 'thickness' with a lite that is 4.00 mm thick, the value 4 is determined. For the Fixed element 'quantity', the number of lites and for a Fixed element 'area' the area of the lites is determined.
With the selection of the calculation operation, you specify on the **Formula for Default Time** dialog how the value determined is used in the default time formula.

#### Factors
With a factor, you can specify a time surcharge that is always calculated if the prerequisite for the use of the factor is fulfilled.

**Example**
With the Value for 'Size of lite' you specify a surcharge on the basis time that is always calculated for oversized lites. When a lite counts as oversized is specified for the factor.
With the selection of the calculation operation, you specify on the **Formula for Default Time** dialog how the value determined is used in the default time formula.

#### Vectors - tables and cubes
Vectors permit an exact planning of default times based on the properties of the workpiece. Vectors can be used to take into account the default time, e.g. for the glass thickness, area to be processed, the edge structure, and the aspect ratio of a lite.

[Image of a vector table for 'Thickness -> factor'.]
*Fig. E-28 Vector 'Thickness -> factor' - time surcharges depending on the lite thickness*

Different lite thicknesses are e.g. allowed for by the vector 'Thickness → factor'. This way, you specify time surcharges depending on the thickness of a lite.
If you specify the value in the Vector 'Thickness→ factor' as table, you can scale the value of the vector, e.g. from 4.00 - 5.99 mm thickness, the value 0.1 applies; for 6.00 - 7.99, the value 0.2 applies, etc.
With the selection of the calculation operation, you specify on the **Formula for Default Time** dialog how vectors are used in the default time formula.

#### Input help for vectors
Vectors are entered on the Factor/vector (name) dialog. This table contains one surcharge value per limit value (scale level). To create such a table, there are two procedures available:
- You specify the values individually in the table. Here, for example, you specify several levels of thicknesses, lengths or weights and assign each of these a value.
- You can have the scale levels and scaled values calculated.

[Image of the Input Help for Vectors dialog showing calculated scale levels.]
*Fig. E-29 Input help for vectors - result*

For this calculation, you specify a start and end value, e.g. 4.00 - 20.00 mm for the thickness. If you specify 2.00 mm as step size, a step is inserted every 2.00 mm between the start and end values.
If you specify 0.1 as start value for the surcharge and 0.1 as the step size, then the value 0.1 applies for the first step, and for all further levels, this value is increased by 0.1.
For the table, the result is: lites with a thickness of 4.00 - 5.99 mm have the value 0.1; from 6.00 - 8.00 mm, the value 0.2, etc.

### Calculation of time surcharges
In the simplest case, a default time formula only consists of a basic time. You can e.g. define a basic time of 30 seconds for a logical machine. This means that any process on this logical machine will take 30 seconds.
In practice, the duration of such a process depends on various factors however, e.g. on the lite thickness and on the length of the edge to be processed. The thicker the lite and the longer the edge to be processed, the more time will a process take.
To consider these dependencies, you can specify time surcharges. There are fixed elements and/or vectors available in the default time formula.

For the default time formula, you can select from the following elements:
- Basic time or start time.
- Time surcharge as fixed element, e.g. the glass thickness.
- Time surcharge as fixed value, e.g. for large lites.
- Time surcharge as vector, e.g. scaling by weight.
- Time surcharge as table for matrix, e.g. edge length.
Basic time and time surcharges are specified in seconds.

#### Sequence of the calculations
For the calculation, you must consider the operator sequence of mathematics: multiplication and division are calculated before addition and subtraction unless parentheses specify the sequence.

**Example**
| Expression | Result | Explanation |
| :--- | :--- | :--- |
| 1 + 2 * 4 | = 9 | Multiplication first |
| (1 + 2) * 4 | = 12 | Brackets first |
| 1 + (2 * 4) | = 9 | |
| 4 * (1 + 2) | = 12 | |
| 6 + (9 / 3) | = 9 | |
| (6 + 9) / 3 | = 5 | |

For calculation of the time surcharges, the following settings are available:

| Setting | Meaning |
| :--- | :--- |
| **+ Table** | The value from the table is added to the intermediate result. |
| **+ b * value** | The basic time is multiplied by the value. The result of the multiplication is added to the intermediate result. |
| **+ value** | The value is added to the intermediate result. |
| **\* (1 + value)** | The value is added to 1 and the result multiplied by the intermediate result from the previous line. |
| **\* Vector** | The result of the previous line is multiplied by the value of the vector. |
*Tab. E-1 Possible settings for the default time formula*

If the calculation begins with the determination from a formula, specify 0 as start value, e.g. the calculation of an area before the first screen printing is applied.
If the calculation is based on the result of the previous line, the sequence of entries is important.

### Editor for formula elements
For the definition of individual formula elements, there is an editor in which you can create your own formulas or select a pre-defined formula.

[Image of the Input of a Formula Element dialog.]
*Fig. E-30 Entering time formula elements*
- **A** Name of the formula element
- **B** Selection of the type
- **C** Labeling
- **D** Calculation formula
- **E** Input format
- **F** Independent parameter

You give the formula element a name (A), which is displayed in the selection of formula elements and a label (C) that is displayed on the **Formula for Default Time** dialog. The second label is displayed before the calculation value.
You use the various element types (B) for the following calculations:
- **Fixed element:** Expressions without user input, e.g. long edge. This setting should no longer be used for new definitions; it has been replaced by **Free element**.
- **Condition:** Expressions with a user input that is used if the condition is true.
- **Free element:** Expressions for which the result is weighted with the user input (e.g. seconds per meter ground).
- **Threshold value:** Expressions for which the threshold value for the condition can be set without changing the formula definition (e.g. quantity surcharge starting with user input).
- **Vector:** Expressions for which a table with value pairs of minimum values and coefficients to be used is maintained.

You can write the actual formula definition (D) of the element as a formula or select a pre-defined formula and adjust it. For vectors, you cannot change the definition, therefore, the field is grayed out.

### Example – default time for the logical machine cutting
You have determined the area dependency of your cut from production statistics. Furthermore, you 'know' that the arc shapes take 20 seconds longer on average and the table requires 10% more time for edge deletion of insulated glass components.
In order to be able to react quickly to production changes, you want to be able to set the complete default time formula to faster or slower with a control parameter.

[Image of an example default time formula for cutting.]
*Fig. E-31 Example - default time formula*

| Line | Definition | Explanation |
| :--- | :--- | :--- |
| Basic time | 0.95 | The control parameter is 95% of the default time, that is, it is set to faster. |
| Edge stripping | \* (1 + 0.1) | The surcharge is only calculated for a coated lite for IG. |
| Area cut | \* Vector | The result is multiplied by the times for the sheet area. |
| Arc shape | + 20 | For a shape with round arcs, 20 seconds are added. |
*Tab. E-2 Example - conditions of calculation*

The actual times are maintained in the vector for the cut area, e.g.:

| Area (qm) | Val. | Description |
| :--- | :--- | :--- |
| 0.1 | 70 | up to 0.99 sq m, 70 seconds are calculated |
| 0.5 | 45 | for 0.1 - 0.499 sq m, 45 seconds are calculated |
| 1.0 | 60 | for 0.5 - 0.999 sq m, 60 seconds are calculated |
| 2.0 | 150 | for 1.5 - 1.999 sq m, 150 seconds are calculated |
| 3.0 | 210 | for 1.999 - 2.999 sq m, 150 seconds are calculated |

In this example, you see that for very small and for large lites, more time is required for cutting. Thus, there is another size surcharge for cutting. For area processings, such a surcharge may be necessary and must be defined on the appropriate logical machine.

**Condition: shape with arcs**
The condition should only supply the user input as result if it is true.
**Definition (example)**
`IF (($Parts_MODELL_NR >= 60 AND $Parts_MODELL_NR <= 81) OR ($Parts_MODELL_NR >= 113 AND $Parts_MODELL_NR <= 118) OR ($Parts_MODELL_NR >= 123 AND $Parts_MODELL_NR <= 125) OR ($Parts_MODELL_NR >= 133 AND $Parts_MODELL_NR <= 199)) THEN 20 END`

> **Length specification in the formula**
> Note that the length values in a formula must be specified in µm.

**Condition: threshold value**
With more than 11 pieces, the default time should be 10% smaller.
**Definition (example)**
`IF ($Parts_MENGE > 11) THEN - 0.1 END`

**Condition: vector for shape cutting**
Vectors can depend on units or depict non-linear situations. If the simple surcharge for shapes with arcs is not precise enough for you, define a vector, with help of which you can query the required coefficients easily and very precisely.
On the dialog for entering a shape element, you can create a new element with the element type **Vector**. For a valid vector, select a formula for the independent parameter, e.g. **AWF_ShapeNumber**.

[Image showing the creation of a vector for shape-dependent surcharges.]
*Fig. E-32 Vector for shape-dependent time surcharges*
- **A** Vector with independent parameters
- **B** Table for shape numbers

The table permits the shape-dependent scaling of the surcharges. The entry for the left column always provides the start value of the validity range. It's good practice to define a value pair for 0 so that the value range is described completely.

### Time formula objects
You can map the BOM or elements of the BOM as formula objects in order to depict the chain of processings. This display serves to test the dependencies of the processings in the default time formula, e.g. to check how the processing depends on what is done in the counter-lite. Formula objects are used for testing formulas with logical quantities.
Formula objects always refer to a particular default time formula. They cannot be used across the boards. You can save the formula objects if you want to have proof that the formula is applied correctly.

[Image of the Time Formula Test dialog, showing a BOM tree of formula objects.]
*Fig. E-33 BOM tree from the point of view of the individual processings*
- **A** Save whole object
- **B** Delete object
- **C** Add object
- **D** Delete selected object
- **E** Objects

In this example, you see the processing BOM of an IG lite. When adding, the formula objects (E) are numbered. With a double-click, you can open each formula object and rename it, e.g. the first object to IG. This makes sense to clarify the structure. When adding (C), a new object is created below the selected object. When deleting (D), the selected object and all sublevels are deleted.

> **Loading a saved object for testing**
> A saved formula object can only be used for the formula for which it was created, e.g. to test changes in the default time formula. Therefore, it makes sense to give meaningful names when saving.

There is an example of a formula object under the test of the default time formula.
⇨ "Here's how to test the calculation of the time formula" on page E-557

### Definition and Management of Default Time Formulas
This unit will tell you how to define, edit, or delete default time formulas.
In the first line on the **Formula for Default Time** dialog, you can define formula elements as templates for all machines. If for the machine 0 you define a time formula, this is saved in the database, however the formula is not used since the machine 0 is not assigned a processing in the MA.

> **Prerequisite**
> Default time formulas are defined for the logical machines that execute a particular work process. Therefore, the appropriate logical machines must be defined in the machine allocation.

For instructions on this subject, please see:
- "Here's how to define a default time formula" on page E-551
- "Here's how to create a vector with the input help" on page E-554
- "Here's how to delete a default time formula" on page E-555

> **Complexity of default time formulas**
> A+W Production allows defining default time formulas of any complexity required. This permits the handling of all sorts of special cases. Keep default time formulas as simple as possible. If in your production it is necessary to use complex default time formulas, please contact the A+W Software GmbH customer service.

#### Here's how to define a default time formula
1. Go to **Master data > Capacity planning > Default times**.
2. Select the logical machine for which you want to define a default time formula.
3. Click **[Edit]**.
The **Formula for Default time** dialog opens.
A warning will be issued if a formula for the processing time has already been entered for this logical machine in machine allocation. If you proceed, the formula entered in machine allocation will be overwritten.

[Image of the Formula for Default Time dialog.]
- **A** Basic Time
- **B** Multiplier for the processing quantity
- **C** Current logical machine
- **D** Add a formula element
- **E** Add a pre-defined formula

4. Enter the basic time (A) in seconds.
You can either add a predefined formula (E) and save the data or build a formula with formula elements. The following steps will demonstrate the building with formula elements.
5. Click **[New]** (D) to select an element.

[Image of the Add Elements dialog.]

6. Select the element, e.g. a vector, and take over the selection with **[OK]**.
The selected element now appears on the list in the **Formula for Default time** dialog.

[Image of the formula editor with a new vector element added.]
- **A** Specify values
- **B** Specify calculation

7. Click **[...]** (A) in order to open the dialog for entering the values.
If you are creating a vector, you can specify limit values and the time values manually or using the input help.
⇨ "Here's how to create a vector with the input help" on page E-554
8. Select the operator (B) for the calculation.
9. Repeat the steps 5 - 8 to add additional elements.
10. Check the sequence of the formula elements.
The sequence is important for the calculation if the surcharge refers to the intermediate total of the previous element.
11. Click **[OK]** to apply the data.
The dialog closes. Thus, you have compiled a default time formula. You can check the calculation and start a calculation with sample values with a formula object.
⇨ "Testing time formulas" on page E-556
⇨ "Time formula objects" on page E-549

#### Here's how to create a vector with the input help
1. Go to **Master data > Capacity planning > Default times > Default time formula**.
2. Enter the basic time in seconds.
3. Click **[New]** and select an element, e.g. **Vector 'thickness -> factor'**.
4. Click **[Input help]**.

[Image of the Input Help for Vectors dialog.]
- **A** Limit values for the scaling
- **B** Values for the time surcharge

First the limit values for the scaling (A) and then the values for the factor (B) are entered. The table is created using these inputs.
5. Enter the start and end values, e.g. **4.00** and **20.00**.
These values specify the smallest and largest thickness.
6. Enter the step size, e.g. **2.00**.
This value specifies at what steps the limit values for the scaling are calculated between the start and end values.
7. Enter the start value and the step size for the factor, e.g. **0.1**.
This value specifies by what size the factor is increased per limit value. Thus, you have entered all necessary values.
8. Click **[OK]** to start the calculation of the table.
The **Input help for vectors** dialog closes. The tables are calculated and taken over on the **Vector -> thickness** dialog.
You can correct and complete the data.

[Image of the vector dialog populated with the calculated data.]

9. Click **[OK]** to save the data.
The **Vector thickness -> factor** dialog closes. The scaling created is taken over in the default time formula.

#### Here's how to delete a default time formula
1. Go to **Master data > Capacity planning > Default times > Default time formula**.
2. Select the element that you want to delete.
3. Click **[Delete]**.
4. Repeat the steps 2 and 3 until all elements that are no longer needed have been removed from the list.
5. Set the basic time to zero.
6. Click **[OK]** to save the data.
The dialog closes.
To delete a default time formula completely, select the default time on the **Default times** dialog and click [Delete].

### Testing time formulas
On the **Time formula test** dialog, you can test formulas and check the values and calculation settings. You can either test the formula you are currently editing on the **Formula for Default time** dialog or load a saved formula into the dialog in order to test it.
The formula test outputs a result that specifies the time for the work process in question in seconds.

For instructions on this subject, please see:
- "Here's how to test the time formula" on page E-556
- "Here's how to test the calculation of the time formula" on page E-557
- "Here's how to create a copy of the time formula syntax" on page E-561

In addition, you can define formula objects that you can use to test all formulas. You specify the specific case there in which you want to test the formula, e.g. the thickness and width of a lite. Thus, you always have the same defaults for the test. This function is described in a separate unit.
⇨ "Time formula objects" on page E-549

#### Here's how to test the time formula
1. Go to **Master data > Capacity planning > Default times > Default time formula**.
2. Select the formula element that you want to test. If you want to test the entire default time formula, you must select the **Basic Time** element. However, you can also test each element individually by selecting it and performing the following steps.
3. Click **[Formula test]**.

[Image of the Time Formula Test dialog.]
- **A** Test result
- **B** Start evaluation

4. Click **[Evaluate]** (B).
The calculation result (A) is displayed. If necessary, you can edit and correct the formula.
5. Click **[OK]** to save the data.
To test the formula with lite data, you can create a formula object for the test and enter values.

#### Here's how to test the calculation of the time formula
1. Go to **Master data > Capacity planning > Default times > Default time formula**.
Dialog **Default time formula** appears.
2. Click **[Formula test]**.
3. Double-click on the formula object (A) to open the dialog for entering the properties.

[Image of the Formula Object Properties dialog.]
- **A** Freely selectable name
- **B** Selection of the type

4. Enter a name (A) and select the type (B), e.g. element.
5. Click **[Add]**.
The fields in the **Properties** column are pre-populated with the elements that are included in the current default time formula.

[Image showing properties like WIDTH and HEIGHT pre-populated.]

6. Enter the appropriate values for each property, e.g. the dimensions for height and width.
Note that you must specify the dimensions in micrometers µm.
7. Click **[Close]** to save the data and close the dialog.
The **Formula test** dialog is displayed in the foreground.
8. Select the formula object for which the calculation should be started.
9. Click **[Formula test]**.
The result of the calculation with the values input is displayed. If the calculation does not do what you want it to, you can check the calculated values.

#### Here's how to create a copy of the time formula syntax
1. Test the time formulas as specified in the previous action sequence.

[Image of the Time Formula Test dialog with the 'Show Formula' checkbox.]
- **A** Display formula

2. Check the **Display formula** checkbox (A).

[Image of a dialog showing the 'Natural Syntax' and 'Native Syntax' of the formula.]

On this dialog, you can check the syntax of the whole formula. To correct the syntax with the help of A+W service, copy the syntax and send the text to A+W.

### Exercises
- Select a logical machine from your test machines and plan the default times for this logical machine on paper:
  - Which lites are going to be processed on this logical machine?
  - Which factors are necessary to define the default times for these lites?
  - How shall these factors be included in the default time formula?
- Create the default time formula based on the necessary elements.
- For the entry 0 - all machines, enter various formula elements, e.g. a specific vector, a table, a threshold value.
- Create a formula object for a formula and test the default time formula in order to check whether the result meets your expectations.

**Additional information**
- ⇨ Software Reference, "Default Times" on page E-638
- ⇨ Software Reference, "Default Time Formula" on page E-640
- ⇨ Software Reference, "Tabelle, Vector (Name)" on page E-645
- ⇨ Software Reference, "Input Help for Vectors" on page E-646
- ⇨ Software Reference, "Entering a formula element" on page E-649

## Machinery Groups

### Objectives
- What are machinery groups in capacity planning?
- How are machine groups defined, edited, and deleted?

### Benefits
- Machine groups are used for combining the machines of an area and for controlling the capacity of the group by means of the number of employees.

### Note

| Term | Definition |
| :--- | :--- |
| **Machinery groups** | Machinery groups combine the machines in certain areas, e.g. cutting or edgework. |
| **Persons** | Assign a number of persons to a machinery group and thus define the capacity of the corresponding machinery group. |
| **Shifts** | The shifts of the machines belonging to the same machinery group have to match. |
| **Bottleneck machine** | A bottleneck machine cannot be booked beyond its capacity. Machines become a bottleneck machine when they are allocated to a machinery group. |

> **Prerequisite**
> The shifts of the machines belonging to the same machinery group have to match. This includes the start and end time of the shifts.

### Definition of the machinery groups
You can combine machines into groups. Machinery groups make sense for machines in the same area. Thus, e.g. you could create a machine group **Cutting** to which you assign all machines in cutting. A specified capacity then applies for the entire machinery group, that is, for cutting.
You can only combine machines into a group whose shifts match; that is, that are available for the same time. Machines that you add to a machinery group automatically become bottleneck machines.

[Image of the Machinery Groups dialog.]
*Fig. E-34 Machinery groups*
- **A** Machinery Group
- **B** Available machines
- **C** Number of people in the group
- **D** Allocated machines

You must assign each of the machinery groups a number of people (C). A+W Production basically assumes that one person is working on each machine. If you reduce the number of employees in the group, the available time per machine decreases.

**Example**
In the **Cutting** machinery group with four machines, there are four people assumed. If the 4 employees work 40 hours per week, 4 x 40 = 160 working hours per week available.
With 3 employees, only 3 x 40 working hours = 120 hours per week are available.

### Definition and Management of Machinery Groups
This unit will tell you how to define, edit, or delete machinery groups.

For instructions on this subject, please see:
- "Here's how to create a machinery group" on page E-565
- "Here's how to edit a machinery group" on page E-567
- "Here's how to delete a machinery group" on page E-567

#### Here's how to create a machinery group
1. Go to **Master data > Capacity planning > Machinery groups**.
2. Click **[New]**.
3. Enter a name for the machinery group, e.g. **Cutting**.
4. Click **[OK]**.
The **Machinery groups** field shows the new machinery group.
5. Select the new machinery group. The list **Machines for group** shows all available machines.
6. Select the machine that you want to add to the group, e.g. **180 Cutting table 8**.
7. Click the arrow to the right and confirm the message. The machine was added to the group.
8. Repeat the steps 5 to 7 to add more machines.
9. Go to field **Machinery groups** and double-Click column **Persons**.
10. Enter the number of persons working in this machinery group.
11. Click **[OK]** to save the data. The dialog closes. That done, you have defined the machinery group.

#### Here's how to edit a machinery group
1. Go to **Master data > Capacity planning > Machinery groups**.
2. Go to the **Machinery groups** field and select the machinery group to be edited. The right side of the list **Machines for group** lists all machines that have been added to the group. The left side lists the available machines.
3. Select a machine to be removed from or added to the group.
4. Click the [Arrow left] or [Arrow right] button to remove a machine from the group or add a machine to the group.
5. Repeat the steps 3 to 4 to remove more machines from the group or add more machines to the group.
6. In the **Machinery groups** field, correct the number of people.
7. Click **[OK]** to save the data. The changes are saved and the dialog closed.

#### Here's how to delete a machinery group
1. Go to **Master data > Capacity planning > Machinery groups**.
2. In the **Machinery groups** field, select the machinery group to be deleted.
3. Click **[Delete]**. The machinery group is removed from the list. This way, you change the available capacity for scheduling.
4. Click **[OK]** to save the data. The changes are saved and the dialog closed.

### Exercises
Create the data so that it is available in all subsequent exercises. If the data for the capacity planning is thus complete, you can test the planning for your own orders in the Production Monitor.
- Decide which machines you want to be arranged in a group.
- Create at least one machinery group on the **Machinery groups** dialog.
- Edit your machinery group.
- Delete one of your machinery groups.

**Additional information**
⇨ Software Reference, "Machinery Groups" on page E-677

## Load Distribution

### Objectives
- What does load distribution mean in connection with capacity planning?
- How can the load distribution be defined, edited, or deleted?

### Benefits
- Load distribution makes sense for machines with a special qualification. If this qualification is not called for, the machine is used for standard processing.

### Note

| Term | Definition |
| :--- | :--- |
| **Physical machine** | Load distribution can only be defined for machines that have been specified as bottleneck machines. For example, you can keep 30% free for shapes on the machine that may be used for rectangles if no shapes are scheduled. |
| **Logical machines** | The load distribution is made among the logical machines that have been defined for a physical machine. This way, you can break down the load distribution of a CNC center as percentages with the three logical machines Special edges, Cut-outs, and Drillings. |
| **Bottleneck machine**| A bottleneck machine cannot be booked beyond its capacity. |

### Definition of load distribution
The load distribution is specified among the logical machines that have been defined for a physical machine. This way, you specify the percentage share of the logical machines of the total capacity of the physical machine.
You use load distribution to guarantee that a machine holds free a guaranteed minimum capacity for special tasks, e.g. for shape cutting. If the capacity held free is not used for shapes, rectangles can also be processed. This load distribution is only possible and makes sense for machines that are defined as bottleneck machines.

[Image of the Load Distribution dialog.]
*Fig. E-35 Load distribution*
- **A** Physical machine
- **B** Enable processing
- **C** Logical machines
- **D** Share of total capacity

You break down the capacity of a machine by allocating percentage shares (C) to the associated logical machines (D).

**Example**
A machine can process shapes, that is, rectangles and shapes. So that this special qualification is not occupied by the simpler rectangles, keep 30% free for shapes, for example. This load distribution is considered during scheduling.
If this 30% is not needed for shapes, rectangles can also be processed.

### Definition and Editing of Load Distribution
This unit will show you how to define, edit, and delete load distributions.

For instructions on this subject, please see:
- "Here's how to set up load distribution" on page E-571
- "Here's how to edit load distribution" on page E-573
- "How to delete load distribution" on page E-574

> **Prerequisite**
> Load distribution can only be defined for machines that have been specified as bottleneck machines.

#### Here's how to set up load distribution
1. Go to **Master data > Capacity planning > Load distribution**.
2. Select the machine (A) whose capacity you want to break down. The selection list includes only the machines that are defined as bottleneck machines. The corresponding logical machines are listed.
3. Check the **Enable check** checkbox (B) to enable the fields. The fields for the logical machines are enabled. If there is no load distribution specified, **Unlimited** will appear in the right column.
4. Double-Click the right column.
5. Enter the percentage for the capacity.
6. Repeat steps 4 and 5 in order to set up the percentage of total capacity of the physical machine for all logical machines.
7. Uncheck the **Enable check** checkbox to prevent inadvertent changes.
8. Click **[OK]** button to save the data and close the **Load distribution** dialog. The data is saved and the dialog closed.

#### Here's how to edit load distribution
1. Go to **Master data > Capacity planning > Load distribution**.
2. Select the machine (A) whose load distribution you want to edit. The selection list includes only the machines that are defined as bottleneck machines.
3. If necessary, check the **Enable check** checkbox (B).
4. For all logical machines, change the percentage value for the capacity.
5. If necessary, uncheck the **Enable check** checkbox.
6. Click **[OK]** to save the data. The changes are saved and the dialog closed.

#### How to delete load distribution
1. Go to **Master data > Capacity planning > Load distribution**.
2. Go to field **Physical machine** and select the machine the load distribution of which you want to delete. The corresponding logical machines are listed.
3. Check the **Enable check** checkbox. The fields will be enabled.
4. For all logical machines, change the percentage value for the capacity to **000%**. **Unlimited** is displayed in the fields.
5. If necessary, uncheck the **Enable check** checkbox.
6. Click **[OK]** to save the data. The changes are saved and the dialog closed. You have deleted the load distribution for this machine.

### Exercises
Create the data so that it is available in all subsequent exercises. If the data for the capacity planning is thus complete, you can test the planning for your own orders in the Production Monitor.
- Check for which machines a load distribution makes sense.
- If necessary, create logical machines for your test machines beforehand.
- Set up at least one load distribution.
- Edit the load distribution.
- Delete the load distribution.

**Additional information**
⇨ Software Reference, "Load Distribution" on page E-679

# A+W Production Capacity Planning - Software Reference

## Table of Contents
- **Overview** ... E-578
- **Scheduling** ... E-579
  - Production Monitor ... E-580
  - Displayed Machines ... E-584
  - Settings ... E-585
  - Please Select an Order/Batch (Filter) ... E-588
    - Filter - Orders ... E-588
    - Filter - Batches ... E-589
    - Filter - Individual Filters ... E-590
  - Create New Filter ... E-591
  - Machine (Name) ... E-592
  - Adjust Shifts for Machine ... E-594
  - Shift Properties ... E-595
  - Reservation Display ... E-597
  - Workplan from Production Monitor ... E-598
    - Work Plan - Details ... E-599
    - Work Plan - Overview ... E-601
  - Scheduling ... E-602
  - BOM Configuration ... E-603
  - Action ... E-604
  - Rescheduling ... E-605
  - Machine Reallocation ... E-610
  - Post-Processing Booking ... E-611
  - Defective Orders ... E-614
  - Asynchronous Processing ... E-615
  - Changes to Scheduled Orders ... E-616
  - Split Items ... E-617
- **Campaigns and Reservations** ... E-619
  - Campaigns ... E-620
    - Campaigns - Individual Dates ... E-621
    - Campaigns - Weekly Dates ... E-623
  - Expired Reservations ... E-624
  - Reservations ... E-626
    - Reservation for Machine ... E-629
    - Select a Customer ... E-630
    - Select Project ... E-631
- **Processings** ... E-632
  - Creation of Processings ... E-633
  - Add an Existing Condition ... E-636
- **Time Master Data** ... E-637
  - Default Times ... E-638
  - Default Time Formula ... E-640
    - Add Elements ... E-644
    - Tabelle, Vector (Name) ... E-645
    - Input Help for Vectors ... E-646
    - Select Formula ... E-648
    - Entering a formula element ... E-649
    - User-defined Table Elements ... E-651
    - Select Limit ... E-652
  - Time Formula Test ... E-653
    - Formula Object Properties ... E-655
    - Formula (Name) ... E-657
    - Course of Formula Evaluation ... E-658
  - Transition Times ... E-659
- **Master Data for the Shifts** ... E-662
  - Shifts ... E-663
  - Shift Calendar ... E-665
  - Shift Plan ... E-666
  - Shift Rule ... E-668
  - Shift Group ... E-670
  - Machine ... E-672
- **Machines and Costs** ... E-674
  - Cost Calculation ... E-675
  - Machinery Groups ... E-677
  - Load Distribution ... E-679

## Overview
The **Production Monitor** dialog is available for planning and organizing the capacities of your production. It displays the work shifts per machine.
The orders are scheduled item by item, whereby the scheduling per item must be successful. If an order item cannot be scheduled successfully, the whole order is not scheduled.
So that the calculation in the Production Monitor are done correctly, the capacity planning master data must be set up. The description of the dialogs is grouped in topics. It does not follow the arrangement of the dialogs in the software reference.

## Scheduling
The **Production Monitor** is the central capacity and order control desk and entry point for work preparation, e.g. batch formation, rescheduling.
This section provides information on the following subjects:
- "Production Monitor" on page E-580
- "Displayed Machines" on page E-584
- "Settings" on page E-585
- "Please Select an Order/Batch (Filter)" on page E-588
- "Create New Filter" on page E-591
- "Machine (Name)" on page E-592
- "Adjust Shifts for Machine" on page E-594
- "Shift Properties" on page E-595
- "Reservation Display" on page E-597
- "Workplan from Production Monitor" on page E-598
- "Scheduling" on page E-602
- "BOM Configuration" on page E-603
- "Action" on page E-604
- "Rescheduling" on page E-605
- "Machine Reallocation" on page E-610
- "Post-Processing Booking" on page E-611
- "Defective Orders" on page E-614
- "Asynchronous Processing" on page E-615
- "Changes to Scheduled Orders" on page E-616
- "Split Items" on page E-617

### Production Monitor
**Display > Production Monitor**
**Detailed view > Context menu > Production Monitor**

[Image of the Production Monitor dialog showing a grid of machines and shifts over time.]
*Abb. E-36 Production Monitor*

This dialog displays the current state of production and the use of machine capacity per work shift. This makes the Production Monitor the capacity and order control desk and the entry point for work preparation, e.g. batch formation, rescheduling.
⇨ Tutorial, "Production Monitor" on page E-454

#### Buttons

| Icon | Function | Description |
| :--- | :--- | :--- |
| [Icon] | Selected machines | ⇨ "Displayed Machines" on page E-584 |
| [Icon] | Settings | ⇨ "Settings" on page E-585 |
| [Icon] | Change display type for all machines | Selection of the display for all machines: Time, Quantity, Area, Weight |
| [Icon] | Change display (shift, day, week) | Changes the display. The machine capacity is shown per shift, per day, or per week. |
| [Icon] | Change view | Changes the view.<br>- **Main view:** All shifts in the specified time period are displayed.<br>- **Detail view:** Only the shifts for the day specified are displayed. |
| [Icon] | Zoom in, zoom out | Enlarges or reduces the display of the steps. |
| [Icon] | Refresh view | Refreshes the view. |
| [Icon] | Given number of days back, forward | Shifts the time period displayed back or forward by the number of days that is specified in the **Days** field. |
| [Icon] | Filter view, remove filter | ⇨ "Please Select an Order/Batch (Filter)" on page E-588 |

- **Start date:** Opens the calendar to select the start day for the display of work shifts.
- **Days:** Specification of by how many days the display with the buttons should be scrolled forward or back.
- **Filter input field:** Specification of the filter criterion, to filter the display by orders or batches.

> **Display**
> The display can be adapted individually. This affects the colors, a time grid, status information, etc.
> ⇨ "Settings" on page E-585

#### Work shifts
The Production Monitor displays the work shifts for all selected machines. Machines that are defined as bottleneck machines are displayed in red. A bottleneck machine cannot be booked beyond its capacity.
The following information is available via the context menu:
- **Properties:** Opens a dialog on which you can change the machine properties.
  ⇨ "Machine (Name)" on page E-592
- **Shift properties:** Opens a dialog on which you can adjust shift times of the machine.
  ⇨ "Adjust Shifts for Machine" on page E-594
- **Display logical machines:** With this entry the display of the logical machines can be activated and deactivated. Until now you had to change the corresponding switch in the master data dialog. When using the context menu, the value stored in the master data is not changed, only the display is adapted, so that the change is only temporary.
  ⇨ "Misc" on page E-593

#### Status of the planning
The colored dots indicate the backlogs:
- **Green:** No backlog.
- **Yellow:** Backlog that can be made up on the same day by using the free capacities.
- **Red:** Backlog that cannot be made up for on the same day.

#### Display of the work shifts
Brief information about the status is displayed in the tooltip for a work shift.
The following information is available via the context menu:
- **Work plan:** Opens the **Work plan: Selection from A+W Production Monitor** dialog with the overview of the batches and orders of the machine and shift.
  ⇨ "Workplan from Production Monitor" on page E-598
- **Delete:** Deletes a selected work shift from the Production Monitor.
- **Shift properties:** Opens the **Shift properties** dialog where you can change the properties of a shift.
  ⇨ "Shift Properties" on page E-595
- **Display reservations:** Opens the **Display reservation** dialog in order to check the reservations for a shift.
  ⇨ "Reservation Display" on page E-597

- **Hatched:** The duration of the work shift is reduced.
- **X:** The work shift is deactivated.
- **!:** The shift was set to **Active for rush orders** and is therefore only available for rush orders.
- **?:** Undefined processings are scheduled in the work shift.
- **Frame:** The shift is defined as a bottleneck.
  ⇨ "Shift Properties" on page E-595

### Displayed Machines
**Display > Production Monitor > [Selected Machines]**

[Image of the Displayed Machines dialog, a list of machines with checkboxes.]
*Abb. E-37 Displayed machines*

On this dialog, you select the machines that will be displayed on the Production Monitor dialog. Here, you can also specify the order. Machines that are defined as bottleneck machines will be displayed in red in the list. A bottleneck machine cannot be booked beyond its capacity.

- **Checkbox:** Specification of whether a machine is displayed on the Production Monitor dialog.
  - ☐ The machine is not displayed.
  - ☑ The machine is displayed.
- **[Arrow up], [Arrow down]:** Shifts the selected machine by one place up or down.
- **[OK]:** Saves and applies the selection and closes the dialog.

### Settings
**Display > Production Monitor > [Settings]**

[Image of the Settings dialog with various color and display options.]
*Abb. E-38 Settings - fields displayed by category*

On this dialog, you can set the display on the Production Monitor dialog, e.g. whether machine groups and backlogs are displayed. Furthermore, you can specify the display of the colors for work shifts, bottlenecks or overloads.

- **[Categories]:** Sorts the elements by categories.
- **[Alphabetically]:** Sorts the elements alphabetically.
- **[Properties]:** Not currently used.

#### Other settings
- **Number of Days before the Start Date:** Specification how many days before the current start are displayed.
- **Treatment of Machine Groups:** Specification whether machine groups are displayed.
- **Treatment of Backlogs:** Specification whether backlogs are displayed.

#### Display
- **Processed:** Color in which processed orders are displayed.
- **Update Time:** Specification of the interval in seconds at which the display on the Production Monitor dialog is updated.
- **Selected Shifts:** Color in which the selected work shift is displayed.
- **Display Capacity Graphically:** Specification whether the capacity is displayed as text.
- **Automated Updates:** Specification whether the display is updated automatically.
- **Scheduled:** Color in which the scheduled orders are displayed.
- **Bottleneck:** Color in which bottlenecks are displayed.
- **Bottleneck Color:** Font color for bottleneck machines.
- **Color of Indication Icons:** Color in which the indication icons are displayed.
- **Free Reservation Time:** Color in which the unbooked reservations are displayed.
- **Intensity of 3D Effects:** Selection of the intensity with which the 3D effects are displayed.
- **Shift:** Color in which the work shifts are displayed.
- **Display Hours:** Specification whether an hour grid is placed behind the shifts.
- **Overload:** Color in which an overload is displayed.
- **Scheduled:** Color in which scheduled work shifts are displayed.
- **Scheduled Work Processes:** Color in which scheduled work processes are displayed.
- **Display Time:** Specification of whether a time grid is displayed.
- **Time Color:** Color in which the time is displayed.

#### Detailed display
- **Work processes with finished primary products:** Specification whether work processes with finished primary products are displayed.
- **Intensity of 3D Effects:** Specification of the intensity of the 3D effect for graphic elements in the Production Monitor.
- **Production Release (quantity-based):** Color in which quantity-based production releases are displayed.
- **Production Release (time-based):** Color in which time-based production releases are displayed.
- **Display Stati:** Selection whether in addition to the machine the status for backlogs is displayed.
- **Unscheduled (quantity-based):** Color in which unscheduled work shifts are displayed. The display is quantity-based.
- **Unscheduled (time-based):** Color in which unscheduled work shifts are displayed. The display is time-based.
- **Scheduled (quantity-based):** Color in which scheduled work shifts are displayed. The display is quantity-based.
- **Scheduled (time-based):** Color in which scheduled work shifts are displayed. The display is time-based.
- **Primary products finished (quantity-based):** Color in which the finished primary products are displayed. The display is quantity-based.
- **Primary products finished (time-based):** Color in which the finished primary products are displayed. The display is time-based.
- **[OK]:** Saves and applies the selection and closes the dialog.

### Please Select an Order/Batch (Filter)
**Display > Production Monitor > [Filter View]**
Use this dialog to select orders, batches, and self-defined filters by which the view in the Production Monitor will be filtered.
The dialog offers the following tabs:
- "Filter - Orders" on page E-588
- "Filter - Batches" on page E-589
- "Filter - Individual Filters" on page E-590

#### Filter - Orders
**Display > Production Monitor > [Filter View] > Orders**

[Image of the Filter - Orders tab.]
*Abb. E-39 Please select an order/batch – orders*

The defined orders are displayed on this tab. You can select one order at a time. The display in the Production Monitor is restricted to the selected order.
- **Order number:** Order number by which filtering should be done.
- **Customer:** Customer name by which filtering should be done. The list of orders is restricted to the customer.
- **Number of records:** Defines the number of orders to be listed.
- **[OK]:** Saves the data.
- **[Reject]:** Closes the dialog without saving the data.

#### Filter - Batches
**Display > Production Monitor > [Filter View] > Batches**

[Image of the Filter - Batches tab.]
*Abb. E-40 Please select an order/batch – batches*

The defined batches are displayed on this tab. You can select one batch at a time. The display in the Production Monitor is restricted to the selected batch.
- **Batch Number:** Batch number by which filtering should be done.
- **Batch Description:** Batch description by which filtering should be done. The list of batches is restricted to the batch.
- **Number of Records:** Defines the number of batches to be listed.
- **[OK]:** Saves the data.
- **[Reject]:** Closes the dialog without saving the data.

#### Filter - Individual Filters
**Display > Production Monitor > [Filter View] > Individual Filters**

[Image of the Filter - Individual Filters tab.]
*Abb. E-41 Please select an order/batch - individual filters*

The individually defined filters are displayed on this tab.
- **[New]:** Opens the dialog **Create new filter** where you can define your own filters.
- **[OK]:** Saves the data.
- **[Reject]:** Closes the dialog without saving the data.

### Create New Filter
**Display > Production Monitor > [Filter View] > tab Individual Filters > [New]**

[Image of the Create New Filter dialog.]
*Abb. E-42 Create new filter*

On this dialog, you can create individual filters for searching in the Production Monitor. You create the filters in the SQL database language.

> **Creating individual filters**
> Please contact the A+W Software GmbH customer service should you need special filters for searching in the Production monitor.

- **Name:** Name of the filter.
- **Description:** Description of the filter.
- **SQL:** Definition of the filter in SQL.
- **[OK]:** Saves the data.
- **[Reject]:** Closes the dialog without saving the data.

### Machine (Name)
**Display > Production Monitor > Machine > Context Menu > Properties**

[Image of the Machine properties dialog.]
*Abb. E-43 Machine (Name)*

On this dialog, you change the properties of the machine in the Production Monitor.
- **[Categories]:** Sorts the elements by categories.
- **[Alphabetical]:** Sorts the elements alphabetically.
- **[Properties]:** Not currently used.

#### Machine properties
- **ID:** Identification number of the machine.
- **Registration point:** Identification number of the registration point.
- **Name:** Machine name.
- **Bottleneck:** Defines whether the machine is a bottleneck machine. Bottleneck machines appear in red letter on the List of machines in the production monitor.
- **Display type:** Selection of the unit in which the shift info displays the status **Completed**. Available for selection are:
  - Percent
  - Quantity
  - Area
  - Weight
  - Linear meters
  - Processing
- **Group:** Machine group to which the machine belongs.
- **Change performance per type of display:** Specification of the unit in which the performance of the machine is displayed.

#### Misc
- **Display logical machines:** Selection of whether the logical machines for the selected machine are also displayed in the Production Monitor, e.g. for the machine **Drilling** (Drilling machine).

- **[OK]:** Saves the data.
- **[Reject]:** Closes the dialog without saving the data.

### Adjust Shifts for Machine
**Display > Production Monitor > Machine > Context Menu > Shift Properties**

[Image of the Adjust shifts for machine dialog.]
*Abb. E-44 Adjust shifts for machine*

On this dialog, you can adjust the work shifts for the machine in question with regard to weekdays.
- **Days:** Specification of the weekdays for which the change applies.
  - ☐ The work shift is not changed for this day.
  - ☑ The work shift is changed for this day.
- **Shift number:** Specification of the shift number.
- **Capacity:** Enter the shift capacity for the selected weekdays.
- **[OK]:** Saves the data.
- **[Reject]:** Closes the dialog without saving the data.

### Shift Properties
**Display > Production Monitor > Display Shifts > Context Menu > Shift Properties**

[Image of the Shift properties dialog.]
*Abb. E-45 Shift properties*

On this dialog, you can display the properties of a work shift with regard to a machine.
- **[Categories]:** Sorts the elements by categories.
- **[Alphabetical]:** Sorts the elements alphabetically.
- **[Properties]:** Not currently used.

#### Shift properties
- **Date:** Date of the selected work shift.
- **Shift number:** Number of the selected work shift.
- **Start, End:** Start and end time from the master data for the selected work shift.
- **Capacity:** Time in hours that are available in the work shift. You can change the capacity of a work shift. The reduced capability is displayed hatched in the Production Monitor.
- **Comment:** Comment about manual changes to the current work shift.
- **Status:** Status of a work shift. On the selection menu, you select from among the following options:
  - **Active:** The work shift is available for the machine in question.
  - **Deactivated:** The work shift is not available for the machine in question. The shift is selected in the Production Monitor with an **X**. ⇨ "Display of the work shifts" on page E-582
  - **Active for rush orders:** The shift is available only for rush orders for the machine in question. The shift is selected in the Production Monitor with an **!**.
- **Bottleneck:** Selection of whether the shift is a bottleneck. A bottleneck machine cannot be booked beyond its capacity.
- **[OK]:** Saves the data.
- **[Reject]:** Closes the dialog without saving the data.

### Reservation Display
**Display > Production Monitor > Shift > Context Menu > Show Reservations**

[Image of the Reservation Display dialog showing booked reservations.]
*Abb. E-46 Reservations - overview*

This dialog displays all reservations for the current shift. You should delete expired or cancelled reservations.
⇨ Tutorial, "Here's how to delete a reservation" on page E-492

### Workplan from Production Monitor
**Display > Production Monitor > Shift > Context Menu > Work Plan**
On this dialog, you can get an overview for a particular shift.
The dialog offers the following tabs:
- "Work Plan - Details" on page E-599
- "Work Plan - Overview" on page E-601

#### Context menu
Via the context menu for the batches, you can open other dialogs in order to display details about the selected batch.
You can select the following entries via the context menu for the columns:

| Entry | Function |
| :--- | :--- |
| **Resort** | Sort column in ascending or descending order. Affects the first three columns. |
| **Formatting** | Select format or unit for the columns, e.g. date format or length unit. |
| **Insert** | Opens the selection for columns that can be inserted in the various categories. |
| **Delete** | Deletes the selected column. |
| **Display Definition** | Opens the Column Definition dialog that shows details concerning the column in question. |

#### Buttons
The functions of the buttons are described in detail in the **Rough Scheduling** section.

#### Work Plan - Details
**Display > Production Monitor > Shift > Context Menu > Work Plan > Details**

[Image of the Work Plan Details tab.]
*Abb. E-47 Work plan: Selection from Production Monitor - Details*

On this tab, you can get an overview of the planned batches in a particular shift. You can check the glass types for the selected entries, check details, and start batches. These functions are described in detail in the **Rough Planning** section.

**Columns**
With the context menu, you can select the columns in order to display the desired information, e.g.:
- **Batch:** Specifies the batch.
- **Order:** Order number.
- **Item (int Itm):** Number of the item.
- **Part No:** Part number.
- **Sequence:** Sequence number for the processing.
- **Proc. No:** Article number of the processing.
- **MA Machine:** Number of the machine, used for this processing.

**Total line**
You can display different totals in the totals row, e.g.:
- **Total Quantity T:** Total quantity and quantity in the selected batches.
- **Total Duration:** Total processing time of the selected batches in hours.

**Filter**
- **[Add filter]:** Adds a filter.
- **Drop-down menu Select a filter:**
  - Click: Opens the drop-down menu from which you select a filter.
  - Right-click: Opens the dialog to edit the current filter.

