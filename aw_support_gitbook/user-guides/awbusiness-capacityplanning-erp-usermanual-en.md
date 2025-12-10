---
title: "A+W Business Pro Capacity Planning - Tutorial and Reference"
source: "EN-UM-AWBusiness_30.pdf"
tags: ["A+W Business Pro", "Capacity Planning", "ERP", "Production Scheduling", "Machine Selection", "Master Data", "Manufacturing Software", "Tutorial", "Software Reference"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive tutorial and software reference for the A+W Business Pro Capacity Planning module. It covers automatic scheduling, machine selection, master data allocation, production cost calculation, and using the control station to monitor and manage production."
long_description: "This document serves as a detailed guide for the A+W Business Pro Capacity Planning module, a software solution for managing manufacturing processes, particularly in the glass, windows, and doors industry. The content is split into a tutorial section and a software reference section, providing both practical, example-driven instructions and detailed descriptions of all features and dialogs. Key topics include Automatic Scheduling, where the system selects the optimal machine based on priority, capacity, and technical restrictions. It details how to configure machine priorities, work types, and restrictions, including special technical restrictions for quantities and other parameters. The manual also covers machine selection for alternative work types and the use of locks to prevent certain operations or machine usage based on product type, customer, or process sequence. A significant portion is dedicated to the allocation of master data, explaining how to define production sequences by linking work types to product types, product classes, and individual products. The guide then moves into the core of Capacity Planning, explaining date calculation (backward/forward scheduling), handling capacity problems through item splitting, and managing production times. The Production section details how to monitor status through reports, registration points, and completion notifications, including handling breakages and remaining quantities. Finally, it covers Production Costs, explaining how time and machine costs are calculated and analyzed through cost centers, and the use of the Control Station, a central hub for viewing machine utilization, rescheduling orders, and managing the entire production plan."
---

# Tutorial

---
## Automatic Scheduling

For automatic scheduling, the machines allocated to the corresponding work type will be selected. Several machines can be allocated to a work type, e.g. several drills to work type Drilling. The combination of work type and machine results in the time required (reserved capacity) and the costs. The automatic selection of the drilling machine is - among other things- based on the free capacities, technical restrictions, and costs.

The selection of a machine can therefore be controlled using the following settings:
*   Priority of the machine (9 to -2)
*   Work type
*   Locking of the machine, e.g. for particular product types
*   Restrictions that refer to the requirements from the order position, e.g. the dimensions, quantity.

In the following two figures, you can see how these settings work together. Priorities and restrictions are then described in detail in separate units.

