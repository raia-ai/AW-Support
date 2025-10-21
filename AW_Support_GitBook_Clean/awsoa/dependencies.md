title: "EN-INST-AW_SOA_Dependencies"
source: "EN-INST-AW_SOA_Dependencies.pdf"
tags: ["A+W", "AWSOA", "Software", "Dependencies", "SOA", "Technical Documentation", "Glass Industry", "Module Dependencies", "Database Access"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical document from A+W Software GmbH, detailing the dependencies for the A+W Service-Oriented Architecture (AWSOA). It outlines required setup dependencies for various modules, provides short descriptions of services, and specifies database and table access for different components as of October 2023."
long_description: "This document, titled \"A+W AWSOA Dependencies (as of 10/2023),\" is a comprehensive technical guide from A+W Software GmbH, a company specializing in software for the glass industry. It is designed for system administrators, developers, and technical consultants involved in the installation, configuration, and maintenance of the A+W Service-Oriented Architecture (AWSOA). The document begins with a table of contents and then delves into the core technical details. The main section, \"Module Dependencies,\" presents a detailed table listing various A+W modules (like CIM.Web, Corporate.Web, AWB/AWE - iQuote) and the specific AWSOA services they require to function correctly. This is crucial for ensuring a stable and operational system setup. Following this, the \"Services Short Description\" section provides a brief overview of the purpose of each service, categorized into domains such as Infrastructure, Facility, CAD, CIM, Corporate, Commercial, Planning, and Web. This helps users understand the function of each component within the larger architecture. A significant portion of the document, \"Access to databases and tables,\" provides explicit listings of the databases (e.g., AWSOA, AWProduction) and specific tables that each SOA service interacts with. This information is vital for database administration, troubleshooting, and understanding data flow. Finally, the \"Domain Overview\" section includes diagrams that visually represent the various service domains (Infrastructure, Corporate, CAD, Facility, Web, Commercial, Planning, CIM) and the services within them, offering a high-level architectural view. The document concludes with the contact information for A+W Software GmbH."
---

# A+W AWSOA Dependencies (as of 10/2023)

## 2. Module Dependencies

| Modules | Required AWSOA Setup Dependencies |
| :--- | :--- |
| All AWSOA Services | Infrastructure Middleware<br>Infrastructure Service Locator (Highlander!) |
| Infrastructure.Web | Infrastructure Collector Service<br>Infrastructure Services<br>Infrastructure Reporting Service (only needed for AWB CR) |
| CIM.Web<br>(Barcoding CE Scanner + SmartTerminal) | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services |
| Corporate.Web<br>(A+W Dashboard) | Infrastructure Services + Web<br>Corporate Dashboard Service<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services |
| Planning.Web<br>(CapaView + Stock/MRPS) | Infrastructure Services + Web<br>Planning DataProvider Service<br>Planning Job Service<br>optional: Cad Services<br>Planning Stock Service |
| AWB/AWE - iQuote<br>(Web.Web) | Infrastructure Services + Web<br>Infrastructure Reporting Service (AWB)<br>Web Configurator Service<br>Commercial Document Service<br>Commercial Converter Service (AWE)<br>CAD Geometry Service<br>AWB/AWE |
| Cantor - iQuote<br>(Web.Web) | Infrastructure Services + Web<br>Web Configurator Service<br>Commercial Document Service (Cantor)<br>Commercial TransactionData Service (Cantor)<br>Commercial MasterData Service (Cantor)<br>Cantor |
| AWB/AWE/Cantor – Route optimization (OTR) | Infrastructure Services + Web<br>Commercial Logistic Service<br>Commercial Logistic Backend Service (AWE/Cantor)<br>OTR |
| AWB - Delivery Date Check | Infrastructure Services + Web<br>Planning Import Service |
| AWB - File-less transfer to production | Infrastructure Services + Web<br>Exchange Service |
| AWB - Automatic process execution<br>(Ex-AIS) | Infrastructure Services + Web<br>Exchange Service |
| AWB - Crystal Report Print | Infrastructure Services + Web<br>Infrastructure Reporting Service |
| AWP Production Terminal<br>PPSWebService | Infrastructure Services + Web |
| RTO with A+W Residual Stock Manager | Infrastructure Services + Web<br>Planning Stock Service |

### CX Modules

| CX Modules | Required AWSOA Setup Dependencies |
| :--- | :--- |
| CX SmartCompanion (Production Module) | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services<br>AWP Booking Service<br>Facility Rack (only needed for AW RackManager Connection) |
| CX SmartCompanion - Cantor (Production Module) | Infrastructure Services + Web<br>Cantor CIM Barcoding Service<br>Cantor CIM SmartCompanion Service |
| CX SmartCompanion (Stock Module) | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services<br>Commercial Purchase Service (AWE – Linux)<br>Commercial Stock Service (AWE – Linux)<br>AWP Booking Service |
| CX SmartCompanion - Cantor (Stock Module) | Infrastructure Services + Web<br>Cantor Commercial Purchase Service<br>Cantor Commercial Stock Service |
| CX Dispatch | Infrastructure Services + Web<br>CIM Barcoding Service<br>Planning Job Service<br>optional: Cad Services<br>Commercial Dispatch Service (AWE – Linux) |
| CX iShape | Infrastructure Services + Web<br>CAD Digitizing Service<br>SN |
| RTO + CX PatternViewer | Infrastructure Services + Web<br>Planning Optimization Service<br>CIM Barcoding Service (reference mark/stamps/logo)<br>CAD Sheets Service (reference mark/stamps/logo) |
| CX SmartFactory | Infrastructure Services + Web<br>CIM Barcoding Service<br>CIM Maps Service<br>CIM Flow Service<br>CIM Furnace Service<br>CIM Sorter Service<br>Facility Layout Service<br>Facility FactoryState Service<br>Planning BOM Service<br>Planning DataProvider Service<br>Planning Detailed Service<br>Planning Job Service<br>Planning Stock Service<br>Cad Services<br>Planning Optimization Service<br>Planning Stock Service<br>Planning Web<br>AWP Booking Service<br>AWP AlcimServer<br>Upcoming Dependency: CX NextGenDynOpt |

### Future

| Future Modules | Required AWSOA Setup Dependencies |
| :--- | :--- |
| CX Sales | Infrastructure Services + Web<br>Commercial Sales Service (AWE – Linux) |
| CX IoT | Infrastructure Services + Web<br>CIM Quality Tracking Service<br>CIM Barcoding Service<br>Corporate Gateway Service<br>Planning Job Service<br>optional: Cad Services<br>AWP Booking Service<br>Commercial Purchase Service (AWE – Linux) |
| CX NextGenDynOpt | Infrastructure Services + Web<br>Facility Services<br>Facility FactoryState Services<br>Facility Layout Services<br>CIM Flow Service |

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
    *   **Sheets** (Referencemark for PV/DXF-Import functionality for SN)
*   **CIM**
    *   **Barcoding** (Dashboard Data & Wi-Fi Barcoding Scanner/Smart Terminal & SmartCompanion & MQTT API)
    *   **Flow** (SmartFactory flow control for providing overall sheet prioritization)
    *   **Furnace** (SmartFactory furnace control)
    *   **MachineryAutomation** (Control/Communication to cutting area machines – Hainan only)
    *   **Maps** (SmartFactory/Multi-stage Automatic Production System)
    *   **Quality Tracking** (Production batch tracking/tracing)
    *   **Sorter** (SmartFactory sorter control)
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
    *   **Detailed** (Detailed Scheduling via QuickOrga – SmartFactory, OXXO)
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
| BasicData | AWSOA | Core_Clients<br>Core_ClientAssignments<br>Core_Languages |
| Config | AWSOA | Core_ConfigDynamicComponents<br>Core_ConfigSysSwitches<br>Core_ConfigUserSwitches<br>Core_CustomTexts |
| Database | AWSOA | Core_DBProtocols<br>Core_DBUpdates<br>Core_DBVersions |
| License | AWSOA | Core_Lic2DeviceAssignments<br>Core_Lic2ForeignAssignments<br>Core_LicDeviceAssignments<br>Core_LicenseConnections<br>Core_LicenseInfoes<br>Core_LicenseParallelUsages<br>Core_LicenseTotalUsages<br>Core_LicenseUsages<br>Core_LicForeignAssignments |
| Reporting | AWSOA | Core_ReportFields<br>Core_ReportGroups<br>Core_Reports<br>Core_ReportTableFields<br>Core_ReportTables |
| Workflow | AWSOA | Core_WFActivities<br>Core_WFActivityArchives<br>Core_WFActivityAssignments |

### 4.2. Facility

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| Layout | AWSOA | Layout_ProcessingTypeMappings<br>Layout_RecipeMappings<br>Layout_Hops<br>Layout_Locations<br>Layout_Machines<br>Layout_Processings<br>Layout_ProductionAreas<br>Layout_ShopfloorConnectors |
| Rack | RackManager | RAOwner<br>RAOwnerGroup<br>RARack<br>RARackType |
| FactoryState | AlcimDB | AWBar_Teile<br>AWBar_Zustand<br>AWBar_ZustandTyp<br>BDEStat_ES |

### 4.3. CAD

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| Digitizing | AWSOA | CAD_DigiShapeContainers<br>CAD_DigiShapeInfoes |
| Sheets | AWSOA | CAD_Sheets_AttrParameters<br>CAD_Sheets_BlockAttr<br>CAD_Sheets_Blocks<br>CAD_Sheets_CADModels<br>CAD_Sheets_Entities<br>CAD_Sheets_Inserts<br>CAD_Sheets_Layers<br>CAD_Sheets_Paths |

### 4.4. CIM

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| Barcoding | AWProduction | AWBar_Bearbeit<br>AWBar_Booking<br>AWBar_Bruch<br>AWBar_Charge<br>AWBar_Gateway_Data<br>AWBar_Gateway_Machine_Data<br>AWBar_Gestelle<br>AWBar_GestDaten<br>AWBar_Historie<br>AWBar_Person<br>AWBar_Stellen<br>AWBar_StellenTyp<br>AWBar_Teile<br>AWBar_Zustand<br>AWBar_ZustandTyp<br>BDEStat_ES<br>Parameter |
| Flow | AWSOA | Flow_PrioritizationCriterias |
| Furnace | AWSOA | Furnace_FurnaceBeds<br>Furnace_FurnaceSheets |
| Maps | AWProduction | Maps_Agents<br>Maps_Brokers<br>Maps_ClientConfigurations<br>Maps_GlassInstances<br>Maps_Hops<br>Maps_Locations<br>Maps_LocationGroups<br>Maps_Optimizations<br>Maps_Queries<br>Maps_ReservationTicketGroupEntries<br>Maps_Sorters<br>Maps_Tickets<br>Maps_TicketGroups<br>Maps_TicketGroupEntries<br>MZO_RealMaschine<br>MZO_PhysMaschine |
| QualityTracking | AWSOA | Quality_TrackingData |

### 4.5. Commercial

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| Logistic | AWSOA | Comm_Breakages<br>Comm_Containers<br>Comm_Destinations<br>Comm_Documents<br>Comm_ItemContainers<br>Comm_Items<br>Comm_Routes |

### 4.6. Corporate

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| Dashboard | AWSOA | Dashboard_ClientViews<br>Dashboard_Containers<br>Dashboard_Controls<br>Dashboard_Pages<br>Dashboard_Panes<br>Dashboard_PaneControls<br>Dashboard_Views<br>Dashboard_ViewPages |

### 4.7. Planning

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| Automation | AWSOA | Planning_JobRelease |
| BOM | AWProduction | ArtikelStamm<br>AWBar_Bearbeit<br>AWBar_InitData<br>BearbeitStamm<br>Bearb_Typ<br>Cap_Kosten<br>MZO_RealMaschine<br>MZO_Route_Map<br>Maps_Processings (View)<br>Modellstamm_Faktor<br>Modellstamm_Description<br>Pool_Auftrag<br>Pool_Bearbeit<br>Pool_Modell<br>Pool_Pos<br>Pool_Selektion<br>Pool_Teile<br>XOpt_Art<br>Zuschlag<br>Zuschlag_Artikel<br>Zuschlag_Masch<br>Zuschlag_Bearbeit<br>Parameter |
| DataProvider | AWProduction | CutGo_Cluster<br>CutGo_Cluster_Unit<br>Pool_GlasArt<br>XOpt_Art<br>XOpt_Jumbo<br>XOpt_Optimierung<br>Parameter |
| Detailed | AWProduction | Detail_CuttingResults<br>Detail_Jobs<br>Detail_Lots<br>Detail_LotItems<br>Detail_PlannedRacks<br>Detail_PlannedRackItems<br>Detail_WorkSteps<br>Fein_Teile<br>Fein_Unit |
| Job | AWProduction | Pool_Auftrag<br>Pool_Bearbeit<br>Pool_Bestellteile<br>Pool_Lauf<br>Pool_Pos<br>Pool_Teile<br>Pool_Modell<br>Pool_Selektion<br>Pool_Txt<br>Mzo_route_map<br>Prozesse<br>Parameter<br>Zuschlag<br>Zuschlag_Artikel<br>Zuschlag_Masch<br>Zuschlag_Bearbeit |
| Optimization | AWSOA | Opti_Defects<br>Opti_OptimizationResults<br>Opti_Patterns<br>Opti_Rectangles<br>Opti_Shapes<br>Opti_Sheets |
| Stock | AWSOA | Stock_ArticleNumberMappings<br>Stock_GlassItems<br>Stock_GlassRequests<br>Stock_IORequests<br>Stock_Items<br>Stock_RackSheetRequests<br>Stock_Residuals<br>Stock_ResidualRequests<br>Stock_SegmentRequests<br>Stock_StockPlates<br>Stock_StockPlateReservations<br>Stock_StockSheets<br>Stock_StockSheetRequests<br>Stock_Storages<br>Stock_StorageLocations<br>Stock_StorageSegments<br>Stock_StorageSegmentProperties |

### 4.8. Web

| SOA Service | Database | Tables |
| :--- | :--- | :--- |
| Configurator | AWSOA | Web_Carts<br>Web_CartItems<br>Web_CartItemActions |

## 5. Domain Overview

(Stand: 03.03.2023)

### Infrastructure Domain
*   BasicData Service
*   Database Service
*   Configuration Service
*   Protocolling Service
*   Collector Service
*   License Service
*   Workflow Service
*   Reporting Service
*   Infrastructure Web
*   (Ice Grid/Ice Storm)

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
*   FactoryState Service

### Web Domain
*   Configurator Service
*   Web Web (iQuote)

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
*   Planing Web (CapaView + Stock)

### CIM Domain
*   Barcoding Service
*   Flow Service
*   Furnace Service
*   Machinery Automation Service
*   MAPS Service
*   QualityTracking Service
*   Sorter Service
*   CIM Web (Barcoding + SmartTerminal)

## 6. Contact Address

**A+W Software GmbH**

Am Pfahlgraben 4 - 10  
35415 Pohlheim  
Germany

Tel. +49 6404 2051 0  
Fax. +49 6404 2051 877

E-Mail: zentrale@a-w.com  
Internet: http://www.a-w.com/
