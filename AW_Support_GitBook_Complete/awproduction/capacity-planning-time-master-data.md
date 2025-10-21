---
title: "EN_AWProduction_Capacity_Planning_4_5"
source: "EN_AWProduction_Capacity_Planning_4_5.pdf"
tags: ["capacity planning", "software reference", "A+W Production", "time master data", "shift planning", "formula editor", "machinery costs", "load distribution", "transition times", "technical manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the A+W Production Capacity Planning module. It provides detailed instructions on configuring time master data, managing work shifts, setting up transition times between machines, calculating machinery costs, and distributing loads. The guide covers all relevant dialogs, fields, and settings for administrators and advanced users."
long_description: "This technical reference manual provides an in-depth guide to the A+W Production Capacity Planning software module. It is designed for system administrators and advanced users responsible for configuring and maintaining production planning parameters. The document systematically explains how to manage master data to optimize production scheduling and resource allocation.

Key sections include:
- **Time Master Data**: Detailed instructions on creating and managing default time formulas for production processes. This covers the calculation sequence, the use of vectors for variable time allowances, and the creation of custom formulas using the integrated formula editor. It explains how to test and validate these formulas to ensure accurate time calculation.
- **Shifts**: A comprehensive guide to defining and managing work shifts. This includes setting up shift calendars to account for non-working days and holidays, creating various shift plans (e.g., two-shift, three-shift), defining shift rules with specific start/end times, grouping shifts, and assigning logical machines to specific shifts.
- **Transition Times**: Explanations on how to configure the time required for products to move between different machines or processing stages. The guide details the hierarchical system for defining transition times, including rules for normal, rush, minimal, and prohibited transitions.
- **Machines and Costs**: Instructions on how to calculate and assign various costs (labor, machinery, other) to logical machines. It also covers how to organize machines into groups for better capacity management and how to use the load distribution feature to allocate capacity on bottleneck machines for specific tasks.
- **Dialogs and Settings**: Each section provides a granular look at the user interface, with descriptions for every dialog box, field, button, and setting. This includes guides for 'Add elements', 'Input Help for Vectors', 'Time Formula Test', and 'User-defined Table Elements', ensuring users can navigate and utilize the software effectively."
---

# Software Reference: Time Master Data

## E-201

### Possible settings for the default time formula

| Setting | Meaning |
| :--- | :--- |
| **+ b * value** | The basic time is multiplied by the value. The result of the multiplication is added to the intermediate result. |
| **+ value** | The value is added to the intermediate result. |
| **\* (1 + value)** | The value is added to 1 and the result multiplied by the intermediate result from the previous line. |
| **\* Vector** | The result of the previous line is multiplied by the value of the vector. |
*Tab. E-5 Possible settings for the default time formula*

### Calculation sequence
For the calculation, you must consider the operator sequence of mathematics: multiplication and division are calculated before addition and subtraction unless parentheses specify the sequence.
Furthermore, you must heed the sequence of the lines if a calculation should build on the result of the previous line.

**[...]**: Opens the dialog Vector (Name) where you can edit the properties of the vector.
⇨ "Tabelle, Vector (Name)" on page E-204

**[Sort]**: Moves a selected element in the default time formula. The sequence of factors is essential if you choose the option Factor multiplied by subtotal.

### [Multiplication of formula result by the processing quantity per part]
You can multiply the result of the formula by the quantity to be processed per part.
- The result of the formula will not be multiplied by the processing quantity per part.
- The result of the formula will be multiplied by the processing quantity per part.

### Own formula
Display of the assigned formula.

**[Zoom]**: Opens the dialog Generic Select Form where you can select self-defined formulas.
⇨ "Select Formula" on page E-207

**[Cross]**: Removes a formula from the field Own formula.

**[Formula editor]**: Opens the Enter a formula element dialog on which you can create a formula.
There is a separate manual on the topic of the Formula editor.
⇨ "Entering a Formula Element" on page E-208

---
*A+W Production Capacity Planning*

## E-202

**Formula test**: Opens the dialog Time Formula Test which is used to analyze formulas for time calculation.
⇨ "Time Formula Test" on page E-212

**[New]**: Opens the dialog Add Elements in which you can select elements.
⇨ "Add elements" on page E-203

**[OK]**: Saves the data.

**[Quit]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-203

# Add elements

> Master data > Capacity planning > Default times > [Edit] > [New]

*Fig. E-118 Add elements*

On this dialog, you can apply elements for time allowances on the Default time formula dialog.
⇨ Tutorial, "Definition and Management of Default Time Formulas" on page E-117

The following elements can be added:
- `<New Element...>`
- `<New Table...>`
- `Coating Factor`
- `Constant element`
- `Factor 'at least triple IG'`
- `Factor 'Gas'`
- `Factor 'LAMI'`
- `Factor 'Large lite`
- `Factor 'Muntins"`
- `Factor 'Small lite`
- `Factor 'SPC SE`
- `Factor 'TGH'`
- `Fixed element 'quantity"`
- `Fixed element 'sqft.'`
- `Fixed element 'thickness'`
- `'Free' element 10`
- `'Free' element 2`
- `'Free' element 3`
- `'Free' element 4`
- `'Free' element 5`
- `'Free' element 6`
- `'Free' element 7`
- `'Free' element 8`
- `'Free' element 9`
- `Vector 'Edge matrix -> Factor'`
- `Vector 'Length -> Factor'`
- `Vector 'Qty. -> Factor'`
- `Vector 'Sqft. -> Factor'`
- `Vector 'Weight -> Factor'`
- `"Width, Height -> Factor'`

**[Delete]**: Deletes the selected entry.

**[OK]**: Takes over the selected entry into the Default time formula dialog.

**[Quit]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-204

# Tabelle, Vector (Name)

> Master data > Capacity planning > Default times > select logical machine > [Edit] > [...]

*Fig. E-119 Value entry - entry into table, matrix display*

On this dialog, you edit the properties of a time allowance. You can edit the values depending on type in the table entry.
⇨ Tutorial, "Definition and Management of Default Time Formulas" on page E-117

**Columns**: The display of the columns depends on the formula element for which the dialog is opened, e.g. thickness, weight, height, and width.

> **Example of thickness**
> If you enter 4.00 mm, 8.00 mm, and 10.00 mm for the thickness in the table, the allocated factors will apply to the thicknesses 4.00 to 7.99 mm, 8.00 to 9.99 mm, etc.

**Value**: Factor (value) per thickness, weight, length, quantity, surface, or edge matrix.

**[Input help]**: Opens the Input help for vectors dialog.
⇨ "Input Help for Vectors" on page E-205

**[OK]**: Takes over the selected entry into the Default time formula dialog.

**[Close]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-205

# Input Help for Vectors

> Master data > Capacity planning > Default times > select logical machine > Edit > [...] > insert vector > [Input help]

*Fig. E-120 Input help for vectors*

On this dialog, you can have the table on the Vector... dialog filled out automatically by specifying values.
⇨ Tutorial, "Definition and Management of Default Time Formulas" on page E-117

### Default values
In this area, you specify the limit values for the calculation of the table.

**Start Value**: Start value with which the table begins.
The start value refers to the table column Thickness, weight, length, quantity, surface, or edge matrix on the Factor/Vector (Name) dialog. For example, for Vector Length -> Factor enter 100 mm as start value to start the calculation at 100 mm.

**End Value**: End value with which the table closes.
The end value refers to the table column Thickness, weight, length, quantity, surface, or edge matrix on the Factor/Vector (Name) dialog.
For example, for Vector Length -> Factor enter 2000 mm as end value to end the calculation at 2000 mm.

**Step Size**: Size with which the limit value is created between start and end value.
The step size refers to the table column Thickness, weight, length, quantity, surface, or edge matrix on the Factor/Vector (Name) dialog.
Enter for example for a vector Vector 'Length -> Factor' a step size of 100 mm. This means that a different value will be assigned to the vector every 100 mm, e.g. 100.00 to 199.00 mm, 200.00 to 299.99 mm, etc.

---
*A+W Production Capacity Planning*

## E-206

### Values
In this area, you specify the values for the calculation of the time allowances per limit value.

**Start Value**: Value with which the time allowance for the smallest of the specified limit values is calculated.
The start value refers to the table column Factor on the Factor/Vector (Name) dialog.
Enter for example for a vector Vector 'Length -> Factor' a start value of 1. This means that the vector will be assigned the value 1 for a length between 100 mm and 199.99 mm.

**Step Size**: Value by which the calculation value per limit value is increased.
The step size refers to the table column Factor on the Factor/Vector (Name) dialog.
Enter for example for a vector Vector 'Length -> Factor' a step size of 2. This means that the value of the vector will be increased by the value 2 every 100 mm, e.g. the values 1, 3, 5, etc.

**[OK]**: Saves the data.

**[Close]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-207

# Select Formula

> Master data > Capacity planning > Default times > Edit > Own formula

*Fig. E-121 Select Formula*

On this dialog, you can select defined formulas and insert them on the Default time formula dialog.
⇨ Tutorial, "Definition and Management of Default Time Formulas" on page E-117

> **Own formulas**
> Additional formulas may have a massive impact on the behavior and the properties of default time formulas.
> Please contact A+W Software GmbH customer service if you need your own formulas or to change existing formulas!

**ID**: Formula ID.

**Formula**: Formula name.

**Description**: Description of the formula.

**Language**: Choose the language in which the formula has been written. If you choose English, for instance, you will see only the formulas that have been defined in this language.

**Text**: Search for a formula by means of its name.

**[OK]**: Saves the data.

**[Reject]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-208

# Entering a Formula Element

> Master data > Capacity planning > Default times > [Edit] > [Formula Editor], [New]

*Fig. E-122 Time formula – entering element*

On this dialog, you can enter an individual element for calculating a time formula.
⇨ Tutorial, "Editor for Formula Elements" on page E-112

**Name**: Name that is displayed in the selection of formula elements.

**Element Type**: Selection of the element type.
- **Fixed element**: Expressions without user entry, e.g. long edge. You should no longer use this setting for new definitions. It has been replaced by Free Element.
- **Condition**: Expressions with a user input that is used if the condition is true.
- **Free element**: Expressions for which the result is weighted with the user input (e.g. seconds per meter ground)
- **Threshold value**: Expressions for which the threshold value for the condition can be set without changing the formula definition (e.g. quantity surcharge starting with user input)
- **Vector**: Expressions for which a table with value pairs of minimum values and coefficients to be used is maintained.

**Labeling**: Designation that is displayed on the Default time formula dialog.

**Definition**: Formula for the calculation for the element types Fixed element, Condition, and Free element.

---
*A+W Production Capacity Planning*

## E-209

**Input format**: Format of the dimension unit for the element types Threshold value and Vector:
- **No unit**: No dimensional unit.
- **Thickness, Length**: Millimeter, inch.
- **Area**: Square meter, square foot.

This setting guarantees that the inputs for the parameters are interpreted in the unit that is configured in A+W Production.

**Labeling**: Designation that is displayed on the Default time formula dialog before the calculation value, e.g. sec. for a time value.

**Definition**: Display of the formula for an independent parameter that is selected for a vector or threshold value.

---
*A+W Production Capacity Planning*

## E-210

# User-defined Table Elements

> Master data > Capacity planning > Default times > [Edit] > [New] > <New table...>

*Fig. E-123 User-defined table elements*

On this dialog, you define a new table element for default time formulas.
⇨ Tutorial, "Structure of Default Time Formulas" on page E-107

### Properties
**Name**: Name of the table element.

**Type**: Type of the formula element.
The following options are available for New table:
- Vector (one-dimensional)
- Table (two-dimensional)
- Cube (three-dimensional)

**Value 1, Value 2, Value 3**: Opens the Select limit dialog where you can select a value. The number of fields depends on the table type selected.
⇨ "Select Limit" on page E-211

**Description**: Description of the table elements.

**[Delete]**: Deletes the selected element.

**[Save]**: Saves the data.

**[New]**: Creates a new table element.

**[Close]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-211

# Select Limit

> Master data > Capacity planning > Default times > [Edit] > [New] > <New table...> select

*Fig. E-124 Limits for table elements*

On this dialog, you can select limit values for a new table element. The table element is used for the formula for calculation of default times.
⇨ "User-defined Table Elements" on page E-210

**[OK]**: Applies the data.

**[Close]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-212

# Time Formula Test

> Master data > Capacity planning > Default times > [Edit] > [Formula -test]

*Fig. E-125 Time formula test*

On this dialog, you can check formulas for time calculation. The test always affects the element selected on the Default time formula dialog. If the whole default time formula should be tested, you must select the Basic Time entry.
⇨ Tutorial, "Testing Time Formulas" on page E-124

### Formula object
**Formula object (name)**: Graphic display of the formula objects. With a double-click, you open a dialog on which you can enter the values for the test, e.g. the lite dimensions.
⇨ "Formula Object Properties" on page E-214

**[New]**: Saves a new formula object.
**[Load]**: Loads a saved formula object.
**[Save]**: Saves the changed formula object.
**[Add]**: Adds an element below the selected element.
**[Delete]**: Deletes the selected element.

---
*A+W Production Capacity Planning*

## E-213

### Diagnosis Tool
**Show formula**: You can have the formula syntax displayed.
- The formula syntax will not be shown.
- Opens the Formula (name) dialog where the syntax of the formula is shown and can be copied.
  ⇨ "Formula (Name)" on page E-215

**Protocol evaluation**: You can create a record of the formula evaluation.
- The evaluation will not be recorded.
- The evaluation of the formula is shown on the Course of Formula Evaluation dialog.
  ⇨ "Course of Formula Evaluation" on page E-216

**Result**: Result of the time calculation in seconds. An arrow up or down indicates that the result of the default time formula is higher or lower than the basic time.

**[Evaluate]**: Starts the formula analysis.
Analysis always starts from the selected formula object. If you have not selected an element, the evaluation begins on the header.
The result of the analysis is displayed in the Result field. If you have selected the Protocol Evaluation checkbox, the Course of Formula Evaluation dialog opens.
⇨ "Course of Formula Evaluation" on page E-216

**[Close]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-214

# Formula Object Properties

> Master data > Capacity planning > Default times > Edit > Formula test > Double-click on the formula object

*Fig. E-126 Time formula test - formula object properties*

On this dialog, you enter the data for the formula test, e.g. a lite with the thickness 4 mm and a width of 2500 mm. On this dialog, lengths and thicknesses are specified in the unit micrometers µm.
⇨ Tutorial, "Time Formula Objects" on page E-116

### Formula Object Properties
**Name**: Name of the formula object.
**Type**: Selection of the option Part or Processing.

### Overview
- **Property**: Assigned property. In the selection list, all factors are available that you have added to the default time formula and their properties can be edited.
- **Value**: Value for the test calculation in question. Length and thickness specifications in micrometers.

---
*A+W Production Capacity Planning*

## E-215

**[Add]**: Adds a new element to the Property list. The display of the properties depends on the elements that are added to the default time formula.

**[Delete]**: Deletes the selected element.

**[Close]**: Closes the dialog without saving the data.

# Formula (Name)

> Master data > Capacity planning > Default times > [Edit] > [Formula -test] > check Display Formula checkbox

*Fig. E-127 Formula syntax*

On this dialog, the formula is displayed in natural syntax in order to find errors in a default time formula.
⇨ Tutorial, "Definition and Management of Default Time Formulas" on page E-117

**[Copy]**: Copies the formula e.g. to add it to an editor.

**[Close]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-216

# Course of Formula Evaluation

> Master data > Capacity planning > Default times > [Edit] > [Formula -test] > check Protocol Evaluation checkbox > [Evaluate]

*Fig. E-128 Course of formula evaluation*

This dialog displays the course of formula evaluation. This evaluation is required by A+W Software GmbH support to analyze a formula calculation.
⇨ Tutorial, "Definition and Management of Default Time Formulas" on page E-117

**[Close]**: Closes the dialog.

---
*A+W Production Capacity Planning*

## E-217

# Transition Times

> Master data > Capacity planning > Transition times

*Fig. E-129 Transition times*

On this dialog, you specify transition times between (logical) machines. You can define transition times for optimal transfer and for accelerated transfers. With the specification of minimum and maximum times, you specify a time span in which the transition can take place. For the planning, the transition is always regarded from the end of a shift.
⇨ Tutorial, "Transition Times" on page E-92

The transition times are processed hierarchically.
- **Machine x -> Machine y** describes the explicit transition between two machines.
- **Machine x -> All machines** describes the transition at the end of machine x.
- **All machines -> Machine x** describes the transition at the entry to machine x.
- **All machines -> All machines** describes the general transition and is evaluated last.
⇨ Tutorial, "Transition Times" on page E-92

---
*A+W Production Capacity Planning*

## E-218

> **Transition times in shifts**
> Generally, transition times are defined in shifts. Only in exceptional cases do you use the duration in hours and minutes, e.g. for drying times.

### Machines
- **Machine 1**: Logical machine from where the transition starts. Double-click on a field to open the dialog to select a logical machine.
- **Machine 2**: Logical machine to which the transition is made. Double-click on a field to open the dialog to select a logical machine.
- **Type**: Type of transition time:
  - **Normal**: Normal transition time. It describes the optimal throughput through production, e.g. without breakdowns of personnel or machines, breakage, etc.
  - **Rush**: Reduced transition time for rush orders, e.g. without dwell times. With this time, the (virtual) costs increase. These transition times are used automatically for orders that have the priority Rush in the ERP system. These orders also use the work shifts reserved for rush orders.
  - **Minimal**: Reduced transition time for top priority orders. You may only use this setting if another reduction is technically possible. In general, this setting is only used if a minimum time must be adhered to, e.g. after the autoclave. Only the transition time from the Transition time 'h:m' is used.
  - **Prohibited**: Machine 2 may not be activated after machine 1. With this setting, you can map, for example, that a machine cannot be reached without internal transport.
- **Transition time 'h:m'**: Minimal transition time in hours and minutes. This setting is used if the time is also calculated across non-working days. You can specify the minimal transition time and maximum transition time in mixed units, e.g. an optimal transition time of 2 hours and a maximum transition time of 2 shifts.
- **Shifts**: Minimum transition time in shifts.
- **Maximum transition time 'h:m'**: Maximum transition time in hours and minutes. Here, a value must be specified that describes at least one weekend since the machine will otherwise not be used on Friday, for example.
- **Maximum shifts**: Maximum transition time in shifts. The value of the maximum transition time is added to the minimum transition time. With a minimum transition time of 1 shift and a maximum transition time of 3 shifts, this produces a transition time of 1 to 4 shifts.

You can specify the minimum transition time and maximum transition time

---
*A+W Production Capacity Planning*

## E-219

in mixed units, e.g. a minimum transition time of 2 hours and a maximum transition time of 2 shifts.

> **Example**
>
>| Transition type | Shifts | Maximum shifts | Time in shifts |
>| :--- | :--- | :--- | :--- |
>| Normal | 2 | 2 | 4 |
>| | 2 | 1 | 3 |
>| Rush | 1 | | 1 |
>| Minimum | 1 | | 1 |

> **Tip**
> For the transition to the last process, e.g. Packing or Dispatch, specify the longest transition time possible. This will give you greater flexibility in critical situations.

**[New]**: Adds a new line in order to define a transition time.

**[Delete]**: Deletes the selected entry.

**[OK]**: Takes over the selected entry into the Default time formula dialog.

**[Quit]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-220

# Master Data for the Shifts

In addition to the default and transition times, it is also possible to define shifts in which the work times can be defined in production per day.

This section provides information on the following subjects:
- "Shifts" on page E-221
- "Shift Calendar" on page E-223
- "Shift Plan" on page E-224
- "Shift Rule" on page E-226
- "Shift Group" on page E-228
- "Machine" on page E-229

---
*A+W Production Capacity Planning*

## E-221

# Shifts

> Master data > Capacity planning > Shifts

The following chapters deal with the Shifts dialog:
- "Shift Calendar" on page E-223
- "Shift Plan" on page E-224
- "Shift Rule" on page E-226
- "Shift Group" on page E-228
- "Machine" on page E-229

*Fig. E-130 Shifts*

Manage shift plans on this dialog.

> **Changing of shifts**
> Changing shifts is a major operation in capacity planning. Check in the Production Monitor whether changes are implemented correctly in work shifts. Orders already scheduled will not be rescheduled automatically. Therefore, change shifts only so that they only become available at a time when no orders are scheduled.
> For last-minute changes, there are various functions available in the Production Monitor. In case of questions, please contact A+W Software GmbH customer service.

⇨ Tutorial, "Shifts" on page E-68

---
*A+W Production Capacity Planning*

## E-222

### Shift editor
In the Shift editor area, the calendar and shift plans are displayed. Using the context menu or the buttons, you can open the various views for the definition of the shift plans:
- Shift Calendar
- Shift Plan
- Shift Rule
- Shift Group
- Machine

**[New]**: Opens the Shift calendar view in order to define a new calendar.

**[Delete]**: Deletes the selected entry.

**[Apply]**: Saves the data.

**[Quit]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-223

# Shift Calendar

> Master data > Capacity planning > Shifts > Calendar

*Fig. E-131 Shifts - calendar*

In this view of the dialog, you define the non-working days.
⇨ Tutorial, "Definition of non-working Days" on page E-71

**Shift calendar**: Specification of the non-working days, for example, holidays.

**Day**: Date of the non-working day.

**Comment**: Description of the non-working day, e.g. Christmas day.

**[New]**: Adds a new line to the shift calendar in order to define a non-working day. Use the selection list to create a new shift plan.
- Shift Plan

**[Delete]**: Deletes the selected day from the shift calendar.

**[Apply]**: Saves the data.

**[Quit]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-224

# Shift Plan

> Master data > Capacity planning > Shifts > Shift plan

*Fig. E-132 Shifts, shift plan*

In this view of the dialog, you manage the shift plans with which you define the shifts.
⇨ Tutorial, "Create a Shift Plan" on page E-74

### Shift plan
In this area, you create and manage a shift plan, e.g. a two-shift plan or a three-shift plan.

**ID**: ID of the shift plan.

**Name**: Freely selectable name of the shift plan.

**Active**: You can specify whether the shift plan can be used for the planning of weekly campaigns.
- The shift plan is available for Weekly dates. It cannot be selected on the Campaigns dialog.
- The shift plan is available for Weekly dates.

**Valid from**: Specification of the date starting on which the shift plan is valid. This way, you can set up the shift plan without making the shift available immediately, e.g. for special shifts on a weekend.

---
*A+W Production Capacity Planning*

## E-225

### Generate shifts
By selecting this option, you specify which calendar is used for the shift plan:
- **Use own shift calendar**: Uses the calendar you have defined in the shifts calendar.
  ⇨ "Shift Calendar" on page E-223
- **Use calendar from ERP system**: Imports a calendar from an ERP system, e.g. from A+W Business.

**From ... to**: Specification of the start and end date. Shifts according to this shift plan will only be generated in the Production Monitor for the specified time period.

**[Create]**: Creates a new shift in the Production Monitor with the new data that you have entered.
The button is only active if you have assigned a shift rule and a shift group with machines.

**[New]**: Creates a new shift plan. The list box is used to create a new shift rule.
- Shift Rule

**[Delete]**: Deletes a selected shift plan.

**[Apply]**: Saves the data.

**[Quit]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-226

# Shift Rule

> Master data > Capacity planning > Shifts > Shift rule

*Fig. E-133 Shifts - Shift rule*

In this view of the dialog, you manage the shift rules of a shift plan.
⇨ Tutorial, "Defining a Shift Rule" on page E-77

### Shift rule
Shift rules apply for an individual shift plan. You can assign a shift group to each shift rule.

**Name**: Freely definable name of the shift rule, e.g. Early shift normal.

**Start of shift, End of shift**: Specification of the time at which the shift begins and ends.

**Capacity**: Display of the capacity of the shift in hours. This is calculated from the shift beginning and shift end.

**Shift number**: Input of the shift number.

---
*A+W Production Capacity Planning*

## E-227

**Days**: Specification of the weekdays on which the shift can be worked.
- The shift is not created.
- The shift can be created in the Production Monitor.

### Generate shifts
By selecting this option, you specify which calendar is used for the shift plan:
- **Use own shift calendar**: Uses the calendar you have defined in the shifts calendar.
  ⇨ "Shift Calendar" on page E-223
- **Use calendar from ERP system**: Imports a calendar from an ERP system, e.g. from A+W Business.

**From... to**: Specification of the start and end date. Shifts according to this shift plan will only be generated in the Production Monitor for the specified time period.

**[Delete]**: Deletes the selected shift rule with all assigned machines. This way, the associated shifts are deleted from the Production Monitor.

**[Create]**: Creates shifts in the Production Monitor with the new data that you have entered. The button is only active if you have assigned a shift rule and a shift group with machines.

**[New]**: Creates a new shift rule. The list box is not used at present.

**[Delete]**: Deletes a selected shift rule.

**[Apply]**: Saves the data.

**[Quit]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-228

# Shift Group

> Master data > Capacity planning > Shifts > Shift group

*Fig. E-134 Shifts - Edit shift group*

In this view of the dialog, you assign the registration points to a shift group. One shift group can be created per shift rule.
⇨ Tutorial, "Creating a Shift Group" on page E-82

### Edit shift group
**Name of Shift Group**: Name of the shift group to which the registration points are assigned.

**Registration Point Number**: Registration point number.

**Name**: Name of the registration point.

**Shift group**: Shift group that has been assigned to the registration point for the current shift plan. You can select another shift group.

**[New]**: Creates a new shift group. Each shift rule can only be assigned one shift group.

**[Delete]**: Deletes a selected shift group.

---
*A+W Production Capacity Planning*

## E-229

**[Apply]**: Saves the data.

**[Quit]**: Closes the dialog without saving the data.

# Machine

> Master data > Capacity planning > Shifts > Shift group > Machine

*Fig. E-135 Shifts - Machine*

In this view of the dialog, you assign the logical machines to a registration point.
⇨ Tutorial, "Creating a Shift Group" on page E-82

### Registration point
Properties of the selected registration point and the logical machines assigned to the registration point.

**Number (number)**: ID of the machine.

**Name**: Machine name.

**Barcode**: Barcode of the machine.

**Machines**: Logical machines assigned to the registration point.

---
*A+W Production Capacity Planning*

## E-230

**[Delete]**: Deletes the selected logical machine.

**[Apply]**: Saves the data.

**[Quit]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-231

# Machines and Costs

Machines can be arranged in groups to help planning the available times. The costs are also stored on the machines.

This section provides information on the following subjects:
- "Cost Calculation" on page E-232
- "Machinery Groups" on page E-234
- "Load Distribution" on page E-235

---
*A+W Production Capacity Planning*

## E-232

# Cost Calculation

> Master data > Capacity planning > Cost calculation

*Fig. E-136 Cost calculation*

On this dialog, you specify costs that arise on logical machines.
If your PPS- and ERP systems, e.g. A+W Enterprise and A+W Business, have been completely set up, the costs will be reported back to the ERP system.
⇨ Tutorial, "Cost Calculation" on page E-87

---
*A+W Production Capacity Planning*

## E-233

### Costs
In the overview, all machines defined are displayed.

- **Machine**: Number and name of the physical machine for which the costs are defined. A double-click opens a dialog to select a machine.
- **Log. Machine**: Assigned logical machine for which the costs are defined. A double-click opens a dialog to select a logical machine.
- **Labor Costs**: Labor costs of the logical machine in the local currency.
- **Machine Costs**: Machine costs for the logical machine in the local currency.
- **Other Costs**: Other costs of the logical machine in the local currency. With these costs, for example, you can consider that additional protective clothing is required on a machine and its costs have to be considered.
- **Comment**: Comments about the logical machine.

**[New]**: Adds a new line to create additional machine costs.

**[Delete]**: Deletes the selected entry.

**[OK]**: Takes over the selected entry into the Default time formula dialog.

**[Quit]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## E-234

# Machinery Groups

> Master data > Capacity planning > Machinery groups

*Fig. E-137 Machinery groups*

On this dialog, you can combine machines into groups and assign a number of people. This way, there is a specified capacity for the entire machine group, e.g. for work areas such as cutting, IG, and dispatch.

Machines can be arranged in a machinery group only if the shifts of all machines in the group match.

When a machine is added to a machinery group, it automatically becomes a bottleneck machine. The overload settings for the logical machine will be adapted to the overload settings of all logical machines in the group.
⇨ Tutorial, "Machinery Groups" on page E-131

### Machinery groups
**Group**: List of defined machinery groups.
**Staff**: Number of staff members who work on the respective machinery group.

---
*A+W Production Capacity Planning*

## E-235

### Machines for group
The field on the left lists the logical machines that can be added to a selected machinery group. The list on the right shows the logical machines that have been added to the machinery group.

**[Allocate]**: Moves a selected element to the other side.
**[New]**: Opens a dialog to create a new machine group.
**[Delete]**: Deletes the selected entry.
**[OK]**: Saves the data.
**[Quit]**: Closes the dialog without saving the data.

# Load Distribution

> Master data > Capacity Planning > Load Distribution

*Fig. E-138 Load distribution*

The Load Distribution dialog defines the loads of the logical machines as a percentage of the physical machines. If two logical machines have been defined for a machine, the 100% of the machine load can be distributed to the logical machines, e.g. 50% each.

You use load distribution to guarantee that a machine holds free a guaranteed minimum capacity for special tasks, e.g. for shape cutting. If the capacity held free is not used for shapes, rectangles can also be processed. This load dis-

---
*A+W Production Capacity Planning*

## E-236

tribution is only possible and makes sense for machines that are defined as bottleneck machines.
⇨ Tutorial, "Load Distribution" on page E-137

### Load Distribution
**Physical machines**: Choose the machines to edit the load distribution.

**Enable check**: The load distribution is locked to prevent accidental changes.
- The load distribution of the logical machines on the list cannot be edited.
- The load distribution of the logical machines on the list can be edited.

**[OK]**: Saves the data.

**[Cancel]**: Closes the dialog without saving the data.

---
*A+W Production Capacity Planning*

## Index: Capacity Planning

### A
- **Action for BOM configuration** E-168
- **Add elements** E-203
- **Adjust shifts** E-160
- **Alternative machines** E-18
- **Asynchronous processing** E-178
- **Automatic rescheduling** E-17

### B
- **BOM**
  - element chains E-16
  - BOM configuration E-167
- **Bottleneck**
  - machine E-29
  - work shift E-27

### C
- **Calculation sequence** E-201
  - default time formula E-111
- **Calendar**
  - creating non-working days E-71
  - deleting non-working days E-73
  - editing non-working days E-72
- **Campaign**
  - creating E-46
  - creating individual date E-47
  - creating individual dates E-47
  - creating weekly date E-49
  - delete date E-51
  - deleting E-52
  - disable E-52
  - edit E-51
- **Campaign days** E-184
- **Campaigns** E-183
  - Campaign days E-184
  - Individual dates E-183
  - individual dates, weekly dates E-44
  - scheduling E-46
  - Weekly dates E-185
- **Changes to scheduled orders** E-179
- **Cost calculation** E-232
  - definition E-88
- **Costs** E-232
  - creating E-89
  - deleting E-91
  - edit E-90
- **Create new filter (Production monitor)** E-158
- **Creating individual dates in campaigns** E-47
- **Creating work shifts** E-77
- **Creation of Processings** E-193
- **Creation of processings**
  - Add condition E-195
  - Sequence E-194

### D
- **Date optimization**
  - rules E-15
- **Dates**
  - campaigns E-44
  - creating a campaign E-47
  - creating campaign E-49
- **Default Time Formula** E-199
- **Default time formula** E-107, E-112
  - Add elements E-203
  - Calculation sequence E-201
  - calculation sequence E-111
  - condition for arcs E-114
  - condition for shape E-115
  - condition for threshold E-115
  - Copy formula E-215
  - creating vector E-121
  - defining E-118
  - Enter time formula element E-208
  - example E-113
  - Factors E-204
  - factors E-108
  - fixed elements E-108
  - Formula E-215
  - Formula evaluation process E-216
  - Formula object properties E-212, E-214
  - Input help for vectors E-110, E-205
  - Limit for table E-211
  - Select formula E-207
  - Show formula E-215
  - table E-109
  - test time formula E-124
  - time formula object E-116
  - Time formula test E-212
  - User-defined table elements E-210
  - Vectors E-204
  - vectors E-109
- **Default time formulas**
  - copy syntax E-129
  - deleting E-123
  - test calculation E-125
  - testing E-124
  - time surcharges E-110
- **Default Times** E-197
- **Default times**
  - definition E-106
- **Defective orders** E-177
- **Deleting expired reservation** E-60
- **Dwell time** see transition times

### E
- **Error**
  - scheduling E-40
- **Expired reservations** E-186
- **Export**
  - Work plan E-33

### F
- **Factors** E-204
- **Factors (default time formula)** E-108
- **Fixed elements (default time formula)** E-108
- **formula editor** E-112
- **Formula evaluation** E-216
- **Formula evaluation process** E-216
- **Formula object properties** E-214
- **formula structure** E-107

### H
- **High-priority order** E-171

### I
- **Individual dates (campaign)** E-183
- **Individual filters (Production monitor)** E-157
- **Input help for vectors** E-205

### L
- **Load Distribution** E-235
- **Load distribution**
  - definition E-138
  - deleting E-142
  - editing E-141
  - set-up E-139
- **Logical machine**
  - create costs E-89
  - default time E-106
  - Shift group E-229
- **Logical machine see also machine**

### M
- **Machine**
  - bottleneck E-29
  - creating costs E-89
  - deleting costs E-91
  - rescheduling E-36
  - setting display type E-32
  - work shift E-28
- **Machine costs**
  - edit costs E-90
- **Machine paths**
  - alternative machines E-18
  - processing chains E-17
- **Machine see also logical machine**
- **Machine shifts** E-147
- **Machinery group**
  - creating E-133
  - deleting E-135
  - editing E-135
- **Machinery groups** E-234
  - definition E-132
- **Machines**
  - Display in Production monitor E-151
  - display in Production Monitor E-30
- **Master data**
  - Capacity planning E-14
  - Machine allocation E-14
  - protection, data back-up E-67
- **Matrix for transition times** E-100

### N
- **Non-working days**
  - creating E-71
  - deleting E-73
  - editing E-72

### O
- **Order**
  - post-processing scheduling E-41
  - rescheduling E-36
  - reservation E-54
  - Schedule E-35
  - Select (Production monitor) E-155

### P
- **Post-processing of scheduling** E-174
  - Changes to scheduled orders E-179
  - Defective orders E-177
- **Processing**
  - adding E-64
  - creating E-64
  - rescheduling E-37
  - resolving E-65
- **Processing chains** E-17
- **Processing creation** E-63
- **removing processing** E-65
- **Processing time** see default times
- **Processings**
  - rescheduling E-38
  - Split items E-180
- **Production dates**
  - evaluation E-19
- **Production Monitor**
  - adjustments E-23
  - detailed view E-23
  - display machines E-30
  - set display E-31
- **Production monitor** E-21, E-147
  - Adjust shifts E-160
  - Create new filter E-158
  - creating work shifts E-77
  - Displayed machines E-151
  - Filter by batch E-156
  - Filter by order E-155
  - Individual filters E-157
  - Machine E-159
  - Presentation of shifts E-152
  - Select batch E-155
  - Select order (Production monitor) E-155
  - Settings E-152
  - Shift properties E-161

### R
- **Rescheduling** E-169, E-173
  - high-priority order E-169
  - lock date E-169
  - machine E-36
  - order E-36
  - Post-processing of scheduling E-174
  - processing E-37
  - Receipt of goods E-171
- **Rescheduling** E-173
- **Reservation**
  - capacities E-54
  - configuration E-53
  - creating E-56
  - deleting E-59
  - deleting expired reservation E-60
  - editing E-58
  - expired E-55
  - order E-54
- **Per shift** E-188
- **Select project** E-191
- **Reservation for Machine** E-189
- **Reservations** E-187
  - by day, by week E-188
  - Expired reservations E-186
  - Per customer E-188
  - Per machine E-188
- **Reserve capacity** E-54
- **Rules**
  - date optimization E-15
  - scheduling E-16

### S
- **Scheduling** E-16, E-146, E-166
  - Asynchronous processing E-178
  - BOM E-16
  - BOM configuration E-167
  - campaigns E-46
  - Changes to scheduled orders E-179
  - Defective orders E-177
  - Error E-174
  - error E-40
  - machine paths E-17
  - post-processing E-41
  - Processing creation E-63
  - production dates E-18
  - Schedule orders E-35
  - Split items E-180
  - transition times E-94
- **Scheduling rules** E-14
- **Select batch** E-155
- **Select customer for reservation Reservation**
- **Select customer** E-190
- **Select formula** E-207
- **Select project (reservation)** E-191
- **Sequence (creation of processings)** E-194
- **Shift**
  - special case for change E-97
- **Shift calendar** E-223
- **Shift change special case** E-97
- **Shift group** E-228
  - creating E-82
  - deleting E-86
  - editing E-85
- **Shift plan** E-224
  - creating E-75
  - deleting E-77
  - editing E-76
- **Shift plans** E-69
- **Shift properties** E-161
- **Shift reservations** E-188
- **Shift rule** E-226
  - creating E-78
  - deleting E-81
  - editing E-80
- **Shifts** E-221
  - Logical machine E-229
  - Shift calendar E-223
  - Shift group E-228
  - shift group E-82
  - shift plan E-224
  - shift plan E-76
  - Shift rule E-226
  - shift rule E-80
- **Transition time** E-218
- **Split items** E-180
- **Surcharges on default time** E-110

### T
- **table (default time formula)** E-109
- **Test time formula** E-124
- **Threshold value (default time formula)** E-115
- **Time formula element** E-208
- **Time formula object** E-116
- **Time formula test** E-124, E-212
  - Formula object properties E-212, E-214
- **Transition**
  - hours E-96
  - in hours or shift E-94
  - shifts E-95
- **Transition time**
  - creating E-101
  - deleting E-103
  - editing E-103
  - hours E-96
  - shifts E-95
  - special case E-97
  - type E-99
- **Transition Times** E-92
- **Transition times** E-217
  - definition E-98
  - matrix E-100
  - scheduling E-94
  - Shifts E-218

### U
- **User-defined table elements** E-210

### V
- **Vectors** E-204
  - input help E-110
  - using in default time formulas E-121
- **Vectors (default time formula)** E-109

### W
- **Weekly dates (campaign)** E-185
- **Work plan**
  - Export E-33
- **Work shift**
  - adjustments E-23
  - bottleneck E-27
  - extending, shortening E-26
  - locking E-25
  - machine E-28
  - reserving E-26
  - setting up additional E-24
- **Work shifts** E-21, E-147
  - display E-31
