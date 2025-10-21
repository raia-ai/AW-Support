---
title: "EN-INST-AW_Smart_Factory"
source: "EN-INST-AW_Smart_Factory.pdf"
tags: ["A+W Clarity", "Smart Factory", "Automated Production", "Installation Instructions", "Software", "Glass Manufacturing", "MAPS", "HEGLA Sortjet", "Furnace Control"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides detailed installation and configuration instructions for the A+W Clarity Smart Factory, a multi-step automated production system for the glass and windows industry. It covers system requirements, database setup, master data configuration, and integration of various components like the HEGLA Sortjet, North-Glass furnace, and shopfloor clients."
long_description: "This is a comprehensive technical manual detailing the setup process for the A+W Clarity Smart Factory - Multistep Automated Production system (MAPS). It is intended for planners and service technicians responsible for installing and configuring the software environment. The document begins with a detailed change history, tracking versions from 1.0 to 2.57. It then outlines the prerequisites, including A+W Production SingleSite environment, specific AWSOA services, and database configurations for Informix. The core of the manual is the 'Installation' section, which guides the user through database schema creation, master data population, and the setup of key services like the MAPS Service, Furnace Service, and Sorter Service. It provides in-depth configuration details for various shopfloor clients, such as the Dynopt Filler Client for optimization, the HEGLA Sortjet Client for sorting, and the North-Glass furnace client. The manual explains the intricacies of the ticket and lite status system within the Smart Factory, the structure of the production timeline, and how to handle events like breaks and remakes. It also covers the user interface, including call and supply dialogs, and the connection to the A+W Production PDC for booking and status updates. The document is rich with technical details, including SQL scripts, XML configuration examples, and screenshots of administrative interfaces."
---

# Software for Glass and Windows
## Installation Instructions
### Beta - A+W Clarity Smart Factory - Multistep Automated Production

### Change history:

| Date | Author | Comments | Version |
| :--- | :--- | :--- | :--- |
| 2019-03-21 | DLA | Document created | 1.0 |
| 2021-01-18 | ΜΜΕ | "SwapFour" as new method for buffer slot assignment | 2.30 |
| 2021-01-21 | DLA | Time horizon | 2.31 |
| 2021-02-09 | MISC | New sort mode for sorter | 2.32 |
| 2021-02-19 | MPH | Supply Dialog BSG In | 2.33 |
| 2021-04-07 | DLA | Validation Status | 2.34 |
| 2021-04-09 | DLA | Clarity Suite | 2.35 |
| 2021-05-06 | MPH | Call dialogs | 2.36 |
| 2021-05-18 | DLA | BDE goes SMF | 2.37 |
| 2021-07-07 | DLA | Assembling units | 2.38 |
| 2022-02-17 | MISC | New CIM.Furnace Service | 2.39 |
| 2022-02-21 | MISC | Help tools | 2.40 |
| 2022-03-08 | MISC | RollerWaveDirection in Furnace Service | 2.41 |
| 2023-01-16 | MISC | Pattern viewer in the sorter client | 2.42 |
| 2023-02-28 | MISC | Several outputs with the same LocationID on a Sortjet | 2.43 |
| 2023-07-28 | MPH | Update status indicator call/supply dialogs | 2.44 |
| 2023-10-12 | MISC | Turning of lites at a turning station in front of an IG line | 2.55 |
| 2023-11-23 | LUSC | Multiple assignment for individual lites and HandleOpenReservationOnRequest added | 2.57 |
| 2024-01-16 | Shahan | Replaced Furnace client with Furnace Service | 2.44 |
| 2024-03-11 | Shahan | Sorter Service | 2.45 |

The installation instructions will assist the planner with the installation and configuration of the software named.

---

## 1 Requirements
A+W Smart Factory is a multi-level automated production system (MAPS). It requires a run-capable A+W Production SingleSite environment.
The associated infrastructure domain has to be configured, the default client is used.
MAPS requires the following services from the AWSOA:
- Planning.Job
- Planning.BOM
- Planning.Detailed
- Planning StockService
- Planning.OptimizationService
- CIM.Maps
- CIM.BarcodeReading

### 1.1 Informix
If A+W Production is running under INFORMIX, there can be problems with the "InsertCursor". Here, it is recommended that you switch off the "InsertCursor" in the infrastructure in the configuration of the A+W production (EnableInsertCursors=0). For the AWSOA database under Informix, this can also be made in the ODBC settings.

