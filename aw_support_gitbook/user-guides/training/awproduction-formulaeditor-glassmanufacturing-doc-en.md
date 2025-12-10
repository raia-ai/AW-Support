---
title: "A+W Formula Editor"
category: "training"
product: "AWProduction"
doc_type: "Documentation"
language: "EN"
tags: ["AWProduction", "FormulaEditor", "GlassManufacturing", "Doc"]
version: "1.0"
last_updated: "2025-12-10"
description: "title: "EN_AWProduction_Formula_Editor_1.02" source: "EN_AWProduction_Formula_Editor_1.02.pdf" tags: ["A+W Production", "Formula Editor", "Software Manual", "Glass Manufacturing", "Window Production", "Conditions", "Formulas", "Allocation", "Technical Documentation", "ERP"] version: "1.0" last_updated: "2025-10-03" short_description: "A technical manual for the A+W Formula Editor, a component of the A+W Production software. This guide details the functional principles, operational steps, and sof"
source_file: "AWProduction-FormulaEditor-GlassManufacturing-Doc-EN.md"
---


title: "EN_AWProduction_Formula_Editor_1.02"
source: "EN_AWProduction_Formula_Editor_1.02.pdf"
tags: ["A+W Production", "Formula Editor", "Software Manual", "Glass Manufacturing", "Window Production", "Conditions", "Formulas", "Allocation", "Technical Documentation", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical manual for the A+W Formula Editor, a component of the A+W Production software. This guide details the functional principles, operational steps, and software reference for creating and managing complex rules, conditions, and formulas for production processes in the glass, window, and door industries."
long_description: "This document serves as a comprehensive guide to the A+W Formula Editor within the A+W Production software suite. It is intended for end-users who need to define and manage rules for various production-related tasks. The manual is divided into several key sections. The 'Functional Principle' section explains the core concepts of the Formula Editor, breaking it down into three levels of complexity, from simple formulas and comparisons to advanced quantity and allocation rules. It also covers the specific syntax of the 'Formula.dll'. The 'Operation' section provides practical, step-by-step instructions for using the editor in different contexts, such as setting conditions for racks, organization groups, and production sections, as well as creating group formation modes. The 'Software Reference' section offers a detailed description of every dialog, field, button, and menu item within the Formula Editor, serving as a quick-reference for UI elements. Finally, the 'Partindex' provides a comprehensive alphabetical index for easy lookup of terms and functions. This manual is essential for users looking to customize and optimize their production logic for tasks like machinery allocation, label selection, and organizational grouping."
---

# A+W Formula Editor

## Introduction

In this part of the documentation you can find editorial notices.

### Revision Overview

| Part Version / Date | Description |
| :--- | :--- |
| 1.00 / 11-2004 | Original Version. |
| 1.01 / 07-2013 | Adapted to CI 2013 layout. |
| 1.02 / 01.2017 | Product and company names adjusted. |

### Editorial

The editorial contains the following themes:
- Notes on this document
- Copyrights
- Trademarks
- Contact

### Notes on this document

This document is intended only for end users of A+W Production.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and is subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The descriptions in this document are based on the full installation of A+W Production.

### Copyrights

© 2017, A+W Software GmbH, any right, also the right of reprint, the production of copies and of the translation, is reserved. The documentation must be copied, completely or in part, saved, or transferred only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH prior approval in writing.

### Trademarks

Any designation of hardware and software being mentioned in the documentation can also be registered trademarks or other commercial rights of third parties being protected by law. Rights of third parties being protected by law are to be observed insofar.

### Contact

**A+W Software GmbH**

Am Pfahlgraben
D-35415 Pohlheim
- +49 6404 2051 0
- +49 6404 2051 877
- aw.zentrale@a-w.com
- http://www.a-w.com

## Contents

### Revision Overview
R-3
### Editorial
R-3
### Contents
R-5
### Functional Principle
R-7
- Formula Editor R-9
- Objective of the Formula Editor R-9
- Elements of the Formula Editor: Level I R-9
  - Formula R-10
  - Comparison R-11
  - Condition R-11
  - Linking of Elementary Conditions R-13
  - Quantity R-14
  - Allocation R-15
- Elements of the Formula Editor: Level II R-15
  - Formula R-15
  - Comparison R-16
  - Condition R-16
  - Quantity R-17
  - Allocation R-18
- Elements of the Formula Editor: Level III R-18
  - Quantity R-18
- Notation Formula.dll R-20
  - Syntax R-20
  - Function R-21
  - Check Results R-23
  - List of Dialogs R-25
### Operation
R-27
- Conditions for Racks R-29
- Conditions for Organization Groups R-31
- Group Formation Mode R-34
- Conditions for Production Sections R-36
- More Examples R-39
### Software Reference
R-43
- Formula Editor R-45
- Select Conditions R-46
- Conditions - Editor R-48
- Condition R-51
- Condition Name R-53
- Info R-54
- Invert R-54
- Given Quantity R-55
- Enter Value (Numeric) R-55
- Select Quantity R-57
- Quantity Editor R-59
- Quantity Name R-61
- Info R-63
- Select Formulas R-64
- Formula Editor R-66
- Select Allocation R-69
- Allocation Editor R-69
### Partindex
R-73
- Index Formula Editor R-75

## Functional Principle

### Formula Editor

The formula editor is available in A+W Production in the sections:
- Organization
- Machinery Allocation
- Labels, Sketches, Bender Text

The formula editor has different levels. The more complex the formula, the higher the level.

The documentation on the formula editor was therefore split into:
- Elements of the Formula Editor: Level I
- Elements of the Formula Editor: Level II
- Elements of the Formula Editor: Level III

#### Objective of the Formula Editor

With regards to Organization, the formula editor is used to define conditions to allocate product properties to the appropriate racks.

In connection with machinery allocation, the formula editor is used to localize machinery depending on the processing, and the product properties.

Regarding labels, the formula editor helps to define conditions to select the necessary label layout with regards to the product properties.

#### Elements of the Formula Editor: Level I

The formula editor consists of the elements:
- "Formula" on page R-10
- "Comparison" on page R-11
- "Condition" on page R-11
- "Quantity" on page R-14
- "Allocation" on page R-15

##### Formula

In the simplest case, a formula consists of a term which can contain the valid object properties, constants, other formulas, and some operators. Possible operators are the basic arithmetical operations +, -, * and / plus brackets. Also, there are the String operators:

- `@LEFT`: Syntax STRING `@LEFT` ANZAHL = STRING
- `@RIGHT`: Syntax STRING `@RIGHT` ANZAHL = STRING
- `@MID`: Syntax STRING `@MID` INDEX = STRING ; the index is 0-based

All these operators can be mixed at random.
The formula affects just one element.

*Fig. R-1: Formula Editor screen showing an input field for a formula, with lists for existing properties and formulas.*

**Examples:**
- `$TEILETYP`
- `$MENGE * ($DICKE+1000)`
- `($BEARB1TEXT @MID $TEILETYP) @RIGHT ($DICKE/1000)`

##### Comparison

A comparison consists of 1-2 formulas, and a so-called comparison rule. Please note that you can use just one formula only if the comparison rule `Only formula 1` is used. In this case, the comparison is fulfilled if the result of formula 1 is one digit bigger than zero, or a non-empty string. Otherwise, the comparison is fulfilled if the term `FORMEL 1 VORSCHRIFT FORMEL 2` is true.

For formula 2, no formula needs to be defined for simple constants. In this case, activate radio button `Value` and enter the required constant.

*Fig. R-2: Comparison dialog showing two formula fields and a dropdown for comparison operators.*

**Examples:**
- Formula Element type = value 1
- Formula IG `Only formula 1`
- Formula triple width < Formula height
- Formula thickness = value 3 mm

##### Condition

*Fig. R-3: Condition with And Connection, showing multiple comparison fields linked together.*

A condition must be fulfilled so that the allocation can be made as defined by the formula(s). It is the top element within the formula structure and, in its simplest type, consists of a number of comparisons. The grouping of comparisons defines how the results of the comparisons must be linked to each other. Comparisons set next to another are linked by AND while comparisons set above one another are linked by OR. A condition is fulfilled if it is possible to find a horizontal path from left to right which only includes fulfilled comparisons.

**Examples: Simplest Type**

*Fig. R-4: Schematic Display of a Condition, showing a "Condition" box labeled "Ist ESG" linked to a "Comparison" box.*
*Fig. R-5: Conditions - Author dialog showing the components of an elementary condition.*

The condition is `toughened glass` is fulfilled if the formula `element type toughened glass` with the property of database field `E_TG` from `Pool_Elements` contains the value One (based on the operation `only formula`).

**Examples: Linking of Elementary Conditions**

*Fig. R-6: Schematic Display of the Linking of Elementary Conditions, illustrating AND and OR linking logic.*
*Fig. R-7: UI example of linking elementary conditions for Shape Number and Processing.*

##### Quantity

*Fig. R-8: Quantities - Creator dialog showing different quantity selection options (Master, Parent, Self, etc.).*

A quantity consists of the rule of how to form the final quantity from the start element (BOM). The following rules can be combined at random.
⇨ Software Reference, "Quantity Editor" on page R-59

An element can represent a processing step.

*Fig. R-9: Schematic Display of the quantity, showing a BOM tree structure for an IG unit.*

For instance, the condition is `toughened glass` and quantity `Parent` results in all final and interim products produced from one or more toughened glass elements.

##### Allocation

The simplest type is the allocation of an object property to a formula. The result of the formula is allocated to the object property.

**Example:**
- EXTRA THICKNESS = formula `2mm`
- STACK WIDTH = `Height`

#### Elements of the Formula Editor: Level II

The formula editor consists of the elements:
- "Formula" on page R-15
- "Comparison" on page R-16
- "Condition" on page R-16
- "Quantity" on page R-17
- "Allocation" on page R-18

##### Formula

The formula now contains a quantity plus instructions. Without the quantity, the formula directly affects the object to be checked. When a quantity is defined, the object to be checked is converted into a quantity, the object being the start object of the quantity. The formula will be applied to each object of the final quantity; the results will be linked according to instructions. If the final quantity contains no objects, a long value -1 is returned.

*Fig. R-10: Formula dialog showing operation options like Total, Average, AND, OR, etc.*

**Examples:**
- `$THICKNESS`; quantity: `all basic elements`; TOTAL➔ total thickness
- `1`; quantity: `all processings`; TOTAL → number of processings

Valid operations are `total`, `average`, `And link`, `Or link`, `minimum` and `maximum`.

##### Comparison

Normally, a comparison consists of 1-2 formulas and the instruction. Alternatively, a comparison can be expressed by a condition (activate radio button `Conditions`). In this case, the comparison is fulfilled if the allocated condition is fulfilled. This type of linking conditions is used whenever two or more conditions are applied to different quantities.

*Fig. R-11: Comparison dialog showing a condition being used instead of a second formula.*

##### Condition

A condition can be inverted, i.e. it is fulfilled if the result of the comparisons is not fulfilled, and vice versa. This way, you can easily create from an existing condition the inverted one. The inverted condition contains just one comparison which will be allocated the original condition. Moreover, the characteristic `invert` will be selected for the inverted condition. The status line shows `INV` in front of the condition name.

The comparisons are usually analyzed for the object to be checked. If you want to check however whether one of the sub-elements of an object has a certain element type/processing type, you can allocate a quantity to the condition. In this case, the object is changed into a quantity, the object being the start object of the quantity. The condition will be analyzed for all elements of the final quantity. You only need to define when the condition is fulfilled. If it is sufficient that part of the final quantity fulfils the condition, select operation `One`. If the condition is only fulfilled if all elements of the final quantity fulfil the condition, select operation `All`. If the final quantity contains no objects, the condition is not fulfilled.

**Examples:**
- Formula `Element type` = value `125`; quantity `All sub-elements`; `One` with processing type =125
- Formula `E_IG` `Only formula 1`, quantity `Main element`; `One` (or `All`). The main element is IG.

*Fig. R-12: Condition Editor showing a condition with an associated quantity.*

##### Quantity

The quantity definition contains a condition. All objects which does not fulfil the condition, will be removed from the final quantity.

**Example:**
- `; Anychild; condition processing;`
  -> The final quantity contains only the processings below the start element.

If a condition is used, the two instructions `Up` and `Addup` can be used. These must not be combined with other instructions.

Using `Up` means that the final quantity consists of one element only. Starting from the start element, all main elements of the start element will be checked whether they fulfil the condition. The final quantity contains the last element fulfilling the condition. Should one element fail to fulfil the condition, the upwards iteration will be aborted.

`Addup` means that the final quantity can consist of more than one element. Like with `Up`, there is an upward iteration from the start element which will be stopped should one element fail to fulfil the condition. The final quantity, however, contains all elements fulfilling the condition.

**Examples:**
- `; Up; condition no processing`
- `; Addup; condition not ordered`

##### Allocation

The allocation can include a quantity. In this case, the result of the formula of the property will be allocated to all objects of the final quantity.

**Example:**
- EXTRA THICKNESS = Formula `2mm`; quantity `All cut elements`

#### Elements of the Formula Editor: Level III

##### Quantity

Quantity definition will always be loaded with a start quantity. In simple cases, the start quantity consists of just one element, namely the start element. Dialog `Quantity Editor` allows to logically group several elements next to each other or below each other, like in the `Conditions Editor`. The elements in the `Quantity Editor` are different. The vertically grouped quantities form the combined quantity while the horizontally grouped quantities form the intersection.

Please note that there is a second window for the edition of quantities. You can switch between the first and second window via button `[+/-]`. The start quantity is found by removing from the quantity of the first(+) window all objects of the quantity of the second(-) window.

**Examples:**
- `{quantity main element or Self; Anychild + Self ; ; }`
  - 1st window (Plus): Quantity `main element` or `self`
  - 2nd window (Minus): empty
  - `Anychild` and `Self` are tagged

This produces a main element, and all sub-elements of the main element. If there is no main element, the final quantity includes the start element and all its sub-elements.

*Fig. R-13: Quantities - Creator dialog showing the setup for a quantity calculation.*

The result is the final quantity with all elements sharing the main element of the start element.

If the iteration for `Up` or `Addup` shall not start with the element itself, but with the main element, first form the start quantity from the start element, using quantity main element `{;Parent;;}`, and use this with the required quantity, and the instruction `Up` or `Addup`.

This quantity can be allocated a formula. In this case, the formula will be analyzed for all elements of the start quantity; the results will be saved. From the final quantity, all elements will be removed the start quantity of which does not contain the result of the formula.

**Example:**
- `; All;; Formula Element type`
  Produces all elements of the BOM which are of the same type as the start element.

### Notation Formula.dll

#### Syntax

**ASSIGNMENT**
Input: Object, UserSet
`PROPERTY = FORMULA ; SET [/USERSET]`

**FORMULA**
Input: Object, UserSet
`[ formulaelements ; SET ; OP [/USERSET]]`
`OP ∈ {total, average, And, Or,Minimum, Maximum}`
`formulaelements = property, FORMULA ; + - * / () 0..9 @LEFT @RIGHT @MID`

**CONDITIONS**
Input: Object, UserSet
`'conditionelements ; SET ; OP [/N] [/USERSET]`
`OP ∈ {NULL,One,All}`
`conditionelements = CONDITION(S)`
or
`(conditionelements OP conditionelements) OP ∈ {And, Or}`

**CONDITION (comparison)**
Input: Object, UserSet
`'FORMULA [OP FORMULA];;'`
`OP ∈ {=,!=,>,>=,<,<=}`

**SET**
Input; Set, UserSet
`{ (setelements)[-(setelements)] ; OP ; CONDITIONS ; FORMULA [/USERSET] }`
Note: Element,`-(setelements)' is used only if it is not ,empty'.
`OP ∈ {All, Master,Parent,Self;Child,Anychild,Bottom,Up,Addup}`
`setelements = 'empty'`
or
`SET`
or
`(setelements OP setelements) OP ∈ {n, U}`

#### Function

**ASSIGNMENT**
The UserSet is transferred to FORMULA and SET.
- **without Set, without UserSet**: The FORMULA will be analyzed for this object. The result of the FORMULA is allocated to the object PROPERTY.
- **With Set**: SET is used to create a quantity from the given object. For every element of this quantity, the FORMULA will be analyzed; the result will be allocated to the PROPERTY of the corresponding object.
- **With UserSet**: For every object of the UserSet, the FORMULA will be analyzed; the result will be allocated to the PROPERTY of the corresponding object.
- **With Set, with UserSet**: Invalid, impossible.

**FORMULA**
The UserSet is transferred to the SET and to all FORMULAs in formula elements.
- **without Set, without UserSet**: All formulaelements for the given object will be analyzed; the complete term will be calculated. The result is returned as MultiValue.
- **With Set**: SET is used to create a quantity from the given object. All formulaelements for every element of this quantity will be analyzed; the complete term will be calculated. The results will be analyzed as per Operation; the total result will be returned as MultiValue.
- **With UserSet**: All formulaelements for every element of the UserSet will be analyzed; the complete term will be calculated. The results will be analyzed as per Operation; the total result will be returned as MultiValue.
- **With Set, with UserSet**: invalid, impossible

**CONDITIONS**
The UserSet is transferred to SET and to all CONDITION(S)s in the conditionelements.
- **without Set, without UserSet**: All conditionelements for the given object will be analyzed; the total result will be calculated and returned as BOOLEAN.
- **With Set, (with Operation != ZERO)**: SET is used to create a quantity from the given object. All formulaelements for every element of this quantity will be analyzed; the complete BOOLEAN term will be calculated. If the Operation = ONE, CONDITIONS will return TRUE if for at least one element the complete BOOLEAN term is fulfilled, i.e. TRUE. If however the Operation = ALL, CONDITIONS will return TRUE if the complete BOOLEAN term is fulfilled, i.e. TRUE for all elements. Otherwise, FALSE will be returned.
- **With UserSet**: All formulaelements for every element of the UserSet will be analyzed; the complete BOOLEAN term will be calculated. If the Operation = ONE, CONDITIONS will return TRUE if for at least one element the complete BOOLEAN term is fulfilled, i.e. TRUE. If however the Operation = ALL, CONDITIONS will return TRUE if the complete BOOLEAN term is fulfilled, i.e. TRUE for all elements. Otherwise, FALSE will be returned.
- **With Set, with UserSet**: invalid, impossible

**CONDITION**
The UserSet is transferred to every FORMULA.
- **Any**: Both FORMULAS, if existing, will be analysed for the given object. If there is only one FORMULA, TRUE will be returned if the result of FORMULA is not ZERO (numeric result), or if it is no empty string for string results. Otherwise, FALSE will be returned. If both FORMULAs do exist, the results will be compared acc. to the Operation. If the comparison is fulfilled, TRUE will be returned; otherwise, FALSE.

**SET**
All SETS, CONDITIONS and FORMULA included in setelements will be transferred to the UserSet.
- **without FORMULA, without UserSet**: All setelements for the given Set will be calculated; the preliminary quantity A will be determined. For every object of this quantity A, quantity BA will be determined as per Operation, to be added to quantity B. From quantity B, all objects will be removed which do not fulfil the CONDITIONS. As a result, quantity B is returned as RelatedSet.
- **with FORMULA, without UserSet**: Initially like A, but quantity B will not be returned. The FORMULA will be analyzed for every object from the given Set. The results will be saved in an array. Next, the FORMULA is analyzed for every object in quantity B. If the array includes the result of the FORMULA for an object from quantity B, the corresponding object will be added to quantity C. As a result, quantity C is returned as RelatedSet.
- **without FORMULA, with UserSet**: Like A, but instead of the given Sets, the UserSet will be used to form quantity A.
- **with FORMULA, with UserSet**: Like B, but instead of the given Sets, the UserSet will be used to form quantity A. Still, the given Set will be used to form the array.

**Example:**
For lite A and a certain number of lites, you want to determine the total number of all lites belonging to the same route as lite A:
`[$MENGE ; { ; ; ; [$TOUR] /USERSET } ; SUM }`

Lite X shall be kept at the rack only if it is laminated glass, and if the total of all lites includes at least 150 laminated lites:
`´ ('[T_VSG;;]=[1;;];;` AND ´[$MENGE;{;;''[T_VSG;;]==[1;;]';;';/USERSET};SUM]`>=[150;;]`) ; ; ``

#### Check Results

To check the results of the formulas, you can view the corresponding log file. To activate the result check for Detailed Scheduling, the following setting must be made in A+W Production:

Master Data > Parameters > Module Detailed Scheduling > Specials > View Formula > Enter value 1

> **Performance**
> Viewing the calculations will impair the performance!

*Fig. R-14: Log file example showing the step-by-step evaluation of a formula.*

The log file for the result check is found in
`\<AlcimRootDir>\Log\(Name of log file of Detailed Scheduling).LOG`

#### List of Dialogs

This list shows all dialogs you need to use the formula editor properly. The references lead to chapter Software Reference in the master data section. You will find detailed information on the dialogs, fields and buttons.

**Base Data Menu**

| Menu Entry | Dialog/Function |
| :--- | :--- |
| The formula editor cannot be reached by means of a menu entry. The individual dialogs will tell you how to access it. | ⇨ "Select Conditions" on page R-46<br>⇨ "Conditions - Editor" on page R-48<br>⇨ "Condition" on page R-51<br>⇨ "Condition Name" on page R-53<br>⇨ "Info" on page R-63<br>⇨ "Select Formulas" on page R-64<br>⇨ "Formula Editor" on page R-66<br>⇨ "Select Allocation" on page R-69<br>⇨ "Allocation Editor" on page R-69 |

## Operation

### Conditions for Racks

Explains how to define, change, or delete conditions for racks in section Organization.

**This is how you define a condition for a rack, filtering all lites with an edge length over 1,20 m**

1.  Open the Organization Dialog via:
    Master Data > Detailed Scheduling > Organization
2.  Open tab `Production Sequence`.
3.  Tag the rack for which you want to define a condition.
4.  Press button `[New Condition]`. The dialog `Select Conditions --1--` appears.
5.  Press button `[New Condition ...]`. This opens the dialog `Conditions Editor`.
6.  In menu `Conditions`, open `Names`. This leads to dialog `Condition Name`. Field `New Name` shows `New Condition` by default. Give the condition a characteristic name. Example: `Large Lite`. Close the dialog via button `[OK]`.
7.  In menu `Conditions`, open `Info`. This opens dialog `Info`. Enter a clear description of this condition. Example: `This condition is true if one edge of a lite is longer than 1,20 m`. Close the dialog via button `[OK]`.
8.  In menu `Partial Conditions`, open `Add Part.Cond. (AND)`. A new element condition appears, and can be configured.
9.  Open the combo box (by default showing `Only Formula 1`) and select `>=` (greater or equal).
10. Activate the radio button `Value`. The dialog `Enter Value (Numeric)` automatically appears. Since the new rack shall only contain lites over 1,20, activate the radio button `Length`, and enter in section `New Value` **1200 mm**. Close the dialog via button `[OK]` This value will appear in the bottom field of the condition.
11. Click on the top input field of the condition. The dialog `Select Formulas --1--` appears automatically. Define what the value entered in the second input field shall refer to.
12. Press button `[New Formula ...]`. The dialog `Formula Editor` appears. Enter a characteristic name for the formula in the top left field. Example: `Large Dimension`.
    ⇨ Software Reference, "Top input field" on page R-67
13. In section `Existing Properties`, double-click on `Large_Dim`.
    ⇨ Software Reference, "Existing Properties" on page R-68
14. Close the dialog via button `[OK]` You will find yourself back in dialog `Condition Editor`.

The defined condition looks like this:
*Fig. R-15: Condition for lites >= 1200 mm, showing the formula 'Large Dimension >= 1200.0 mm'.*

Close the dialog via menu `Conditions > OK`, or by clicking on the checkmark. You will find yourself back in dialog `Select Conditions --1--`. You will find the defined condition `Large Lite` at the end of the list `Existing Properties`.

**This is how to allocate a condition to a rack**

1.  Open the Organization Dialog via:
    Master Data > Detailed Scheduling > Organization
2.  Open tab `Production Sequence`.
3.  Tag the rack the condition shall be allocated to.
4.  Press button `[New Condition]`. The dialog `Select Conditions --1--` appears.
5.  On the list of `Existing Conditions`, tag the condition to be allocated to this rack.
6.  Close the dialog via button `[OK]`.
7.  The condition was added to the rack tagged in tab `Production Sequence`.

**How to delete a condition allocated to a rack**

1.  Open the Organization Dialog via:
    Master Data > Detailed Scheduling > Organization
2.  Open tab `Production Sequence`.
3.  Double-click on the rack to open it.
4.  Tag the condition to be deleted.
5.  Press the `[Delete]` button. The condition will be deleted instantly.

> **Delete**
> Deletion is not accompanied by a security check. If you have deleted something by mistake, leave the tab `Production Sequence` via button `[Cancel]`. The system will want to know whether the changes shall be ignored. Answer `[OK]`. The Organization Dialog will be closed. When you open it next, the data will still be there.

### Conditions for Organization Groups

Explains how to define, change, or delete conditions for organization groups in section Organization.

**How to define a condition for an organization group, filtering IG with Grills for a second production step**

1.  Open the Organization Dialog via:
    Master Data > Detailed Scheduling > Organization
2.  Open tab `Production Sequence`.
3.  Tag the rack for which you want to define an organization group.
4.  Press button `[New Condition]`. The dialog `Select Conditions --1--` appears.
5.  Press button `[New Condition ...]`. This opens the dialog `Conditions Editor`.
6.  In menu `Conditions`, open `Names`. This leads to dialog `Condition Name`. Field `New Name` shows `New Condition` by default. Give the condition a characteristic name. In our example: `IG – Grills`. Close the dialog via button `[OK]`.
7.  In menu `Conditions`, open `Info`. This opens dialog `Info`. Enter a clear description of this condition. In our example: `Item was allocated to production step 2 MZO_ROUTE_MAP.ROUTE =2`. Close the dialog via button `[OK]`.
8.  In menu `Partial Conditions`, open `Add Part.Cond. (AND)`. A new element condition appears, and can be configured.
9.  Open the combo box (by default showing `Only Formula 1`) and select `==` (equal).
10. Activate the radio button `Value`. The dialog `Enter Value (Numeric)` automatically appears. Since IG with Grills only produced in production step 2, activate the radio button `Digit` and enter in section `New Value` **2**. Close the dialog via button `[OK]`. This value will appear in the bottom field of the condition.
11. Click on the top input field of the condition. The dialog `Select Formulas --1--` appears automatically. Define what the value entered in the second input field shall refer to.
12. Press button `[New Formula ...]`. The dialog `Formula Editor` appears. Enter a characteristic name for the formula in the top left field. In our example: `Production Step`.
13. In section `Existing Properties` double-click on `Route`. Section `Formula` shows `$Route`.
14. Close the dialog via button `[OK]`. You will find yourself back in dialog `Condition editor`.

The defined condition looks like this:
*Fig. R-16: Condition Production Step = 2, showing the formula 'Production Step == 2'.*

Close the dialog via menu `Conditions > OK`, or by clicking on the checkmark. You will find yourself back in dialog `Select Conditions --1--`. You will find the defined condition `IG - Grills` at the end of the list `Existing Properties`.
15. Tag the condition and press `[Ok]`. The condition will be added to the previously tagged organization group.

**How to allocate an existing property to an organization group**

1.  Open the Organization Dialog via:
    Master Data > Detailed Scheduling > Organization
2.  Open tab `Production Sequence`.
3.  Tag the organization group to define a condition.
4.  Press button `[New Condition]`. The dialog `Select Conditions --1--` appears.
5.  On the list of `Existing Conditions`, tag the condition to be allocated to this organization group.
6.  Close the dialog via button `[OK]`.
7.  The condition was added to the organization group tagged in tab `Production Sequence`.

**How to delete a condition allocated to an organization group**

1.  Open the Organization Dialog via:
    Master Data > Detailed Scheduling > Organization
2.  Open tab `Production Sequence`.
3.  Double-click on the organization group to open it.
4.  Tag the condition to be deleted.
5.  Press the `[Delete]` button. The condition will be deleted instantly.

> **Delete**
> Deletion is not accompanied by a security check. If you have deleted something by mistake, leave the tab `Production Sequence` via button `[Cancel]`. The system will want to know whether the changes shall be ignored. Answer `[OK]`. The Organization Dialog will be closed. When you open it next, the data will still be there.

### Group Formation Mode

This example serves to add another selectable mode for group formation for organization groups and racks.

**This is how you create a grouping by number of lites per customer, i.e. a group will be created per customer and this group will be sorted by the number of lites included. The group with the largest number of lites will be produced first.**

1.  Open the `Grouping/Sorting` Dialog via:
    Master Data > Detailed Scheduling > Grouping
2.  Press button `[Formulas ...]`. The dialog `Select Formulas --1--` appears.
3.  Press button `[New Formula ...]`. The dialog `Formula Editor` appears.
4.  Enter the name for the grouping formula in the top left field. In our example, `number of lites per customer`.
5.  In section `Existing Properties`, double-click on `Qty`. Section `Formula` shows `$Qty`.
6.  Press button `[Quantity ...]`. The dialog `Select Quantity --1--` appears.
7.  Use button `[New Quantity ...]` to define a new quantity. This opens dialog `Quantity Editor`. Starting from a given quantity we will perform quantity operations to get the final quantity. Detailed Scheduling transfers to the formula editor values for a customer's item, the quantity calculation, and all orders of the job on hand. Just add the customer number.
8.  In menu `Quantity`, open `Names` and enter a new, characteristic name for the quantity. In our example, `number of lites per customer`. Close the dialog via button `[OK]`.
9.  In menu `Quantity`, open `Given Quantity`. As a result, not only the item used to start the quantity editor will be considered for quantity calculation, but also all items of the job.
10. As the required quantity shall not include all elements, but only the released elements, activate in dialog `Quantity Editor` the checkbox `Master`.
11. To add the customer number as a property to the quantity, select in menu `Quantity`, `Formula`. The dialog `Select Formulas --2--` appears. Use button `[New Formula ...]` to enter the formula for the customer number. The dialog `Formula Editor` appears.
12. Enter the formula name in the top left input field. In our example, `Customer Number`.
13. In section `Existing Properties`, double-click on `Customer No.` Section `Formula` shows `$Customer No.`
14. Press `[Ok]`. You will return to dialog `Select Formulas --2--`. The last entry on the list will be the just defined formula for the customer number. Tag the `Customer No.` on the list, and press `[Ok]`. This brings you back to dialog `Quantity Editor`.
15. The right side of the status line of the quantity editor shows whether - and if so, which - formula is used to define the new quantity. In our example, this is: `Formula: Customer No.`
16. Tag all open dialogs via `[Ok]` until you reach dialog `Grouping/Sorting`.
17. The list of formulas now includes the formula `number of lites per customer`. Tag the formula and press `[Add]`. The formula will be added to the groupings in tab `Grouping Editor`. It will be available in the settings for the `Organization Groups` and the `Racks`, in section `Group Formation`.

### Conditions for Production Sections

This tells you how to define, change, or delete conditions for production sections in part `Machinery Allocation`.

**How to define a condition for a production section, filtering all lites with Grills**

1.  Open dialog `Production Sections` via:
    Master Data > Machinery Allocation > Setup
2.  Tag the production section for which you want to define a condition.
3.  Use the right mouse key. The context menu appears. From the context menu, select:
    `Condition of production section > New`
4.  The dialog `Select Conditions --1--` appears.
5.  Press button `[New Condition ...]`. This opens the dialog `Conditions Editor`.
6.  In menu `Conditions`, open `Names`. This leads to dialog `Condition Name`. Field `New Name` shows `New Condition` by default. Give the condition a characteristic name. In our example: `Grills - IG`. Close the dialog via button `[OK]`.
7.  In menu `Conditions`, open `Info`. This opens dialog `Info`. Enter a clear description of this condition. Example: `This condition is true if the item shows a Grill flag`. Close the dialog via button `[OK]`.
8.  In menu `Partial Conditions`, open `Add Part.Cond. (AND)`. A new element condition appears, and can be configured.
9.  The combo box shows `Only Formula 1` by default. In our example, this remains unchanged.
10. The radio button `Normal` is active by default. In our example, this remains unchanged, too.
11. Click on the top input field of the condition. The dialog `Select Formulas --1--` appears automatically.
12. Press button `[New Formula ...]`. The dialog `Formula Editor` appears. Enter a characteristic name for the formula in the top left field. In our example: `Grills`.
13. In section `Existing Properties` double-click on `Item_Grill_Flag`. Section `Formula` shows `$Item_Grill_Flag`.
14. Close the dialog via button `[OK]`. This brings you to dialog `Select Formulas --1--`. The just defined formula is tagged already.
15. Close the dialog via button `[OK]`. You will find yourself back in dialog `Condition Editor`.

The defined condition looks like this:
*Fig. R-17: Condition IG with Grills, showing the formula 'Grills' with 'Only Formula 1'.*

Close the dialog via menu `Conditions > OK`, or by clicking on the checkmark.
You will find yourself back in dialog `Select Conditions --1--`. You will find the defined condition `Grills - IG` at the end of the list `Existing Properties`.

**This is how to allocate a condition to a production section**

1.  Open dialog `Production Section` via:
    Master Data > Machinery Allocation > Setup
2.  Tag the production section the condition shall be allocated to.
3.  Use the right mouse key. The context menu appears. From the context menu, select:
    `Condition for Production Section > New`
4.  The dialog `Select Conditions --1--` appears.
5.  On the list of `Existing Conditions`, tag the condition to be allocated to this production section.
6.  Close the dialog via button `[OK]`.
7.  The condition was added to the tagged production section.

**How to delete a condition allocated to a production section**

1.  Open dialog `Production Section` via:
    Master Data > Machinery Allocation > Setup
2.  Double-click on the production section to open it.
3.  Tag the condition to be deleted.
4.  Use the right mouse key. The context menu appears. From the context menu, select `Delete Condition`.
    The condition will be deleted instantly!

> **Delete**
> Deletion is not accompanied by a security check. If you have deleted something by mistake, leave the tab `Production Sections` via button `[Cancel]`. When you open it next, the data will still be there.

### More Examples

**How to define a condition for toughened glass within IG, or float glass processing**

1.  **First step**
    *Fig. R-18: Toughened Glass condition.*
    In formula `Toughened Glass`, the property `E_TG` is returned.
2.  **Now check whether the element is part of IG**
    *Fig showing a complex quantity operation to identify a 'Mate' part by starting with a parent, finding all children, and subtracting itself.*
3.  As an element cannot be toughened glass and IG at the same time, the condition shown in step 2 cannot work. Hence ...
4.  Check the Or connection, whether one of the sub-elements is a processing step. Another condition will be created, checking the formula `Processing` for all childs.
    *Fig. R-19 & R-20: OR connection logic to check if a part is TGH OR its parent is IG, and checking for processing steps.*

**The processing steps directly below**

1.  The final quantity shall contain only the processing steps below the start element which will be made after the last processing steps defined.
2.  The system first unites all sub-elements which are no processings.
3.  Quantity `Defined processing steps below` = `{ ; ANYCHILD ; condition is no processing; }`
4.  This quantity is used to define the number of elements and processing steps below the start element you do not require.
5.  Quantity `Unwanted elements/processing steps below` = `{ number of defined processing steps below ; ANYCHILD+SELF ; ; }`
6.  The required quantity is determined by the number of `all sub-elements` and the number of `unwanted elements/processing steps below`.
    `{ number of all sub-elements - number of unwanted elements/processings below; SELF ; ; }`

## Software Reference

### Formula Editor

The Formula Editor is used in the following areas of A+W Production:
- Organization
- Machinery Allocation
- Labels, Sketches, Bender text

Instructions on how to open individual dialogs are provided in the following dialog descriptions. If there exist alternative methods to open a dialog, these are also specified.

### Select Conditions

**Load via**

-   **Organization**
    -   Master Data > Detailed Scheduling > Organization > Tab: Production Sequence > Tag Organization Group > [New Condition]
    -   Master Data > Detailed Scheduling > Organization > Tab: Production Sequence > Tag Rack > [New Condition]
-   **Machinery Allocation**
    -   Master Data > Machinery Allocation > Setup > Tag Production Section > right mouse key > Condition of Production Section > New
    -   Master Data > Machinery Allocation > Setup > Tag Condition of Production Section > right mouse key > Edit Condition
    -   Master Data > Machinery Allocation > Setup > [Technology] > [New] > [New]
    -   Master Data > Machinery Allocation > Setup > [Technology] > [Change] > [New]/[Edit]
-   **Labels, Sketches, Bender Text**
    -   Master Data > Labels / Sketches / Bender texts > Configuration ... > Tag Condition > [Formula Editor]

*Fig. R-21: Select Conditions --1-- dialog.*

This dialog allows to select, or change existing conditions for the sections Organization, Machinery Allocation and Labels, Sketches, Bender text, or to define new conditions.

**Fields**

-   **Existing Conditions**: The table lists all conditions existing in the system for the sections Organization, Machinery Allocation and Labels, Sketches, Bender text. The contents differ from section to section!
-   **No Condition**: If this checkbox is active, the dialog shows as a result that `Nothing` was selected.
-   **Description**: The field contains a detailed description of the condition. This is the text entered in field `Info`.

**Buttons**

-   **Delete**: Use this button to delete the tagged condition. Deletion will be made without a security check.
-   **New Condition**: Press this button to open dialog `Conditions - Editor`. You can define a new condition.
-   **Edit**: Press this button to open dialog `Conditions - Editor` for the tagged condition.

**Additional information on conditions**
-   Functional Principle, “Elements of the Formula Editor: Level I" on page R-9
-   Functional Principle, "Elements of the Formula Editor: Level II" on page R-15

### Conditions - Editor

**Load via**

-   **Organization**: Master Data > Detailed Scheduling > Organization > ... > [New Condition ...] / [Edit]
-   **Machinery Allocation**: Master Data > Machinery Allocation > Setup > ... > [New Condition ...] / [Edit]
-   **Labels, Sketches, Bender text**: Master Data > Labels / Sketches / Bender text > Configuration > ... > [New Condition ...] / [Edit]

*Fig. R-22: Conditions - Editor dialog.*

Conditions - Editor allows to change a tagged condition, or to define a new condition.

**Menu and Dialog Functions**

| Menu Entry | Dialog/Function |
| :--- | :--- |
| **Menu Conditions:** | |
| Name | ⇨ "Condition Name" on page R-53 |
| Info | ⇨ "Info" on page R-54 |
| Quantity | ⇨ "Select Quantity" on page R-57 |
| Invert | ⇨ "Invert" on page R-54 |
| Transferred quantity | ⇨ "Given Quantity" on page R-55 |
| OK | Closes dialog, saving changes |
| Abort | Closes dialog, discarding changes |
| **Menu Element Conditions:** | |
| ⇨ Add (column) | Adds an AND condition |
| Add (line) | Adds an OR condition |
| Delete | Deletes the selected condition |

**Tool Bar**

| Tool | Explanation |
| :--- | :--- |
| ✅ | The defined condition will be saved, and the editor is closed |
| ❌ | The defined condition will be rejected, and the editor is closed |
| `++` | Opens the window to define the condition. Double-click to open two windows next to another; these represent an **And** connection. ⇨ "Condition" on page R-51 |
| `‡` | Opens the window to define the condition. Double-click to open two windows, one below the other; these represent an **Or** connection. ⇨ "Condition" on page R-51 |
| `-` | Deletes the selected condition. |

**Radio Buttons**

-   **All**: Considers the conditions for all elements of a BOM. With this setting, a lite without pattern - for instance - will be allocated to a rack with the condition pattern if the mate is patterned.
-   **One**: Only the characteristics of the lite in question will be considered.
-   **Null**: The quantity allocated to the condition will not be taken into account.

### Condition

**Load via**
This dialog is accessed by clicking the `++` or `‡` buttons in the `Conditions - Editor`.

*Fig. R-23: Condition dialog.*

-   **Top Input field**: Click on the field to open the dialog `Select Formulas`. You can select an existing formula, or enter a new one.
-   **Central Selection Field**: Open the combo box and select the operator. Valid entries:
    -   Only Formula 1
    -   == equal
    -   != unequal
    -   < smaller
    -   <= smaller or equal
    -   > bigger
    -   >= bigger or equal
-   **Bottom Input Field**: Click on the field to open dialog `Select Formulas`, `Enter Value (Numeric)` or `Select Conditions`. The active radio button (`Normal`, `Value`, `Conditions`) defines which dialog is going to be opened.
    -   **Normal**: Activate the radio button, then click on the bottom input field to open the dialog `Select Formulas`.
    -   **Value**: Activate this radio button to open dialog `Enter Value (Numeric)`.
    -   **Conditions**: Activate the radio button, then click on the bottom input field to open dialog `Selection Conditions --2 --`.

### Condition Name

**Load via**
This dialog is accessed from the `Conditions` menu in the `Conditions - Editor`.

*Fig. R-24: Condition Name dialog.*

Give the conditions characteristic names. The name will be shown in the status line of dialog `Conditions - Editor`.

**Fields**

-   **Old Name**: If a condition was given no name so far, this field will read `new condition` by default. When a name was allocated, this will be shown.
-   **New Name**: Enter the name of the condition. This can be overridden at any time.

### Info

**Load via**
This dialog is accessed from the `Conditions` menu in the `Conditions - Editor`.

*Fig. R-25: Condition Information dialog.*

You can describe the condition. The text will appear in dialog `Select Conditions` in section `Description`.

### Invert

A condition can be inverted, i.e. it is fulfilled if the result of the comparisons is not fulfilled, and vice versa. This way, you can easily create from an existing condition the inverted one. The inverted condition contains just one comparison which will be allocated the original condition. Moreover, the characteristic `invert` will be selected for the inverted condition. The status line shows `INV` in front of the condition name. This menu can be enabled or disabled as required.

### Given Quantity

This menu can be enabled or disabled as required. If it is active, the system will not only consider the item by which the dialog `Conditions - Editor` was opened, but also all items of the job when determining the quantities.

### Enter Value (Numeric)

**Load via**
This dialog is accessed from the `Condition` dialog when the `Value` radio button is active.

*Fig. R-26: Enter Value (Numeric) dialog.*

This dialog is used to enter numerical values. Activate the appropriate radio button to specify whether the numerical value is `Digit`, `Thickness`, `Text`, `Length` or `Airspace`.

**Fields**

-   **Old Value**: If a condition was given no value so far, this field will read 0 by default. If a value was allocated, this will be shown.
-   **New Value**: Enter the value for the condition. This can be overridden at any time.

**Radio Buttons**

-   **Digit**: If the condition refers to a quantity.
-   **Thickness**: If this condition refers to Thickness in mm.
-   **Text**: If this condition refers to Text.
-   **Length**: If this condition refers to a length.
-   **Airspace**: If the condition refers to an airspace.

### Select Quantity

**Load via**
This dialog is accessed from various points in the Formula Editor, typically via a `[Quantity ...]` button.

*Fig. R-27: Select Quantity dialog.*

This dialog allows to select, or change existing quantities.

**Fields**

-   **Existing Quantities**: The table lists all quantities existing in the system.
-   **No Quantity**: If this checkbox is active, the dialog shows as a result that `Nothing` was selected.
-   **Description**: The field contains a detailed description of the quantity.

**Buttons**

-   **Delete**: Deletes the tagged quantity.
-   **New Quantity**: Opens the `Quantity Editor` to define a new quantity.
-   **Edit**: Opens the `Quantity Editor` for the tagged quantity.

### Quantity Editor

**Load via**
This dialog is accessed from the `Select Quantity` dialog via the `[New Quantity]` or `[Edit]` buttons.

*Fig. R-28: Quantity - Editor dialog.*

`Quantity Editor` allows to change a tagged quantity, or to define a new quantity.

**Menu and Dialog Functions**

| Menu Entry | Dialog/Function |
| :--- | :--- |
| **Menu Quantity:** | |
| Name | ⇨ "Quantity Name" on page R-61 |
| Info | ⇨ "Info" on page R-63 |
| Condition | ⇨ "Select Conditions" on page R-46 |
| Formula | ⇨ “Select Formulas" on page R-64 |
| OK / Cancel | Closes the dialog |
| **Menu Partial Quantities:** | |
| Add Part. Cond.(AND) | Adds an AND condition |
| Add Part. Cond.(OR) | Adds an OR condition |
| Remove / Change | Modifies the selected partial quantity |

**Tool Bar**

| Tool | Explanation |
| :--- | :--- |
| ✅ | The defined quantity will be saved; the editor will be closed. |
| ❌ | The defined quantity will be rejected while the editor is closed. |
| `++` | Opens the window to define the quantity for an **And** connection. |
| `‡` | Opens the window to define the quantity for an **Or** connection. ⇨ "Condition" on page R-51 |
| `-` | Deletes the selected quantity. |
| `+/-`| Switches between the first and the second window (for subtraction). |

**Checkboxes**

-   **All**: All parts of the BOM containing the start part.
-   **Master**: The top part of the BOM (header) containing the start part.
-   **Parent**: Part right above the start part in the BOM.
-   **Self**: Start part.
-   **Child**: All direct sub-parts of the start part.
-   **Anychild**: All sub-parts of the start part, even the indirect ones.
-   **Bottom**: All basic parts below the start part.
-   **Up**: The final quantity consists of just one part. Iterates upwards from the start part checking a condition.
-   **AddUp**: The final quantity can consist of more than one part. Iterates upwards and includes all parts that fulfill the condition.

### Quantity Name

**Load via**
Accessed from the `Quantity` menu in the `Quantity Editor`.

*Fig. R-29: Quantity Name dialog.*

Give a characteristic name to the quantity. The name will be shown in the status line of dialog `Quantity Editor`.

**Fields**
- **Old Name**: Shows the existing name or `New Quantity` by default.
- **New Name**: Enter the name of the quantity.

### Info

**Load via**
Accessed from the `Quantity` menu in the `Quantity Editor`.

*Fig. R-30: Info dialog.*

You can describe the quantity. The text will appear in dialog `Select Quantity` in section `Description`.

### Select Formulas

**Load via**
Accessed from various points where a formula needs to be selected, such as the `Condition` dialog.

*Fig. R-31: Select Formulas dialog.*

This dialog allows to select, or change existing formulas or define new formulas.

**Fields**

-   **Existing Formulas**: The table lists all formulas existing in the system.
-   **No Formula**: If this checkbox is active, the dialog shows as a result that `Nothing` was selected.
-   **Description**: The field contains a detailed description of the formula.

**Buttons**

-   **Delete**: Deletes the tagged formula.
-   **New Formula**: Opens `Formula Editor` to define a new formula.
-   **Edit**: Opens `Formula Editor` for the tagged formula.

### Formula Editor

**Load via**
Accessed from `Select Formulas` via `[New Formula]` or `[Edit]`.

*Fig. R-32: Formula Editor dialog.*

This dialog allows to define new formulas.

**Fields**

-   **Top input field**: Enter a characteristic name for the formula.
-   **Description**: Enter a detailed description of the formula.
-   **Formula**: Enter the database field or expression for the formula.
-   **Quantity**: Press this button to open dialog `Select Quantity`.
-   **Given Quantity**: If this checkbox is active, the system will consider all items of the batch for the quantity creation.
-   **Existing Properties**: Lists database fields that can be used in formulas.
-   **Existing Formulas**: Lists other formulas that can be used.

**Radio buttons in section Operation**
(Active only when a quantity is allocated)
-   **Total (Value)**: Total results.
-   **Average**: Total/number of results.
-   **And Operation**: The results will be linked by a logical And.
-   **Or Operation**: The results will be linked by a logical Or.
-   **Minimum**: Smallest result.
-   **Maximum**: Biggest result.
-   **Number of Results**: Number of different results.

### Select Allocation

**Load via**
Master Data > Detailed Scheduling > Allocations

*Fig. R-33: Select Allocation dialog.*

This dialog allows to select or change allocations only for section Organization, or to define new allocations.

**Buttons**
- **Delete**: Deletes the tagged allocation.
- **New Allocation**: Opens `Allocation Editor`.
- **Edit**: Opens `Allocation Editor` for the tagged allocation.

### Allocation Editor

**Load via**
Master Data > Detailed Scheduling > Allocations > [New Allocation] / [Edit]

*Fig. R-34: Allocation Editor dialog.*

Use this dialog to define a new allocation. The simplest type is the allocation of an object property to a formula.

**Fields**

-   **Top Input Field**: Give the allocation a characteristic name.
-   **Property**: Select the database field (property) to be changed.
    > **Existing properties**
    > Object properties for Detailed Scheduling are firmly linked for reasons for performance, and cannot be extended without program amendments.
    -   **Important allocations:**
        -   **Stack width**: Will be used for rack loads.
        -   **Assessment**: 100 by default. Used in optimization to distribute lites to stockplates.
        -   **Difference in thickness**: Defines to what extent the glass thickness may change when lites are added.
        -   **Group number**: 0 by default. Used to create production groups.
        -   **Box**: Freely disposable.
        -   **Extra thickness**: 0 mm by default. Can be used for lites with silk screening.
-   **Formula**: Press this button to open dialog `Select Formulas`.
-   **Quantity**: Press this button to open dialog `Select Quantity`.
-   **Given Quantity**: Checkbox to consider all items of the batch for quantity creation.

## Partindex

### Index Formula Editor

**A**
- **AddUp**
  - Quantity Editor R-61
- **Airspace**
  - Enter Value (Numeric) R-56
- **All**
  - Conditions - Editor R-50
  - Quantity Editor R-61
- **Allocation**
  - Level I R-15
  - Level II R-18
- **Allocation Editor**
  - Characteristic R-70
  - Dialog R-69
  - Formula R-71
  - Given Quantity R-71
  - Quantity R-71
  - Top input field R-70
- **And Operation**
  - Formula Editor R-67
- **Anychild**
  - Quantity Editor R-61
- **Average**
  - Formula Editor R-67

**B**
- **Bottom**
  - Quantity Editor R-61
- **Bottom input field**
  - Condition R-52

**C**
- **Central selection field**
  - Condition R-52
- **Characteristic**
  - Allocation Editor R-70
- **Child**
  - Quantity Editor R-61
- **Comparison**
  - Level I R-11
  - Level II R-16
- **Condition**
  - Bottom input field R-52
  - Central selection field R-52
  - Condition R-51
  - Conditions R-52
  - Given Quantity R-55
  - Invert R-54
  - Level I R-11
  - Level II R-16
  - Normal R-52
  - Top input field R-51
  - Value R-52
- **Condition Name**
  - Dialog R-53
  - New Name R-53
  - Old Name R-53
- **Conditions**
  - Condition R-52
- **Conditions - Author**
  - Menu R-49
  - Tool bar R-49
- **Conditions - Editor**
  - All R-50
  - Dialog R-48
  - Null R-50
  - One R-50

**D**
- **Delete**
  - Select Allocation R-69
  - Select Conditions R-47
  - Select Formula R-65
  - Select Quantity R-58
- **Description**
  - Formula Editor R-67
  - Select Allocation R-69
  - Select Conditions R-47
  - Select Formula R-65
  - Select Quantity R-58
- **Dialog**
  - Allocation Editor R-69
  - Condition Name R-53
  - Conditions-Editor R-48
  - Enter Value (Numeric) R-55
  - Formula Editor R-66
  - Info R-54, R-63
  - Quantity Editor R-59
  - Quantity Name R-61
  - Select Allocation R-69
  - Select Conditions R-46
  - Select Formulas R-64
  - Select Quantity R-57
- **Digit**
  - Enter Value (Numeric) R-56

**E**
- **Edit**
  - Select Allocation R-69
  - Select Conditions R-47
  - Select Formula R-65
  - Select quantity R-58
- **Enter Value (Numeric)**
  - Airspace R-56
  - Dialog R-55
  - Digit R-56
  - Length R-56
  - New Value R-56
  - Old Value R-56
  - Text R-56
  - Thickness R-56
- **Existing Allocation**
  - Select Allocation R-69
- **Existing Conditions**
  - Select Conditions R-46
- **Existing Formulas**
  - Formula Editor R-68
  - Select Formula R-65
- **Existing Properties**
  - Formula Editor R-68
- **Existing Quantity**
  - Select Quantity R-58

**F**
- **Formula**
  - Allocation Editor R-71
  - Formula Editor R-67
  - Level I R-10
  - Level II R-15
- **Formula Editor**
  - And Operation R-67
  - Average R-67
  - Description R-67
  - Dialog R-66
  - Existing Formulas R-68
  - Existing Properties R-68
  - Formula R-67
  - Maximum R-67
  - Minimum R-67
  - Number of Results R-67
  - Or Operation R-67
  - Quantity R-67
  - Top input field R-67
  - Total R-67
- **Formula editor**
  - Transferred quantity R-67

**G**
- **Given Quantity**
  - Allocation Editor R-71
  - Condition R-55

**I**
- **Info**
  - Dialog R-54, R-63
- **Invert**
  - Condition R-54

**L**
- **Length**
  - Enter Value (Numeric) R-56

**M**
- **Master**
  - Quantity creator R-61
- **Maximum**
  - Formula Editor R-67
- **Menu**
  - Conditions-Author R-49
  - Quantity creator R-60
- **Minimum**
  - Formula Editor R-67

**N**
- **New Allocation**
  - Select Allocation R-69
- **New Condition**
  - Select Conditions R-47
- **New Formula**
  - Select Formula R-65
- **New Name**
  - Condition Name R-53
  - Quantity Name R-62
- **New Quantity**
  - Select Quantity R-58
- **New Value**
  - Enter Value (Numeric) R-56
- **No Allocation**
  - Select Allocation R-69
- **No Condition**
  - Select Conditions R-47
- **No Formula**
  - Select Formula R-65
- **No Quantity**
  - Select Quantity R-58
- **Normal**
  - Condition R-52

**O**
- **Old Name**
  - Condition Name R-53
  - Quantity Name R-62
- **Old Value**
  - Enter Value (Numeric) R-56
- **One**
  - Conditions - Editor R-50
- **Or Operation**
  - Formula Editor R-67

**P**
- **Parent**
  - Quantity Editor R-61

**Q**
- **Quantity**
  - Allocation Editor R-71
  - Formula Editor R-67
  - Level I R-14
  - Level II R-17
  - Level III R-18
- **Quantity creator**
  - Master R-61
  - Menu R-60
- **Quantity Editor**
  - AddUp R-61
  - All R-61
  - Anychild R-61
  - Bottom R-61
  - Child R-61
  - Dialog R-59
  - Parent R-61
  - Self R-61
  - Tool bar R-60
  - Up R-61
- **Quantity Name**
  - Dialog R-61
  - New Name R-62
  - Old Name R-62

**S**
- **Select Allocation**
  - Delete R-69
  - Description R-69
  - Dialog R-69
  - Edit R-69
  - Existing Allocations R-69
  - New Allocation R-69
  - No Allocation R-69
- **Select Conditions**
  - Delete R-47
  - Description R-47
  - Dialog R-46
  - Edit R-47
  - Existing Conditions R-46
  - New Condition R-47
  - No Condition R-47
- **Select Formula**
  - Delete R-65
  - Description R-65
  - Edit R-65
  - Existing Formulas R-65
  - New Formula R-65
  - No Formula R-65
- **Select Formulas**
  - Dialog R-64
- **Select Quantity**
  - Delete R-58
  - Description R-58
  - Dialog R-57
  - Existing Quantity R-58
  - New Quantity R-58
  - No Quantity R-58
- **Select quantity**
  - Edit R-58
- **Self**
  - Quantity Editor R-61

**T**
- **Text**
  - Enter Value (Numeric) R-56
- **Thickness Value**
  - Enter Value (Numeric) R-56
- **Tool bar**
  - Conditions-Author R-49
  - Quantity Editor R-60
- **Top input field**
  - Allocation Editor R-70
  - Condition R-51
  - Formula Editor R-67
- **Total**
  - Formula Editor R-67
- **Transferred quantity**
  - Formula editor R-67

**U**
- **Up**
  - Quantity Editor R-61

**V**
- **Value**
  - Condition R-52

