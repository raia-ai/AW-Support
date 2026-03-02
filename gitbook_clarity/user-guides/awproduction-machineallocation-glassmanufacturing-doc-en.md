---
description: "EN_AWProduction_Machinery_Allocation_2.10"
---


# A+W Machine Allocation D

---
## A+W Production
A+W - Software for Glass, Windows and Doors

## Introduction

This part of the documentation contains editorial notes.

### Revision Overview

| Machine Allocation Version / Date | Description |
| :--- | :--- |
| 2.10 / 11-2018 | New chapter regarding Machine type. Screenshots updated. |
| 2.02 / 01-2017 | Product and company names adjusted. |
| 2.01 / 01-2013 | Layout adjusted to CI 2013. |
| 2.00 / 09-2012 | Creation of tutorial, revision of software reference. |
| 1.00 / 01-2003 | Original version. |

### Editorial

The editorial contains the following themes:
- Notes on this document
- Copyrights
- Trademarks
- Contact

**Notes on this document**

This document is intended only for end users of A+W Production.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and is subject to changes without prior notice.

The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The descriptions in this document are based on the full program level of A+W Production.

### Copyrights

© 2018, A+W Software GmbH, all rights, including the right of reprint, production of copies and translation, are reserved.

The documentation must be copied, completely or in part, saved, or transferred only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH prior approval in writing.

### Trademarks

All hardware and software names mentioned in this documentation might also be registered trademarks or other property rights of third parties. The property rights of third parties must be observed.

### Contact

**A+W Software GmbH**
Am Pfahlgraben
D-35415 Pohlheim
📞 +49 6404 2051 0
📠 +49 6404 2051 877
✉️ aw.zentrale@a-w.com
🌐 http://www.a-w.com

## Contents

- **Introduction**
  - Revision Overview: D-3
  - Editorial: D-3
- **Tutorial**
  - Overview: D-9
    - Documentation: D-10
    - Tutorial Structure: D-10
    - Display Conventions: D-11
  - Basics: D-12
  - Machine Allocation: D-14
    - Machines: D-15
      - Machines and Machine Allocation: D-16
      - Machine Definition and Management: D-22
      - Definition and Editing of Machine Restrictions: D-26
      - Machines Exercises: D-32
    - Logical Machines: D-33
      - Machines and Machine Allocation: D-34
      - Definition and Management of Logical Machines: D-36
      - Logical Machines - Exercises: D-40
    - Work Processes: D-41
      - Work Processes and Machine Allocation: D-42
      - Work Process Definition and Management: D-49
      - Work Processes - Exercises: D-51
    - Allocation of Work Processes: D-52
      - Flexible Adaptation of Work Processes: D-53
      - Allocation of Work Processes and Logical Machines: D-58
      - Work Process Allocation - Exercises: D-62
    - Conditions, Formulas, Restrictions: D-63
      - Conditions and Formulas in Connection with Machine Allocation: D-64
      - Select a Condition: D-65
      - Select a Formula for the Processing Time of a Logical Machine: D-66
      - Selection of Conditions - Exercises: D-68
    - Processing Types and Processing Articles: D-69
      - Processing Types and Machine Allocation: D-70
      - Processing Articles and Machinery Allocation: D-71
      - Definition and Management of Processing Types: D-73
      - Definition and Management of Processing Articles: D-76
      - Machine Allocation - Exercises: D-80
    - Machine Allocation - Buttons: D-81
- **Software Reference**
  - Machine Allocation: D-85
  - MA Editor: D-86
    - MA Editor - Machines: D-87
    - MA Editor - Logical Machines: D-88
    - MA Editor - Work Processes: D-90
    - MA Editor - Work Process Allocation: D-91
    - MA Editor - Machine Types: D-93
  - New Machine: D-94
  - Machine: D-95
  - Dimension Restrictions: D-100
  - Spacer Restrictions: D-101
  - Select a Condition: D-102
  - New Logical Machine: D-103
  - Logical Machine: D-104
  - Formula Selection: D-106
  - New Work Process: D-107
  - Work Process: D-108
  - New Machine Type: D-110
  - Machine Type: D-111
  - Machine Allocation - Formulas: D-113
    - Select Conditions: D-114
    - Condition Editor (Graphic Version): D-115
    - New Condition: D-117
    - Info (about the new condition): D-117
    - Select quantity: D-118
    - Condition Editor (Text Version): D-119
    - Formula Editor: D-120
  - Processings in Machine Allocation: D-122
    - Processing Types: D-123
    - Processing Articles: D-125
  - Adjust Columns: D-128
  - Column Definition: D-129
- **Section Index**: D-131

# Tutorial

## Overview

The tutorial on the Machine Allocation (MA) module deals with the allocation of machines in A+W Production. Machine allocation assigns the scheduled processing steps to the individual machines, taking into account machine restrictions and instructions for production control. Check programs provided by the machine manufacturers can be used in A+W Production to see whether the processes are plausible.

> **The functions depend on the released modules**
> Please note that the individual functions are available only if the corresponding modules and interfaces have been installed and released.
> If you detect functions in this description which are not available in your version, please contact A+W Software GmbH.

### Prerequisite knowledge

This tutorial is meant for persons in charge of production scheduling in A+W Production who are responsible for organizing the optimum production process. Participants must be familiar with the master data concept in A+W Production.

### Documentation

The following documents are available on module Machine Allocation:

**PDF**
- Complete documentation
- Tutorial
- Software reference
- Index

**Online help <F1>**
- Context-sensitive dialog help

### Tutorial Structure

This tutorial consists of subjects with several training modules each. Each session consists of the following elements:

- **Overview**: Each training session starts with an overview of the major topics:
  - Objectives: What shall be conveyed?
  - Benefit: What can this knowledge be used for?
  - Maxims: Which correlations are to be remembered?

- **Concepts**: Concepts and terms of the corresponding training session will be explained first. This is followed by examples and operating instructions.

- **Exercises**: There are exercises featuring special tasks for some of the training sessions.

### Display Conventions

Certain parts of the sentences are specially marked. Their meanings are:

| Convention | Meaning |
| :--- | :--- |
| *Italics* | mark character strings describing software elements, e.g. the dialog *New machine*. |
| **Bold** | marks character strings to be entered via keyboard, e.g. **Enter 0**. |
| `>` | shows the way to open a dialog, e.g. Master data > MA > MA editor > Machines > New. |
| `[]` | Square brackets mark the buttons in the dialog, e.g. [OK] to save the data. |
| `<>` | Pointed brackets refer to keys or shortcuts on the keyboard, e.g. `<F1>` is used to open the online help. |

### Reading instructions

The contents of a training session are based on the knowledge conveyed in the previous session. We therefore recommend not to skip any session.

If you are already familiar with a subject you should at least read the summary at the beginning of the session in order to bring the main details to mind.

## Basics

The machine allocation depicts the references between work processes and machine. Based on the machines and the work processes, the capacity planning can schedule the orders optimally.

To set up the master data, the following questions must be answered:
- What task must be performed by the processing on a lite of an order: **What** must be done.
- What method will be used: **How** will this be done.
- What tool will be used: **Where** will the processing be performed.
- Which ranking and restrictions have to be adhered to: **Why or when** will the machine be used.

**Figure D-1: Elements of machine allocation.**
This figure shows the software elements belonging to machine allocation and how they are connected.
- **Restrictions, formulas**: e.g. minimum thickness 2 mm
- **Properties**: e.g. registration point 180, cost center 25
- **Machine type**: e.g. cutting -> **Machine**: e.g. cutting table 8
- **Formulas**: e.g. is a shape -> **Logical machine**: e.g. logical cutting table 8
- **Processing article**: e.g. float cutting -> **Processing type**: e.g. cutting -> **Work process**: e.g. IG cutting
- All these elements connect through **Allocation of work** which is issued by **A+W Production**.

Machines are defined by a Machine type, Properties, and Restrictions. In the above example, cutting table 8 is allocated to machine type *Cutting*.

One of the properties of cutting table 8 is that it is allocated to registration point 180 and cost center 25. The logical machine for cutting table 8 is called logical cutting table 8. It has been assigned the formula *Is a shape*.

### Description of the work processes

Using the work processes, the material streams in production are divided up and can be handled separately. Work processes therefore have to be regarded first.

For the set-up of the work processes, the following questions are considered:
- Which processings can be combined and which may not be combined?
- Are there processings that are performed but that do not appear in the BOM?
- Are there different material streams, e.g. series lites, bathroom mirrors, RV lites that make very individual ways through production and therefore should be distinguished early on?
- Are there work processes that are not performed here, e.g. sand blasting at the other end of the city?

### Description of the machines

In that the machines are described precisely, it is guaranteed that lites to be produced find valid machines. Here, there is a distinction between physical restrictions and logical machines with additional restrictions, cost rates and transition times.

Added to the list of machines are places that are not machines in the usual sense but that are relevant for production, e.g. warehouse, incoming goods, shipping warehouse, loading ramp, additional production locations.

### Description of the logical machine

Logical machines are used to express different transition times, cost rates or processing durations in the capacity planning. As a guideline, you can set up a logical machine if a machine can be used in different operating modes.

## Machine Allocation

This chapter tells you which sections of A+W Production are part of machine allocation (MA) and how to allocate the machines.

The MA editor is used to manage machines, logical machines, and processes as well as their allocations and properties.

Machine allocation includes the following chapters:
- "Machines" on page D-15
- "Logical Machines" on page D-33
- "Work Processes" on page D-41
- "Allocation of Work Processes" on page D-52
- "Conditions, Formulas, Restrictions" on page D-63
- "Processing Types and Processing Articles" on page D-69

The following sessions will familiarize you with the machines, logical machines, processes, and allocation of processes. This knowledge will be deepened later on when we will be dealing with processing types and the selection of formulas.

### Machines

**Objectives**
- The meaning of machines in A+W Production and especially in the context of machine allocation.
- How to manage, define, edit, or delete machines.
- The use of meaningful names and numbers.

**Benefit**
- Machines represent the physical machinery. Machines are therefore the basis for production control.

**Note**
- **Machines**: Machines represent the physical machinery. Names and numbers are systematically assigned in A+W Production.
- **Machine types**: Machine types are already defined in A+W Production and are allocated to the machines. Machine types define the type of machine, e.g. cutting, spacer bender or Others.
- **Relations**: AND-/OR relations are the operators by which restrictions, conditions, and formulas are linked in A+W Production.
- **Cuts**: Z- and W cuts are more complex cuts which can be allocated an additional cost factor, Costs per Z cut.

> **Prerequisite**
> To define a machine in A+W Production, the suitable machine type must be defined first. The machine type is selected in dialog *New machine*.
> If the corresponding machine type is not available in dialog *New machine* please contact A+W Software GmbH.

#### Machines and Machine Allocation

This session shows you how to reflect your machinery in A+W Production and the properties of the machines.

*(Image: Fig. D-2 MA editor - Machines. Shows the list of physical machines in the Machinery Allocation Editor.)*

Tab *Machines* lists all physical machines. Tab *Machines* therefore reflects your actual machinery.

Each machine can be identified uniquely with an ID. For each machine, there is a registration point for the recording of the production data collection (PDC). You assign each machine a machine type that specifies what kind it is, for example *Cutting*, *CNC Center* or *muntin construction*. The machines types are permanently defined and cannot be changed. A+W Production automatically creates a logical machine for every machine.

That is, for each machine that actually exists in your plant, you must create a machine in A+W Production and define its properties.

*(Image: Fig. D-3 Machines in A+W Production. Diagram showing how physical machinery (e.g., Cutting table 1, CNC machine 1) is represented as software entities in A+W Production.)*

In this example, no machine is created in A+W Production for drilling machine 2. Thus, the machine is not known to the software and it also cannot be controlled.

**Machine properties**

For each machine created in A+W Production, the following properties of the machine must be specified.
- **Manual operation**: Identifier for machines that do not have automatic loading equipment. This identification prevents, among other things, that using the manual processing time there is a split or that items are automatically scheduled on manual cutting tables.
- **Individual processing**: Identifier for machines whose processings may not be combined, e.g.
  - drillings = 0: for two drillings on the same machine, two dates are not determined.
  - Screen printing or coatings = 1: for two coatings, two different dates are not determined, even if they are done on the same machine.
- **Minimum size**: Minimum dimensions for a lite that can be produced on the machine, e.g. without falling through the rollers. If you can place small lites on a larger lite, e.g. to print them, do not specify the size restriction on the machine, but on the logical machine, e.g. as screen printing with carrier lite.
- **Maximum size**: Maximum dimensions for a lite that can be produced on the machine because it exceeds the width of the guide rails, the furnace width or the ceiling height. If you can produce larger lites by unscrewing the side walls on the processing center and setting up spray protection, for example, do not specify the size restriction on the machine, but on the logical machine, e.g. as processing center for extra-large sizes.
- **Thicknesses**: Thickness range in which the machine can work. Other thicknesses cannot be processed on the machine, e.g. because 3 mm is not supported reliably and the guides are too narrow for 15 mm. If a 15 mm lite can be produced by reconstructing the machine, do not place the size restriction on the machine, but on the logical machine, e.g. grinding machine for thick glass.
- **Shapes**: Specification whether the machine can produce only rectangles, only shapes or both. Consider, for example, that free shapes or arcs cannot be produced, e.g. for LG cutting.
- **Weight**: Maximum weight of a lite for which the machine is approved. In order to express that the machine can process the weight but there must be a second employee ready for handling, enter the restriction for the logical machines, e.g. one-sider with two people.

> **Delete machine**
> Deleting a machine can affect your production! Before you delete a machine, always make sure that it is no longer used on the shop floor.

**Assigning names, IDs, and numbers**

For machines of the same type, assign IDs in the same range of hundreds, e.g. for all cutting tables IDs from 100 to 199. Cutting tables are therefore easily recognizable on the list. If you have no special number areas for machines, use the numbering pattern of operational data collection as a guideline.

Always use the same names for machines of the same type, numbering them all the way through; the eighth cutting table at your plant will therefore be called Cutting table 8.

**Machine restrictions**

Depending on their construction, machines can have different restrictions, e.g. being able to process lites only up to a certain size. The restrictions of the individual machines can be edited in dialog *Machine*.

Restrictions available in dialog *Machine*:
- Minimum thickness
- Maximum thickness
- Shapes
- Coated glass
- Patterned glass
- Stepped IG
- Dimensions
- AIR

If there are machines which come with further restrictions, additional conditions have to be used to define these restrictions. These conditions can also contain formulas.
(See "Conditions and Formulas in Connection with Machine Allocation" on page D-64)

Below are some examples of restrictions available in dialog *Machine*.

- **Example: Restriction thickness**
  - If the machine can process only lites from a thickness of 8 mm upwards, enter the restriction *minimum thickness 8 mm*.
  - If the machine can process only lites up to a thickness of 15 mm, enter the restriction *maximum thickness 15 mm*.

- **Example: Restriction Shapes**
  - No restriction: the machine can process shapes and rectangles, which is the case for modern cutting tables.
  - The machine can only process shapes, e.g. to prevent rectangular lites from being transferred to a CNC center for grinding.
  - The machine cannot process shapes but only rectangles which is the case for grinding/drilling lines.

- **Example: Restriction Coated glass**
  - No restriction: the machine can process coated and uncoated lites.
  - The machine can only process coated glass.
  - The machine can only process uncoated glass.

- **Example: Restriction Patterned glass**
  - No restriction: the machine can process patterned glass and glass without patterns.
  - The machine can only process patterned glass.
  - The machine can only process glass without a pattern.

- **Example: Restriction Stepped IG**
  - No restriction: the machine can process stepped IG and common IG.
  - The machine can only process stepped IG.
  - The machine can only process common IG.

**Size restrictions and lite format**

You can define the minimum and maximum size of lites to be processed by a machine. You should use the machine's direction of movement as a guideline. The entries for the *Width* and *Height* only serve as landmarks; you can also process lites the width and height of which have been exchanged. The lite must be aligned by hand on the machine in this case.

**Spacer restrictions**

This defines whether the machine can process common IG with one spacer or multiple IG with two spacers. A minimum and a maximum value can be entered for every spacer.

**AND-/OR relations**

When defining the machine restrictions you have to enter them as logical relations (AND/OR). These are basic relations in the Boolean algebra which serve to show logical relations.
- **AND relation**: If two (or more) statements apply, a statement is true. Example: A machine can process only lites which are wider than 150 mm and higher than 200 mm. It follows that: Width >= 150 mm AND height >= 200 mm.
- **OR relation**: If one or the other statement applies, the statement is true. Example: A machine can process only lites which are wider than 150 mm or shorter than 3500 mm. It follows that: Width >= 150 mm OR length <= 3500 mm.

**Element ID**

The element ID is only used for the machine types *Line*, *Cutting*, and *Bender*. The element ID can be used to distinguish lines, tables, or benders if there are several machines of the same type. The tables 1, 2, and 3 for example could get the element IDs TB1, TB2, and TB3. The element ID defines the format in which the NC code is issued.

**Additional conditions**

Additional conditions seriously influence the behavior and the properties of machines. If an additional condition is defined, you have to understand its consequences.

#### Machine Definition and Management

This session will show you how to define new machines and edit or delete existing ones. After entering a machine you have to edit the machine data.

> **Prerequisite**
> A new machine can only be entered if a suitable machine type has been defined, e. g. *Cutting*, *CNC center*, *Spacer bender*, *Others*. The machine type catalog is predefined in A+W Production. It appears in a combo box when you enter a new machine.

**How to define a machine**

1.  Go to **Master data > MA > MA editor > Machines > [New]**.
    *(Image: 'New machine' dialog box)*
2.  Enter an ID from the number area intended for this machine type, e.g. **180**.
3.  Enter a name which clearly describes the machine, e.g. **Cutting table 8**.
4.  Choose the appropriate machine type, e.g *Cutting*.
5.  Enter an element ID, e.g. **TB8**.
    You have to enter an element ID for the machine types *Line*, *Table*, or *Bender*. This allows to recognize the machines should there be several of the same type.
    *(Image: Fig. D-4 Example for a new machine dialog filled out)*
6.  Click on [OK] to save the data.
    With that, you have entered a new machine. It will appear on the list of *Machines* in the MA Editor dialog. You have to define properties and allocations to describe the machine in detail.

**How to enter the machine's properties**

1.  Go to **Master data > MA > MA editor > Machines**.
    *(Image: Fig. D-5 MA editor - Machines tab)*
2.  Select the machine you want to edit.
3.  Click on the [Edit].
    *(Image: Fig. D-6 Machine properties dialog with 'General properties' and a 'Combo box' highlighted.)*
4.  Add the General properties (A). When you click on a field you can select data from the combo box (B). The restrictions in the bottom part of the dialog can be completed later.
5.  Confirm by [OK]. With that, you have defined the machine master data. Machine restrictions will be introduced in a special session. (See "Definition and Editing of Machine Restrictions" on page D-26)

**How to delete a machine**

> **Delete machines**
> Deleting machines in A+W Production can affect your production. Before you delete a machine, always make sure that it is no longer used.

1.  Go to **Master data > MA > MA editor > Machines**.
2.  Tag the machine you want to delete.
3.  Click on [Delete]. A security query appears.
4.  Confirm this security query by [Yes] to delete the machine once and for all. The machine data will be deleted.

#### Definition and Editing of Machine Restrictions

In this unit, you will learn how to specify the restrictions for a machine.

> **Restrictions and additional condition at the same time**
> Active restrictions in connection with the selection of a formula can cause a conflict. Restrictions can neutralize each other. In case of questions please contact the A+W Software GmbH support team.

**How to edit restrictions regarding the thickness**

1.  Go to **Master data > MA > MA editor > Machines**.
    *(Image: Fig. D-7 MA editor - Machines tab)*
2.  Select the machine you want to edit.
3.  Click on [Edit].
    *(Image: Fig. D-8 Restriction - edit thickness dialog)*
4.  Double-click on [...] (B) to open the input field.
5.  Click on the [Arrow] to enter the value for the minimum thickness.
6.  Enter the minimum thickness in millimeters.
7.  Click on [OK] to save the value. With that, you have changed the minimum thickness for the machine.
8.  Repeat the steps 4 to 7 to edit the restrictions for the maximum thickness.

**How to edit the restrictions for shapes, coated glass, patterned glass, and stepped IG**

1.  Go to **Master data > MA > MA editor > Machines**.
2.  Select the machine you want to edit.
3.  Click on [Edit].
    *(Image: Fig. D-9 Restriction - edit shapes dialog)*
4.  Double-click on [...] after *Shapes*. An [Arrow] appears.
5.  Click on the [Arrow] (B) to activate shapes.
    *(Image: Fig. D-10 Shape restrictions, combinations of checkboxes)*
6.  Choose the required combination of checkboxes to define the restriction:
    - No restriction (A, B)
    - No shapes (C, D)
    - No rectangles (E, F)
7.  Click on the [OK] button to save the shape restrictions.
8.  Edit the restrictions for *coated glass*, *patterned glass*, and *stepped IG* in the same way.

**How to edit the restrictions for sizes and spacers**

> **Restrictions will be deleted irrevocably**
> Dimension restrictions are deleted permanently and without security query if you click the [cross].

1.  Go to **Master data > MA > MA editor > Machines**.
2.  Select the machine you want to edit.
3.  Click on [Edit].
    *(Image: Fig. D-11 Restrictions – Edit sizes dialog)*
4.  Click on the [Pen icon] in field *Dimensions* to open the *Size restrictions* dialog.
    *(Image: 'Dimension Restrictions' dialog)*
5.  Check the checkboxes of the input fields you want to edit.
6.  Fill in the input fields.
7.  Click on [OK] to save the amended size restrictions. The restriction is shown in field *Dimensions* as AND/OR relations.
8.  Edit the spacer restrictions in the same way.

**How to remove the size and spacer restrictions**

> **Deletion of size restrictions**
> Dimension restrictions are deleted permanently and without security query if you click the [cross].

1.  Go to **Master data > MA > MA editor > Machines**.
2.  Select the machine you want to edit.
3.  Click on [Edit]. Dialog *Machine* appears.
4.  Click in the *Dimensions* area on [X] to remove a restriction.
5.  Click on [OK] to save the changes.
6.  Delete the spacer restrictions in the same way.

#### Machines Exercises

The following exercises shall help to strengthen your newly acquired knowledge.
- Take a piece and paper and sketch your factory's machinery.
- Note which machines belong to which machine type.
- Systematically assign IDs to the machines (number ranges).
- Note the properties which apply to the machines and whether there are restrictions:
  - Are there restrictions like e.g. minimum thickness, maximum thickness, or size restrictions.
  - Can the machine process IG or triple IG? Where must these entries be made?
- Enter the machines as exercise machines in A+W Production and amend them to match your machinery.
- Keep those test machines as a basis for further exercises.

**Additional information**
- Software Reference, "New Machine" auf Seite D-94
- Software Reference, "Machine" auf Seite D-95
- Software Reference, "Dimension Restrictions" auf Seite D-100
- Software Reference, "Spacer Restrictions" auf Seite D-101

### Logical Machines

**Objectives**
- The meaning of logical machines in A+W Production and especially in the context of machine allocation.
- Why do logical machines exist?
- How to assign names and numbers.
- How to manage, define, edit, or delete logical machines.
- When can logical machines be deleted, and when not?

**Benefit**
- Logical machines represent one machine function. If a machine can be used for drilling and edgework, two logical machines will be created for this machine in A+W Production. In the next step, a process can be allocated to the machine function.
- Among other things, A+W Production barcoding (production data collection) analyses data of the logical machines, e.g. for statistics.

**Note**
- **Logical machines**: Logical machines represent a function of a real machine. Logical machines are used for production control and cost calculation. Logical machines are used for production data collection. When you enter a machine, a logical machine will be created automatically. Any number of logical machines can be defined for one (physical) machine.
- **Allocation**: Logical machines are allocated to processes.

#### Machines and Machine Allocation

Logical machines represent one function of a real machine. The properties of the machine are applied to the logical machine. The properties of the logical machine are valid in addition to the properties of the (real) machine.

*(Image: Fig. D-12 Logical machines tab in the Machinery Allocation Editor.)*

Logical machines are used for:
- Describing individual machine functions.
- Allocating processes.
- Prioritizing processes.
- Capacity planning and rescheduling.
- Logical machines distinguish individual machine functions. Thus, e.g. different rates or transition times can be defined for a machine.
- Statistical evaluations.

**Example**
You have a CNC machine that can drill, grind, and polish. Define the machine as CNC machine 1. A+W Production automatically creates a logical machine. Since the CNC machine has three functions, three logical machines will be defined.
Define this machine and enter the master data for Drilling. Now define two more logical machines for CNC machine 1; for one of them, enter the master data for Grinding and for the other, the master data for Polishing.

*(Image: Fig. D-13 Example: Three logical machines result from one CNC center. A diagram shows a 'Real CNC machine' with functions for drilling, grinding, and polishing branching into three separate 'Logical CNC machines' for each function.)*

The processing times that a logical machine requires for its allocated work process are defined as formula in the capacity planning. For this, the separate documentation for the *Capacity planning* part is available.

#### Definition and Management of Logical Machines

This part of the tutorial will show you how to define new logical machines and edit or delete existing ones.

> **Prerequisite**
> You can define logical machines only after you have entered the corresponding (real) machine.

**How to define a logical machine**

1.  Go to **Master data > MA > MA editor > Logical machines**.
    *(Image: Fig. D-14 Logical machine selected in the editor.)*
    A+W Production automatically creates a logical machine for every machine. All additional logical machines can only be defined based on the existing one.
2.  Select the logical machine that shall be used as a basis for the new logical machine.
3.  Click on [New].
4.  Enter the ID and the name.
    *(Image: 'New logical machine' dialog box.)*
5.  Click on [OK] to save the data.
    *(Image: Fig. D-15 New logical machine now appearing in the list.)*
    With that, you have entered a new logical machine. The new logical machine is listed on tab *Logical machines* in the MA editor. You can now edit the properties of the new logical machine.

**How to edit a logical machine**

1.  Go to **Master data > MA > MA editor > Logical machines**. Tab *Logical machines* appears in the MA editor.
2.  Select the logical machine you want to edit.
3.  Click on [Edit].
    *(Image: Fig. D-16 Logical machine - properties dialog.)*
4.  Enter the data for the logical machine, e.g. for a cutting table.
5.  Click on [OK] to save the data. With this, you have defined the master data for the logical machine.

**How to delete a logical machine**

> **Delete logical machines**
> A+W Production automatically creates a logical machine for every machine defined. This automatically created logical machine cannot be deleted. When a machine is deleted, all related logical machines will be automatically deleted too.
> If you delete a logical machine, you delete the function of a machine. This can cause significant problems in the production process. Make sure that the logical machine and the machine are not used in production before you delete them.

1.  Go to **Master data > MA > MA editor > Logical machines**.
2.  Select the logical machine you want to delete.
3.  Click on [Delete]. A security query appears.
4.  Confirm this security query by [Yes] to delete the logical machine once and for all. The data will be deleted.

#### Logical Machines - Exercises

The following exercises shall help to strengthen your newly acquired knowledge.
- Define the exercise machines representing the machinery in your factory or use the exercise machines from the previous session.
  - Note the processes that can be executed by the individual machines, e. g. drilling, grinding, arrissing.
  - Create the appropriate logical machines.
- A toughening furnace can toughen and semi-toughen the lites. Would you create different logical machines for the two functions? List the benefits and disadvantages.

**Additional information**
- "Machines Exercises" on page D-32
- Software Reference, "New Logical Machine" auf Seite D-103
- Software Reference, "Logical Machine" auf Seite D-104

### Work Processes

**Objectives**
- The meaning of work processes in the context of machinery allocation.
- How to manage, define, edit, or delete work processes.
- Why work processes have priorities, and how they can be changed.
- The relation between work processes, processing types and articles?

**Benefit**
- A work process fulfils the request to perform a processing step defined in the bill of materials. This requested process may be polishing or grinding. Based on this request, the work process defines the special type of polishing or grinding.
- The level of the logical machine establishes the connection between the work process and the physical machine which is to perform the work process.

**Note**
- **Work processes**: Work processes bring together the properties of processing type, like e.g. *Cutting* with the properties of the work piece. Work processes are based on processing types or articles.
- **Conditions/formulas**: Conditions/formulas can also be used to define work processes.

#### Work Processes and Machine Allocation

A work process is defined by a processing type, a processing article, an article group, and/or an additional condition.
(See "Processing Types and Processing Articles" on page D-69)

*(Image: Fig. D-17 Work processes list in the Machinery Allocation Editor.)*

If a processing type has been defined for a work process, e.g. *Cutting*, this describes the technical type of processing for this work process. We recommend using the standard A+W Software GmbH processing type catalog for defining work processes.

Only create your own processing types if there are no appropriate pre-defined processing types. You create separate work processes if you can make statements about your production, e.g.:
- You combine screen printing in dark colors on a particular day of the week because you then dispose of the solvent (possible campaign planning).
- The thick lites are ground on machine 1. The thin lites on machine 2, but they serve one another as substitute machine (selection of the tool).
- Series lites may only be drilled on the automatic drilling line. If it breaks down, you must shift the delivery date.

The work process *pseudo-processing* stands for processings in the BOM that have an informative character, e.g. *do not stamp*, *use gloves*, *heed tolerance*. So that no scheduling is done for these processings, they are scheduled on a machine *Dummy for informative processings*, which has no PDC registration point and thus also no shift plan.

**Processing items on work process**

If a processing type has been defined for a work process, e.g. *Shape cutting for laminated glass*, you can set off the processing of laminated glass shapes from the processing of other shapes even before the actual machinery allocation.

*(Image: Fig. D-18 Work process – article restriction options dialog.)*

You can specify the work process even further by additionally choosing a restriction in field *Article*. The *Article type* (A) is predefined by A+W Software GmbH. It includes basic articles, e. g. *toughened glass*, *laminated glass*, and *Muntins*.

If you select e.g. the processing type *Cutting* and also the article *Toughened glass*, you define a work process for the cutting of toughened glass.

The *Article group* (B) can be used to choose a production article group you have defined before. For the processing type *Cutting* for example, you can choose the article group *Glass doors*. This way, you have defined a work process for the cutting of glass doors.

Select an *Article* (C) to allocate a work process to a special article. Enter e. g. for a work process the processing type *Cutting* and the article *Float 6 mm* to define a work process for the cutting of 6 mm float glass.

> **Processing types**
> There is a special session on processing types: "Processing Types and Processing Articles" on page D-69

*(Image: Fig. D-19 Examples of differently defined work processes. Diagram shows 'Work process for cutting', 'Work process for toughened glass cutting', and 'Work process for Float 6 mm cutting'.)*

**Exact definition of work processes**

Use the options in dialog *Work process* in field *Article* for a detailed definition of work processes.

- **Example 1:** Laminated glass can only be cut on cutting tables that have two heads or use other technologies like e.g. Waterjet. The work process *Cutting* has already been defined for float glass cutting. Define a new work process for laminated glass cutting. Select processing type *Cutting* glass type *LAMI*. This defines a work process that takes into account the peculiarities of laminated glass cutting and which can only be allocated logical machines which can perform this type of processing.

- **Example 2, option Article group:** Certain articles are produced only infrequently. To handle this case, define an article group that includes these rare articles, then start a campaign. Since campaign planning is based on a work process, choose the article group containing rare articles for this campaign. You can thus plan when and how those rarely occurring articles shall be produced. Campaigns are described in detail in section *Capacity planning*.

**Non-allocated work processes**

A work process is shown in red until it is assigned a logical machine. Always allocate a logical machine to the work processes. If the corresponding logical machine has not been defined yet you should allocate *Dummy* as a logical machine.
(See "Allocation of Work Processes" on page D-52)

**Priority of work processes**

Work processes can be moved upwards or downwards on the list. For allocating work processes, the list is processed from top to bottom. A work process will be allocated if all conditions allocated to work process are met. The priority allocated to specialized work processes must therefore always be higher than the priority allocated to unspecialized work processes.

**Several work processes for the same lite**

You have got an order for a glass door. This requires the work processes *Rectangular grinding*, *Drilling*, and *Cut-outs*.

Instead of using the more cost-effective rectangular grinding machine for grinding, all three work processes can be performed by the CNC center. This makes the single work process *Rectangular grinding* expensive but it saves time because all three processes can be executed on one machine, right after another.

You have defined the work process *Rectangular grinding on CNC center* for this purpose, to which you have allocated the logical machine *CNC center rectangular grinding*, with high priority.
To avoid bottlenecks, the work process *Rectangular grinding on CNC center* is also allocated to the logical machine *Rectangular grinding machine*, with low priority.

**Additional conditions in work processes**

Work processes are not exclusively linked to processing steps. They can also include additional conditions. A condition can be for example: *This work process is executed on the CNC center*. When you define the work process you can therefore define the machinery to be used with priority.

An additional condition can also check the bill of materials. Defining such a condition can therefore be used to control the lite's progress on the shop floor. The condition could be for instance: If the lite's bill of material includes the processing steps *Grinding*, *Drilling*, and *Cut-out*, the lite shall be completely produced on the CNC center.

*(Image: Fig. D-20 Example: An additional condition in the work process queries the bill of material.)*

The example shows another way of controlling the lite's progress on the shop floor, a work process allocation based on a processing article.

Define the processing article *Glass door* for example. The processing article *Glass door* is executed by the work process *Glass door*, and the work process *Glass door* includes the condition that it is produced on the CNC center.

*(Image: Fig. D-21 Example: Work process allocation based on a processing article.)*

- **Example: Bottleneck because of an additional condition**
  The condition defined for the work process *Glass door* says that glass doors are produced on the CNC center. The condition can either refer to the bill of material, or to a processing article.
  If there is another order in addition to the order for glass doors, this time e.g. including shapes, there is going to be a bottleneck at the CNC center.
  **Solution**: Change the priority of the logical machine CNC center so that the CNC center is no longer the first choice for glass doors. This means that glass doors are not produced on the CNC center but in individual steps on the rectangular grinding machine, the automatic drill, and the cutting table for cut-outs. While this increases the handling effort for the glass doors it permits to produce the shapes on the CNC center at the same time. When the bottleneck has been resolved, the original priorities for the logical machines must be restored.

Work processes can also be defined for a processing article which makes sense for instance if you want to explicitly add a processing step to the bill of material.

- **Example: Work process based on processing articles**
  A TG has been coated after which it must be handled with gloves.
  In this case, define the processing article *Wear gloves!* and choose it as the basis for this work process. In work process allocation, allocate this work process to the logical machine *Dummy*.
  This way, you have introduced a work process that does not run on any machine but exists on the shop floor as *handle coated TG with gloves*.

> **Work process based on processing article only as an exception**
> Work processes based on processing articles are an exception because you have to complete and maintain the work process allocation in order to add new processing articles. The definition of work processes based on processing articles makes sense only in exceptional cases, like the above example.

#### Work Process Definition and Management

This session shows you how to define and edit new work processes, and who to delete them from the list.

> **IDs for work processes**
> Always allocate to a work process the ID of the processing and/or item, multiplied by 10.
> Example: The work process is based on the processing step *Arrissing* (ID 1000) from the standard processing catalog. In this case, allocate the new work process the ID 100000. With this system, it is easy to keep processings, items and work processes apart, but the fact that they belong together is still apparent.

**How to define a work process**

1.  Go to **Master data > MA > MA editor > Work processes > [New]**. Dialog *New work process* appears.
2.  Enter the data.
    *(Image: Fig. D-22 New work process dialog.)*
3.  Click on [OK] to save the data. Dialog *New work process* appears to edit the restrictions.

> **Work processes in red**
> In the MA editor, a work process is shown in red until it is assigned a logical machine. Always allocate a logical machine to the work processes. If the corresponding logical machine has not been defined yet you should allocate *Dummy* as a logical machine.

**This is how to edit the restrictions for a work process**

1.  Go to **Master data > MA > MA editor > Work processes**. Tab *Work processes* appears.
2.  Select the work process you want to edit.
3.  Click on [Edit].
    *(Image: Fig. D-23 Work process - edit restrictions dialog.)*
4.  Select the necessary options and corresponding types or articles to define the work process. You have edited the work process.
5.  Click on [OK] to save the data.

**How to delete a work process**

1.  Go to **Master data > MA > MA editor > Work processes**. Tab *Work processes* appears.
2.  Select the work process to be deleted. A work process is shown in red in the MA editor until it is assigned a logical machine.
3.  Click on [Delete]. A security query appears.
4.  Click on [Yes] to delete the work process for good. The data will be deleted.

#### Work Processes - Exercises

The following exercises shall help to strengthen your newly acquired knowledge.
- Define the exercise machines and the logical machines representing the machinery in your factory or use the exercise machines and logical exercise machines from the previous sessions.
  - "Machines Exercises" on page D-32
  - "Logical Machines - Exercises" on page D-40
  - Define an exercise work process *Polishing* based on the standard processing catalog.
  - Define the exercise work process *handle coated toughened lites with gloves*. The work process shall be based on a processing article.
  - Define the exercise work process *Laminated glass cutting* based on the standard processing catalog; use an article to define it in closer detail.
- Take a piece of paper and sketch your factory's machinery, then list the resulting logical machines. Look at the orders on hand: Which work processes have to be defined in this situation?

**Additional information**
- Software Reference, "New Work Process" auf Seite D-107
- Software Reference, "Work Process" auf Seite D-108

### Allocation of Work Processes

**Objectives**
- Introducing and understanding work process allocation
- Allocating work processes
- Resolving allocations
- Changing the priority of logical machines
- The use of defining priorities for logical machines

**Benefit**
- Work process allocation serves to allocate logical machines to work processes. Clever allocation will help to optimize the production costs.

**Note**
- **Allocation of work processes**: Work process allocation links logical machines and work processes.
- **Priorities**: Work process allocation serves to define the priorities of logical machines. You therefore define that the specified work process shall be performed on the optimal machine, as cost-effective as possible.
- **Allocation of work processes**: Work process allocation allows the user to intervene in the production process.

#### Flexible Adaptation of Work Processes

Logical machines are allocated to work processes. The sequence, and thus the priority of the logical machines, can be individually defined for every work process. You therefore define the priorities of machines in the production process.

Work processes tend to be allocated to machines that can perform several functions like the CNC center for instance, rather than being allocated to more specialized machines which can perform just one function. As a result, more work processes are allocated to the expensive CNC center which will cause a bottleneck sooner or later.

This can be prevented by defining priorities in the allocation of work processes, and by defining flexibly adaptable work processes.

Define work processes which exactly reflect the individual applications, and allocate these work processes to suitable logical machines. This makes sure that the work processes will be performed by the most cost-effective machine.

**Condition in a work process**

Work processes can include additional conditions. When you define the work process you can therefore define the machinery to be used with priority.

An additional condition can also check the bill of materials. The condition could be for instance: If the lite's bill of material includes the processing steps *Grinding*, *Drilling*, and *Cut-out*, the lite shall be completely produced on the CNC center. Defining such a condition can therefore be used to control the lite's progress on the shop floor.

> **Always allocate work processes**
> A work process is shown in red until it is assigned a logical machine. Always allocate a logical machine to the work processes. If the corresponding logical machine has not been defined yet you should allocate *Dummy* as a logical machine.

*(Image: Fig. D-24 Example: An additional condition in the work process queries the bill of material.)*
*(Image: Fig. D-25 Example: Work process allocation based on a processing article.)*

*(Image: Fig. D-26 Example: Flexibly adapted work process allocation with newly defined work processes highlighted.)*

**Example: Flexibly adapted work process allocation**
You have got a rectangular grinding machine and a CNC center on your shop floor. Both can execute the processing step *Grinding*.
- The list of work processes includes the work process *Rectangular grinding* which is used for all rectangular lites. In work process allocation, the work process *Rectangular grinding* is allocated to the *Rectangular grinder*. It has got top priority.
- The list of work processes includes the work process *Shape grinding* which is used for all shapes. In work process allocation, the work process *Shape grinding* is allocated to the CNC center.
- The CNC center is also allocated to the work process *Rectangular grinding*, albeit with a lower priority.
With these settings, rectangular lites will be ground by the more cost-effective rectangular grinder. In case of a bottleneck, rectangular lites will also be ground by the CNC center.

*(Image: Fig. D-27 Example: Flexibly adapted work process allocation, showing work processes for Rectangular and Shape grinding.)*

If a lite is to undergo several work processes, it may be reasonable to accept slightly higher costs for a single work process. The number of lites to be produced is usually the crucial factor.

- **Example: Several work processes for the same lite**
  To produce a glass door the work processes *Rectangular grinding*, *Drilling*, and *Cut-outs* are required. Instead of using the more cost-effective rectangular grinding machine for grinding, all three work processes can be performed by the CNC center. This makes the single work process *Rectangular grinding* expensive but it saves time because all three processes can be executed on one machine, right after another.
  You have defined the work process *Rectangular grinding on CNC center* for this purpose, to which you have allocated the logical machine *CNC center rectangular grinding*, with high priority. To avoid bottlenecks, the work process *Rectangular grinding on CNC center* is also allocated to the logical machine *Rectangular grinding machine*, with low priority.

*(Image: Fig. D-28 Example: Several work processes for the same lite, showing allocations for rectangular grinding on a CNC center and a dedicated rectangular grinder.)*

#### Allocation of Work Processes and Logical Machines

This session is about allocating logical machines to work processes, separating work processes and logical machines, and changing the priorities of logical machines.

**How to allocate a logical machine to a work process**

1.  Go to **Master data > MA > MA editor > Work process allocation**. Tab *Work process allocation* appears.
2.  Select the work process and the logical machine you want to allocate to each other.
    *(Image: Fig. D-29 Work process and logical machine selected in the editor.)*
3.  Click on the arrow pointing to the right to allocate the logical machine to the work process. The logical machine has been allocated to the work process and appears on the list below the work process, highlighted in gray.
    *(Image: Fig. D-30 Work process and logical machine allocated.)*
4.  Click on [Accept] to save the data. The allocation will be saved.

**How to separate logical machines from work processes**

1.  Go to **Master data > MA > MA editor > Work process allocation**. Tab *Work process allocation* appears.
2.  Click on the [+] for the work process. The view opens and the logical machines allocated to the work process are listed.
3.  Select the logical machine you want to remove.
    *(Image: Fig. D-31 Separating work process and logical machine.)*
4.  Click on the arrow pointing right to separate the logical machine from the work process.
5.  Click on [Accept] to save the changes.

> **Logical machine still in use**
> If an assignment should be removed that is still in use, it is deactivated automatically. Deactivated assignments are depicted in italics and with an appropriate icon. Please note, if a deactivated logical machine represents an alternative for a work process in an existing order but this assignment has been deactivated in the meantime, this alternative is offered during the scheduling now as before. Only with a repetition of the MZO for this order is the deactivation taken into consideration.

**How to change a logical machine's priority**

1.  Go to **Master data > MA > MA editor > Work process allocation**. Tab *Work process allocation* appears.
2.  Click on the [+] for a work process to view the allocated logical machines.
    > **Show all logical machines**
    > You can view all allocated logical machines by checking the checkbox [Open all].
3.  Select the logical machine the priority of which you want to change.
4.  Click on the arrow up or arrow down to raise or lower the priority.
    *(Image: Fig. D-32 Changing the priority of logical machines by reordering them in the list.)*
    The logical machine will be moved further up or down the list depending on its new priority.
5.  Click on [Accept] to adopt the changes. The new priority will be saved.

#### Work Process Allocation - Exercises

The following exercises shall help to deepen your newly acquired knowledge.
- For test purposes, define exercise machines, logical exercise machines, and exercise work processes reflecting your machinery, or use the exercise machines, logical exercise machines, and exercise work processes from previous sessions:
  - "Machines Exercises" on page D-32
  - "Logical Machines - Exercises" on page D-40
  - "Work Processes - Exercises" on page D-51
  - Allocate the logical "test" machines and work processes.
  - Try various scenarios and define priorities to execute work processes on the most cost-effective machine to run several work processes on a CNC center.
- Consider the actual situation of your machinery and the machines, logical machines, and work processes defined. Make a note of which work process allocation is practical for the orders on hand and which priorities have to be defined to achieve the optimum results.

**Additional information**
- Software Reference, "New Work Process" auf Seite D-107
- Software Reference, "Work Process" auf Seite D-108

### Conditions, Formulas, Restrictions

**Objectives**
- The use of formulas and conditions
- Selecting formulas and conditions
- The difference of formulas and conditions and their meaning

**Benefit**
- Formulas and restrictions are used to define machines, logical machines, and work processes in closer detail.

**Note**
- **Formulas**: Formulas are used in connection with machines, logical machines, and work processes. Formulas are predefined or can be defined by means of the graphic formula editor or the text formula editor. Formulas are used to define restrictions for machines, logical machines, and work processes. Formulas are restrictions or conditions which can be expressed in the database language SQL.
- **Formula editor**: The formula editor is a tool that enables the user to define restrictions of his own.

#### Conditions and Formulas in Connection with Machine Allocation

This session shows you how to select formulas/conditions.
Machine allocation can be completed by formulas and conditions for machines, logical machines, and work processes. The terms 'restrictions' and 'conditions' are often used in connection with formulas. In A+W Production, formulas, restrictions, and conditions are related as follows:
- Machines, logical machines, and work processes have certain properties which are often restrictive. Cutting tables for instance can handle lites only up to a certain size. The *Machine* dialog offers predefined fields for some of the most common restrictions. The values entered there will be saved as a formula in the master data of the machine, logical machine, or work process.
- Apart from that, the field *Additional condition* allows to define one's own formulas. You are therefore free to define facts and circumstances which match your production precisely.

> **Definition of formulas**
> In case of questions on how to define or amend formulas please contact the A+W Software GmbH support team.
> There is a separate tutorial on formula definition and management.

#### Select a Condition

You can select a condition in the properties of the machines, logical machines or work processes. You edit the formulas for a condition in the formula editor.
(See "Select a Formula for the Processing Time of a Logical Machine" on page D-66)

**How to select a condition**

1.  Go to **Master data > MA > MA editor > Logical machines**. In this example, the condition for a logical machine is set up. The description applies analogously for machines and work processes.
2.  Select the logical machine and click [Edit].
3.  Click the [magnifying glass] in the *Additional condition* area in order to select a condition.
    *(Image: Fig. D-33 Select a condition dialog.)*
4.  Select the condition you want to adopt. If a formula is created for the condition, the content is displayed in the Text field.
5.  Click on [OK] to adopt the condition. The designation is displayed in the *Additional condition* area.
6.  Click on [OK] to save the data. In order to edit the formula, you must change to the formula editor.

#### Select a Formula for the Processing Time of a Logical Machine

You can select a formula for processing duration directly in the properties of the logical machines. You edit the formulas for a condition in the formula editor. Alternatively, the processing duration of a logical machine can also be created or edited in the A+W Production capacity planning.

**How to select a formula for the processing time**

1.  Go to **Master data > MA > MA editor > Logical machines**.
2.  Select the logical machine and click [Edit].
    *(Image: Fig. D-34 Logical machine properties dialog, with 'Processing time' and 'Formula selection' highlighted.)*
3.  Click on [...] (B).
4.  Go to dialog *Formula selection* and select a formula.
    *(Image: Fig. D-35 Formula selection dialog.)*
5.  Click on [OK] to adopt the formula in the properties of the logical machine. The formula is displayed in the *Processing duration* line.
6.  Click on [OK] to save the data. You can edit the formula by clicking [Edit]. There is a detailed description of the formulas in the documentation for the *Formulas* part.

#### Selection of Conditions - Exercises

The following exercises shall help to strengthen your newly acquired knowledge.
- Make a note of the machine allocation dialogs in which you can select conditions.
- Take a piece of paper and sketch your factory's machinery with all the machines, logical machines, and work processes. Or use your existing notes:
  - "Machines Exercises" on page D-32
  - "Logical Machines - Exercises" on page D-40
  - "Work Processes - Exercises" on page D-51
  - "Work Process Allocation - Exercises" on page D-62
  - Which conditions are practical for your machinery and the orders on hand?
  - Which effects would the conditions have on the other areas of machine allocation?

**Additional information**
- Software Reference, "Select a Condition" auf Seite D-102
- Software Reference, "Select Conditions" auf Seite D-114

### Processing Types and Processing Articles

**Objectives**
- Definition of processing types in A+W Production and especially in connection with machine allocation
- Defining, editing and deleting processing types
- The reason why processing types cannot be deleted
- The meaning of processing articles in A+W Production and especially with regard to machine allocation
- Defining, editing and deleting processing articles

**Benefit**
- Work processes can be defined based on processing types or processing articles.
- If a processing type has been defined for a work process, it describes the technical type of processing, e.g. *Cutting*.
- If a processing article has been defined, it describes the technical type of processing, but more detailed than the processing type. A processing article is used to define a work process e.g. as *Bevelling*.

**Note**
- **Processing types**: Processing types describe the technical type of processing. Processing types are processing steps defined by the user. In addition to that, there is the predefined catalog from A+W Software GmbH.
- **Processing article**: Processing articles define - in closer detail than the processing type - the technical type of processing.

#### Processing Types and Machine Allocation

The processing type describes the technical type of processing. It defines for example if this is *Cutting*, *Assembly*, *Arrissing*, *Grinding*, or *Packing*.
Work processes are based on processing types. The work process unites the properties of the work piece and those of the processing type.

*(Image: Fig. D-36 Diagram showing a new work process being created from various processing types like Arrissing, Cutting, Grinding, Polishing.)*

Processing types are predefined by A+W Software GmbH but can also be defined by the user.

*(Image: Fig. D-37 Processing types dialog.)*

#### Processing Articles and Machinery Allocation

Processing articles refer to processing types. Processing articles can be used to describe processing types in closer detail. For the processing type *Grinding* for instance, you can define the processing articles *Bevelling*, *Mitres*, *Grooving*, *Frosting*, and *Rounded corners* to describe the technical process.

Since processing articles refer to the corresponding processing type, amendments can be made centrally. When you change the setting *Count processing steps* for the processing type *Grinding* for instance, this setting also changes for all related processing articles like *Bevelling*, *Mitre*, *Grooving*, *Frosting*, and *Rounded corners*.

*(Image: Fig. D-38 Diagram showing a work process 'Bevelling' created from processing articles like Mitre, Bevelling, Grooving, Frosting.)*

The example shows how work processes can be defined based on processing articles. The work process unites the properties of the work piece and those of the processing article. You can define processing articles of your own.

*(Image: Fig. D-39 Processing articles dialog.)*

#### Definition and Management of Processing Types

This session will tell you how to define, edit, or delete processing types.

> **Standard catalog of processing types**
> A+W Production offers a standard catalog of processing types. They have got four-digit numbers and must not be amended or deleted by the user. You can define additional processing types. We recommend to use the appropriate processing type from the standard catalog as a basis.

**How to define a processing type**

1.  Go to **Master data > Processings > Processing types**.
    *(Image: Fig. D-40 Define a processing type dialog.)*
2.  Select the processing type that shall be used as a basis for the new processing type (A).
3.  Click on [New] (B). The input fields (C) are released.
4.  Enter the data. (See Software Reference, "Processing Types" auf Seite D-123)
5.  Click on [Save] to save the new processing type. You have defined a new processing type. You can now edit it further if required. Click on the [Reject] button to abort the process without saving the data.

**How to edit a processing type**

1.  Go to **Master data > Processings > Processing types**.
    *(Image: Fig. D-41 Editing a processing type dialog.)*
2.  Select the processing type you want to edit (A).
3.  Click on [Change] (B). The input fields for the processing type - except the ID - are released and can be edited (C). (See Software Reference, "Processing Types" auf Seite D-123)
4.  Enter the data.
5.  Click on [Save] to save the changes. Click on [Reject] to abort the process without saving the data.

**How to delete a processing type**

> **Prerequisite**
> Processing types cannot be deleted if they are allocated to a processing article. An error message appears in this case. Resolve the allocation before you delete a processing type. (See "How to undo the allocation of a processing type and a processing article" on page D-79)

1.  Go to **Master data > Processings > Processing types**. Dialog *Processing types* appears.
2.  Select the processing type to be deleted.
3.  Click on [Delete]. A security check appears.
4.  Click on [Yes] to delete the processing type.

#### Definition and Management of Processing Articles

This session will show you how to define, edit, and delete processing articles and how to undo the allocation of a processing type and a processing article.

**How to define a processing article**

1.  Go to **Master data > Processing > Processing articles**.
    *(Image: Fig. D-42 Defining a processing article dialog.)*
2.  Select the processing article to be used as a basis for the new processing article (A).
3.  Click on [New] (B). The input fields (C) are released and can be edited.
4.  Enter the data. (See Software Reference, "Processing Articles" auf Seite D-125)
5.  Click on [Save] to save the processing article. You have defined a new processing article. You can now edit it further if required. Click on [Reject] to abort the process without saving the data.

**How to edit a processing article**

1.  Go to **Master data > Processing > Processing articles**.
    *(Image: Fig. D-43 Editing a processing article dialog.)*
2.  Select the processing article (A) you want to edit.
3.  Click on [Change] (B). The input fields (C) are released and can be edited. (See Software Reference, "Processing Articles" auf Seite D-125)
4.  Enter the data.
5.  Click on [Save] to save the changes. [Reject] can be used to abort the process without saving the data.

**How to undo the allocation of a processing type and a processing article**

1.  Go to **Master data > Processing > Processing articles**. Dialog *Processing articles* appears.
2.  Select the processing article that shall be allocated to another processing type. You can sort the list of processing articles by *Processing type* to make searching for the appropriate processing article easier.
3.  Click [Change]. The input fields of the processing article are released and can be edited.
4.  Select another processing type from combo box *Processing type*.
5.  Click on [Save] to save the processing article. [Reject] can be used to abort the process without saving the data.

**How to delete a processing article**

1.  Go to **Master data > Processing > Processing articles**. Dialog *Processing articles* appears.
2.  Select the processing article to be deleted.
3.  Click on [Delete]. A security check appears.
4.  Click on [Yes] to delete the processing article.

#### Machine Allocation - Exercises

The following exercises shall help to deepen your newly acquired knowledge. Enter the following master data:
- **Define an exercise machine, *Drilling*.** Enter the following restrictions for the drill:
  - The drill can process only lites from a thickness of 10 mm upwards, up to a thickness of 20 mm.
  - The machine cannot process shapes.
  - The machine can process lites with and without patterns.
- **Define an exercise machine *Line*.** Enter the following restrictions for the line:
  - The machine can process stepped and common IG.
  - The minimum lite size is 200 x 300 mm.
  - The maximum lite size is 2500 x 4000 mm.
  - The machine can process triple IG without size restrictions.
  - Enter an additional condition. Which effects can an additional condition have on the machine?
- **Define an exercise machine *CNC center*.**
  - The CNC center shall include two logical machines for the processing steps *Drilling* and *Polishing*.
- **Define an exercise cutting table** where the lites are put upright onto the machine.
- **Define an exercise work process, *Drilling*.**
  - Allocate the drill and the CNC center to the work process. The drill shall have top priority.
- **Define an exercise work process *Drilling on CNC center*** and allocate it to the CNC center with top priority. Allocate the drill to this work process with a lower priority, in case of bottlenecks.
- **Define an exercise work process based on the processing article.**
- **Define your own exercise processing type *Drilling*.**
- **Amend the work processes** from this exercise so that they are based on your own exercise processing type *Drilling*.

**Additional information**
- "Machines" on page D-15
- "Logical Machines" on page D-33
- "Work Processes" on page D-41
- "Allocation of Work Processes" on page D-52
- "Conditions, Formulas, Restrictions" on page D-63
- "Processing Types and Processing Articles" on page D-69

### Machine Allocation - Buttons

| Button | Meaning |
| --- | --- |
| 