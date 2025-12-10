---
description: "A+W Business - Reject Handling for Purchase Orders"
---


# A+W Functional Description: A+W Business - Reject Handling for Purchase Orders

---
## Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2017, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH assumes no liability for data errors that rely on basic principles of the standard functions made available by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Business |
| **Module number** | 210015 |
| **Module** | Reject Handling for Purchase Orders |
| **Brief description** | Reordering of defective purchased parts during production |
| **Available** | Starting with A+W Business 5.5/6.0; A+W Production 6.0 |

### 3.2. Description

For the breakage of a purchased sheet in A+W Production, a report can be made to A+W Business. The breakage report is made with A+W Production Terminal or a scanner reading. The report includes the name and type of the breakage state from the A+W Production master data and the information whether no reorder is required due to an excess quantity. Using the breakage state, A+W Business detects whether the break happened in production or whether it was broken on delivery.

If it is determined during production that a purchased glass cannot be used or if this glass breaks during production, a message is sent to the ERP system. With this message, employees in order/purchase order entry are informed and a reorder can be generated on a separate dialog. There are three possibilities for the generation:

- **Reorder:** if the defect is the fault of production, a for-cost reorder can be generated.
- **Complaint:** if the defect is the fault of the supplier, a free complaint can be created.
- **Value allocation:** if the defect is the fault of the supplier, but the purchased part should not be reordered, a credit request for the supplier can be created.

### 3.3. Requirements

- A+W Production (Barcode Manager)
- A+W Business (core module)
- The functionality requires a connection from A+W Business via the PPS Webservice to the production system.
- The fileless reporting must be activated.

### 3.4. List of functions

- Notification of employees in case of breakage of purchased parts in production.
- Generation of reorders and complaints for purchased parts.
- Reduction of the item quantities (commercial subquantity) if purchased part is not reordered.
- In A+W Business, the actions for the reported breakage reasons can be pre-set.

### 3.5. Restrictions

- If due to the breakage report for the purchased sheet a remake item is generated in A+W Production, there is no report.
- The reduction of the item quantity in case of broken subpart is not automatically supported by the system.

### 3.6. Notes
*(No content provided in this section.)*

## Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

**Tel:** +49 641 96620-0
**E-mail:** info@a-w.com
**Internet:** http://www.a-w.com/
