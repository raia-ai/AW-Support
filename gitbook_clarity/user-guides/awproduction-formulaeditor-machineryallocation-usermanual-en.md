---
description: "EN_UM_AWProduction_8"
---


# Tutorial: Formula Editor

---
## Comparison
A comparison consists of 1-2 formulas, and a so-called comparison rule. Please note that you can use just one formula only if the comparison rule **Only formula 1** is used. In this case, the comparison is fulfilled if the result of formula 1 is one digit bigger than zero, or a non-empty string. Otherwise, the comparison is fulfilled if the term FORMEL 1 VORSCHRIFT FORMEL 2 is true.

For formula 2, no formula needs to be defined for simple constants. In this case, activate the radio button **Value** and enter the required constant.

(Reference Fig. F-2 Comparison GUI showing two formulas being compared with operators like '== (equal)', '< (smaller)', etc.)

## Examples
- Formula Part type = Value 1
- Formula IG Only formula 1
- Formula triple width < Formula height
- Formula Thickness = Value 3 mm

## Condition
A condition must be fulfilled so that the allocation can be made as defined by the formula(s). It is the top part within the formula structure and, in its simplest type, consists of a number of comparisons. The grouping of comparisons defines how the results of the comparisons must be linked to each other. Comparisons set next to another are linked by **AND** while comparisons set above one another are linked by **OR**. A condition is fulfilled if it is possible to find a horizontal path from left to right which only includes fulfilled comparisons.

(Reference Fig. F-3 Condition with And connection GUI showing three parallel comparisons for 'Thickness', 'Glass Type', and 'Number Child Part', implying an AND link.)

## Examples: Simplest Type

A schematic display of a condition (Fig. F-4) shows a `Condition` named "Is TG" which is composed of:
- A `Formula` ("Part Type TGH") which uses a `Property` ("ST TGH").
- A `Comparison` rule ("Only Formula 1").
- This structure forms an `Elementary Condition`.

Possible operations for comparison include: Only Formula, equal, unequal, smaller, smaller or equal, greater, greater or equal.

The condition "is TG" is fulfilled if the formula "Part type TG" with the property of database field `P_TG` from `Pool_Teile` contains the value One (based on the operation Only formula).

The Condition Editor (Fig. F-5) is composed of:
- **A**: Formula (e.g., Part Type TGH)
- **B**: Comparison (e.g., Only Formula 1)
- **C**: Elementary condition (e.g., Normal, Value, Conditions)

## Examples: Linking of elementary conditions

A schematic display (Fig. F-6) illustrates how elementary conditions can be linked.
- A `Condition` named "Free Shape with Processing" is shown.
- It contains two main blocks linked by an **OR** connection.
- The first block is a comparison: `Formula (Shape Number)` `== (equal)` `Value (99)`.
- The second block is another comparison: `Formula (Shape Number)` `== (equal)` `Value (98)`.
- This second block is linked via an **AND** connection to another condition: `Formula (Processing)` `Only Formula 1`.
- This demonstrates a complex condition: `(Shape Number == 99) OR (Shape Number == 98 AND Processing exists)`.

(Reference Fig. F-7 shows the GUI implementation of these linked elementary conditions.)

## Quantity
A quantity consists of the rule of how to form the final quantity from the start part (BOM). The following rules can be combined at random.
(See Software Reference, "Quantity editor" on page F-748)

An part can represent a processing step.

A schematic display of the quantity (Fig. F-9) shows a hierarchical part tree starting from an `IG` part, branching down based on a `Condition: Is TGH`, and leading to final `Float` parts through various implicit and explicit processing steps like Toughening, Arrissing, and Silk Screening.

For instance, the condition `Is TG` and quantity `Parent` results in all final and interim products produced from one or more toughened glass parts.

## Allocation
The simplest type is the allocation of an object property to a formula. The result of the formula is allocated to the object property.

**Example:**
- `SURCHARGETHICKNESS` = Formula 2mm
- `STACKINGWIDTH` = Height

# parts of the formula editor: Level II
The formula editor consists of the parts:
- "Formula" on page F-705
- "Comparison" on page F-706
- "Condition" on page F-706
- "Quantity" on page F-708
- "Allocation" on page F-708

## Formula
The formula now contains a quantity plus instructions. Without the quantity, the formula directly affects the object to be checked. When a quantity is defined, the object to be checked is converted into a quantity, the object being the start object of the quantity. The formula will be applied to each object of the final quantity; the results will be linked according to instructions. If the final quantity contains no objects, a long value -1 is returned.

**Examples:**
- `$THICKNESS` ; Number of all base parts; `SUM` → Total thickness
- `1`; quantity of all processings; `SUM` → Number of all processings

Valid operations are `Sum`, `Average`, `And-link`, `Or-link`, `minimum` and `maximum`.

(Reference Fig. F-10 Formula dialog showing operation options.)

## Comparison
Normally, a comparison consists of 1-2 formulas and the instruction. Alternatively, a comparison can be expressed by a condition (activate radio button `Conditions`). In this case, the comparison is fulfilled if the allocated condition is fulfilled. This type of linking conditions is used whenever two or more conditions are applied to different quantities.

(Reference Fig. F-11 Comparison dialog showing condition-based comparison.)

## Condition
A condition can be inverted. That means, it is fulfilled if the result of the comparisons is not fulfilled, and vice versa. This way, you can easily create from an existing condition the inverted one. The inverted condition contains just one comparison which will be allocated the original condition. Moreover, the characteristic `invert` will be selected for the inverted condition. The status line shows `INV` in front of the condition name.

The comparisons are usually analyzed for the object to be checked. If you want to check however whether one of the sub-parts of an object has a certain part type/processing type, you can allocate a quantity to the condition. In this case, the object is changed into a quantity, the object being the start object of the quantity. The condition will be analyzed for all parts of the final quantity. You only need to define when the condition is fulfilled. If it is sufficient that part of the final quantity fulfils the condition, select operation `One`. If the condition is only fulfilled if all parts of the final quantity fulfil the condition, select operation `All`. If the final quantity contains no objects, the condition is not fulfilled.

**Examples:**
- Formula `Part type = value 125`; quantity `All sub-parts`; `One`
- With processing type =125
- Formula `P_IG Only formula 1`, quantity `Header part`; `One` (or `All`)
  - The header part is IG

(Reference Fig. F-12 Condition dialog showing a condition with an associated quantity.)

## Quantity
The quantity definition contains a condition. All objects which does not fulfil the condition, will be removed from the final quantity.

**Example:**
- `; Anychild ; condition Processing;`
  -> The final quantity contains only the processings below the start part.

If a condition is used, the two instructions `Up` and `Addup` can be used. These must not be combined with other instructions.

- **Up**: means that the final quantity consists of one part only. Starting from the start part, all upper parts of the start part will be checked whether they fulfil the condition. The final quantity contains the last part fulfilling the condition. Should one part fail to fulfill the condition, the upwards iteration will be aborted.
- **Addup**: means that the final quantity can consist of more than one part. Like with `Up`, there is an upward iteration from the start part which will be stopped should one part fail to fulfil the condition. The final quantity, however, contains all parts fulfilling the condition.

**Examples:**
- `; Up; condition No processing`
- `; Addup; condition Not ordered`

## Allocation
The allocation can include a quantity. In this case, the result of the formula of the property will be allocated to all objects of the final quantity.

**Example:**
- `SURCHARGETHICKNESS` = Formula 2mm ; Quantity `Alle cut parts`

# Elements of the formula editor: Step III

## Quantity
Quantity definition will always be loaded with a start quantity. In simple cases, the start quantity consists of just one element, namely the start part. The `Quantity editor` allows to logically group several elements next to each other or below each other, like in the `Conditions editor`. The parts in the `Quantity` editor are different. The vertically grouped quantities form the combined quantity while the horizontally grouped quantities form the intersection.

Please note that there is a second window for the edition of quantities. You can switch between the first and second window via button `[+/-]`. The start quantity is found by removing from the quantity of the first(+) window all objects of the quantity of the second(-) window.

**Examples:**
- `{Quantity Upper part or Self; Anychild + Self; ; }`
  - 1st window (Plus): Quantity upper part or self
  - 2nd window (Minus): empty
  - `Anychild` and `Self` are tagged
- This produces an upper part, and all sub parts of the upper part. If there is no upper part, the final quantity includes the start element and all its sub part.
- The result is the final quantity with all parts sharing the upper part of the start part.

If the iteration for `Up` or `Addup` shall not start with the part itself, but with the upper part, first form the start quantity from the start part, using quantity upper part `{;Parent;;;}`, and use this with the required quantity, and the instruction `Up` or `Addup`.

This quantity can be allocated a formula. In this case, the formula will be analyzed for all elements of the start quantity; the results will be saved. From the final quantity, all parts will be removed the start quantity of which does not contain the result of the formula.

**Example:**
- `; All;; Formula Part type`
  - Produces all parts of the part tree which are of the same type as the start part.

# Notation Formula.dll

## Syntax

**ASSIGNMENT**
- Input: Object, UserSet
- `PROPERTY = FORMULA ; SET [/USERSET]`

**FORMULA**
- Input: Object, UserSet
- `[formulaelements ; SET ; OP [/USERSET]]`
- `OP ∈ {Sum, Average, And, Or, Minimum, Maximum}`
- `formulaelements = property, FORMULA ; + - * / () 0..9 @LEFT @RIGHT @MID`

**CONDITIONS**
- Input: Object, UserSet
- `conditionelements ; SET ; OP [/N] [/USERSET]`
- `OP ∈ {NULL, One, All}`
- `conditionelements = CONDITION(S) or (conditionelements OP conditionelements)`
- `OP ∈ {Und, Oder}`

**CONDITION (comparison)**
- Input: Object, UserSet
- `FORMULA [OP FORMULA] ; ;`
- `OP ∈ {=,!=,>,>=,<,<=}`

**SET**
- Input; Set, UserSet
- `{ (setelements)[-(setelements)] ; OP ; CONDITIONS ; FORMULA [/USERSET] }`
- Note: Part `-(setelements)` is used only if it is not 'empty'.
- `OP ∈ {All, Master, Parent, Self; Child, Anychild, Bottom, Up, Addup}`
- `setelements = 'empty' or SET or (setelements OP setelements)`
- `OP ∈ {n, U}`

## Function

### ASSIGNMENT
The UserSet is transferred to FORMULA and SET.
- **Without Set, without UserSet:** The FORMULA will be analyzed for this object. The result of the FORMULA is allocated to the object PROPERTY.
- **With Set:** SET is used to create a quantity from the given object. For every part of this quantity, the FORMULA will be analyzed; the result will be allocated to the PROPERTY of the corresponding object.
- **With UserSet:** For every object of the UserSet, the FORMULA will be analyzed; the result will be allocated to the PROPERTY of the corresponding object.
- **With Set, with UserSet:** Invalid, impossible.

### FORMULA
The UserSet is transferred to the SET and to all FORMULAs in formulaelements.
- **Without Set, without UserSet:** All formulaelements for the given object will be analyzed; the complete term will be calculated. The result is returned as MultiValue.
- **With Set:** SET is used to create a quantity from the given object. All formulaelements for every part of this quantity will be analyzed; the complete term will be calculated. The results will be analyzed as per Operation; the total result will be returned as MultiValue.
- **With UserSet:** All formulaelements for every part of the UserSet will be analyzed; the complete term will be calculated. The results will be analyzed as per Operation; the total result will be returned as MultiValue.
- **With Set, with UserSet:** Invalid, impossible

### CONDITIONS
The UserSet is transferred to SET and to all CONDITION(S)s in the conditionelements.
- **Without Set, without UserSet:** All conditionelements for the given object will be analyzed; the total result will be calculated and returned as BOOLEAN.
- **With Set, (with operation != NULL):** SET is used to create a quantity from the given object. All conditionelements for every element of this quantity will be analyzed; the complete BOOLEAN term will be calculated. If the Operation = `ONE`, CONDITIONS will return `TRUE` if for at least one element the complete BOOLEAN term is fulfilled, i.e. `TRUE`. If however the Operation = `ALL`, CONDITIONS will return `TRUE` if the complete BOOLEAN term is fulfilled, i.e. `TRUE` for all parts. Otherwise, `FALSE` will be returned.
- **With UserSet:** All conditionelements for every element of the UserSet will be analyzed; the complete BOOLEAN term will be calculated. If the Operation = `ONE`, CONDITIONS will return `TRUE` if for at least one element the complete BOOLEAN term is fulfilled, i.e. `TRUE`. If however the Operation = `ALL`, CONDITIONS will return `TRUE` if the complete BOOLEAN term is fulfilled, i.e. `TRUE` for all parts. Otherwise, `FALSE` will be returned.
- **With Set, with UserSet:** Invalid, impossible

### CONDITION
The UserSet is transferred to every FORMULA.
- **Random:** Both FORMULAS, if existing, will be analyzed for the given object. If there is only one FORMULA, `TRUE` will be returned if the result of FORMULA is not `ZERO` (numeric result), or if it is no empty string for string results. Otherwise, `FALSE` will be returned. If both FORMULAs do exist, the results will be compared acc. to the Operation. If the comparison is fulfilled, `TRUE` will be returned; otherwise, `FALSE`.

### SET
All SETS, CONDITIONS and FORMULA included in setelements will be transferred to the UserSet.
- **Without FORMULA, without UserSet:** All setelements for the given Set will be calculated; the preliminary quantity A will be determined. For every object of this quantity A, quantity BA will be determined as per Operation, to be added to quantity B. From quantity B, all objects will be removed which do not fulfil the CONDITIONS. As a result, quantity B is returned as RelatedSet.
- **With FORMULA, without UserSet:** Initially like A, but quantity B will not be returned. The FORMULA will be analyzed for every object from the given Set. The results will be saved in an array. Next, the FORMULA is analyzed for every object in quantity B. If the array includes the result of the FORMULA for an object from quantity B, the corresponding object will be added to quantity C. As a result, quantity C is returned as RelatedSet.
- **Without FORMULA, with UserSet:** Like A, but instead of the given Sets, the UserSet will be used to form quantity A.
- **With FORMULA, with UserSet:** Like B, but instead of the given Sets, the UserSet will be used to form quantity A. Still, the given Set will be used to form the array.

### Example
For sheet A and a certain number of sheets, you want to determine the total number of all sheets belonging to the same route as sheet A:
`[$QUANTITY; { ; ; ; [$TOUR] /USERSET } ; SUM }`

Sheet X shall be kept at the rack only if it is laminated glass, and if the total of all sheets includes at least 150 laminated sheets:
`'('[P_LAMI;;]==[1;;];;` AND `[$QUANTITY;{;;''[P_LAMI;]==[1;;]';;';/USERSET};SUM]`>=[150;;]`) ; ;`

### Check results
To check the results of the formulas, you can view the corresponding log file. To activate the result check for **Detailed scheduling**, the following setting must be made in A+W Production:
Master data > Parameters > Module Detailed scheduling > Specials > View-Formula > Enter value 1

> **Performance**
> Viewing the calculations will impair the performance!

The log file for the result check is found in:
`\<AlcimRootDir>\Log\(Name of log file of detailed scheduling).LOG`

(Reference Fig. F-14 Log file example)

# Conditions for Racks
Explains how to define, change, or delete conditions for racks in section Organization.

### This is how you define a condition for a rack, filtering all sheets with an edge length over 1.20 m
1. Open the Organization dialog via: Master data > Detailed scheduling > Organization
2. Open tab **Production sequence**
3. Tag the rack for which you want to define a condition
4. Press button [New condition]. The dialog **Select conditions --1--** appears
5. Press button [New condition ...]. This opens the dialog **Conditions editor**
6. In menu Conditions, open **Names**. This leads to dialog **Condition name**. Field **New name** shows *New condition* by default. Give the condition a characteristic name. Example: *Large sheet*. Close the dialog via button [OK]
7. In menu Conditions, open **Info**. This opens dialog **Info**. Enter a clear description of this condition. Example: *This condition is true if one edge of a sheet is longer than 1,20 m*. Close the dialog via button [OK]
8. In menu Part conditions, open **Add (column)**. A new element condition appears, and can be configured.
9. Open the combo box (by default set with *only formula 1*) and select **>= (equal or bigger)**
10. Activate the radio button **Value**. The dialog **Enter numerical value** automatically appears. Since the new rack shall only contain sheets over 1,20, activate the radio button **Length**, and enter in section **New value** 1200 mm. Close the dialog using [OK]. This value will appear in the bottom field of the condition
11. Click on the top input field of the condition. The dialog **Select formulas --1--** appears automatically. Define what the value entered in the second input field shall refer to.
12. Press button [New formula ...]. The dialog **Formula editor** appears. Enter a characteristic name for the formula in the top left field. Example: *Big size*.
13. In section **Existing properties**, double-click on **Big size**.
14. Close the dialog using [OK]. You will find yourself back in dialog **Condition editor**.
The defined condition looks like:
(Image shows a condition named 'Large Dimension' with operator '>=' and value '1200.0 mm')

Close the dialog via menu Conditions > OK, or by clicking on the checkmark icon.
You will find yourself back in dialog **Select conditions --1--**. You will find the defined condition **Large sheet** at the end of the list **Existing properties**.

### This is how to allocate a condition to a rack
1. Open the Organization dialog via: Master data > Detailed scheduling > Organization
2. Open tab **Production sequence**
3. Tag the rack the condition shall be allocated to
4. Press button [New condition]. The dialog **Select conditions --1--** appears
5. On the list of **Existing conditions**, tag the condition to be allocated to this rack
6. Close the dialog via button [OK]
7. The condition was added to the rack tagged in tab **Production sequence**

### How to delete a condition allocated to a rack
1. Open the Organization dialog via: Master data > Detailed scheduling > Organization
2. Open tab **Production sequence**
3. Double-click on the rack to open it
4. Tag the condition to be deleted
5. Click the [Delete] button. The condition will be deleted instantly

> **Delete**
> Deletion is not accompanied by a security check. If you have deleted something by mistake, leave the tab **Production sequence** via button [Abort]. The system will want to know whether the changes shall be ignored. Answer [OK]. The Organization dialog will be closed. Next time you open it, the data will still be there.

# Conditions for Organization Groups
Explains how to define, change, or delete conditions for organization groups in section Organization.

### How to define a condition for an organization group, filtering IG with Muntins for a second production section
1. Open the Organization dialog via: Master data > Detailed scheduling > Organization
2. Open tab **Production sequence**
3. Tag the rack for which you want to define an organization group
4. Press button [New condition]. The dialog **Select conditions --1--** appears
5. Press button [New condition]. This opens the dialog **Conditions editor**
6. In menu Conditions, open **Names**. This leads to dialog **Condition name**. Field **New name** shows *New condition* by default. Give the condition a characteristic name. In our example: *IG muntins*. Close the dialog via button [OK]
7. In menu Conditions, open **Info**. This opens dialog **Info**. Enter a clear description of this condition. In our example: *Item was allocated to production section 2 MZO_ROUTE_MAP.ROUTE =2*. Close the dialog via button [OK]
8. In menu Partial Conditions, open **Add (column)**. A new element condition appears, and can be configured.
9. Open the combo box (by default showing *only formula 1*) and select **== (equal)**
10. Activate the radio button **Value**. The dialog **Enter numerical value** automatically appears. Since IG with muntins is only produced in production section 2, activate the radio button **Digit** and enter in section **New value** 2. Close the dialog using [OK]. This value will appear in the bottom field of the condition.
11. Click on the top input field of the condition. The dialog **Select formulas --1--** appears automatically. Define what the value entered in the second input field shall refer to.
12. Press button [New formula ...]. The dialog **Formula editor** appears. Enter a characteristic name for the formula in the top left field. In our example: *Production section*.
13. In section **Existing properties** double-click on **Route**. Section **Formula** shows `$Route`.
14. Close the dialog using [OK]. You will find yourself back in dialog **Condition editor**.
The defined condition looks like:
(Image shows a condition named 'Production Step' with operator '==' and value '2')
15. Tag the condition and press [Ok]. The condition will be added to the previously tagged organization group.

### How to allocate an existing property to an organization group
1. Open the Organization dialog via: Master data > Detailed scheduling > Organization
2. Open tab **Production sequence**
3. Tag the organization group to define a condition
4. Press button [New condition]. The dialog **Select conditions --1--** appears
5. On the list of **Existing conditions**, tag the condition to be allocated to this organization group
6. Close the dialog via button [OK]
7. The condition was added to the organization group tagged in tab **Production sequence**

### How to delete a condition allocated to an organization group
1. Open the Organization dialog via: Master data > Detailed scheduling > Organization
2. Open tab **Production sequence**
3. Double-click on the organization group to open it
4. Tag the condition to be deleted
5. Click the [Delete] button. The condition will be deleted instantly

> **Delete**
> Deletion is not accompanied by a security check. If you have deleted something by mistake, leave the tab **Production sequence** via button [Abort]. The system will want to know whether the changes shall be ignored. Answer [OK]. The Organization dialog will be closed. Next time you open it, the data will still be there.

# Group Formation Mode
This example serves to add another selectable mode for group formation for organization groups and racks.

### This is how you create a grouping by number of sheets per customer
i.e. a group will be created per customer and this group will be sorted by the number of sheets included. The group with the largest number of sheets will be produced first.

1. Open the Grouping/Sorting dialog via: Master data > Detailed scheduling > Group editor
2. Press button [Formulas...]. Dialog **Select formulas --1--** appears
3. Press button [New formula ...]. The dialog **Formula editor** appears
4. Enter the name for the grouping formula in the top left field. In our example, *Number of sheets per customer*
5. In section **Existing properties**, double-click on **Quantity**. Section **Formula** shows `$MENGE`
6. Click the [Quantity ...] button. The dialog **Select quantity --1--** appears
7. Use button [New quantity ...] to define a new quantity. This opens dialog **Quantity - Editor**.
8. In menu Quantity, open **Names** and enter a new, characteristic name for the quantity. In our example, *Number of sheets per customer*. Close the dialog via button [OK]
9. In menu Quantity, open **Transferred quantity**. As a result, not only the item used to start the quantity editor will be considered for quantity calculation, but also all items of the job
10. As the required quantity shall not include all parts, but only the released parts, activate in dialog **Quantity editor** the checkbox **Master**.
11. To add the customer number as a property to the quantity, select in menu **Quantity, Formula**. The dialog **Select formulas --2--** appears. Use button [New formula ...] to enter the formula for the customer number. The dialog **Formula editor** appears.
12. Enter the formula name in the top left input field. In our example, *Customer number*
13. In section **Existing properties**, double-click on **Customer number**. Section **Formula** shows `$Customer number`.
14. Click the [OK] button. You will return to dialog **Select formulas --2--**. The last entry on the list will be the just defined formula for the customer number. Tag the **Customer number** on the list, and press [OK]. This brings you back to dialog **Quantity editor**.
15. The right side of the status line of the quantity editor shows whether - and if so, which - formula is used to define the new quantity. In our example, `Formula: Customer number`
16. Tag all open dialogs via [Ok] until you reach dialog **Grouping/Sorting**
17. The list of formulas now includes the formula *number of sheets per customer*. Tag the formula and press [Add]. The formula will be added to the groupings in tab **Group editor**. It will be available in the settings for the Organization groups and the Racks, in section **Group formation**.

# Conditions for Production Sections
This tells you how to define, change, or delete conditions for production sections in section Machine allocation.

### How to define a condition for a production section, filtering all sheets with muntins
1. Open dialog **Production sections** via: Master data > Machine allocation > Configuration
2. Tag the production section for which you want to define a condition
3. Use the right mouse key. The context menu appears. From the context menu, select: **Condition for production section > New**
4. The dialog **Select conditions --1--** appears
5. Press button [New condition]. This opens the dialog **Conditions editor**
6. In menu Conditions, open **Names**. This leads to dialog **Condition name**. Field **New name** shows *New condition* by default. Give the condition a characteristic name. In our example: *Muntin IG*. Close the dialog via button [OK]
7. In menu Conditions, open **Info**. This opens dialog **Info**. Enter a clear description of this condition. Example: *This condition is true if the item shows a muntin flag*. Close the dialog via button [OK]
8. In menu Part conditions, open **Add (column)**. A new part condition appears, and can be configured.
9. The combo box shows **Only Formula 1** by default. In our example, this remains unchanged.
10. The radio button **Normal** is active by default. The dialog **Enter numerical value** automatically appears. In our example, this remains unchanged, too.
11. Click on the top input field of the condition. The dialog **Select formulas --1--** appears automatically.
12. Press button [New formula ...]. The dialog **Formula editor** appears. Enter a characteristic name for the formula in the top left field. In our example: *Muntins*
13. In section **Existing properties** double-click on **Itm_Muntin_Flag**. Section **Formula** shows `$Itm_Muntins_Flag`
14. Close the dialog using [OK]. This brings you to dialog **Select formulas --1--**. The just defined formula is tagged already.
15. Close the dialog using [OK]. You will find yourself back in dialog **Condition editor**.
The defined condition looks like:
(Image shows a condition named 'Grills' with the operator 'Only Formula 1')

Close the dialog via menu **Conditions > OK**, or by clicking on the checkmark icon. You will find the defined condition **Muntins - IG** at the end of the list **Existing properties** in the **Select conditions --1--** dialog.

### This is how to allocate a condition to a production section
1. Open dialog **Production section** via: Master data > Machine allocation > Configuration
2. Tag the production section the condition shall be allocated to
3. Use the right mouse key. The context menu appears. From the context menu, select: **Condition for production section > New**
4. The dialog **Select conditions --1--** appears
5. On the list of **Existing conditions**, tag the condition to be allocated to this production section
6. Close the dialog via button [OK]
7. The condition was added to the tagged production section.

### How to delete a condition allocated to a production section
1. Open dialog **Production section** via: Master data > Machine allocation > Configuration
2. Double-click on the production section to open it
3. Tag the condition of the production section to be deleted
4. Use the right mouse key. The context menu appears. From the context menu, select **Delete condition**. The condition will be deleted instantly!

> **Delete**
> Deletion is not accompanied by a security check. If you have deleted something by mistake, leave the dialog **Production sections** via button [Abort]. Next time you open it, the data will still be there.

# More Examples

### How to define a condition for TG within IG, or float glass processing
1. **First step:**
   - In formula `TG`, the property `P_TG` is returned.
   (Image shows a condition for 'Toughened Glass' using 'Only Formula 1')

2. **Now check whether the element is part of IG:**
   - This involves a complex quantity operation:
     - **Elementary Condition:** Define a condition for `Part Type TGH`.
     - **General Quantity Description:** Define a quantity for `All direct Childs of Parents`.
     - **Composite Start Quantity:** The operation begins with the start quantity, searches child parts of all parents.
     - **Minus or Reduction Size:** Subtracts `Myself`. The final quantity is the remaining mates.

3. **As a part cannot be TG and IG at the same time, the condition shown in step 2 cannot work. Hence ...**
   - A condition is created with an `OR` connection. One part checks if the part is `TGH`, the other checks if `Parent is IG`.
   (Image shows two conditions side-by-side: `TGH` (Only Formula 1) and `Parent is IG` (Parent, ONE))

4. **Check the Or connection, whether one of the sub parts is a processing step.**
   - Another condition will be created, checking the formula `Processing` for all sub parts.
   (Fig. F-16 shows three conditions stacked vertically, implying an `OR` link: `TGH`, `Parent is IG`, and `Processings below me`)

### The processing steps directly below
1. The final quantity shall contain only the processing steps below the start part which will be made after the last processing steps defined.
2. The system first unites all sub parts which are no processings.
3. Quantity **Defined processing steps below** = `{ ; ANYCHILD ; condition is No processing; }`
4. This quantity is used to define the number of parts and processing steps below the start part you do not require.
5. Quantity **Unwanted parts/processing steps below** = `{ number of defined processing steps below ; ANYCHILD+SELF ; ; }`
6. The required quantity is determined by the number of **All sub parts** and the number of **unwanted parts/processing steps below**.
   - `{Number of all sub parts - number of unwanted parts/processings below ; SELF ; ; }`

# List of Dialogs
This list shows all dialogs you need to use the formula editor properly. The references lead to chapter Software Reference in the base data section. It provides detailed information on the dialogs, fields and buttons.

### Master Data Menu
The formula editor cannot be reached by means of a menu entry. The individual dialogs will tell you how to access it.

| Dialog/Function | Page Reference |
| :--- | :--- |
| "Select conditions" | F-734 |
| "Condition editor" | F-736 |
| "Condition" | F-739 |
| "Condition name" | F-741 |
| "Info" | F-754 |
| "Select formulas I" | F-755 |
| "Formula editor" | F-757 |
| "Select allocation" | F-760 |
| "Allocation editor" | F-760 |

---

# Software Reference

This section provides information on the following subjects related to the Formula Editor.

- Formula Editor (F-733)
- Select conditions (F-734)
- Condition editor (F-736)
- Condition (F-739)
- Condition name (F-741)
- Info (F-742)
- Invert (F-742)
- Transferred quantity (F-743)
- Enter value (numeric) (F-744)
- Select quantities (F-746)
- Quantity editor (F-748)
- Quantity name (F-752)
- Info (F-754)
- Select formulas I (F-755)
- Formula editor (F-757)
- Select allocation (F-760)
- Allocation editor (F-760)

## Formula Editor
The Formula Editor is used in the following areas of A+W Production:
- Organization
- Machinery allocation
- Labels, sketches, bender text

Instructions on how to open individual dialogs are provided again in the following dialog descriptions.

## Select conditions

### Load via
- **Organization**
  - Master data > Detailed scheduling > Organization > tab: Production sequence > Tag organization group > [New condition]
  - Master data > Detailed scheduling > Organization > tab: Production sequence > Tag rack > [New condition]
- **Machinery allocation**
  - Master data > Machinery allocation > Configuration > Tag production section > Right mouse key > Condition for the production section > New
  - Master data > Machinery allocation > Configuration > Tag condition of production section > Right mouse key > Edit condition
  - Master data > Machinery allocation > Configuration > [Technology] > [New] > [New]
  - Master data > Machinery allocation > Configuration > [Technology] > [Change] > [New]/[Edit]
- **Labels, sketches, bender text**
  - Master data > Labels / Sketches / Bender text > Configuration ... > Tag condition > [Formula editor]

### Description of fields
- **Existing conditions**: The table lists all conditions existing in the system for the sections Organization, Machinery allocation and Labels, sketches, bender text. The contents differ from section to section!
- **No condition**: If this checkbox is active, the dialog shows as a result that Nothing was selected.
- **Description**: The field contains a detailed description of the condition. This is the text entered in field Info.

### Description of buttons
- **Delete**: Use this button to delete the tagged condition. Deletion will be made without a security check.
- **New condition**: Press this button to open dialog **Condition editor**. You can define a new condition.
- **Edit**: Press this button to open dialog **Condition editor** for the tagged condition.

## Condition editor

### Load via
- **Organization**: Master data > Detailed scheduling > Organization > tab: Production sequence > Tag organization group > [New condition] > [New condition ...] / [Edit]
- **Machinery allocation**: Master data > Machinery allocation > Configuration > Tag production section > Right mouse key > Condition for the production section > New > [New condition...] / [Edit]
- **Labels, sketches, bender text**: Master Data > Labels / Sketches / Bender texts > Configuration ... > Tag Condition > [Formula Editor] > [New condition ...] / [Edit]

### Menus and Functions

| Menu entry | Dialog/Function |
| :--- | :--- |
| **Menu Conditions:** | |
| Name | "Condition name" on page F-741 |
| Info | "Info" on page F-742 |
| Quantity | "Select quantities" on page F-746 |
| Invert | "Invert" on page F-742 |
| Transferred quantity | "Transferred quantity" on page F-743 |
| OK | The defined condition will be saved, and the editor is closed. |
| Cancel | The defined condition will be rejected, and the editor is closed. |
| **Menu Part conditions:** | |
| Add (column) | Opens a window to define a condition (And connection). |
| Add (line) | Opens a window to define a condition (Or connection). |
| Remove | Deletes the selected condition. |

### Tool bar

| Tool | Explanation |
| :--- | :--- |
| ✅ | The defined condition will be saved, and the editor is closed. |
| ❌ | The defined condition will be rejected, and the editor is closed. |
| `++` | Opens the window to define the condition. Double-click to open two windows next to another; these represent an **And** connection. |
| `‡` | Opens the window to define the condition. Double-click to open two windows, one below the other; these represent an **Or** connection. |
| `-` | Deletes the selected condition. |

### Description of radio buttons
- **All**: Considers the conditions for all elements of a BOM. With this setting, a lite without pattern - for instance - will be allocated to a rack with the condition "pattern" if the counterpane is patterned. Only the characteristics of the lite in question will be considered.
- **Zero**: The quantity allocated to the condition will not be taken into account.

## Condition (Dialog)

### Load via
- **Organization**: Master data > Detailed scheduling > Organization > ... > Menu Part conditions > Add...
- **Machinery allocation**: Master data > Machinery allocation > Configuration > ... > Menu Part condition > Add ...
- **Labels, sketches, bender text**: Master Data > Labels / Sketches / Bender texts > ... > Menu Part conditions > Add ...

### Fields
- **Top input field**: Click on the field to open the dialog **Select formulas I**. You can select an existing formula, or enter a new one.
- **Central selection field**: Open the combo box and select the operator. Possible values:
  - Only Formula 1
  - `==` equal
  - `!=` unequal
  - `<` less than
  - `<=` smaller or equal
  - `>` greater than
  - `>=` greater or equal
- **Bottom input field**: Click on the field to open either **Select formulas I**, **Enter value (numeric)** or **Select conditions**. The active radio button (`Normal`, `Value`, `Conditions`) defines which dialog is going to be opened.
  - **Normal**: Activate the radio button, then click on the bottom input field to open the dialog **Select formulas I**.
  - **Value**: Activate this radio button to open dialog **Enter value (numeric)**.
  - **Conditions**: Activate the radio button, then click on the bottom input field to open dialog **Selection Conditions --2 --**.

## Condition name

### Load via
- **Organization**: ... > Menu conditions > Name
- **Machinery allocation**: ... > Menu conditions > Name
- **Labels, sketches, bender text**: ... > Menu conditions > Name

### Description of fields
- **Old name**: If a condition was given no name so far, this field will read *New condition* by default.
- **New name**: Enter the name of the condition. This can be overridden at any time. The defined name appears in the status line of **Condition editor**.

## Info
You can describe the condition. The text will appear in dialog **Select conditions** in section **Description**.

## Invert
A condition can be inverted. It is fulfilled if the result of the comparisons is not fulfilled, and vice versa. The status line shows `INV` in front of the condition name. This menu can be enabled or disabled as required.

## Transferred quantity
This menu can be enabled or disabled as required. If it is active, the system will not only consider the item by which the dialog **Condition editor** was opened, but also all items of the job when determining the quantities.

## Enter value (numeric)

### Load via
Accessed by activating the radio button [value] in a new partial condition.

### Description of fields
- **Old value**: If a condition was given no value so far, this field will read 0 by default.
- **New value**: Enter the value for the condition. This can be overridden at any time.

### Description of radio buttons
- **Digit**: If the condition refers to a quantity for instance, activate this radio button.
- **Thickness**: If this condition refers to Thickness, enter the value in mm.
- **Text**: If this condition refers to Text.
- **Length**: If the condition refers to a length.
- **AIR**: If the condition refers to an airspace.

## Select quantities
This dialog allows to select, or change existing quantities for the sections Organization, Machinery allocation and Labels, sketches, bender text, or to define new conditions.

### Description of fields
- **Existing quantities**: The table lists all quantities existing in the system.
- **No quantity**: If this checkbox is active, the dialog shows as a result that *Nothing* was selected.
- **Description**: The field contains a detailed description of the quantity.

### Description of buttons
- **Delete**: Deletes the tagged quantity.
- **New quantity**: Opens the **Quantity editor** to define a new quantity.
- **Edit**: Opens the **Quantity editor** for the tagged quantity.

## Quantity editor
Allows to change a tagged quantity, or to define a new quantity.

### Menus and Functions

| Menu entry | Dialog/Function |
| :--- | :--- |
| **Menu Quantity:** | |
| Name | "Quantity name" on page F-752 |
| Info | "Info" on page F-754 |
| Condition | "Select conditions" on page F-734 |
| Formula | "Select formulas I" on page F-755 |
| **Menu Partial quantities:** | |
| Add (column) / Add (line) | Adds a new partial quantity. |
| Remove / Change | Modifies the selected partial quantity. |

### Tool bar

| Tool | Explanation |
| :--- | :--- |
| ✅ / ❌ | Save / Reject changes. |
| `++` / `‡` | Open window to define quantity (And / Or connection). |
| `-` | Deletes the selected quantity. |
| `+/-` | Switches between the first and the second window. |

### Description of check boxes
- **All**: All parts of the part tree containing the start part.
- **Master**: The top part of the part tree (head part) containing the start part.
- **Parent**: Part right above the start part in the part tree.
- **Self**: Start part.
- **Child**: All direct sub parts of the start part.
- **Anychild**: All sub part of the start part, even the indirect ones.
- **Bottom**: All basic parts below the start part.
- **Up (SI)**: The final quantity consists of one part only. It performs an upward iteration from the start part, checking a condition. The iteration stops if a part fails the condition.
- **Addup**: The final quantity can consist of more than one part. Similar to Up, it performs an upward iteration but includes all parts that fulfilled the condition before the iteration stopped.

## Quantity name
Give a characteristic name to the quantity. The name will be shown in the status line of dialog **Quantity editor**.

### Fields
- **Old name**: If no name was given, this field reads *New quantity*.
- **New name**: Enter the name of the quantity.

## Info (on quantity)
You can describe the quantity. The text will appear in dialog **Select quantities** in section **Description**.

## Select formulas I
This dialog allows to select, or change existing formulas or to define new formulas.

### Fields
- **Existing formulas**: Lists all formulas in the system.
- **No formula**: If checked, nothing is selected.
- **Description**: Detailed description of the selected formula.

### Buttons
- **Delete**: Deletes the tagged formula.
- **New formula**: Opens the **Formula editor** to define a new formula.
- **Edit**: Opens the **Formula editor** for the tagged formula.

## Formula editor
This dialog allows to define new formulas.

### Fields
- **Top input field**: Enter a characteristic name for the formula.
- **Description**: Enter a detailed description of the formula.
- **Formula**: Enter the database field required for the formula by selecting from **Existing properties**.
- **Quantity**: Press to open dialog **Select quantities**.
- **Transferred quantity**: If this checkbox is active, the system will consider all items of the batch for the quantity creation.

### Radio buttons in section Operation
These are active only if a quantity was allocated to the formula. The results of the formula applied to all parts of the quantity will be processed as follows:
- **Total (value)**: Total results
- **Average**: Total/number of results
- **And connection**: Results linked by a logical And.
- **Or operation**: Results linked by a logical Or.
- **Minimum**: Smallest result
- **Maximum**: Biggest result
- **Number of results**: Number of different results

> **And/Or operations**
> And/Or operations make sense only if the result of the formulas is 0 or 1!

### Existing properties
> Object properties within the organization are firmly linked for reasons for performance, and cannot be extended without program amendments. Object properties in connection with machinery allocation and labels can be flexibly extended via script DBInit.

## Select allocation
This dialog allows to select or change allocations only for section Organization.

### Fields and Buttons
- **Existing allocations**: Lists all existing allocations.
- **No allocation**: If checked, nothing is selected.
- **Description**: Detailed description of the allocation.
- **Delete**: Deletes the tagged allocation.
- **New allocation**: Opens the **Allocation editor**.
- **Edit**: Opens the **Allocation editor** for the tagged allocation.

## Allocation editor
Use this dialog to define a new allocation. The simplest type is the allocation of an object property to a formula. The allocation can also include a quantity.

### Fields
- **Top input field**: Give the allocation a characteristic name.
- **Property**: Select the required database field to be changed.
- **Formula**: Press this button to open **Select formulas I**.
- **Quantity**: Press this button to open **Select quantities**.
- **Transferred quantity**: Checkbox to consider all items of the batch for quantity creation.

> **Existing properties**
> Object properties for detailed scheduling are firmly linked for reasons for performance, and cannot be extended without program amendments.

**Important allocations:**
- **Stack width**: Will be used for rack loads. Normally, this property represents the lite width.
- **Assessment**: 100 by default. In connection with optimization, this serves to distribute lites to several stockplates.
- **Difference in thickness**: Defines to what extent the glass thickness may change when lites are added.
- **Group number**: 0 by default. If used to create production groups, this property must be allocated an appropriate formula first.
- **Box**: Freely disposable.
- **Surcharge thickness**: 0 mm by default. Can be used to define that when stacking lites, the system will consider lites thicker than determined by the glass thickness (e.g., for silk-screened lites).

---

# Tutorial: A+W Production Machinery Allocation

## Revision overview of the module

| Date | Changes |
| :--- | :--- |
| 11-2018 | New chapter regarding Machine type. Screenshots updated. |
| 01-2017 | Product and company names adjusted. |
| 01-2013 | Complete revision of ALCIM documentation and adjustment to A+W Production. |
| 09-2012 | Creation of tutorial, revision of software reference. |
| 01-2003 | Original version. |

This module provides information on:
- Tutorial
- Software Reference

## Overview
The tutorial on the Machinery Allocation (MA) module deals with the allocation of machines in AWP. Machinery allocation assigns the scheduled processing steps to the individual machines, taking into account machine restrictions and instructions for production control.

> **The functions depend on the released modules**
> Please note that the individual functions are available only if the corresponding modules and interfaces have been installed and released. If you detect functions in this description which are not available in your version, please contact A+W Software GmbH.

### Prerequisite knowledge
This tutorial is meant for persons in charge of production scheduling in A+W Production who are responsible for organizing the optimum production process. Participants must be familiar with the master data concept in A+W Production.

### Tutorial Structure
Each session consists of the following elements:
- **Overview**: Objectives, Benefit, Maxims.
- **Concepts**: Concepts and terms explained with examples.
- **Exercises**: Special tasks for some training sessions.

### Reading instructions
The contents of a training session are based on the knowledge conveyed in the previous session. We therefore recommend not to skip any session.

## Basics
The machinery allocation depicts the references between work processes and machine. Based on the machines and the work processes, the capacity planning can schedule the orders optimally.

To set up the master data, the following questions must be answered:
- What task must be performed? (**What**)
- What method will be used? (**How**)
- What tool will be used? (**Where**)
- Which ranking and restrictions have to be adhered to? (**Why** or **when**)

(Reference Fig. G-1 shows the interconnected elements of machinery allocation: Machine, Machine type, Properties, Formulas, Restrictions, Logical machine, Work process, Processing type, Processing article, all leading to 'Allocation of work'.)

### Description of the work processes
Using work processes, the material streams in production are divided up. For setup, consider:
- Which processings can/cannot be combined?
- Are there processings performed but not in the BOM?
- Are there different material streams (e.g., series sheets, bathroom mirrors)?
- Are there work processes not performed here (e.g., sand blasting elsewhere)?

### Description of the machines
Precisely described machines guarantee that sheets find valid machines. A distinction is made between physical restrictions and logical machines (with additional restrictions, cost rates, transition times). The list can also include non-machine locations relevant to production (warehouse, loading ramp, etc.).

### Description of the logical machine
Logical machines are used to express different transition times, cost rates, or processing durations in capacity planning. A logical machine can be set up if a physical machine can be used in different operating modes.

# Machine Allocation

This chapter tells you which sections of A+W Production are part of machinery allocation (MA) and how to allocate the machines.

Machinery allocation includes the following chapters:
- "Machines"
- "Logical Machines"
- "Work Processes"
- "Allocation of Work Processes"
- "Conditions, Formulas, Restrictions"
- "Processing Types and Processing Articles"

## Machines

### Objectives
- Understand the meaning of machines in A+W Production.
- Learn how to manage, define, edit, or delete machines.
- Use meaningful names and numbers.

### Benefit
- Machines represent the physical machinery and are the basis for production control.

### Note
- **Machines**: Represent physical machinery with systematic names and numbers.
- **Machine types**: Pre-defined in A+W Production (e.g., cutting, spacer bender), allocated to machines to define their type.
- **Relations**: AND-/OR relations link restrictions, conditions, and formulas.
- **Cuts**: Z- and W-cuts can be allocated an additional cost factor.

> **Prerequisite**
> To define a machine, the suitable machine type must be defined first. If the corresponding machine type is not available in the **New machine** dialog, please contact A+W Software GmbH.

### Machines and Machine Allocation
This session shows how to reflect your machinery and its properties in A+W Production.

The **Machines** tab in the Machinery Allocation Editor lists all physical machines, reflecting your actual machinery. Each machine has a unique ID, a registration point for production data collection (PDC), and an assigned machine type (e.g., Cutting, CNC Center). Machine types are permanently defined. A+W Production automatically creates a logical machine for every physical machine.

(Reference Fig. G-2, MA editor - Machines tab)

### Machine properties
For each machine created, the following properties must be specified:
- **Manual operation**: Identifier for machines without automatic loading. Prevents split scheduling on manual tables.
- **Individual processing**: Identifier for machines whose processings may not be combined (e.g., two drillings on the same machine do not get two separate dates).
- **Minimum/Maximum size**: Dimensions for a sheet that can be processed.
- **Thicknesses**: Thickness range the machine can handle.
- **Shapes**: Whether the machine can produce rectangles, shapes, or both.
- **Weight**: Maximum weight of a sheet the machine is approved for.

> **Delete machine**
> Deleting a machine can affect your production! Before you delete a machine, always make sure that it is no longer used on the shop floor.

### Assigning names, IDs, and numbers
Assign IDs in the same range of hundreds for machines of the same type (e.g., cutting tables 100-199). Use consistent naming conventions (e.g., Cutting table 1, Cutting table 2, etc.).

### Machine restrictions
Machines can have different restrictions edited in the **Machine** dialog.
- **Minimum/Maximum thickness**: e.g., if a machine processes lites from 8 mm up to 15 mm.
- **Shapes**:
  - *No restriction*: Processes shapes and rectangles.
  - *Only shapes*: e.g., a CNC center for grinding.
  - *Only rectangles*: e.g., a grinding/drilling line.
- **Coated glass**: Can process coated, uncoated, or both.
- **Patterned glass**: Can process patterned, non-patterned, or both.
- **Stepped IG**: Can process stepped IG, common IG, or both.
- **Dimensions**: Min/Max width and height.
- **AIR**: Airspace restrictions.

### Size restrictions and lite format
You can define min/max size of lites. Use the machine's direction of movement as a guideline. The sheet can be aligned by hand if width and height are exchanged.

### Spacer restrictions
Defines whether a machine can process common IG (one spacer) or multiple IG (two spacers). Min/Max values can be set for each spacer.

### AND-/OR relations
- **AND relation**: True if all statements apply (e.g., Width >= 150 mm AND height >= 200 mm).
- **OR relation**: True if at least one statement applies (e.g., Width >= 150 mm OR length <= 3500 mm).

### Element ID
Used for machine types **Line**, **Cutting**, and **Bender** to distinguish between multiple machines of the same type (e.g., TB1, TB2, TB3). It also defines the format for the NC code.

### Additional conditions
These can seriously influence machine behavior and must be understood before defining.

## Machine Definition and Management
This session shows how to define, edit, or delete machines.

> **Prerequisite**
> A new machine can only be entered if a suitable machine type has been defined (e.g., Cutting, CNC center). The catalog is predefined.

### How to define a machine
1. Go to **Master data > MA > MA editor > Machines > [New]**.
2. Enter an **ID** from the appropriate number range (e.g., 180 for a cutting table).
3. Enter a descriptive **Name** (e.g., Cutting table 8).
4. Choose the **Machine Type** (e.g., Cutting).
5. Enter an **Element ID** for Line, Table, or Bender types (e.g., TB8).
6. Click [OK] to save.

### How to enter the machine's properties
1. Go to **Master data > MA > MA editor > Machines**.
2. Select the machine to edit.
3. Click on [Edit].
4. Add the **General properties**. When you click a field, you can select data from the combo box.
5. Confirm by [OK]. (Machine restrictions can be completed later).

### How to delete a machine
> **Delete machines**
> Deleting machines can affect your production. Always make sure the machine is no longer in use before deleting.
1. Go to **Master data > MA > MA editor > Machines**.
2. Tag the machine you want to delete.
3. Click on [Delete].
4. Confirm the security query by [Yes].

## Definition and Editing of Machine Restrictions
This unit covers specifying restrictions for a machine.

> **Restrictions and additional condition at the same time**
> Active restrictions combined with a formula selection can cause a conflict. Restrictions can neutralize each other. Contact A+W Support if you have questions.

### How to edit restrictions regarding the thickness
1. Go to **Master data > MA > MA editor > Machines**.
2. Select the machine and click [Edit].
3. In the **Restrictions** section of the **Machine** dialog, double-click the `[...]` button next to the thickness field.
4. Activate the restriction by checking the box.
5. Click the arrow to open the input field.
6. Enter the minimum/maximum thickness in millimeters.
7. Click [OK] to save.

### How to edit the restrictions for shapes, coated glass, patterned glass, and stepped IG
1. Go to **Master data > MA > MA editor > Machines**, select the machine, and click [Edit].
2. In the **Restrictions** section, double-click the `[...]` button next to **Shapes**. An arrow appears.
3. Click the arrow to activate the checkboxes.
4. Choose the required combination:
   - **No restriction**: The main `Shapes` box is checked but the inner box is not. Machine processes rectangles and shapes.
   - **No shapes**: Both main and inner `Shapes` boxes are checked. Machine can only process rectangles.
   - **No rectangles**: Main box is checked, inner box shows `Shapes` with a cross. Machine can only process shapes.
5. Click [OK] to save.
6. Edit restrictions for coated glass, patterned glass, and stepped IG in the same way.

### How to edit the restrictions for sizes and spacers
1. Go to **Master data > MA > MA editor > Machines**, select the machine, and click [Edit].
2. Click the [Pen icon] in the **Dimensions** field to open the **Size restrictions** dialog.
3. Check the boxes for the input fields you want to edit (Min. Width, Min. Height, etc.).
4. Fill in the values.
5. Click [OK] to save. The restriction is shown as an AND/OR relation string.
6. Edit spacer restrictions similarly.

### How to remove the size and spacer restrictions
> **Deletion of size restrictions**
> Dimension restrictions are deleted permanently and without a security query if you click the [cross].
1. Go to the **Machine** dialog.
2. Click the [X] icon in the **Dimensions** area to remove a restriction.
3. Click [OK] to save the changes.
4. Delete spacer restrictions in the same way.

## Machines Exercises
- Sketch your factory's machinery.
- Note which machines belong to which machine type and assign IDs.
- Note properties and restrictions (e.g., thickness, size, IG/triple IG capabilities).
- Enter these machines as exercise machines in A+W Production.
- Keep these test machines for further exercises.

## Logical Machines

### Objectives
- Understand the meaning and purpose of logical machines.
- Learn to manage, define, edit, and delete them.

### Benefit
- Logical machines represent one machine function. If a machine can drill and edge, two logical machines will be created. Processes can then be allocated to specific functions.
- Barcoding (PDC) analyzes data from logical machines for statistics.

### Note
- A logical machine represents a function of a real machine.
- They are used for production control, cost calculation, and PDC.
- When you enter a physical machine, one logical machine is created automatically.
- Any number of logical machines can be defined for one physical machine.
- Logical machines are allocated to processes.

### Machines and Machine Allocation
Logical machines represent one function of a real machine. The properties of the physical machine are applied to the logical machine, and the properties of the logical machine are valid in addition to those.

(Reference Fig. G-4, Logical machines tab in MA editor)

Logical machines are used for:
- Describing individual machine functions.
- Allocating processes.
- Prioritizing processes.
- Capacity planning and rescheduling.
- Distinguishing machine functions to define different rates or transition times.
- Statistical evaluations.

### Example
You have a CNC machine that can drill, grind, and polish.
1. Define the physical machine `CNC machine 1`. A+W Production automatically creates one logical machine.
2. Manually define two more logical machines based on the first one.
3. Configure one for **Drilling**, one for **Grinding**, and one for **Polishing**.
This results in three logical machines from one physical CNC center.

(Reference Fig. G-5 diagram)

## Definition and Management of Logical Machines

> **Prerequisite**
> You can define logical machines only after entering the corresponding physical machine.

### How to define a logical machine
A+W Production automatically creates a logical machine for every physical machine. Additional logical machines are based on the existing one.
1. Go to **Master data > MA > MA editor > Logical machines**.
2. Select the logical machine to be used as a basis.
3. Click on [New].
4. Enter the new **ID** and **Name**.
5. Click [OK] to save. The new logical machine will be listed.

### How to edit a logical machine
1. Go to **Master data > MA > MA editor > Logical machines**.
2. Select the logical machine and click on [Edit].
3. Enter the data for the logical machine (e.g., for a cutting table).
4. Click [OK] to save.

### How to delete a logical machine
> **Delete logical machines**
> The automatically created logical machine cannot be deleted. When a physical machine is deleted, all its related logical machines are deleted too. Deleting a logical machine deletes a machine function, which can cause significant problems. Ensure it is not in use before deleting.
1. Go to **Master data > MA > MA editor > Logical machines**.
2. Select the logical machine to delete.
3. Click on [Delete].
4. Confirm the security query by [Yes].

## Logical Machines - Exercises
- Define or use the exercise machines from the previous session.
- Note the processes that can be executed by each machine (e.g., drilling, grinding, arrissing).
- Create the appropriate logical machines.
- A toughening furnace can toughen and semi-toughen lites. Would you create different logical machines for these two functions? List the benefits and disadvantages.

## Work Processes

### Objectives
- Understand the meaning of work processes in machinery allocation.
- Learn how to manage, define, edit, and delete them.
- Understand work process priorities and the relation to processing types/articles.

### Benefit
- A work process fulfills a processing step request from the bill of materials (e.g., polishing, grinding).
- The logical machine level connects the work process to the physical machine.

### Note
- Work processes bring together properties of a processing type (e.g., Cutting) with properties of the work piece.
- They are based on processing types or articles.
- Conditions/formulas can also be used to define them.

### Work Processes and Machine Allocation
A work process is defined by a processing type, a processing article, an article group, and/or an additional condition.

(Reference Fig. G-6, Work Processes tab in MA editor)

If a processing type (e.g., Cutting) is defined for a work process, this describes the technical type of processing. You should only create your own processing types if no appropriate predefined ones exist. Create separate work processes if you can make statements about your production, e.g.:
- You combine screen printing in dark colors on a specific day (campaign planning).
- Thick sheets are ground on machine 1, thin sheets on machine 2.
- Series sheets may only be drilled on the automatic drilling line.

The work process `pseudo-processing` is for informational processings in the BOM (e.g., *do not stamp*, *use gloves*). They are scheduled on a machine `Dummy for informative processings` which has no PDC registration point or shift plan.

### Processing items on work process
You can further specify a work process by choosing a restriction in the **Article** field.
- **Article type (A)**: Predefined by A+W, includes basic articles like toughened glass, laminated glass, etc.
- **Article group (B)**: A user-defined production article group.
- **Article (C)**: A specific article.

**Example**:
- Selecting processing type `Cutting` and article `Toughened glass` defines a work process for cutting toughened glass.
- Selecting processing type `Cutting` and article `Float 6 mm` defines a work process for cutting 6 mm float glass.

(Reference Fig. G-7, Work process – article dialog and Fig. G-8, Examples of differently defined work processes)

### Exact definition of work processes
Use the options in the **Work process** dialog to create detailed definitions.

**Example 1:**
Laminated glass can only be cut on tables with two heads or special technology. The work process `Cutting` is for float glass. Define a new work process for laminated glass cutting by selecting processing type `Cutting` and glass type `LAMI`. This new work process can only be allocated to logical machines that can perform this specific task.
