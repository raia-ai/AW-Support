---
description: "A+W Business (PRO) - Door Entry: Fitting and Processings"
---


# A+W Functional Description
# A+W Business (PRO) - Door Entry: Fitting and Processings

---
## 1. Content

1.  **Content**
2.  **Notes on this Document**
    1.  Trademarks
    2.  Copyrights
    3.  Exclusion of liability
3.  **Performance Description**
    1.  Data
    2.  Description
    3.  Requirements
    4.  List of functions
    5.  Restrictions
    6.  Notes
4.  **Contact Address**

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The greatest care was used in compiling the texts and figures. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2016, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Without the prior written permission of A+W Software GmbH, the documentation may not be transmitted electronically, by recording or in any other form.

### 2.3. Exclusion of liability

A+W Software GmbH assumes no liability for data errors that rely on basic principles of the standard functions made available by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All adjustments, expansions, database queries, reports, analyses, and interface expansions that were created individually for our customers and/or machines and software partners as well as all costs and efforts associated with these were borne by the client (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary in order to ensure that the adjustments/expansions commissioned that were undertaken/developed for a version will also work perfectly and be used in the subsequent version.

## 3. Performance Description

### 3.1. Data

| Product | A+W Business (Pro) |
| :--- | :--- |
| **Module number** | 210035, 230025 |
| **Module** | Door Order Entry: Fitting and Processings |
| **Brief description** | This module simplifies the entry of glass door fittings and processings. |
| **Available** | Starting with A+W Business (Pro) v6.0 |

### 3.2. Description

The A+W Business module "Door Order Entry: Fitting and Processings" is a module for the automatic entry of processings that are required for the affixing of fittings to a glass sheet.
For this purpose, in the master data, fittings can be entered with processings and the associated processing parameters in the master data. If the fitting is then added to the BOM via the processing entry, the associated processings are added to the BOM with the defined values (or calculation of the values using dimension formulas). If the fitting is changed or deleted, the associated processings are also deleted or changed.
The assignment is done taking into consideration the hinge side (studio doors).

### 3.3. Requirements

*   A+W Business (core module)
*   Master data creation for the assignments.
*   Training of the module.
*   Possibly: report adjustment for items in the BOM (fittings)

### 3.4. List of functions

*   Assigned processings of a fitting are inserted with it into the BOM.
*   When deleting a fitting, the assigned processings are also removed.
*   When exchanging the fitting, the assigned processings are also exchanged.
*   By changing the hinge side (studio doors), all processings are replaced with the appropriate processings for the other side.
*   Automatic fitting exchange due to hinge side change (e.g. locks, if different items for other hinge side).
*   Multiple entry of processings for a fitting based on priority, that is, if the same fitting is inserted several times, the processing assignments are determined by priority. (e.g. door hinge first top, then bottom, then middle)
*   Text generation: linking of processing texts and fittings (text formula; option)
*   Product search for fittings by "fitting type" (e.g. lock).
*   Change of the variant (color) for all fittings simultaneously.

### 3.5. Restrictions

*   The master data must have been created by the customer.
*   The fittings are inserted into the BOM of the item and not attached as individual items.
*   Only the entry for rectangles is supported (shape 0 or shapes with diagonal edge). For other shapes, the behavior is not defined clearly.
*   The logic is only implemented in the course of the processing entry in the item; not for EDI.
*   It only affects the item in which the fittings are entered; not adjacent sheets (GGA)

### 3.6. Notes
*(This section is intentionally blank in the source document.)*

## 4. Contact Address

**A+W Software GmbH**

Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com
Internet: http://www.a-w.com/
