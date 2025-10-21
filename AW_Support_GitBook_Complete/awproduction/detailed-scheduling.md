---
title: "EN_AWProduction_Detailed_Scheduling_3.00"
source: "EN_AWProduction_Detailed_Scheduling_3.00.pdf"
tags: ["A+W Production", "Detailed Scheduling", "Glass Manufacturing", "Window Production", "Door Production", "ERP", "MES", "Optimization", "Production Planning", "Software Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical manual for the Detailed Scheduling module of the A+W Production software. It provides comprehensive guidance for end-users on configuring and utilizing the software for efficient production planning in the glass, window, and door manufacturing industries."
long_description: "This manual serves as a comprehensive guide to the A+W Production 'Detailed Scheduling' module, version 3.00. It is intended for end-users, system administrators, and trainees involved in the production planning processes for glass, windows, and doors. The document is divided into two main parts: a Tutorial and a Software Reference. The Tutorial section offers a hands-on approach to learning the core concepts, including Grouping and Sorting, Racks and Stacking Modes, various Optimization Modes, and the setup of Organizations. It explains how to balance production sequence, yield, and flexibility to meet specific manufacturing requirements. The Software Reference section provides detailed descriptions of all dialogs, fields, and settings within the Detailed Scheduling module. It covers master data configuration for organizations, racks, groupings, lot types, and processing steps. It also details the functionality for handling special elements like filler orders, residue plates, and rejects. This guide is essential for understanding how to optimize production batches, manage rack allocation, and configure the system for maximum efficiency and minimal waste."
---

# A+W Detailed Scheduling

A+W Production

A+W - Software for Glass, Windows and Doors

## Introduction

In this part of the documentation you can find editorial notices.

### Revision Overview

| Part Version / Date | Description |
| :--- | :--- |
| 3.00 / 01-2023 | Complete revision. |
| 2.02 / 01-2017 | Product and company names adjusted, fields added |
| 2.01 / 08-2013 | Complete revision of the ALCIM documentation and adjustment to A+W Production. |
| 2.00 / 11-2012 | Complete revision. |
| 1.00 / 09-2007 | Original version. |

### Editorial

The editorial contains the following themes:

*   Notes on this document
*   Copyrights
*   Trademarks
*   Contact

**Notes on this document**

This document is intended only for end users of A+W Production.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and is subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The descriptions in this document are based on the full installation of A+W Production.

**Copyrights**

© 2023, A+W Software GmbH, any right, also the right of reprint, the production of copies and of the translation, is reserved. The documentation must be copied, completely or in part, saved, or transferred only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH prior approval in writing.

### Trademarks

Any designation of hardware and software being mentioned in the documentation can also be registered trademarks or other commercial rights of third parties being protected by law. Rights of third parties being protected by law are to be observed insofar.

### Contact

**A+W Software GmbH**
Am Pfahlgraben 4 - 10
D-35415 Pohlheim
Germany
📞 +49 6404 2051 0
📠 +6404 2051 877
Zentrale@a-w.com
http://www.a-w.com

## Tutorial

### Notes on the Documentation

The tutorial on module Detailed Scheduling deals with the basics of the whole production process. Starting from cutting, via the different production lines, up to the transport racks. It is based on the knowledge of rough scheduling.

> **The functions depend on the released modules**
> Please note that the individual functions are available only if the corresponding modules and interfaces have been installed and released.
> If you detect functions in this description which are not available in your version, please contact A+W Software GmbH.

**Sets of Topics**

The training on module Detailed Scheduling consists of the following sets of topics:

*   Grouping and Sorting
*   Racks and Stacking Modes
*   Optimization Modes
*   Organizations

### Important Notes

This documentation is meant as an aid for the daily business and as a training document for software training accompanied by a certified A+W trainer. It is not meant for self-studies and cannot guarantee an operation which is completely free of errors because the complexity does not depend on the software but rather on the real processes. Detailed scheduling defines the entire organization and production process within your production. According to your requirements, it can be quite complex which is why it will be exclusively set up by an experienced member of the A+W team, and installed together with you. Should you want to change the settings please always contact A+W first to avoid undesired effects!

The user has to be versed in the application of physical processes in glass production and organization.

**Product names**

In the course of strategic product realignment, the product range and product names of A+W have been simplified. *ALCIM* for instance has become *A+W Production*.

Since the old as well as the new product versions have been adapted and extended in the product development cycle, we shall be using only the old product names in this document to simplify matters - the new product versions are also covered by the old names.

### Documentation

Training on *A+W Production* is supported by the following documents:

| Hand-out | Printed training documentation for the participants |
| :--- | :--- |
| **PDF** | Complete documentation<ul><li>Tutorial</li><li>Software Reference</li><li>Index</li></ul> |
| **Online help <F1>** | Context-sensitive dialog help in the *A+W Production* software reference. |

### Tutorial Structure

This tutorial consists of sets of topics with several sessions each. Each session consists of the following elements:

| | |
| :--- | :--- |
| **Overview** | Each training session starts with an overview of the major topics:<ul><li>Objectives: What shall be conveyed?</li><li>Benefit: What can this knowledge be used for?</li><li>Maxims: Which correlations are to be remembered?</li></ul> |
| **Concepts** | Concepts and terms of the corresponding training session will be explained first. This is followed by examples and operating instructions. |
| **Exercises** | For some of the sessions, exercises with certain tasks and suggested solutions are available. |
| **Cross references** | At the end of each learning unit there is a section with cross reference pointing out the corresponding descriptions in the software reference.<br>This shall help you to extend your new-found knowledge. |

**Reading instructions**

The contents of a learning unit are based on the knowledge conveyed in the previous unit. We therefore recommend not to skip any learning units. The contents of a learning unit are based on the knowledge conveyed in the previous unit. We therefore recommend not to skip any learning units.

If you are already familiar with a subject you should at least read the summary at the start of the session in order to bring the main details to mind.

The practical part of each training unit automatically includes the software reference and the exercises on the cross references. This will provide a central thread through the entire documentation. The practical part of each training unit automatically includes the software reference and the exercises on the cross references. This will provide a central thread through the entire documentation.

### Display Conventions

Individual elements of the sentences are displayed in a special form. Their meanings are:

| | |
| :--- | :--- |
| *Italics* | mark character strings describing the software elements, e.g. the dialog *Grouping*. |
| **Bold** | marks phrases to be entered via keyboard, e.g. the number **0**. |
| > | shows the way to open a dialog, e.g. **File > Import > Transfer file**. **Master data > Detailed scheduling > Organization** |
| [] | Square brackets mark the buttons in the dialog, e. g. **[OK]** to save the data. |
| <> | Pointed brackets refer to keys or shortcuts on the keyboard, e. g. **<F1>** is used to open the online help. |

## Detailed Scheduling - Overview

The glass required for production is usually cut from stockplates on the cutting tables. Most companies have several, automatic cutting tables and at least one cutting table for manual cutting or shapes.

After cutting, the lites are put onto racks depending on the next processing step (e.g. A racks); the rack is then moved to the next processing station.

In a working area (e.g. cutting) or within a process chain (e.g. cutting > IG line), dwelling and processing times can very considerably. Among other things, this depends on the space available in this area for the racks onto which the lites are put, on the complexity of the stacking logic, and on the distance to be covered in between steps. These are essential questions in terms of *Detailed scheduling*. If there is only little space for the racks behind the cutting table, this fact must be compensated by the appropriate optimization and the sequence of lites so that as few racks as possible are needed and only little additional sorting is required.

For assembly on the IG line, the lites of a unit have to be stacked as closely together as possible. They do not have to be put onto the same rack however. This means that depending on the optimization, sorting may have to take place before the line.

