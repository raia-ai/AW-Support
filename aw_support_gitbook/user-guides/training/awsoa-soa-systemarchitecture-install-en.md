---
title: "A+W AWSOA Dependencies (as of 03/2022)"
category: "training"
product: "AWSOA"
doc_type: "Unknown"
language: "EN"
tags: ["AWSOA", "Soa", "SystemArchitecture", "Install"]
version: "1.0"
last_updated: "2025-12-10"
description: "title: "A+W AWSOA Dependencies" source: "EN-INST-AW_SOA_Dependencies.pdf" tags: ["A+W", "AWSOA", "Software Dependencies", "SOA", "System Architecture", "Database Schema", "Technical Documentation", "Glass Industry Software"] version: "1.0" last_updated: "2025-10-03" short_description: "Technical document detailing the module dependencies, service descriptions, and database table access for the A+W AWSOA software suite as of March 2022. It covers various domains including Infrastructure, CIM, Pla"
source_file: "AWSOA-Soa-SystemArchitecture-Install-EN.md"
---


title: "A+W AWSOA Dependencies"
source: "EN-INST-AW_SOA_Dependencies.pdf"
tags: ["A+W", "AWSOA", "Software Dependencies", "SOA", "System Architecture", "Database Schema", "Technical Documentation", "Glass Industry Software"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Technical document detailing the module dependencies, service descriptions, and database table access for the A+W AWSOA software suite as of March 2022. It covers various domains including Infrastructure, CIM, Planning, and Commercial."
long_description: "This document provides a comprehensive overview of the A+W Service-Oriented Architecture (AWSOA) dependencies, effective as of March 2022. It is intended for system administrators, developers, and technical consultants involved in the setup, configuration, and maintenance of A+W software solutions for the glass industry. The document begins by outlining the dependencies between various software modules, specifying which services are required for each component to function correctly. It then provides short descriptions for each service, categorized by domain (e.g., Infrastructure, CAD, CIM, Commercial, Planning). A significant portion of the document is dedicated to detailing the database access layer, listing the specific database tables accessed by each SOA service. This provides crucial information for database administration and troubleshooting. Finally, a high-level domain overview is presented, illustrating the logical grouping of services into domains like Infrastructure, Corporate, Commercial, and Planning. This helps in understanding the overall system architecture and the relationships between different functional areas."
---

# A+W AWSOA Dependencies (as of 03/2022)

**A+W - Software for Glass**

## 1. Content
1.  Content
2.  Module Dependencies
3.  Services Short Description
4.  Access to databases and tables
    4.1. Infrastructure
    4.2. Facility
    4.3. CAD
    4.4. CIM
    4.5. Commercial
    4.6. Corporate
    4.7. Planning
    4.8. Web
5.  Domain Overview
6.  Contact Address

## 2. Module Dependencies

| Modules | Required AWSOA Setup Dependencies |
| :--- | :--- |
| **All AWSOA Services** | Infrastructure Middleware<br>Infrastructure Service Locator (Highlander!) |
| **Infrastructure.Web** | Infrastructure Collector Service<br>Infrastructure Services<br>Infrastructure Reporting Service (only needed for AWB CR) |
| **CIM.Web (Barcoding CE Scanner + SmartTerminal)** | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service |
| **Corporate.Web (A+W Dashboard)** | Infrastructure Services + Web<br>Corporate Dashboard Service<br>CIM Barcoding Service<br>Planning Job Service<br>Planning DataProvider Service |
| **Planning.Web (CapaView + Stock/MRPS)** | Infrastructure Services + Web<br>Planning DataProvider Service<br>Planning Job Service<br>Planning Stock Service |
| **AWB/AWE - iQuote (Web.Web)** | Infrastructure Services + Web<br>Infrastructure Reporting Service (AWB)<br>Web Configurator Service<br>Commercial Document Service<br>Commercial Converter Service (AWE)<br>CAD Geometry Service<br>AWB/AWE |
| **Cantor - iQuote (Web.Web)** | Infrastructure Services + Web<br>Web Configurator Service<br>Commercial Document Service (Cantor)<br>Commercial TransactionData Service (Cantor)<br>Commercial MasterData Service (Cantor)<br>Cantor |
| **AWB/AWE/Cantor – Route optimization (OTR)** | Infrastructure Services + Web<br>Commercial Logistic Service<br>Commercial Logistic Backend Service (AWE/Cantor)<br>OTR |
| **AWB - Delivery Date Check** | Infrastructure Services + Web<br>Planning Import Service |
| **AWB - File-less transfer to production** | Infrastructure Services + Web<br>Exchange Service |
| **AWB - Automatic process execution (Ex-AIS)** | Infrastructure Services + Web |
| **AWB - Crystal Report Print** | Infrastructure Services + Web<br>Infrastructure Reporting Service |
| **AWP Production Terminal PPSWebService** | Infrastructure Services + Web |
| **RTO with A+W Residual Stock Manager** | Infrastructure Services + Web<br>Planning Stock Service |
| **CX SmartCompanion (Production Module)** | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>AWP Booking Service<br>Facility Rack (only needed for AW RackManager Connection) |
| **CX SmartCompanion - Cantor (Production Module)** | Infrastructure Services + Web<br>Cantor CIM Barcoding Service<br>Cantor CIM SmartCompanion Service |
| **CX SmartCompanion (Stock Module)** | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>Commercial Purchase Service (AWE – Linux)<br>Commercial Stock Service (AWE – Linux)<br>AWP Booking Service |
| **CX SmartCompanion - Cantor (Stock Module)** | Infrastructure Services + Web<br>Cantor Commercial Purchase Service<br>Cantor Commercial Stock Service |
| **CX Dispatch** | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>Commercial Dispatch Service (AWE – Linux) |
| **CX iShape** | Infrastructure Services + Web<br>CAD Digitizing Service<br>SN |
| **RTO + CX PatternViewer** | Infrastructure Services + Web<br>Planning Optimization Service<br>CIM Barcoding Service (reference mark/stamps/logo)<br>CAD Sheets Service (reference mark/stamps/logo) |
| **CX SmartFactory** | Infrastructure Services + Web<br>CIM Barcoding Service<br>CIM MAPS Service<br>Planning BOM Service<br>Planning Data Provider Service<br>Planning Detailed Service<br>Planning Job Service<br>Planning Optimization Service<br>Planning Stock Service<br>Planning Web<br>AWP Booking Service<br>AWP AlcimServer |
| **Future** | |
| **CX Sales** | Infrastructure Services + Web<br>Commercial Sales Service (AWE – Linux) |
| **CX IoT** | Infrastructure Services + Web<br>CIM QualityTracking Service<br>CIM Barcoding Service<br>Corporate Gateway Service<br>Planning Job Service<br>AWP Booking Service<br>Commercial Purchase Service (AWE – Linux) |

## 3. Services Short Description

### Infrastructure
- **BasicData** (Clients/Sites, User Assignments & Languages)
- **Configuration** (Switches)
- **Database** (Database Update)
- **License** (License, License Usage Register/View – Production Terminal/PPSWebService, Licensing for SmartCompanion)
- **Protocol + Collector** (Protocol Viewer + Alert Email messaging)
- **Reporting** (AWB - Crystal Report Printing)
- **Workflow** (Workflow Management)

### Facility
- **Rack** (AW RackManager Connection for SmartCompanion)

### CAD
- **Bar** (Bar/Muntin management)
- **Digitizing** (Picture processing for iShape)
- **Geometry** (Shapes and processing pictures for iQuote)
- **Sheets** (Referencemark for PV/DXF Import functionality for SN)

### CIM
- **Barcoding** (Dashboard Data & Wi-Fi Barcoding Scanner/Smart Terminal & SmartCompanion & MQTT API)
- **Furnace** (SmartFactory furnace control)
- **Sorter** (SmartFactory sorter control)
- **MAPS** (SmartFactory/Multi-stage Automatic Production System)
- **Quality Tracking** (Production batch tracking/tracing)
- **MachineryAutomation** (Control/Communication to cutting area machines – Hainan only)

### Corporate
- **Dashboard** (Dashboard)
- **Gateway** (IoT Platform/Connection to Actiware)
- **KPI** (Dashboard connection to Cantor – deprecated)

### Commercial
- **Converter** (AWEnterprise FIX connection, AWDesign + SN pictures for iQuote (AWE))
- **DataProvider** (ClarityExperience Dispatch + Sales UI)
- **Dispatch** (ClarityExperience Dispatch UI)
- **Document** (Connection of ERP Solution for iQuote AWB/AWE/Cantor)
- **Exchange** (Automatic process execution (Ex-AIS), Communication with SGG-WebService)
- **Logistic** (OTR)
- **LogisticBackend** (OTR connection to Cantor or AWE)
- **MasterData** (Master data exchange with Cantor)
- **Purchase** (SmartCompanion Stock + IoT Platform)
- **Sales** (ClarityExperience Sales UI)
- **Stock** (SmartCompanion Stock)
- **TransactionData** (Order data exchange with Cantor)

### Planning
- **BOM** (Bill of Material, SmartFactory)
- **DataProvider** (Legacy database table reading support & Dashboard Data)
- **Detailed** (Detailed Scheduling via QuickOrga – SmartFactory, OXXO)
- **Import** (AWB Delivery DateCheck & File-less transfer to production)
- **Job** (CapaView & Rough Scheduling & Barcoding & Dashboard Data & SmartCompanion & SmartFactory)
- **Optimization** (Optimization for RTO with PatternViewer, Furnace Opti SmartFactory)
- **Stock** (Stock management/Sorter management SmartFactory /RTO with RPMS)
- **Automation** (Workflow controlled Rough-, Detailed-Scheduling and DynOpt Import – OXXO only)

### Web
- **Configurator** (iQuote)

## 4. Access to databases and tables

### 4.1. Infrastructure

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **BasicData** | AWSOA | Core_Clients<br>Core_ClientAssignments<br>Core_Languages |
| **Config** | AWSOA | Core_ConfigDynamicComponents<br>Core_ConfigSysSwitches<br>Core_ConfigUserSwitches<br>Core_CustomTexts |
| **Database** | AWSOA | Core_DBProtocols<br>Core_DBUpdates<br>Core_DBVersions |
| **License** | AWSOA | Core_Lic2DeviceAssignments<br>Core_Lic2ForeignAssignments<br>Core_LicDeviceAssignments<br>Core_LicenseConnections<br>Core_LicenseInfoes<br>Core_LicenseParallelUsages<br>Core_LicenseTotalUsages<br>Core_LicenseUsages<br>Core_LicForeignAssignments |
| **Reporting** | AWSOA | Core_ReportFields<br>Core_ReportGroups<br>Core_Reports<br>Core_ReportTableFields<br>Core_ReportTables |
| **Workflow** | AWSOA | Core_WFActivities<br>Core_WFActivityArchives<br>Core_WFActivityAssignments |

### 4.2. Facility

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Rack** | RackManager | RAOwner<br>RAOwnerGroup<br>RARack<br>RARackType |

### 4.3. CAD

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Digitizing** | AWSOA | CAD_DigiShapeContainers<br>CAD_DigiShapeInfoes |
| **Sheets** | AWSOA | CAD_Sheets_AttrParameters<br>CAD_Sheets_BlockAttr<br>CAD_Sheets_Blocks<br>CAD_Sheets_CADModels<br>CAD_Sheets_Entities<br>CAD_Sheets_Inserts<br>CAD_Sheets_Layers<br>CAD_Sheets_Paths |

### 4.4. CIM

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Barcoding** | AWProduction | AWBar_Bearbeit<br>AWBar_Booking<br>AWBar_Bruch<br>AWBar_Charge<br>AWBar_Gateway_Data<br>AWBar_Gateway_Machine_Data<br>AWBar_Gestelle<br>AWBar_GestDaten<br>AWBar_Historie<br>AWBar_Person<br>AWBar_Stellen<br>AWBar_StellenTyp<br>AWBar_Teile<br>AWBar_Zustand<br>AWBar_ZustandTyp<br>BDEStat_ES |
| **Furnace** | AWSOA | Parameter<br>Furnace_FurnaceBeds<br>Furnace_FurnaceSheets |
| **MAPS** | AWProduction | Maps_Agents<br>Maps_Brokers<br>Maps_ClientConfigurations<br>Maps_GlassInstances<br>Maps_Hops<br>Maps_Locations<br>Maps_LocationGroups<br>Maps_Optimizations<br>Maps_Queries<br>Maps_ReservationTicketGroupEntries<br>Maps_Sorters<br>Maps_Tickets<br>Maps_TicketGroups<br>Maps_TicketGroupEntries |
| **QualityTracking** | AWSOA | Quality_TrackingData |

### 4.5. Commercial

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Logistic** | AWSOA | Comm_Breakages<br>Comm_Containers<br>Comm_Destinations<br>Comm_Documents<br>Comm_ItemContainers<br>Comm_Items<br>Comm_Routes |

### 4.6. Corporate

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Dashboard** | AWSOA | Dashboard_ClientViews<br>Dashboard_Containers<br>Dashboard_Controls<br>Dashboard_Pages<br>Dashboard_Panes<br>Dashboard_PaneControls<br>Dashboard_Views<br>Dashboard_ViewPages |

### 4.7. Planning

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Automation** | AWSOA | Planning_JobRelease |
| **BOM** | AWProduction | ArtikelStamm<br>AWBar_Bearbeit<br>AWBar_InitData<br>BearbeitStamm<br>Bearb_Typ<br>Cap_Kosten<br>MZO_RealMaschine<br>MZO_Route_Map<br>Maps_Processings<br>Modellstamm_Faktor<br>Modellstamm_Description<br>Pool_Auftrag<br>Pool_Bearbeit<br>Pool_Modell<br>Pool_Pos<br>Pool_Selektion<br>Pool_Teile<br>XOpt_Art<br>Zuschlag<br>Zuschlag_Artikel<br>Zuschlag_Masch<br>Zuschlag_Bearbeit |
| **DataProvider** | AWProduction | Parameter<br>CutGo_Cluster<br>CutGo_Cluster_Unit<br>Pool_GlasArt<br>XOpt_Art<br>XOpt_Jumbo<br>XOpt_Optimierung |
| **Detailed** | AWProduction | Parameter<br>Detail_CuttingResults<br>Detail_Jobs<br>Detail_Lots<br>Detail_LotItems<br>Detail_PlannedRacks<br>Detail_PlannedRackItems<br>Detail_WorkSteps<br>Fein_Teile<br>Fein_Unit |
| **Job** | AWProduction | Pool_Auftrag<br>Pool_Bearbeit<br>Pool_Bestellteile<br>Pool_Lauf<br>Pool_Pos<br>Pool_Teile<br>Prozesse |
| **Optimization** | AWSOA | Parameter<br>Opti_Defects<br>Opti_OptimizationResults<br>Opti_Patterns<br>Opti_Rectangles<br>Opti_Shapes<br>Opti_Sheets |
| **Stock** | AWSOA | Stock_ArticleNumberMappings<br>Stock_GlassItems<br>Stock_GlassRequests<br>Stock_IORequests<br>Stock_Items<br>Stock_Residuals<br>Stock_ResidualRequests<br>Stock_SegmentRequests<br>Stock_StockPlates<br>Stock_StockPlateReservations<br>Stock_StockSheets<br>Stock_StockSheetRequests<br>Stock_Storages<br>Stock_StorageLocations<br>Stock_StorageSegments<br>Stock_StorageSegmentProperties |

### 4.8. Web

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Configurator** | AWSOA | Web_Carts<br>Web_CartItems<br>Web_CartItemActions |

## 5. Domain Overview

### Infrastructure Domain
- BasicData Service
- Database Service
- Configuration Service
- Protocolling Service
- Collector Service
- License Service
- Workflow Service
- Reporting Service
- Infrastructure Web
- Ice Grid / Ice Strom

### Corporate Domain
- Dashboard Service
- Gateway Service
- KPI Service
- Corporate Web (Dashboard)

### CAD Domain
- Bar Service
- Digitizing Service
- Dxf Service
- Geometry Service

### Facility Domain
- Rack Service

### Web Domain
- Configurator Service
- Web Web (iQuote)

### Commercial Domain
- Converter Service
- DataProvider Service
- Dispatch Service
- Document Service
- Exchange Service
- Logistic Service
- LogisticBackend Service
- (CA) Masterdata Service
- Purchase Service
- Sales Service
- Stock Service
- (CA) TransactionData Service

### Planning Domain
- BOM Service
- DataProvider Service
- Detailed Service
- Import Service
- Job Service
- Optimization Service
- Stock Service
- Automation Service
- Planning Web (CapaView + Stock)

### CIM Domain
- Barcoding Service
- Furnace Service
- MAPS Service
- QualityTracking Service
- Machinery Automation Service
- CIM Web (Barcoding + SmartTerminal)

