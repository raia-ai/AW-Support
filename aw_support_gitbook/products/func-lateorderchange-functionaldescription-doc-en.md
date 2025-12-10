---
title: "A+W Late Order Change Functional Description"
source: "EN-FUNC-AW_Enterprise_Late_Order_Change.pdf"
tags: ["A+W", "Late Order Change", "Software for Glass", "Functional Description", "A+W Enterprise", "Production Management", "ERP", "Order Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a functional description of the 'A+W Late Order Change' module for the A+W Enterprise software system. It details how the module enables users to modify non-technical order data, such as delivery information and routes, even after the production process has commenced. The functionality aims to improve the organization and flexibility of production and delivery workflows."
long_description: "This functional description outlines the capabilities, requirements, and operational details of the 'A+W Late Order Change' module (No. 200020), a for-fee extension for A+W Enterprise v6 and later. The module is designed to allow for the modification of select commercial data in A+W Production after an order has already entered the production phase. The document specifies the system requirements, including compatible versions of A+W Enterprise 5, A+W Production 5 (with Service Pack 5), and the A+W Enterprise 5 OrderXML Service. It classifies order modifications into three categories: purely commercial changes that remain local to the ERP system; informational changes (e.g., delivery address updates) that are forwarded to production without requiring new scheduling; and production-relevant changes (e.g., quantity, product specs) that necessitate rescheduling for unlocked items. The guide also covers restrictions related to system settings, logging mechanisms for changes, and notes that this is a Value+ function."
---

# A+W Late Order Change Functional Description

**A+W - Software for Glass**

---
## Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### Copyrights

© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### Disclaimer of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## Performance Description

### Data

| | |
| :--- | :--- |
| **Product** | A+W Enterprise |
| **Module number** | 200020 |
| **Module** | Late Order Change |
| **Brief description** | With this module, non-technical data can also be transferred to A+W Production even after production has already started. |
| **Available** | Starting with A+W Enterprise v6 |

### Description

With this module, non-technical data can also be transferred to A+W Production even after production has already started.

Select commercial data such as delivery data, address, and routes can be updated during ongoing production in A+W Production. This improves the organization of the production and delivery processes.

### Requirements

For the activation of this function, the following modules must be in versions that are compatible with one another.

- A+W Enterprise 5
- A+W Enterprise 5 OrderXML Service
- A+W Production 5

Both the PPS and the ERP system must be Version 5 with the Service Pack 5.

Minimum requirement for ORDERXML_VERSION is "5.2."

This module is a for-fee module that must be activated in the system. The A+W Enterprise system configuration may only be done after the update of A+W Production 5.5!

The use of the module may depend on other system settings. These will be discussed later in the document.

### List of functions

Three types of order changes in A+W Enterprise will be classified:
- Purely commercial changes
- Changes that are forwarded as information to production
- Production-relevant changes

#### Purely commercial changes

Such as prices, terms, user data, invoice and print options, payment options, etc.: these changes always remain local and are not forwarded, there is no query.

If another transfer is nevertheless desired, it can be made with the Renewed transfer to production menu element. For this transfer, no change in the order is required.

#### Changes that are forwarded to production as information

Such as packaging type, declaration of performance, file attachments, delivery address, customer address, delivery date (for locked orders): These changes can be taken over by all items and forwarded, even if they are already locked by ordering or production.
Thus, there is no new scheduling.

#### Production-relevant change that require new scheduling

Such as change to product, quantity, dimensions, delivery date, route, etc.: These changes are only possible for items that are not locked and are only forwarded for such. If there is only one comprehensive production-relevant change in the order, then the locked items have the identifier "no change" and are read over during takeover into production. Items with the procurement type "none" can also not get an identifier for the production-relevant changes. All newly-entered items in correction mode naturally count immediately as production-relevant, except those with the procurement type "none."

**Exception**: All items that are run on "error during scheduling" are set to "production-relevant" correction with each correction of the order.

The changes that set the status "info to production" or "production-relevant" are logged. This logging is not active by default, however, and it has to be activated. The reason for the transfer to production as well as the decision of the person whether the changes should be transferred to production is also logged. This logging runs by default.

The changes are noted item by item. If there is an order-spanning change (such as change of the customer data), then the change type is taken over into all items if these still do not have their own or a lower change status. The already-locked items will not assume the status "production-relevant." For these items, production-relevant changes remain local. The change status in the items is retained until the changes are acknowledged by production (`kauf.uebertragen = 1`).

The evaluation of the changes in the process takes place with each correction. As long as the order was not forwarded to production and was not reported "processed" by production, the change status on all items remains "production-relevant."

Depending on the type of change, items can have different status and change flags in the order.

### Restrictions

The transfer of order changes to production depends on other system settings such as "Lock logic by item" and permissible status update with existing purchase orders or receipt of goods.

### Notes

This functionality is a Value+ function.

## Contact Address

**A+W Software GmbH**  
Siemensstraße 3  
35463 Fernwald  
Germany

**Tel.** +49 641 96620-0  
**E-mail:** [info@a-w.com](mailto:info@a-w.com)  
**Internet:** [http://www.a-w.com/](http://www.a-w.com/)
