---
title: "EN_AWBusiness_Capacity_Planning_4_1"
source: "EN_AWBusiness_Capacity_Planning_4_1.pdf"
tags: ["A+W Business Pro", "Capacity Planning", "Software Tutorial", "Glass Manufacturing", "Window and Door Software", "Master Data Management", "Production Scheduling", "Time Management", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A comprehensive tutorial for the A+W Business Pro Capacity Planning module. This document guides users through setting up master data, planning production capacities, and monitoring machine utilization for glass, window, and door manufacturing."
long_description: "This document serves as a detailed user guide and tutorial for the Capacity Planning module within the A+W Business Pro software suite. It is designed for end-users, such as production planners, who are responsible for managing and monitoring production capacities in the glass, window, and door manufacturing industries. The tutorial covers the fundamental principles of capacity planning, from initial setup to daily operational use. It provides step-by-step instructions on how to configure master data, including machines, production areas, work types, shift schedules, and default production times. The guide explains how to allocate products to specific work types and machines, handle restrictions, and manage priorities for automatic scheduling. It also details the process of scheduling orders, handling capacity problems, and monitoring production status through various reports and the control station. The document emphasizes the interaction between different master data components and how they collectively influence production start dates, time costs, and overall plant efficiency. It includes numerous examples, diagrams, and screenshots to illustrate concepts such as calculating time surcharges, handling alternative work types, and managing transition times between production stages."
---

# A+W Capacity Planning
---
## A+W Business Pro
**A+W - Software for Glass, Windows and Doors**

---

## Introduction
This part of the documentation contains editorial notes.

### Revision Overview

| Part Version/Date | Description |
| :--- | :--- |
| 1.00/12-2003 | Initial creation |
| 1.01/08-2008 | Spelling and grammar corrections, graphic tables converted, figures and part numbering adjusted |
| 1.02/09-2010 | Layout adjusted to document concept 2010 |
| 2.00/05-2012 | Initial creation of the tutorial, software reference completely reworked |
| 3.00/08-2013 | Adjustment of the ALFAK documentation to A+W Business Pro. |
| 4.00/04-2014 | Complete revision. |
| 4.01/04-2015 | Adjustment A+W Business Pro. |
| 4.02/01-2017 | Product and company names adjusted. |

### Editorial
The editorial contains information about the following topics:
- Notes on this document
- Copyrights
- Trademarks
- Contacts

**Notes on this document**
This publication is conceived exclusively for end users of A+W Business Pro.

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The greatest care was used in compiling the texts and figures. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

This document describes the complete stage of expansion of A+W Business Pro.

### Copyrights
©2017, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation.

The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Without the prior written permission of A+W Software GmbH, the documentation may not be transmitted electronically, by recording or in any other form.

### Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### Contacts
**A+W Software GmbH**
Am Pfahlgraben 4 - 10
D-35415 Pohlheim
Germany
📞 +49 6404 2051 0
📠 +6404 2051 877
📧 Zentrale@a-w.com
🌐 http://www.a-w.com

## Contents
- **Introduction**
  - Revision Overview
  - Editorial
- **Tutorial**
  - **Overview**
    - Documentation
    - Tutorial Structure
    - Display Conventions
    - Menu Overview
    - Basic Principles of Capacity Planning
    - Using Capacity Planning
  - **Master Data**
    - Machines and Production Areas
    - Shift and Working Hours
    - Default Times
    - Selection of Machines
    - Allocate the A+W Business Pro Master Data
  - **Capacity Planning**
    - Scheduling Orders
  - **Production**
    - Reports about Production Status
  - **Production Costs**
    - Time Costs
  - **Control Station**

## Tutorial

### Overview
The tutorial for the Capacity planning module focuses on the basic principles of planning production capacities in A+W Business Pro. The tutorial is based on the knowledge of master data and documents.

> **Functions depend on the enabled modules**
> Please note that the various functions are only available if the corresponding modules and interfaces are installed and enabled.
> If you find functions in this description that are not available in your version, please contact A+W Software GmbH.

**Subjects**
This tutorial includes the following subjects:
- Master Data
- Capacity Planning

**Required knowledge**
The tutorial is meant for those who plan capacities in A+W Business Pro and thus monitor the utilization of the machines. Participants must be familiar with the concept of master data in A+W Business Pro and the Documents module. Knowledge of the Production and Stock Management modules is advantageous.

### Documentation
The following documents are available for the Capacity planning module:

| Format | Scope |
| :--- | :--- |
| Handout | Printout of the tutorial for the training |
| PDF | Complete documentation: Tutorial, Software reference, Index |
| Online help `<F1>` | Context-sensitive dialog help of A+W Business Pro software reference and tutorial |

### Tutorial Structure
The tutorial consists of subjects with several training modules each. Each training module consists of the following elements:

- **Overview**: Each training module starts with an overview of the major topics: Objectives (What shall be conveyed?), Benefit (What can this knowledge be used for?), and Maxims (Which correlations are to be remembered?).
- **Concepts**: First, the concepts and terms of the corresponding training module will be explained. This is followed by examples and instructions.
- **Exercises**: For some of the training modules, exercises with certain tasks and suggested solutions are available.
- **Cross-references**: At the end of each training module there is a section with cross references pointing out additional information in the software reference and in other sections. This will help you to extend your newly acquired knowledge.

### Display Conventions
Certain parts of sentences are specially marked. The meanings are:

| Convention | Meaning |
| :--- | :--- |
| *Italic* | marks character strings describing the software elements, e.g. the *Stock info* dialog. |
| **Bold** | marks character strings to be entered via keyboard, e.g.: Enter the value **0**. |
| > | The so-called breadcrumb trail shows how to open a dialog, e.g. *Production > Capacity planning > Control station*. |
| [ ] | Square brackets mark buttons in a dialog, e.g. [OK] to save the data. |
| < > | Angle brackets refer to keys or shortcuts on the keyboard, e.g. `<F1>` is used to open the online help. |

**Reading instructions**
The contents of a training module are based on the knowledge conveyed in the previous module. We therefore recommend not to skip any training modules.
If you are already familiar with a subject you should at least read the summary at the start of a training module to bring the main details to mind.

### Menu Overview
The capacity planning module in A+W Business Pro consists of two areas: the setup of capacity planning and the planning and monitoring of capacities. The associated dialogs are in the Capacity planning and Production modules. Both modules are introduced briefly.

**Capacity Planning Module**
In the *Capacity planning* module, you set up the master data and other specifications for planning the capacities.

