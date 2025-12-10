---
title: "EN-INST-AW_Clarity_SmartFactory"
source: "EN-INST-AW_Clarity_SmartFactory.pdf"
tags: ["A+W Clarity", "Smart Factory", "Installation Instructions", "Automated Production", "Software for Glass", "MAPS", "HEGLA Sortjet", "North-Glass Furnace", "Technical Documentation", "Software Configuration"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides installation instructions for the Beta version of A+W Clarity Smart Factory, a multistep automated production software for glass and windows. It details system requirements, installation procedures for core components like the database and MAPS service, and configuration for various shopfloor clients such as HEGLA Sortjet and North-Glass furnaces."
long_description: "This document is a comprehensive installation guide for the \"A+W Clarity Smart Factory - Multistep Automated Production\" software, a multi-level automated production system (MAPS). It is intended for planners and technicians responsible for installing and configuring the software. The guide details system requirements, including necessary A+W Production, StockService, and OptimizationService components, and specific Informix database settings. It provides step-by-step instructions for installing the database schema, master data, MAPS service, and various shopfloor clients (e.g., Dynopt Filler, HEGLA Sortjet, North-Glass furnace). The document also explains the internal ticket system, lite statuses, and the flow of production within the Smart Factory. Key configuration areas, such as setting up sorters, furnace optimization, and integrating with Panorama clients, are covered in depth with XML examples. Finally, it addresses advanced topics like handling production sections (diving), breakage management, timeline structuring, and PDC connections."
---

# Installation Instructions
**Beta - A+W Clarity Smart Factory - Multistep Automated Production**

---
## Change history:

| Date | Author | Comments | Version |
| :--- | :--- | :--- | :--- |
| 2019-03-21 | DLA | Document created | 1.0 |
| ... | ... | ... | ... |
| 2021-01-18 | MME | "SwapFour" as new method for buffer slot assignment | 2.30 |
| 2021-01-21 | DLA | Time horizon | 2.31 |
| 2021-02-09 | MISC | New sort mode for sorter | 2.32 |
| 2021-02-19 | MPH | Supply Dialog BSG In | 2.33 |
| 2021-04-07 | DLA | Validation Status | 2.34 |
| 2021-04-09 | DLA | Clarity Suite | 2.35 |
| 2021-05-06 | MPH | Call dialogs | 2.36 |
| 2021-05-18 | DLA | BDE goes SMF | 2.37 |
| 2021-07-07 | DLA | Assembling units | 2.38 |

The installation instructions will assist the planner with the installation and configuration of the software named.

## 1 Requirements
A+W Clarity SmartFactory is a multi-level automated production system (MAPS). It requires a run-capable A+W Production SingleSite environment.
The associated infrastructure domain has to be configured, the default client is used.
MAPS requires the following services from the AWSOA:
- Planning.Job
- Planning.BOM
- Planning.Detailed
- Planning.StockService
- Planning.OptimizationService
- CIM.Maps
- CIM.BarcodeReading

### 1.1 Informix
If A+W Production is running under INFORMIX, there can be problems with the "InsertCursor". Here, it is recommended that you switch off the "InsertCursor" in the infrastructure in the configuration of the A+W production (EnableInsertCursors=0). For the AWSOA database under Informix, this also in the ODBC settings.

**Figure 1-1 Informix configuration**
The connection string in the IBM Informix ODBC Driver Setup should be modified to include `EnableInsertCursors=0`.
```
dsn=${DataSourceName};uid=${DatabaseUser};pwd=${DatabasePassword};EnableInsertCursors=0
```
The "Insert Cursors" option in the driver setup should be unchecked.

### 1.2 A+W Production
For all places defined in MAPS, there has to be a corresponding registration point in A+W Production. These can be used by the MAPS clients in order to trigger bookings.
Output from the MAPS system and sorter require no definition in the machine assignment; other places do, however.
The sequence of the processings in A+W Production has to correspond to the sequence defined in MAPS since MAPS tries to arrange a BOM as transferred.
Example: [Cutting - Stamping - Grinding - Sorter] is the sequence in MAPS, for 3 processings for cutting, stamping, and grinding have to exist in the BOM in precisely this sequence.

### 1.3 A+W StockService
Each sorter that should be controlled via the MAPS system (currently HEGLA Sortjets are supported) has to be mapped in the SortingService (function of the A+W StockService). This way, MAPS saves the state of the sorter; this is required, for example, in order to synchronize with the sorter.
Communication runs via a MAPS ShopFloor client for the Sortjet.
The configuration of a Sortjet is currently done via SQL and can look as follows for a Sortjet with 2 physical buffers and 4 virtual ones. The GUIDs in the SQLs are examples!

```sql
INSERT INTO Stock_Storages (Guid, VersionId, LockingToken, Id, Description) VALUES ('99aff9d1-b89e-43f2-ab2c-aabf00a15a8e', 1, '00000000-0000-0000-0000-000000000000', 1, 'SortJet');

INSERT INTO Stock_StorageLocations (Guid, VersionId, LockingToken, Id, Description, Type, State, LockId, StorageGuid) VALUES ('a1c15e0a-e736-4d56-bc3c-aabf00a15a9c', 1, '00000000-0000-0000-0000-000000000000', 1, 'Pyhsical Buffer 1', 2, 1, '', '99aff9d1-b89e-43f2-ab2c-aabf00a15a8e');
INSERT INTO Stock_StorageLocations (Guid, VersionId, Locking Token, Id, Description, Type, State, LockId, StorageGuid) VALUES ('84c1f6c7-d980-41b4-8b5d-aabf00a15aa1', 1, '00000000-0000-0000-0000-000000000000', 2, 'Physical Buffer 2', 2, 1, '', '99aff9d1-b89e-43f2-ab2c-aabf00a15a8e');

INSERT INTO Stock_StorageSegmentProperties (Guid, VersionId, Locking Token, Description, AccessBehavior, SegmentType, MaxThickness, MaxHeight, MaxWidth, StartGroupNr, MaxGroupCount, MaxWeight, MinHeight, MinWidth, MinThickness, DistanceBetweenItems) VALUES ('09df2f5d-1f4a-4f15-970a-aabf00a15aa1', 1, '00000000-0000-0000-0000-000000000000', 'Virtual Buffer 1', 2, 3, 12000, 2300000, 6000000, 1, 75, 6000, 250000, 350000, 4000, 0);
INSERT INTO Stock_StorageSegmentProperties (Guid, VersionId, Locking Token, Description, AccessBehavior, SegmentType, Max Thickness, MaxHeight, MaxWidth, StartGroupNr, MaxGroupCount, MaxWeight, MinHeight, MinWidth, MinThickness, DistanceBetween Items) VALUES ('dd1679d3-6992-4b94-8a35-aabf00a15aa6', 1, '00000000-0000-0000-0000-000000000000', 'Virtual Buffer 2', 2, 3, 12000, 2800000, 6000000, 1, 275, 6000, 250000, 350000, 4000, 0);
INSERT INTO Stock_StorageSegment Properties (Guid, VersionId, LockingToken, Description, AccessBehavior, SegmentType, Max Thickness, MaxHeight, MaxWidth, StartGroupNr, MaxGroupCount, MaxWeight, MinHeight, MinWidth, MinThickness, DistanceBetween Items) VALUES ('0e554c05-1944-435f-8b50-aabf00a15aaa', 1, '00000000-0000-0000-0000-000000000000', 'Virtual Buffer 3', 2, 3, 12000, 2800000, 6000000, 1, 125, 6000, 250000, 350000, 4000, 0);
INSERT INTO Stock_StorageSegmentProperties (Guid, VersionId, LockingToken, Description, AccessBehavior, SegmentType, Max Thickness, MaxHeight, MaxWidth, StartGroupNr, MaxGroupCount, MaxWeight, MinHeight, MinWidth, MinThickness, DistanceBetweenItems) VALUES ('0a1c2fd4-00d7-47ee-a94e-aabf00a15aaa', 1, '00000000-0000-0000-0000-000000000000', 'Virtual Buffer 4', 2, 3, 19000, 2300000, 6000000, 1, 50, 6000, 250000, 350000, 10000, 0);

INSERT INTO Stock_StorageSegments (Guid, VersionId, Locking Token, Id, Description, State, LockId, StorageLocationGuid, PropertiesGuid) VALUES ('75e23876-a798-459a-9954-aabf00a15aaa', 1, '00000000-0000-0000-0000-000000000000', 1, 'Virtual Buffer 1', 1, '', 'a1c15e0a-e736-4d56-bc3c-aabf00a15a9c', '09df2f5d-1f4a-4f15-970a-aabf00a15aa1');
INSERT INTO Stock_StorageSegments (Guid, VersionId, LockingToken, Id, Description, State, LockId, StorageLocationGuid, PropertiesGuid) VALUES ('aec580be-c24b-4eb0-9706-aabf00a15aaf', 1, '00000000-0000-0000-0000-000000000000', 2, 'Virtual Buffer 2', 1, '', 'a1c15e0a-e736-4d56-bc3c-aabf00a15a9c', 'dd1679d3-6992-4b94-8a35-aabf00a15aa6');
INSERT INTO Stock_StorageSegments (Guid, VersionId, LockingToken, Id, Description, State, LockId, StorageLocationGuid, PropertiesGuid) VALUES ('10820fb1-3f52-428d-b2ab-aabf00a15aaf', 1, '00000000-0000-0000-0000-000000000000', 3, 'Virtual Buffer 3', 1, '', '84c1f6c7-d980-41b4-8b5d-aabf00a15aa1', '0e554c05-1944-435f-8b50-aabf00a15aaa');
INSERT INTO Stock_StorageSegments (Guid, VersionId, LockingToken, Id, Description, State, LockId, StorageLocationGuid, PropertiesGuid) VALUES ('094cadb4-60ed-4583-b7c0-aabf00a15aaf', 1, '00000000-0000-0000-0000-000000000000', 4, 'Virtual Buffer 4', 1, '', '84c1f6c7-d980-41b4-8b5d-aabf00a15aa1', '0a1c2fd4-00d7-47ee-a94e-aabf00a15aaa');
```
If additional buffers should be created, attention should be paid that the IDs of the physical and virtual buffers in the StockService are unique. This means that the second Sortjet cannot have the ID 1 for its first physical buffer. In this case, it could be number 3. The implementation between ID in the StockService and that of HEGGLA for the control of the Sortjet is done in the MAPS Sortjet client.

### 1.4 A+W OptimizationService for furnace optimization
The A+W Optimization service is required in order to conduct furnace optimizations in the furnace client and to retain the result. The result is required in order to move furnace beds in and out of the Sortjet.
For details about the configuration of the furnace optimization in the A+W Optimization service, please see the appropriate documentation. Currently it is so that the optimization itself is still done via the BATCH file `ORGA.BAT`. This configuration is saved in the Windows user directory of the user of the service:
`C:\Users\{AWSOA Dienst Benutzer}\AppData\Roaming\A+W\Techsoft\XOPT\Ofenopti\`
On the first start, the data is copied from the program directory into the user directory:
`{ProgramFilesx86}\A+W\Techsoft\XOPT\Ofenopti\`
Configuration files such as `XOPT.CFG` and `LABEL.SET` are also in this directory. In the `LABEL.SET`, as in A+W Production, a barcode has to be defined.
Via the `XOPT.CFG`, the behavior of the optimization can be adjusted accordingly. The following switches can be important:

- **ReduceFurnaceBedLength**
  0 (Default) / 1; If active, tries to keep the optimization of a furnace bed as short as possible
- **FurnaceBedsToCompute**
  Currently, the furnace optimization only uses and produces the first furnace bed. The others are discarded. With this switch, the furnace optimization can be configured so that only the first furnace bed is used. The optimization is also faster since it doesn't have to compute to the end. If the switch is set, the first N furnace beds are used, e.g.: `FurnaceBedsToCompute=1`

## 2 Installation
An installation consists of several components: the MAPS service, the MAPS navigator, several MAPS ShopFloor clients, and possibly several additional clients, which are integrated in Panorama scripts, for example.

### 2.1 Database
Data is stored in the A+W Production database in individual tables (prefix of the tables: `Maps_`). The data structure has to be created by hand using an SQL editor since there are still no automatic database update scripts.
The corresponding SQL script (`MapsDatabaseSchemaSQLServer.sql` or `MapsDatabaseSchemaInformix.sql`) is found in the installed service in the subfolder `Database`.
In addition, the database VIEW `maps_processings` in the A+W Production database is required. These also have to be installed manually from the SQL file `maps_processings.sql`.

### 2.2 Master data
Master data has to be filled manually via a SQL because there are still no master data editors. The script `MAPSMasterDataDefaultContent.sql` can serve for support.
When creating the master data, pay attention to the following. Each MAPS client that makes bookings requires a registration point and a person with which the booking is done. This data has to be created in the PDC master data. MAPS locations that are not sorters or outputs also require a corresponding MZO machine ID.
In the master data there are agents (`Maps_Agents`), each of which manages a production area. If the agent is a Sortjet, then the corresponding sorter (`Maps_Sorters`) has to be assigned. What kind of type the agent is has to be defined. Currently, there are the following types for a MAPS agent:
- 1 = IGU
- 2 = buffer
- 3 = TG
- 4 = DYNOPT
- 5 = FPG
- 6 = Output from the MAPS system
- 7 = Processing
- 8 = Supply
- 9 = LAMI

The individual locations in the MAPS system through which the lites pass are so-called locations (`Maps_Locations`). For the definition, it is recommended that the `Locationld` be assigned the corresponding number of the associated registration point. However, this is not obligatory. Optionally, a location is assigned to a MZO machine. This is not necessary for output and sorters.
A MAPS locations is always assigned to an agent. Several locations can be assigned to the same agent. Locations are grouped (`Maps_LocationGroups`). A MAPS location 0 ("somewhere") always has to exist.
A location has a type (`LocationKind`) that consists of a combination of the following values:
- **0 = None**
  The location can have inputs and outputs. No processing is conducted in this location. Example: a Sortjet for which there is no processing in the BOM or an output for which you want to generate an individual ticket.
- **1 = Machine**
  This location can have inputs and outputs. A processing is carried out. Location 0 (Somewhere) is an exception here). Example: a grinding machine, the grinding processing for this machine is in the BOM.
- **2 = Source**
  This location is a source, there is no connection to this location. Example: cutting or goods receipt.
- **4 = Input**
  This location can receive tickets from Location 0 (Somewhere). Example: a ticket runs via this location, but has no direct connection. The prerequisite is that the location before it also have an output to Location 0.
- **8 = Output**
  This location can send tickets to the Location 0 (Somewhere). Example: a machine has a manual output that is used if no other route is valid.

Example: a cutting table with a manual output has the type 11: 1 (processing cutting in BOM) + 2 (it is a generating processing) + 8 (manual output).

To connect the locations and define routes through the MAPS system accordingly, there are the hops (`Maps_Hops`). A hop is a connection between 2 locations. It can be defined on a hop whether the planned sequence of the lites is inverted if it goes over the hop (field `Sorting = 1`). This setting is evaluated on a hop that refers to an end location. This is necessary, e.g. on an output on the system that stores on A-racks. The sequence in both locations is inverted in this case.
For communication with the clients, there are the brokers (`Maps_Brokers`). Each broker is assigned to an agent, an agent can belong to only one broker. There is a 1:1 relation here.
Last but not least, we need the configuration of the various clients (`Maps_ClientConfigurations`). A SmartFactory client is assigned to a broker. Several clients can be assigned to the same broker. A client has a registration point, a PDC person barcode, and a PDC `Stationld` with which it can trigger PDC bookings. Optionally there is a `Stationld` for optimizations, this is important for the DYNOPT clients.
The name of the client is unique. If a client starts, it logs into the MAPS service with its name.
The SmartFactory navigator is also a client, but it has no configuration here.

### 2.3 MAPS service
The MAPS service resides in the CIM domain (CIM.Maps) and is installed with an individual diskset. Preferably on a ProcessServer on which the other services of the related domains were installed.

### 2.4 Clarity Suite
To use the Smart Factory interfaces, the Clarity Suite has to be installed, and also the Smart Factory AddOn. The following disk sets are required:
- A+W Clarity Suite
- A+W Clarity Suite Maps

After the installation, the Clarity Suite has to be started again in order to create the configuration files automatically. These are in our directory: `%APPDATA%\A+W\AWSuite\`

In the `Settings.xml` created in the directory, the Maps module has to be activated in order to integrate the Smart Factory interfaces.
**Figure 2-1 Configuration Settings.xml for Clarity Suite**
```xml
<?xml version="1.0" encoding="utf-8"?>
<settings>
  <application theme="Fluent" culture="de-DE" />
  <modules>
    <module>Maps</module>
  </modules>
</settings>
```

### 2.5 Shopfloor Clients
The Smart Factory clients are console applications that are installed via the A+W Clarity MAPS diskset. Installation is in the directory `C:\Program Files (x86)\A+W\Clarity\Maps\Shopfloor Clients\`.
There has to be a connection to the AWSOA infrastructure so that the MAPS service can be addressed. The client is called via `Maps.Shopfloor.Client.exe` with the name of the client from the configuration of the master data (table `Maps_ClientConfigurationa`). Which tasks the client should take over is controlled in the master data via the field `Maps_ClientConfigurations.ControlTyeName`.
In addition, some client types require an XML configuration file that is provided via the second parameter. Other necessary settings are stored in this configuration file.
It is recommended that you store these configuration files and the links to the call of the individual clients on the TRANS drive under a directory MAPS.

Example BAT file for call of a client:
```bat
C:
CD "C:\Program Files (x86)\A+W\Clarity\Maps\Shopfloor Clients\"
START Maps.Shopfloor.Client.exe "MyClient" \\AWPFileServer\trans\Maps\MyClient.xml
```
So that a DOS box doesn't just hang during operation, you have to switch off the "Quick Edit" mode. If this is not the case, a DOS box hangs if you click in it. You can see this from the title of the DOS box, where you will see the word "Selection" in front of the name. To come out of the mode, you have to press "Enter" in the box once.

**Figure 2-2 Quick-Edit mode in DOS box**
In the properties of the console window, under the "Options" tab, ensure that "Quick Edit Mode" is unchecked.

#### 2.5.1 Dynopt Filler Client
The DynOpt client has to be installed in an environment with an ODBC data source for A+W Production. The data source has to have the name that is stored in the AWSOA configuration.
In the DYNOPT environment, the new clusters are written to the DYNOPT system via the client. As soon as this has happened, the DYNOPT is executed as usual via the A+W Realtime Optimizer (prerequisite for this is a completely configured DYNOPT).
In the PANORAMA model of the DYNOPT, the MAPS service has to be called in order to set the status of the lite accordingly to "produced" during production; for this, the PANORAMA model needs the GUID of the DYNOPT client.
The Dynopt Filler client needs an XML file for the configuration:
`<DynOptFiller>`
- **DefectBarcode**: Status barcode for defect booking; if not set, barcode 500000020 is used. Defect bookings are made for lites that cannot be reported broken in the SmartFactory during validation of the SmartFactory with the breakage pool.
- **NumberOfOutputLines**: Number of output lines in Dynopt. The value is equal to the value of `NumberIGLines` from the section `[Panoprama]` in the `xopton.cfg`.
- **DynoptCuttingTables**: Dynopt tables. The tables' names can be taken from `xopton.cfg`, e.g. `TB1,TB2`.
- **SorterId**: ID of the sorter in the A+W StockService for which DYNOPT should reserve lites. The client determines the possible virtual buffers and forwards this information to DYNOPT.
- **SplitClusterByGroupkey** (bool, default: false): `false`: do not split cluster by the tickets's groupkey, `true`: split cluster by the ticket's groupkey.
- **<OutputLine>**: Output configuration
  - **Id**: Output's Id.
  - **DynoptIGLinie**: DynoptIGLinie number from the `Xopton.cfg`.
  - **FinalLocation**: Final Ticket Location Id in SmartFactory, e.g. Unload SJ2.
  - **FinalLocationName**: Name of the Final Ticket location.
  - **<PrimaryBufferSegment>**: Primary buffer segment for the output. The selection of the primary buffer segment corresponds to the production efficiency. Example: the output line is in the area of buffer segment 2. Then `PrimaryBufferSegment ="2"`.
  - **<Name>**: Output's name. Not currently used.
  - **<OutputLineType>**: The output type can be 0 (harp rack) or 1 (IG line). The value of the `OutputLineType` has to be equal to the value of `OutputType` from the section `[Panorama]` in the `xopton.cfg`. Important: if in the `xopton.cfg` the `OutputType` for the output is not set, the RTO uses the default value 0. In this case, `OutputLineType=0`.
  - **<BufferSegments></BufferSegments>**: Permitted buffer segments for this output.
  - **<AvoidBufferSegments></AvoidBufferSegments>**: Buffer segments to be avoided for this output. Here the buffer segments are listed, which may only be used if the lites do not fit the other buffer segments due to their dimensions.
- **TimeHorizonMinutes**: Defines the time horizon in minutes. Default value is 480 minutes. To deactivate this function, set the switch to 0.
- **BacklogEfficiency**: Defines the efficiency for how a backlog can be cleared. Is required in order to calculate the time for the backlog for the time horizon. Default value is 1, means 100%.
  - 0.5 means 50%: for one hour's work on the backlog, 2 hours are required to clear it.
  - 1.5 means 150%: for one hour's work on the backlog, 30 minutes are required to clear it.

**Example: Xopton.cfg**
```ini
[PANORAMA]
NumberlGLines=2
OutputType1=1
OutputType2=0
```

**XML file example:**
```xml
<DynOptFiller NumberOfOutputLines="2" DefectBarcode="500000020">
  <DynoptCuttingTables>TB1,TB2</DynoptCuttingTables>
  <SorterId>1</SorterId>
  <SplitClusterByGroupkey>false</SplitClusterByGroupkey>
  <OutputLine Id="1" DyoptIGLine="1" FinalLocation="119" PrimaryBufferSegment="2" FinalLocationName="ABockWand SJ1" OutputLineType="1" ItemsPerBufferSlot="1">
    <BufferSegments>2</BufferSegments>
    <BufferSegments>3</BufferSegments>
    <BufferSegments>4</BufferSegments>
    <AvoidBufferSegments>4</AvoidBufferSegments>
  </OutputLine>
  <OutputLine Id="2" DyoptIGLine="2" FinalLocation="1319" PrimaryBufferSegment="1" FinalLocationName="AbockWand SJ2" OutputLineType="1" ItemsPerBufferSlot="1">
    <BufferSegments>1</BufferSegments>
    <BufferSegments>3</BufferSegments>
    <BufferSegments>2</BufferSegments>
    <BufferSegments>4</BufferSegments>
    <AvoidBufferSegments>4</AvoidBufferSegments>
  </OutputLine>
</DynOptFiller>
```

#### 2.5.2 HEGLA Sortjet Client
The Sortjet Client is controlled via `Maps_ClientConfiguration.ControlTyeName=MachineControlHeglaSorter`. The map of the HEGLA Sortjet is stored in the A+W StockService. For this, the Id has to be stored in the master data of the sorter (`Maps_Sorters.StockServiceld`) under which the StockService manages this Sortjet.
The client also needs another XML file for the configuration in which the connection information for HEGLA MMI is set.
Tag `<Sorter>`:
- **<Ip>**: IP address on which the HEGLA MMI is running
- **<Port>**: Port via which the client communicates with the MMI
- **<Interface>**: Version of the HEGLA interface
- **<ClientId>**: ID of the HEGLA client that is provided during LOGON
- **<DummyMode>**: In this mode the client works with an internal dummy instead of the correct HEGLA MMI. This is no simulation and the IP has to be 127.0.0.1 here.
- **<TimeOutInSeconds>**: Timeout for the connection to HEGLA in seconds.
- **<Station>**: There can be several stations configured in that `<Station>` is entered several times, one after another. This switch has the following attributes:
  - **Id**: Number of the Hegla station
  - **Type** (InputStation; OutputStation; PhysicalStorage; VirtualStorage): The type of station.
  - **Locationld**: The MAPS Location ID of the MAPS tickets on this input, output or the sorter itself. Using the location ID, the client detects which station should be sent to HEGLA.
  - **Description**: Optional: a description of the station.
  - **ManualStation** (True or False; default=false): Relevant for OutputStation; if True, then this is a manual station where the removal of a lite has to be acknowledged by the user, which causes a ManualSheetRemove Meldung from HEGLA to the client. This doesn't happen with automatic stations.
  - **NextRegistrationPoint**: Optional switch via the PDC registration point to the next station. Is relevant for OutputStation. If set, a PDC booking is made on this station as soon as the lite has reached the HEGLA output station.
  - **SetBatchld** (True or False; default=False): If set, when filling the OutputSequence on the HEGLA is also sent the telegram SetBatchld. For this, data (e.g. from a furnace bed optimization) has to be present.
  - **StockServiceMapping**: Optional; if the ID of a virtual or physical buffer does not fit the ID in the A+W StockService, then the ID from the StockService has to be entered here. If the parameter does not exist, it is assumed that both IDs are identical.
  - **SortingMode**: Optional; mode that determines the sequence for the input or OutputSequence. Possible values:
    - **CurrentTime** (Standard), sorted by the time stamp how the lites came to the station
    - **FurnaceOptimization** uses the result of a furnace optimization that for OutputSequence happened afterward or for InputSequence before. Only the first lite of the optimization is used.
  - **SlotReservation**: Is required for an OutputStation and describes the mode that should be used for a reservation:
    - **Single** (default), one lite per slot
    - **AscendingSequence**, several lites in ascending order
    - **SwapTwo**, slots are filled in pairs. These have to be next to one another in their sequence.
    - **SwapTwoAndAscendingSequence**, slots are filled in pairs and in sequence, depending on what is better.
    - **SwapFour** this is like SwapTwo. The buffer slots are filled in groups of four lites and have to be next to one another in the output sequence. This can be used if according to the buffer it is possible to change the sequence and if the lites can be exchanged during transport. Example: with presence of a wall with 4 slots on the output side.
  - **MaxSheetsPerSlot**: Default value=1; Maximum of lites in a slot. This is used for reservations in the "AscendingSequence" mode. Has no effect on other modes. If the value is 1, then the maximum of lites is ignored. If you only want to have one lite per slot, use the "single" mode.
  - **SlotReservationGroup**: Optional for an OutputStation. It describes how the lites to be reserved that the MAPS services gives the client should be grouped again. Generally lites of a group are stored together in a slot (exception with UnitCrossBatch mode). The sorting from the MAPS service is not changed in the process (as long as no supply lites are involved).
    - **None** (default), no further grouping
    - **Unit**, lites of a unit (after barcode of the parent part) are grouped
    - **Component**, the same lites of units are grouped (order, item, part number)
    - **Glass**, the lites of the same glass type are grouped (glass type and thickness)
    - **UnitIgnoreOrigin**, lites of a unit (after barcode of the parent part) are grouped, across batch limits. `Unit` mode considers the groups (batch rack), this mode does not. In addition, in this mode the origin of the lite (direct entry, e.g. supply or grinding and origin, e.g. cutting 1 or 2) is ignored. This mode may not be used if lites of a unit come from different inputs, which can overflow.
  - **SupplyStation** (True or False; default=False): This switch affects input stations. For a supply station, the Sortjet itself determines the quantity of work to be reserved and requests them from the supply client.
  - **MaxSlotsInUse** (Optional, default = 0): Currently, this switch is used for a supply station. This is the maximum number of slots that may be reserved for lites that are set via the supply input.
  - **InaccessibleVirtualBuffer** (Optional): A list of virtual buffers that cannot be reached from this station. This can be configured for input or output stations. Sheets that run via an input or output station are not reserved in the virtual buffer defined here.
  - **AssemblyStation** (Optional, True or False; default=False): This switch affects the content of the `GetSheetData` telegram of HEGLA. If the value is 'true', then for lites - that move through this station - the `IsoCount`, `IsoIndex`, and `IsoUnitLabel` are set in the telegram. Relevant for TG lites.
- **<OutputLineConfiguration>**: Several output lines can be configured in that `<OutputLineConfiguration>` is entered several times one after another. This switch has the following attributes:
  - **Id** - (int) Output Line Id
  - **FinalLocation** - (int) Final Location
  - **Name** - (string) Name of the output line
  - **<OutputFactorConfiguration>**: Several entries for the factors per output can be configured. The switch has two attributes:
    - **SheetsCount** - (int) the number of lites in SJ1 for the output
    - **Factor** - (int) the number in the range from 2.0 to 0
    - **Example**:
      ```xml
      <OutputLineConfiguration Id="1" FinalLocation="2011" Name="BSG">
        <OutputFactorConfiguration SheetsCount="0"   Factor="2.0" />
        <OutputFactorConfiguration SheetsCount="50"  Factor="1.5" />
        <OutputFactorConfiguration SheetsCount="130" Factor="0.6" />
        <OutputFactorConfiguration SheetsCount="200" Factor="0.3" />
        <OutputFactorConfiguration SheetsCount="400" Factor="0" />
      </OutputLineConfiguration>
      <OutputLineConfiguration Id="2" FinalLocation="1319" Name="ESG">
        <OutputFactorConfiguration SheetsCount="0"   Factor="2.0" />
        <OutputFactorConfiguration SheetsCount="50"  Factor="1.5" />
        <OutputFactorConfiguration SheetsCount="130" Factor="0.6" />
        <OutputFactorConfiguration SheetsCount="200" Factor="0.3" />
        <OutputFactorConfiguration SheetsCount="400" Factor="0" />
      </OutputLineConfiguration>
      ```
    The SJ client determines the number of lite N in the Sortjet for the output and compares this with the `SheetsCount` from the configuration. Among all `SheetsCount < N` the largest value of the `SheetsCount` is selected and the corresponding factor is used as output factor.

#### 2.5.3 North-Glass furnace client
The North-Glass furnace client is controlled via `Maps_ClientConfiguration.ControlTyeName = MachineControlNorthGlassFurnace`.
To execute a furnace optimization, the A+W OptimizationService is required. It must be configured appropriately so that a furnace optimization can also be executed. This includes an appropriately set `XOPT.CFG` and a `LABEL.SET` with the "BARCODE" field.
In order to request the lites of an optimization, a connection to the A+W StockService is required since previously the lites have to be reserved there for a sorter after the furnace.
Every furnace client is configured appropriately via an XML configuration. Here the FurnaceClient requests lites from an upstream Sortjet and transfer these after the furnace to a downstream Sortjet:
`<Furnace>`
- **MaxOptiPatterns** (integer, Default 3): Because for the furnace optimization only the first optimization pattern is used, it makes little sense to optimize a lot of lites at the same time. Only as many lites are optimized so that the maximum number of optimization patterns anticipated is not exceeded. The optimal value has to be determined empirically. If the parameter is not set, the default value=3 is used. The optimal value is in the range from 3 to 6.
- **Optimization**: True (default) / False. If true, then this furnace client will execute a furnace bed optimization on the available lites of the next glass type. The first bed of the result is reserved and the bed requested.
- **MoveBedInProduction**: True (default) / False. If true, then the client may move a furnace bed into the furnace.
- **MoveBedOutProduction**: True (default) / False. If true, then the client may set a furnace bed produced and move it out of the furnace.
- **<InputSorterId>**: ID of the sorter in the A+W StockService in front of the furnace for which the furnace requests lites.
- **<OutputSorterId>**: ID of the sorter in the A+W StockService behind the furnace for which the furnace should reserve lites.
- **<Port>**: Port under which the North Glass controller logs into the client.
- **<FurnaceBedWidth>**: Width of a furnace bed in millimeters.
- **<FurnaceBedHeight>**: Height of a furnace bed in millimeters.
- **<FurnaceBedDistanceBetweenSheets>**: Distance between the lites on the furnace bed in millimeters.
- **<TimeOutInSeconds>**: Timeout for the connection to North Glass in seconds.
- **<MoveBedOutTravereOrder>** (default Inverse): `Inverse`: move-out subplates are reserved in the reverse sequence. `Normal`: the subplates are reserved in the sequence that is defined by the optimization.
- **<FurnaceOptimizationMode>** (int, default=1): 1:Furnace optimization runs without logical buffer, 2: Furnace optimization runs with the simple process for the logical buffer.
- **<OutputSorterSheetsProSlots>** (int, default =1): 1: single assignment in the logical buffer, 2: two lites per slot in the logical buffer.

**Furnace recipes**
The furnace has different recipes for the glass processing. AWProduction and the furnace have different designations for the same processing types. The processing type for each lite is defined by AW Production and can be seen from the table `Maps_Tickets.LotType`. The `<ProcessingType>` tag makes a machine-specific code (Processld) that is defined by the machine manufacturer available to each LotType.
`<ProcessingType>` tag:
- **Processld** - (integer) Machine-specific code for the processing
- **FeinLotType** - (integer) Processing type according to AWProduction
- **ProcessingName** – (string) Processing description; no effect at the moment
- **JumboNr** - (integer, default=0) specifies the jumbo number for the process. Is used to change the furnace space dynamically. The furnace dimensions are defined in the table `xopt_jumbo`. For each value `JumboNr`, you can define several furnace dimensions depending on glass type and thickness. If `JumboNr` is not set or if there is no entry in `xopt_jumbo`, default furnace dimensions are used.

> **Important**: if the TG client gets a lite with the `FeinLotType` for which there is no `<ProcessingType>` configuration, the lite is not produced (the TG client does not know which `Processld` has to be sent to the machine).

**Outputs**
The furnace client has to recognize the outputs behind the next sorter in order to guarantee an even filling of the sorter for all outputs. For each output, there is one of the following tags.
`<FurnaceOutputLine>` tag:
- **Id** -(int) unique Id of the output
- **FinalLocation** –(int) The MAPS location to which the output leads
- **Name** - (string) A name of the output, is used for display
- **Type** - (int) Type of the output
  - 1 (RackOrdered)
  - 2 (LaufOrdered)

**PatternViewer**
Furnace bed optimization can be displayed in the PatternViewer controlled by the client. Here, both the ones in the furnace, the one before the furnace, and the furnace bed just optimized can be displayed. For display, an entry in the configuration is required for each station:
`<PatternViewerConfiguration>` tag:
- **ViewerName**: Name of the PatternViewer instance to be addressed, e.g.: "1#TB1#001"
- **ViewerType**: Describes which furnace bed should be displayed. Possible values are: `Optimization`, `Incoming`, `Outcoming`

#### 2.5.4 Sample XML file
There is a current sample configuration file in the installation directory under "Configuration".
```xml
<?xml version="1.0" encoding="utf-8" ?>
<ClientConfigurationExtension>
  <Sorter>
    <Ip>127.0.0.1</Ip>
    <Port>15000</Port>
    <Interface>SJ.4.1.0.4</Interface>
    <DummyMode>1</DummyMode>
    <ClientId>1</ClientId>
    <TimeOutInSeconds>180</TimeOutInSeconds>
    <Station Id="208" Type="InputStation" LocationId="999" Description="KSR">
      <InaccessibleVirtualBuffer>1</InaccessibleVirtualBuffer>
      <InaccessibleVirtualBuffer>3</InaccessibleVirtualBuffer>
    </Station>
    <Station Id="210" Type="InputStation" LocationId="410" Description="Benteler"/>
    <Station Id="212" Type="InputStation" LocationId="210" Description="Supply" SupplyStation="True" MaxSlotsInUse="20"/>
    <Station Id="1" Type="PhysicalStorage" LocationId="118" Description="S1" StockServiceMapping="1"/>
    <Station Id="2" Type="PhysicalStorage" LocationId="118" Description="S2" StockServiceMapping="2"/>
    <Station Id="214" Type="OutputStation" LocationId="119" Description="To Wall" ManualStation="True" NextRegistrationPoint="119" SlotReservation="AscendingSequence" SlotReservationGroup="Component"/>
    <Station Id="401" Type="OutputStation" LocationId="1310" SetBatchId="True" SortingMode="FurnaceOptimization"/>
    <Station Id="402" Type="OutputStation" LocationId="1510" AssemblyStation="True">
      <InaccessibleVirtualBuffer>1</InaccessibleVirtualBuffer>
    </Station>
    <Station Id="1" Type="VirtualStorage" LocationId="118" StockServiceMapping="1"/>
    <Station Id="2" Type="VirtualStorage" LocationId="118" StockServiceMapping="2"/>
    <Station Id="3" Type="VirtualStorage" LocationId="118" StockServiceMapping="3"/>
    <Station Id="4" Type="VirtualStorage" LocationId="118" StockServiceMapping="4"/>
  </Sorter>
  <Furnance Optimization="True" MoveBedInProduction="True" MoveBedOutProduction="True">
    <SorterId>2</SorterId>
    <Port>8888</Port>
    <FurnaceBedWidth>2850</FurnaceBedWidth>
    <FurnaceBedHeight>6000</FurnaceBedHeight>
    <FurnaceBedDistanceBetweenSheets>100</FurnaceBedDistanceBetweenSheets>
    <TimeOutInSeconds>180</TimeOutInSeconds>
    <PatternViewerConfiguration ViewerName="1#TB1#001" ViewerType="Incoming" />
  </Furnance>
</ClientConfigurationExtension>
```

### 2.6 Panorama Clients
MAPS can be integrated into Panorama scripts, e.g. in the A+W Realtime Optimizer with DYNOPT or in an A+W Production Terminal. There is also a Maps client that requires appropriate configuration.

### 2.7 Dynopt configuration Xopton.cfg
#### 2.7.1 Section [CutGo]
- **Import=2**
  If a batch has been imported successfully from the DynopFiller, DynoptFiller writes the value `300+Stationld` to `pool_lauf.cutgo_status`. If `Import=2`, Dynopt searches for newly imported batches and restarts the optimization.

## 3 The ticket system in the Smart Factory
A lite is unique in the MAPS system and with scheduling in the MAPS system, receives a ticket for each location it passes. The lite can be identified uniquely via the `SheetId`. The `SheetId` can be the BARCODE of a lite from the PPS system, but it does not have to be. Tickets are saved in the table `Maps_Tickets`.

### 3.1 The ticket status
A ticket has a status. With status between Committed and Finished, the tickets are in production (`Maps_Tickets.Status`):
- **0 = None**: No status assigned
- **1 = Raw**: Data for the ticket was collected, as planned in the PPS detailed scheduling
- **2 = Prepared**: The BOM information for the lite is assigned and made plausible.
- **5 = Scheduled**: MAPS production steps determined
- **8 = Confirmed**: MAPS production steps confirmed
- **10 = Committed**: Lite scheduled in the MAPS system
- **20 = TreatmentPossible**: All prerequisites for production fulfilled, if lite is ready, it can start
- **30 = ReadyForProduction**: Lite ready for production
- **35 = IncomingRequest**: Lite was requested for this step
- **40 = Incoming**: Lite moves into location
- **50 = InProduction**: Lite is being produced
- **60 = ProducedAndReadyForNextStep**: Lite has been produced and is ready for next ticket
- **65 = OutgoingRequest**: Lite was requested for the next step
- **70 = Outgoing**: Lite is being moved out
- **75 = ToCleanByClient**: Lite leaves the system (e.g. due to a break) and this ticket should be cleaned by a client (e.g. a Sortjet client deletes reservations on the machine)
- **80 = Finished**: Lite has run completely through this step
- **85 = CleanedByClient**: Ticket that should be cleaned by a client (status 75) was cleaned by a client.
- **90 = Broken**: Lite is broken
- **91 = Canceled**: Lite is canceled, no longer in the system
- **93 - Cleaned**: Ticket was cleaned by the MAPS Service, e.g. after a break. Cleaning by a client is not necessary.

### 3.2 The lite status
The information for a lite is saved in the table `Maps_GlassInstances`. Here there is a `SheetStatus` that applies for the whole lite, and thus to all tickets of the lite:
- **0 = None**: The lite has no status, it has not yet been initialized and it is thus not ready.
- **1 = Initialized**: Lite was initialized
- **2 = PreparedForProduction**: Lite is prepared for production, e.g. reservations on a SortJet were made.
- **3 = InProduction**: Lite is in production
- **4 = Somewhere**: The lite has left the MAPS system, it may come back
- **10 = Scrutiny**: The lite was taken out of production in order to be scrutinized, it can come back to production. Until then, it may not be produced further.
- **11 = Broken**: Lite is broken
- **20 = Cleaned**: Lite is in the status for cleaning. This process is asynchronous, it is cleaned if all tickets for the lite have the status Cleaned (93) or CleanedByClient (85)
- **21 = PreparedForRemake**: A broken lite is prepared for a remake. Here, e.g. the remake counter is incremented.
- **30 = RouteFound**: The lite has found a valid route through production.
- **80 = Finished**: The lite is finished and will no longer return to the MAPS system
- **90 = Canceled (not yet used)**: The lite is canceled and will no longer return to the MAPS system.

### 3.3 The validation status
If the ticket chain is displayed in our interfaces, normally the ticket status is not displayed directly, but rather the validation status. This is derived from the ticket status, but it also checks whether this status is OK. If, for example, a ticket has been hung for hours at the inlet of a machine, then a corresponding status is displayed that indicates the hanging of the lite.
- **1 = Unknown**: The list has a non-defined status on this ticket.
- **2 = Error**: The lite on this ticket has an error.
- **3 = Temporary**: The lite is only temporarily on this ticket. This is, for example, if the lite has been requested. This status remains only until the lite arrives.
- **4 = Planned**: The ticket for this lite is planned.
- **5 = InProduction**: The lite is in production
- **6 = Moving**: The lite on this ticket is moving.
- **7 = Produced**: The lite on this ticket is produced.
- **8 = Remake**: The lite is broken and the ticket for the lite is ready for a remake.
- **9 = Canceled**: The ticket for the lite was canceled.
- **10 = Delayed**: The ticket for the lite is behind the planned date.
- **11 = Stuck**: The lite is stuck in the ticket's station
- **12 Vanished**

### 3.4 ValidateAndExecuteSheetTask
With the `ValidateAndExecuteSheetTask` interface, a client can report a break or a remake to the MAPS service. For each request, the `TaskCode` has to be transferred, whereby currently not all of these are supported by the outside; some are not yet implemented and others have only an internal function.

**Figure 3-1 Lite movement in MAPS** (This figure shows a state diagram for lite statuses and transitions)

- **None = 0**: No action, lite "lives"
- **Validate = 1**: Checks the lite according to the options transferred by the client to see whether, e.g. a lite could be regular, a break or a remake
- **StartInvestigation = 10**: A lite is begun with an investigation and locked in the process for further processing
- **FinishInvestigation = 11**: The investigation was ended and the lite is set back to its old status
- **ReportBroken = 20**: Inquiry can come from all clients in order to react to a breakage report
- **Cleanup = 30**: Lite is in the cleaning of its data, whereby various clients are instructed to cleanse their data (e.g. to delete reservations in a Sortjet)
- **PrepareRemake = 40**: Prepares a lite in order to be used again as remake. Here, e.g. the remake counter is incremented.
- **DetermineProductionRoute = 50**: A route through production is found. Can be the old route for a remake.
- **PrepareForProduction = 70**: Prepares the lite for production, lite was not yet started in production, but may be reserved for machines.
- **FinishProduction = 80**: Lite is definitely finished and out of the MAPS system. It cannot be retrieved

Currently the server supports a `ReportBroken` and a `PrepareRemake`.
With the `TaskCode` options are also transferred that consist of a combination of the following `TaskOption`.
- **None = 0**: No additional options, the task will be processed asynchronously. Errors in the validation cause the whole task not to be executed.
- **Synchronous = 1**: The task will be executed synchronously, return if result is present. This option is currently not implemented.
- **OverrideErrors = 2**: If this option is active, lites in the task that have no errors in the validation are also executed if there are lites with validation errors in the task.

In addition to the `TaskCode` and the `TaskOption` a list of the lites to be processed is transferred. Here the lite is recognized by its `Sheetld`. In addition, a time stamp of a break can be transferred and a combination of the following options:
- **None = 0**: No special option is used
- **IsBroken = 4**: The client identifies this lite as broken
- **IsRemake = 8**: The client identifies the lite as a remake. In contrast to a lite that appears for the first time.
- **IsCanceled = 16**: The client identifies the lite as cancellation; this lite is no longer needed. This option is not yet implemented.

The function returns a return value for each lite transferred. This is either `0` (None) if everything is good, `1` (Pending) if the lite is still in processing (e.g. in `CleanUp`) or a value greater than 1, which is then an error code.

**Examples:**
- `SheetStatus 3` → `TaskCode 20, SheetOption 4` = Result 0 / 1
- `SheetStatus 0` → `TaskCode 20, SheetOption 4` = Result > 1
- `SheetStatus 20` → `TaskCode 40, SheetOption 8` = Result 0 / 1
- `SheetStatus 3` → `TaskCode 40, SheetOption 8` = Result > 1
- `SheetStatus 3` → `TaskCode 40, SheetOption 4+8` = Result 0 / 1

### 3.5 Ticket flow in production
If a lite is in production, you can see from the status of the individual tickets in which state the lite is in production. The status of the individual tickets is incremented here. The sequence of the tickets of a lite describes its path through production.
There are a few coupled ticket stati that have an effect on the status of the predecessor or successor ticket. The following coupling affects tickets of a ticket chain in a section (DIVE):
- Predecessor: `ProducedAndReadyForNextStep` → Successor `ReadyForProduction`
- Predecessor: `OutgoingRequest` → Successor `IncomingRequest`
- Predecessor: `Outgoing` → Successor `Incoming`
- Successor: `IncomingRequest` → Predecessor: `OutgoingRequest`
- Successor: `Incoming` → Predecessor: `Outgoing`
- Successor: `InProduction` → Predecessor: `Finished`

If a lite from the SmartFactory is ejected via an UNLOAD station and it should later be put into the SmartFactory via a SUPPLY station, this coupling does not apply between the two tickets of the two sections. If a client ejects a lite, it has to inform the SmartFactory of this (MAPS Interface `ProgressLeft`). In this case the ticket is set to `Finished`, the successor (SUPPLY) to `TreatmentPossible`.

## 4 HEGLA Sortjet
If a HEGLA SortJet is activated, the appropriate ShopFloor client for this is required. The client receives the lites via the MAPS service that are in range. Here the client communicates with the A+W StockService in order to control the HEGLA SortJet and with HEGLA around the SortJet.
In the A+W StockService the current assignment of the StockService is saved, in the process reservations are included. In addition, for each input and each output on the SortJet, a corresponding list is managed, which describes which lite is precisely where at the moment.
If the connection to HEGLA is re-established (e.g. due to the restart of our client), they synchronize both systems. HEGLA inquires with us in which state the system is and reports to us the outgoing movements since the dropping of the connection. If something isn't right, the worker has to make the appropriate decisions via the HEGLA terminal in order to restore a current state.

### 4.1 Reservations for transport in and out
A lite that should be moved into a Sortjet first has to be reserved in the SortJet. This is normally done by a client in front of the SortJet (e.g. Panorama in the RTO before cutting of a stockplate). If there is no reservation, HEGLA does not recognize the lite and it can thus also not be moved into the SortJet. A reservation is made via a virtual HEGLA buffer, not the physical HEGLA buffer.
If a lite should be moved from the SortJet, the slot for transport out has to be locked. This is requested by a client behind the SortJet. In the process, all lites of a slot are set in the A+W StockService to an appropriate status. This means that no more reservations can be added in this slot. The locking for transport out is only possible if there are no open reservations for the slot in question.
During transport out, not all lites of a slot have to be requested; one is enough. The slot is locked completely. Lites have to be requested in the sequence in which they are in the slot since the HEGLA system has no possibility to exchange the lites at will during transport out.
If several lites may be in a slot, this has to be set for each output in the configuration in the client. Regardless of this, the client does not mix any SmartFactory groups and no lites that come from different inputs or should go to different outputs.

### 4.2 Moving lites into and out of the SortJet
If a lite is ready to move into the SortJet, this lite is written by the client to HEGLA to the input list (`AppendInputSequence` telegram).
When moving a lite out of the SortJet, the client writes the lite to HEGLA in an output list (`AppendOutputSequence` telegram).
If lites are in the lists, these lites are moved in sequence by HEGLA. HEGLA reports each movement to the client (`GlassPosition` telegram). The client saves the movements in the A+W StockService. Here, a station, slot, and time stamp are always transferred. The station is the physical component where the lite is currently located (e.g. a shuttle), the slot can be important, for example, for a shuttle with several slots.
If a lite moves into the Sorjet, the same message (`GlassPosition` telegram) is sent, the station is the physical buffer and the slot is the slot in the physical buffer. The client recognizes from the station from its configuration that this is the Sortjet itself and it reports this to the A+W StockService. In this case, the A+W StockService removes the lite from the input line and changes the reservation to a confirmation.
When moving out of the SortJet, the lite remains in the A+W StockService until the HEGLA reports the first lite movement (`GlassPosition` telegram).
A lite is moved completely out of a SortJet until the last message (`GlassPosition` telegram) comes with the HEGLA station of the output or until HEGLA sends a manual confirmation (`ManuelSheetRemove` telegram). What precisely is correct has to be configured for each output on the client.

Adding to an inlet list is something the client does automatically if its ticket is set to the state `ReadyForProduction`. The ticket status is set automatically to `Incoming` as soon as the lite was written to the input list.
To reach the state `ReadyForProduction`, the previous ticket has to be set to `ProducedAndReadyForNextStep`. In case of several tickets with status `ReadyForProdction`, the time stamp when the status is set decides about the sequence in the input list.
To get a lite in an output list, the ticket has to be set to the status `OutgoingRequest`. When writing, the status does not change in the output line. This happens only if HEGLA moves the lite and moves out (`GlassPosition` telegram). Then the status of the ticket is set to `Outgoing`.
In order to reach the state `OutgoingRequest`, the following ticket has to be set to `IncomingRequest`. In case of several tickets with status `OutgoingRequest`, the time stamp when the status is set decides about the sequence in the output list.

If a whole furnace bed is written to the input or output line, previously the furnace bed and its assignment is reported to HEGLA (`SetBatchld` telegram). Here, an ID of the furnace bed (Batchld), a 16-digit character string (created from the GUID of the optimization) is also transferred. Using this, HEGLA communicates later directly with the furnace and it with us, in order to identify the furnace bed in question. The client determines the assignment of furnace beds with a GUID via the A+W OptiService.

## 5 Control of North-Glass furnace
For the furnace activation, divided into 4 function blocks. These can be obtained in a Maps ShopFloor client. It is recommended that you control it via 3 different clients.
Each of the function blocks has its own A+W PatternViewer in order to display the furnace bed in question.

### 5.1 NorthGlass communication
Communication with the NorthGlass furnace is a function block. If several clients should control the furnace, only one may handle the communication with the furnace. Here it is recommended that you use the client that also executes the optimization. In the other clients, set the port for communication to 0 in the XML configuration.
If there is communication with NorthGlass in the client, this will be displayed accordingly.
If no communication can be established, you should check whether the firewall is locking the port for communication.
So that a furnace bed moves into the furnace, NorthGlass receives a signal from HEGLA that the next furnace bed is complete and can be moved in. The signal includes the 16-digit Batchld of the furnace, which we previously reported to HEGLA. With this Batchld, NorthGlass asks the client about the composition of the furnace bed. This information is required so that NorthGlass can find the correct recipe.
Additional information from NorthGlass is the moving in of a furnace bed and the breakage reporting of a whole furnace bed. Currently the breakage reporting is not supported due to technical problems at NorthGlass. Lites have to be reported broken individually at the output.

### 5.2 Furnace optimization
Furnace beds are moved into the furnace; beforehand, these have to be optimized via the furnace optimization. A furnace optimization is possible if there are lites ready (in the HEGLA SortJet to move out for the furnace output) and the last furnace bed requested has begun to move to the furnace. In the process, several furnace beds can be under construction in front of the furnace.

**Figure 5-1 Starting furnace optimization** (Screenshot of a console client showing furnace bed status and prompting to execute the next furnace optimization).

If lites are being optimized, then the first furnace bed of the optimization is used, the rest are discarded. There is an attempt to reserve the lites on this bed. So that a reservation works, the corresponding ShopFloor client on the HEGLA Sortjet has to run behind the furnace. After 10 attempts, the optimization is cancelled and there can be a re-optimization. The client determines the virtual buffer for the lites to be reserved using the data from the StockService.
If the reservation was successful, the tickets of the furnace bed are regrouped on the furnace. The group key is the GUID under which the optimization is stored in the OptimizationService. Using the grouping, you can recognize a furnace bed.
After the grouping, the furnace bed is requested, in that the status of the tickets is set to `IncomingRequest`; the consequence of this is that the coupled status of the predecessor (ticket on the HEGLA SortJet in front of the furnace) is set to `OutgoingRequest`.
As long as a furnace bed exists where all tickets have the status `IncomingRequest`, no further optimization is started. If a lite of the furnace bed has the status `incoming`, another optimization can be started. A lite gets the status `Incoming` if the ticket is set on the HEGLA Sortjet to status `Outgoing`. This happens as soon as HEGLA moves out one of the lites from the Sortjet and it is reported on the ShopFloorClient on the Sortjet.
The current furnace bed of the optimization can be displayed on a PatternViewer. A furnace bed is identified via a unique 16-digit `Batchld`. This `Batchld` is determined from the GUID of the furnace bed (not the GUID of the optimization!) and is saved on the ticket in the `CurrentLocation` field for queries.

**Figure 5-2 Result of a furnace optimization in the PatternViewer** (Screenshot of the A+W PatternViewer showing the optimized layout of glass lites on a furnace bed).

### 5.3 Moving furnace beds in and out of the furnace
Additional functions are moving a furnace bed in and out of the furnace.
You confirm the moving in or out manually in a client. Reporting happens either in the client or in the connected PatternViewer.
Moving in can come automatically via the communication from the NorthGlass furnace. If you want to report a break, this has to happen before the NorthGlass report.

**Without PatternViewer**
If you are not using a PatternViewer, the current furnace bed is displayed in the client and the tickets are set to status `InProduction` with confirmation with the Y key. To update the display, another key can be pressed.
**Figure 5-3 ShopFloor client in front of the furnace without PatternViewer** (Screenshot of the console client).

**With PatternViewer**
If a PatternViewer is used, then the current furnace bed there is displayed. You can mark lites broken. The furnace bed is confirmed in that you press the right arrow to continue.
**Figure 5-4 ShopFloor Client in front of the furnace with PatternViewer** (Screenshot of the console client).
**Figure 5-5 PatternViewer in front of the furnace** (Screenshot of the A+W PatternViewer showing the incoming furnace bed layout).

### 5.4 Determining the size of the furnace bed dynamically
The size of a furnace bed is determined via the XML configuration. If you want to use different furnace bed sizes for different TG articles, this can be done via the A+W Production master data.
For a TG article, a glass article and a stock dimension have to be created in the master data. This is normally not required.
The shape trim in the glass article describes the (minimum) distance between two lites. The trim of the glass articles can describe an additional edge of the furnace bed.

**Figure 5-6 Glass article master data for managing furnace beds** (Screenshot of A+W Production master data screen for glass articles).

Via the stock dimension management, various dimensions of furnace beds can be created for a glass type. Each stock dimension HAS to be assigned to a table. Here, the manual cutting is selected.
The usable dimensions of the furnace bed are managed in:
- **Width**: corresponds to the furnace bed length
- **Height**: corresponds to the furnace bed width

**Figure 5-7 Stock dimension master data for managing furnace beds** (Screenshot of A+W Production master data screen for stock dimensions).

The key field `Lagermass-Nr` serves to provide various restriction records. Whether for different processing types or different furnaces. The assignment is made in the XML configuration of the client.
Processing types for tempering:
- 1500 - Tempering
- 1505 - Marine glass
- 1510 - Partial tempering

**Example of XML configuration of the client:**
```xml
<ClientConfigurationExtension>
  <Furnance Optimization="True" ...>
    <ProcessingType ProcessId="1" JumboNr="1500" FeinLosTyp="1500" ProcessingName="ESG" />
    <ProcessingType ProcessId="2" JumboNr="1510" FeinLosTyp="1510" ProcessingName="TVG" />
    <ProcessingType ProcessId="4" JumboNr="1505" FeinLosTyp="1505" ProcessingName="Marine" />
  </Furnance>
</ClientConfigurationExtension>
```

## 6 Assembling units with the SmartFactory
To assemble lites, special things have to be considered so that the right lites are assembled in the right order.
There is a sorting system before a LAMI, FPG or IG line. If the slots of the sorting system can be assigned multiple times, the output to the lines has to be configured so that a unit can be stored together. This means that only lites for a single unit are in a slot.
The units are produced in the sequence from the detailed scheduling; in the SmartFactory, this is the sequence of the parents of the individual lites. When calling up to the line, this sequence is considered during removal.
The sequence for how the individual lites are moved on the line is determined from the detailed scheduling. Here it is absolutely necessary that the individual lites of a unit are in the usage batches on a harp rack. The sequence corresponds to the sequence of the slot numbers. So that this is achieved, the harp rack has to be of the mode "together" in the detailed scheduling. With this mode and the function of the `AUSGANGSNR`, you can determine the sequence of the individual lites in the detailed scheduling. Another mode, e.g. "compact," is not permitted here.

## 7 Diving through the SmartFactory
In production, it can happen that a lite passed through the same station several times. A prominent example of this would be multiple screen printing.
More relevant in the SmartFactory are lites that leave the SmartFactory in order to be processed outside of the SmartFactory and then inserted back into the SmartFactory.
**Example**: We have filled a sorter from cutting and from it, a furnace is fed. Now lites are in the sorter, which receive a processing that is done outside of the SmartFactory before the hardening. Thus the lites do not initially move into the furnace; instead, they are moved out of the sorter and moved back into the sorter after the processing. As soon as the lite is in the sorter for the second time, it can now be moved into the furnace. After the furnace, the lite should be installed in a LAMI. Since the LAMI line is filled via the sorter, the lite has to be moved back into the sorter. The lite thus passes through the sorter station three times.
So that the SmartFactory can distinguish the sections of a lite, the ticket chain is subdivided into partial sections. The boundary of a segment is always a supply input into the SmartFactory. As soon as this limit has been passed, the lite is in the new section.
The lite from the example has the following ticket chain:
`CUT → GRIND → SORTER → UNLOAD SORTER → SUPPLY → SORTER → FURNACE → UNLOAD FURNACE → SUPPLY → SORTER → LAMI`
This chain is divided into 2 sections:
- Section 2: `CUT → GRIND → SORTER → UNLOAD SORTER`
- Section 1: `SUPPLY → SORTER → FURNACE → UNLOAD FURNACE`
- Section 0: `SUPPLY → SORTER → LAMI`

The last section of a ticket chain always gets the number 0. The number of the section is then increased to the first ticket. This number is saved on the ticket in the database field `MAPS_TICKETS.DIVENUMBER`.
In order to detect in which section production is happening, the number of the current section is saved in the database field `MAPS_GLASSINSTANCES.ACTUALDIVE`.
With the transfer from the SmartFactory via an unload ticket in the SmartFactory via a supply ticket, the client has to communicate at the unload of the SmartFactory that it has now "let the lite go." If this happens, the status of the supply ticket is set to `TreatmentPossible` (20) and the current section is reduced by one.
If the sorter client now asks the SmartFactory for this lite, then it receives the data of the ticket of the current section.

## 8 Breakage in the SmartFactory
Breaks in the SmartFactory have to be reported to the A+W Production PDC by the triggering client if they should go into the breakage pool there. The SmartFactory itself does not do this automatically. The ShopFloor clients have a connection to the PDC and book breakage accordingly.

If a breakage message is triggered in the SmartFactory, the tickets have to be cleaned up. The `SheetStatus` of the lite is set to `20 Cleaned`. The tickets that can be cleaned up by the MAPS Service directly get the status `93 Cleaned`. Tickets that have to be cleaned up by a client get the status `75 ToBeCleanedbyClient`. The affected client has to process these tickets and if successful, the ticket gets the status `85 CleanedByClient`.
Currently, this only affects the Sortjet clients since these have to clean up any existing reservations.

If a remake tries to produce, a cleaned-up lite can be brought back to life if all tickets have the status 85 or 93.
So that the client responsible for cutting the remake knows whether a remake is OK or not, it has to query the service before cutting. For this purpose, there is the function `ValidateRemakes` in the Query-Interface. Only if this gives the OK can a remake be produced.

### 8.1 Validation of the remake pool
It can happen that remakes try to cut and this is not possible in the SmartFactory. If this happens, the remakes are not cut, they disappear or the system stops. There are different causes for this problem. One of the causes is that a lite was reported broken outside of the SmartFactory, but the SmartFactory still has access to this lite. The lite might be still being processed by a machine or be in a SortJet. The SmartFactory cannot know where the lite actually is if nobody tells it this. It can happen that a lite is missing and you don't know where it is and it has simply been reported broken. Now, according to the SmartFactory, it is still in a SortJet. Then you have to check whether this is really the case and if so, either ignore the break and continue producing the lite or remove the lite and then report it broken to the SmartFactory. If the lite is still supposedly being processed on a machine, then you also have to check there whether this is the case. If there was a machine breakdown and the lite was simply removed from the machine without telling the SmartFactory about this, then the message has to be repeated.

So that these problematic cases are detected, lites that are in the breakage pool should not simply be re-optimized. Beforehand, there should be a validation by the SmartFactory. This is currently done with the Dynopt Filler Client. It asks the MAPS Service to do this validation every 5 minutes. For this, it queries the current breakage pool with all non-validated lites. The result of the validation can be that the lite has no relevance for the Smart factory; that the lite can be re-cut in the SmartFactory; or that it cannot be re-cut.

The result is reported back to the breakage pool and to the controlling client (Dynopt Filler). The client triggers a defect booking for the problem lites in the PDC. The status barcode for the defect booking can be set via the XML configuration file of the DYNOPT Filler Client:
```xml
<DynOptFiller DefectBarcode="500000020">
```

Lites in the breakage pool (`FEIN_TEILE.JOB = 10000`) have after inserting in the field `FEIN_TEILE.MASCHINE2` the value 0. After the validation, the value for possible remakes >= 100000 (100000 + MASCHINE1) and for the problem lites the value is set to -1.
The A+W Realtime Optimizer has to be configured so that it only uses broken lites from the breakage pool whose value for `FEIN_TEILE.MASCHINE2 >= 100000`. For this, the `XOPTON.CFG` in a DYNΟΡΤ operation has to be adjusted as follows:
```ini
[CutGo]
BreakageMode=3
BreakageSelection=N
BDEBreakageSelection=Y
InsertBreakageFeinteileRecord=N
```
In addition, the MZO ID of the permitted cutting table has to be stored in the following comma-separated list since only broken lites of these tables are used.
```ini
[BrokenSheetPool]
MZOPhysId=110,120
```
So that rejected lites are detected, the field `FEIN_TEILE.MASCHINE2` in the breakage pool (Designer Technik) are visualized accordingly.

The entire breakage pool is validated with each run. If the problem with a rejected lite has been solved in the meantime, the next validation will now accept this still-rejected remake.

> **Attention!**
> Updating of the data records in the breakage pool is done by the `Planning.Detailed` Service, which uses the database field `FEIN_TEILE.LASTMODZEIT` for its write operations.
> Since the SOA services only master the versioning to the millisecond, most time stamps in our Informix database are created for 10ns precision, under some circumstances there may be `ObjectStateExceptions` when writing the results.
> When updating the data, the program determines technically correctly but practically completely unusably that the time stamp in the database deviates from the own time stamp and 'someone has probably changed the record in the meantime'.
> To prevent this, the time stamp has to be adjusted to INFORMIX databases and in case of doubt, corrected manually.
```sql
ALTER TABLE fein_teile MODIFY (lastmodzeit DATETIME YEAR TO FRACTION(3) DEFAULT CURRENT NOT NULL);
```

## 9 Structure of the timeline
The timeline in the SmartFactory corresponds to the sequence of how batches were transferred to the SmartFactory. A particularity are batches that have a rush flag (`POOL_LAUF.Prioritaet > 0`). These are arranged in the timeline so that they are begun immediately.
With the release of the batches and any accrued backlogs, a pipeline forms, which depending on the machine ties up capacity and has to be worked through before the machine is free for the next batches.

**Figure 9-1 Time horizon** (Diagram showing a backlog and a timeline of jobs entering the Smart Factory, including a rush job, constrained by a time horizon).

The time horizon describes how many batches can be planned in production. The size of the time horizon can be configured freely and represents a quantity of work in time. A next batch is only begun if its work quantity and pipeline fit in the time horizon.
In order to express that backlog and already-begun batches for the future cannot be processed with the same efficiency as planned, an efficiency can be specified for the processing. If the backlog can only be processed with an efficiency of 50%, then one hour work on the pipeline means 2 hours time occupied in the time horizon.

A batch that is larger than the maximum time horizon cannot be released for production and would (temporarily) block production. This effect can be eliminated with a last-minute extension of the TimeHorizon. In the medium term (end of 2021), it is planned to create possibilities for the easy shifting of batches on the timeline.

The DYNOPT Filler Client release batches to the SmartFactory according to this method.

## 10 User interface
### 10.1 Call dialogs
The call dialogs are opened via the Production Terminal on the stations in question:
If no data can be called up, you will see a message: "Keine Läufe zum Abruf bereit" (No batches ready for call).

#### 10.1.1 Status descriptions
Batch status is displayed in different colors; furthermore, the currently selected batch is highlighted.

**Status Color Legend:**

| Status | Description |
| :--- | :--- |
| **Complete** | All of the lites to be called up for the batch are present. |
| **Complete (without remakes)** | All missing lites are remakes. |
| **Not complete** | At least one non-remake lite is missing. |
| **Remake** | Part of the batch was called up and there is at least one remake in the lites yet to be called up. |
| **Call active** | The batch is being called. |

#### 10.1.2 General batch information

| Column | Description |
| :--- | :--- |
| **Production date** | The planned production date |
| **Supply** | Number of supply lites |
| **Status** | Status of the batch |
| **Batch** | Batch number |
| **Total** | Total number of lites |
| **Project** | Name for the orders from the project business |
| **Customer** | Name of the customer for the order |
| **Deliv. Date** | Date of delivery to the customer |

#### 10.1.3 Assembly
In the overview, the available batches are displayed sorted in ascending order by time stamp:

##### 10.1.3.1 LAMI
The data corresponds to the information described in general batch information.

##### 10.1.3.2 BSG TPS
The following data is displayed next to the general batch information:

| Column | Description |
| :--- | :--- |
| **Primer** | **Primer**: at least one lite in the batch receives a fire protection coating<br>**No Primer**: none of the lites in the batch is coated |
| **Filled corner** | **Automatic**: for all units included in the batch, the filled corner is set automatically<br>**Manual**: for at least one unit in the batch, the filled corner has to be set manually |

##### 10.1.3.3 Cancel
By default, batches with canceled lites/units are not displayed in Production Terminal or called up via the call dialog. Such lites can be recognized because after the call, they are still on the list and have lites in the buffer.

Furthermore, there is a trace entry per lite:
`| "Sheet 002599384 was cancelled and will not be requested "`

In order to call up batches with canceled lites/units, a setting on the Production Terminal menu is required:
- In the `Ansicht` (View) menu, select `Storno anzeigen` (Show cancellation).
- **The setting is not saved when you exit!**
- Furthermore, it is necessary to activate the options "Allow incomplete units" (`Erlaube unvollständige Einheiten`) and "Allow incomplete batches" (`Erlaube unvollständige Läufe`) on the Options menu.

Then the call can be made and the canceled lites are displayed in yellow. The lites can be moved from the buffer with "Produce" and have to be removed manually after that.

#### 10.1.4 Hegla A-rack wall
##### 10.1.4.1 WallOut 1/2
The following data is displayed next to the general batch information:

| Column | Description |
| :--- | :--- |
| **Following tool** | Next processing step/machine |

### 10.2 Supply dialogs
The dialogs for setting supply lites are opened via the Production Terminal on the stations in question:

#### 10.2.1 Supply SortJet 1/2
In the overview, the available batches are displayed sorted in ascending order by time stamp.

**The following statuses are possible:**

| Status | Description |
| :--- | :--- |
| **Reserved** | All supply lites are reserved and can be set via the PT interface. |
| **Not reserved** | In the batch, supply lites for setting in the SortJet can be reserved. |
| **Reservation is running** | The reservation in the Maps service is active. |
| **Cannot be reserved** | There are no reservable supply lites in the batch. |

Using the button with the arrow, the detail view of the lites missing in the batch can be opened. The view shows a summary and details of the supply sheets.

Only batches with the status "not reserved" can be transferred to the Maps service with a click on "set selected group". The dialog is then closed and can be opened again to check the status again. The status of the batch then changes to "Reservation running". A successfully reserved batch receives the status "reserved".

The associated supply lites are then visible in the Production Terminal and can be selected individually and set with "Produce".

## 11 PDC connection to the SmartFactory
There is not a SmartFactory client at every point. If at such a point the SmartFactory needs information about the progress, this can be done with the PDC in A+W Production.

Prerequisite for this is a ticket in this place. A registration point can be assigned an agent. If a lite is booked to this registration point via the PDC, then the SmartFactory will set the associated ticket to the ticket status `produced` if the status is less than and the lite is in the SmartFactory (not broken or outside it).

The registration point has to be entered in the `MAPS_Agents.RegistartionPointProduced` field and has to be greater than 0 in order to activate the function. This function may not be activated on an agent that depends directly on the automation and has a client that controls it. If this happens nevertheless, chaos may arise in the automation due to the PDC messages.

The PDC messages can be issued by all common tools; the booking service sends all messages to the SmartFactory, which then decides whether or not the message can be ignored. If the SmartFactory cannot be reached, this message is lost.

Other connections, e.g. breakage messages, are planned but not currently implemented.

## 12 Table of figures
- Figure 1-1 Informix configuration
- Figure 2-1 Configuration Settings.xml for Clarity Suite
- Figure 2-2 Quick-Edit mode in DOS box
- Figure 3-1 Lite movement in MAPS
- Figure 5-1 Starting furnace optimization
- Figure 5-2 Result of a furnace optimization in the PatternViewer
- Figure 5-3 ShopFloor client in front of the furnace without PatternViewer
- Figure 5-4 ShopFloor Client in front of the furnace with PatternViewer
- Figure 5-5 PatternViewer in front of the furnace
- Figure 5-6 Glass article master data for managing furnace beds
- Figure 5-7 Stock dimension master data for managing furnace beds
- Figure 9-1 Time horizon
