---
title: "EN-FUNC-AW_Business_OpenTRANS_Export"
source: "EN-FUNC-AW_Business_OpenTRANS_Export.pdf"
tags: ["A+W", "openTRANS", "Data Export", "ERP", "Software", "Functional Description", "Glass Industry", "A+W Business", "EDI", "Document Transfer"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a functional description for the A+W Business software module, 'Export of documents in the openTRANS format 2.1'. It details the module's capability to export key business documents such as order confirmations, invoices, credit notes, and delivery notices using the standardized openTRANS 2.1 format. The document outlines the module's functions, requirements, restrictions, and provides essential notes for implementation."
long_description: "This functional description provides a comprehensive overview of the A+W Business module designed for exporting business documents in the openTRANS 2.1 format. The module, named 'Document Transfer in openTRANS Format 2.1,' is available starting with A+W Business v6. It facilitates electronic data interchange (EDI) between trading companies by allowing for the automated and standardized export of critical documents, including order confirmations, invoices, credit notes, and delivery notices. The document specifies the scope of the module, listing the exact functions provided, such as the export of specific document types. It also clearly states the restrictions, noting that other document types included in the openTRANS 2.1 standard are not supported and that the exported documents are not electronically signed. Additionally, it highlights requirements, like the necessity of having A+W Business v6, and includes important notes regarding potential needs for for-fee adjustments due to different interpretations of the standard by various providers. The document concludes with legal disclaimers, copyright information, and contact details for A+W Software GmbH."
---

# A+W Functional Description: Export of documents in the openTRANS format 2.1

---
## 1. Contents

1.  **Contents**
2.  **Notes on this Document**
    - 2.1. Trademarks
    - 2.2. Copyrights
    - 2.3. Exclusion of liability
3.  **Performance Description**
    - 3.1. Data
    - 3.2. Description
    - 3.3. Requirements
    - 3.4. List of functions
    - 3.5. Restrictions
    - 3.6. Notes
4.  **Contact Address**

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | **A+W Business** |
| **Module number** | |
| **Module** | **Document Transfer in openTRANS Format 2.1** |
| **Brief description** | **Module to export order confirmations, invoices/credit notes, and delivery notice in openTRANS 2.1 format** |
| **Available** | **Starting with A+W Business v6** |

### 3.2. Description

Document Transfer in openTRANS 2.1 is a module for exporting order confirmations, delivery notices, and invoices/credits in the openTRANS 2.1 format.
openTRANS 2.1 is an open standard for support of electronic data exchange for business transactions between trading companies. By using the module, trade partner can make business documents available automatically in a standardized format. Documentation of the openTRANS 2.1 standard is available on the Internet site www.opentrans.de.

### 3.3. Requirements

- This module is available only in connection with A+W Business v6.

### 3.4. List of functions

- Export of invoices/credit notes
- Export of order confirmations
- Export of delivery notice

### 3.5. Restrictions

- Other document types than the ones listed in the function list are currently not exported, even if they are included in the openTRANS 2.1 standard.
- The documents are not signed electronically.

### 3.6. Notes

Programs from different providers interpret individual fields differently than the standard. For this reason, for-fee adjustments may be required in individual cases.

With the order confirmation, only quantities, items, and dates are confirmed. The product structure and changes to the BOM are not transmitted (are not provided in the standard).

## 4. Contact Address

**A+W Software GmbH**  
Siemensstraße 3  
35463 Fernwald  
Germany

**Tel.** +49 641 96620-0

**E-mail:** info@a-w.com  
**Internet:** http://www.a-w.com/
