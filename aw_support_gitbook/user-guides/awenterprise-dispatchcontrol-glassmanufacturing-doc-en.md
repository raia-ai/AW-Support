---
title: "EN_AWEnterprise_DispatchControl"
source: "EN_AWEnterprise_DispatchControl.pdf"
tags: ["A+W Enterprise", "Dispatch Control", "Logistics Software", "Glass Manufacturing", "Window Manufacturing", "Order Management", "Shipping", "Route Planning", "Rack Management", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference manual for A+W Enterprise Dispatch Control, a logistics module for managing the dispatch of glass, windows, and doors. It details the features and functions for planning, processing, and tracking delivery orders."
long_description: "This comprehensive software reference manual provides detailed instructions and descriptions for the A+W Enterprise Dispatch Control module. This module serves as the central control center for all logistics and dispatch operations within the A+W Enterprise software suite, specifically tailored for the glass, windows, and doors industries. The manual covers the entire dispatch workflow, starting from initial program functions like searching for orders and market partners, to the detailed management of deliveries. It explains the hierarchical structure of dispatch documents, which are organized into four levels: Delivery Dates, Tours/Routes, Orders, and Items. Users will find in-depth information on navigating the Dispatch Explorer, understanding its tree structure, and interpreting the various data tabs available at each level, including RouteInfo, RackInfo, VehicleInfo, and Optimization tabs. The guide also details numerous functions such as postponing shipments, managing rack allocations, booking goods, handling missing quantities, and printing essential documents like loading lists and delivery notes. The manual is intended for end-users of A+W Enterprise, providing them with the necessary knowledge to efficiently manage dispatch processes, ensure timely deliveries, and maintain accurate records of all shipping activities."
---

# A+W Dispatch Control G

**A+W Enterprise**

*A+W - Software for Glass, Windows and Doors*

---

---
## Introduction

This part of the documentation contains editorial notes.

### Revision Overview

| Section Version/Date | Software version | Description |
| :--- | :--- | :--- |
| 2.00/04-2022 | 6 | Update of software reference. |
| 1.03/01-2017 | 5.2.4 | Product and company names adjusted. |
| 1.02/02-2014 | 5.2.4 | Product names adjusted |
| 1.01/01-2013 | 5.2.4 | Layout adapted to CI 2013 |
| 1.00/11-2012 | 5.2.4 | Original version |

### Editorial

The editorial provides information on the following topics:
- Notes on this Document
- Copyrights
- Trademarks
- Contacts

#### Notes on this Document

This document is intended for end users of A+W Enterprise.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice. The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice.

The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The descriptions in this document are based on the full program level of A+W Enterprise.

The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior approval in writing.

#### Copyrights

©2022, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation.

#### Trademarks

All hardware and software names mentioned in this documentation can also be registered trademarks or other property rights of third parties. Third-party copyrights must therefore be observed.

#### Contacts

**A+W Software GmbH**
Am Pfahlgraben 4-10
35415 Pohlheim
+49 6404 2051-0
+49 6404 2051 877
Zentrale@a-w.com
http://www.a-w.com

---

## Software Reference

### Overview

All Dispatch Control views, dialogs, and functions are accessible via the Logistics module. You can also start the module directly from FixWin. In the default configuration, you start directly with the Dispatch Explorer:
⇨ "Dispatch Explorer" on page G15

With Dispatch Control, you find, plan, process, and send your delivery orders on time. Dispatch Control is the control center for dispatch and provides quick and easy access to all delivery orders. For example, you create a list of all delivery dates for a period or jump directly into the delivery order you're looking for. For the overview of the dispatch documents, each delivery order is divided into the following four levels:

- Delivery dates
- Tours and routes
- Orders
- Items

The first level shows the delivery dates. A delivery date includes the corresponding routes or tours.

The second level shows the routes and tours. A tour includes the corresponding orders and can consist of one or more routes. A tour represents at least one route on a certain delivery date. The route is a defined route to be traveled. Routes can be assigned to certain weekdays or certain times. The tour level offers an overview of existing dispatch documents.

The orders are shown on the third level. An order consists of the appropriate items and shipping address. The order level offers an overview of existing dispatch documents.

Items are shown on the fourth level. An item includes the appropriate units.

Open tours, orders or items are locked for processing by other employees. They are then only opened with read rights.

### Start functions

A+W Enterprise offers various functions for searching for delivery dates and orders.

The following information is available on this subject:
⇨ "Program start" on page G11
⇨ "Find Order" on page G13
⇨ "Find Market Partner" on page G14

#### Program start
*Logistics > Dispatch Control*

**Fig. G 1: Search Mode**
