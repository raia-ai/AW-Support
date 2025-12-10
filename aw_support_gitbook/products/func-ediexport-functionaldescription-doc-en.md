---
description: "EN-FUNC-AW_Enterprise_EDI_Export"
---


# A+W – Enterprise: Export in the A+W standard format
---
### A+W Functional Description

---

## 1. Contents

1.  **Contents**
2.  **Notes on this Document**
    *   2.1. Trademarks
    *   2.2. Copyrights
    *   2.3. Exclusion of liability
3.  **Performance description**
    *   3.1. Data
    *   3.2. Description
    *   3.3. Requirements
    *   3.4. List of functions
    *   3.5. Restrictions
    *   3.6. Notes
4.  **Contact Address**

---

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. **A+W Software GmbH** cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. Third party copyrights must be observed.

### 2.2. Copyrights

© 2021, **A+W Software GmbH**, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of **A+W Software GmbH**.

### 2.3. Exclusion of liability

**A+W Software GmbH** does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

**A+W Software GmbH** reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions that have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions that have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance description

### 3.1. Data

| **Product** | **A+W Enterprise** |
| :--- | :--- |
| **Article no.** | 200012 |
| **Module** | EDI Export |
| **Brief description** | Export of POs in the A+W standard format |
| **Available** | Starting with A+W Enterprise 6 (June 2021) |

### 3.2. Description

With appropriate configuration, existing POs can be exported in a file in the A+W standard format. To learn which data records are exported and how the individual fields are filled, see the interface description "EN-A+W EDI Import.pdf" section "A+W Enterprise Export-specific field notes" and the configuration instruction "EN-CONFIG-A+W Enterprise EDI.pdf" section "PO export/A+W EDI Export".

The configuration of the export can be tailored to the supplier.

### 3.3. Requirements

*   A+W Enterprise (core module)
*   Use of the A+W processing types

### 3.4. List of functions

*   Creation of an interface file in a configured directory with a configurable name
*   Export of the defined data records
*   Supplier-individual details can be output via individual stored procedure
*   Record types that are currently written
    *   FH - File header record
    *   K1 - Header record general
    *   K2 - Header record customer address
    *   K3 - Header records delivery address
    *   P1 - Item
    *   P2 - Item
    *   P3 - Item
    *   BC - Barcode
    *   S1 - BOM
    *   B1 - Processing parameters
    *   C1 - Muntin record
    *   CA - Muntin record asymmetrical
    *   M1 - Shape record
    *   T1 - Text record item
    *   T2 - Text record document

### 3.5. Restrictions

The export writes the data records to the interface file according to the specification. However, attention must be paid that the import of this file cannot be done 1:1 in all A+W products. In some cases, the functional scope of the export is greater than the import of the individual modules.

These restrictions affect:

a) Only POs are exported

b) Not all BOM elements are exported as S1 record:
    *   **Glass:** For multiple glasses, the glass of the first BOM level is always exported. If the first BOM level is a stock size (e.g. LAMI), then the 2nd BOM level is exported.
    *   **Foils:** Foils are only exported if the EA flag is set.
    *   **Spacer/AIR:** Spacers are always exported.
    *   **Muntins:** Muntins are always exported.
    *   **Accessory:** Accessories are only exported with set EA flag.
    *   **Processings:** Processings are only exported if the EA flag is set.
    *   **Steps:**
        Caution: The step export to A+W Business is not supported.
        Otherwise, steps are always exported
    *   **Gas:**
        Caution: The export of mixed gases to A+W business is not supported.
        Otherwise, gas is always exported.
    *   **Shapes:** The shape S1 record is not always absolutely necessary. Frequently a M1 record is sufficiently. Therefore, the S1 record for shapes is only exported if it was configured via the special shape S1 record stored procedure (see "EN-CONFIG-A+W Enterprise EDI.pdf")

c) BOM record S1 – field "Item on level": This field is not filled for
    *   Gas
    *   Step
    *   Muntins
    *   Processings
    *   Accessory
    *   Shape
    
    since this information is not available. If a storage of this information is absolutely necessary, this must be agreed upon with A+W before start-up.

d) Foils can be exported but not imported into A+W Enterprise.

e) Processings and glass exchange on deeper BOM levels are not imported in A+W Enterprise.

f) For LAMI, all glass can be exported, but only 3 can be imported into A+W Enterprise.

g) Muntin items can be exported, but not imported into A+W Enterprise.

h) Not all A+W processing types supported in A+W Enterprise are exported. The supported A+W processing types are documented in the interface description "EN-A+W EDI Import". Furthermore, not all exported A+W processing types are imported. The supported A+W processing types in the import are documented in the interface documentation "EN-A+W EDI Import".

Generally, exports for A+W Business must be tested in advance on a case by case basis since the BOM requirements can differ significantly.

### 3.6. Notes

Currently, there is no automatic transfer of the files to the supplier.

---

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-Mail: info@a-w.com
Internet: http://www.a-w.com/
