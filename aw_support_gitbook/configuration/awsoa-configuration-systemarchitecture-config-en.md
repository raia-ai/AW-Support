---
title: "EN-CONFIG-AW_SOA_Dependencies"
source: "EN-CONFIG_AW_SOA_Dependencies.pdf"
tags: ["A+W", "AWSOA", "Software Dependencies", "Configuration", "System Architecture", "SOA", "Glass Industry", "Module Dependencies", "Database Schema", "Service-Oriented Architecture"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a technical overview of the A+W Service-Oriented Architecture (AWSOA) as of March 2025. It details the dependencies between different software modules, offers short descriptions of various services, maps services to their corresponding database tables, and provides a high-level domain overview of the system architecture. It is intended for system administrators and developers working with the A+W software suite for the glass industry."
long_description: "This technical configuration document, \"AWSOA Dependencies (as of 03/2025),\" serves as a comprehensive guide to the A+W Service-Oriented Architecture. It is designed for technical personnel, including system architects, administrators, and developers, who are responsible for installing, configuring, and maintaining the A+W software ecosystem. The document is structured into several key sections. It begins by outlining the \"Module Dependencies,\" specifying which core AWSOA services are required for various A+W application modules like CIM.Web, Corporate.Web, iQuote, and the CX suite to function correctly. The \"Services Short Description\" section provides a functional summary of services across different categories such as Infrastructure, Facility, CAD, CIM, Commercial, and Planning. A significant portion of the document is dedicated to \"Access to databases and tables,\" which meticulously maps each SOA service to the specific databases (e.g., AWSOA, AWProduction, AlcimDB) and tables it interacts with, offering crucial insights for database administration and troubleshooting. Finally, the \"Domain Overview\" section presents a high-level architectural view, grouping services into logical domains like Infrastructure, Corporate, Commercial, Planning, and CIM, illustrating the overall structure of the software."
---

# A+W Configuration: AWSOA Dependencies (as of 03/2025)

---
## 1. Content

1.  **Content**
2.  **Module Dependencies**
3.  **Services Short Description**
4.  **Access to databases and tables**
    4.1. Infrastructure
    4.2. Facility
    4.3. CAD
    4.4. CIM
    4.5. Commercial
    4.6. Corporate
    4.7. Planning
    4.8. Web
5.  **Domain Overview**

## 2. Module Dependencies

| Modules | Required AWSOA Setup Dependencies |
| :--- | :--- |
| **All AWSOA Services** | Infrastructure Middleware<br>Infrastructure Service Locator (Highlander!) |
| **Infrastructure.Web** | Infrastructure Collector Service<br>Infrastructure Services<br>Infrastructure Reporting Service (only needed for AWB CR) |
| **CIM.Web (Barcoding CE Scanner + SmartTerminal)** | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services |
| **Corporate.Web (A+W Dashboard)** | Infrastructure Services + Web<br>Corporate Dashboard Service<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services<br>Planning DataProvider Service |
| **Planning.Web (CapaView + Stock/MRPS)** | Infrastructure Services + Web<br>Planning Data Provider Service<br>Planning Job Service<br>optional: Cad Services<br>Planning Stock Service |
| **AWB/AWE - iQuote (Web.Web)** | Infrastructure Services + Web<br>Infrastructure Reporting Service (AWB)<br>Web Configurator Service<br>Commercial Document Service<br>Commercial Converter Service (AWE)<br>CAD Geometry Service<br>AWB/AWE |
| **Cantor - iQuote (Web.Web)** | Infrastructure Services + Web<br>Web Configurator Service<br>Commercial Document Service (Cantor)<br>Commercial TransactionData Service (Cantor)<br>Commercial MasterData Service (Cantor)<br>Cantor |
| **AWB/AWE/Cantor – Route optimization (OTR)** | Infrastructure Services + Web<br>Commercial Logistic Service<br>Commercial Logistic Backend Service (AWE/Cantor)<br>OTR |
| **AWB - Delivery Date Check** | Infrastructure Services + Web |
| **AWB - File-less transfer to production** | Planning Import Service |
| **AWB - Automatic process execution (Ex-AIS)** | Infrastructure Services + Web<br>Exchange Service |
| **AWB - Crystal Report Print** | Infrastructure Services + Web<br>Infrastructure Reporting Service |
| **AWP Production Terminal PPSWebService** | Infrastructure Services + Web |
| **RTO with A+W Residual Stock Manager** | Infrastructure Services + Web<br>Planning Stock Service |

**CX Modules**

| Modules | Required AWSOA Setup Dependencies |
| :--- | :--- |
| **CX SmartCompanion (Production Module)** | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services<br>AWP Booking Service<br>Facility Rack (only needed for AW RackManager Connection) |
| **CX SmartCompanion - Cantor (Production Module)** | Infrastructure Services + Web<br>Cantor CIM Barcoding Service<br>Cantor CIM SmartCompanion Service |
| **CX SmartCompanion (Stock Module)** | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services<br>Commercial Purchase Service (AWE – Linux)<br>Commercial Stock Service (AWE – Linux)<br>AWP Booking Service |
| **CX SmartCompanion - Cantor (Stock Module)** | Infrastructure Services + Web<br>Cantor Commercial Purchase Service<br>Cantor Commercial Stock Service |
| **CX Dispatch** | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services<br>Commercial Dispatch Service (AWE – Linux) |
| **CX iShape** | Infrastructure Services + Web<br>CAD Digitizing Service<br>SN |
| **RTO + CX PatternViewer** | Infrastructure Services + Web<br>Planning Optimization Service<br>CIM Barcoding Service (reference mark/stamps/logo)<br>CAD Sheets Service (reference mark/stamps/logo) |
| **CX SmartFactory** | Infrastructure Services + Web<br>CIM Barcoding Service<br>CIM Maps Service<br>CIM Flow Service<br>CIM Furnace Service<br>CIM Sorter Service<br>Facility Layout Service<br>Facility FactoryState Service<br>Planning BOM Service<br>Planning DataProvider Service<br>Planning Detailed Service<br>Planning Job Service<br>Planning Stock Service<br>Cad Services<br>Planning Optimization Service<br>Planning Stock Service<br>Planning.Web<br>AWP Booking Service<br>AWP AlcimServer<br>Upcoming Dependency: CX NextGenDynOpt |

**Future Modules**

| Modules | Required AWSOA Setup Dependencies |
| :--- | :--- |
| **CX Sales** | Infrastructure Services + Web<br>Commercial Sales Service (AWE – Linux) |
| **CX IoT** | Infrastructure Services + Web<br>CIM Quality Tracking Service<br>CIM Barcoding Service<br>Corporate Gateway Service<br>Planning Job Service<br>optional: Cad Services<br>AWP Booking Service<br>Commercial Purchase Service (AWE – Linux) |
| **CX NextGenDynOpt** | Infrastructure Services + Web<br>Facility Services<br>Facility FactoryState Services<br>Facility Layout Services<br>CIM Flow Service<br>CIM Cutting Service |

## 3. Services Short Description

*   **Infrastructure**
    *   **BasicData** (Clients/Sites, User Assignments & Languages)
    *   **Configuration** (Switches)
    *   **Database** (Database Update)
    *   **License** (License, License Usage Register/View – Production Terminal/PPSWebService, Licensing for SmartCompanion)
    *   **Protocol + Collector** (Protocol Viewer + Alert Email messaging)
    *   **Reporting** (AWB - Crystal Report Printing)
    *   **Workflow** (Workflow Management)
*   **Facility**
    *   **Layout** (NextGenDynOpt and A+W SmartFactory for providing machinery/shopfloor layouts and machinery "localization” mappings)
    *   **Rack** (AW RackManager Connection for SmartCompanion)
    *   **FactoryState** (Gets machinery state and sets machinery states)
*   **CAD**
    *   **Bar** (Bar/Muntin management)
    *   **Digitizing** (Picture processing for iShape)
    *   **Geometry** (Shapes and processing pictures for iQuote)
    *   **Sheets** (Referencemark for PV/DXF Import functionality for SN)
*   **CIM**
    *   **Barcoding** (Dashboard Data & Wi-Fi Barcoding Scanner/Smart Terminal & SmartCompanion & MQTT API)
    *   **Flow** (SmartFactory flow control for providing overall sheet prioritization)
    *   **Furnace** (SmartFactory furnace control)
    *   **MachineryAutomation** (Control/Communication to cutting area machines – Hainan only)
    *   **Maps** (SmartFactory/Multi-stage Automatic Production System)
    *   **Quality Tracking** (Production batch tracking/tracing)
    *   **Sorter** (SmartFactory sorter control)
    *   **Cutting** (NGD Cutting control)
    *   **Driver** (NGD driver control for cutting tables)
*   **Corporate**
    *   **Dashboard** (Dashboard)
    *   **Gateway** (IoT Platform/Connection to Actiware)
    *   **KPI** (Dashboard connection to Cantor - deprecated)
*   **Commercial**
    *   **Converter** (AWEnterprise FIX connection, AWDesign + SN pictures for iQuote (AWE))
    *   **DataProvider** (ClarityExperience Dispatch + Sales UI)
    *   **Dispatch** (ClarityExperience Disptach UI)
    *   **Document** (Connection of ERP Solution for iQuote AWB/AWE/Cantor)
    *   **Exchange** (Automatic process execution (Ex-AIS), Communication with SGG-WebService)
    *   **Logistic** (OTR)
    *   **LogisticBackend** (OTR connection to Cantor or AWE)
    *   **MasterData** (Master data exchange with Cantor)
    *   **Purchase** (SmartCompanion Stock + IoT Platform)
    *   **Sales** (ClarityExperience Sales UI)
    *   **Stock** (SmartCompanion Stock)
    *   **TransactionData** (Order data exchange with Cantor)
*   **Planning**
    *   **BOM** (Bill of Material, SmartFactory)
    *   **DataProvider** (Legacy database table reading support & Dashboard Data)
    *   **Detailed** (Detailed Scheduling via QuickOrga - SmartFactory, OXXO)
    *   **Import** (AWB Delivery DateCheck & File-less transfer to production)
    *   **Job** (CapaView & Rough Scheduling & Barcoding & Dashboard Data & SmartCompanion & SmartFactory)
    *   **Optimization** (Optimization for RTO with PatternViewer, Furnace Opti SmartFactory)
    *   **Stock** (Stock management/Sorter management SmartFactory /RTO with RPMS)
    *   **Automation** (Workflow controlled Rough-, Detailed-Scheduling and DynOpt Import – OXXO only)
*   **Web**
    *   **Configurator** (iQuote)

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
| **Layout** | AWSOA | Layout_ProcessingTypeMappings<br>Layout_RecipeMappings<br>Layout_Hops<br>Layout_Locations<br>Layout_Machines<br>Layout_Processings<br>Layout_ProductionAreas<br>Layout_ShopfloorConnectors |
| **Rack** | RackManager | RAOwner<br>RAOwnerGroup<br>RARack<br>RARackType |
| **FactoryState** | AlcimDB | AWBar_Teile<br>AWBar_Zustand<br>AWBar_ZustandTyp<br>BDEStat_ES |

### 4.3. CAD

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Digitizing** | AWSOA | CAD_DigiShapeContainers<br>CAD_DigiShapeInfoes |
| **Sheets** | AWSOA | CAD_Sheets_AttrParameters<br>CAD_Sheets_BlockAttr<br>CAD_Sheets_Blocks<br>CAD_Sheets_CADModels<br>CAD_Sheets_Entities<br>CAD_Sheets_Inserts<br>CAD_Sheets_Layers<br>CAD_Sheets_Paths |

### 4.4. CIM

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Barcoding** | AWProduction | AWBar_Bearbeit<br>AWBar_Booking<br>AWBar_Bruch<br>AWBar_Charge<br>AWBar_Gateway_Data<br>AWBar_Gateway_Machine_Data<br>AWBar_Gestelle<br>AWBar_GestDaten<br>AWBar_Historie<br>AWBar_Person<br>AWBar_Stellen<br>AWBar_StellenTyp<br>AWBar_Teile<br>AWBar_Zustand<br>AWBar_ZustandTyp<br>BDEStat_ES |
| **Flow** | AWSOA | Parameter<br>Flow_PrioritizationCriterias<br>Flow_OutputAreas<br>Flow_OutputStreams<br>Flow_OutputGroups<br>Flow_SubGroups<br>Flow_OutputItems<br>Flow_FlowItems |
| **Furnace** | AWSOA | Furnace_FurnaceBeds<br>Furnace_FurnaceSheets |
| **Maps** | AWProduction | Maps_Agents<br>Maps_Brokers<br>Maps_BookingActions<br>Maps_ClientConfigurations<br>Maps_GlassInstances<br>Maps_Hops<br>Maps_Locations<br>Maps_LocationGroups<br>Maps_Optimizations<br>Maps_Queries<br>Maps_ReservationTicketGroupEntries<br>Maps_Sorters<br>Maps_Tickets<br>Maps_TicketGroups<br>Maps_TicketGroupEntries<br>MZO_RealMaschine<br>MZO_PhysMaschine |
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
| **BOM** | AWProduction | ArtikelStamm<br>AWBar_Bearbeit<br>AWBar_InitData<br>BearbeitStamm<br>Bearb_Typ<br>Cap_Kosten<br>MZO_RealMaschine<br>MZO_Route_Map<br>Maps_Processings (View)<br>Modellstamm_Faktor<br>Modellstamm_Description<br>Pool_Auftrag<br>Pool_Bearbeit<br>Pool_Modell<br>Pool_Pos<br>Pool_Selektion<br>Pool_Teile<br>Prozesse<br>XOpt_Art<br>Zuschlag<br>Zuschlag_Artikel<br>Zuschlag_Masch<br>Zuschlag_Bearbeit |
| **DataProvider** | AWProduction | Parameter<br>CutGo_Cluster<br>CutGo_Cluster_Unit<br>Pool_GlasArt<br>XOpt_Art<br>XOpt_Jumbo<br>XOpt_Optimierung |
| **Detailed** | AWProduction | Parameter<br>Detail_CuttingResults<br>Detail_Jobs<br>Detail_Lots<br>Detail_LotItems<br>Detail_PlannedRacks<br>Detail_PlannedRackItems<br>Detail_WorkSteps<br>Fein_Teile<br>Fein_Unit |
| **Job** | AWProduction | Pool_Auftrag<br>Pool_Bearbeit<br>Pool_Bestellteile<br>Pool_Lauf<br>Pool_Pos<br>Pool_Teile<br>Pool_Modell<br>Pool_Selektion<br>Pool_Txt<br>Mzo_route_map<br>Prozesse |
| **Optimization** | AWSOA | Parameter<br>Zuschlag<br>Zuschlag_Artikel<br>Zuschlag_Masch<br>Zuschlag_Bearbeit<br>Opti_AutoRackSplits<br>Opti_BreakStartAndDirections<br>Opti_Channels<br>Opti_ChannelTypes<br>Opti_CombinedShapes<br>Opti_ControlParameters<br>Opti_Defects<br>Opti_InputGeometries<br>Opti_InputPrimitives<br>Opti_InvalidSheets<br>Opti_Jumbos<br>Opti_JumboWithDefectInfoes<br>Opti_KeepOrientations<br>Opti_LimitRackIdInSubPlates<br>Opti_MaximumWithCosts<br>Opti_MinimumWithCosts<br>Opti_OptimizationIds<br>Opti_OptimizationResults<br>Opti_OptimizationTasks<br>Opti_Patterns<br>Opti_ProductionGroups<br>Opti_ProductionItems<br>Opti_ProductionPanes<br>Opti_ProductionSequences<br>Opti_Rectangles<br>Opti_ResidualPatterns<br>Opti_RestrictionParameters<br>Opti_Sheets<br>Opti_Sorters<br>Opti_SpecialSheetAlignments<br>Opti_StockParameters<br>Opti_SubChannels<br>Opti_Trims |
| **Stock** | AWSOA | Stock_ArticleNumberMappings<br>Stock_GlassItems<br>Stock_GlassRequests<br>Stock_IORequests<br>Stock_Items<br>Stock_RackSheetRequests<br>Stock_Residuals<br>Stock_ResidualRequests<br>Stock_SegmentRequests<br>Stock_StockPlates<br>Stock_StockPlateReservations<br>Stock_StockSheets<br>Stock_StockSheetRequests<br>Stock_Storages<br>Stock_StorageLocations<br>Stock_StorageSegments<br>Stock_StorageSegmentProperties |

### 4.8. Web

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| **Configurator** | AWSOA | Web_Carts<br>Web_CartItems<br>Web_CartItemActions |

## 5. Domain Overview
*As of: 05.03.2025*

### Infrastructure Domain
*Associated with Ice Grid / Ice Strom*
*   BasicData Service
*   Database Service
*   Configuration Service
*   Protocolling Service
*   Collector Service
*   License Service
*   Workflow Service
*   Reporting Service
*   Infrastructure Web

### Corporate Domain
*   Dashboard Service
*   Gateway Service
*   KPI Service
*   Corporate Web (Dashboard)

### CAD Domain
*   Bar Service
*   Digitizing Service
*   Sheets Service
*   Geometry Service

### Facility Domain
*   Rack Service
*   Layout Service
*   Factory State Service

### Web Domain
*   Configurator Service
*   Web.Web (iQuote)

### Commercial Domain
*   Converter Service
*   DataProvider Service
*   Dispatch Service
*   Document Service
*   Exchange Service
*   Feedback Service
*   Logistic Service
*   LogisticBackend Service
*   (CA) Masterdata Service
*   Purchase Service
*   Sales Service
*   Stock Service
*   (CA) TransactionData Service

### Planning Domain
*   BOM Service
*   DataProvider Service
*   Detailed Service
*   Import Service
*   Job Service
*   Optimization Service
*   Stock Service
*   Automation Service
*   Planning Web (CapaView + Stock)

### CIM Domain
*   Barcoding Service
*   Flow Service
*   Furnace Service
*   Machinery Automation Service
*   MAPS Service
*   Quality Tracking Service
*   Sorter Service
*   Cutting Service
*   Driver Service
*   CIM Web (Barcoding + SmartTerminal)
