---
description: "EN-FUNC-AW_Enterprise_Internal_EDI"
---


# A+W Functional Description: A+W Enterprise - Internal document transfer

**A+W - Software for Glass**

---

---
## 1. Content
- **1. Content**
- **2. Notes on this Document**
  - 2.1. Trademarks
  - 2.2. Copyrights
  - 2.3. Exclusion of liability
- **3. Performance Description**
  - 3.1. Data
  - 3.2. Description
  - 3.3. Requirements
  - 3.4. List of functions
    - 3.4.1. Automatic transfer
    - 3.4.2. Change service
    - 3.4.3. Dependent order number at the production company
    - 3.4.4. References
    - 3.4.5. Reports
    - 3.4.6. Free customer orders
    - 3.4.7. Price transfer
    - 3.4.8. Transfer of attached documents
    - 3.4.9. Responsible employee for the document transferred
    - 3.4.10. Extended workbench (ordered processings)
    - 3.4.11. Location-spanning PDC
  - 3.5. Limitations
  - 3.6. Notes
- **4. Contact Address**

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

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
|---|---|
| **Product** | A+W Enterprise |
| **Module number** | No stand-alone module / Component of the basic functionality |
| **Module** | Document transfer |
| **Brief description** | Transfer of orders and POs between associated companies |
| **Available** | In all current versions |

### 3.2. Description
The "internal document transfer" is a module for the automatic transfer of POs to an associated company that also works with A+W Enterprise. The process for transferring documents can be done both completely automatically as well as partially manually.

With this module, the purchasing process, especially for companies with different production and retail locations, is simplified and speeded up. In addition, manual entry errors are reduced. With the expansion of the "status report" all participating companies always know what the current status of their orders is.

### 3.3. Requirements
To use this module, harmonized item master data is required. The same item numbers must refer to the same product structure. In addition, the computers of the participating sites must be accessible via ftp. At the start, the use of this module requires extensive process consulting and configuration by our project department.

### 3.4. List of functions
The "internal document transfer" is divided into 2 basic transfer processes, order linking and PO transfer.

For the order linking, a production order is created at the production company based on the sales order in the retail company.

For the order transfer, an order is initially created at the retail company based on the sales order. A production order is then generated at the production company based on the PO.

In addition, it is possible to shift orders to a test system. This function may not be enabled permanently, since it is not possible to process orders in productive system and shift these to the test system simultaneously.

#### 3.4.1. Automatic transfer
The system can be configured so that the document to be transferred is transferred to the associated company immediately after its creation or release.

#### 3.4.2. Change service
As long as none of the dependent documents includes a lock status, changes on the underlying order are transferred automatically to the dependent documents.

#### 3.4.3. Dependent order number at the production company
The system at the production company can be configured so that the order number at the production company is generated with an offset from the document number at the retail company. This means that for the order linking, the order number at the production company is based on the order number at the retail company. For the PO transfer, the order number at the production company is based on the PO number at the retail company.

Alternatively, for orders that are received via internal document transfer, an individual number range for the assignment of the local order number can be used.

> **Warning:** When using order coupling with offset, it is not possible to work with breakage POs from production. Furthermore, this function for order coupling can no longer be used for multisite installations.

#### 3.4.4. References

**External customer reference**
The assignment of the external customer reference can be configured individually. It can assume the following values:
- Document number of the document transferred by the sending company
- PO number of the ordering company
- Order and PO number of the sending company
- PO and order number of the sending company
- Unchanged transfer of the external customer reference from the document to be transferred.
- When using the PO transfer, it must be heeded that during the PO generation, the external customer reference of the order is not retained; instead, it is overwritten with new values in the PO.

**Reference to the underlying document**
At the production company, the reference to the directly underlying document (order or PO) is visible.

**Reference to the end customer address**
At the production company, the end customer address is visible. This means that it can be detected at the production company to whom the goods shall be sent in the end. This is also visible if the production company delivers to the retail company and not directly to the end customer.

#### 3.4.5. Reports
Within the internal EDI, processing status and production status in the documents in the retail company are transferred from the production company.

#### 3.4.6. Free customer orders
If a document is marked as free, this identifier is transferred to the production site. However, a "free order" does not automatically become a "free PO". However, a PO set manually to "free PO" becomes a free order at the production company.

#### 3.4.7. Price transfer
The system can be configured so that the purchase price of the retail company applies as sales price at the production company.

#### 3.4.8. Transfer of attached documents
Within the PO transfer, attached documents and motif files can be transferred. Attached documents are documents attached to the order manually on the order or item level. Motif files are image files for special glass processings.

#### 3.4.9. Responsible employee for the document transferred
By default, the document transferred counts are created by the system. With appropriate system configuration, it is possible to define that another employee is defined as responsible for these documents.

#### 3.4.10. Extended workbench (ordered processings)
If only a processing on included glass to be delivered should be ordered, the functionality of the "extended workbench" is required. This functionality is then available exclusively with the PO transfer.

#### 3.4.11. Location-spanning PDC
The location-spanning PDC enables the transfer of a label number and the PDC quantity identifier to individual locations, each of which has its own production system and therefore cannot process the labels from the other system. This functionality is available exclusively with the PO transfer.

### Function Comparison Table

| Function | Order linking | PO transfer |
| :--- | :--- | :--- |
| **a) Automatic transfer** | X | X |
| **b) Change service** | X | X |
| **c) Dependent document number at the production company** | Offset based on original order number<br>No automatic breakage PO from production possible<br>Cannot be used for multisite | Offset based on original PO number |
| **d) a. Retention of the external customer reference on through to the production order** | X | - |
| **e) Status reports** | X | X |
| **f) "Free order" at the retail company automatically becomes a free order at the production company** | X | - |
| **g) Purchase price becomes sales price** | X | X |
| **h) Transfer of attached files** | - | X |
| **Transfer of motif files** | - | X |
| **i) Special function for determining the responsible employee of a transferred PO** | - | X |
| **j) Ordered processings** | - | X |
| **k) Location-spanning PDC** | - | X |
| **Discounts (configuration: RABATTLOGIK_2005)** | - | Will be determined anew at the receiving company |
| **Transfer of delivery route from the customer order to the production order** | X | - |

### 3.5. Limitations

### 3.6. Notes

## 4. Contact Address
**A+W Software GmbH**  
Siemensstraße 3  
35463 Fernwald  
Germany

**Tel.** +49 641 96620-0  
**E-mail:** info@a-w.com  
**Internet:** http://www.a-w.com/
