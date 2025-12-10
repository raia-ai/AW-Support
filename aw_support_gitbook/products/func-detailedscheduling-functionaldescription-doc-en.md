---
description: "EN-FUNC-AW_Production-Detailed_Scheduling"
---


# A+W Functional Description: A+W Production - Detailed Scheduling

---
## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2016, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to perform changes to software data, structure and interfaces as part of program extensions without prior notice. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This also includes possibly necessary long-term costs and expenses for amending and extending subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Functional Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Article number** | 220014 |
| **Module** | Detailed Scheduling |
| **Brief description** | Detailed Scheduling. Planning and orientation of the production organization for the cutting and processing of flat glass (control of grouping, sorting, rack organization, and rack assignment) |
| **Available** | Starting with ALCIM 2000 |

### 3.2. Description

The glass required for the production is generally cut from stock plates on the cutting tables. Frequently at a company there are several automatic cutting tables as well as at least one cutting table for hand cutting or for shapes.

The lites are stored on storage racks (e.g. A-racks) after processing (for example cutting) depending on their next processing step and moved with the rack to their next processing. Within a work area (e.g. cutting) or a process chain (e.g. cutting > LG line), the logic of the rack and removal of the glass can be quite diverse. Among other things, this depends on how much space is available in this area for racks in order to store the glass and how broad the travel paths are. These questions are important for detailed scheduling. If, for example, behind cutting there is little space for racks, this situation must be balanced out with good optimization and sequence of the lites so that as few racks as possible are needed and there must be little re-sorting.

For efficient assembly on the IGU and/or LG line, the individual lites of the unit must be as close to one another as possible. They do not necessarily have to be on a rack. This means that, depending on the organization, there must be re-sorting before the line.

The A+W Production (ALCIM) detailed scheduling controls the grouping, sorting, and stacking of glass on racks. Thus the production sequence for the parts included in the batches is controlled and at the same time all racks for glass on the path through production from cutting to packaging are defined.

### 3.3. Requirements

- A+W Production (ALCIM) (article number 220001 and 220002)
- A+W Basic Flow Planner for the production types to be handled (article number 22x003)
- Defined criteria (formulas) for filters, grouping and sorting keys
- Storage rack organization set up in the master data (production and usage organization)
- For the setup and efficient use of the detailed scheduling logic and setting possibilities, an extensive and detailed training by an experienced A+W consultant is indispensable.
- An appropriate batch formation is required for efficient detailed scheduling. Thus, for example, for the mapping of a multi-stage production, a creation of separate production and use batches is necessary (e.g. for the mapping and organization of TG in LG in IGU).

### 3.4. List of functions

**1. Formula**
- Using the formulas, any criteria (formulas) for filters, grouping and sorting keys can be defined.
- For this, there are two editors available: a graphic editor and a free formula editor.
- Using the free formula editor, the definition and use of SQL commands and the call/incorporation of stored procedures is possible.

**2. Racks**
- A+W Production detailed scheduling is based on the calculation with logical racks.
- A calculation based on physical racks is possible - with the add-on A+W Stack Optimizer (article number 220032).
- It is possible to use A-racks, L-racks, and harp racks for stacking the glass.
- For these rack types, physical rack parameters (e.g. maximum loading weight, maximum stack depth) can be set.
- With use of the A+W Stack Optimizer add-on (article number 220032) for the calculation of phys. racks and the storage of glass on these racks, all rack parameters are evaluated (e.g. width of the rack and maximum number of stacks per rack).

**3. Stacking modes**
- There are 4 pre-defined stacking modes, which have different requirements and results for storing the glass: glass, unit, production, and VABGLA. For a precise description of the possibilities, properties, and requirements with respect to this stacking mode, please see the A+W Production Detailed Scheduling manual.
- The stacking modes (for an organization) defined and pre-set in the master data can be changed flexibly in the optimization.

**4. Optimization modes**
- Using the flexible settings and parameters of the detailed scheduling (e.g. grouping and sorting keys, stacking mode), different degrees of freedom for the yield optimization can be achieved and thus results that vary in quality gained.
- In total, there are 5 different optimization modes: XOPTS 6.2, XOPTS 6.1, XOPTS 5.2, XOPTS 5.1, and XOPT. These distinguish themselves with respect to the formation and sorting of groups, as well as the sorting of glass within the groups. XOPTS distinguishes itself through a yield optimization taking into consideration a defined sequence of the glass; XOPT is a chaotic yield optimization. To use the XOPTS modes, the A+W Sequence Optimizer is required (article number 220014).
- These modes do not absolutely have to be familiar to the user. The achievement of the desired optimization and grouping and sorting results is possible purely with settings of detailed scheduling parameters (e.g. selection of the grouping and sorting key, selection of the stacking mode).
- For a precise description of the setting possibilities for the various optimization modes as well as their results/effects, please see the A+W Production Detailed Scheduling manual.
- For the orientation of the production sequence for insulated glass and/or LG, the first and second lites always have the same sequence - for different glass types. Thus it is guaranteed that the sequence of the first glass type (after the optimization) considers the second glass type for the optimization. This is already defined in the system background and does not have to be stored separately by the user or the master data administrator.
- It is possible when stacking the glass to work with split or complete groups. This affects the number of logical racks generated as well as the stacking (and also removal) of the glass of a group for the production. The results can - depending on the stacking mode selected - vary greatly and offer various advantages and disadvantages in reality (with respect to number of racks, travel paths, and complexity of the stacking and removal of the glass). For a precise description of stacking with complete or split groups, please see the A+W Production Detailed Scheduling manual.
- The optimization parameters can be stored as defaults in the master data of a rack organization. However, these parameters can be changed flexibly in an optimization and thus the stored default settings can be overridden.

**5. Grouping and sorting**
- Using the formula, any grouping and sorting keys can be defined (e.g. grouping by customer and glass type, sorting by size ascending or descending).

**6. Storage rack organization (organization)**
- Organizations can be defined freely with the specified editor. Here, it is possible per lot type (glass type) to define an individual organization with its own parameters.
- It is possible to map a multi-step production (e.g. TG in LG in IGU).
- It is possible for a production step to define production organization (e.g. IGU) and use organization (e.g. TG for IGU). Here different parameters and rules can be stored for production and use organizations.
- No production organization has to be defined.
- Formulas/criteria can be defined on the levels Orga group and Rack. Per orga group and/or rack, up to 7 additive criteria can be stored as filters.
- The sequence/priority of the filter criteria can be defined per organization (Master data > Orga > Test sequence).
- It is possible to consider ordered parts in an organization and to store these ordered parts in the appropriate work step on a logical rack (with a logic and numbering defined for this). This glass can be sorted easily and flexibly for each respective work step.

**7. Optimization/interface**
- It is possible to change the settings and parameters stored in the master data (orga) flexibly in the optimization (for example, grouping and sorting keys, stacking mode, use of complete or split groups, stacking depth).
- The use/consideration of individual stacks can be deactivated.
- The results of the rack assignment and yield optimization can be displayed graphically.
- Broken lites from the plant data collection (FDC for short) from the A+W Production Terminal or the A+W Realtime Optimizer can be selected and re-optimized in the course of detailed scheduling.
- Rush lites entered in A+W Production can be selected and re-optimized in the course of detailed scheduling.
- It is possible to set a so-called free optimization. Here the character of the sequence of the first lite is written onto the sequence of the second lite. This can be necessary and helpful if the sequence has very negative consequences for the yield of the second glass type (for example for an expensive glass type). First and second lite can then be optimized with different grouping and sorting keys (and thus optimization mode).
- The cutting patterns can be examined in another editor.

### 3.5. Limitations

**1. Formula**
- Supported in the standard are only the basic computation types (+ - x :)
- Logarithms and root expressions can only be mapped using free SQL expressions or the calling of stored procedures.

**2. Racks**
- Only logical racks are calculated (A-racks). For harp racks, logical racks = physical racks.
- For a calculation and consideration of physical racks (A-racks), the add-on A+W Stack Optimizer (article number 220032) is required.
- Without the A+W Stack Optimizer add-on (article number 220032), for the calculation of the number of logical racks and the storage of glass on the logical racks, only the rack parameters maximum stacking depth and maximum weight per stack are considered.
- Without the A+W Stack Optimizer add-on (article number 220032), there is no assignment of logical rack - physical rack. It is left to the user to distribute the logical racks to physical racks and to determine the necessary number of physical racks for production.
- With use of the A+W Stack Optimizer (article number 220032), the functionalities for the changing of optimization parameters for the detailed scheduling in the dialog interface (grouping, sorting, stacking mode, etc.) are severely limited.

**3. Stacking modes**
- It is not possible to define new, additional stacking modes.
- The stacking mode unit offers the greatest degree of freedom for the optimization and therefore, in contrast to the other 3 stacking modes, offers the possibility for the best optimization results (yield optimization).
- The 4 stacking modes and their results/effects must be known in order to achieve the desired results for the real handling of the glass.

**4. Optimization modes**
- No new optimization modes can be defined.
- No new logic with respect to the stacking of groups can be defined (in addition to complete groups and split groups).
- The efficient setting of optimization parameters assumes good previous knowledge of the areas of yield optimization, stacking, and sorting of glass.

**5. Grouping and sorting**
- The settings with respect to grouping and sorting in the area of optimization have a significant influence on the optimization mode and the yield results thus achieved, as well as on the stacking of the glass and the work associated with this in production.

**6. Storage rack organization**
- No more than 7 additive filter criteria per organization group and/or rack can be defined.
- The filter criteria stored in an orga can only be changed in the orga master data with respect to their sequence/priority. A flexible changing in the course of the optimization is not possible.
- Filter criteria can only be assigned on the level of organization group and rack. On the level of the master organization or organization, this is not possible.
- Between a production and a use orga, there are no logical and data-technical relationships. There is no inheritance of data from a production organization to a corresponding use organization.
- The handling of broken lites and the corresponding stacking and sorting of this glass requires a specific logic and strict adherence on the part of the workers in production.

**7. Optimization/interface**
- It is not possible in the course of the optimization to define new formulas (filter criteria, grouping and sorting keys).
- It is not possible in the course of the optimization to define new racks/ rack types.
- The results with respect to rack calculation and assignment cannot be edited in the course of the optimization.

### 3.6. Notes

**Setting up a new orga**
- The set-up is done in the course of a customer project. For this, a detailed orga conversation is initiated, in which the customer (e.g. Production Manager and employees who handle work preparation) and the A+W consultant analyze the basic conditions and real requirements together. Then there is an attempt to map this in the rules and settings of an orga.
- Since the creation and management of an orga are truly complex - not with respect to the software, but the multiple possibilities and effects in reality - it is recommended that customers do not attempt this without the support of A+W. A+W practical experience has shown this to be the case.
- In a new project, a database with a set of defined and standard orgas can be made available to the customer. This guarantees that a) production using the standard orgas is quick and easy using the default views defined and b) these orgas continue to function in the course of update and patches.
- A change in the area of detailed scheduling can have significant effects on the production sequence and yield results, and can thus result in significant added costs. Therefore, it is recommended that you familiarize yourself intensively with the possibilities and editors of the A+W Production Detailed Scheduling in the course of a training. Furthermore, it is recommended that in case of changes in the detailed scheduling master data area, you always contact A+W Support.

**Additional notes and detailed information**
- For additional notes and detailed information, please see the A+W Production Detailed Planning manual as well as the help.
- For detailed questions before you have purchased product(s), please contact A+W Sales or, in the course of cooperation, A+W Support.

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com
Internet: http://www.a-w.com/
