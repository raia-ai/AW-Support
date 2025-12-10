---
title: "EN_AWProduction_Capacity_Planning_4_3"
source: "EN_AWProduction_Capacity_Planning_4_3.pdf"
tags: ["capacity planning", "A+W Production", "transition times", "default times", "machinery groups", "load distribution", "manufacturing software", "production scheduling", "BOM", "master data"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A comprehensive tutorial and software reference for the A+W Production Capacity Planning module. This document details the setup and management of master data, including transition times, default processing times, machinery groups, and load distribution, which are essential for effective production scheduling."
long_description: "This document serves as a detailed guide for configuring the Master Data of Capacity Planning within the A+W Production software suite. It is structured into two main parts: a Tutorial and a Software Reference. The Tutorial section provides step-by-step, illustrated instructions for administrators and power users on how to define, edit, and delete critical master data components. These components include: 'Transition Times', which define the time required for a part to move between machines; 'Default Times', which are complex, formula-based calculations for processing duration on a specific machine, considering variables like area, thickness, and shape; 'Machinery Groups', used to combine machines for collective capacity management and bottleneck analysis; and 'Load Distribution', for allocating a machine's capacity across different types of tasks. The tutorial is rich with examples, screenshots, and tips to ensure correct setup. The Software Reference section provides a functional overview of the core scheduling tools, primarily the 'Production Monitor'. It describes its interface, features, and how it is used for planning, organizing, and rescheduling production capacities, including batch formation and handling defective orders. This manual is an essential resource for ensuring that the capacity planning system is configured accurately to reflect real-world production constraints and capabilities."
---

# Tutorial: Master Data of Capacity Planning

---
## Definition and Management of Transition Times

This unit will show you how to define, edit, or delete transition times. Consider that set-up and handling times must also be considered in the transition times.

For instructions on this subject, please see:
- "How to enter a transition time" on page E-101
- "How to edit a transition time" on page E-103
- "How to delete a transition time" on page E-103

> **Prerequisite**
> Before entering transition times you have to define the corresponding logical machines in machine allocation.

### How to enter a transition time

1. Go to **Master data > Capacity planning > Transition times**.
2. Click **[New]**.

A new line is added at the top of the list of machines.

**(Image: Setting up transition times - Fig. E-55)**
The user interface for setting up transition times shows a table with the following columns and controls:
- **A**: New line button
- **B**: Machine from which the part is departing
- **C**: Machine at which the part is arriving
- **D**: Type of transition time (e.g., Normal, Rush)
- **E**: Normal transition time in hours or shifts
- **F**: Maximum transition time in hours or shifts

3. Double-click in the field (B) in order to open the dialog for selecting the machine.
4. Select the desired machine with a double-click.
5. Repeat the step for the machine (C) for which you are specifying the transition. Also use the options *All machines to machine X* and *Machine X to all machines*.
6. Select the type (D) for the transition time and enter the appropriate time (E). Use shifts if possible. In exceptional cases, you can also use time periods, e.g. drying times.
7. Enter the maximum transition time (F). This way, you allow the system to extend the transition time. Here, you can also use hours or shifts.
    > **Tip**
    > For the transition to the last process, e.g. Packing or Dispatch, specify the longest transition time possible. This will give you greater flexibility in critical situations.
8. Repeat steps 2 and 7 for the next transition type (D) of the same machine combination.
9. Click [OK] to save the data.

You have thus created the transition times in the various transition types for a transition.

### How to edit a transition time

1. Go to **Master data > Capacity planning > Transition times**.
2. Correct the transition times for the desired machines. Activate the fields with a double-click.
3. If necessary, add a machine combination by creating data for another transition type. To do this, follow the description in the action sequence for creating transition times.
4. Click [OK] to save the changes. With that, you have changed the transition time.

### How to delete a transition time

1. Go to **Master data > Capacity planning > Transition times**.
2. In the first column, select the transition time to be deleted. The whole line for this transition time is highlighted.
3. Click **[Delete]**. The transition time is deleted from the list.
    > In case you have deleted a transition time from the list by mistake: Click the [End] button. If you confirm the message with [No], the dialog closes without saving the changes. The transition time is displayed in the list again when you open the dialog.
4. Click [OK] to close the dialog. The changes will be taken over in the database.

### Exercises

Create the data so that it is available in all subsequent exercises. If the data for the capacity planning is thus complete, you can test the planning for your own orders in the Production Monitor.
- Work with your trainer to create a new machine in the machine allocation completely, which you mark clearly as test machine for the capacity planning.
- Define the transition times for this machine in the rush and common grid.
- Create transition times between two machines for all types of transition times that are required for the transitions.
- Change the transition times.
- Check the results in the production monitor by means of a test order.

### Additional information
⇨ Software Reference, "Transition Times" on page E-217

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

## Definition of the Default Times

With a default time, you define how the duration of a work process is calculated on a logical machine. The basis of the calculation is the respective area or edge length of the individual order item.

> **Default Times**
> The default times are called processing times in machine allocation (MA). Since the default times are assigned to logical machines you can also enter formulas for default times in machinery allocation. This is done by means of the machine allocation editor, Logical machine tab in the Processing time field. These formulas from the MA cannot be changed on the Default Times dialog.

This dialog lists the logical machines via which processings are controlled. Default times are specified in A+W Production with default time formulas. You define the default time formulas on the **Formula for Default Time** dialog.

## Structure of Default Time Formulas

Each default time formula is based on a basis time that is specified in seconds. Default time formulas can be defined with specified elements. In addition, you can also create your own elements and use them in the formula.

**(Image: Default Time Formula - Fig. E-58)**
The "Formula for Default Time" dialog consists of:
- **A**: Elements of the default time formula
- **B**: Basis time in seconds
- **C**: Selection of the calculation operation
- **D**: Sorting sequence of the elements
- **E**: Multiplier for the processing quantity

With each line, a time surcharge is specified, which is either calculated as a formula or determined as a value of a table.

You can use several different elements (A) in a default time formula. For this, select the desired element, specify a value in seconds, and specify how the value should be used in the calculation operation (C). Important here is that the sequence (D) is sorted correctly. This is especially true if the next calculation operation builds on the intermediate result of the previous operation.

The basis time counts as start value. All other elements of the formula are therefore surcharges on the start value. If you do not enter a basis time, all calculations build on the result of the first entry (A).

By default, various elements are offered for selection, to which you can add with your own definitions:
⇨ "Editor for Formula Elements" on page E-112

### Example gas and shape

| Item | Value / Calculation |
| :--- | :--- |
| Basis time | 23 s |
| Factor for size | 23 * size factor |
| Factor for gas | Intermediate result * gas factor |
| Constants for shape | Intermediate result + shape constant |

With this default formula, you can calculate times for lites with gas filling and for shapes. If, however, you want to calculate LAMI, the formula must be structured as follows:

### Example LAMI, size and gas

| Item | Value / Calculation |
| :--- | :--- |
| Basis time | 23 s |
| Factor LAMI | + LAMI factor |
| Factor for size | Intermediate result 1 * size factor |
| Factor for gas | Intermediate result 2 + (23 * gas factor) |

### Fixed elements
Fixed elements are not assigned a value; instead, it is only specified how the elements affect the default formula. For calculation, the actual values of the glass are used. Thus, for example, for the Fixed element 'thickness' with a lite that is 4.00 mm thick, the value 4 is determined. For the Fixed element 'quantity', the number of lites and for a Fixed element 'area' the area of the lites is determined.

With the selection of the calculation operation, you specify on the **Formula for Default Time** dialog how the value determined is used in the default time formula.

### Factors
With a factor, you can specify a time surcharge that is always calculated if the prerequisite for the use of the factor is fulfilled.

**Example**
With the Value for 'Size of lite' you specify a surcharge on the basic time that is always calculated for oversized lites. When a lite counts as oversized is specified for the factor.

With the selection of the calculation operation, you specify on the **Formula for Default Time** dialog how the value determined is used in the default time formula.

### Vectors - tables and cubes
Vectors permit an exact planning of default times based on the properties of the workpiece. Vectors can be used to take into account the default time, e.g. for the glass thickness, area to be processed, the edge structure, and the aspect ratio of a lite.

**(Image: Vector 'Thickness -> factor' - Fig. E-59)**
This shows a table where time surcharges (as a factor) are defined based on lite thickness.
Example:
- 4 mm -> 1
- 6 mm -> 1.2
- 8 mm -> 1.4

Different lite thicknesses are e.g. allowed for by the vector 'Thickness → factor'. This way, you specify time surcharges depending on the thickness of a lite.

If you specify the value in the Vector 'Thickness→ factor' as table, you can scale the value of the vector, e.g. from 4.00 - 5.99 mm thickness, the value 0.1 applies; for 6.00 - 7.99, the value 0.2 applies, etc.

With the selection of the calculation operation, you specify on the **Formula for Default Time** dialog how vectors are used in the default time formula.

### Input help for vectors
Vectors are entered on the Factor/vector (name) dialog. This table contains one surcharge value per limit value (scale level). To create such a table, there are two procedures available:
- You specify the values individually in the table. Here, for example, you specify several levels of thicknesses, lengths or weights and assign each of these a value.
- You can have the scale levels and scaled values calculated.

For this calculation, you specify a start and end value, e.g. 4.00 - 20.00 mm for the thickness. If you specify 2.00 mm as step size, a step is inserted every 2.00 mm between the start and end values.

If you specify 0.1 as start value for the surcharge and 0.1 as the step size, then the value 0.1 applies for the first step, and for all further levels, this value is increased by 0.1.

For the table, the result is: lites with a thickness of 4.00 - 5.99 mm have the value 0.1; from 6.00 - 8.00 mm, the value 0.2, etc.

### Calculation of Time Surcharges
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

### Sequence of the calculations
For the calculation, you must consider the operator sequence of mathematics: multiplication and division are calculated before addition and subtraction unless parentheses specify the sequence.

**Example**

| Expression | Result | Note |
| :--- | :--- | :--- |
| `1 + 2 * 4` | = 9 | Multiplication first |
| `(1 + 2) * 4` | = 12 | Brackets first |
| `1 + (2 * 4)` | = 9 | |
| `4 * (1 + 2)` | = 12 | |
| `6 + (9 / 3)` | = 9 | |
| `(6 + 9) / 3` | = 5 | |

For calculation of the time surcharges, the following settings are available:

**Tab. E-1: Possible settings for the default time formula**

| Setting | Meaning |
| :--- | :--- |
| `+ Table` | The value from the table is added to the intermediate result. |
| `+ b * value` | The basic time is multiplied by the value. The result of the multiplication is added to the intermediate result. |
| `+ value` | The value is added to the intermediate result. |
| `* (1 + value)` | The value is added to 1 and the result multiplied by the intermediate result from the previous line. |
| `* Vector` | The result of the previous line is multiplied by the value of the vector. |

If the calculation begins with the determination from a formula, specify 0 as start value, e.g. the calculation of an area before the first screen printing is applied.

If the calculation is based on the result of the previous line, the sequence of entries is important.

### Editor for Formula Elements
For the definition of individual formula elements, there is an editor in which you can create your own formulas or select a pre-defined formula.

**(Image: Entering time formula elements - Fig. E-61)**
The editor dialog contains:
- **A**: Name of the formula element
- **B**: Selection of the type
- **C**: Labeling
- **D**: Calculation formula
- **E**: Input format
- **F**: Independent parameter

You give the formula element a name (A), which is displayed in the selection of formula elements and a label (C) that is displayed on the **Formula for Default Time** dialog. The second label is displayed before the calculation value.

You use the various element types (B) for the following calculations:
- **Fixed element**: Expressions without user input, e.g. long edge. This setting should no longer be used for new definitions; it has been replaced by **Free element**.
- **Condition**: Expressions with a user input that is used if the condition is true.
- **Free element**: Expressions for which the result is weighted with the user input (e.g. seconds per meter ground).
- **Threshold value**: Expressions for which the threshold value for the condition can be set without changing the formula definition (e.g. quantity surcharge starting with user input).
- **Vector**: Expressions for which a table with value pairs of minimum values and coefficients to be used is maintained.

You can write the actual formula definition (D) of the element as a formula or select a pre-defined formula and adjust it. For vectors, you cannot change the definition, therefore, the field is grayed out.

### Example – Default Time for the Logical Machine Cutting
You have determined the area dependency of your cut from production statistics. Furthermore, you 'know' that the arc shapes take 20 seconds longer on average and the table requires 10% more time for edge deletion of insulated glass components.

In order to be able to react quickly to production changes, you want to be able to set the complete default time formula to faster or slower with a control parameter.

**(Image: Example – default time formula - Fig. E-62)**
The formula setup shows:
- Basic Time: `0.95` with operation `* (1 + Value)`
- Edge Del...: `0.1` with operation `*Vector`
- Cutting Surface:
- Round Arch...: `20` with operation `+ Value`

**Tab. E-2: Example - conditions of calculation**

| Line | Definition | Explanation |
| :--- | :--- | :--- |
| Basic time | `0.95` | The control parameter is 95% of the default time, that is, it is set to faster. |
| Edge stripping | `* (1 + 0.1)` | The surcharge is only calculated for a coated lite for IG. |
| Area cut | `* Vector` | The result is multiplied by the times for the sheet area. |
| Arc shape | `+ 20` | For a shape with round arcs, 20 seconds are added. |

The actual times are maintained in the vector for the cut area, e.g.:

| Area (qm) | Val. | Explanation |
| :--- | :--- | :--- |
| 0.1 | 70 | up to 0.099 sq m, 70 seconds are calculated |
| 0.5 | 45 | for 0.1 - 0.499 sq m, 45 seconds are calculated |
| 1.0 | 60 | for 0.5 - 0.999 sq m, 60 seconds are calculated |
| 2.0 | 150 | for 1.5 - 1.999 sq m, 150 seconds are calculated |
| 3.0 | 210 | for 2.0 - 2.999 sq m, 210 seconds are calculated |

In this example, you see that for very small and for large lites, more time is required for cutting. Thus, there is another size surcharge for cutting. For area processings, such a surcharge may be necessary and must be defined on the appropriate logical machine.

#### Condition: shape with arcs
The condition should only supply the user input as result if it is true.
**Definition (example)**
```
IF (($Parts_MODELL_NR >= 60 AND $Parts_MODELL_NR <= 81) OR
($Parts_MODELL_NR >= 113 AND $Parts_MODELL_NR <= 118) OR
($Parts_MODELL_NR >= 123 AND $Parts_MODELL_NR <= 125) OR
($Parts_MODELL_NR >= 133 AND $Parts_MODELL_NR <= 199))
THEN 20 END
```
> **Length specification in the formula**
> Note that the length values in a formula must be specified in µm.

#### Condition: threshold value
With more than 11 pieces, the default time should be 10% smaller.
**Definition (example)**
```
IF ($Parts_MENGE > 11) THEN - 0.1 END
```

#### Condition: vector for shape cutting
Vectors can depend on units or depict non-linear situations. If the simple surcharge for shapes with arcs is not precise enough for you, define a vector, with help of which you can query the required coefficients easily and very precisely.

On the dialog for entering a shape element, you can create a new element with the element type **Vector**. For a valid vector, select a formula for the independent parameter, e.g. `AWF_ShapeNumber`.

The table permits the shape-dependent scaling of the surcharges. The entry for the left column always provides the start value of the validity range. It's good practice to define a value pair for 0 so that the value range is described completely.

### Time Formula Objects
You can map the BOM or elements of the BOM as formula objects in order to depict the chain of processings. This display serves to test the dependencies of the processings in the default time formula, e.g. to check how the processing depends on what is done in the counter-lite. Formula objects are used for testing formulas with logical quantities.

Formula objects always refer to a particular default time formula. They cannot be used across the boards. You can save the formula objects if you want to have proof that the formula is applied correctly.

**(Image: BOM tree from the point of view of the individual processings - Fig. E-64)**
The dialog shows:
- **A**: Save whole object
- **B**: Delete object
- **C**: Add object
- **D**: Delete selected object
- **E**: Objects (in a tree structure)

In this example, you see the processing BOM of an IG lite. When adding, the formula objects (E) are numbered. With a double-click, you can open each formula object and rename it, e.g. the first object to IG. This makes sense to clarify the structure. When adding (C), a new object is created below the selected object. When deleting (D), the selected object and all sublevels are deleted.

> **Loading a saved object for testing**
> A saved formula object can only be used for the formula for which it was created, e.g. to test changes in the default time formula. Therefore, it makes sense to give meaningful names when saving.

There is an example of a formula object under the test of the default time formula.
⇨ "Here's how to test the calculation of the time formula" on page E-125

## Definition and Management of Default Time Formulas

This unit will tell you how to define, edit, or delete default time formulas.

In the first line on the **Formula for Default Time** dialog, you can define formula elements as templates for all machines. If for the machine 0 you define a time formula, this is saved in the database, however the formula is not used since the machine 0 is not assigned a processing in the MA.

> **Prerequisite**
> Default time formulas are defined for the logical machines that execute a particular work process. Therefore, the appropriate logical machines must be defined in the machine allocation.

For instructions on this subject, please see:
- "Here's how to define a default time formula" on page E-118
- "Here's how to create a vector with the input help" on page E-121
- "Here's how to delete a default time formula" on page E-123

> **Complexity of default time formulas**
> A+W Production allows defining default time formulas of any complexity required. This permits the handling of all sorts of special cases. Keep default time formulas as simple as possible. If in your production it is necessary to use complex default time formulas, please contact the A+W Software GmbH customer service.

### Here's how to define a default time formula

1. Go to **Master data > Capacity planning > Default times**.
2. Select the logical machine for which you want to define a default time formula.
3. Click **[Edit]**. The **Formula for Default time** dialog opens.
   A warning will be issued if a formula for the processing time has already been entered for this logical machine in machine allocation. If you proceed, the formula entered in machine allocation will be overwritten.
4. Enter the basic time (A) in seconds. You can either add a predefined formula (E) and save the data or build a formula with formula elements. The following steps will demonstrate the building with formula elements.
5. Click [New] (D) to select an element.
6. Select the element, e.g. a vector, and take over the selection with [OK]. The selected element now appears on the list in the **Formula for Default time** dialog.
7. Click **[...]** (A) in order to open the dialog for entering the values.
8. Select the operator (B) for the calculation.
9. Repeat the steps 5 - 8 to add additional elements.
10. Check the sequence of the formula elements. The sequence is important for the calculation if the surcharge refers to the intermediate total of the previous element.
11. Click [OK] to apply the data. The dialog closes. Thus, you have compiled a default time formula. You can check the calculation and start a calculation with sample values with a formula object.
    - ⇨ "Testing Time Formulas" on page E-124
    - ⇨ "Time Formula Objects" on page E-116

### Here's how to create a vector with the input help

1. Go to **Master data > Capacity planning > Default times > Default time formula**.
2. Enter the basic time in seconds.
3. Click [New] and select an element, e.g. **Vector 'thickness -> factor'**.
4. Click [Input help].
5. Enter the start and end values for the scaling, e.g. **4.00** and **20.00**. These values specify the smallest and largest thickness.
6. Enter the step size, e.g. **2.00**. This value specifies at what steps the limit values for the scaling are calculated between the start and end values.
7. Enter the start value and the step size for the factor, e.g. **0.1**. This value specifies by what size the factor is increased per limit value.
8. Click [OK] to start the calculation of the table. The **Input help for vectors** dialog closes. The tables are calculated and taken over on the **Vector -> thickness** dialog. You can correct and complete the data.
9. Click [OK] to save the data. The **Vector thickness -> factor** dialog closes. The scaling created is taken over in the default time formula.

### Here's how to delete a default time formula

1. Go to **Master data > Capacity planning > Default times > Default time formula**.
2. Select the element that you want to delete.
3. Click [Delete].
4. Repeat the steps 2 and 3 until all elements that are no longer needed have been removed from the list.
5. Set the basic time to zero.
6. Click [OK] to save the data.
The dialog closes.

To delete a default time formula completely, select the default time on the **Default times** dialog and click **[Delete]**.

### Testing Time Formulas

On the **Time formula test** dialog, you can test formulas and check the values and calculation settings. You can either test the formula you are currently editing on the **Formula for Default time** dialog or load a saved formula into the dialog in order to test it.

The formula test outputs a result that specifies the time for the work process in question in seconds.

For instructions on this subject, please see:
- "Here's how to test the time formula" on page E-124
- "Here's how to test the calculation of the time formula" on page E-125
- "Here's how to create a copy of the time formula syntax" on page E-129

In addition, you can define formula objects that you can use to test all formulas. You specify the specific case there in which you want to test the formula, e.g. the thickness and width of a lite. Thus, you always have the same defaults for the test.
⇨ "Time Formula Objects" on page E-116

#### Here's how to test the time formula
1. Go to **Master data > Capacity planning > Default times > Default time formula**.
2. Select the formula element that you want to test. If you want to test the entire default time formula, you must select the **Basic Time** element. However, you can also test each element individually.
3. Click **[Formula test]**.
4. Click **[Evaluate] (B)**. The calculation result (A) is displayed. If necessary, you can edit and correct the formula.
5. Click [OK] to save the data.

To test the formula with lite data, you can create a formula object for the test and enter values.

#### Here's how to test the calculation of the time formula
1. Go to **Master data > Capacity planning > Default times > Default time formula**. Dialog **Default time formula** appears.
2. Click **[Formula test]**.
3. Double-click on the formula object (A) to open the dialog for entering the properties.
4. Enter a name (A) and select the type (B), e.g. element.
5. Click **[Add]**. The fields in the **Properties** column are pre-populated with the elements that are included in the current default time formula.
6. Enter the appropriate values for each property, e.g. the dimensions for height and width. Note that you must specify the dimensions in micrometers µm.
7. Click **[Close]** to save the data and close the dialog. The **Formula test** dialog is displayed in the foreground.
8. Select the formula object for which the calculation should be started.
9. Click **[Formula test]**. The result of the calculation with the values input is displayed. If the calculation does not do what you want it to, you can check the calculated values.

#### Here's how to create a copy of the time formula syntax
1. Test the time formulas as specified in the previous action sequence.
2. Check the **Display formula** checkbox (A).
On this dialog, you can check the syntax of the whole formula. To correct the syntax with the help of A+W service, copy the syntax and send the text to A+W.

### Exercises

- Select a logical machine from your test machines and plan the default times for this logical machine on paper:
    - Which lites are going to be processed on this logical machine?
    - Which factors are necessary to define the default times for these lites?
    - How shall these factors be included in the default time formula?
- Create the default time formula based on the necessary elements.
- For the entry `0 - all machines`, enter various formula elements, e.g. a specific vector, a table, a threshold value.
- Create a formula object for a formula and test the default time formula in order to check whether the result meets your expectations.

### Additional information
- ⇨ Software Reference, "Default Times" on page E-197
- ⇨ Software Reference, "Default Time Formula" on page E-199
- ⇨ Software Reference, "Tabelle, Vector (Name)" on page E-204
- ⇨ Software Reference, "Input Help for Vectors" on page E-205
- ⇨ Software Reference, "Entering a Formula Element" on page E-208

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

## Definition of the Machinery Groups

You can combine machines into groups. Machinery groups make sense for machines in the same area. Thus, e.g. you could create a machine group **Cutting** to which you assign all machines in cutting. A specified capacity then applies for the entire machinery group, that is, for cutting.

You can only combine machines into a group whose shifts match; that is, that are available for the same time. Machines that you add to a machinery group automatically become bottleneck machines.

You must assign each of the machinery groups a number of people (C). A+W Production basically assumes that one person is working on each machine. If you reduce the number of employees in the group, the available time per machine decreases.

**Example**
In the **Cutting** machinery group with four machines, there are four people assumed. If the 4 employees work 40 hours per week, 4 x 40 = 160 working hours per week available.
With 3 employees, only 3 x 40 working hours = 120 hours per week are available.

## Definition and Management of Machinery Groups

This unit will tell you how to define, edit, or delete machinery groups.

For instructions on this subject, please see:
- "Here's how to create a machinery group" on page E-133
- "Here's how to edit a machinery group" on page E-135
- "Here's how to delete a machinery group" on page E-135

### Here's how to create a machinery group

1. Go to **Master data > Capacity planning > Machinery groups**.
2. Click **[New]**.
3. Enter a name for the machinery group, e.g. **Cutting**.
4. Click **[OK]**.
5. Select the new machinery group. The list **Machines for group** shows all available machines.
6. Select the machine that you want to add to the group, e.g. **180 Cutting table 8**.
7. Click the arrow to the right and confirm the message. The machine was added to the group.
8. Repeat the steps 5 to 7 to add more machines.
9. Go to field **Machinery groups** and double-click the **Persons** (Staff) column.
10. Enter the number of persons working in this machinery group.
11. Click [OK] to save the data. The dialog closes. That done, you have defined the machinery group.

### Here's how to edit a machinery group

1. Go to **Master data > Capacity planning > Machinery groups**.
2. Go to the **Machinery groups** field and select the machinery group to be edited. The right side of the list **Machines for group** lists all machines that have been added to the group. The left side lists the available machines.
3. Select a machine to be removed from or added to the group.
4. Click the [Arrow left] or [Arrow right] button to remove a machine from the group or add a machine to the group.
5. Repeat the steps 3 to 4 to remove more machines from the group or add more machines to the group.
6. In the **Machinery groups** field, correct the number of people.
7. Click [OK] to save the data. The changes are saved and the dialog closed.

### Here's how to delete a machinery group

1. Go to **Master data > Capacity planning > Machinery groups**.
2. In the **Machinery groups** field, select the machinery group to be deleted.
3. Click **[Delete]**. The machinery group is removed from the list. This way, you change the available capacity for scheduling.
4. Click [OK] to save the data. The changes are saved and the dialog closed.

### Exercises

Create the data so that it is available in all subsequent exercises. If the data for the capacity planning is thus complete, you can test the planning for your own orders in the Production Monitor.
- Decide which machines you want to be arranged in a group.
- Create at least one machinery group on the **Machinery groups** dialog.
- Edit your machinery group.
- Delete one of your machinery groups.

### Additional information
⇨ Software Reference, "Machinery Groups" on page E-234

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
| **Logical machines** | The load distribution is made among the logical machines that have been defined for a physical machine. This way, you can break down the load distribution of a CNC center as percentages with the three logical machines: Special edges, Cut-outs, and Drillings. |
| **Bottleneck machine** | A bottleneck machine cannot be booked beyond its capacity. |

## Definition of Load Distribution

The load distribution is specified among the logical machines that have been defined for a physical machine. This way, you specify the percentage share of the logical machines of the total capacity of the physical machine.

You use load distribution to guarantee that a machine holds free a guaranteed minimum capacity for special tasks, e.g. for shape cutting. If the capacity held free is not used for shapes, rectangles can also be processed. This load distribution is only possible and makes sense for machines that are defined as bottleneck machines.

You break down the capacity of a machine by allocating percentage shares (D) to the associated logical machines (C).

**Example**
A machine can process shapes, that is, rectangles and shapes. So that this special qualification is not occupied by the simpler rectangles, keep 30% free for shapes, for example. This load distribution is considered during scheduling.
If this 30% is not needed for shapes, rectangles can also be processed.

## Definition and Editing of Load Distribution

This unit will show you how to define, edit, and delete load distributions.

For instructions on this subject, please see:
- "Here's how to set up load distribution" on page E-139
- "Here's how to edit load distribution" on page E-141
- "How to delete load distribution" on page E-142

> **Prerequisite**
> Load distribution can only be defined for machines that have been specified as bottleneck machines.

### Here's how to set up load distribution

1. Go to **Master data > Capacity planning > Load distribution**.
2. Select the machine (A) whose capacity you want to break down. The selection list includes only the machines that are defined as bottleneck machines.
3. Check the **Enable check** checkbox (B) to enable the fields. The fields for the logical machines are enabled. If there is no load distribution specified, **Unlimited** will appear in the right column.
4. Double-Click the right column.
5. Enter the percentage for the capacity.
6. Repeat steps 4 and 5 in order to set up the percentage of total capacity of the physical machine for all logical machines.
7. Uncheck the **Enable check** checkbox to prevent inadvertent changes.
8. Click [OK] button to save the data and close the **Load distribution** dialog. The data is saved and the dialog closed.

### Here's how to edit load distribution

1. Go to **Master data > Capacity planning > Load distribution**.
2. Select the machine whose load distribution you want to edit. The selection list includes only the machines that are defined as bottleneck machines.
3. If necessary, check the **Enable check** checkbox.
4. For all logical machines, change the percentage value for the capacity.
5. If necessary, uncheck the **Enable check** checkbox.
6. Click [OK] to save the data. The changes are saved and the dialog closed.

### How to delete load distribution

1. Go to **Master data > Capacity planning > Load distribution**.
2. Go to field **Physical machine** and select the machine the load distribution of which you want to delete. The corresponding logical machines are listed.
3. Check the **Enable check** checkbox. The fields will be enabled.
4. For all logical machines, change the percentage value for the capacity to **000%**. **Unlimited** is displayed in the fields.
5. If necessary, uncheck the **Enable check** checkbox.
6. Click [OK] to save the data. The changes are saved and the dialog closed. You have deleted the load distribution for this machine.

### Exercises

Create the data so that it is available in all subsequent exercises. If the data for the capacity planning is thus complete, you can test the planning for your own orders in the Production Monitor.
- Check for which machines a load distribution makes sense.
- If necessary, create logical machines for your test machines beforehand.
- Set up at least one load distribution.
- Edit the load distribution.
- Delete the load distribution.

### Additional information
⇨ Software Reference, "Load Distribution" on page E-235

---

# Software Reference

## Overview

The **Production Monitor** dialog is available for planning and organizing the capacities of your production. It displays the work shifts per machine.

The orders are scheduled item by item, whereby the scheduling per item must be successful. If an order item cannot be scheduled successfully, the whole order is not scheduled.

So that the calculation in the Production Monitor is done correctly, the capacity planning master data must be set up. The description of the dialogs is grouped in topics. It does not follow the arrangement of the dialogs in the software reference.

The software reference provides information on the following subjects:
- "Scheduling" on page E-146
- "Campaigns and Reservations" on page E-182
- "Processings" on page E-192
- "Time Master Data" on page E-196
- "Master Data for the Shifts" on page E-220
- "Machines and Costs" on page E-231

## Scheduling

The **Production Monitor** is the central capacity and order control desk and entry point for work preparation, e.g. batch formation, rescheduling.

This section provides information on the following subjects:
- "Production Monitor" on page E-147
- "Displayed Machines" on page E-151
- "Settings" on page E-152
- "Please Select an Order/Batch" on page E-155
- "Create New Filter" on page E-158
- "Machine (Name)" on page E-159
- "Adjust Shifts for Machine" on page E-160
- "Shift Properties" on page E-161
- "Reservation Display" on page E-162
- "Workplan from Production Monitor" on page E-163
- "Scheduling" on page E-166
- "BOM Configuration" on page E-167
- "Action" on page E-168
- "Rescheduling" on page E-169
- "Machine Reallocation" on page E-173
- "Post-Processing Booking" on page E-174
- "Defective Orders" on page E-177
- "Asynchronous Processing" on page E-178
- "Changes to Scheduled Orders" on page E-179
- "Split Items" on page E-180

### Production Monitor
**Display > Production Monitor**
**Details View > Context Menu > Production Monitor**

This dialog displays the current state of production and the use of machine capacity per work shift. This makes the Production Monitor the capacity and order control desk and the entry point for work preparation, e.g. batch formation, rescheduling.
⇨ Tutorial, "Production Monitor" on page E-21

#### Buttons and Fields

| Icon / Field | Function | Description |
| :--- | :--- | :--- |
| (Icon) | Selected machines | ⇨ "Displayed Machines" on page E-151 |
| (Icon) | Settings | ⇨ "Settings" on page E-152 |
| (Icon) | Change display type for all machines | Selection of the display for all machines: Time, Quantity, Area, Weight |
| (Icon) | Change display (shift, day, week) | Changes the display. The machine capacity is shown per shift, per day, or per week. |
| (Icon) | Change view | Changes the view. **Main view**: All shifts in the specified time period are displayed. **Detail view**: Only the shifts for the day specified are displayed. |
| (Icon) | Zoom in, zoom out | Enlarges or reduces the display of the steps. |
| (Icon) | Refresh view | Refreshes the view. |
| (Icon) | Given number of days back, forward | Shifts the time period displayed back or forward by the number of days that is specified in the **Days** field. |
| (Icon) | Filter view, remove filter | ⇨ "Please Select an Order/Batch" on page E-155 |
| **Start date** | | Opens the calendar to select the start day for the display of work shifts. |
| **Days** | | Specification of by how many days the display with the buttons should be scrolled forward or back. |
| **Filter input field** | | Specification of the filter criterion, to filter the display by orders or batches. |

#### Display
The display can be adapted individually. This affects the colors, a time grid, status information, etc.
⇨ "Settings" on page E-152

#### Work shifts
The Production Monitor displays the work shifts for all selected machines. Machines that are defined as bottleneck machines are displayed in red. A bottleneck machine cannot be booked beyond its capacity.

The following information is available via the context menu:
- **Properties**: Opens a dialog on which you can change the machine properties. ⇨ "Machine (Name)" on page E-159
- **Shift properties**: Opens a dialog on which you can adjust shift times of the machine. ⇨ "Adjust Shifts for Machine" on page E-160
- **Display logical machines**: With this entry the display of the logical machines can be activated and deactivated. When using the context menu, the value stored in the master data is not changed, only the display is adapted, so that the change is only temporary. ⇨ "Misc" on page E-160

#### Status of the planning
The colored dots indicate the backlogs:
- **Green**: No backlog.
- **Yellow**: Backlog that can be made up on the same day by using the free capacities.
- **Red**: Backlog that cannot be made up for on the same day.

#### Display of the work shifts
Brief information about the status is displayed in the tooltip for a work shift. The following information is available via the context menu:
- **Work plan**: Opens the Work plan: Selection from A+W Production Monitor dialog with the overview of the batches and orders of the machine and shift. ⇨ "Workplan from Production Monitor" on page E-163
- **Delete**: Deletes a selected work shift from the Production Monitor.
- **Shift properties**: Opens the Shift properties dialog where you can change the properties of a shift. ⇨ "Shift Properties" on page E-161
- **Display reservations**: Opens the Display reservation dialog in order to check the reservations for a shift. ⇨ "Reservation Display" on page E-162

**Visual Indicators:**
- **Hatched**: The duration of the work shift is reduced.
- **X**: The work shift is deactivated.
- **!**: The shift was set to *Active for rush orders* and is therefore only available for rush orders.
- **?**: Undefined processings are scheduled in the work shift.
- **Frame**: The shift is defined as a bottleneck. ⇨ "Shift Properties" on page E-161
