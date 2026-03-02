---
description: "A+W Capacity Planning"
---


# A+W Capacity Planning
A+W - Software for Glass, Windows and Doors

---
## Introduction
In this part of the documentation you can find editorial notices.

### Revision Overview

| Section Version / Date | Edition |
| :--- | :--- |
| 4.50 / 01-2023 | Export work plan added. |
| 4.00 / 11-2017 | Revision |
| 3.01 / 01-2017 | Product and company names adjusted. |
| 3.00 / 08-2013 | Initial creation of Tutorial and complete revision of Software Reference. |
| 2.00 / 04-2008 | Revision |
| 1.20 / 11-2007 | Change of name (AWCapacity/Capacity Planning) |
| 1.10 / 2007 | Change of chapter Work Plan |
| 1.00 / 2007 | Original version |

### Editorial
The editorial contains the following themes:
- Notes on this Document
- Copyrights
- Trademarks
- Contact

**Notes on this Document**

This document is intended for end users of A+W Production.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of the master data.

**Copyrights**

© 2023, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation.

The documentation must be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

**Trademarks**

Any designation of hardware and software being mentioned in the documentation can also be registered trademarks or other commercial rights of third parties being protected by law. Rights of third parties being protected by law are to be observed insofar.

**Contact**

> A+W Software GmbH
> Am Pfahlgraben 4 - 10
> D-35415 Pohlheim
> Germany
>
> 📞 +49 6404 2051 0
> 📠 +6404 2051 877
> 📧 Zentrale@a-w.com
> 🌐 http://www.a-w.com

# Tutorial
A+W Production
A+W - Software for Glass, Windows and Doors

## Overview
The tutorial on the *Capacity planning* module deals with the planning of your production process and the optimum use of your machine capacity. The main goals of capacity planning are the adherence to delivery dates, using the machinery to the best effect, and being able to react flexibly to unforeseeable events. Optimal capacity planning is always a balancing act between the greatest possible efficiency and greatest possible flexibility.

This tutorial describes how you can intervene manually in the planning and how the master data for capacity planning is set up.

This tutorial includes the following subjects:
- "Basic Principles" on page E-14
- "Planning and Scheduling" on page E-20
- "Master Data of Capacity Planning" on page E-67

### Prerequisite knowledge
This tutorial is meant for persons in charge of production scheduling in A+W Production who are responsible for organizing the optimum production process. Participants must be familiar with the master data concept in A+W Production. Knowledge of rough and detailed scheduling are also useful.

> **Protecting master data against access**
> The master data of A+W Production and especially of A+W Capacity Planning are highly sensitive data. Uncontrolled or unintentional interventions and changes can bring production to a complete standstill. Therefore, set up the workstations so that only the administrators or employees with appropriate functions have access to the master data.

> **Data back-up**
> Create a full back-up of the master data before beginning any processing of the master data. The backup tool is located under: `C:\Programs (x86)\A+W\Techsoft\Tools\AWSplicer\AWSplicer.exe`.
> Shift the saved back-up out of your user directory into a directory to which support also has access. Discuss the upcoming changes in advance with your planner at A+W Software GmbH.

### Documentation
The following documents are available for the *Capacity planning* module:

| Format | Scope |
| :--- | :--- |
| PDF | Complete documentation <br> - Tutorial <br> - Software reference <br> - Index |
| Online help `<F1>` | Dialog help |

### Tutorial Structure
This tutorial consists of subjects with several training modules each. Each unit consists of the following elements:

- **Overview**: Each training unit starts with an overview of the major topics:
    - Objectives: What shall be conveyed?
    - Benefit: What can this knowledge be used for?
    - Maxims: Which correlations are to be remembered?
- **Concepts**: Concepts and terms of the corresponding training session will be explained first. This is followed by examples and operating instructions.
- **Exercises**: There are exercises featuring special tasks for some of the training units.

### Display Conventions
Certain parts of the sentences are specially marked. The meanings are:

- **Italics**: mark character strings describing the software elements, e.g. the dialog *Campaign planning*.
- **Bold**: marks character strings to be entered via keyboard, e.g. **Enter 0**.
- **>**: The so-called 'breadcrumb trail' shows how to open a dialog, e.g. `Master data > Capacity planning > Campaign planning > Add campaign`.
- **[]**: Square brackets mark the buttons in the dialog, e.g. [OK] to save the data.
- **<>**: Pointed brackets refer to keys or shortcuts on the keyboard, e.g. `<F1>` is used to open the online help.

### Reading instructions
The contents of a training unit are based on the knowledge conveyed in the previous unit. We therefore recommend not to skip any unit.

If you are already familiar with a subject you should at least read the summary at the beginning of the unit in order to bring the main details to mind.

## Basic Principles
A+W Capacity Planning is designed so that even for products with unusually deep BOMs, usually several secure paths from the start technology to dispatch are found. The capacity planning accesses the work processes that the lites run through from cutting to delivery.

### Master data for machine allocation
The machine allocation (MA) establishes the connection between work processes and machines and maps the assessment according to preferred machines. So that the machines valid for the lites to be produced are found, the machines must be described precisely. In the machine allocation, there is a distinction between physical restrictions and logical machines with additional restrictions, cost rates and transition times.

Since the steps for setting up the capacity planning rely on the logical machines, the machine park must be described completely. The information for this is in the Machine Allocation section.

### Master data for capacity planning
For the date determination, shift plans, transition times, and times for the processing duration are required.

- So that a simple picture for the utilization arises for testing the data, it is recommended that you specify the processing durations across the board in seconds per piece, e.g. 1 - 5 minutes per lite depending on the machine.
- For the transition times, the optimal and realistic production throughput should be described. The specification of the times in whole shifts ensures a simple, predictable date determination. On machines that can also work unattended, the transition time (storage time) in hours can be specified, e.g. heat soak, autoclave, or hardening of silicon seals. In the exercises, ensure that you have the needed space in the operation in order to store the glass quantity of a shift.
- The scheduling bottlenecks can be determined from the times for the processing duration.

### Scheduling rules
The scheduling rules are specified as configuration parameters for A+W Capacity Planning. They influence the program behavior, the message culture, and the possible user reactions. This affects, for example:

- May delivery dates be shifted.
- When is the earliest production start for a scheduled order.
- How are quotations scheduled and do they have to be canceled again.
- How are rush orders put through.
- Starting with what quantity do items need to be split.

### Date Optimization
The date optimization begins with the last machine on or before the delivery date: the loading. With a view to the Production Monitor, the date optimization can be depicted as follows.

*Fig. E-1: Scheduling paths with and without conflicts*
This diagram shows a backward scheduling process across multiple days (Monday, Friday, Thursday, Wednesday) and various machines (Vehicle fleet, Packing, IG sealing, etc.).
- **(A) Vehicle fleet - loading:** The starting point of the backward scheduling.
- **(F) Production beginning cutting:** The calculated final start date.
- The process searches backward from the delivery date (A), accounting for transition times (D) between processes, which are counted in shifts.
- It identifies potential conflicts (E) and calculates different paths (B, C) to find the optimal, cost-effective schedule.

Starting from the drive date, after deducting the customer handling time (in working days), the production end is specified. From the end of the last possible work shift (A), the scheduling searches backwards for the latest possible production beginning.

The transition times from one processing to the next are counted in shifts (D), whereby 0 is the immediately following processing in the same shift. Locked shifts, which are marked with an X, are counted too.

The calculation always checks all possible cost-effective paths. In case of date conflicts, transition times are kept and there is a buffer at the end of production. If in the process storage times that are too long result, the buffer times must be distributed manually. The solutions arising this way are much more expensive, however.

### Scheduling
This section summarizes the technical background information for the scheduling.
Scheduling and interactive rescheduling uses the A+W Capacity Planning functions for allocating valid processing dates and machines to the bills of material.

Scheduling runs through five phases:
1. Analysis of the BOM.
2. Definition of machine paths.
3. Definition of feasible production dates.
4. Evaluation of feasible production dates.
5. Selection of the most favorable solution.

#### BOM analysis
The BOM is broken down into element chains; those are the BOM sections whose first processing has no preceding processing or that unites several BOM parts. The individual element chains are calculated independently and in parallel. The individual results are matched to the final BOM at the conclusion of the calculation.

*Fig. E-2: Formation of element chains from the BOM*
This diagram illustrates how a complex Bill of Materials (BOM) is broken down into smaller, parallel "element chains" for scheduling. For example, an Insulated Glass (IG) unit is broken down into its components like Float glass, Spacer, Laminated glass (LAMI), etc., which are then scheduled as separate chains before being combined.

While the BOM for the scheduling is being constructed, it is checked for plausibility at the same time. Here, errors in the BOM are detected and reported:

- Abandoned BOM elements and processing steps will be detected and skipped. A warning is written in the logfiles.
- Processing sequences are checked and adjusted. Defining processings receive the sequence 100; processings with smaller sequence are arranged according to the defining processing.
- Any missing defining processings will be detected and reported.
- Any missing logical machines will be detected and reported.
- Inconsistencies between the processing data and machine allocation master data will be detected.

#### Definition of machine paths
For the calculation of the machine paths, there are two features available in A+W Capacity Planning: best technology and automatic machine rescheduling. If only best technology is used, there is precisely one machinery path. Alternative machines are not used.

*Fig. E-3: Machinery path with best technology*
This diagram shows a linear production path where each processing step (A) like Cutting, Grinding, Polishing is assigned to one specific machine (B) like T1, S1, etc. This represents the "best technology" path with no alternatives.
- **(A)** Processing
- **(B)** Defined machines
- **(C)** No machine change
- **(D)** Informative processing
- **(E)** No machine change
- **(F)** Screen printing + subsequent screen printing

By forming processing chains on a machine, subsequent processings can be summarized insofar as the machine alternatives are the same. Subsequent processings (C, E) without machine change are done on the same date. To prevent this, e.g. with two screen printings one after another (F), a transition time must be defined so that the first printing can dry before the second is applied. Informative processings (D) are assigned to the preceding processing.

> **Processing chains and automatic rescheduling**
> The settings for processing chains and automatic rescheduling are specified in the machine properties. The machines are described in the Machine Allocation (MA) part.

For automatic machine rescheduling, all machine alternatives are determined and connected to one another for each processing in the element chain. The number of machine paths can thus get so large that no solution is possible. Therefore, the number of alternative machines must be limited.

*Fig. E-4: Automatic machine rescheduling*
This diagram contrasts with the previous one by showing multiple machine options for each processing step.
- **(A)** Preferred machines (e.g., T1, S1, BM1)
- **(B)** Alternative machines (e.g., T2, S2, BM2)
- **(C)** Manual production (e.g., HZ, HS, HB1)

In this example, you see that the alternative machines are limited: all machines where manual work is done are not included in the determination of the machine paths.

For each processing in an element chain, the quantity of valid alternative machines is loaded and transition times are assigned.
- For each processing, the machine specified by rescheduling determined by the MA or by earlier rescheduling applies.
- Subsequent processings without machine change are done on the same date.
- Machines that form processing chains can combine successive processings provided that their processing alternatives are identical.
- Machines that are not assigned to any registration point process only informative processings, e.g. Shape corners. These processings are assigned to the preceding processing and planned with it. The first processing of an element chain may therefore not be an informative processing.

All machines found are associated with their preceding machines insofar as the transitions are permitted. Thus the set of all machine paths with start points and end points will be created for an element chain. All processing steps of the element chain must not be included more than once in every path of the set.

> **Keep the number of alternative machines small**
> For each processing in the element chain, all machine alternatives are determined and connected to one another. The number of machine paths can thus get so large that no solution is possible. Therefore, limit the number of machine alternatives. Also form processing chains. This increases performance significantly.

#### Definition of feasible production dates
Using the machine paths, the shift plans, and the transitions between the participating logical machines, the possible production dates for the individual processings steps are determined. For this, their (virtual) costs are calculated and the scheduling rights determined, which are required for the use of the transitions.

Random transitions are permitted below the last processing step in the BOM, below each joining processing steps, and below campaigns, rescheduling targets, and date locks.

This makes sure that valid production dates are available even if the scheduling variance has been extremely restricted.

The result is a set of all scheduled machine paths from which the following evaluation can determine the most favorable paths.

#### Evaluation of feasible production dates
The set of all production dates found will be checked and evaluated. This results in solution sets for start and end dates of the machine paths and their (virtual) costs. This supports:
- A production flow that is as fast as possible
- Priority use of the transition type *Normal*.
- Scheduling for the preferred machine.
- Buffer times at the end of production.
- Use of the transition type *Rush* at the start of production.

If the production needs to be brought forward because of date conflicts, overload, locked shifts or for other reasons, this is done by moving the entire processing chain forward.

The result of this step is for every element chain a set of the most favorable solutions for every completion date of the next step.

#### Finding the optimal solution
The individual solutions for the element chains are linked with the transition costs to the next steps to achieve the optimal result for the entire BOM.

For every start date of a laminated sheet or IG unit, the most favorable solutions for all sub-elements are combined and passed on to the next step for every completion date.

#### Reporting to the ERP system
The calculated time and personnel costs and material consumption are reported in the order and the storage management of the ERP system. In connection with the ERP integration, the following data is transmitted:
- Scheduling state.
- Machine and personnel cost determination.
- Calculation of earliest possible delivery date.
- Query of the driving dates for route planning.
- Query of the receipt of goods dates.
- Fileless completion reporting via webservices.
- Online progress display from ERP via webservices.

## Planning and Scheduling
In this section, you will find information about how the scheduled orders are displayed and edited in the Production Monitor. In addition, you can correct incorrect schedulings and reserve production times.

This section provides information on the following subjects:
- "Production Monitor" on page E-21
- "Scheduling and Rescheduling" on page E-34
- "Campaign Planning" on page E-43
- "Reservations" on page E-53
- "Creating Processings" on page E-62

### Production Monitor
The Production Monitor is the central capacity and order control desk and entry point for work preparation, e.g. batch formation, rescheduling.

On the *Production Monitor* dialog, you check and edit production planning. Here, the capacity utilization of the machines is displayed per work shift.

*Fig. E-5: Production Monitor*
This image shows the main Production Monitor interface, which is a Gantt-style chart.
- **Rows (A):** Displayed machines (Schneidtisch 1, Schleifmaschine, etc.).
- **Columns (B):** Dates and their corresponding work shifts.
- **Bars (C):** Scheduled orders, color-coded to show status.
- **(D):** A shortened work shift.
- **(E):** A bottleneck, indicating a fully utilized shift.
- **(F):** A disabled/locked shift, marked with an 'X'.
- **(G):** A shift reserved for rush orders, marked with a '!'.
- **(H):** Undefined processings.

In this example, you see that for most machines, there are 2 work shifts available. For some machines, 3 work shifts are displayed and can be booked. These work shifts are set up and generated via the master data for the capacity planning. (⇨ "Master Data of Capacity Planning" on page E-67)

The orders are scheduled from the point of view of date optimization. Here, the rules of A+W Capacity Planning, the times of the work shifts, the locking of shifts, the defined bottlenecks, and the (virtual) costs are considered.

The details of how the scheduling is calculated is described in a separate unit. (⇨ "Date Optimization" on page E-15)

Generally, the orders from the ERP system are scheduled automatically. The work processes (processings) are scheduled accordingly on the machines' work shifts so that the delivery date promised in the order is adhered to. In special situations, you must intervene in this planning:

- **Shift orders to other machines or dates.**
    - ⇨ "Rescheduling" on page E-36
    - ⇨ "Rescheduling Processings" on page E-38
- **Eliminate missing information from the orders.**
    - ⇨ "Incorrect Scheduling" on page E-40
    - ⇨ "Post-Processing of Scheduled Orders" on page E-41
    - ⇨ "Creation of Processings" on page E-64
- **Lock, reserve or set up additional work shifts.**
    - ⇨ "Campaign Planning" on page E-43
    - ⇨ "Reservations" on page E-53
- **Eliminate missing information from the orders.**
    - ⇨ "Creating Processings" on page E-62
- **Adjust utilization on a daily basis.**
    - ⇨ "Daily Adjustments of the Work Shifts" on page E-23
- **Furthermore, you can set up the colored display of the work shifts as you wish.**
    - ⇨ "Setting up Production Monitor" on page E-30

#### Detail view
*Fig. E-6: Production Monitor - detailed view*
This image shows a zoomed-in view of the Production Monitor, focusing on the scheduling details for a single day.

In the detailed view, you can check the scheduling for individual days. In order to edit the schedulings, you must change back to the main view.

### Daily Adjustments of the Work Shifts
The work shifts in the Production Monitor are generated from the capacity planning master data. They apply for the assigned machines on particular days of the week and in a defined period of time. Changes to the master data therefore apply regardless of the current planning.

You can control the planning day by day by adding individual work shifts for a machine, for example; by disabling machines to exclude them from the scheduling; equalizing the planning by defining machines or work shifts as bottlenecks.

In order to adjust individual work shifts to current needs for ongoing orders, you have the following possibilities:
- "Here's how to create an additional work shift" on page E-24
- "Here's how to lock a work shift completely" on page E-25
- "Here's how to reserve a work shift" on page E-26
- "Here's how to edit the working hours for a work shift" on page E-26
- "Here's how to define a work shift as bottleneck" on page E-27
- "Here's how to set up the work shifts for a machine" on page E-28
- "Here's how to define a machine as bottleneck machine" on page E-29

**Here's how to create an additional work shift**

> **No automatic rescheduling**
> If you set up an additional shift in the Production Monitor, already scheduled orders are not rescheduled automatically.

1.  Select `A+W Production > Production Monitor`.
2.  Open the context menu for the machine and the day on which you need an additional work shift.
3.  Select the *Enter new shift* menu.
4.  In the *Define new shift* dialog, select the start and end time (B).
5.  Select the date (A) of the start and end times. The end date of a night shift must be on the following day.
6.  Save the setting with [OK].
The new work shift is displayed in the Production Monitor.

**Here's how to lock a work shift completely**

1.  Select `A+W Production > Production Monitor`.
2.  Mark the work shift (A) that you want to lock.
3.  Select *Shift properties* from the context menu (B).
    *Fig. E-7: Work shift - Properties*
4.  In the *Shift Properties* dialog, set the status to *Disabled*.
5.  Save the setting with [OK].
The locked shift is marked in the Production Monitor with an X.

**Here's how to reserve a work shift**

1.  Open the *Shift Properties* dialog as shown in the previous action sequence.
2.  Set the status to *Active for rush orders*.
3.  Save the setting with [OK].
The reserved work shift is marked in the Production Monitor with a `!`.

**Here's how to edit the working hours for a work shift**

1.  Open the *Shift Properties* dialog as shown in the previous action sequence.
2.  Enter the duration of the time in hours and minutes in the *Capacity* field (A).
3.  Save the setting with [OK].
Shortening of the work shift is indicated with cross-hatching in the Production Monitor.

**Here's how to define a work shift as bottleneck**

1.  Open the *Shift Properties* dialog as shown in the previous action sequence.
2.  Change the setting for the *Bottleneck* entry (A) to *Yes* (B).
3.  Save the setting with [OK].
The setting applies only for the current work shift. It prevents the work shift from being booked beyond its capacity.

> **Setting several work shifts to bottleneck**
> You can mark several work shifts by pressing `<Ctrl>` and marking the shift. When you're holding the `<Ctrl>` key down, you can also drag a rectangle across all shifts that should be marked. Then you can mark all highlighted shifts together as *Bottleneck*.

**Here's how to set up the work shifts for a machine**

1.  In the Production Monitor, open the context menu for the desired machine and select *Shift properties*.
2.  In the *Adjust shift plan* dialog, mark the days of the week (C) on which the machine is available in the work shift.
3.  Enter the number (A) of the shift to which the changes refer.
4.  Enter the duration (B) in which the machine is available on the marked days of the week.
5.  Save the setting with [OK].
6.  If necessary, update the Production Monitor so that the changes to the machine shifts are displayed.

**Here's how to define a machine as bottleneck machine**

1.  In the Production Monitor, open the context menu for the desired machine and select *Properties*.
2.  In the *Machine properties* dialog, change the setting for the *Bottleneck* entry (A) to *Yes* (B).
The setting only applies for the current machine and only until it is reset again manually. This way, the machine cannot be booked beyond its capacity.

> **Defining bottleneck machines at the very start of the process**
> To equalize production, bottleneck machines must be defined as far toward the beginning of the production process as possible. This setting should be specified at the beginning of the start-up of the Production Monitor via the setting of the machines displayed.
> ⇨ "Here's how to display the machines in the Production Monitor" on page E-30

### Setting up Production Monitor
In order to adjust the display to your planning needs, you have the following possibilities:
- "Here's how to display the machines in the Production Monitor" on page E-30
- "Here's how to set the display of the colors" on page E-31
- "Here's how to set the display type for all machines" on page E-32
- "Here's how to set the display type for one machine" on page E-32

**Here's how to display the machines in the Production Monitor**

1.  Select `A+W Production > Production Monitor`.
2.  Click [Selected machines].
    *Fig. E-9: Selection of the machines*
    On this dialog, all machines from the MA are listed. The red font marks machines that are defined as bottleneck machines. These machines cannot be booked beyond their capacity.
3.  Check whether the settings as bottleneck machines are correct. Via the context menu for a machine, you can change the setting.
4.  Mark the machines that should be displayed in the Production Monitor.
5.  Save the setting with [OK]. The dialog closes.
6.  If necessary, update the Production Monitor so that the changes to the machines are displayed.

**Here's how to set the display of the colors**

1.  Click [Settings].
    *Fig. E-10: Settings for the Production Monitor*
2.  Specify the settings with which the work shifts and scheduling should be displayed in the Production Monitor, e.g.:
    - Number of days (A) that are displayed before the start date.
    - Color (B, C) in which the times are displayed, e.g. assigned times, reservations.
    - Specification (D) whether particular information is displayed, e.g. the time, planned work processes.
3.  Save the settings with [OK]. The dialog closes.
4.  If necessary, update the Production Monitor so that the changes to the machines are displayed.

**Here's how to set the display type for all machines**

1.  Click [Change display type for all machines].
2.  Select with which values the scheduling in the Production Monitor should be displayed (e.g., *Time*, *Quantity*, *Sqft.*, *Weight*).
3.  Save the setting with [OK].
4.  If necessary, update the Production Monitor so that the changes to the machines are displayed.

**Here's how to set the display type for one machine**

1.  In the Production Monitor, open the context menu for the desired machine.
2.  In the *Machine properties* dialog, specify whether the assigned logical machines (A) should also be displayed for the machine.
3.  Select with which values (B) the scheduling of the machine in the Production Monitor should be displayed.
4.  Save the setting with [OK]. The dialog closes.
5.  If necessary, update the Production Monitor so that the changes to the machines are displayed.

### Export work plan
*Abb. E-11: Export work plan*

If you have opened the work plan in the production monitor via the context menu, you can export the data to a CSV file. Select the desired entries and open the `Display` menu. There you select `Export`. The dialog *Save as...* opens. Enter an appropriate name and click on [Save].

### Scheduling and Rescheduling

**Objectives**
- What is scheduling and how are orders scheduled?
- How can you react to problems which occur during scheduling?
- What is rescheduling and how is it done?

**Benefit**
- During scheduling, order and quotation data transferred by the ERP system are processed and calculated. Based on these data, dates are calculated and restrictions relevant for production are checked to make sure that your order is produced efficiently.
- Rescheduling can be used to allocate processing steps to other dates and machines.

| Term | Note |
| :--- | :--- |
| **Scheduling** | Scheduling means the processing and calculation of data after an order or a quotation has been transferred by the ERP system. The orders or quotations are generally scheduled automatically. You can re-work a failed scheduling. |
| **Bottleneck machine** | A bottleneck machine cannot be booked beyond its capacity. |
| **Scheduling** | Scheduling start with the selection of processings. The target dates are binding. They are treated like processings with a single campaign date. Delivery dates are protected - exception: The processing Shipping can be shifted. |
| **Processing sequences** | Processing sequences in ascending order define the sequence of processing steps. |
| **Rescheduling mode** | Possibilities for rescheduling: Complete BOM, Only predecessor processing, Only successor processing, Individual processing. Rescheduling mode and direction are independent. Processings that do not participate are excepted from the scheduling. |
| **Rescheduling of orders** | - **Date rescheduling:** Orders are shifted to other dates. <br> - **Machine rescheduling:** Orders are produced on other machines than originally planned. |

#### Scheduling of Orders
Generally, automatic scheduling of orders is set up in A+W Production. The data import runs as background process. You can trace the process of scheduling in the *A+W ServiceMonitor*. Manual interventions are only required if individual orders or order items could not be scheduled. The processing of these orders is described in a separate unit.
⇨ "Incorrect Scheduling" on page E-40

You can check and edit the scheduled orders that cannot be processed further on the *Orders* dialog. This topic is discussed in the *Rough Scheduling* section.

If manual scheduling has been configured in A+W Production you will have to use the *Scheduling* dialog. When scheduling has been successful, field *Status* will show the actual time.

The scheduling is calculated in A+W Production until a solution is found that corresponds to the scheduling rules. If no acceptable solution was found, you must control the scheduling manually. For this, for example, large items can be split. The position split is described in detail in the *Rough Planning* section.

> **Settings for the data transfer**
> Please check the settings for the data transfer from the ERP system to A+W Production with the A+W Software GmbH customer service team.

#### Rescheduling
You can reschedule orders if they cannot be put through production as originally planned. Here, you can either select another machine or shift the processing to another date.

- Scheduling begins with the selection of processings.
- With the various rescheduling modes, you have the following possibilities for rescheduling: Complete BOM, only predecessor, only successor, individual processing.
- The target dates are binding: The target dates are assigned and locked. They are handled like processings with a single campaign date.
- Delivery dates are protected: This does not apply for the processing *Shipping*.
- Rescheduling mode and direction are independent. Processings that do not participate are excepted from the scheduling. If due to the rescheduling an invalid processing sequence would arise, all successors are rescheduled if this achieves a valid result. An invalid rescheduling would be, for example, the rescheduling *Only predecessors* in the direction later than the successors.

**Machine reallocation**
With a machine reallocation, the production of an order is shifted to other machines. This can be necessary, for example, if a machine is not available due to repairs.

*Fig. E-13: Machine reallocation*
The *Machine Reallocation* dialog shows currently scheduled machines/routes (A) on the left and a list of available alternative machines (B) on the right, allowing a user to move a job.

#### Processing rescheduling
For the rescheduling of a production date, a processing is shifted to another date so that the order is completed earlier or later. This can be necessary, for example, if the priority of an order changes.

*Fig. E-14: Rescheduling*
This dialog allows detailed rescheduling.
- **1. Select Processing Steps (A):** A list of processings for an order.
- **2. Select Date, Shift, and Machine (B):** A Gantt chart to visually select a new machine, date, and shift.
- **3. Execute Re-scheduling (C):** A dropdown to select the rescheduling mode.
- **Specifications (D):** Checkboxes for options like *Keep Protected Processing Dates*, *Reschedule as High-Priority Order*, etc.

You can reschedule a processing (A) for another date (B) or another machine. For this, you can specify how the transition times (D) should be considered. The dates recalculated by a rescheduling can then be locked. Thus, they are protected against further rescheduling.

The following modes are available for rescheduling (C):
- **Reschedule complete BOM:** The complete parts list to which the processing belongs is rescheduled.
- **Only marked processing:** Only the marked processing is rescheduled.
- **Selected processing and all following processings:** The selected processing and all following processing steps for the lite will be rescheduled.
- **Marked and all previous processings:** The marked and all previous processings of the lite are rescheduled.
- **Unconditional allocation of dates for selected processing:** Scheduling of the selected processing will be forced on the selected date irrespective of the machine capacities.

With all these options, shipping and delivery date will be kept unless they are explicitly rescheduled. If you permit the shifting of the delivery date (D), you should also send the new delivery date back to the ERP system.

### Rescheduling Processings
This unit will teach you how you can shift the processings to another date.

**Here's how to reschedule a processing**

1.  Go to `Display > Orders > Context menu for selected orders > Processings > Context menu for selected processings > Work schedule > Rescheduling`.
    *Fig. E-15: Reschedule date*
2.  Choose the processings (A) to be rescheduled. If you select several processings, you can only shift the date.
3.  Select the setting for the scheduling (E):
    - **Force rescheduling:** With this setting, the capacity limits of bottleneck machines are not considered. Therefore, it is possible to overbook the work shifts.
    - **Allow Express Grid:** For rescheduling, the transition times of the type *Rush* are used.
    - **Reschedule as High-Priority Order:** The processing is rescheduled with the minimum transition times. Caution: Here, the times for campaigns can also be used. Use this setting only in emergencies.
4.  Mark the shift in which the processing should be rescheduled (B).
5.  Choose the rescheduling mode (D). The button to start the rescheduling is enabled.
6.  Click [Reschedule] to start the rescheduling. The times are recalculated. The result is displayed on a dialog. If the rescheduling was not successful, you must change the conditions and try rescheduling again.

### Incorrect Scheduling
The scheduling of orders can fail for various reasons, e.g. in the following cases:
- Undefined articles in orders.
- Undefined production articles in orders.
- Undefined processing steps in orders.
- Invalid order data.
- Shift restrictions cannot be met.
- Shifts do not exist, e.g. because the shift plans have expired.

You can rework these orders and then repeat the scheduling.

*Fig. E-16: Incorrect scheduling*
This dialog shows orders that failed to schedule.
- **(A) Defective Orders:** A list of orders with scheduling errors.
- **(B) Selection criteria for the display:** A list of error types to filter the orders (e.g., Undefined Articles, Invalid Order Data).

To filter the orders, you can select one of the possible error causes (B). The display of the corresponding orders (A) is updated automatically. You can select per order how the orders are handled. For this, you have the following options:
- **Take over data again:** The order data is scheduled again and unchanged. For this, you must correct the master data, e.g. extend shift plans, and then schedule without renewed transfer of the data from the ERP system.
- **Force scheduling:** The scheduling is forced. Here, the capacity of bottleneck machines is not considered. Therefore, the work shifts can be overbooked.
- **Ignore scheduling:** The production dates are determined without consideration of transfer times, capacity limits, and campaign dates. All other orders and their delivery dates are pushed back.
- **Delete invalid orders:** The corresponding orders are deleted. Speak to your colleagues in order entry so that the orders will be corrected and re-entered into A+W Production.
- **Confirm determined delivery date:** The delivery date proposed by A+W Production is accepted. The new delivery date is reported back to the ERP system.

### Post-Processing of Scheduled Orders
This unit will teach you how you can manually re-work the orders that could not be scheduled.

**Here's how to re-work a scheduling**

1.  Go to `Master data > Post-processing of scheduling`.
    *Fig. E-17: Post-processing of invalid scheduling*
2.  Select the filter criterion (B) for the display of the orders and sorting (C). The list of orders is filtered.
3.  Select the order (A) to be edited.
4.  Click [Edit].
5.  Depending on the filter criterion, a dialog opens. Select the option with which you can eliminate the error.
    - *Asynchronous Processing*: Options to "Try again", "Try again without processing parameters", or "Ignore Error".
    - *Defective Orders*: Options to "Repeat data import", "Force scheduling", "Ignore scheduling rules", "Delete invalid orders", or "Confirm calculated delivery date".
    - *Changes to Scheduled Orders*: Options to "Create new line item", "Try again", "Ignore modification", or "Apply the changes to the existing batches".
6.  Click [OK] to adopt the changes. The order is treated according to the options selected.

### Campaign Planning

**Objectives**
- What is a campaign?
- How are campaigns defined, edited, and deleted?
- What are *Individual dates*?
- What are *Weekly dates*?

**Benefit**
- Campaigns are processes that are executed only on certain days, in certain shifts, and on certain machines, e.g. blue screen printing every Friday in shift 2.

| Term | Note |
| :--- | :--- |
| **Campaigns** | Campaigns will help you process specific orders for customers or projects and plan them in due time. Campaigns are fixed, repeating dates for particular processes, which are largely untouchable. However, they can be overridden by "High-priority orders" or in the rescheduling editor with date assignments. |
| **Individual dates** | Individual dates are campaigns which are executed just once. |
| **Weekly dates** | Weekly dates are campaigns which are run on a regular basis. |

> **Prerequisite**
> Campaigns can be defined only if the appropriate work processes and shifts have been defined and if the corresponding shift plan is active. (⇨ "Shifts" on page E-68)

#### Definition of the Campaigns
Campaigns serve especially to set up a machine correctly, e.g. for coatings that require long set-up times. This means that the machine is used in different modes.

With campaigns, you can plan capacities for particular work processes, e.g. for screen printing in a different color for each day of the week. From this, e.g. campaigns *Blue on Monday* or *Green on Tuesday* are created. The advantage of reserving the screen printing capacities in this way is that the cleaning and set-up work can be minimized.

Campaigns can also be set up so that particular work processes are done in a particular shift, e.g. all the cutting of special glass types in the first shift.

The time reserved for a campaign can only be overridden by high-priority orders.

*Fig. E-19: Campaigns*
This dialog is for managing campaigns.
- **Work process (A):** A list of all available work processes.
- **Activated campaign (E):** Work processes that have been designated as campaigns.
- **Day of the campaign (B):** Tabs for *Individual Dates* and *Weekly Dates* to define the schedule.
- **Available shifts (C):** Shifts available for the selected day.
- **Day of the planned campaign (D):** The final list of scheduled campaign dates and shifts.

A campaign always applies for a particular work process (A). It is either specified as individual date or as weekly date on a particular day of the week (B). If on the day there are several shifts available (C), the respective shifts must be specified.

Campaigns are used exclusively for work processes. The machine on which the processing is done plays no role here. For this, the work processes may not be bound to a particular machine.

> **Example**
> If two different screen printings are defined, during scheduling it must be detected which of the screen printings is the one in question. Here it plays no role on which machine the screen printing is done.
> A work process *Screen printing for campaign X* must be set up in the MA so that it is only used for campaigns. This work process must be assigned to the logical machine to which the campaigns are allocated.

### Campaigns in Scheduling
For the scheduling for campaigns, all dates are hidden for which the work process does not apply.

*Fig. E-20: Scheduling for campaigns*
This diagram shows how the scheduler handles campaigns. It hides non-campaign work shifts (A) and uses flexible transition times (B, D) to find an optimal solution (E) that respects the campaign dates, even if there are multiple campaigns in the BOM (C).

In this example, you see that the optimal solution (E) has a transition from one shift apiece. If the scheduling finds no result, it is checked whether there is a solution if campaign dates are ignored. If necessary, a corresponding message indicates that campaign dates are missing.

Work processes with campaigns automatically receive a flexible transition time at entry. If in the BOM there are several campaigns (C), then the system searches for earlier start dates (B, D) in order to avoid conflicts.

### Definition and Management of Campaigns
This unit will show you how to define, edit, or delete campaigns.

For instructions on this subject, please see:
- "Here's how to define a campaign as an Individual date" on page E-47
- "Here's how to define a campaign as a weekly date" on page E-49
- "Here's how to edit a campaign" on page E-51
- "Here's how to delete a campaign" on page E-52

> **Prerequisite**
> Campaigns can be defined only if the appropriate work processes and shifts have been defined and if the corresponding shift plan is active.
> ⇨ "Here's how to draw up a shift plan" on page E-75

**Here's how to define a campaign as an Individual date**

> **Prerequisite**
> On the *Individual dates* tab, only activated shift plans are displayed. If necessary, activate the shift plans that are required for the campaign.

1.  Go to `Master data > Capacity planning > Campaign planning`.
2.  Mark the work process (A) for the campaign. The buttons are enabled.
3.  Click the arrow to the right. The work process is displayed in the *Campaigns* field.
4.  Check the checkbox of this work process in the *Campaigns* field. The *Individual dates* tab is active now.
5.  Mark the date for the campaign (B) on the calendar. The *Available shifts* field lists the shifts that are available for this date.
6.  Choose the shift in which the campaign shall be run.
7.  Specify how many days or weeks (C) the campaign should last.
8.  Click [+]. The new campaign is displayed in the *Individual dates* field. If the campaign should run through several shifts, repeat the steps 6 - 8 for each individual shift.
9.  Click [OK] to save the campaign. The campaign is saved, the dialog closed.

**Here's how to define a campaign as a weekly date**

> **Prerequisite**
> On the *Weekly dates* tab, only activated shift plans are displayed. If necessary, activate the shift plans that are required for the campaign.

1.  Go to `Master data > Capacity planning > Campaign planning`.
2.  Mark the work process for the campaign. The buttons are enabled.
3.  Click the arrow to the right. The work process is displayed in the *Campaigns* field.
4.  Check the checkbox of this work process in the *Campaigns* field. The *Weekly dates* tab is enabled.
5.  Change to the *Weekly dates* tab.
6.  Mark the day of the week for the campaign (A) on the calendar. The *Available shifts* field lists the shifts that are available for this day of the week.
7.  Choose the shift (B) in which the campaign shall be run.
8.  Click [+]. The new campaign appears in the *Weekly dates* field. If the campaign should run through several shifts, repeat the steps 6 - 8 for each individual shift.
9.  Click [OK] to save the campaign. The campaign is saved, the dialog closed.
