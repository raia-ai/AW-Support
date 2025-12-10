---
title: "EN INST A+W Smart Factory"
category: "installation"
product: "A+W Smart Factory"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Smart Factory"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions       Beta - A+W Clarity Smart Factory - Multistep      Automated Production    Change history:      Date            Author               Comments                                               Version      2019-03-21      DLA                  Document created                                        1.0      …               …                    …                                                       …      2021-01-18      MME                  "SwapFour" as new method"
source_file: "EN-INST-A+W Smart Factory.pdf"
---


# EN INST A+W Smart Factory

     Installation Instructions

     Beta - A+W Clarity Smart Factory - Multistep
     Automated Production
   Change history:
     Date            Author               Comments                                               Version
     2019-03-21      DLA                  Document created                                        1.0
     …               …                    …                                                       …
     2021-01-18      MME                  "SwapFour" as new method for buffer slot                2.30
                                          assignment
     2021-01-21      DLA                  Time horizon                                            2.31
     2021-02-09      MISC                 New sort mode for sorter                                2.32
     2021-02-19      MPH                  Supply Dialog BSG In                                    2.33
     2021-04-07      DLA                  Validation Status                                       2.34
     2021-04-09      DLA                  Clarity Suite                                           2.35
     2021-05-06      MPH                  Call dialogs                                            2.36
     2021-05-18      DLA                  BDE goes SMF                                            2.37
     2021-07-07      DLA                  Assembling units                                        2.38
     2022-02-17      MISC                 New CIM.Furnace Service                                 2.39
     2022-02-21      MISC                 Help tools                                              2.40
     2022-03-08      MISC                 RollerWaveDirection in Furnace Service                  2.41
     2023-01-16      MISC                 Pattern viewer in the sorter client                     2.42
     2023-02-28      MISC                 Several outputs with the same LocationID on a Sortjet 2.43
     2023-07-28      MPH                  Update status indicator call/supply dialogs             2.44
     2023-10-12      MISC                 Turning of lites at a turning station in front of an IG 2.55
                                          line
     2023-11-23      LUSC                 Multiple assignment for individual lites and            2.57
                                          HandleOpenReservationOnRequest added
     2024-01-16      Shahan               Replaced Furnace client with Furnace Service            2.44
     2024-03-11      Shahan               Sorter Service                                          2.45




     The installation instructions will assist the planner with the installation and
     configuration of the software named.




04.04.2025                          EN-INST-A+W Smart Factory.docx                                1
     Content



   Installationsanleitung ................................................................................ 1

   Beta - A+W Smart Factory - Multistep Automated Production ................... 1

   1         Voraussetzungen ............................................................................ 5
   1.1       Informix ................................................................................................................5
   1.2       A+W Production ...................................................................................................6
   1.3       A+W Stock Service ................................................................................................7
   1.4       A+W Optimization Service für Ofenoptimierung ..................................................8
   1.5       A+W Furnace Service für Ofensteuerung ..............................................................8
   1.5.1     Roller Wave Direction im Furnace Service ............................................................9

   2         Installation ................................................................................... 11
   2.1       Datenbank ..........................................................................................................11
   2.2       Stammdaten .......................................................................................................11
   2.3       MAPS Service ......................................................................................................12
   2.4       Furnace Service...................................................................................................12
   2.5       Sorter Service .....................................................................................................17
   2.6       Clarity Suite.........................................................................................................17
   2.7       Shopfloor Clients ................................................................................................18
   2.7.1     Dynopt Filler Client .............................................................................................19
   2.7.2     HEGLA Sortjet Client ...........................................................................................21
   2.7.3     North-Glass Ofen Client ......................................................................................25
   2.8       Hilfs-Tools ...........................................................................................................28
   2.9       Panorama Clients ................................................................................................29
   2.10      Dynopt Konfiguration Xopton.cfg .......................................................................29
   2.10.1    Sektion [CutGo] ..................................................................................................29

   3         Das Ticketsystem in der Smart Factory ......................................... 30
   3.1       Der Ticketstatus ..................................................................................................30
   3.2       Der Scheibenstatus .............................................................................................31
   3.3       Der Validationstatus ...........................................................................................32
   3.4       ValidateAndExecuteSheetTask ...........................................................................33


04.04.2025                                    EN-INST-A+W Smart Factory.docx                                                         2
   3.5       Ticketflow in Produktion .....................................................................................35

   4         HEGLA Sortjet ............................................................................... 36
   4.1       Reservierungen für Ein- und Austransport..........................................................36
   4.2       Scheiben in den SortJet hineinfahren und heraus fahren ...................................36
   4.3       ‚Conveyor‘-Modus ..............................................................................................37
   4.3.1     Patternviewer am Conveyor ...............................................................................38
   4.4       Mehrere Ausgänge mit gleicher LocationId an einem Sortjet .............................40
   4.5       Ansteuerung einer Drehstation vor einer ISO-Linie ............................................41
   4.6       Mehrfachbelegung für Einstellscheiben .............................................................43
   4.7       SJSJ-Interface ......................................................................................................43
   4.8       Manuelle Scheiben zur ISO-Linie ........................................................................46

   5         Ansteuerung North-Glass Ofen ..................................................... 49
   5.1       NorthGlass Kommunikation ................................................................................49
   5.2       Ofenoptimierung ................................................................................................49
   5.3       Ofenbetten in und aus dem Ofen fahren ............................................................51
   5.4       Größe des Ofenbetts dynamisch bestimmen......................................................52

   6         Mit der Smart Factory Einheiten zusammenbauen ....................... 55

   7         Durch die Smart Factory tauchen .................................................. 56

   8         Bruch in der Smart Factory ........................................................... 57
   8.1       Validierung des Nachläuferpools ........................................................................57

   9         Aufbau der Timeline ..................................................................... 59

   10        User Interface ............................................................................... 60
   10.1      Abrufdialoge .......................................................................................................60
   10.1.1    Statusbeschreibungen ........................................................................................60
   10.1.2    Allgemeine Laufinformationen ...........................................................................60
   10.2      Supply Dialoge ....................................................................................................64
   10.2.1    Supply SortJet 1/2 ...............................................................................................64

   11        BDE-Anbindung an die A+W Smart Factory ................................... 66



04.04.2025                                   EN-INST-A+W Smart Factory.docx                                                       3
   11.1      Ticket-Entwertung/Archivierung in der SmartFactory ........................................67




04.04.2025                            EN-INST-A+W Smart Factory.docx                                    4
1 Requirements
A+W Smart Factory is a multi-level automated production system (MAPS). It requires a run-capable
A+W Production SingleSite environment.
The associated infrastructure domain has to be configured, the default client is used.
MAPS requires the following services from the AWSOA:
    • Planning.Job
    •    Planning.BOM
    •    Planning.Detailed
    •    Planning StockService
    •    Planning.OptimizationService
    •    CIM.Maps
    •    CIM.BarcodeReading

1.1 Informix
If A+W Production is running under INFORMIX, there can be problems with the "InsertCursor". Here,
it is recommended that you switch off the "InsertCursor" in the infrastructure in the configuration of
the A+W production (EnableInsertCursors=0). For the AWSOA database under Informix, this can also
be made in the ODBC settings.




Figure 1-1 Informix configuration



By activating the so-called ConnectionPooling, for access of the SOA services to an Informix
database can be speeded up significantly (~100ms per service call).
For this, in the global ODBC settings, the setting must be made for the corresponding Informix
driver.




04.04.2025                           EN-INST-A+W Smart Factory.docx                                 5
Currently, the default value 60 can be used.




1.2 A+W Production
For all places defined in MAPS, there has to be a corresponding registration point in A+W Production.
These can be used by the MAPS clients in order to trigger bookings.
Output from the MAPS system and sorter require no definition in the machine assignment; other
places do, however.
The sequence of the processings in A+W Production has to correspond to the sequence defined in
MAPS since MAPS tries to arrange a BOM as transferred.
Example: [Cutting – Stamping – Grinding - Sorter] is the sequence in MAPS, for 3 processings for
cutting, stamping, and grinding have to exist in the BOM in precisely this sequence.



04.04.2025                           EN-INST-A+W Smart Factory.docx                                6
1.3 A+W Stock Service
Each sorter that should be controlled via the MAPS system (currently HEGLA Sortjets are supported)
has to be mapped in the Sorting Service (service interface of the A+W Stock Service). This way, MAPS
saves the state of the sorter; this is required, for example, in order to synchronize with the sorter.
Communication runs via a MAPS ShopFloor client for the Sortjet.
The configuration of a Sortjet is currently done via SQL and can look as follows for a Sortjet with 2
physical buffers and 4 virtual ones. The GUIDs in the SQLs are examples!
INSERT INTO Stock_Storages (Guid, VersionId, LockingToken, Id, Description) VALUES ('99aff9d1-b89e-
43f2-ab2c-aabf00a15a8e', 1, '00000000-0000-0000-0000-000000000000', 1, 'SortJet');

INSERT INTO Stock_StorageLocations (Guid, VersionId, LockingToken, Id, Description, Type, State,
LockId, StorageGuid) VALUES ('a1c15e0a-e736-4d56-bc3c-aabf00a15a9c', 1, '00000000-0000-0000-0000-
000000000000', 1, 'Pyhsical Buffer 1', 2, 1, '', '99aff9d1-b89e-43f2-ab2c-aabf00a15a8e');
INSERT INTO Stock_StorageLocations (Guid, VersionId, LockingToken, Id, Description, Type, State,
LockId, StorageGuid) VALUES ('84c1f6c7-d980-41b4-8b5d-aabf00a15aa1', 1, '00000000-0000-0000-0000-
000000000000', 2, 'Physical Buffer 2', 2, 1, '', '99aff9d1-b89e-43f2-ab2c-aabf00a15a8e');

INSERT INTO Stock_StorageSegmentProperties (Guid, VersionId, LockingToken, Description,
AccessBehavior, SegmentType, MaxThickness, MaxHeight, MaxWidth, StartGroupNr, MaxGroupCount,
MaxWeight, MinHeight, MinWidth, MinThickness, DistanceBetweenItems) VALUES ('09df2f5d-1f4a-4f15-970a-
aabf00a15aa1', 1, '00000000-0000-0000-0000-000000000000', 'Virtual Buffer 1', 2, 3, 12000, 2300000,
6000000, 1, 75, 6000, 250000, 350000, 4000, 0);
INSERT INTO Stock_StorageSegmentProperties (Guid, VersionId, LockingToken, Description,
AccessBehavior, SegmentType, MaxThickness, MaxHeight, MaxWidth, StartGroupNr, MaxGroupCount,
MaxWeight, MinHeight, MinWidth, MinThickness, DistanceBetweenItems) VALUES ('dd1679d3-6992-4b94-8a35-
aabf00a15aa6', 1, '00000000-0000-0000-0000-000000000000', 'Virtual Buffer 2', 2, 3, 12000, 2800000,
6000000, 1, 275, 6000, 250000, 350000, 4000, 0);
INSERT INTO Stock_StorageSegmentProperties (Guid, VersionId, LockingToken, Description,
AccessBehavior, SegmentType, MaxThickness, MaxHeight, MaxWidth, StartGroupNr, MaxGroupCount,
MaxWeight, MinHeight, MinWidth, MinThickness, DistanceBetweenItems) VALUES ('0e554c05-1944-435f-8b50-
aabf00a15aaa', 1, '00000000-0000-0000-0000-000000000000', 'Virtual Buffer 3', 2, 3, 12000, 2800000,
6000000, 1, 125, 6000, 250000, 350000, 4000, 0);
INSERT INTO Stock_StorageSegmentProperties (Guid, VersionId, LockingToken, Description,
AccessBehavior, SegmentType, MaxThickness, MaxHeight, MaxWidth, StartGroupNr, MaxGroupCount,
MaxWeight, MinHeight, MinWidth, MinThickness, DistanceBetweenItems) VALUES ('0a1c2fd4-00d7-47ee-a94e-
aabf00a15aaa', 1, '00000000-0000-0000-0000-000000000000', 'Virtual Buffer 4', 2, 3, 19000, 2300000,
6000000, 1, 50, 6000, 250000, 350000, 10000, 0);

INSERT INTO Stock_StorageSegments (Guid, VersionId, LockingToken, Id, Description, State, LockId,
StorageLocationGuid, PropertiesGuid) VALUES ('75e23876-a798-459a-9954-aabf00a15aaa', 1, '00000000-
0000-0000-0000-000000000000', 1, 'Virtual Buffer 1', 1, '', 'a1c15e0a-e736-4d56-bc3c-aabf00a15a9c',
'09df2f5d-1f4a-4f15-970a-aabf00a15aa1');
INSERT INTO Stock_StorageSegments (Guid, VersionId, LockingToken, Id, Description, State, LockId,
StorageLocationGuid, PropertiesGuid) VALUES ('aec580be-c24b-4eb0-9706-aabf00a15aaf', 1, '00000000-
0000-0000-0000-000000000000', 2, 'Virtual Buffer 2', 1, '', 'a1c15e0a-e736-4d56-bc3c-aabf00a15a9c',
'dd1679d3-6992-4b94-8a35-aabf00a15aa6');
INSERT INTO Stock_StorageSegments (Guid, VersionId, LockingToken, Id, Description, State, LockId,
StorageLocationGuid, PropertiesGuid) VALUES ('10820fb1-3f52-428d-b2ab-aabf00a15aaf', 1, '00000000-
0000-0000-0000-000000000000', 3, 'Virtual Buffer 3', 1, '', '84c1f6c7-d980-41b4-8b5d-aabf00a15aa1',
'0e554c05-1944-435f-8b50-aabf00a15aaa');
INSERT INTO Stock_StorageSegments (Guid, VersionId, LockingToken, Id, Description, State, LockId,
StorageLocationGuid, PropertiesGuid) VALUES ('094cadb4-60ed-4583-b7c0-aabf00a15aaf', 1, '00000000-
0000-0000-0000-000000000000', 4, 'Virtual Buffer 4', 1, '', '84c1f6c7-d980-41b4-8b5d-aabf00a15aa1',
'0a1c2fd4-00d7-47ee-a94e-aabf00a15aaa');


If additional buffers should be created, attention should be paid that the IDs of the physical and virtual
buffers in the Stock Service are unique. This means that the second Sortjet cannot have the ID 1 for
its first physical buffer. In this case, it could be number 3. The implementation between ID in the Stock
Service and that of HEGLA (for the control of the Sortjet) is done in the MAPS Sortjet client.




04.04.2025                             EN-INST-A+W Smart Factory.docx                                   7
1.4 A+W Optimization Service for furnace optimization
The A+W Optimization service is required in order to conduct furnace optimizations in the furnace
client and to retain the result. The result is required in order to move furnace beds in and out of the
Sortjet.
For details about the configuration of the furnace optimization in the A+W Optimization service,
please see the appropriate documentation. Currently it is so that the optimization itself is still done
via the BATCH file ORGA.BAT. This configuration is saved in the Windows user directory of the user
of the service:
C:\Users\{AWSOA Dienst Benutzer}\AppData\Roaming\A+W\Techsoft\XOPT\Ofenopti\
On the first start, the data is copied from the program directory into the user directory:
{ProgramFilesx86}\A+W\Techsoft\XOPT\Ofenopti\
Configuration files such as XOPT.CFG and LABEL.SET are also in this directory. In the LABEL.SET, as in
A+W Production, a barcode has to be defined.
Via the XOPT.CFG, the behavior of the optimization can be adjusted accordingly. The following
switches can be important:
    • ReduceFurnaceBedLength
        0 (Default) / 1; If active, tries to keep the optimization of a furnace bed as short as possible




                          0                                1
    •   FurnaceBedsToCompute
        Currently, the furnace optimization only uses and produces the first furnace bed. The others
        are discarded. With this switch, the furnace optimization can be configured so that only the
        first furnace bed is used. The optimization is also faster since it doesn't have to compute to
        the end. If the switch is set, the first N furnace beds are used, e.g.:
        FurnaceBedsToCompute=1

1.5 A+W Furnace Service for furnace control
        The A+W Furnace Service replaces the previous A+W Shopfloor Clients for furnace
        control (1 to 3 clients, depending on the configuration). The A+W Furnace Service
        offers the same functionality as the previous clients. In addition, there are more
        functions available.



04.04.2025                            EN-INST-A+W Smart Factory.docx                                  8
        The new service is in a position to communicate with various furnaces (currently:
        Glaston and NorthGlass). There are also still various views in the CX Suite in order
        to monitor the furnace area. This way, for example, you can see the last furnace
        beds optimized or prioritize furnace beds.
        The service is now not an active, cyclical querying of the Map Service, as with the
        old clients. Instead, the Furnace Service is notified by the Maps Service via publish-
        subscribe in case of new furnace tickets. If notifications are not received by the
        Furnace Service, then the MapsTester offers the opportunity to trigger a
        notification at any time. This is especially helpful for service cases and can be used
        by a service technician to eliminate problems.


        For configuration of the Furnace Service, there is a new switch in the A+W
        Infrastructure 6 Web with which, among other things, settings for furnace bed
        optimization (size of the default furnace bed, distances between lites in the
        furnace, etc.) can be defined.
1.5.1 Roller wave direction in the Furnace Service
        It's possible to specify a direction along the furnace bed transport rollers for each
        lite:
             o 1. Coordinates (width) along the transport direction
                or
             o 2. Coordinates (height) along the transport direction
        This information is already defined in the ERP system when the order is entered
        and stored within A+W Production as an informative processing on the BOM. This
        information can be read out with a current A+W Planning Bom Service and
        provided to Smart Factory accordingly. For this, the A+W CIM Maps Service must
        also be up-to-date.
        The result is an appropriate 'RollerWaveDirection' on a lite in the Smart Factory.
        Technically,      the     data      is   found       in      the      DB     field
        "Maps_Glassinstances.RollerWaveDirection".


        This information is then used within the A+W CIM Furnace Service in order to
        specify the exact rotation of a lite on a furnace bed and to transmit this information
        accordingly to the furnace optimization. For this, a current A+W Planning
        Optimization Service must also be used, which works on the new data structures.



04.04.2025                          EN-INST-A+W Smart Factory.docx                               9
04.04.2025   EN-INST-A+W Smart Factory.docx   10
2 Installation
An installation consists of several components: the MAPS service, CX Suite with Smart Factory
module, several MAPS ShopFloor clients, and possibly several additional clients, which are integrated
in Panorama scripts, for example.

2.1 Database
Data is stored in the A+W Production database in individual tables (prefix of the tables: Maps_). The
data structure has to be created by hand using an SQL editor since there are still no automatic
database update scripts.
The        corresponding       SQL        script       (MapsDatabaseSchemaSQLServer.sql            or
MapsDatabaseSchemaInformix.sql) is found in the installed service in the subfolder Database.
In addition, the database VIEW maps_processings in the A+W Production database is required. These
also have to be installed manually from the SQL file maps_processings.sql.

2.2 Master data
Master data has to be filled manually via a SQL because there are still no master data editors. The
script MAPSMasterDataDefaultContent.sql can serve for support.
When creating the master data, pay attention to the following. Each MAPS client that makes bookings
requires a registration point and a person with which the booking is done. This data has to be created
in the PDC master data. MAPS locations that are not sorters or outputs also require a corresponding
MZO machine ID.
In the master data there are agents (Maps_Agents), each of which manages a production area. If the
agent is a Sortjet, then the corresponding sorter (Maps_Sorters) has to be assigned. What kind of type
the agent is has to be defined. Currently, there are the following types for a MAPS agent:
     • 1 = IGU
    •   2 = buffer
    •   3 = TG
    •   4 = DYNOPT
    •   5 = FPG
    •   6 = Output from the MAPS system
    •   7 = Processing
    •   8 = Supply
    •   9 = LAMI

The individual locations in the MAPS system through which the lites pass are so-called locations
(Maps_Locations). For the definition, it is recommended that the LocationId be assigned the
corresponding number of the associated registration point. However, this is not obligatory.
Optionally, a location is assigned to a MZO machine. This is not necessary for output and sorters.
A MAPS locations is always assigned to an agent. Several locations can be assigned to the same agent.
Locations are grouped (Maps_LocationGroups). A MAPS location 0 ("somewhere") always has to exist.
A location has a type (LocationKind) that consists of a combination of the following values:



04.04.2025                           EN-INST-A+W Smart Factory.docx                                11
    •   0 = None
        The location can have inputs and outputs. No processing is conducted in this location.
        Example: a Sortjet for which there is no processing in the BOM or an output for which you
        want to generate an individual ticket.
    •   1 = Machine
        This location can have inputs and outputs. A processing is carried out. Location 0
        (Somewhere) is an exception here). Example: a grinding machine, the grinding processing for
        this machine is in the BOM.
    •   2 = Source
        This location is a source, there is no connection to this location. Example: cutting or goods
        receipt.
    •   4 = Input
        This location can receive tickets from Location 0 (Somewhere). Example: a ticket runs via this
        location, but has no direct connection. The prerequisite is that the location before it also have
        an output to Location 0.
    •   8 = Output
        This location can send tickets to the Location 0 (Somewhere). Example: a machine has a
        manual output that is used if no other route is valid.
Example: a cutting table with a manual output has the type 11: 1 (processing cutting in BOM) + 2 (it
is a generating processing) + 8 (manual output).

To connect the locations and define routes through the MAPS system accordingly, there are the hops
(Maps_Hops). A hop is a connection between 2 locations. It can be defined on a hop whether the
planned sequence of the lites is inverted if it goes over the hop (field Sorting = 1). This setting is
evaluated on a hop that refers to an end location. This is necessary, e.g. on an output on the system
that stores on A-racks. The sequence in both locations is inverted in this case.
For communication with the clients, there are the brokers (Maps_Brokers). Each broker is assigned to
an agent, an agent can belong to only one broker. There is a 1:1 relation here.
Last but not least, we need the configuration of the various clients (Maps_ClientConfigurations). A
SmartFactory client is assigned to a broker. Several clients can be assigned to the same broker. A client
has a registration point, a PDC person barcode, and a PDC StationId with which it can trigger PDC
bookings. Optionally there is a StationId for optimizations, this is important for the DYNOPT clients.
The name of the client is unique. If a client starts, it logs into the MAPS service with its name.
The CX Suite is also a client, but here has no individual configuration within the Smart Factory.

2.3 MAPS service
The MAPS service resides in the CIM domain (CIM.Maps) and is installed with an individual diskset.
Preferably on a ProcessServer on which the other services of the related domains were installed.

2.4 Furnace Service
The furnace service is also in the CIM domain and can be installed from the same diskset as the MAPS
service. To create a furnace bed with the furnace optimization, the A+W optimization service (from
the planning domain) and the flow service from the CIM domain are required.



04.04.2025                            EN-INST-A+W Smart Factory.docx                                  12
In order to configure the furnace service appropriately, there is a new switch "CIM MAPS Furnace
Settings" in the A+W Infrastructure 6 Web, with which we can make 5 types of settings.

    1. Furnace Bed Configuration




             1.   Width in mm: Width of the furnace bed in mm.
             2.   Height in mm: Height of the furnace bed in mm.
             3.   X Across the Flow Direction: Distance between the subplates along the X-axis.
             4.   Y Across the Flow Direction: Distance between the subplates along the Y-axis.
             5.   Distance to Edges Bottom in mm: Distance to the lower edge in mm.
             6.   Distance to Edges Left in mm: Distance to the left edge in mm.
             7.   Distance to Edges Right in mm: Distance to the right edge in mm.
             8.   Distance to Edges Top in mm: Distance to the upper edge in mm.




04.04.2025                            EN-INST-A+W Smart Factory.docx                              13
             9. Line Orientation: This is the direction in which the longer edge of a lite should be
                oriented.




                      i. 'None' should be set if the "furnace rollers" of the furnace bed should be
                         taken into account accordingly.
                     ii. ‘XDirection’ means that the longer edge of the lite is arranged according to
                         the X-axis of the furnace bed.
                    iii. ‘YDirection’ means that the longer edge of the lite is arranged according to
                         the Y-axis of the furnace bed.
All of the following factors are used to calculate special "floating corridors" (values with '0' prevent a
calculation).


             10. Factorization in % to Width Variation:
             11. Factorization in % to Length Variation:
             12. Factorization in % to Width Aspect Ratio Variation:
             13. Factorization in % to area Variation:



04.04.2025                             EN-INST-A+W Smart Factory.docx                                  14
             14. Reduce Furnace Bed Length: 0 (Default) / 1; With ‘1’ there is an attempt to keep the
                 length of the furnace bed as short as possible.




                          0                                 1
           15.         Furnace Beds to Compute: At the moment, the furnace bed optimization only
               uses the 1st furnace bed of an optimization. All additional furnace beds are discarded.
               With this setting, this behavior can be influenced. If only one furnace bed must be
               calculated, the optimization is faster since the remaining lites must be placed on
               additional furnace beds.
           16. Queue Length: Setting for determining the number of allowed (optimized) furnace
               beds in front of the furnace.
    2. Furnace Bed Optimization



             1. Desirable Number of Lites: Lites are assigned 3 optimization priorities.
                     i. Must Have
                    ii. Nice to Have
                   iii. Fillers

                This value specifies the % share of lites that should be counted to the category "Nice
                - To Have".
             2. Traverse Sequence Inverted on Output: > True: Transport out of the lites or of the
                subplates is done in the reverse order of the transport in (relevant depending on how
                the infeed and outfeed of the furnace are arranged).

    3. A+W Pattern Viewer Settings




04.04.2025                            EN-INST-A+W Smart Factory.docx                               15
             1. DisplayID:
                Designation of the pattern viewer instance to be activated, e.g.: “1#Furnace#OPTI”.
             2. DisplayType
                Describes which type of pattern viewer should be displayed. Possible values are:
                Optimization, Incoming, Outcoming
             3. WorkingMode:
                Describes in which processing mode lites should be processed in and out of the
                furnace (relevant, e.g., whether processing is done manually or automatically).
                Possible values; BedWise, SheetBySheet
             4. AllowBreakage:
                (Yes/No): If YES is selected, breaks can be reported via the Pattern Viewer.
                NOTE: Should not be allowed for the "optimization" pattern viewer.

    4. Machine Settings




             1. Machine Manufacturer: Specifies the machine manufacturer. Currently, the
                following manufacturers are supported: NorthGlass, Glaston
             2. Communication Type: Specifies the type of communication between machine and
                service. Currently the following communication types are supported: IP, OPC,
                Telegram.



04.04.2025                           EN-INST-A+W Smart Factory.docx                              16
             3. Corridor: Special corridor types for furnace bed optimization. Currently, the following
                values are defined: Unkown, Floating, Fixed
             4. Sortjet Id at Entry: Id of the Sortjet within the A+W StockService before transport
                into the furnace, which requests lites from this Sortjet.

    5. Communication




             1. IP: IP address of the service for communication with the machine.
             2. Port: Port of the service under which the machine controller logs into the client.
             3. TimeOut         In       Seconds:       Timeout        of      the       connection.


2.5 Sorter Service
The sorter service is also in the CIM domain and can be installed from the same diskset as the
MAPS service. It requires the CIM Maps and the Planning Stock Service. At the moment, the sorter
service is used within the "Sortjet view" in the CX Suite to provide the following information:

    1. Assignment of the virtual Sortjet buffer

    2. Assignment of the individual Sortjet slots
    3. Lites grouped according to the Sortjet outputs

For configuration, the sorter service must point to the correct physical Sortjet and for this, the
following settings must be made in the ICE-Grid-Admin tool:




    •   Machine and Locationid: Appropriate machine name and location ID of the Sortjet.
    •   StorageId: Id of          the         Sortjets within            the      A+W Stock Service.


2.6 Clarity Suite
To use the Smart Factory interfaces, the Clarity Suite has to be installed, and also the Smart Factory
AddOn. The following disk sets are required:
    • A+W Clarity Suite
    • A+W Clarity Suite Maps

After the installation, the Clarity Suite has to be started again in order to create the configuration files
automatically. These are in our directory:



04.04.2025                              EN-INST-A+W Smart Factory.docx                                   17
        %APPDATA%\A+W\AWSuite\

In the Settings.xml created in the directory, the Maps module has to be activated in order to
integrate the Smart Factory interfaces.




Figure 2-1 Configuration Settings.xml for Clarity Suite




2.7 Shopfloor Clients
The Smart Factory clients are console applications that are installed via the A+W Clarity MAPS diskset.
Installation is in the directory C:\Program Files (x86)\A+W\Clarity\Maps\Shopfloor Clients\.
There has to be a connection to the AWSOA infrastructure so that the MAPS service can be addressed.
The client is called via Maps.Shopfloor.Client.exe with the name of the client from the configuration
of the master data (table Maps_ClientConfigurationa). Which tasks the client should take over is
controlled in the master data via the field Maps_ClientConfigurations.ControlTypeName.
In addition, some client types require an XML configuration file that is provided via the second
parameter. Other necessary settings are stored in this configuration file.
It is recommended that you store these configuration files and the links to the call of the individual
clients on the TRANS drive under a directory MAPS.
Example BAT file for call of a client:
          C:
          CD "C:\Program Files (x86)\A+W\Clarity\Maps\Shopfloor Clients\"
          START Maps.Shopfloor.Client.exe "MyClient" \\AWPFileServer\trans\Maps\MyClient.xml

So that a DOS box doesn't just hang during operation, you have to switch off the "Quick Edit" mode.
If this is not the case, a DOS box hangs if you click in it. You can see this from the title of the DOS box,
where you will see the word "Selection" in front of the name. To come out of the mode, you have to
press "Enter" in the box once.




04.04.2025                                     EN-INST-A+W Smart Factory.docx                            18
Figure 2-2 Quick-Edit mode in DOS box

2.7.1 Dynopt Filler Client
The DynOpt client has to be installed in an environment with an ODBC data source for A+W
Production. The data source has to have the name that is stored in the AWSOA configuration.
In the DYNOPT environment, the new clusters are written to the DYNOPT system via the client. As
soon as this has happened, the DYNOPT is executed as usual via the A+W Realtime Optimizer
(prerequisite for this is a completely configured DYNOPT).
In the PANORAMA model of the DYNOPT, the MAPS service has to be called in order to set the status
of the lite accordingly to "produced" during production; for this, the PANORAMA model needs the
GUID of the DYNOPT client.
The Dynopt Filler client needs an XML file for the configuration:
 <DynOptFiller>
     • DefectBarcode
         Status barcode for defect booking; if not set, barcode 500000020 is used. Defect bookings
         are made for lites that cannot be reported broken in the Smart Factory during validation of
         the Smart Factory with the breakage pool.
     • NumberOfOutputLines
         Number of output lines in Dynopt. The value is equal to the value of NumberIGLines from
         the section [Panoprama] in the xopton.cfg
     • DynoptCuttingTables
         Dynopt tables. The tables' names can be taken from xopton.cfg, e.g. TB1,TB2.
     • SorterId
         ID of the sorter in the A+W StockService for which DYNOPT should reserve lites. The client
         determines the possible virtual buffers and forwards this information to DYNOPT.
     • SplitClusterByGroupkey (bool, default false) false: do not split cluster by the tickets’s
         groupkey, true: split cluster by the ticket’s groupkey
     • <OutputLine>
         Output configuration
           o Id
               Output's Id.
           o DynoptIGLinie



04.04.2025                              EN-INST-A+W Smart Factory.docx                           19
               DynoptIGLinie number from the Xopton.cfg
           o FinalLocation
               Final Ticket Location Id in SmartFactory, e.g. Unload SJ2
           o FinalLocationName
               Name of the Final Ticket location
           o < PrimaryBufferSegment >
               Primary buffer segment for the output. The selection of the primary buffer segment
               corresponds to the production efficiency. Example: the output line is in the area of
               buffer segment 2. Then PrimaryBufferSegment ="2".
           o <Name>
               Output's name. Not currently used
           o < OutputLineType >
               The output type can be 0 (harp rack) or 1 (IG line). The value of the OutputLineType
               has to be equal to the value of OutputType from the section[Panorama] in the
               xopton.cfg. Important: if in the xopton.cfg the OutputType for the output is not set,
               the RTO uses the default value 0. In this case, OutputLineType=0.
           o < BufferSegments></BufferSegments>
               Permitted buffer segments for this output
           o < AvoidBufferSegments ></AvoidBufferSegments >
               Buffer segments to be avoided for this output. Here the buffer segments are listed,
               which may only be used if the lites do not fit the other buffer segments due to their
               dimensions.
    •    TimeHorizonMinutes
         Defines the time horizon in minutes. Default value is 480 minutes. To deactivate this
         function, set the switch to 0.
    •    BacklogEfficiency
         Defines the efficiency for how a backlog can be cleared. Is required in order to calculate the
         time for the backlog for the time horizon. Default value is 1, means 100%.
         0.5 means 50%: for one hour's work on the backlog, 2 hours are required to clear it
         1.5 means 150%: for one hour's work on the backlog, 30 minutes are required to clear it
    •    ValidateCuttingBacklogAndRemakesTimeSpan
         Defines the call interval in seconds to the Maps service, which releases new approved
         batches according to the internal Maps timeline (see also TimeHorizonMinutes) and with
         the detailed service calls up potential remakes and approves them for renewed recutting if
         necessary. Default: 120 seconds.

Example:
Xopton.cfg
[PANORAMA]
NumberIGLines=2
OutputType1=1
OutputType2=0

XML-Datei Beispiel:

<DynOptFiller NumberOfOutputLines="2" DefectBarcode="500000020">
<DynoptCuttingTables>TB1,TB2</DynoptCuttingTables>
<SorterId>1</SorterId>
<SplitClusterByGroupkey>false</SplitClusterByGroupkey>
        <OutputLine Id="1" DyoptIGLine="1" FinalLocation ="119" PrimaryBufferSegment="2"



04.04.2025                            EN-INST-A+W Smart Factory.docx                                 20
                FinalLocationName="ABockWand SJ1" OutputLineType ="1" ItemsPerBufferSlot="1">
                <BufferSegments>2</BufferSegments>
                <BufferSegments>3</BufferSegments>
                <BufferSegments>4</BufferSegments>

                <AvoidBufferSegments>4</AvoidBufferSegments>
        </OutputLine>

        <OutputLine Id="2" DyoptIGLine="2" FinalLocation ="1319" PrimaryBufferSegment="1"
                FinalLocationName="AbockWand SJ2" OutputLineType ="1" ItemsPerBufferSlot="1" >
                <BufferSegments>1</BufferSegments>
                <BufferSegments>3</BufferSegments>
                <BufferSegments>2</BufferSegments>
                <BufferSegments>4</BufferSegments>

                <AvoidBufferSegments>4</AvoidBufferSegments>

        </OutputLine>
</DynOptFiller>

2.7.2 HEGLA Sortjet Client
The     Sortjet    Client    is   controlled     via    Maps_ClientConfiguration.ControlTyeName=
MachineControlHeglaSorter. The map of the HEGLA Sortjet is stored in the A+W StockService. For this,
the Id has to be stored in the master data of the sorter (Maps_Sorters.StockServiceId) under which
the StockService manages this Sortjet.
The client also needs another XML file for the configuration in which the connection information for
HEGLA MMI is set.
Tag <Sorter>:
    • <Ip>
        IP address on which the HEGLA MMI is running
    •   <Port>
        Port via which the client communicates with the MMI
    •   <Interface>
        Version of the HEGLA interface
    •   <ClientId>
        ID of the HEGLA client that is provided during LOGON
    •   <DummyMode>
        In this mode the client works with an internal dummy instead of the correct HEGLA MMI. This
        is no simulation and the IP has to be 127.0.0.1 here.
    •   <ConveyorMode>
        If this entry is 1, then the client works as a special HEGLA conveyor. This conveyor only has
        several infeed lines and no buffer. The customer "PressGlass" uses it as a kind of "transport
        conveyor" from the furnace into 2 possible Sortjets.
    •   <ForwardReservations>
    •   If this entry is present or is on 1, then the Sortjet client works in a special mode (similar to the
        ConveyorMode above). At the moment, this mode is only used for the customer "Eko-Okna"
        since the SJ3 controls the infeed line of the SJ4. For this, on the A+W side, a reservation must
        be made in SJ3 and this reservation must be "forwarded" accordingly for the lites that should
        go into the SJ4. That's why this new mode. Here, the SJ3 client opens a new reservation for
        the SJ4.


04.04.2025                             EN-INST-A+W Smart Factory.docx                                    21
    •   <TimeOutInSeconds>
        Timeout for the connection to HEGLA in seconds.
    •   <ChangeBufferReservationOnInput>
        True or False. If activated, a new item is calculated as soon as a lite runs into the sorting
        system. See Multiple assignment for individual lites for more information.
    •   <HandleOpenReservationOnRequest>
        True or False. If activated, tries to move the open reservations in called slots into other slots.
    •   <Station>
        There can be several stations configured in that <Station> is entered several times, one after
        another. This switch has the following attributes:
             o   Id
                 Number of the Hegla station
             o   Type (InputStation; OutputStation; PhysicalStorage; VirtualStorage;       ConveyorEnd)
                 The type of station.
             o   LocationId
                 The MAPS Location ID of the MAPS tickets on this input, output or the sorter itself.
                 Using the location ID, the client detects which station should be sent to HEGLA.
             o   Description
                 Optional: a description of the station.
             o   ManualStation (True or False; default=false)
                 Relevant for OutputStation; if True, then this is a manual station where the removal
                 of a lite has to be acknowledged by the user, which causes a ManualSheetRemove
                 Meldung from HEGLA to the client. This doesn't happen with automatic stations.
             o   NextRegistrationPoint
                 Optional switch via the PDC registration point to the next station. Is relevant for
                 OutputStation. If set, a PDC booking is made on this station as soon as the lite has
                 reached the HEGLA output station.
             o   SetBatchId (True or False; default=False)
                 If set, when filling the OutputSequence on the HEGLA is also sent the telegram
                 SetBatchId. For this, data (e.g. from a furnace bed optimization) has to be present.
             o   StockServiceMapping
                 Optional; if the ID of a virtual or physical buffer does not fit the ID in the A+W
                 StockService passt, then the ID from the StockService has to be entered here. If the
                 parameter does not exist, it is assumed that both IDs are identical.
             o   SortingMode
                 Optional; mode that determines the sequence for the input or OutputSequence.
                 Possible values:
                        CurrentTime (Standard), sorted by the time stamp how the lites came to the
                         station
                        FurnaceOptimization uses the result of a furnace optimization that for
                         OutputSequence happened afterward or for InputSequence before. Only the
                         first lite of the optimization is used.


04.04.2025                            EN-INST-A+W Smart Factory.docx                                   22
             o   SlotReservation
                 Is required for an OutputStation and describes the mode that should be used for a
                 reservation:
                        Single (default), one lite per slot
                        AscendingSequence, several lites in ascending order
                        SwapTwo, slots are filled in pairs. These have to be next to one another in
                         their sequence.
                        SwapTwoAndAscendingSequence, slots are filled in pairs and in sequence,
                         depending on what is better.
                        SwapFour this is like SwapTwo. The buffer slots are filled in groups of four
                         lites and have to be next to one another in the output sequence. This can be
                         used if according to the buffer it is possible to change the sequence and if the
                         lites can be exchanged during transport. Example: with presence of a wall
                         with 4 slots on the output side.
             o   MaxSheetsPerSlot
                 Default value=1; Maximum of lites in a slot. This is used for reservations in the
                 "AscendingSequence" mode. Has no effect on other modes. If the value is 1, then the
                 maximum of lites is ignored. If you only want to have one lite per slot, use the "single"
                 mode.
             o   SlotReservationGroup
                 Optional for an OutputStation. It describes how the lites to be reserved that the MAPS
                 services gives the client should be grouped again. Generally lites of a group are stored
                 together in a slot (exception with UnitCrossBatch mode). The sorting from the MAPS
                 service is not changed in the process (as long as no supply lites are involved).
                        None (default), no further grouping
                        Unit, lites of a unit (after barcode of the parent part) are grouped
                        Component, the same lites of units are grouped (order, item, part number)
                        Glass, the lites of the same glass type are grouped (glass type and thickness)
                        UnitIgnoreOrigin, lites of a unit (after barcode of the parent part) are
                         grouped, across batch limits. Unit mode considers the groups (batch rack),
                         this mode does not. In addition, in this mode the origin of the lite (direct
                         entry, e.g. supply or grinding and origin, e.g. cutting 1 or 2) is ignored. This
                         mode may not be used if lites of a unit come from different inputs, which can
                         overflow.
             o   SupplyStation (True or False; default=False)
                 This switch affects input stations. For a supply station, the Sortjet itself determines
                 the quantity of work to be reserved and requests them from the supply client.
             o   MaxSlotsInUse (Optional, default = 0)
                 Currently, this switch is used for a supply station. This is the maximum number of
                 slots that may be reserved for lites that are set via the supply input.



04.04.2025                             EN-INST-A+W Smart Factory.docx                                  23
             o       InaccessibleVirtualBuffer (Optional)
                     A list of virtual buffers that cannot be reached from this station. This can be
                     configured for input or output stations. Sheets that run via an input or output station
                     are not reserved in the virtual buffer defined here.
             o  AssemblyStation (Optional, True or False; default=False)
                This switch affects the content of the GetSheetData telegram to HEGLA. If the value
                is 'true', then for lites - that move through this station - the IsoCount, IsoIndex, and
                IsoUnitLabel are set in the telegram. Relevant for TG lites.
            o NoReservation (Optional, True or False; default=False)
                With this switch, reservations can be activated or deactivated. If the value is 'true',
                then no reservations are sent to Hegla (within the stock service, however,
                reservations are always created). Note: The value can only be used on a station of the
                type 'VirtualStorage'. Accordingly, reservations can be configured per virtual buffer.
            o FlowDirectionChangeOnInput (Optional, True or False, default=False)
                Must be set if ChangeBufferReservationOnInput is activated and the flow direction of
                the lites on the infeed line changes. See Multiple assignment for individual lites.
    •   <OutputLineConfiguration>
        Several output lines can be configured in that <OutputLineConfiguration> is entered several
        times one after another. This switch has the following attributes:
                 o    Id - (int) Output Line Id
                 o    FinalLocation - (int) Final Location
                 o    Name - (string) Name of the output line
                 o    <OutputFactorConfiguration>
                      Several entries for the factors per output can be configured. The switch has two
                      attributes:
                            SheetsCount - (int) the number of lites in SJ1 for the output
                             Factor – (int) the number in the range from 2.0 to 0
                              Example:
                          <OutputLineConfiguration Id="1" FinalLocation="2011" Name="BSG">
                          <OutputFactorConfiguration SheetsCount="0"   Factor="2.0" />
                          <OutputFactorConfiguration SheetsCount="50" Factor="1.5" />
                          <OutputFactorConfiguration SheetsCount="130" Factor="0.6" />
                          <OutputFactorConfiguration SheetsCount="200" Factor="0.3" />
                          <OutputFactorConfiguration SheetsCount="400" Factor="0" />
                          </OutputLineConfiguration>
                          <OutputLineConfiguration Id="2" FinalLocation="1319" Name="ESG">
                          <OutputFactorConfiguration SheetsCount="0"   Factor="2.0" />
                          <OutputFactorConfiguration SheetsCount="50" Factor="1.5" />
                          <OutputFactorConfiguration SheetsCount="130" Factor="0.6" />
                          <OutputFactorConfiguration SheetsCount="200" Factor="0.3" />
                          <OutputFactorConfiguration SheetsCount="400" Factor="0" />
                          </OutputLineConfiguration>
    •   The SJ client determines the number of lite N in the Sortjet for the output and compares this
        with the SheetsCount from the configuration. Among all SheetsCount <N the largest value of
        the SheetsCount is selected and the corresponding factor is used as output factor.




04.04.2025                                 EN-INST-A+W Smart Factory.docx                                24
    •   <PatternViewerConfiguration>
        An individual pattern viewer can be configured for the conveyor mode. It displays the lite to
        be created in the zoom level. This is configured as follows:
        <PatternViewerConfiguration ViewerName="1#CONV#001" ViewerType="Incoming" />
             o   ViewerName
                 Name of the PatternViewer instance to be addressed, e.g.: "1#CONV#001"
             o   ViewerType
                 Describes which lite is displayed. Possible value currently: Incoming


                      .
2.7.3 North-Glass furnace client
The North-Glass furnace client is controlled via Maps_ClientConfiguration.ControlTyeName =
MachineControlNorthGlassFurnace.
To execute a furnace optimization, the A+W OptimizationService is required. It must be configured
appropriately so that a furnace optimization can also be executed. This includes an appropriately set
XOPT.CFG and a LABEL.SET with the "BARCODE" field.
In order to request the lites of an optimization, a connection to the A+W StockService is required since
previously the lites have to be reserved there for a sorter after the furnace.
Every furnace client is configured appropriately via an XML configuration. Here the FurnaceClient
requests lites from an upstream Sortjet and transfer these after the furnace to a downstream Sortjet:
<Furnace>
    • MaxOptiPatterns
        (integer, Default 3) Because for the furnace optimization only the first optimization pattern
        is used, it makes little sense to optimize a lot of lites at the same time. Only as many lites are
        optimized so that the maximum number of optimization patterns anticipated is not exceeded.
        The optimal value has to be determined empirically. If the parameter is not set, the default
        value=3 is used. The optimal value is in the range from 3 to 6.
    •   Optimization
        True (default) / False. If true, then this furnace client will execute a furnace bed optimization
        on the available lites of the next glass type. The first bed of the result is reserved and the bed
        requested.
    •   MoveBedInProduction
        True (default) / False. If true, then the client may move a furnace bed into the furnace.
    •   MoveBedOutProduction
        True (default) / False. If true, then the client may set a furnace bed produced and move it out
        of the furnace.
    •   <InputSorterId>
        ID of the sorter in the A+W StockService in front of the furnace for which the furnace requests
        lites.




04.04.2025                            EN-INST-A+W Smart Factory.docx                                   25
    •   <OutputSorterId>
        ID of the sorter in the A+W StockService behind the furnace for which the furnace should
        reserve lites.
    •   <Port>
        Port under which the North Glass controller logs into the client.
    •   <FurnaceBedWidth>
        Width of a furnace bed in millimeters.
    •   <FurnaceBedHeight>
        Height of a furnace bed in millimeters.
    •   <FurnaceBedDistanceBetweenSheets>
        Distance between the lites on the furnace bed in millimeters.
    •   <TimeOutInSeconds>
        Timeout for the connection to North Glass in seconds.
    •   <MoveBedOutTravereOrder> (default Inverse) Inverse: move-out subplates are reserved in
        the reverse sequence. Normal: the subplates are reserved in the sequence that is defined by
        the optimization.
    •   <FurnaceOptimizationMode>
        (int, default=1) 1:Furnace optimization runs without logical buffer, 2: Furnace optimization
        runs with the simple process for the logical buffer.
    •   <OutputSorterSheetsProSlots>
        (int, default =1) 1: single assignment in the logical buffer, 2: two lites per slot in the logical
        buffer.
Furnace recipes
The furnace has different recipes for the glass processing. AWProduction and the furnace have
different designations for the same processing types. The processing type for each lite is defined by
AW Production and can be seen from the table Maps_Tickets.LotType. The <ProcessingType> tag
makes a machine-specific code (ProcessId) that is defined by the machine manufacturer available to
each LotType.
<ProcessingType> tag
     • ProcessId – (integer) Machine-specific code for the processing
    •   FeinLotType – (integer) Processing type according to AWProduction
    •   ProcessingName – (string) Processing description; no effect at the moment
    •   JumboNr - (integer, default=0) specifies the jumbo number for the process. Is used to change
        the furnace space dynamically. The furnace dimensions are defined in the table xopt_jumbo.
        For each value JumboNr, you can define several furnace dimensions depending on glass type
        and thickness. If JumboNr is not set or if there is no entry in xopt_jumbo, default furnace
        dimensions are used.
Important: if the TG client gets a lite with the FeinLotType for which there is no <ProcessingType>
configuration, the lite is not produced (the TG client does not know which ProcessId has to be sent to
the machine).



04.04.2025                             EN-INST-A+W Smart Factory.docx                                  26
Outputs
The furnace client has to recognize the outputs behind the next sorter in order to guarantee an even
filling of the sorter for all outputs. For each output, there is one of the following tags.
< FurnaceOutputLine> tag
      • Id –(int) unique Id of the output
    •   FinalLocation –(int) The MAPS location to which the output leads
    •   Name – (string) A name of the output, is used for display
    •   Type – (int) Type of the output
        1 - (RackOrdered)
        2 - (LaufOrdered)
PatternViewer
Furnace bed optimization can be displayed in the PatternViewer controlled by the client. Here, both
the ones in the furnace, the one before the furnace, and the furnace bed just optimized can be
displayed. For display, an entry in the configuration is required for each station:
<PatternViewerConfiguration> tag
    • ViewerName
        Name of the PatternViewer instance to be addressed, e.g.: "1#TB1#001"
    •   ViewerType
        Describes which furnace bed should be displayed. Possible values are: Optimization,
        Incoming, Outcoming
Sample XML file
There is a current sample configuration file in the installation directory under "Configuration".
<?xml version="1.0" encoding="utf-8" ?>
<ClientConfigurationExtension>
  <Sorter>
    <Ip>127.0.0.1</Ip>
    <Port>15000</Port>
    <Interface>SJ.4.1.0.4</Interface>
    <DummyMode>1</DummyMode>
    <ClientId>1</ClientId>
    <TimeOutInSeconds>180</TimeOutInSeconds>
    <HandleOpenReservationOnRequest>True<HandleOpenReservationOnRequest>
    <Station Id="208" Type="InputStation" LocationId="999" Description="KSR">
      <InaccessibleVirtualBuffer>1</InaccessibleVirtualBuffer>
      <InaccessibleVirtualBuffer>3</InaccessibleVirtualBuffer>
    </Station>
    <Station Id="210" Type="InputStation" LocationId="410" Description="Benteler"/>
    <Station Id="212" Type="InputStation" LocationId="210" Description="Supply" SupplyStat
ion="True" MaxSlotsInUse="20"/>
    <Station Id="1" Type="PhysicalStorage" LocationId="118" Description="S1" StockServiceM
apping="1"/>
    <Station Id="2" Type="PhysicalStorage" LocationId="118" Description="S2" StockServiceM
apping="2"/>
    <Station Id="214" Type="OutputStation" LocationId="119" Description="To Wall" ManualSt
ation="True" NextRegistrationPoint="119" SlotReservation ="AscendingSequence" SlotReservat
ionGroup="Component"/>
    <Station Id="401" Type="OutputStation" LocationId="1310" SetBatchId="True"
SortingMode="FurnaceOptimization"/>
    <Station Id="402" Type="OutputStation" LocationId="1510" AssemblyStation="True" >
      <InaccessibleVirtualBuffer>1</InaccessibleVirtualBuffer>
    </Station>



04.04.2025                            EN-INST-A+W Smart Factory.docx                                27
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


2.8 Help tools
In order to resolve problems or blockade situations within the Smart Factory, there are
several special console programs. These tools are defined primarily for knowledgeable
service technicians since operations here are performed directly on the customer's (live)
database. The programs are located in the Tools directory of the AWSOA services and bear
the names MapsTester, SorterTester, and FurnaceTester. Each of the programs forms part
of the functions of the respective AWSOA service. All three programs are called directly
from the cmd. Additional parameters such as client name or a lite barcode are transferred
to the call via additional arguments. With "?" you can display a list of all functions.




04.04.2025                       EN-INST-A+W Smart Factory.docx                             28
This way, for example, you can update the ticket status of a lite with the MapsTester or
generate new publish messages for the Furnace Service (if it has not received some
notification).




Here you see the syntax for booking the Sortjet-1 ticket of the lite with the barcode
"12345" to the TicketStatus "ReadyForProduction".

2.9 Panorama Clients
MAPS can be integrated into Panorama scripts, e.g. in the A+W Realtime Optimizer with DYNOPT or
in an A+W Production Terminal. There is also a Maps client that requires appropriate configuration.

2.10 Dynopt configuration Xopton.cfg
2.10.1 Section [CutGo]
    -   Import=2
        If a batch has been imported successfully from the DynopFiller, DynoptFiller writes the value
        300+StationId to pool_lauf.cutgo_status. If Import=2, Dynopt searches for newly imported
        batches and restarts the optimization.




04.04.2025                           EN-INST-A+W Smart Factory.docx                                29
3 The ticket system in the Smart Factory
A lite is unique in the MAPS system and with scheduling in the MAPS system, receives a ticket for each
location it passes. The lite can be identified uniquely via the SheetId. The SheetId can be the BARCODE
of a lite from the PPS system, but it does not have to be. Tickets are saved in the table Maps_Tickets.

3.1 The ticket status
A ticket has a status. With status between Committed and Finished, the tickets are in production
(Maps_Tickets.Status):
    • 0 = None
        No status assigned
    •   1 = Raw
        Data for the ticket was collected, as planned in the PPS detailed scheduling
    •   2 = Prepared
        The BOM information for the lite is assigned and made plausible.
    •   5 = Scheduled
        MAPS production steps determined
    •   8 = Confirmed
        MAPS production steps confirmed
    •   10 = Committed
        Lite scheduled in the MAPS system
    •   20 =TreatmentPossible
        All prerequisites for production fulfilled, if lite is ready, it can start
    •   30 = ReadyForProduction
        Lite ready for production
    •   35 = IncomingRequest
        Lite was requested for this step
    •   40 = Incoming
        Lite moves into location
    •   50 = InProduction
        Lite is being produced
    •   60 = ProducedAndReadyForNextStep
        Lite has been produced and is ready for next ticket
    •   65 = OutgoingRequest
        Lite was requested for the next step
    •   70 = Outgoing
        Lite is being moved out
    •   75 = ToCleanByClient
        Lite leaves the system (e.g. due to a break) and this ticket should be cleaned by a client (e.g.
        a Sortjet client deletes reservations on the machine)


04.04.2025                              EN-INST-A+W Smart Factory.docx                                30
    •   80 = Finished
        Lite has run completely through this step
    •   85 = CleanedByClient
        Ticket that should be cleaned by a client (status 75) was cleaned by a client.
    •   90 = Broken
        Lite is broken
    •   91 = Canceled
        Lite is canceled, no longer in the system
    •   93 – Cleaned
        Ticket was cleaned by the MAPS Service, e.g. after a break. Cleaning by a client is not
        necessary.

3.2 The lite status
The information for a lite is saved in the table Maps_GlassInstances. Here there is a SheetStatus that
applies for the whole lite, and thus to all tickets of the lite:
    • 0 = None
         The lite has no status, it has not yet been initialized and it is thus not ready.
    •   1 = Initialized
        Lite was initialized
    •   2 = PreparedForProduction
        Lite is prepared for production, e.g. reservations on a SortJet were made.
    •   3 = InProduction
        Lite is in production
    •   4 = Somewhere
        The lite has left the MAPS system, it may come back
    •   10 = Scrutiny
        The lite was taken out of production in order to be scrutinized, it can come back to
        production. Until then, it may not be produced further.
    •   11 = Broken
        Lite is broken
    •   20 = Cleaned
        Lite is in the status for cleaning. This process is asynchronous, it is cleaned if all tickets for
        the lite have the status Cleaned (93) or CleanedByClient (85)
    •   21 = PreparedForRemake
        A broken lite is prepared for a remake. Here, e.g. the remake counter is incremented.
    •   30 = RouteFound
        The lite has found a valid route through production.




04.04.2025                             EN-INST-A+W Smart Factory.docx                                        31
    •   80 = Finished
        The lite is finished and will no longer return to the MAPS system. It is delivered and can only
        be produced again with a new order.
    •   90 = Canceled (not yet used)
        The lite is canceled and will no longer return to the MAPS system.

3.3 The validation status
If the ticket chain is displayed in our interfaces, normally the ticket status is not displayed directly, but
rather the validation status. This is derived from the ticket status, but it also checks whether this
status is OK. If, for example, a ticket has been hung for hours at the inlet of a machine, then a
corresponding status is displayed that indicates the hanging of the lite.

    •   1 = Unknown
        The list has a non-defined status on this ticket.
    •   2 = Error
        The lite on this ticket has an error.
    •   3 = Temporary
        The lite is only temporarily on this ticket. This is, for example, if the lite has been requested.
        This status remains only until the lite arrives.
    •   4 = Planned
        The ticket for this lite is planned.
    •   5 = InProduction
        The lite is in production
    •   6 = Moving
        The lite on this ticket is moving.
    •   7 = Produced
        The lite on this ticket is produced.
    •   8 = Remake
        The lite is broken and the ticket for the lite is ready for a remake.
    •   9 = Canceled
        The ticket for the lite was canceled.
    •   10 = Delayed
        The ticket for the lite is behind the planned date.
    •   11 = Stuck
        The lite is stuck in the ticket's station
    •   12 Vanished




04.04.2025                              EN-INST-A+W Smart Factory.docx                                    32
3.4 ValidateAndExecuteSheetTask




Figure 3-1 Lite movement in MAPS

With the ValidateAndExecuteSheetTask interface, a client can report a break or a remake to the MAPS
service. For each request, the TaskCode has to be transferred, whereby currently not all of these are
supported by the outside; some are not yet implemented and others have only an internal function.
    • None = 0
         No action, lite "lives"
    •    Validate = 1
         Checks the lite according to the options transferred by the client to see whether, e.g. a lite
         could be regular, a break or a remake
    •    StartInvestigation = 10
         A lite is begun with an investigation and locked in the process for further processing
    •    FinishInvestigation = 11
         The investigation was ended and the lite is set back to its old status
    •    ReportBroken = 20
         Inquiry can come from all clients in order to react to a breakage report
    •    Cleanup = 30
         Lite is in the cleaning of its data, whereby various clients are instructed to cleanse their data
         (e.g. to delete reservations in a Sortjet)
    •    PrepareRemake = 40
         Prepares a lite in order to be used again as remake. Here, e.g. the remake counter is
         incremented.
    •    DetermineProductionRoute = 50
         A route through production is found. Can be the old route for a remake.



04.04.2025                             EN-INST-A+W Smart Factory.docx                                     33
    •   PrepareForProduction = 70
        Prepares the lite for production, lite was not yet started in production, but may be reserved
        for machines.
    •   FinishProduction = 80
        Lite is definitely finished and out of the MAPS system. It cannot be retrieved
Currently the server supports a ReportBroken and a PrepareRemake.
With the TaskCode options are also transferred that consist of a combination of the following
TaskOption.
    • None = 0
        No additional options, the task will be processed asynchronously. Errors in the validation
        cause the whole task not to be executed.
    •   Synchronous = 1
        The task will be executed synchronously, return if result is present. This option is currently
        not implemented.
    •   OverrideErrors = 2
        If this option is active, lites in the task that have no errors in the validation are also executed
        if there are lites with validation errors in the task.
In addition to the TaskCode and the TaskOption a list of the lites to be processed is transferred. Here
the lite is recognized by its SheetId. In addition, a time stamp of a break can be transferred and a
combination of the following options:
    • None = 0
         No special option is used
    •   IsBroken = 4
        The client identifies this lite as broken
    •   IsRemake = 8
        The client identifies the lite as a remake. In contrast to a lite that appears for the first time.
    •   IsCanceled = 16
        The client identifies the lite as cancellation; this lite is no longer needed. This option is not
        yet implemented.

The function returns a return value for each lite transferred. This is either 0 (None) if everything is
good, 1 (Pending) if the lite is still in processing (e.g. in CleanUp) or a value greater than 1, which is
then an error code.
Examples
SheetStatus 3  TaskCode 20, SheetOption 4                   = Result 0 / 1
SheetStatus 0  TaskCode 20, SheetOption 4                   = Result > 1
SheetStatus 20  TaskCode 40, SheetOption 8                  = Result 0 / 1
SheetStatus 3  TaskCode 40, SheetOption 8                   = Result > 1
SheetStatus 3  TaskCode 40, SheetOption 4+8                 = Result 0 / 1




04.04.2025                             EN-INST-A+W Smart Factory.docx                                       34
3.5 Ticket flow in production
If a lite is in production, you can see from the status of the individual tickets in which state the lite is
in production. The status of the individual tickets is incremented here. The sequence of the tickets of
a lite describes its path through production.
There are a few coupled ticket stati that have an effect on the status of the predecessor or successor
ticket. The following coupling affects tickets of a ticket chain in a section (DIVE):
           Predecessor: ProducedAndReadyForNextStep                Successor ReadyForProduction
           Predecessor: OutgoingRequest                            Successor IncomingRequest
           Predecessor: Outgoing                                   Successor Incoming
           Successor: IncomingRequest                              Predecessor: OutgoingRequest
           Successor: Incoming                                     Predecessor: Outgoing
           Successor: InProduction                                 Predecessor: Finished

If a lite from the Smart Factory is ejected via an UNLOAD station and it should later be put into the
Smart Factory via a SUPPLY station, this coupling does not apply between the two tickets of the two
sections. If a client ejects a lite, it has to inform the Smart Factory of this(MAPS Interface
ProgressLeft). In this case the ticket is set to Finished, the successor (SUPPLY) to TreatmentPossible.




04.04.2025                             EN-INST-A+W Smart Factory.docx                                    35
4 HEGLA Sortjet
If a HEGLA SortJet is activated, the appropriate ShopFloor client for this is required. The client receives
the lites via the MAPS service that are in range. Here the client communicates with the A+W
StockService in order to control the HEGLA SortJet and with HEGLA around the SortJet.
In the A+W StockService the current assignment of the StockService is saved, in the process
reservations are included. In addition, for each input and each output on the SortJet, a corresponding
list is managed, which describes which lite is precisely where at the moment.
If the connection to HEGLA is re-established (e.g. due to the restart of our client), they synchronize
both systems. HEGLA inquires with us in which state the system is and reports to us the outgoing
movements since the dropping of the connection. If something isn't right, the worker has to make the
appropriate decisions via the HEGLA terminal in order to restore a current state.

4.1 Reservations for transport in and out
A lite that should be moved into a Sortjet first has to be reserved in the SortJet. This is normally done
by a client in front of the SortJet (e.g. Panorama in the RTO before cutting of a stockplate). If there is
no reservation, HEGLA does not recognize the lite and it can thus also not be moved into the SortJet.
A reservation is made via a virtual HEGLA buffer, not the physical HEGLA buffer.
If a lite should be moved from the SortJet, the slot for transport out has to be locked. This is requested
by a client behind the SortJet. In the process, all lites of a slow are set in the A+W StockService to an
appropriate status. This means that no more reservations can be added in this slot. The locking for
transport out is only possible if there are no open reservations for the slot in question.
During transport out, not all lites of a slot have to be requested; one is enough. The slot is locked
completely. Lites have to be requested in the sequence in which they are in the slot since the HEGLA
system has no possibility to exchange the lites at will during transport out.
If several lites may be in a slot, this has to be set for each output in the configuration in the client.
Regardless of this, the client does not mix any Smart Factory groups and no lites that come from
different inputs or should go to different outputs.

4.2 Moving lites into and out of the SortJet
If a lite is ready to move into the SortJet, this lite is written by the client to HEGLA to the input list
(AppendInputSequence telegram).
When moving a lite out of the SortJet, the client writes the lite to HEGLA in an output list
(AppendOutputSequence telegram).
If lites are in the lists, these lites are moved in sequence by HEGLA. HEGLA reports each movement to
the client (GlassPosition telegram). The client saves the movements in the A+W StockService. Here, a
station, slot, and time stamp are always transferred. The station is the physical component where the
lite is currently located (e.g. a shuttle), the slot can be important, for example, for a shuttle with
several slots.
If a lite moves into the Sortjet, the same message (GlassPosition telegram) is sent, the station is the
physical buffer and the slot is the slot in the physical buffer. The client recognizes from the station
from its configuration that this is the Sortjet itself and it reports this to the A+W StockService. In this
case, the A+W StockService removes the lite from the input line and changes the reservation to a
confirmation.
When moving out of the SortJet, the lite remains in the A+W StockService until the HEGLA reports the
first lite movement (GlassPosition telegram).



04.04.2025                             EN-INST-A+W Smart Factory.docx                                   36
A lite is moved completely out of a SortJet until the last message (GlassPosition telegram) comes with
the HEGLA station of the output or until HEGLA sends a manual confirmation (ManuelSheetRemove
telegram). What precisely is correct has to be configured for each output on the client.

Adding to an inlet list is something the client does automatically if its ticket is set to the state
ReadyForProduction. The ticket status is set automatically to Incoming as soon as the lite was written
to the input list.
To reach the state ReadyForProduction, the previous ticket has to be set to
ProducedAndReadyForNextStep. In case of several tickets with status ReadyForProdction, the time
stamp when the status is set decides about the sequence in the input list.
To get a lite in an output list, the ticket has to be set to the status OutgoingRequest. When writing,
the status does not change in the output line. This happens only if HEGLA moves the lite and moves
out (GlassPosition telegram). Then the status of the ticket is set to Outgoing.
In order to reach the state OutgoingRequest, the following ticket has to be set to IncomingRequest.
In case of several tickets with status OutgoingRequest, the time stamp when the status is set decides
about the sequence in the output list.

If a whole furnace bed is written to the input or output line, previously the furnace bed and its
assignment is reported to HEGLA (SetBatchId telegram). Here, an ID of the furnace bed (BatchId), a
16-digit character string (created from the GUID of the optimization) is also transferred. Using this,
HEGLA communicates later directly with the furnace and it with us, in order to identify the furnace
bed in question. The client determines the assignment of furnace beds with a GUID via the A+W
OptiService.

4.3 "Conveyor" mode
The "conveyor mode" was created for the customer "PressGlass" since it has two possible Sortjets at
the outlet of its furnace as destination of the lites and furthermore there is a small gap between the
furnace outlet and this conveyor. Due to this gap, the tempered furnace bed is placed lite by lite on
the conveyor and this is confirmed on the HEGLA-MMI. Therefore, this conveyor is not a simple
transport conveyor with GlassPosition messages, but rather a type of Sortjet -- however, it has several
infeed lines and must also be synchronized with HEGLA. That's why this special mode.

That's why the conveyor is also created like a Sortjet:
   • Within the A+W Stock Service, as individual "Sortjet" with its own "Storage" and one pseudo
        "Location" and "segment" entry. The ID of this storage must then be stored in the table
        "maps_sorters" -- per new entry.

With regard to a ticket chain, the following is possible:

    •   Dynopt-2 Bottom -> Sorting 3 Furnace -> Furnace -> Sorting 4 Conveyor -> Sorting 1 -> (IGU
        IN 3 / IGU IN 4 / Sorting 1 Wall Out)

The conveyor ticket is between furnace and Sortjet. This is how the furnace reserves the Sortjet client.
So that this works, the conveyor ticket must be assigned to an agent that is not a sorter agent.

Then a possible XML configuration for the conveyor:



04.04.2025                            EN-INST-A+W Smart Factory.docx                                 37
Figure 4-1 XML configuration of a HEGLA conveyor

In comparison to a normal "Sortjet" configuration, the following is adjusted:
    • ConveyorMode
           o Serves to activate this special mode (default: 0 or tag optional).
    • Station with type "ConveyorEnd"
           o This is a new type for triggering a ticket update to 60-
               ProducedAndReadyForNextStep. This is necessary since at the end of the conveyor,
               there is a transfer to the following Sortjet and its infeed line. Here, the last stations
               between conveyor and Sortjet overlap. Due to the ticket update, the corresponding
               Sortjet ticket is set to 30-ReadyForProduction, so that the Sortjet fills its infeed line
               accordingly and the lite can then be taken over by its HEGLA MMI.
           o The ID of the station is set here to the value "210" and identifies the last station
               before the conveyor's output station. If necessary, this value must be adjusted so that
               the Sortjet transfer can occur without problems.
    • Pattern viewer for display of the lite to be placed
           o <PatternViewerConfiguration ViewerName="1#CONV#001" ViewerType="Incoming"
               />
                           ViewerName
                            Name of the PatternViewer instance to be addressed, e.g.: "1#CONV#001"
                           ViewerType
                            Describes which lite is displayed. Possible value currently: Incoming


4.3.1 Pattern viewer on the conveyor
The PatternViewer on the conveyor always displays the next lite to be removed from a
tempered furnace bed. The lite enters the display as soon as the conveyor ticket is set to
'30-ReadyForProduction'. It is displayed until the first GlassPosition message (= Input) is
sent by Hegla.



04.04.2025                                 EN-INST-A+W Smart Factory.docx                            38
In order to fulfill the requirement of an output-specific "standing edge" for the customer
Pressglass, two new activities were created in the PatternViewer:
    •   MoveStandingEdge
    •   RemoveText
With the first activity, it is possible - depending on the output - to shift the standing edge
accordingly. Pressglass needs this since there is a tilting table that lifts the lite toward the
inside at both outlets. This produces the requirement of placing the lite accordingly. Since
the lites usually also have logos and/or stamps in one corner, the standing edge must also
be depicted in order to be able to determine the final position.




                           Figure 4-2 Configuration of the MoveStandingEdge activity

On the sheet structure in the PatternViewer, the property "OutputId" is filled with the respective
NextLocationId of the conveyor ticket. This defines which path the lite takes (that is, the next location
can be Sortjet 3 or Sortjet 1).

The activity could, in principle, use any text property with a specific integer value. Here we use the
previously mentioned OutputId. This is therefore entered in the "TextId" variables (note quotation
marks). The "TextValue" variables are whole-number fields. Here the LocationId is entered for which
the StandingEdge must be redrawn. The number of segments by which the StandingEdge must be
shifted is stored in "MoveBy". Since Pressglass only lets rectangular lites run over the conveyor, a 2 is
entered here. Thus, a StandingEdge that is on segment 1 is shifted to segment 3. Shaped lites are not
intended here and if necessary, a fixed defined value of 2 would also not always be correct.

The second "RemoveText" activity serves only to remove the one property from the lite structure so
that it is not also displayed in the tooltip in the PatternViewer.




04.04.2025                             EN-INST-A+W Smart Factory.docx                                 39
                              Figure 4-3 Configuration of the RemoveText activity

Here, the "OutputId" is specified (in quotation marks), which should be removed again before the
final display.

Finally, the flow within a corresponding workflow looks like this:




                                     Figure 4-4 Sequence of the activities



Important is only that the optional 'RemoveText' activity is done after the 'MoveStandingEdge'.
Otherwise, the OutputId property would be removed and a shifting of the standing edge would no
longer be possible.

4.4 Several outputs with the same LocationID on a Sortjet
With some sorting systems, it can happen that there are several outputs with the same
LocationId. Thus, for example, there can be two transport out walls on a Sortjet that have
the same transport out restrictions and thus only get one LocationId within the
SmartFactory. However, both transport out walls have different machine-specific IDs,
which are required, e.g., for Hegla for the correct transport out. This constellation was not
previously possible since the transport out functioned using a single LocationId.


The following expansions have now been added to the Maps service and the Sort-
Shopfloor Client in order to enable this constellation.




04.04.2025                             EN-INST-A+W Smart Factory.docx                              40
Figure 45 Sortjet configuration for sorter client

In comparison to other sorter configurations, it is noteworthy here that there are two Hegla-specific
IDs (203 and 204) for the same LocationId (712). Here, 203 and 204 are two identical transport out
walls.

The corresponding Production Terminal then requests lites at the respective Hegla output. So that it
is clear at which output the tickets should leave the system, there is the following new column in the
configuration table "maps_clientconfigurations":


Figure 4-6 Excerpt from 'maps_clientconfigurations'

Here the corresponding Hegla ID for the output is assigned to the respective client name (which is
used in the corresponding panorama file of the PTs). Thus the corresponding Output ID is assigned to
the Production Terminal belonging to the client name. This configuration must be made appropriately
in this table (in addition to the corresponding configuration of the stations in the sorter configuration,
see above).


4.5 Activation of a turning station in front of an IG line
If can be necessary to turn lites when calling from a Sortjet before IG assembly according
to their structure/coating. This is also required if there are several IG lines for a sorter,
which are arranged to the left and right of the glass flow direction.
If necessary, it is first decided dynamically on the respective IG line which lites are called
up, depending on utilization. The prerequisite is that the IG lines have the same lite
restrictions. Then there will very probably be online one LocationId for the IGIn tickets in
the smart factory.
If, for example, there are 3 IG lines that are not all oriented the same way, lites may need
to be turned if they were planned for line 1 and now are called to line 3.
For this, the sorter configuration must first be expanded:




04.04.2025                                     EN-INST-A+W Smart Factory.docx                          41
Figure 47 Sortjet configuration for turning logic

There are three new parameters for this:
   • AdditionalColumnForOrientationCheck
           o For this, the column must be specified that is relevant, whether or not the
              respective lite must be turned (not relevant if it is a float lite). This information
              must be filled via a special SP after the detailed scheduling (in addition to the
              required 'prodmirror' field that defines the turning). For the configuration, the
              tables 'Param1-Param5' of the table 'fein_unit' can be used. If no column is
              specified, the turning logic is not active by default.
   • OrientationInGlassFlow
           o The orientation of the line within the glass flow is described here. As values,
              "None, Left, Right" are provided, whereby 'None' is the default if nothing is
              specified.
   • MachineId
           o The physical machine is entered here that belongs to this line. The Id is
              required in order to be able to determine whether the 'prodmirror' field must
              be inverted.

It is also noteworthy with the configuration above that all three IG lines have the same
LocationId. This enables dynamic calling to the respective lines.

Final example:
Line A is planned on line 1 and has 'prodmirror' flag 1. If this lite is now called to line 3, the
'prodmirror' flag must be inverted (that is, prodmirror becomes 0) -- but with call to line 2
not. Why?

The reason is that lines 1 and 2 have the same orientation in the glass flow, but line 3 does
not.



04.04.2025                                     EN-INST-A+W Smart Factory.docx                   42
The shopfloor sorter client checks on transport out whether the planned and now calling line
are different, and if so, whether their glass flow directions differ. If this is the case, the original
'prodmirror' flag of the planned line is inverted. For all affected lites, before the actual
'AppendOutputSequence' telegram, a corresponding 'ChangeSheetData' telegram with
appropriate turning information is sent to HEGLA.


4.6 Multiple assignment for individual lites
So that the shopfloor sorter client stores more than one lite per slot, the parameter
ChangeBufferReservationOnInput must be set. With this, another calculation of the item
of a lite is initiated as soon as it is fed into the SortJet. Then a ChangeBufferReservation
telegram with the new slot is sent to the Hegla SortJet. This applies for every input line.
Here, special attention must be paid to the direction of the glass flow along the entire
infeed line. If the lites are transported from the left on the shuttle and they leave it on the
left, the glass flow direction changes. In this case, the parameter
FlowDirectionChangeOnInput must be set for the corresponding station in order to ensure
the correct sequence of the lites. If the lites are transported from the left to the shuttle
and they leave it to the right, the parameter does not have to be set.

4.7 SJSJ interface
This mode was created specially for the customer 'Eko-Okna' since here there are two Sortjets one
after another, the front Sortjet manages the lites for the rear Sortjet in its infeed sequence. The reason
for this is that it is a type of "Bypass" and the infeed shuttle of the front Sortjet can transport lites
both into its own buffer as well as on the infeed line to the rear SJ.

Both Sortjets are configured entirely normally in the SMF. A particularity is that the front Sortjet gets
another virtual buffer configured, which maps the rear Sortjet. The reason for this is that a reservation
is required if lites come from several tables but have the same LocationId on the ticket. So that the
shopfloor client can reserve the lites accordingly in this second buffer, the panorama of the RTOs
must also be adjusted. For this, please also check the installed version of the RTO and update if
necessary.




Figure 4-8 Configuration of the RTO options – part 1/2

First, this assignment of ticket locations to virtual buffers must be created accordingly. IN this case,
tickets of the rear Sortjet have the location 740 and thus it is assigned her to the 2nd newly created
buffer. The other two locations 1651 and 1661 are both IG line outputs and are assigned to the 1st
virtual buffer. Here it is noted that the first Sortjet has only one own virtual buffer.


04.04.2025                                   EN-INST-A+W Smart Factory.docx                            43
Figure 4-9 Configuration of the RTO options – part 2/2

Furthermore, the following property "DECIDE_SMARTFACTORYBUFFER" must be created. This finally
sets the right virtual buffer for each lite.




Figure 4-10 Creating the second virtual buffer

The additional virtual buffer can be seen here, which must be created under "Warehouse" accordingly
in the Planning.Web. Here you can see that another physical buffer was created for this virtual buffer.
This serves a better overview and structure.




04.04.2025                                       EN-INST-A+W Smart Factory.docx                     44
Figure 4-11 Configuration of the front Sortjet

In Abbildung 4-1, you can see the configuration of the front Sortjet. Especially the following options
are                          now                             relevant                            here:

     •    ForwardReservations
              o A 1 must be entered here. This ensures that for all lites that must go into the rear
                  Sortjet, an appropriate reservation must also be made with the 2nd Sortjet. It is then
                  worked through in the shopfloor client of the front Sortjet. Only if this reservation
                  was successful is the original reservation completed on the front Sortjet.
     •    Station with type "ConveyorEnd"
              o Here the "transfer station" of Hegla must be specified, at which the lites should then
                  be transferred to the input sequence of the rear Sortjet.
     •    Station with type "OutputStation"
              o Here you can also see from the description that the corresponding output station of
                  the 1st Sortjet is toward the 2nd Sortjet. For LocationId the location of the 2nd Sortjet
                  ticket must be specified. Furthermore, you can also see here that the virtual buffer 1
                  is defined as not available. This ensures that lites for this output are also only assigned
                  to the 2nd virtual buffer.
     •    Station with type "VirtualStorage"
              o Here the special 2nd virtual buffer is defined. Note that for the Location Id the
                  location of the 2nd Sortjet ticket must be specified.




04.04.2025                                       EN-INST-A+W Smart Factory.docx                           45
Figure 4-12 Configuration of the rear Sortjet

With this configuration, it must only be configured that for the "SourceToStationMappings" the client
name of the front Sortjet must be entered. Thus the lites from the front Sortjet are assigned the input
station with the ID 201 (via station and LocationId).


4.8 Manual lites to the IG line
If lites for assembly of an IG unit also reach an IG line manually from a rack, then the automation of
the line must be stopped accordingly in order to be able to let the operator set up these lites. This
occurs for the manufacturer Hegla with a special ActionCode, which can occur as a placeholder in an
output sequence of automatic lites.

So that the stopping of the line works, all required A+W components must have the corresponding
status and furthermore, Hegla must also support the IsoLineEventFinished telegram in its SJ interface
at the customer (see also release notes for feature #127809).

The SMF must be configured appropriately in order to be able to generate an appropriate supply
ticket (additional hops, locations, etc.). Via the restrictions in the layout service (table
"Layout_FunctionalExpressions"), restrictions are defined that must be attached, e.g., to the SMF
location (table "Layout_Locations.RestrictionGuid") of the Sortjet supply ticket in order to be able to
distinguish prolonging (e.g. => lite goes through the Sortjet again) and re-use (e.g. => lite is placed on
the line manually).




04.04.2025                                      EN-INST-A+W Smart Factory.docx                         46
Figure 4-13 View of a PT IG call dialog with 'manual supply' information

In the view above, you now see a new column 'Manual supply', which contains two values separated
by '/'. The first value displays the currently available of the total 'Manual supply' lites (2nd value). By
default, this new column is not active. In order to show the column on the dialog, the following option
must be set in the corresponding "Options.cs" for the respective panorama of the IG line:




Figure 4-14 Setting of the 'Manual Supply' option in IG-Options.cs



A lite is available if the corresponding ticket receives the status '60-ProducedAndReadyForNextStep'.
This can be triggered via a corresponding registration point booking in the SMF. For this, first a new
registration point for the rack next to the IG line should be created, to which the prepared rack can
be booked by the operator if the lites are needed on the IG line in the near future. Next, the SMF must
be configured appropriately so that with this booking, the corresponding ticket of the 'Manual supply'
agent should be updated to the status '60-ProducedAndReadyForNextStep'. For this, see also chapter
BDE-Anbindung an die A+W Smart Factory.

This creates a corresponding workflow, with which these additional lites are available and the
operator on the IG line can get a complete overview of all units.




04.04.2025                                   EN-INST-A+W Smart Factory.docx                             47
If now a unit with such additional lites is called up, then the Sortjet's outfeed to the IG line stops
accordingly and the operator can place the lites manually and confirm this on the machine with the
corresponding button.




Figure 4-15 Example of a 'Manual Supply' lite with corresponding ticket chain

In the figure above, you see a lite that was previously booked with "ReUse" in the Production Terminal
and thus has received an expanded ticket chain expanded by two new tickets. So that the lite is not
put back through the Sortjet on the line, in this example, the SMF restriction on the "Sorting-3 IN"
supply infeed of the Sortjet must be created so that this input e.g. is only met e.g. with "Prolonging"
actions in the Production Terminal.




04.04.2025                                   EN-INST-A+W Smart Factory.docx                         48
5 Control of North-Glass furnace
The furnace activation is divided into 4 function blocks. These can be obtained in a Maps ShopFloor
client. It is recommended that you control it via 3 different clients.
Each of the function blocks has its own A+W PatternViewer in order to display the furnace bed in
question.

5.1 NorthGlass communication
Communication with the NorthGlass furnace is a function block. If several clients should control the
furnace, only one may handle the communication with the furnace. Here it is recommended that you
use the client that also executes the optimization. In the other clients, set the port for communication
to 0 in the XML configuration.
If there is communication with NorthGlass in the client, this will be displayed accordingly.
If no communication can be established, you should check whether the firewall is locking the port for
communication.
So that a furnace bed moves into the furnace, NorthGlass receives a signal from HEGLA that the next
furnace bed is complete and can be moved in. The signal includes the 16-digit BatchId of the furnace,
which we previously reported to HEGLA. With this BatchId, NorthGlass asks the client about the
composition of the furnace bed. This information is required so that NorthGlass can find the correct
recipe.
Additional information from NorthGlass is the moving in of a furnace bed and the breakage reporting
of a whole furnace bed. Currently the breakage reporting is not supported due to technical problems
at NorthGlass. Lites have to be reported broken individually at the output.

5.2 Furnace optimization
Furnace beds are moved into the furnace; beforehand, these have to be optimized via the furnace
optimization. A furnace optimization is possible if there are lites ready (in the HEGLA SortJet to move
out for the furnace output) and the last furnace bed requested has begun to move to the furnace. In
the process, several furnace beds can be under construction in front of the furnace.




04.04.2025                            EN-INST-A+W Smart Factory.docx                                 49
Figure 5-1 Starting furnace optimization

If lites are being optimized, then the first furnace bed of the optimization is used, the rest are
discarded. There is an attempt to reserve the lites on this bed. So that a reservation works, the
corresponding ShopFloor client on the HEGLA Sortjet has to run behind the furnace. After 10
attempts, the optimization is cancelled and there can be a re-optimization. The client determines the
virtual buffer for the lites to be reserved using the data from the StockService.
If the reservation was successful, the tickets of the furnace bed are regrouped on the furnace. The
group key is the GUID under which the optimization is stored in the OptimizationService. Using the
grouping, you can recognize a furnace bed.
After the grouping, the furnace bed is requested, in that the status of the tickets is set to
IncomingRequest; the consequence of this is that the coupled status of the predecessor (ticket on the
HEGLA SortJet in front of the furnace) is set to OutgoingRequest.
As long as a furnace bed exists where all tickets have the status IncomingRequest, no further
optimization is started. If a lite of the furnace bed has the status incoming, another optimization can
be started. A lite gets the status Incoming if the ticket is set on the HEGLA Sortjet to status Outgoing.
This happens as soon as HEGLA moves out one of the lites from the Sortjet and it is reported on the
ShopFloorClient on the Sortjet.
The current furnace bed of the optimization can be displayed on a PatternViewer. A furnace bed is
identified via a unique 16-digit BatchId. This BatchId is determined from the GUID of the furnace bed
(not the GUID of the optimization!) and is saved on the ticket in the CurrentLocation field for queries.




04.04.2025                                 EN-INST-A+W Smart Factory.docx                             50
Figure 5-2 Result of a furnace optimization in the PatternViewer


5.3 Moving furnace beds in and out of the furnace
Additional functions are moving a furnace bed in and out of the furnace.
You confirm the moving in or out manually in a client. Reporting happens either in the client or in the
connected PatternViewer.
Moving in can come automatically via the communication from the NorthGlass furnace. If you want
to report a break, this has to happen before the NorthGlass report.
Without PatternViewer
If you are not using a PatternViewer, the current furnace bed is displayed in the client and the tickets
are set to status InProduction with confirmation with the Y key. To update the display, another key
can be pressed.




Figure 5-3 ShopFloor client in front of the furnace without PatternViewer




04.04.2025                                   EN-INST-A+W Smart Factory.docx                          51
With PatternViewer
If a PatternViewer is used, then the current furnace bed there is displayed. You can mark lites broken.
The furnace bed is confirmed in that you press the right arrow to continue.




Figure 5-4 ShopFloor Client in front of the furnace with PatternViewer




Figure 5-5 PatternViewer in front of the furnace


5.4 Determining the size of the furnace bed dynamically
The size of a furnace bed is determined via the XML configuration. If you want to use different furnace
bed sizes for different TG articles, this can be done via the A+W Production master data.
For a TG article, a glass article and a stock dimension have to be created in the master data. This is
normally not required.
The shape trim in the glass article describes the (minimum) distance between two lites. The trim of
the glass articles can describe an additional edge of the furnace bed.




04.04.2025                                   EN-INST-A+W Smart Factory.docx                         52
Figure 5-6 Glass article master data for managing furnace beds

Via the stock dimension management, various dimensions of furnace beds can be created for a glass
type. Each stock dimension HAS to be assigned to a table. Here, the manual cutting is selected.
The usable dimensions of the furnace bed are managed in:
    • Width: corresponds to the furnace bed length
    •    Height: corresponds to the furnace bed width
The key field Lagermass-Nr serves to provide various restriction records. Whether for different
processing types or different furnaces. The assignment is made in the XML configuration of the client.
Processing types for tempering:
    • 1500 – Tempering
    •    1505 – Marine glass
    •    1510 - Partial tempering




04.04.2025                                  EN-INST-A+W Smart Factory.docx                         53
Figure 5-7 Stock dimension master data for managing furnace beds

Example of XML configuration of the client:
...
<ClientConfigurationExtension>
 <Furnance Optimization="True" ...>
  ...
  <ProcessingType ProcessId="1" JumboNr="1500" FeinLosTyp="1500" ProcessingName="ESG" />
  <ProcessingType ProcessId="2" JumboNr="1510" FeinLosTyp="1510" ProcessingName="TVG />
  <ProcessingType ProcessId="4" JumboNr="1505" FeinLosTyp="1505" ProcessingName="Marine" />
  ...
 </Furnance>
</ClientConfigurationExtension>
...




04.04.2025                                 EN-INST-A+W Smart Factory.docx                     54
6 Assembling units with the Smart Factory
To assemble lites, special things have to be considered so that the right lites are assembled in the
right order.
There is a sorting system before a LAMI, FPG or IG line. If the slots of the sorting system can be
assigned multiple times, the output to the lines has to be configured so that a unit can be stored
together. This means that only lites for a single unit are in a slot.
The units are produced in the sequence from the detailed scheduling; in the Smart Factory, this is the
sequence of the parents of the individual lites. When calling up to the line, this sequence is considered
during removal.
The sequence for how the individual lites are moved on the line is determined from the detailed
scheduling. Here it is absolutely necessary that the individual lites of a unit are in the usage batches
on a harp rack. The sequence corresponds to the sequence of the slot numbers. So that this is
achieved, the harp rack has to be of the mode "together" in the detailed scheduling. With this mode
and the function of the AUSGANGSNR, you can determine the sequence of the individual lites in the
detailed scheduling. Another mode, e.g. "compact," is not permitted here.




04.04.2025                            EN-INST-A+W Smart Factory.docx                                  55
7 Diving through the Smart Factory
In production, it can happen that a lite passed through the same station several times. A prominent
example of this would be multiple screen printing.
More relevant in the Smart Factory are lites that leave the Smart Factory in order to be processed
outside of the SmartFactory and then inserted back into the Smart Factory.
Example: We have filled a sorter from cutting and from it, a furnace is fed. Now lites are in the sorter,
which receive a processing that is done outside of the Smart Factory before the hardening. Thus the
lites do not initially move into the furnace; instead, they are moved out of the sorter and moved back
into the sorter after the processing. As soon as the lite is in the sorter for the second time, it can now
be moved into the furnace. After the furnace, the lite should be installed in a LAMI. Since the LAMI
line is filled via the sorter, the lite has to be moved back into the sorter. The lite thus passes through
the sorter station three times.
So that the Smart Factory can distinguish the sections of a lite, the ticket chain is subdivided into
partial sections. The boundary of a segment is always a supply input into the Smart Factory. As soon
as this limit has been passed, the lite is in the new section.
The lite from the example has the following ticket chain
           CUT  GRIND  SORTER  UNLOAD SORTER  SUPPLY  SORTER  FURNACE  UNLOAD
           FURNACE  SUPPLY  SORTER  LAMI
This chain is divided into 2 sections:
           Section 2: CUT  GRIND  SORTER  UNLOAD SORTER
           Section 1: SUPPLY  SORTER  FURNACE  UNLOAD FURNACE
           Section 0: SUPPLY  SORTER  LAMI
The last section of a ticket chain always gets the number 0. The number of the section is then
increased to the first ticket. This number is saved on the ticket in the database field
MAPS_TICKETS.DIVENUMBER.
In order to detect in which section production is happening, the number of the current section is
saved in the database field MAPS_GLASSINSTANCES.ACTUALDIVE.
With the transfer from the Smart Factory via an unload ticket in the Smart Factory via a supply ticket,
the client has to communicate at the unload of the Smart Factory that it has now "let the lite go." If
this happens, the status of the supply ticket is set to TreatmentPossible (20) and the current section
is reduced by one.
If the sorter client now asks the Smart Factory for this lite, then it receives the data of the ticket of
the current section.




04.04.2025                             EN-INST-A+W Smart Factory.docx                                  56
8 Breaks in the Smart Factory
Breaks in the Smart Factory have to be reported to the A+W Production PDC by the triggering client
if they should go into the breakage pool there. The Smart Factory itself does not do this automatically.
The ShopFloor clients have a connection to the PDC and book breakage accordingly.

If a breakage message is triggered in the Smart Factory, the tickets have to be cleaned up. The
SheetStatus of the lite is set to 20 Cleaned. The tickets that can be cleaned up by the MAPS Service
directly get the status 93 Cleaned. Tickets that have to be cleaned up by a client get the status 75
ToBeCleanedbyClient. The affected client has to process these tickets and if successful, the ticket gets
the status 85 CleanedByClient.
Currently, this only affects the Sortjet clients since these have to clean up any existing reservations.

If a remake tries to produce, a cleaned-up lite can be brought back to life if all tickets have the status
85 or 93.
So that the client responsible for cutting the remake knows whether a remake is OK or not, it has to
query the service before cutting. For this purpose, there is the function ValidateRemakes in the
Query-Interface. Only if this gives the OK can a remake be produced.

8.1 Validation of the remake pool
It can happen that there is an attempt to cut remakes and this is not possible in the Smart Factory. If
this happens, the remakes are not cut, they disappear or the system stops. There are different causes
for this problem.
One of the causes is that a lite was reported broken outside of the Smart Factory, but the Smart
Factory still has access to this lite. The lite might be still being processed by a machine or be in a
SortJet. The Smart Factory cannot know where the lite actually is if nobody tells it this. It can happen
that a lite is missing and you don't know where it is and it has simply been reported broken. Now,
according to the Smart Factory, it is still in a SortJet. Then you have to check whether this is really the
case and if so, either ignore the break and continue producing the lite or remove the lite and then
report it broken to the Smart Factory. If the lite is still supposedly being processed on a machine, then
you also have to check there whether this is the case. If there was a machine breakdown and the lite
was simply removed from the machine without telling the Smart Factory about this, then the message
has to be repeated.

So that these problematic cases are detected, lites that are in the breakage pool should not simply be
re-optimized. Beforehand, there should be a validation by the Smart Factory. This is currently done
with the Dynopt Filler Client. It asks the MAPS Service to do this validation every 5 minutes. For this,
it queries the current breakage pool with all non-validated lites. The result of the validation can be
that the lite has no relevance for the Smart Factory; that the lite can be re-cut in the Smart Factory;
or that it cannot be re-cut.

The result is reported back to the breakage pool and to the controlling client (Dynopt Filler). The client
triggers a defect booking for the problem lites in the PDC. The status barcode for the defect booking
can be set via the XML configuration file of the DYNOPT Filler Client:
         <DynOptFiller DefectBarcode="500000020">




04.04.2025                             EN-INST-A+W Smart Factory.docx                                   57
Lites in the breakage pool (FEIN_TEILE.JOB = 10000) have after inserting in the field
FEIN_TEILE.MASCHINE2 the value 0. After the validation, the value for possible remakes >= 100000
(100000 + MASCHINE1) and for the problem lites the value is set to -1.
The A+W Realtime Optimizer has to be configured so that it only uses broken lites from the breakage
pool whose value for FEIN_TEILE.MASCHINE2 >= 100000. For this, the XOPTON.CFG in a DYNOPT
operation has to be adjusted as follows:

        [CutGo]
        BreakageMode=3
        BreakageSelection=N
        BDEBreakageSelection=Y
        InsertBreakageFeinteileRecord=N

In addition, the MZO ID of the permitted cutting table has to be stored in the following comma-
separated list since only broken lites of these tables are used.
        [BrokenSheetPool]
        MZOPhysId=110,120

So that rejected lites are detected, the field FEIN_TEILE.MASCHINE2 in the breakage pool (Designer
Technik) are visualized accordingly.

The entire breakage pool is validated with each run. If the problem with a rejected lite has been solved
in the meantime, the next validation will now accept this still-rejected remake.

Attention!
Updating of the data records in the breakage pool is done by the Planning.Detailed Service, which
uses the database field FEIN_TEILE.LASTMODZEIT for its write operations.

Since the SOA services only master the versioning to the millisecond, most time stamps in our Informix
database are created for 10ns precision, under some circumstances there may be
ObjectStateExceptions when writing the results.
When updating the data, the program determines technically correctly but practically completely
unusably that the time stamp in the database deviates from the own time stamp and 'someone has
probably changed the record in the meantime'.

To prevent this, the time stamp has to be adjusted to INFORMIX databases and in case of doubt,
corrected manually.
ALTER TABLE fein_teile MODIFY (lastmodzeit DATETIME YEAR TO
FRACTION(3) DEFAULT CURRENT NOT NULL);




04.04.2025                            EN-INST-A+W Smart Factory.docx                                 58
9 Structure of the timeline
The timeline in the SmartFactory corresponds to the sequence of how batches were transferred to
the SmartFactory. A particularity are batches that have a rush flag (POOL_LAUF.Prioritaet > 0). These
are arranged in the timeline so that they are begun immediately.
With the release of the batches and any accrued backlogs, a pipeline forms, which depending on the
machine ties up capacity and has to be worked through before the machine is free for the next
batches.




Figure 9-1 Time horizon



The time horizon describes how many batches can be planned in production. The size of the time
horizon can be configured freely and represents a quantity of work in time. A next batch is only begun
if its work quantity and pipeline fit in the time horizon.
In order to express that backlog and already-begun batches for the future cannot be processed with
the same efficiency as planned, an efficiency can be specified for the processing. If the backlog can
only be processed with an efficiency of 50%, then one hour work on the pipeline means 2 hours time
occupied in the time horizon.

A batch that is larger than the maximum time horizon cannot be released for production and would
(temporarily) block production. This effect can be eliminated with a last-minute extension of the
TimeHorizon. In the medium term (end of 2021), it is planned to create possibilities for the easy
shifting of batches on the timeline.

The DYNOPT Filler Client release batches to the SmartFactory according to this method.




04.04.2025                           EN-INST-A+W Smart Factory.docx                                59
10 User interface
10.1 Call dialogs
The call dialogs are opened via the Production Terminal on the stations in question. If no
data can be called up, you will see a message:




10.1.1 Status descriptions
Batch status is displayed in different colors; furthermore, the currently selected batch is highlighted:




 Status                            Description
 Can be called                     All of the lites to be called up for the batch are present
 Can be called (remakes            All missing lites are remakes, some lites are in the buffer
 missing)
 In the inlet                      At least one non-remake lite is missing
 Wait for remake                   No lites in the buffer, all missing are remakes
 Call active                       The batch is being called



10.1.2 General batch information
This data is provided by the MapsService:
 Column                   Description
 Batch                    Batch number
 Rack                     Rack number (outwall, hidden in IG)
 Prio                     Batch priority normal or high
 FE                       MoveToFastestExit active
 Total                    Total number of lites


04.04.2025                            EN-INST-A+W Smart Factory.docx                                  60
 Complete                      Produced lites
 In the buffer                 Lites current in the buffer
 Missing                       Lites that are not in the buffer
 Supply                        Number of supply lites
 Status                        Batch status

Additional data can be called up via SQL and displayed. In the "options.cs" file of the
station, it is possible to generate a statement with the variable "SQLForAdditionalMain"
that provides additional information (e.g. fill corners in FPG, TPS).
The following example adds the production date as "ProdDate" column, the customer
name as "Customer" column, and the delivery date as "DeliveryDate" column:
public static readonly string SQLForAdditionalMain = @"SELECT distinct Cast(Cast(ft.lauf as varchar(10)) + '/' +
Cast(ft.bock as varchar(10)) as varchar(30)) as ControlId, pl.prod_termin, 104) as ProdDate, pa.kunde_name1 as
Customer, pa.objnr as Object, convert(varchar(10), pa.lief_term, 104) as DeliveryDate

      FROM pool_teile pt, pool_auftrag pa, pool_lauf pl, fein_teile ft

      WHERE pt.auftnr = pa.auftnr and pt.lauf = pl.lauf

      AND pt.lauf = ft.lauf

      AND ft.lauf in ({0}) and ft.bock in({1})

      GROUP BY ft.lauf, ft.bock, pt.lauf, pl.prod_termin, pa.kunde_name1, pa.objnr, pa.lief_term

      ORDER BY pt.lauf"

Important to note is that the first results colum is defined as "ControlId" and configured
according to the station (out: batch/rack, IG: batch). This is required in order to be able to
assign the data on the dialog.
Furthermore, a distinction must be made between SQL Server and Informix.




04.04.2025                                       EN-INST-A+W Smart Factory.docx                                    61
10.1.2.1 Cancel
By default, batches with canceled lites/units are not displayed in Production Terminal or
called up via the call dialog. Such batches can be recognized because after the call, they
are still on the list and have lites in the buffer:




Furthermore, there is a trace entry per lite:


In order to call up batches with canceled lites/units, a setting on the Production Terminal
menu is required:




The setting is not saved when you exit!
Furthermore, it is necessary to activate the options "Allow incomplete units" and "Allow incomplete
batches" on the Options menu:




Then the call can be made and the canceled lites are displayed in yellow:



04.04.2025                           EN-INST-A+W Smart Factory.docx                              62
The lites can be moved from the buffer with "Produce" and have to be removed manually after that.




04.04.2025                         EN-INST-A+W Smart Factory.docx                              63
10.2 Supply dialogs
The dialogs for setting supply lites are opened via the Production Terminal on the stations in question:
10.2.1 Supply SortJet 1/2
In the overview, the available batches are displayed sorted in ascending order by time stamp:




The following statuses are possible:
 Status                            Description
 Can be called                     All lites are in the buffer and can be produced via the Call-up
                                   dialog (a batch with this status should not be visible on the
                                   Supply dialog)
 Ready to reserve                  The supply lites can be reserved and set via the PT
 Not ready to reserve              Some lites are not ready to reserve
 Being processed                   The reservation in the Maps service is active

Using the button with the arrow, the detail view of the lites missing in the batch can be opened:




Only batches with the status "ready to reserve" can be transferred to the Maps service with a click on
"set selected group". The dialog is then closed and can be opened again to check the status again.
The status of the batch then changes to "Being processed". A successfully reserved batch receives the
status "reserved".




04.04.2025                            EN-INST-A+W Smart Factory.docx                                 64
The associated supply lites are then visible in the Production Terminal and can be selected
individually and set with "Produce":




04.04.2025                           EN-INST-A+W Smart Factory.docx                           65
11 PDC connection to the A+W Smart Factory
There it not a Smart Factory client at every point. If at such a point the Smart Factory needs
information about the progress, this can be done with the PDC in A+W Production. This must be
activated explicitly in the PDC master data.

Prerequisite in the SmartFactory is a ticket. A registration point can be assigned an agent. If a lite is
booked to this registration point via the PDC, then the Smart Factory will set the associated ticket to
the configured ticket status if the status is less than and the lite is in the Smart Factory (not broken or
outside it).

For this, there must be a corresponding entry with the agent ("MAPS_AGENTS") and its Guid value as
FK attached in the table "MAPS_BOOKINGACTIONS". In addition to the third-party key, the values
RegistrationPoint and Status must be filled. The first column gets the corresponding registration point,
where the action should be performed and the latter the corresponding ticket status. It is possible to
specify several ticket stati for a registration point. These are then executed in ascending order.

This function may not be activated on an agent that depends directly on the automation and has a
client that controls it. If this happens nevertheless, chaos may arise in the automation due to the PDC
messages as ticket updates are then executed in parallel.

The PDC messages can be issued by all common tools. The booking service sends all messages to the
Smart Factory, which then decides whether or not the message can be ignored. If the Smart Factory
cannot be reached, this message is lost.

The following PDC messages are currently processed by the Smart Factory:
    • Registration point bookings
            o Label number of the lite
    • Packed/sent bookings
            o Order item
    • Breakage reports
            o Label number of the lite
    • Prolonging bookings
            o Label number of the lite
    • Re-use bookings
            o Label number of the lite

In case of breakage messages by the PDC, it is also possible that a lite already archived can be
"activated" again and then the ticket chain reported broken in the Smart Factory. For this, if necessary
there is a look at the canceled/archived tickets in the database, and if there are tickets for a barcode,
then these are restored. For this, it is noted that a ticket is archived as soon as there is a packed or
sent booking in the PDC (see also chapter 12.1). Now it is ensured that late breakage messages trigger
an automatic remake or new production in the Smart Factory.


Prolonging bookings can be used to "extend" the ticket chain of a lite. An application case for this
is the breakage report of subelements in a component (IGU, for example) or the reuse of a



04.04.2025                             EN-INST-A+W Smart Factory.docx                                   66
subelement. This way, lites with, e.g., a scratch can be reported broken and reusable lites can be
put back into a Sortjet via supply via "prolonging".



11.1 Ticket cancellation/archiving in the SmartFactory
For the cancellation/archiving of a ticket, first the following SmartFactory options must be set in the
A+W master data:




                       Figure 11-1: Parameter setting for the PDC for extension of a ticket




04.04.2025                              EN-INST-A+W Smart Factory.docx                               67
                  Figure 11-2: Parameter settings for the AlcimServer for the archiving of a ticket

The deletion of a ticket in the SmartFactory is divided into two steps:
    1. Cancellation/archiving of a ticket
    2. Deletion of a ticket

The first step is triggered if the PDC transmits a corresponding packed or sent message for an order
item to the SMF. Then the corresponding tickets are "cancelled" or the archiving flag (table
Maps_Tickets.ArchiveStatus) is set to 1 and the tickets are removed internally by their respective
Maps agents. Now these tickets are no longer "recognized" in the SmartFactory; at the same time,
however, they are still present in the database.

The 2nd step is triggered if the AlcimServer archives the corresponding production run in A+W
Production. This is also transmitted to the SmartFactory and through this the deletion of the
corresponding orders is initiated. Through this AlcimServer archiving, tickets are finally removed
from the database.




04.04.2025                               EN-INST-A+W Smart Factory.docx                               68

