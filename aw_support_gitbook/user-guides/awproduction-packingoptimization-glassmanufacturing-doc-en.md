---
title: "EN_AWProduction_PMO_2.00"
source: "EN_AWProduction_PMO_2.00.pdf"
tags: ["A+W", "Packing Optimization", "Software Manual", "Glass Manufacturing", "Window Manufacturing", "Logistics", "PMO", "PackView"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical manual for A+W Packing Optimization, a software module for A+W Production. It details the processes for optimizing the packing of glass, windows, and doors onto racks and boxes to save space, reduce sorting time, and streamline logistics."
long_description: "This document is a comprehensive guide to the A+W Packing Optimization (PMO) software, a component of the A+W Production suite. The manual is intended for end-users and provides a thorough overview of the software's functionality, from basic concepts to advanced features. It begins with a tutorial section that explains the core idea behind packing optimization: adapting the production process for direct packing to maximize the use of transport racks and boxes. It covers different packing structures (tree and matrix), the role of master data files like .RUL (Optimization Rules) and .VAL (Settings), and the various parameters that control the optimization. The guide walks users through the software's user interface, including the Packing Group View for managing packing jobs and the PackView tool for 3D visualization and manual editing of packing results. The software reference section provides a detailed breakdown of all menus, dialogs, icons, and fields, serving as a complete reference for users. This includes creating and managing packing groups, optimizing them, and manually adjusting the results in different editing modes (Full Screen, Edit, Expert, Free Edit)."
---

# A+W Packing Optimization

---
## Introduction
In this part of the documentation you can find editorial notices.

### Revision Overview

| Packing Optimization Version / Date | Description |
| :--- | :--- |
| 2.00 / 01-2023 | Free edit mode added. |
| 1.02 / 01-2017 | Product and company names adjusted. |
| 1.01 / 07-2013 | Layout adapted to CI 2013. |
| 1.00 / 03-2007 | Original version. |

### Editorial
The editorial contains the following themes:
- Notes on this document
- Copyrights
- Trademarks
- Contact

#### Notes on this document
This document is intended only for end users of A+W Production.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and is subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The descriptions in this document are based on the full installation of A+W Production.

#### Copyrights
© 2023, Product and company names adjusted., any right, also the right of reprint, the production of copies and of the translation, is reserved. The documentation must be copied, completely or in part, saved, or transferred only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without Product and company names adjusted. prior approval in writing.

#### Trademarks
Any designation of hardware and software being mentioned in the documentation can also be registered trademarks or other commercial rights of third parties being protected by law. Rights of third parties being protected by law are to be observed insofar.

#### Contact
**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
+49 6404 2051-0
+49 6404 2051-877
Zentrale@a-w.com
http://www.a-w.com

## Tutorial

### The Basic Idea
Packing optimization saves tedious resorting as well as the temporary stock. It adapts the entire production process to **Direct packing** and to the optimum use of the racks and boxes.

In a production without packing optimization (PMO), all units produced are put into a temporary stock. After that, the units have to be packed onto transport racks which requires time-consuming sorting. Mostly, the units in the temporary stock are not available in the sequence required for the transport rack. It may also be the case that the transport rack has to be loaded according to the customer's instructions, or you have to stick to a certain route or unloading sequence.

The task of the packing optimization is to distribute the corresponding order items onto racks, taking into account all defined conditions, that as little transport space as possible is needed and the customer's requirements regarding the rack load are fulfilled. The scheduling strategy is defined by the packing rules. Apart from information on the physical properties such as height, width, and weight, these include customized parameters for the racks to be used such as the number of stacks that can be loaded next to or on top of each other.

Packing optimization splits orders into groups that are going to be packed together (packing groups), e.g. same delivery date, same route, same shipping address.

### General
This chapter describes the structure of the packing optimization (PMO) and how it basically works. The master data of the packing optimization are complex and its proper implementation requires specialist knowledge.

Packing optimization includes two definition areas which have to be handled separately:
- The physical conditions (rules), that must be kept at dispatch (weight, arrangement of stacks, distances, etc.)
- Order treatment (grouping, sorting, loaded on special racks, etc.) required by the customer.

For the customer, the focus mostly lies on the unloading sequence of the transport racks. The more rigid the restrictions for this sequence, the less freedom is left for the packing optimization when planning the racks. The planning density is apt to become worse as a result.

A frequent requirement is to unload units together. All units of the same order shall be unloaded together for example. Or all units of an item shall be unloaded in a row. It is not even sure that units to be unloaded together are even close to another on the racks. It may well be that the units have been put into different stacks or even different racks. The optimization always makes sure that no other units have to be unloaded before you get at the units that shall be unloaded together. The more freedom is given to the optimization, the better the planning density on the racks, and the less racks will be needed.

A packing group can be split into sets (corresponding to the orders). This means that the items of a set can be unloaded without having to unload other items first. The set may be distributed to different stacks or racks. The unloading sequence of the sets can be defined by the packing optimization, or can be set. You can also plan the sets so that the unloading sequence is random.

Stacks on the rack have to have a **tree structure**, e.g. starting with a big stack, followed by maximally two stacks in front of which can, again, be maximally two stacks. From the top, this looks like that (the back of the rack is shown in grey):

*Fig. 1-1: Rack load, top view*
