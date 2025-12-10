---
description: "EN CONFIG A+W SOA Dependencies"
---



# EN CONFIG A+W SOA Dependencies

     Configuration
                     3



AWSOA Dependencies (as of
03/2025)




                            english
1. Content
1.   Content                                                         3
2.   Module Dependencies                                             4
3.   Services Short Description                                      9
4.   Access to databases and tables                                 11
     4.1. Infrastructure                                            11
     4.2. Facility                                                  11
     4.3. CAD                                                       12
     4.4. CIM                                                       12
     4.5. Commercial                                                13
     4.6. Corporate                                                 13
     4.7. Planning                                                  14
     4.8. Web                                                       16
5.   Domain Overview                                                17




A+W Software GmbH             EN-CONFIG-A+W SOA Dependencies.docx        3
2. Module Dependencies
Modules                                  Required AWSOA Setup Dependencies
All AWSOA Services                       Infrastructure Middleware
                                         Infrastructure Service Locator (Highlander!)
Infrastructure.Web                       Infrastructure Collector Service
                                         Infrastructure Services
                                         Infrastructure Reporting Service (only needed for AWB CR)
CIM.Web                                  Infrastructure Services + Web
(Barcoding CE Scanner + SmartTerminal)   CIM Barcoding Service
                                         Planning                     Job                   Service
                                         optional: Cad Services
Corporate.Web                            Infrastructure Services + Web
(A+W Dashboard)                          Corporate Dashboard Service
                                         CIM Barcoding Service
                                         Planning                     Job                   Service
                                         optional: Cad Services
                                         Planning DataProvider Service
Planning.Web                             Infrastructure Services + Web
(CapaView + Stock/MRPS)                  Planning DataProvider Service
                                         Planning                     Job                   Service
                                         optional: Cad Services
                                         Planning Stock Service
AWB/AWE - iQuote                         Infrastructure Services + Web
(Web.Web)                                Infrastructure Reporting Service (AWB)
                                         Web Configurator Service
                                         Commercial Document Service
                                         Commercial Converter Service (AWE)
                                         CAD Geometry Service
                                         AWB/AWE
Cantor - iQuote                          Infrastructure Services + Web
(Web.Web)                                Web Configurator Service
                                         Commercial Document Service (Cantor)
                                         Commercial TransactionData Service (Cantor)
                                         Commercial MasterData Service (Cantor)
                                         Cantor
AWB/AWE/Cantor –                         Infrastructure Services + Web
Route optimization (OTR)                 Commercial Logistic Service
                                         Commercial Logistic Backend Service (AWE/Cantor)
                                         OTR
AWB – Delivery Date Check                Infrastructure Services + Web
AWB – File-less transfer to production   Planning Import Service
AWB – Automatic process execution        Infrastructure Services + Web
(Ex-AIS)                                 Exchange Service
AWB – Crystal Report Print               Infrastructure Services + Web
                                         Infrastructure Reporting Service
AWP Production Terminal                  Infrastructure Services + Web
PPSWebService


A+W Software GmbH              EN-CONFIG-A+W SOA Dependencies.docx                            4
RTO with A+W Residual Stock Manager   Infrastructure Services + Web
                                      Planning Stock Service




A+W Software GmbH           EN-CONFIG-A+W SOA Dependencies.docx       5
CX Modules
CX SmartCompanion (Production Module) Infrastructure Services + Web
                                       CIM Barcoding Service
                                       Planning Job Service
                                       optional: Cad Services
                                       AWP Booking Service
                                       Facility Rack (only needed for AW RackManager
                                       Connection)
CX SmartCompanion - Cantor (Production Infrastructure Services + Web
Module)                                Cantor CIM Barcoding Service
                                       Cantor CIM SmartCompanion Service
CX SmartCompanion (Stock Module)       Infrastructure Services + Web
                                       CIM Barcoding Service
                                       Planning Job Service
                                       optional: Cad Services
                                       Commercial Purchase Service (AWE – Linux)
                                       Commercial Stock Service (AWE – Linux)
                                       AWP Booking Service
CX SmartCompanion - Cantor (Stock Infrastructure Services + Web
Module)                                Cantor Commercial Purchase Service
                                       Cantor Commercial Stock Service
CX Dispatch                            Infrastructure Services + Web
                                       CIM Barcoding Service
                                       Planning Job Service
                                       optional: Cad Services
                                       Commercial Dispatch Service (AWE – Linux)
CX iShape                              Infrastructure Services + Web
                                       CAD Digitizing Service
                                       SN
RTO + CX PatternViewer                 Infrastructure Services + Web
                                       Planning Optimization Service
                                       CIM Barcoding Service (reference mark/stamps/logo)
                                       CAD Sheets Service (reference mark/stamps/logo)
CX SmartFactory                        Infrastructure Services + Web
                                       CIM Barcoding Service
                                       CIM Maps Service
                                       CIM Flow Service
                                       CIM Furnace Service
                                       CIM Sorter Service
                                       Facility Layout Service
                                       Facility FactoryState Service
                                       Planning BOM Service
                                       Planning DataProvider Service
                                       Planning Detailed Service
                                       Planning Job Service
                                       Planning Stock Service
                                       Cad Services
                                       Planning Optimization Service
                                       Planning Stock Service


A+W Software GmbH           EN-CONFIG-A+W SOA Dependencies.docx                         6
                              Planning Web
                              AWP Booking Service
                              AWP AlcimServer
                              Upcoming Dependency: CX NextGenDynOpt




A+W Software GmbH   EN-CONFIG-A+W SOA Dependencies.docx               7
Future
CX Sales                      Infrastructure Services + Web
                              Commercial Sales Service (AWE – Linux)
CX IoT                        Infrastructure Services + Web
                              CIM QualityTracking Service
                              CIM Barcoding Service
                              Corporate Gateway Service
                              Planning Job Service
                              optional: Cad Services
                              AWP Booking Service
                              Commercial Purchase Service (AWE – Linux)
CX NextGenDynOpt              Infrastructure Services + Web
                              Facility Services
                              Facility FactoryState Services
                              Facility Layout Services
                              CIM Flow Service
                              CIM Cutting Service




A+W Software GmbH   EN-CONFIG-A+W SOA Dependencies.docx                   8
3. Services Short Description
•   Infrastructure
    •   BasicData (Clients/Sites, User Assignments & Languages)
    •   Configuration (Switches)
    •   Database (Database Update)
    • License (License, License Usage Register/View – Production Terminal/PPSWebService,
    Licensing for SmartCompanion)
    •   Protocol + Collector (Protocol Viewer + Alert Email messaging)
    •   Reporting (AWB – Crystal Report Printing)
    •   Workflow (Workflow Management)
•   Facility
    • Layout (NextGenDynOpt and A+W SmartFactory for providing machinery/shopfloor
    layouts and machinery “localization” mappings)
    •   Rack (AW RackManager Connection for SmartCompanion)
    •     FactoryState (Gets machinery state and sets machinery states)
•   CAD
    •   Bar (Bar/Muntin management)
    •   Digitizing (Picture processing for iShape)
    •   Geometry (Shapes and processing pictures for iQuote)
    •   Sheets (Referencemark for PV/DXF Import functionality for SN)
•   CIM
    •   Barcoding (Dashboard Data & Wi-Fi Barcoding Scanner/Smart Terminal &
        SmartCompanion & MQTT API)
    •   Flow (SmartFactory flow control for providing overall sheet prioritization)
    •   Furnace (SmartFactory furnace control)
    •   MachineryAutomation (Control/Communication to cutting area machines – Hainan only)
    •   Maps (SmartFactory/Multi-stage Automatic Production System)
    •   Quality Tracking (Production batch tracking/tracing)
    •   Sorter (SmartFactory sorter control)
    •   Cutting (NGD Cutting control)
    •   Driver (NGD driver control for cutting tables)
•   Corporate
    •   Dashboard (Dashboard)
    •   Gateway (IoT Platform/Connection to Actiware)



A+W Software GmbH               EN-CONFIG-A+W SOA Dependencies.docx                          9
    •   KPI (Dashboard connection to Cantor - deprecated)
•   Commercial
    •   Converter (AWEnterprise FIX connection, AWDesign + SN pictures for iQuote (AWE))
    •   DataProvider (ClarityExperience Dispatch + Sales UI)
    •   Dispatch (ClarityExperience Disptach UI)
    •   Document (Connection of ERP Solution for iQuote AWB/AWE/Cantor)
    •   Exchange (Automatic process execution (Ex-AIS), Communication with SGG-WebService)
    •   Logistic (OTR)
    •   LogisticBackend (OTR connection to Cantor or AWE)
    •   MasterData (Master data exchange with Cantor)
    •   Purchase (SmartCompanion Stock + IoT Platform)
    •   Sales (ClarityExperience Sales UI)
    •   Stock (SmartCompanion Stock)
    •   TransactionData (Order data exchange with Cantor)
•   Planning
    •   BOM (Bill of Material, SmartFactory)
    •   DataProvider (Legacy database table reading support & Dashboard Data)
    •   Detailed (Detailed Scheduling via QuickOrga – SmartFactory, OXXO)
    •   Import (AWB Delivery DateCheck & File-less transfer to production)
    • Job (CapaView & Rough Scheduling & Barcoding & Dashboard Data & SmartCompanion &
    SmartFactory)
    •   Optimization (Optimization for RTO with PatternViewer, Furnace Opti SmartFactory)
    •   Stock (Stock management/Sorter management SmartFactory /RTO with RPMS)
    • Automation (Workflow controlled Rough-, Detailed-Scheduling and DynOpt Import – OXXO
    only)
•   Web
    •   Configurator (iQuote)




A+W Software GmbH               EN-CONFIG-A+W SOA Dependencies.docx                         10
4. Access to databases and tables
4.1. Infrastructure
SOA Service         Database      Tables
BasicData           AWSOA         Core_Clients
                                  Core_ClientAssignments
                                  Core_Languages
Config              AWSOA         Core_ConfigDynamicComponents
                                  Core_ConfigSysSwitches
                                  Core_ConfigUserSwitches
                                  Core_CustomTexts
Database            AWSOA         Core_DBProtocols
                                  Core_DBUpdates
                                  Core_DBVersions
License             AWSOA         Core_Lic2DeviceAssignments
                                  Core_Lic2ForeignAssignments
                                  Core_LicDeviceAssignments
                                  Core_LicenseConnections
                                  Core_LicenseInfoes
                                  Core_LicenseParallelUsages
                                  Core_LicenseTotalUsages
                                  Core_LicenseUsages
                                  Core_LicForeignAssignments
Reporting           AWSOA         Core_ReportFields
                                  Core_ReportGroups
                                  Core_Reports
                                  Core_ReportTableFields
                                  Core_ReportTables
Workflow            AWSOA         Core_WFActivities
                                  Core_WFActivityArchives
                                  Core_WFActivityAssignments


4.2. Facility
SOA Service         Database      Tables
Layout              AWSOA         Layout_ProcessingTypeMappings
                                  Layout_RecipeMappings
                                  Layout_Hops
                                  Layout_Locations
                                  Layout_Machines
                                  Layout_Processings
                                  Layout_ProductionAreas
                                  Layout_ShopfloorConnectors
Rack                RackManager   RAOwner
                                  RAOwnerGroup
                                  RARack


A+W Software GmbH         EN-CONFIG-A+W SOA Dependencies.docx     11
                                   RARackType
FactoryState        AlcimDB        AWBar_Teile
                                   AWBar_Zustand
                                   AWBar_ZustandTyp
                                   BDEStat_ES




4.3. CAD
SOA Service         Database       Tables
Digitizing          AWSOA          CAD_DigiShapeContainers
                                   CAD_DigiShapeInfoes
Sheets              AWSOA          CAD_Sheets_AttrParameters
                                   CAD_Sheets_BlockAttr
                                   CAD_Sheets_Blocks
                                   CAD_Sheets_CADModels
                                   CAD_Sheets_Entities
                                   CAD_Sheets_Inserts
                                   CAD_Sheets_Layers
                                   CAD_Sheets_Paths


4.4. CIM
SOA Service         Database       Tables
Barcoding           AWProduction   AWBar_Bearbeit
                                   AWBar_Booking
                                   AWBar_Bruch
                                   AWBar_Charge
                                   AWBar_Gateway_Data
                                   AWBar_Gateway_Machine_Data
                                   AWBar_Gestelle
                                   AWBar_GestDaten
                                   AWBar_Historie
                                   AWBar_Person
                                   AWBar_Stellen
                                   AWBar_StellenTyp
                                   AWBar_Teile
                                   AWBar_Zustand
                                   AWBar_ZustandTyp
                                   BDEStat_ES

                                   Parameter
Flow                AWSOA          Flow_PrioritizationCriterias
                                   Flow_OutputAreas
                                   Flow_OutputStreams
                                   Flow_OutputGroups
                                   Flow_SubGroups
                                   Flow_OutputItems


A+W Software GmbH         EN-CONFIG-A+W SOA Dependencies.docx     12
                                   Flow_FlowItems
Furnace             AWSOA          Furnace_FurnaceBeds
                                   Furnace_FurnaceSheets
Maps                AWProduction   Maps_Agents
                                   Maps_Brokers
                                   Maps_BookingActions
                                   Maps_ClientConfigurations
                                   Maps_GlassInstances
                                   Maps_Hops
                                   Maps_Locations
                                   Maps_LocationGroups
                                   Maps_Optimizations
                                   Maps_Queries
                                   Maps_ReservationTicketGroupEntries
                                   Maps_Sorters
                                   Maps_Tickets
                                   Maps_TicketGroups
                                   Maps_TicketGroupEntries

                                   MZO_RealMaschine
                                   MZO_PhysMaschine
QualityTracking     AWSOA          Quality_TrackingData


4.5. Commercial
SOA Service         Database       Tables
Logistic            AWSOA          Comm_Breakages
                                   Comm_Containers
                                   Comm_Destinations
                                   Comm_Documents
                                   Comm_ItemContainers
                                   Comm_Items
                                   Comm_Routes


4.6. Corporate
SOA Service         Database       Tables
Dashboard           AWSOA          Dashboard_ClientViews
                                   Dashboard_Containers
                                   Dashboard_Controls
                                   Dashboard_Pages
                                   Dashboard_Panes
                                   Dashboard_PaneControls
                                   Dashboard_Views
                                   Dashboard_ViewPages




A+W Software GmbH         EN-CONFIG-A+W SOA Dependencies.docx           13
4.7. Planning
SOA Service         Database       Tables
Automation          AWSOA          Planning_JobRelease
BOM                 AWProduction   ArtikelStamm
                                   AWBar_Bearbeit
                                   AWBar_InitData
                                   BearbeitStamm
                                   Bearb_Typ
                                   Cap_Kosten
                                   MZO_RealMaschine
                                   MZO_Route_Map
                                   Maps_Processings (View)
                                   Modellstamm_Faktor
                                   Modellstamm_Description
                                   Pool_Auftrag
                                   Pool_Bearbeit
                                   Pool_Modell
                                   Pool_Pos
                                   Pool_Selektion
                                   Pool_Teile
                                   XOpt_Art
                                   Zuschlag
                                   Zuschlag_Artikel
                                   Zuschlag_Masch
                                   Zuschlag_Bearbeit

                                   Parameter
DataProvider        AWProduction   CutGo_Cluster
                                   CutGo_Cluster_Unit
                                   Pool_GlasArt
                                   XOpt_Art
                                   XOpt_Jumbo
                                   XOpt_Optimierung

                                   Parameter
Detailed            AWProduction   Detail_CuttingResults
                                   Detail_Jobs
                                   Detail_Lots
                                   Detail_LotItems
                                   Detail_PlannedRacks
                                   Detail_PlannedRackItems
                                   Detail_WorkSteps
                                   Fein_Teile
                                   Fein_Unit
Job                 AWProduction   Pool_Auftrag
                                   Pool_Bearbeit
                                   Pool_Bestellteile
                                   Pool_Lauf
                                   Pool_Pos

A+W Software GmbH         EN-CONFIG-A+W SOA Dependencies.docx   14
                                Pool_Teile
                                Pool_Modell
                                Pool_Selektion
                                Pool_Txt
                                Mzo_route_map
                                Prozesse

                                Parameter
                                Zuschlag
                                Zuschlag_Artikel
                                Zuschlag_Masch
                                Zuschlag_Bearbeit
Optimization        AWSOA       Opti_AutoRackSplits
                                Opti_BreakStartAndDirections
                                Opti_Channels
                                Opti_ChannelTypes
                                Opti_CombinedShapes
                                Opti_ControlParameters
                                Opti_Defects
                                Opti_InputGeometries
                                Opti_InputPrimitives
                                Opti_InvalidSheets
                                Opti_Jumbos
                                Opti_JumboWithDefectInfoes
                                Opti_KeepOrientations
                                Opti_LimitRackIdInSubPlates
                                Opti_MaximumWithCosts
                                Opti_MinimumWithCosts
                                Opti_OptimizationIds
                                Opti_OptimizationResults
                                Opti_OptimizationTasks
                                Opti_Patterns
                                Opti_ProductionGroups
                                Opti_ProductionItems
                                Opti_ProductionPanes
                                Opti_ProductionSequences
                                Opti_Rectangles
                                Opti_ResidualPatterns
                                Opti_RestrictionParameters
                                Opti_Sheets
                                Opti_Sorters
                                Opti_SpecialSheetAlignments
                                Opti_StockParameters
                                Opti_SubChannels
                                Opti_Trims
Stock               AWSOA       Stock_ArticleNumberMappings
                                Stock_GlassItems
                                Stock_GlassRequests
                                Stock_IORequests
                                Stock_Items


A+W Software GmbH       EN-CONFIG-A+W SOA Dependencies.docx    15
                                  Stock_RackSheetRequests
                                  Stock_Residuals
                                  Stock_ResidualRequests
                                  Stock_SegmentRequests
                                  Stock_StockPlates
                                  Stock_StockPlateReservations
                                  Stock_StockSheets
                                  Stock_StockSheetRequests
                                  Stock_Storages
                                  Stock_StorageLocations
                                  Stock_StorageSegments
                                  Stock_StorageSegmentProperties


4.8. Web
SOA Service         Database      Tables
Configurator        AWSOA         Web_Carts
                                  Web_CartItems
                                  Web_CartItemActions




A+W Software GmbH         EN-CONFIG-A+W SOA Dependencies.docx      16
5. Domain Overview




A+W Software GmbH   EN-CONFIG-A+W SOA Dependencies.docx   17
A+W Software GmbH   EN-CONFIG-A+W SOA Dependencies.docx   18

