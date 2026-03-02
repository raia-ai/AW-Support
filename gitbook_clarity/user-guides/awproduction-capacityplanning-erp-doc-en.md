---
description: "EN-AWProduction_Capacity_Planning_HC"
---


# A+W Capacity Planning Help Cards

This guide is based on the delivery version A+W Production 2015. Individual steps in the workflows may deviate, depending on the configuration.

---
## Shifts

This section covers the management of working and non-working days.

### Definition of Non-Working Days (CAP 01-001)

**Objective of this activity**
Define the days when no work is done.

**Prerequisites**
- Shift must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  In the field **Shift editor**, choose the option **Calendar**.
3.  Click **[New]**. A new line is added in the **Calendar** box.
4.  Edit the non-working day by selecting the fields and changing the **Day** and the **Comment**.
5.  Click **[Accept]** to save the data.

> **UI Reference: Shifts Dialog**
>
> *   **Description:** Define work-free days (e.g., holidays) here, for which no shifts shall be created. Click on "New" to create new entries. If you are using the ERP-WebService, you can also take the calendar from the ERP-System to create shifts.
> *   **Shift editor:** Calendar
> *   **Shift Calendar Table:**
>     | Day | Comment |
>     | :--- | :--- |
>     | 12/25/2013 | Christmas |
>     | 12/26/2013 | Christmas |
>     | 12/31/2013 | Silvester |
>     | 1/1/2014 | New Year |
> *   **Buttons:** [New], [Delete], [Accept], [Quit]

### Edit Non-Working Days (CAP 01-002)

**Objective of this activity**
Make corrections for days when no work is done.

**Prerequisites**
- Non-working days must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  In the field **Shift editor**, choose the option **Calendar**.
3.  Select the field to be edited from the **Calendar** box.
4.  Change the values.
5.  Click **[Accept]** to save the data.

### Deleting non-working days (CAP 01-003)

**Objective of this activity**
Delete days when no work is done.

**Prerequisites**
- Non-working days must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  Select a line from the **Calendar** box by marking the first column of the corresponding line.
3.  Click **[Delete]**.
4.  Click **[Accept]** to save the data.

## Shift Plans

This section explains how to create, edit, and delete shift plans.

### Create a Shift Plan (CAP 02-001)

**Objective of this activity**
Define a shift plan.

**Prerequisites**
- Shift must be defined.

**Additional info**
A shift plan can be saved after a shift rule and a shift group including machines have been allocated.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  In the field **Shift editor**, choose the option **Calendar**.
3.  Click on the selection list **[New]**.
4.  Go to **New Shift Plan**.
5.  A new shift plan called "New" is created in the **Shift editor** section. Alternatively, a right-click on the **Calendar** will open the context menu from which you can select the entry **New shift plan**.
6.  Enter a name for the new shift plan in the **Name** field in the **Shift plan** section, e.g., Common two-shift.
7.  Click **[Accept]** to save the data.
8.  Click on the **[Create]** button to create the data for this shift plan.

> **UI Reference: Shift Plan Section**
>
> *   **ID:** (System-generated)
> *   **Name:** New
> *   **Enabled:** (Checkbox)
> *   **Valid from:** (Date)
> *   **Generate Shifts:**
>     *   Use own shift calender
>     *   Use calender from ERP system
>     *   from (Date) to (Date)
> *   **Buttons:** [Create], [New], [Delete], [Accept], [Quit]

### Edit Shift Plan (CAP 02-002)

**Objective of this activity**
Make changes to a shift plan.

**Prerequisites**
- Shift plan must be defined.

**Additional info**
Editing a shift plan is a typical means of extending existing shift plans.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  Select the shift plan to be edited in the **Shift editor** section.
3.  Edit the entries for the shift plan in the **Shift plan** section.
4.  Click **[Accept]** to save the data.
5.  Click on the **[Create]** button to create the data for this shift plan. The **[Create]** button is active after a shift rule and a shift group have been allocated.

### Delete a Shift Plan (CAP 02-003)

**Objective of this activity**
Delete an existing shift plan.

**Prerequisites**
- Shift plan must be defined.

**Additional info**
If you delete a shift plan, the corresponding shift rule and shift group will be deleted as well!

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  Select the shift plan you want to delete.
3.  Click **[Delete]**.
4.  Click **[Accept]** to save the data.

## Shift Rule

This section covers the definition, editing, and deletion of shift rules.

### Define a Shift Rule (CAP 03-001)

**Objective of this activity**
Define a shift rule.

**Prerequisites**
- Shift plan must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  Select the shift plan to which the shift rule shall be assigned.
3.  Click on the selection list **[New]**.
4.  Go to **New shift rule**.
5.  Enter a name for the shift rule, e.g., `Early shift`.
6.  Enter the start and end of the shift, e.g., **Start of shift** at 6 AM and **End of shift** at 2 PM for the `Early shift`.
7.  Select the weekdays on which this shift shall be run, e.g., Mon-Fri for a five-day working week.
8.  Click **[Accept]** to save the data.
9.  Click on **[Create]** to create the data for the shift rule.

> **UI Reference: Shift Rule Section**
>
> *   **Name:** Early Shift normal
> *   **Start of Shift:** 06:00
> *   **End of Shift:** 14:00
> *   **Capacity:** 08:00
> *   **Shift Number:** 3
> *   **Days:** Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday, Mo-Fr (Checkboxes)
> *   **Buttons:** [New shift rule]

### Edit a Shift Rule (CAP 03-002)

**Objective of this activity**
Make changes to a shift rule.

**Prerequisites**
- Shift rule must be defined.

**Additional info**
Editing a shift rule is a typical means of extending shift plans. Change the period in the **Generate shifts** section, save your entry, then create new shifts.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  Select the shift rule you want to edit.
3.  Change the entries in the **Shift rule** section.
4.  Click **[Accept]** to save the data.
5.  Click on **[Create]** to create the data for the shift rule. If you do not formally adopt the changes, A+W Enterprise will plan your production with the old data.

### Delete a Shift Rule (CAP 03-003)

**Objective of this activity**
Delete an existing shift rule.

**Prerequisites**
- Shift rule must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  Select the shift rule you want to delete.
3.  Click **[Delete]**.
4.  Click **[Accept]** to save the data.
5.  Go to the **Shift plan** menu.
6.  Click on **[Create]** so that the amended shift rule data are saved and thus come into effect.

## Shift Group

This section details how to manage groups of machines and their shifts.

### Create a Shift Group (CAP 04-001)

**Objective of this activity**
Create a shift group.

**Prerequisites**
- (None listed)

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  Go to the **Shift editor** section and select the shift rule to which the shift group shall be allocated.
3.  Click on the selection list **[New]**.
4.  Select **New shift group**.
5.  Select an existing shift group in the field **Name of shift group** or enter an appropriate name for a new shift group.
6.  The **Edit shift group** section lists the available machines. Assign every machine to a shift group.
7.  Click **[Accept]** to save the data.
8.  Go to the **Shift rule** menu.
9.  Click on the **[Create]** button to create the amended data for this shift group.

> **UI Reference: Edit Shift Group Section**
>
> *   **Name of Shift Group:** New
> *   **Table of Machines:**
>     | Registration Point Number | Name | Shift Group |
>     | :--- | :--- | :--- |
>     | 110 | Tisch 1 | 2 Shifts early |
>     | 120 | Tisch2 | 2 Shifts early |
>     | ... | ... | ... |

### Edit Shift Group (CAP 04-002)

**Objective of this activity**
Make changes to a shift group.

**Prerequisites**
- Shift group must be defined.

**Additional info**
Changing the allocation of a machine to a machine group is a typical means of moving a machine to another shift pattern.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  Select the shift group to be edited from the **Shift editor** section.
3.  In the **Edit shift group** section, you can assign machines to other shift groups or change the name of an existing shift group.
4.  Click **[Accept]** to save the data.
5.  Go to the **Shift rule** menu.
6.  Click on **[Create]** to create the amended data for the shift group. This needs to be done for all shifts.

### Delete Shift Group (CAP 04-003)

**Objective of this activity**
Delete an existing shift group.

**Prerequisites**
- Shift group must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Shifts**.
2.  Select the shift group to be deleted from the **Shift editor** section.
3.  Click **[Delete]**.
4.  Click **[Accept]** to save the data.
5.  Go to the **Shift rule** menu.
6.  Click on **[Create]** to create the amended data for the shift group.

## Transition Times

This section explains how to manage the time required to switch between different production tasks.

### Create Transition Times (CAP 05-001)

**Objective of this activity**
Enter a transition time.

**Prerequisites**
- Before entering transition times, you have to define the corresponding logical machines in machine allocation.

**Workflow**
1.  Go to **Master data > Capacity planning > Transition times**.
2.  Click **[New]**. A new line `-1/-1` is added at the top of the list of Machines.
3.  Select the logical machines between which you want to enter the transition time. You can also use the options **All machines to machine X** and **Machine X to all machines**.
4.  Enter the times for a machine either in hours or shifts; do not combine these units.
5.  In the columns 'maximum duration' or 'maximum shifts', enter a value which allows the system to stretch the transition time to a maximum. Here, you can also use hours or shifts.
6.  Click **[OK]** to save the data. With that, you have entered a new transition time.

### Edit Transition Times (CAP 05-002)

**Objective of this activity**
Make changes to a transition time.

**Prerequisites**
- Transition time must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Transition times**.
2.  Edit any number of fields on the list of **Machines**. Activate the fields with a double-click.
3.  Click **[OK]** to save the data.

### Delete Transition Time (CAP 05-003)

**Objective of this activity**
Delete an existing transition time.

**Prerequisites**
- Transition time must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Transition times**.
2.  In the first column, select the transition time to be deleted. The whole line for this transition time is highlighted.
3.  Click **[Delete]**. The transition time is deleted from the list.
4.  In case you have deleted a transition time from the list by mistake:
    1.  Click the **[End]** button. The **Transition times** dialog is closed and the **Save changes** dialog appears.
    2.  Click on **[No]**.
5.  Click on **[OK]** to close the dialog and adopt the changes, i.e., the deletion of transition times.

## Default Times

This section describes how to define, manage, and test default time formulas for production processes.

### Define Default Time Formula (CAP 06-001)

**Objective of this activity**
Define a default times formula.

**Prerequisites**
- (None listed)

**Workflow**
1.  Go to **Master data > Capacity planning > Default times**. The **Default times** dialog appears.
2.  Select the logical machine for which you want to define a default time formula.
3.  Click **[Edit]**. The **Default time formula** dialog appears. A warning will be issued if a formula for the processing time has already been entered for this logical machine in machine allocation. If you proceed, the formula entered in machine allocation will be overwritten.
4.  Enter the basic time in seconds.
5.  Click on **[New]** to add a Factor, a Vector, or a Fixed element to the default time formula. The **Add elements** dialog appears.
6.  Choose a Factor, Vector, or a Fixed element from the list. The selected element now appears on the list in the **Default time formula** dialog.
7.  Repeat steps 5 and 6 to add further elements to the default time formula.
8.  Use the checkboxes to define how the elements shall be included in the default time formula.
9.  Click on **[OK]** to close the **Default time formula** dialog and adopt the data. You have now compiled a default time formula plus the necessary factors.

### Input Help for Vectors (CAP 06-002)

**Objective of this activity**
Make changes to a vector.

**Prerequisites**
- (None listed)

**Workflow**
1.  Go to **Master data > Capacity planning > Default times > Default time formula**.
2.  Click on **[...]** of the factor you want to edit. The dialog **Factor/vector (name)** appears, e.g., `Vector 'Thickness -> Factor'`.
3.  Click **[Input help]**. The **Input help for vectors** dialog appears. First enter the values for the step then the values for the factor. Based on these entries, the table will be drawn up automatically.
4.  Enter the start value, e.g., `4.00`. This value defines the sheet thickness from which the factor shall apply.
5.  Enter the end value, e.g., `20.00`. This value defines the lite thickness up to which the factor shall apply.
6.  Enter the step size, e.g., `2.00`. This value defines the distance of the steps in between the start value and the end value.
7.  Enter the start value and the step size for the factor, e.g., `0.1`. Thus, you have entered all necessary values.
8.  Click on **[OK]** to save the data and close the **Input help for vectors** dialog.
9.  The **Vector-> Thickness** dialog appears. The table shows the steps plus the corresponding factors. Check whether the data are correct.
10. Click on **[OK]** to save the data and close the **Vector 'Thickness -> Factor'** dialog.
11. Use the checkboxes in the **Default time formula** dialog to define how the factor shall influence the default time formula.

### Delete Default Time Formula (CAP 06-003)

**Objective of this activity**
Delete an existing default time formula.

**Prerequisites**
- Default time formula must be created.

**Workflow**
1.  Go to **Master data > Capacity planning > Default times > Default time formula**.
2.  Select a factor from the list.
3.  Click on **[Delete]** to remove the factor from the list.
4.  Repeat steps 2 and 3 until no factor is left on the list.
5.  Set the basic time to zero.
6.  Click on **[OK]** to save the data and close the **Default time formula** dialog. With this, you have deleted the default time formula.

### Display Default Time Formula (CAP 06-004)

**Objective of this activity**
Display a default time formula.

**Prerequisites**
- Default time formula must be created.

**Workflow**
1.  Go to **Master data > Capacity planning > Default times > Default time formula**. The **Default time formula** dialog appears.
2.  Click **[Formula test]**. The **Time formula test** dialog appears.
3.  Tick the checkbox **Display formula**. The message **(Formula name)** appears and shows the entire formula.
4.  Click on **[Copy]** to import the formula into the temporary memory. You can insert the temporarily saved formula in another program.
5.  Click on **[Close]** to close the message box.
6.  Click on **[Close]** to go to the **Default time formula** dialog.
7.  Click on **[OK]** to save the data and close the **Default time formula** dialog.

### Run Time Formula Test (CAP 06-005)

**Objective of this activity**
Test a time formula.

**Prerequisites**
- Default time formula must be created.

**Additional info**
The formula tester provides a result showing the time for the corresponding process in seconds.

**Workflow**
1.  Go to **Master data > Capacity planning > Default times > Default time formula**. The **Default time formula** dialog appears.
2.  Click **[Formula test]**. The **Time formula test** dialog appears.
3.  You can record the time formula analysis. To do this, tick the checkbox **Record evaluation**.
4.  Click on **[Evaluate]**. This shows the result of the time formula in seconds. If you have ticked the **Record evaluation** checkbox, the **Formula evaluation process** box appears.
5.  If you have ticked the **Record evaluation** checkbox, click on **[Close]** to close the **Process of formula evaluation** dialog.
6.  Click on **[Close]** to return to the **Default time formula** dialog.
7.  Click on **[OK]** to save the data and close the **Default time formula** dialog.

### Create Time Formula Snapshot (CAP 06-006)

**Objective of this activity**
Define a snapshot of a time formula to save the state of the formula.

**Prerequisites**
- Default time formula must be created.

**Additional info**
The formulas can be loaded again later for further use.

**Workflow**
1.  Go to **Master data > Capacity planning > Default times > Default time formula**. The **Default time formula** dialog appears.
2.  Click on **[Snapshots]**. The **Time formula snapshots** dialog appears.
3.  Click **[New]**. The **Description** dialog appears.
4.  Enter a description of the time formula snapshot. This description should include any specialties of the time formula.
5.  Click on **[OK]** to save the description and close the **Description** dialog.
6.  The time formula snapshot is created and displayed in the **Time formula snapshots** dialog in **Snapshots for (logical machine)**. Point the cursor at the numbered snapshots to display their creation date.
7.  Click on **[OK]** to save the data and close the **Time formula snapshots** dialog.

### Delete Time Formula Snapshot (CAP 06-007)

**Objective of this activity**
Delete a time formula snapshot.

**Prerequisites**
- Time formula snapshot must be created.

**Workflow**
1.  Go to **Master data > Capacity planning > Default times > Default time formula**. The **Default time formula** dialog appears.
2.  Click on **[Snapshots]**. The **Time formula snapshots** dialog appears.
3.  Select the time formula snapshot you want to delete. The selected time formula snapshot is marked in red.
4.  Click **[Delete]**. The time formula snapshot is removed from the list.
5.  Click on **[OK]** to save the data and close the **Time formula snapshots** dialog.

### Time Formula Based on Snapshot (CAP 06-008)

**Objective of this activity**
Create a default time formula based on a time formula snapshot.

**Prerequisites**
- Time formula snapshot must be created.

**Workflow**
1.  Go to **Master data > Capacity planning > Default times > Default time formula**. The **Default time formula** dialog appears.
2.  Click on **[Snapshots]**. The **Time formula snapshots** dialog appears.
3.  Select the time formula snapshot you want to restore. The selected time formula snapshot is marked in red.
4.  Click on **[OK]** to load the time formula snapshot into the **Default time formula** dialog and close the **Time formula snapshots** dialog.
5.  The default time formula is now available in the **Default time formula** dialog.

## Campaigns

This section covers setting up production campaigns for specific dates or weekly schedules.

### Define Campaign as an Individual Date (CAP 07-001)

**Objective of this activity**
Define a campaign as an individual date.

**Prerequisites**
- Campaigns can be defined only if the appropriate work processes and shifts have been defined and if the corresponding shift plan is active.

**Workflow**
1.  Go to **Master data > Capacity planning > Campaign planning**.
2.  Select the work processes required for this campaign in the **Work process** section. The button **[Arrow to the right]** is active now.
3.  Click on **[Arrow to the right]**. The work process now appears in the **Campaigns** section and is greyed out in the **Work process** section.
4.  Tick the checkbox of this work process in the **Campaign** section. The **Individual dates** tab is active now.
5.  Choose the date for the campaign in the **Calendar** field. The **Available shifts** field lists the shifts defined for this date.
6.  Go to the **Available shifts** field and select the shift in which the campaign shall be run.
7.  Go to the section **Add to the next** and enter the duration of this campaign in days or weeks.
8.  Click on **[Add campaign]**. The new campaign appears in the **Individual dates** field.
9.  Click **[OK]** to save the changes.

### Define Campaign as Weekly Date (CAP 07-002)

**Objective of this activity**
Define a campaign as a weekly date.

**Prerequisites**
- The **Weekly dates** tab only shows the shift plans which have been ticked in the **Shifts** dialog. Enable the shift plans required for this campaign in the **Shifts** dialog.

**Workflow**
1.  Go to **Master data > Capacity planning > Campaign planning**.
2.  Select the work processes required for this campaign in the **Work process** section. The button **[Arrow to the right]** is active now.
3.  Click on **[Arrow to the right]**. The work process now appears in the **Campaigns** section and is greyed out in the **Work process** section.
4.  Tick the checkbox of this work process in the **Campaign** section. The **Individual dates** tab is active now.
5.  Click on the **Weekly dates** tab.
6.  Go to the **Weekdays** field and select a weekday for the Weekly date. The **Available shifts** field lists the shifts defined for this date.
7.  Choose the shift in which the campaign shall be run.
8.  Click on **[Add campaign]**. The new campaign appears in the **Weekly dates** field.
9.  Click **[OK]** to save the changes.

### Edit Campaign (CAP 07-003)

**Objective of this activity**
Make changes to a campaign.

**Prerequisites**
- (None listed)

**Workflow**
1.  Go to **Master data > Capacity planning > Campaign planning**.
2.  Tick the checkbox of a work process on the **Campaigns** list. The tabs **Individual dates** and **Weekly dates** show the dates for which campaigns have been defined.
3.  Double-click on the corresponding fields to change the date or the shift.
4.  Click **[OK]** to save the changes.

### Delete Date from Campaign (CAP 07-004)

**Objective of this activity**
Delete a date from a campaign.

**Prerequisites**
- Date must be created.

**Workflow**
1.  Go to **Master data > Capacity planning > Campaign planning**.
2.  Tick the checkbox of a work process on the **Campaigns** list. The tabs **Individual dates** and **Weekly dates** show the dates for which campaigns have been defined.
3.  Tick the date to be deleted.
4.  Click **[Delete]**. The date is deleted.
5.  Click **[OK]** to save the changes.

### Delete Campaign (CAP 07-005)

**Objective of this activity**
Delete a campaign.

**Prerequisites**
- Campaign must be created.

**Workflow**
1.  Go to **Master data > Capacity planning > Campaign planning**.
2.  Tick the work process to be deleted from the **Campaigns** list.
3.  Click on **[Arrow to the right]**. The campaign including all its dates is deleted.
4.  Click **[OK]** to save the changes.

## Reservations

This section explains how to reserve capacity on bottleneck machines for specific customers or projects.

### Create Reservation (CAP 08-001)

**Objective of this activity**
Enter a reservation.

**Prerequisites**
- Reservations can only be made for machines defined as bottleneck machines.

**Workflow**
1.  Go to **Master data > Capacity planning > Reservations**.
2.  Go to the **Machine** field and choose the machine for which a reservation shall be made, e.g., cutting table 8 (180).
3.  In the **Start week** field, enter the calendar week starting from which the reservations shall be displayed in the **Weekly reservations** section, e.g., 50 / 2012.
4.  Go to the **Weeks** field and enter the number of weeks for which the reservations shall be shown, e.g., 5. The **Weekly reservations** section lists the reservations for the selected calendar weeks and machine.
5.  Click **[New]**. The **Reservation for (machine)** dialog appears.
6.  Select a customer or a project.
7.  Go to the **Start week** field and choose the week in which the reservations start by clicking on **[Arrow left]** or **[Arrow right]**.
8.  Go to the **End week** field and choose the week in which the reservations end by clicking on the buttons **[Arrow left]** or **[Arrow right]**.
9.  In the **Reservation in %** field, enter the percentage of the machine capacity to be reserved for the selected period.
10. Click on **[OK]** to save the reservation and close the **Reservation for (machine)** dialog. The data appears on the **Reservations** dialog.
11. Choose a Calendar week in the **Weekly reservations** field in the **Reservations** dialog. The new reservation for the selected calendar week appears in the **List of reservations** field.
12. Click on **[OK]** to close the **Reservations** dialog and accept the changes.

### Edit Reservations (CAP 08-002)

**Objective of this activity**
Edit a reservation.

**Prerequisites**
- Reservations can only be made for machines defined as bottleneck machines.

**Workflow**
1.  Go to **Master data > Capacity planning > Reservations**.
2.  Select the start week for the reservation in the **Start week** field.
3.  Go to the **Weeks** field and enter the number of weeks to be displayed in **Weekly reservations**.
4.  In the **Weekly reservations** field, choose the week in which the reservation has been made.
5.  The reservations for the selected week are listed in the **List of reservations**.
6.  Select the field to be edited from the **List of reservations**.
7.  Change the entry in the selected field.
8.  Repeat steps 6 and 7 for all fields you want to edit.
9.  Click on **[OK]** to close the **Reservations** dialog and accept the changes.

### Delete Reservation (CAP 08-003)

**Objective of this activity**
Delete a reservation.

**Prerequisites**
- Reservation must be created.

**Workflow**
1.  Go to **Master data > Capacity planning > Reservations**.
2.  Choose the machine for which you want to delete a reservation.
3.  Select the start week for the reservation in the **Start week** field.
4.  Go to the **Weeks** field and enter the number of weeks to be displayed in the **Weekly reservations** field.
5.  In the **Weekly reservations** field, choose the week in which the reservation has been made. The reservations for the selected week are listed in the **List of reservations**.
6.  In the first column, select the reservation to be deleted.
7.  Click on **[Delete]** to delete the selected reservation. The selected reservation will be removed from the list.
8.  Click on **[OK]** to close the **Reservations** dialog and accept the changes.

### Delete an Expired Reservation (CAP 08-004)

**Objective of this activity**
Delete an expired reservation.

**Additional info**
This dialog appears automatically when you open the **Reservations** dialog and there are any expired reservations.

**Workflow**
1.  Go to **Master data > Capacity planning > Reservations**. The **Expired Reservations** dialog opens if applicable.
2.  Select the reservations to be deleted from the list.
3.  Click on **[Delete]**. The reservations are deleted.
4.  Click on **[OK]** to save the changes and close the **Expired reservations** dialog. The main **Reservations** dialog opens.

## Cost Calculation

This section provides instructions for defining, editing, and deleting costs associated with logical machines.

### Define Costs (CAP 09-001)

**Objective of this activity**
Define the costs for a logical machine.

**Prerequisites**
- Costs can only be calculated for defined logical machines.

**Additional info**
If a machine called -1 is listed in the **Cost calculation** dialog, delete it before entering the costs.

**Workflow**
1.  Go to **Master data > Capacity planning > Cost calculation**.
2.  Click **[New]**. An entry called -1 is created on the list.
3.  Double-click on the **Machine** field of the new entry -1. The **Please select a machine** dialog appears.
4.  Choose a machine and close the **Please select a machine** dialog by pressing **[OK]**.
5.  Double-click on the **Technology** field of the new entry. The **Please select a technology** dialog appears. It lists all logical machines defined for the selected machine.
6.  Choose a logical machine and close the **Please select a technology** dialog by pressing **[OK]**.
7.  Click on the **Labour costs** field of the new entry and enter the labour costs per hour for a worker.
8.  Repeat step 7 for the fields **Machine costs**, **Other costs**, and **Comment**.
9.  Click **[OK]** to save the data.
10. Click on **[End]** to close the **Cost calculation** dialog.

### Edit Costs (CAP 09-002)

**Objective of this activity**
Edit the costs for a logical machine.

**Prerequisites**
- Costs must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Cost calculation**.
2.  Select the field to be edited.
3.  Change the entry in this field.
4.  Repeat steps 2 and 3 for all fields in which the entries are outdated.
5.  Click **[OK]** to save the data.
6.  Click on **[End]** to close the **Cost calculation** dialog.

### Delete Costs (CAP 09-003)

**Objective of this activity**
Delete the costs for a logical machine.

**Prerequisites**
- Costs must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Cost calculation**.
2.  Select the line header of the line to be deleted. The whole line is selected.
3.  Click **[Delete]**. The entry will be deleted from the list. Should you have deleted an entry by mistake, click on **[End]** and answer the security query "Do you want to save the changes" by **[No]**.
4.  Click **[OK]** to apply the data.
5.  Click on **[End]** to close the **Cost calculation** dialog.

## Machinery Groups

This section covers the grouping of machines to manage them as a single unit.

### Define Machinery Groups (CAP 10-001)

**Objective of this activity**
Defining a machinery group.

**Prerequisites**
- The shifts of the machines belonging to the same machinery group have to match. This includes the start and end time of the shifts.

**Workflow**
1.  Go to **Master data > Capacity planning > Machinery groups**.
2.  Click **[New]**. The **New machinery group** dialog appears.
3.  Enter a name for the machinery group, e.g., `Cutting`.
4.  Click **[OK]**. The **Machinery groups** field shows the new machinery group.
5.  Select the new machinery group. The list **Machines for group (name of the machine group)** shows all machines that can be added to the group.
6.  Select a machine to be added to the group, e.g., `180 Cutting table 8`.
7.  Click the **[Arrow to the right]**. The machine was added to the group.
8.  Repeat steps 6 to 7 to add more machines to the group.
9.  Go to the **Machinery groups** field and double-click the **Persons** column. The input field is active.
10. Enter the number of persons working in this machinery group.
11. Click on **[OK]** to save the data and close the **Machinery groups** dialog. That done, you have defined the machinery group.

### Edit Machinery Group (CAP 10-002)

**Objective of this activity**
Edit a machinery group.

**Prerequisites**
- Machinery group must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Machinery groups**.
2.  Go to the **Machinery groups** field and select the machinery group to be edited.
3.  Select a machine to be removed from or added to the group. The right side lists machines in the group; the left side lists available machines.
4.  Click on **[Arrow left]** or **[Arrow right]** to remove a machine from the group or add a machine to the group.
5.  Repeat steps 3 to 4 to remove more machines from the group or add more machines to the group.
6.  Go to the **Machinery groups** field and double-click the **Persons** column. The input field is active.
7.  Enter the number of persons working in this machinery group.
8.  Click on **[OK]** to save the data and close the **Machinery groups** dialog. That done, you have changed the machine group.

### Delete Machinery Group (CAP 10-003)

**Objective of this activity**
Delete a machinery group.

**Prerequisites**
- Machinery group must be defined.

**Workflow**
1.  Go to **Master data > Capacity planning > Machinery groups**.
2.  Go to the **Machinery groups** field and select the machinery group to be deleted.
3.  Click **[Delete]**. The machinery group has been removed from the list. Should you have deleted an entry by mistake, click on **[End]** and answer the security query "Do you want to save the changes" by **[No]**.
4.  Click on **[OK]** to save the data and close the **Machinery groups** dialog.

## Load Distribution

This section explains how to split the capacity of a bottleneck machine across several logical functions.

### Set-up Load Distribution (CAP 11-001)

**Objective of this activity**
Split the capacity of a machine.

**Prerequisites**
- Load distribution can only be defined for machines which have been specified as bottleneck machines.

**Workflow**
1.  Go to **Master data > Capacity planning > Load distribution**.
2.  Go to the **Physical machines** field and choose a machine whose capacity you want to split, e.g., `910 - CNC Centre`. The list box offers for selection only the machines defined as bottleneck machines. The corresponding logical machines are listed.
3.  Check the **Enable check** checkbox. The logical machines can be edited now.
4.  Double-click the right column.
5.  Enter the percentage for the capacity.
6.  Repeat steps 4 to 5 to change the remaining capacities.
7.  Click the **[OK]** button to save the data and close the **Load distribution** dialog. With that, you have changed the load distribution for this machine.

### Edit Load Distribution (CAP 11-002)

**Objective of this activity**
Edit the load distribution.

**Prerequisites**
- Load distribution must have taken place.

**Workflow**
1.  Go to **Master data > Capacity planning > Load distribution**.
2.  Go to the **Physical machines** field and choose a machine whose capacity you want to split, e.g., `910 - CNC Centre`. The list box offers for selection only the machines defined as bottleneck machines. The corresponding logical machines are listed.
3.  Check the **Enable check** checkbox. The logical machines can be edited now. If no load distribution has been defined yet, the right column reads "unlimited".
4.  Double-click the right column.
5.  Enter the percentage for the capacity.
6.  Repeat steps 4 to 5 to define the capacities for the remaining logical machines.
7.  Click the **[OK]** button to save the data and close the **Load distribution** dialog.

### Delete Load Distribution (CAP 11-003)

**Objective of this activity**
Delete a load distribution.

**Prerequisites**
- Load distribution must have taken place.

**Workflow**
1.  Go to **Master data > Capacity planning > Load distribution**.
2.  Go to the **Physical machines** field and choose a machine you want to delete, e.g., `910 - CNC Center`. The corresponding logical machines are listed.
3.  Check the **Enable check** checkbox. The logical machines can be edited now.
4.  Double-click the right column.
5.  Enter `000%`.
6.  Press the `<Enter>` key. The field now reads "unlimited," i.e., the load distribution for this logical machine has been cancelled.
7.  Repeat steps 4 to 6 to set the remaining capacities to `000%`.
8.  Click the **[OK]** button to save the data and close the **Load distribution** dialog. You have deleted the load distribution for this machine.

## Scheduling

This section provides guidance on handling scheduling issues.

### Post-processing of Scheduling

**Objective of this activity**
Re-work orders whose scheduling has failed.

**(Further details not provided in the document)**
