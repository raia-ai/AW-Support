---
description: "A+W Multisite PO Tracking"
---


# A+W Functional Description: A+W Multisite PO Tracking

**A+W - Software for Glass**

---

---
## 1. Content

1.  **Content**
2.  **Notes on this Document**
    *   2.1. Trademarks
    *   2.2. Copyrights
    *   2.3. Exclusion of liability
3.  **Performance Description**
    *   3.1. Data
    *   3.2. Description
    *   3.3. Requirements
    *   3.4. Function list
    *   3.5. Limitations
    *   3.6. Notes
4.  **Contact Address**

---

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2019, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions that have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220089 |
| **Module** | A+W Multisite PO Tracking |
| **Brief description** | Location-spanning tracking of ordered glass |
| **Available** | Starting with version v6 |

### 3.2. Description

With the **A+W Multisite PO Tracking** module, it is possible to track order glass between the individual operations via PDC in A+W Production. This is done by ensuring that the ordering and producing locations receive the same bar code number for the products ordered.

This functionality is available only in connection with A+W Enterprise and A+W Business.

### 3.3. Requirements

It must be guaranteed that the label ID ranges in each location are separate. Only this way can it be ensured that the label ID from location A is not already used in location B.

The separation of the label IDs can be done in various ways. In each operation, you can set the smallest and largest label value in the parameters. Depending on the overlap of the label IDs, the following scenarios emerge:

**a) No overlap of the label IDs**

This situation is easiest to resolve because the label ranges are already unique for each operation.

| | Label IDs | A | B | C | D | E | F | G | H | I | J |
| :--- | :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| **Actual situation** | Location A | 🟨 | 🟨 | 🟨 | | | | | | | |
| | Location B | | | | | 🟨 | 🟨 | 🟨 | | | |
| **Restriction** | Location A | | | | | | | | | | |
| | Location B | | | | | | | | | | |

**b) Unique overlap of the label IDs**

| | Label IDs | A | B | C | D | E | F | G | H | I | J |
| :--- | :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| **Actual situation** | Location A | 🟨 | 🟨 | 🟩 | 🟩 | | | | | | |
| | Location B | | | 🟩 | 🟩 | 🟨 | 🟨 | | | | |
| **Restriction** | Location A | 🟨 | 🟨 | | | | | | | | |
| | Location B | | | | | 🟨 | 🟨 | | | | |

This situation is also reasonably easy to resolve (depending on the size of the overlap). Important here is that the current jointly-used ranges (gray) may not be used at the beginning.

**c) Scattered overlap of the label IDs**

This situation is more difficult to resolve because in the parameters for each operation, you can only ever enter a start and end number for the labels. That is, the final usable label range must be coherent. The jointly-used ranges may not be used at the beginning under any circumstances! If both operations move only in the restricted label ID ranges, the restriction set can be expanded again.

| | Label IDs | A | B | C | D | E | F | G | H | I | J |
| :--- | :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| **Actual situation** | Location A | | 🟨 | 🟩 | | | 🟩 | | | | |
| | Location B | | | 🟩 | 🟨 | 🟨 | 🟩 | 🟨 | | | |
| **Restriction** | Location A | | 🟨 | | | | | | | | |
| | Location B | | | | 🟨 | 🟨 | | 🟨 | | | |

**d) Too-large overlap range of the label IDs**

Situations can also arise with which the overlaps are so large that there are not enough label IDs left for the individual operations. In this situation, you can only put the module into operation in several steps. That is, in the first step, the label IDs are restricted as described above. This ensures that future orders will remain in this range of label IDs. There should be fewer and fewer jointly-used ranges, so that later in a 2nd step, the full functionality can be switched on.

| | Label IDs | A | B | C | D | E | F | G | H | I | J |
| :--- | :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| **Actual situation** | Location A | 🟨 | 🟩 | 🟩 | 🟩 | 🟩 | | | | | |
| | Location B | | 🟩 | 🟩 | 🟩 | 🟩 | 🟨 | 🟨 | | | |
| **Restriction** | Location A | 🟨 | | | | | | | | | |
| | Location B | | | | | | 🟨 | 🟨 | | | |

### 3.4. Function list

1.  The end customer places an order in Location A. This order is entered in A+W Enterprise and
2.  transferred to A+W Production.
3.  In A+W Production, the necessary label IDs for the individual components are determined
4.  Now, an order is triggered from A+W Production in A+W Enterprise, for which the start label ID* determined for the parts ordered is transferred too.
5.  Location A now orders the necessary components in Location B and forwards the start label ID in the process.
6.  The order is now transferred to A+W Production and the required label IDs are calculated there based on the starting label ID and the item quantity. Thus, the label IDs for the ordered parts are identical in both locations.
7.  After production, the ordered parts are packed and
8.  delivered to the Location A
9.  Here, the parts delivered can be entered in incoming goods and repacked if necessary. The labels can be processed both with the scanners and with A+W Production Terminals. Ideally, series are booked with an A+W Production Terminal.
10. After that, they are delivered to the end customers.

***
*Start label ID: the smallest label ID of a part of an item. The other label IDs can be calculated with this start label ID and the item quantity.
***

**Process Flow Diagram:**

The document includes a diagram illustrating the 10-step process described above.
- **Step 1:** An order is placed by the customer (Kunde) at Plant A (Werk A).
- **Steps 2-4:** The order is processed in Plant A's system, and label IDs are determined.
- **Step 5:** Plant A places an order for components with Plant B (Werk B).
- **Step 6:** Plant B processes the order using the same label IDs.
- **Steps 7-8:** Plant B produces and ships the components to Plant A.
- **Step 9:** Plant A receives the components.
- **Step 10:** Plant A delivers the final product to the customer.

This technique works in both directions and can also be used for several plants (>2). However, each additional plant restricts the labels available. That is, for the separation of the label ID ranges, you must pay careful attention that each operation has enough labels available for an appropriate time period.

At the moment, the following flows are possible:

-   Normal transfer, e.g. of an ISO with an ordered TG (the label ID is transferred to the 2nd location and is the same for the TG in both systems). It is also checked whether a generated label is already or still in use. However, this check is only done if the start label ID should be assigned for the first time (e.g. after activation of the features or in case of an overrun of the range).
-   If the order has not yet been started (it is planned), changes can still be made to the main order, which also arrive in the production site and are reported to the production system there accordingly.
-   Scheduling-NL functionality is possible both in the producing and in the ordering production system. With the latter, a remake order is triggered, which is transferred to the 2nd production system. There, internal check routines are run, which report for this case the already-existing label of the original 1st order as broken, so that the scheduling remake can be produced again with the label.

### 3.5. Limitations

Currently, there are the following restrictions:

-   The quantities PDC is not supported.
-   As soon as production has begun in Location B (planning), then the order in A+W Enterprise are in local correction. Therefore, cancellations will not be created automatically. Here, the operator can only act manually (e.g. inform plant B by telephone).
-   The Surplus dialog may not be used since otherwise labels are created that the ordering plant does not recognize.
-   Rack-related goods receipt is not supported.
-   The same ERP system must be used in the plants involved (i.e. either A+W Enterprise or A+W Business).

### 3.6. Notes

*(This section is empty in the source document.)*

---

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0
E-mail: info@a-w.com
Internet: http://www.a-w.com/
