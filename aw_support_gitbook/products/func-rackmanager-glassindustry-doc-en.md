---
title: "EN-FUNC-AW_Rack_Manager"
source: "EN-FUNC-AW_Rack_Manager.pdf"
tags: ["A+W", "Rack Manager", "Software", "Glass Industry", "Logistics", "ERP", "Functional Description"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A functional description of the A+W Rack Manager software module. This document outlines the module's purpose, which is to manage transport racks for glass products, including tracking their location, status, and involving customers in the booking and return process. It covers key features, system requirements, and integration possibilities."
long_description: "This document provides a detailed functional description for the A+W Rack Manager software, a module designed to integrate with A+W Business, A+W Business Pro, and A+W Enterprise systems. The A+W Rack Manager is a tool for managing the logistics of transport racks used in the glass industry. It enables glass processors and their customers to track the movement and status of racks from the producer to the customer, building sites, and back. The system allows for manual or automated (via barcode scanning) registration of racks, linking them to shipping addresses, order data, and rack load. A key feature is the ability for customers to use an internet portal to report the unloading of racks and release them for collection, streamlining the return process. The document details the system's master data management (owners, customers, racks, workflow), movement data tracking, and evaluation capabilities (history, current data, statistics). It also lists technical requirements, functional limitations (e.g., invoicing is handled by a separate commercial system), and contact information for A+W Software GmbH."
---

# A+W Functional Description
# A+W Rack Manager

**A+W - Software for Glass**

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
        1.  Master data
        2.  Movement data
        3.  Evaluations
    5.  Limitations
    6.  Notes
4.  **Contact Address**

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and is subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation might also be registered trademarks or other property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2019, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation must be copied, completely or in part, saved, or transferred only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance Description

### 3.1. Data

| **Product** | **A+W Business / A+W Business Pro / A+W Enterprise** |
| :--- | :--- |
| **Module number** | 210006 / 230006 / 200006 |
| **Module** | A+W Rack Manager |
| **Brief description** | The module manages transport racks and makes it possible to involve the customer in the booking process. |
| **Available** | In connection with all current versions |

### 3.2. Description

A+W Rack Manager manages transport racks and makes it possible to involve the customer in the booking process. When loading, the racks are registered manually or by scanning their barcode; whereby the system automatically links the shipping address, order data, and rack load. Via Internet, the customer can comfortably report the unloading of the racks and release them for collection.

This program can be used both stand-alone as well as in combination with A+W Enterprise, A+W Business or A+W Business Pro (rack invoicing/order data) and A+W Barcode Manager (rack information from the PDC).

Racks are loaded at the producer's end, to be transported to the customer or a processor. Customers have the racks shipped to building sites while processors will reload the racks, to ship them to their customers, their building sites, or to other processors.

### 3.3. Requirements

*   Windows Server 2016 or higher
*   SQL Server 2014 or higher or Informix IDS 11.5 or higher

### 3.4. List of functions

*   Entry of rack master data
*   Entry and analysis of all rack movements
*   Display of the load of racks to be shipped (with A+W Barcode Manager)
*   Management of own and external racks
*   Input of external racks upon receipt
*   Central system, i. e. within a group (e.g. group of companies), rack information will be managed centrally (only one server, web services)
*   Open booking interface for external programs (web services)
*   Display of rack load, histories and statistics
*   Display of data (rent period, rack, customer) for rack invoicing.
*   Quick access via Internet.

#### 3.4.1. Master data

Master data is described in the A+W Rack that describes the participants in the rack system, their relations, and the owners of the individual racks.

Master data are distinguished by:
*   Owners and owner groups
*   Customers and racks
*   Logins
*   Workflow

**Owners and owner groups**

Every rack has an owner. Owners always belong to an owner group. The simplest case is a group consisting of just one owner.

Within a group, the owners can exchange racks without invoicing. It can be configured how racks are invoiced externally. Within a group, all owners can view all rack movements as long as they have the authorization for this.

Every owner can connect his commercial (order entry) system with the rack system to export invoice data, and to import order data. A combination with the A+W Barcode Manager enables the automatic booking of racks and rack assignments based on the PDC readings.

**Customers and racks**

Insofar as they have a login and password, customers can use the A+W Rack Manager to view the rack load of the racks delivered. A customer can report racks he no longer needs, ready for pick-up.

**Workflow**

In the A+W Rack Manager, you can define a workflow. This way, you can define the statuses a rack can or has to go through and when particular bookings are not permitted.

#### 3.4.2. Movement data

Movement data constantly record the whereabouts and status of racks. These bookings can be made manually or automatically, in the background.

Based on the movement booking, the responsibility for a rack is transferred to another owner or customer. This is valid until the next booking is made for the rack. Since all bookings are saved for all racks, the movements of every rack can be traced.

#### 3.4.3. Evaluations

A major feature of the rack system is the analysis of rack information based on these bookings. The available information is split into three groups:

*   **History:** all bookings for a rack in chronological sequence
*   **Current rack data (current booking record):** information about racks that fulfill particular criteria (e.g. postal code, route, owner, etc.) with the current booking record
*   **Statistics:** specific average value across all racks, e.g. rack removal/receipt, average duration of stay at customer's, average maintenance duration, etc.

### 3.5. Limitations

The A+W Rack Manager supplies the data for invoicing. The actual invoicing must be done by means of a local, commercial system.

No coupling with the A+W Logistics Optimizer and the GestellPool Europe is possible.

### 3.6. Notes
(No content provided in this section)

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

**Tel.** +49 641 96620-0
**E-mail:** info@a-w.com
**Internet:** http://www.a-w.com/
