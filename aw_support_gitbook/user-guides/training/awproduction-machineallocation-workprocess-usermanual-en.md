---
description: "AWProduction MachineAllocation WorkProcess UserManual EN"
---



title: "EN_UM_AWProduction_9"
source: "EN_UM_AWProduction_9.pdf"
tags: ["Machine Allocation", "Work Process", "A+W Production", "Logical Machines", "Manufacturing Software", "Production Planning", "Formulas", "Conditions", "Restrictions", "Glass Manufacturing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive user manual for the Machinery Allocation (MA) module of the A+W Production software. It serves as both a tutorial and a software reference, guiding users through the process of defining, managing, and allocating machines, work processes, and related manufacturing parameters to optimize production workflows in a glass, windows, and doors factory setting."
long_description: "This document provides an in-depth guide to the Machinery Allocation (MA) functionality within the A+W Production software suite. It is structured into a tutorial, a detailed software reference, and a set of quick-reference help cards. The manual is designed for production planners, system administrators, and technical staff responsible for configuring the manufacturing environment. The tutorial section offers practical examples and step-by-step exercises on how to define physical and logical machines, create work processes, and establish allocation priorities to manage production flow and prevent bottlenecks. It covers complex scenarios, such as handling rare articles through campaigns, processing items with multiple steps on a single CNC machine, and using conditions to control a lite's progress on the shop floor. The software reference section provides a systematic breakdown of every dialog, field, and function within the MA editor. It details the management of machines, logical machines, work processes, processing types, and processing articles. It also explains the powerful use of formulas, conditions, and restrictions (expressed in SQL) to create highly specific and flexible rules for machine allocation, capacity planning, and processing time calculations. This allows for precise control over the production environment, aligning software logic with real-world factory constraints. The final section includes help cards for common tasks, such as adding a new machine or configuring a machine for the Production Terminal, offering a quick and actionable guide for users."
---
## Machine Allocation

### Example 2, option Article group:
Certain articles are produced only infrequently.

To handle this case, define an article group that includes these rare articles, then start a campaign. Since campaign planning is based on a work process, choose the article group containing rare articles for this campaign.

You can thus plan when and how those rarely occurring articles shall be produced.

Campaigns are described in detail in section Capacity planning.

### Non-allocated work processes
A work process is shown in red until it is assigned a logical machine. Always allocate a logical machine to the work processes. If the corresponding logical machine has not been defined yet you should allocate Dummy as a logical machine.

⇨ "Allocation of Work Processes" on page G-808

### Priority of work processes
Work processes can be moved upwards or downwards on the list. For allocating work processes, the list is processed from top to bottom. A work process will be allocated if all conditions allocated to work process are met. The priority allocated to specialized work processes must therefore always be higher than the priority allocated to unspecialized work processes.

### Several work processes for the same lite
You have got an order for a glass door. This requires the work processes Rectangular grinding, Drilling, and Cut-outs.

Instead of using the more cost-effective rectangular grinding machine for grinding, all three work processes can be performed by the CNC center. This makes the single work process Rectangular grinding expensive but it saves time because all three processes can be executed on one machine, right after another.

You have defined the work process Rectangular grinding on CNC center for this purpose, to which you have allocated the logical machine CNC center rectangular grinding, with high priority.
To avoid bottlenecks, the work process Rectangular grinding on CNC center is also allocated to the logical machine Rectangular grinding machine, with low priority.

If you would produce the glass door on less expensive machines, the production flow would look like this:
*   Grinding on the rectangular grinding machine.
*   Then drilling on the automatic drilling machine.

---
A+W Production Machinery Allocation
G-801
---

## Machine Allocation Tutorial

*   Then production of the cut-outs on the CNC center. Added to this are 2x handling, 2x washing and the set-up time for the CNC center.

All things considered, producing the entire glass door on the CNC center may therefore be more reasonable.

### Additional conditions in work processes
Work processes are not exclusively linked to processing steps. They can also include additional conditions. A condition can be for example: This work process is executed on the CNC center. When you define the work process you can therefore define the machinery to be used with priority.

An additional condition can also check the bill of materials. Defining such a condition can therefore be used to control the lite's progress on the shop floor. The condition could be for instance: If the sheet's bill of material includes the processing steps Grinding, Drilling, and Cut-out, the sheet shall be completely produced on the CNC center.


