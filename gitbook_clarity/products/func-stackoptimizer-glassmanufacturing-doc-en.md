---
description: "EN-FUNC-AW_Stack_Optimizer"
---


# A+W Functional Description
# A+W Stack Optimizer

> **Discontinued**

**A+W - Software for Glass**

---

---
## 1. Contents

1.  **Contents**
2.  **Notes on this Document**
    *   2.1. Trademarks
    *   2.2. Copyrights
    *   2.3. Disclaimer of liability
3.  **Performance Description**
    *   3.1. Data
    *   3.2. Description
    *   3.3. Requirements
    *   3.4. List of functions
    *   3.5. Limitations
    *   3.6. Notes
4.  **Contact Address**

---

## 2. Notes on this Document

This documentation and the software described in it are only licensed and may only be used and copied pursuant to this license. The contents of the documentation are for information purposes only and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation may also be registered trademarks or other industrial property rights held by third parties. Copyrights of third parties must be complied with.

### 2.2. Copyrights

© 2016, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Disclaimer of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to perform changes to software data, structure and interfaces as part of program extensions without prior notice. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This also includes possibly necessary long-term costs and expenses for amending and extending subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220032 |
| **Module** | A+W Stack Optimizer |
| **Brief description** | Calculates the size of glass stacks and the number of required physical A racks |
| **Available** | Starting with A+W Production 5.5 |

### 3.2. Description

During the detailed planning, this product calculates the size of the glass stacks and the number of actually-required, physical A racks after glass cutting with the best possible yield for the configuration.

For each glass type/thickness combination, several possible solutions are displayed, the user can select the one best-suited for him, this can be, e.g. the optimization with the best yield or with the fewest physical racks.

### 3.3. Requirements

The A+W Stack Optimizer is called during the detailed planning so that A+W Production must be present in every case.

The A+W Stack Optimizer itself calls up the cutting and rack optimization.

For the rack optimization within the A+W Stack Optimizer, special master data must be maintained for the cutting rack.

### 3.4. List of functions

First, the detailed planning determines the requested production sequence for all lots participating in the batch (glass type/thickness combinations). After that, the results are transmitted to the Stack Optimizer, which now determines using various iterative procedures, the physical racks required for each lot. Here it is constantly ensured that the breakout sequence suits the production sequence previously determined by the detailed planning. With each iteration step, you get a result consisting of cutting and rack optimization, and thus the glass yield and number of physical racks required. The results of the respective iteration steps for each lot are displayed with the most important key figures in an individual user interface where the user can then select the suitable solution per lot.

In addition, the user can decide whether a lot should be set to hand cutting; in this case, the result of the Stack Optimizer is discarded for this lot.

### 3.5. Limitations

*   Currently there is a limitation on insulated glass lites.
*   Currently only one rack type can be used per batch.
*   For the determination of rack loading, there is currently only one mode for packing the rack as densely as possible. This can mean that the total space for the rack during cutting is not used, which in turn is yield-relevant.
*   Rack numbers are currently determined for this process in ascending order from 1, so that the usual number ranges for logical racks do not apply.

### 3.6. Notes

*(No notes provided in this section.)*

---

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com
Internet: http://www.a-w.com/
