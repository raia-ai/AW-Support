---
description: "EN-FUNC-AW_Enterprise_openTRANS_Export"
---


# Document Transfer in openTRANS Format 2.1

---
## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2017, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Enterprise |
| **Module Number** | 200024 |
| **Module** | Document Transfer in openTRANS Format 2.1 |
| **Brief description** | Module to export quotations, invoices/credit notes, and delivery notice in openTRANS 2.1 format |
| **Available** | Starting with A+W Enterprise v6 |

### 3.2. Description

Document Transfer in openTRANS 2.1 is a module for exporting order confirmations, delivery notices, and invoices/credits in the openTRANS 2.1 format.

openTRANS 2.1 is an open standard for support of electronic data exchange for business transactions between trading companies. By using the module, trade partner can make business documents available automatically in a standardized format. Documentation of the openTRANS 2.1 standard is available on the Internet site www.opentrans.de.

### 3.3. Requirements

- This module is available only in connection with A+W Enterprise.

| A+W Enterprise B2B Service | A+W Enterprise | Note |
| :--- | :--- | :--- |
| Version 6 or higher | Version 6 or higher | An expansion of the transaction SQL is required for operation. |

### 3.4. List of Functions

- Export of invoices/credit notes
- Export of order confirmations
- Export of delivery notice

### 3.5. Restrictions

- The delivery notice is created analogous to the advance delivery not based on the data from dispatch control.
- As soon as a delivery note exists in the system, no more delivery notice can be generated for it.
- Other document types than the ones listed in the function list are currently not exported, even if they are included in the openTRANS 2.1 standard.
- The documents are not signed electronically.

### 3.6. Notes

Programs from different providers interpret individual fields differently than the standard. For this reason, for-fee adjustments may be required in individual cases.

A+W Cantor can process the documents generated.

The data mapping between A+W Enterprise data and the elements of an export document is described in separate documentation.

With the order confirmation, only quantities, items, and dates are confirmed. The product structure and changes to the BOM are not transmitted (are not provided in the standard).

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0
E-mail: info@a-w.com
Internet: http://www.a-w.com/
