---
title: "EN-CONFIG-AW_Production_1"
source: "EN-CONFIG-AW_Production_1.pdf"
tags: ["A+W Production", "Software Configuration", "Glass Manufacturing", "Scheduling", "Crystal Reports", "Batch Release", "Technical Manual", "ERP", "A+W Software"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is an internal configuration manual for the A+W Production software, a solution designed for the glass industry. It provides detailed instructions on setting up and managing various production-related modules and functions."
long_description: "This is a comprehensive technical guide for the configuration of the A+W Production software system. Intended for internal use by system administrators and technical staff, it details the setup, functionality, and customization of key components. The manual covers a wide range of topics, starting with a detailed change history tracking versions from 1.0 to 1.72. Core sections include instructions on scheduling (Orders4Production), rough scheduling with features like FIX filters, batch release management, and generating reports using Crystal Reports. It also provides in-depth guidance on handling surplus quantities, remake handling, and configuring various production terminals (e.g., TG-In, LG-Assembly, IG-Out). Advanced functions such as multi-site configuration, data archiving, and integration with A+W IoT Smart Trace are also explained. The document serves as a central reference for ensuring the A+W Production environment is correctly configured to meet specific operational requirements in glass manufacturing."
---

# A+W Configuration: A+W Production

This is an internal document for A+W - Software for Glass.

---
## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2018-05-11 | DLA | Macro resolution, FIX filter | 1.0 |
| 2018-06-07 | DLA | CrystalReports | 1.1 |
| 2018-06-11 | JMO | O4P | 1.2 |
| 2018-06-12 | JMO | Extension O4P – SPCall | 1.3 |
| 2018-07-30 | DLA | Configure sketch | 1.4 |
| 2018-08-02 | DLA | Reports chapter | 1.5 |
| 2018-06-12 | DLA | Release of several instances/furnace bed optis | 1.6 |
| 2018-08-10 | PK | Foil preview in the PT LG_Assembly | 1.7 |
| 2018-09-21 | DLA | VIEWS + AWPLogoTableEditor | 1.8 |
| 2018-09-27 | DLA | Release with cancelled items | 1.9 |
| 2018-09-27 | DLA | AUW functions | 1.10 |
| 2018-10-08 | DLA | Existing English texts translated back to German | 1.11 |
| 2018-10-08 | DLA | Document links | 1.12 |
| 2019-02-06 | RI | Background printing in booking | 1.13 |
| 2019-02-08 | DLA | Multi-site | 1.14 |
| 2019-02-19 | JMO | Update and new prerequisite label for capacity | 1.15 |
| 2019-02-22 | DLA | Adjustments print booking | 1.16 |
| 2019-04-05 | DLA | Cancellation of orders | 1.17 |
| 2019-05-07 | JMO | PrintMode feature added | 1.18 |
| 2019-05-08 | DLA | Parameter Administrator | 1.19 |
| 2019-05-16 | RI | Specifying environment for scripts and reports | 1.20 |
| 2019-05-31 | DLA | Archiving | 1.21 |
| 2019-07-29 | SFR | Section 6.3. Opening the A+W Production Terminal QA with [F1] | 1.22 |
| 2019-08-12 | SFR, OSO | Merge IoT configuration instructions into this document (IoT Smart Trace basic configuration) | 1.23 |
| 2019-08-20 | SFR | Restructuring of the subchapter for A+W Production Terminal, new: PT order section Automatic Generation of a Batch Number | 1.24 |
| 2019-09-13 | SFR | New: Production Terminal IG-Out, section incorporating the LoadRackDialog | 1.25 |
| 2019-09-16 | SFR | New: A+W Realtime Optimizer, section Multiple User Login | 1.26 |
| 2019-09-20 | OSO | Barcoding area added | 1.27 |
| 2019-09-23 | SFR, STM | New: Filtering the display of the racks on the dialog by allowed tables | 1.28 |
| 2019-10-01 | SFR | Layout fine-tuning | 1.29 |
| 2019-10-01 | RI | Production Terminal IG-In – PMO data | 1.30 |
| 2019-10-09 | DLA | Resolve Makro Processing chapter broken down since in the previous version, the assignment of the titles to the individual chapters was not right. | 1.31 |
| 2019-10-14 | OSO | Scanner configuration added under A+W Production Terminal IG-IN | 1.32 |
| 2019-10-15 | OSO | Scanner configuration (optional) added under A+W Production Terminal IG-ASSEMBLY | 1.33 |
| 2019-10-15 | SFR | Replacement of the figures with English screenshots, formatting | 1.34 |
| 2019-10-17 | OSO | Addition of note the quality characteristic for Vipotron must be entered in apostrophes in the configuration | 1.35 |
| 2019-10-18 | OSO | Screenshot replaced for Figure 8-11 | 1.36 |
| 2019-10-21 | SFR | Transfer of PMO data to Production Terminal IG-In reworked and completed. | 1.37 |
| 2019-10-24 | OSO | Addition of the information the lot types must be specified for the various stations | 1.38 |
| 2019-10-29 | SFR | Reworking of the subsections for the Production Terminal IG-Out and IG-Assembly | 1.39 |
| 2019-11-01 | OSO | Addition of the area entry of additional quantities | 1.40 |
| 2019-11-04 | OSO | Addition of parts precise entry of additional quantities and entry of additional quantities in A+W Business | 1.41 |
| 2019-11-11 | SFR | Fine-tuning of Realtime Optimizer section | 1.42 |
| 2019-11-25 | SFR | Formatting of values in Production Terminal, specific and global | 1.43 |
| 2018-11-26 | PK | Reworking of the surplus and additional quantities | 1.44 |
| 2019-12-09 | STM | Part type filter in PT TG-In | 1.45 |
| 2019-12-16 | STM | Addition to rack feedback | 1.46 |
| 2020-01-30 | SFR | New section: checking of the rack for existence in the A+W Rack Manager | 1.47 |
| 2020-02-03 | OSO | Addition of configuration scanner connection to Production Terminal (8.1.5) | 1.48 |
| 2020-02-13 | OSO | Addition of A+W Production Terminal Processing | 1.49 |
| 2020-03-19 | STM | SP for turning in PT IG-In | 1.50 |
| 2020-04-30 | PK | Installation after ERP item | 1.51 |
| 2020-05-28 | OSO | Addition reporting from goods receipt | 1.52 |
| 2020-06-03 | OSO | Addition SN driver call for each lite | 1.53 |
| 2020-07-21 | PK | Automatic archiving | 1.54 |
| 2020-07-24 | STM | Display of additional parts in Production Terminal | 1.55 |
| 2020-09-23 | PK | Performance Counter | 1.56 |
| 2020-10-19 | PK | Break with incomplete installed message | 1.57 |
| 2020-11-30 | STM | Production Terminal TG-Out with several scanners | 1.58 |
| 2021-01-28 | DLA | Archiving of SKIZZEN | 1.59 |
| 2021-02-23 | PK | Expanded archiving | 1.60 |
| 2021-02-23 | PK | Archiving via customizing | 1.61 |
| 2021-03-24 | STM | Addition to the Performance Counter | 1.62 |
| 2021-04-27 | RI | Production Terminal Tracing | 1.63 |
| 2021-07-07 | STM | Rack feedback extended workbench | 1.64 |
| 2022-05-23 | STM | Timestamp of bookings | 1.65 |
| 2023-10-02 | STM | Messages to the Smart Factory | 1.66 |
| 2023-11-09 | STM | Remake handling | 1.67 |
| 2024-01-02 | EB | Production monitor (document content from market solution) | 1.68 |
| 2024-01-03 | EB | Chapter A+W Capacity (document content from market solution) | 1.69 |
| 2024-01-03 | EB | Scheduling remakes (document content from market solution) | 1.70 |
| 2024-04-03 | JMO | O4P worksteps "AfterWorks" and "AfterWorksParallel" added. | 1.71 |
| 2024-04-25 | JMO | Late transfer of production-irrelevant data | 1.72 |

## 1. Scheduling
Currently there are two scheduling variants since a newer version should replace the previous Items4Alcim (14A). The newer scheduling variant Orders4Production (O4P) will be discussed primarily below.

### 1.1. Orders4Production
In contrast to Items4Alcim, Orders4Production no longer works in item-oriented fashion, but rather order-based. Furthermore, the scheduling is taken apart into individual work steps. If a work step has completely processed an order, the next work step comes and processes it.

The sequence of the work steps can be configured. Some basic rules of sequence are checked programmatically and, in case of non-adherence, cause the stopping of the scheduling. Thus, for example, the Capa may not be run through before the MA. This also makes sense because the machines are not previously assigned and therefore, no capacities can be booked.

*Figure 1-1 Parameter administrator: specification of the sequences in O4P*
```
Parameter administrator [JM]
Parameter: A-W Production, Barcoding booking service, BreakagePool dialogue, Capacity Planning, Data import (Infos4Alcim), Data Import (Items4Alcim), Detailed scheduling, Former Data Import (ALCIMPRT), General, Machinery allocation, Order import (Orders4Production), Production monitor, Reassignment, Release dialogue, Rough scheduling, Scheduling Remake Dialogue, A+W Production Terminal
Station ID: 65, 0
Activation of SOA import
Settings: Sequence to import quotations, Sequence to import orders, Sequence for cost calculation, Sequence for reservations, Sequence for late takeover of production irrelevant data
Value: Enumerate; 1, SNCreation; 4, CheckUp1; 1, BomConfigura..
Value: Enumerate: 1. SNCreation: 4. CheckUp 1: 1. BomConfigurator
Value: Enumerate, 1, CheckUp1, 1, BomConfigurator, 1, CheckUp2;
Value: Change: 1
Description: Here you can define the sequence and the number of threads of the individual worksteps for a quotation. Note: Some worksteps may only be executed by one thread (e.g. Capacity, Machinery Allocation...). And, the sequence must meet certain conditions (e.g. Capacity after Machinery Allocation....).
Existing worksteps:
-AlcimWorks (calculation of edge allowances).
-Assignment (allocations).
AWDesign (creation of muntin file).
-BasicScript (execution of individual BasicScripts).
-BomConfigurator (BOM configurator for A-W Production BOM).
-Capacity (A+W Capacity Planning).
CheckUp1 (intermal check module, should always be enabled).
-CheckUp2 based on BOM configurator (see CheckUp1).
Enumerate (part numbering).
-GrindArea (edge deletion),
Label (assignment of label numbers).
-MachineryAllocation (Machinery Allocation).
-Resolve MacroProcessing (resolve macro processing steps from SN)
SNCreation (SN creation).
SPCall (execution of individual Stored Procedures).
Range: ORDERS4PRODUCTION_SETTINGS
Entry: SEQUENCE_OF_EXECUTION_OFFER
```
In the parameter administrator (Fig. 1.1), you can also see that the sequences for orders, quotations, reservation, and calculations can be specified individually. This creates additional flexibility.

Below, the focus is on the set-up of the O4P and the description of the individual possible WorkSteps.

#### 1.1.1. Set-up
If an import "Items4Alcim" is already configured, then nothing further has to be configured. The sequences of the WorkSteps are initially pre-assigned from the standard database or initialized by a DB script (awupdate_alcim_2_593.xml). The other switches are identical to those from I4A.
Then during use of the import SPs, the SPs may have to be adjusted. See section "1.1.2.16 SPCall."

### 1.1.2. Description of the work step
As already explained, the entire scheduling process is divided into individual work steps, which can be run through in nearly any order. Some work steps can be omitted completely if they are not necessary in a project or only for particular order types.

There are two work steps that cannot be configured. Thus each scheduling begins internally with a "WorkStepStart" and each scheduling ends with a work step "WorkStepEnd“.

Behind the work steps is a comma-separated number. This number specifies how often this work step may be present within the scheduling process. If the number is greater than 1, then two orders can be processed simultaneously in this step. Thus it is possible that an order can "overtake" another within the processing chain. However, this possibility does not exist for all work steps and furthermore, with use of too many WorkSteps and thus too few CPU cores, there can be performance issue. Here, you must experiment to get the best results. No general statement can be made since there are too many configurable options and external dependencies.

#### 1.1.2.1. WorkStepStart (internal)
Here the data of the OrderXML structure is taken over into the memory and checked roughly. It is also checked whether the order is already in the database and the data is then loaded. Similarly, it is checked whether the order is in the manual NR and with which NR decision the re-import should take place.

#### 1.1.2.2. AlcimWorks
This work step calculates the edge surcharges, processes the SN file, and generates images for the sketches.

This work step can be run in parallel, edited, but always only one item of all available orders at a time.

Before this work step, the steps "MachineryAllocation", "Enumerate" and "CheckUp1" must have been run through.

#### 1.1.2.3. AfterWorks
**Prerequisite**
The work step "AlcimWorks" must have been run already.

**Description**
The work step can perform different tasks.
a) Set-up edge detection

Machines can be selected for the set-up edge selection in the machine allocation.
If machines are selected here in "Lines", the SP that was configured under "Afterworks SP" is called, which should then determine the set-up edge.

b) Transport edge detection or validation
If no lines are configured as under a), then the work step takes over the transport edge detection if machines were stored in "Transport Systems" according to the machine allocation.

*Parameter-Administrator [JM]*
```
Parameter: A+W Production, Allgemein, Auftragsimport (Orders4Produc, AV-Nachläufer-Dialog, BDE-Buchungsdienst, BruchPool-Dialog, Datenübernahme (Infos4Alcim), Datenübernahme (Items4Alcim), Datenübernahme alt (ALCIMPR, Feinplanung, Freigabe-Dialog, Grobplanung, Kapazitätsplanung, Kontinuierliches Schneiden, Maschinenzuordung, Produktionsmonitor, Umlastung, A+W Production Terminal
Filter: Routen, Sondereinstellungen, Stammdatenstruktur, Transportsysteme
Routen:
Verwendung von Laufweg: 0
Verwendung von BearbFolge: 0
Kettenbildung Laufweg: 1
Kettenbildung Bearbeitungen: 1
Sondereinstellungen:
Folgetechnologie bestimmen: 0
Folgetechnologie nach Sondertextnumme: 5
Aufstellkanten bestimmen: 0
Produktionstermine berechnen: 0
Lagerplattenprüfung: 1
Transportsysteme: 1620
Linien:
Behandlung von freien Formen als Rechte: 0
Vermaßungstyp für Logo-Bearbeitung: 0
Afterworks-SP
Stammdatenstruktur:
Import: 0
Modus: 1
Transportsysteme: Aufzählung der Transportsysteme (ID_PHYS) für die Transportkantenbestimmung während der Einlastung im Workstep 'AfterWorks'
Bereich: MZO FILTER
Eintrag: TRANSPORTSYSTEME
Typ: PropertiesMZO
Name: MZO_FILTER_TRANSPORTSYSTEME
```
The results are written in `mzo_aufsttellkante`.

c) Takeover of the geometry data from the CADSheetsService
All production data (incl. cutting) is transmitted to the CADSheetsService.
This part is always executed by the "AfterWorks" work step.

For the transport edge detection, the machine allocation (MZO.dll) is used. It can only ever make one calculation at a time. If several threads are configured for the "AfterWorks" work step, all threads that share this possibility must be executed one after another.

Furthermore, the machine allocation is also used by the machine allocation (MZO.dll). With this work step, the AfterWorks must also share the use of the machine allocation.

Remedy: => "MachineryAllocation2" or "MachineryAllocationParallel" and "AfterWorksParallel"

#### 1.1.2.4. After Works Parallel
(available starting with the QR, which follows QR2403)

The content of this work step is identical to the "AfterWorksParallel" work step.
However, this, if the transport edge detection was configured, generates several instances of the machine allocation (MZO.dll) in an individual process ("Albwir.Alcim.MAPipeServer.exe"). This way, as many processes are generated as the system has CPU kernels. The items of an order are then distributed evenly to the processes, which means that an individual order can be processed much faster.
It must be noted that the work step "MachineryAllocationParallel" works with the same principle. If both work steps are configured, "MachineryAllocationParallel" and "AfterWorksParallel" must share the instances of the MZO.dll.

**Assignment**
In this work step, the familiar assignments are made.
This work step can be run in parallel.

**AWDesign**
This work step is familiar in I4A as CustomizingStep AWDesign. The AWD files are generated here.
This work step can be run in parallel.
Before this work step, the steps "Enumerate", "CheckUp1" and "CheckUp2" must have been run through.

**BasicScript**
This work step must be included if a basic script should be executed for customizing purposes.
This work step can be run in parallel.

**BomConfigurator**
Here, the actions of the parts tree configurator are executed for deleting/adding parts/processings.
During use it must be noted that the order is not yet in the database at this point in time, so that no formulas with SQL statements will work. (analogous to I4A)
This work step can be run in parallel.
Before the work step, the "CheckUp1" step must have been run through.

**Capacity**
Execution of the A+W Capacity Planner.
This work step can be run in parallel, edited, but nevertheless always only order at a time.
Before this work step, the steps "Enumerate", "CheckUp1", "Label", and "MachineryAllocation" must have been run through.

**CheckUp1**
After loading the OrderXML structure, this modules takes care of the isolation of additional properties, creation of new items in the master data, synchronization of the data, and verification of the parts tree.
This work step can be run in parallel.

**CheckUp2**
After execution of the BOMConfigurator, it may be necessary to repeat CheckUp1 with the manipulated parts tree.
This work step can be run in parallel.
Before this work step, the steps "Enumerate", "CheckUp1" and "BOMConfigurator" steps must have been run through.

**Enumerate**
Executes the parts numbering, for which there are currently three modes. See also I1A in the parameter administrator.
This work step can be run in parallel and may exist multiple times.

**GrindArea**
This work step executes the decoating module.
This work step can be run in parallel.
Before this work step, the "Enumerate", "CheckUp1" and "MachineryAllocation" steps must have been run through.

**Label**
The labeling is done here.
This work step can be run in parallel.
Before this work step, the "Enumerate", "CheckUp1" and "CheckUp2" steps must have been run through.

**MachineryAllocation**
An elementary component is the machine allocation, which is executed with this work step.
The results are not yet available in the database after execution; instead, they are placed in the memory.
This work step can be run in parallel, but always only one item of all available orders at a time is processed.
Before this work step, the "Enumerate" and "CheckUp1" steps must have been run through.

**Resolve MacroProcessings**
Additional function for resolving a macro processing into individual processings. A detailed description of this function is in a separate chapter in this document.
This work step can be run in parallel and may exist multiple times.

**SNCreation**
The module automatically generates SN files for the A+W CAD Designer (shapes) taking the OrderXML files into consideration.
This work step can be run in parallel and may exist multiple times.

**SPCall**
In this step, the familiar SPs cu_prt_itemwrt, cu_prt_ordwrt, and cu_mzo_extended are executed.
CAUTION: To be noted here is that the data in this work step is temporarily written with a negative order number. If you use this order number in the SP, in order to determine an order number range, for example, the SP must be adjusted after change from I4A to O4P!

**WorkStepEnd (internal)**
In the last step, with successful scheduling, the results are written to the database, the PDC initialization is started, and the report to the ERP is sent.
In case of errors during scheduling, the error message is reported to the ERP and the table POOL_IMPORT is updated for manual NR

### 1.1.3. ResolveMacroProcessings
This document describes the function for resolving macro processings into their part processings in A+W Production (#414206).

Background, a macro processing is a combination of various processings, e.g. a drilling and a cut-out. What precisely is included in the macro is not visible. The various processings in a macro cannot be scheduled on different machines. A statistical evaluation is also difficult to perform. This function was developed so that this is possible.

The O4P scheduling and a SN drawing of the item are the prerequisites for this function. If it is active, a macro is taken apart into its part processings. For each part processing, a processing based on our A+W processing type catalog is generated in the BOM. If for the A+W processing types included, there is no appropriate processing in the master data, the item gets stuck in the manual re-working and cannot be scheduled.

This function is available again starting with A+W Production Version 6.4 with database version 2.611.

**Configuration**
In O4P, the new work step ResolveMacroProcessing must be entered for the scheduling of orders and reservations next to the work step CheckUp2.

*Figure 1-2 Parameter administrator: Specification of the sequences in O4P - example of ResolveMacroProcessing*
```
String Collection Editor:
Enter the strings in the collection (one per line):
Enumerate; 1
AWDesign: 1
SNCreation: 1
Check Up 1; 1
BomConfigurator: 1
Assignment: 1
Check Up2; 1
Resolve Macro Processing: 1
Label: 1
Machinery Allocation: 1
Capacity: 1
Alcim Works: 1
GridArea: 1
SPCall; 1
```
In the processing master data, there must be at least one processing for each A+W processing type. If there are several processings, one must be selected. In order to assign this processing to the A+W processing type, a SQL editor is required since there is no user dialog yet.

The table `AW_BEARBTYPEN` has been expanded to include the field `STANDARD_ARTNR`. The processing item number belonging to the A+W processing type must be entered in this field. This processing item must exist in the A+W Production master data.
```sql
SELECT aw_bearbtyp, standard_artnr, * FROM aw_bearbtypen ORDER BY 1;
UPDATE aw_bearbtypen SET standard_artnr = ? WHERE aw_bearbtyp = ?;
```
After a restart of the scheduling, this feature is active.

> **Caution**: if new processings and processing types are created, it must be ensured that these can also be scheduled in the MA on appropriate machines. New processing types (not A+W processing types) must also be assigned to a batch type for detailed scheduling.

**Result**
If a macro is resolved it can be detected in the table `POOL_BEARBEIT`. There are 2 new fields: `MAKRO_AUFGELOEST` and `MAKRO_REFERENZ`.

If the field is `MAKRO_AUFGELOEST > 0`, then this is a macro processing that was resolved. Then there is at least one new part processing with which the field `MAKRO_REFERENZ` is filled with the number from `MAKRO_AUFGELOEST` of the macro processing.

The `SEQUENZ` of the newly generated part processings corresponds to the `SEQUENZ` of the macro processing. Which of the part processings is done first cannot be determined. These part processings can be traced via the PDC. Reports are made via the macro processings since the part processings are unknown in the ERP system.

Resolved macro processings are not loaded in the detailed scheduling and can thus not form lots.

**Characteristics**
Macros can contain cut-outs that cannot be described as A+W standard cut-outs. (Notched corner(1300), notch(1400), inner cut-out(1405, 1415)). New A+W processing types were defined: general notched corner (1303), general notch (1403), and general inner cut-out (1418). If a processing cannot be described by the previous types, the new A+W processing types are stored. In the parameters for these processing types, the size of the notch and the minimum rounding radius are returned. These values can be used for machine allocation.

These new A+W processing types cannot be entered via our ERP systems since you cannot generate an SN drawing using these types.

**Display in rough scheduling**
In the rough scheduling displays, you don't always want to see processings of resolved macros. You can achieve this by filtering these processings in the displays. For this, there is a FIX filter `AUW_FIX_NO_RESOLVE_MACRO` that is active in our default displays.

These processings can also be filtered on the Production Monitor if the display is controlled via the VIEW `AUW_CAPA_OVERVIEW`. For this, there is a new `AUW_SETTINGS` parameter `[CAPA_VIEW/SHOW_RESOLVED_MACROS]`, which is used to control the VIEW.

## 1.2. Cancellation of orders
Orders can be cancelled via the scheduling. For this, the ERP systems write an OrderXML file with a cancellation flag. This way, it is currently only possible to cancel entire orders, cancellation of individual items is not possible.

The behavior described here also corresponds to the behavior via a cancellation via the PPS WebService.

The entire order is cancelled, but the items behave differently depending on their status. The same for all items is that the cancellation flag is set (AUFTKZ = 1).

If an order is in the POOL, in a pot or in a roughly scheduled batch, then this order is automatically moved to the cancellation pot (12600). A now-empty batch or pot is resolved.

If the item is roughly scheduled in a batch with a greater status, then nothing further happens with the order. It is cancelled and the other applications react to this cancellation flag. If a cancelled lite is read on an A+W Production Terminal, an appropriate message appears there. If the lite was in a finely scheduled batch when it was cancelled, there will be a warning on the release of the batch, so that this item can be removed and deleted from the batch if necessary.

If an item was planned in a package optimization, in the manual follow-up, there is a message about this cancellation. The message can be confirmed, the removal from a package optimization must be done manually by the user.

## 1.3. Later transfer of production-irrelevant data
It is now possible to take over changes to certain data from the ERP even after planning.

Generally, this is the following data:
- Delivery date
- Customer data
- Delivery address
- Route
- File attachment with identifier for production transfer
- Order/item texts with identifier for production transfer
- Commission data
- Customer item

Such a transfer of the data is done in the OrderXML file with the ordering type "ChangeProduce" or "ChangeOffer".

Meanwhile, the identification of the ordering type is possible down to the item level. The identifier exists once on the order level and once for each item.

In this context, the ordering type "NoChange" was also introduced. Items marked this way remain untouched in the import. This helps save time.

Meanwhile, it is also possible to transfer an OrderXML file with mixed ordering types.

Here, however, the rule applies that an order that consists only of "ChangeProduce" or "NoChange" items is treated completely as a "ChangeProduce" order. Similarly, a "ChangeProduce" order that consists only of normal "Produce" and "NoChange" items is treated as a normal "Produce" order.

On transfer of a complete "NoChange" order, no data is changed. Here it is not important which identifier the item contains.

### 1.3.1. Changing order data
a) **Takeover of the delivery date and route**
Generally, the delivery date is taken over from the OrderXML from the UDX.AW.ORDER-INFOS. There is tag delivery there.

e.g.:
```xml
<Delivery tour="2" description="Tour Nord / Route North" deliveryDay="2023-09-
30T00:00:00" enrouteDate="2023-09-30T08:00:00" requestedDeliveryDay="2023-09-
30T00:00:00" calendarWeek="201920" />
```
Here, the `deliveryDay`, `enrouteDate`, `description` and `tour` are read out. The following database fields are thus updated:
- `deliveryDay` => `pool_auftrag.lief_term`
- `enrouteDate` => `pool_auftrag.fahr_term`
- `description` => `pool_auftrag.tour_info`
- `tour` => `pool_auftrag.tour`

However, this only happens under the condition that the new delivery date is in the future and should take place later than the original delivery date.

However, this condition can be cancelled with the switch `ITEMS4ALCIM_SPECIAL/ALLOW_LATE_POSTPONE_TO_PAST`. The switch is in the Parameter Administrator under `A+W Production > Order Import > Late Takeover of Production-Relevant Data > Allow Delivery Date Change in the Past`.

*Figure 1-3: ALLOW_LATE_POSTPONE_TO_PAST*
```
Parameter-Administrator [JM]
Setting: Erlaube Lieferterminverschiebung in die Vergangenheit
Description: Bei der späten Übergabe produktionsirrelevanter Daten ist standardmäßig eine Lieferterminverschiebung in die Vergangenheit nicht möglich. Dieser Schalter bewirkt. dass auch Termine in der Vergangenheit akzeptiert werden.
0: Der früheste akzeptierte Liefertermin wäre der aktuelle Zeitpunkt.
1: Jeder Liefertermin wird akzeptiert.
Erlaubte Werte: 0, 1
Standardwert: 0
Bereich: ITEMS4ALCIM SPECIAL
Eintrag: ALLOW_LATE_POSTPONE_TO_PAST
Typ: Properties Order4Production
Name: ALLOW_LATE_POSTPONE_TO_PAST
```

b) **Takeover of order documents**
Order documents are transferred in the OrderXML_Datei in `UDX.AW.ORDERINFOS > Attachements`. These are then compared to the existing documents in `pool_dokumente` and added if necessary.

c) **Takeover of order texts**
Order texts are transferred in the OrderXML file in the `UDX.AW.ORDERINFOS > CUSTOMER REFERENCES` and in `ProcessPlanning`. These are then compared to the existing documents in `pool_txt` and added if necessary.

d) **Takeover of customer data**
Here a whole series of data is taken over. The data is in the OrderXML under `ORDER_HEADER > ORDER INFO > ORDER PARTIES > BUYER PARTY`
- Customer number: `PARTY ID` => `pool_auftrag.kunde_nr`
- Name: `NAME` => `pool_auftrag.kunde_name1`
- Name2: `NAME2` => `pool_auftrag.kunde_name2`
- Name3: `NAME 3` => `pool_auftrag.kunde_name3`
- PLZ (Postfach): `ZIPBOX` => `pool_auftrag.kunde_plz_postfach`
- Postfach: `ΒΟΧΝΟ` => `pool_auftrag.kunde_postfach`
- Straße: `STREET` => `pool_auftrag.kunde_strasse`
- PLZ: `ZIP` => `pool_auftrag.kunde_plz_ort`
- Ort: `CITY` => `pool_auftrag.kunde_ort`
- Landeskennung: `COUNTRY` => `pool_auftrag.kunde_landeskennung`
- Telefon: `PHONE` => `pool_auftrag.kunde_telefon`

e) **Takeover of shipping address**
The data for the shipping address is in the OrderXML under `ORDER_HEADER > ORDER INFO > ORDER PARTIES > DELIVERY PARTY`
- Name: `NAME` => `pool_auftrag.lief_name1`
- Name2: `NAME2` => `pool_auftrag.lief_name2`
- PLZ (Postfach): `ZIPBOX` => `pool_auftrag.lief_plz_postfach`
- Postfach: `ΒΟΧΝΟ` => `pool_auftrag.lief_postfach`
- Straße: `STREET` => `pool_auftrag.kunde_strasse`
- PLZ: `ZIP` => `pool_auftrag.lief_plz_ort`
- Ort: `CITY` => `pool_auftrag.lief_ort`
- Landeskennung: `COUNTRY` => `pool_auftrag.kunde_landeskennung`

### 1.3.2. Change of item data
a) **Takeover of item documents**
Item documents are transferred in the OrderXML_Datei in `UDX.AW > Attachements`. These are then compared to the existing documents in `pool_dokumente` and added if necessary.

b) **Takeover of item texts**
Item texts are transferred in the OrderXML file in the `UDX.AW > CUSTOMER REFERENCES` and in the `ADVICES` of the parts and processings. These are then compared to the existing item texts in `pool_txt` and added if necessary.
Here there is the particularity that texts with a configuring ID (`ADVICE > key`) can be ignored. E.g. if texts were generated by SPs and never transferred via the OrderXML file.
This happens in the Parameter Administrator in `A+W Production > Order Import > Late Transfer of Production-Irrelevant Data > Ignore Changes to Texts`

*Figure 1-4: IGNORE_TEXTCHANGES_IN_LATEORDERCHANGE*
```
Parameter-Administrator [JM]
Setting: Ignoriere Änderung an Texten
Description: Hier können Texttypen in einer kommaseparierten Liste angegeben werden, die bei der späten Übernahme produktionsirrelevanter Änderungen ignoriert werden sollen. Sind bestimmte Texttypen z. B. nicht in der Übergabedatei enthalten und durch eine SP im Import erzeugt worden, bleiben diese Texte erhalten.
Standardwert:
Bereich: ORDERS4PRODUCTION_SPECIAL
Eintrag: IGNORE_TEXTCHANGES_IN_LATEORDERCHANGE
Typ: Properties Order4Production
Name: IGNORE_TEXTCHANGES_IN_LATEORDERCHANGE
```

c) **Change of commission data**
This data is in the OrderXML file under `UDX.AW > Commission`.
The customer order from `CustomerLineItemID` and the texts from `ADVICES` are taken over.
The takeover of this data can be suppressed with the switch `ORDERS4PRODUCTION_SPECIAL/IGNORE_COMISSION_CHANGES`

*Figure 1-5: IGNORE_COMISSION_CHANGES*
```
Parameter-Administrator [JM]
Setting: Ignoriere Kommissionsänderungen
Description: Ist dieser Schalter aktiviert, werden bei der "späten Übernahme produktionsirrelevanter Daten" Änderungen an den Daten für die Kundenposition und Kundenkommission nicht übernommen.
0: Übernahme der Kundenposition und Kundenkommission (Standard)
1: keine Übernahme
Erlaubte Werte: 0, 1
Standardwert: 0
Bereich: ORDERS4PRODUCTION_SPECIAL
Eintrag: IGNORE_COMISSION_CHANGES
Typ: Properties Order4Production
Name: IGNORE_COMISSION_CHANGES
```
d) **Change of the item delivery date**
This date (in `pool_pos.lief_term`) is only changed with appropriate configuration. The switch for activation is in the Parameter Administrator under `A+W Production > Order Import > Late Takeover of Production-Irrelevant Data > Adjustment of Item Delivery Date`.
Here, the same order delivery date is written in the item (`pool_pos.lief_term`).

*Figure 1-6: CHANGE_POS_LIEFTERM*
```
Parameter-Administrator [JM]
Setting: Anpassung Positionsliefertermin
Description: Ist dieser Schalter aktiviert, werden bei der "Späten Übernahme produktionsirrelevanter Daten" nicht nur der Auftragsliefertermin übernommen, sondern dieser auch als Positionsliefertermin übernommen.
0: nur der Auftragsliefertermin wird übernommen
1: die Positionen erhalten den gleichen Liefertermin wie der Auftrag bei der "Späten Übernahme produktionsirrelevanter Daten"
Erlaubte Werte: 0, 1
Standardwert: 0
Bereich: ORDERS4PRODUCTION_SPECIAL
Eintrag: CHANGE_POS_LIEFTERM
Typ: Properties Order4Production
Name: CHANGE_POS_LIEFTERM
```

## 2. Rough Scheduling
### 2.1. FIX filter
Displaying a normal filter in the A+W Production POOL can be changed and saved for each station ID. A FIX filter is a filter that is linked directly to a view and cannot be changed.
For example, you might want to define a view only for IG units. Without a FIX filter, you must select an IG filter for each station; these can be taken away by the customer at any time and then will not display the IG units.

#### 2.1.1. How can a FIX filter be configured?
A FIX filter is defined like a normal filter. The type for which view a filter is defined is not important for a FIX filter.
The AUW standard FIX filters are not linked to any special type (`POOL_FILTER.VIEWS` is empty). This has the advantage that nobody sees the filter in the filter list and thus cannot change the behavior.

#### 2.1.2. How is a FIX filter linked to a display?
Currently, configuration is only possible with a SQL editor.
First the name of the filter to be used must be determined:
```sql
SELECT name, * FROM pool_filter;
```
The value from column `name` must be used in the view. For this, the main data record of the affected view must be determined in the database table `POOL_SORT` with the following SELECT:
```sql
SELECT sortiertyp, station, feldname, titel, sprache, def_filter FROM pool_sort WHERE rang = 0;
```
As soon as the view has been determined, insert the name of the filter in the `def_filter` field:
```sql
UPDATE pool_sort SET def_filter = '<name of FIX filter from table POOL_FILTER>' WHERE rang = 0 AND sortiertyp = '<view type>' AND station = '<station>' AND feldname = '<name of view>' AND sprache = '<Language of view>';
```

#### 2.1.3. How can you see that your FIX filter is active?
If a view is opened in A+W Production, you can only see starting with Version 5.4 from the displayed non-changeable filter name in the display that a FIX filter is active.

*Figure 2-1 Pool display - selected filters*
`AUW_FIX_IG`

#### 2.1.4. FIX filter for the standard displays
The names of the standard FIX filters begin with `AUW_FIX_`. These may not be changed. With an update since Version 5.3, they are inserted automatically with `awupdate_alcim_AUW_FIX_filter.xml` (database update tool) and overwritten.

#### 2.1.5. Known Problems
- A FIX filter is active, but not used. In the SQL instruction for the view, the filter is missing: since Version 5.4, a FIX filter definition with more than 127 characters is ignored → #332610

### 2.2. VIEW database for rough scheduling views
For the configuration of the rough scheduling views, it is not just possible to load data from tables. If information is missing, this can be determined via a VIEW database. Thus, for each usable table, there are 2 VIEWs in the database, which are available for selection during the configuration of the fields in the rough scheduling and also automatically in the A+W Production Terminal. The name of the VIEW consists of the table name and an abbreviation "AUW_" or "CUV_" in front of it.

Example for the table POOL_TEILE, there can be the following VIEWS: `CUV_POOL_TEILE` and `AUW_POOL_TEILE`.

The VIEWs with the abbreviation "AUW_" are created by development and may not be edited or created in the projects. If this should happen, they are overwritten automatically in case of an update.

In the project, VIEWs with the abbreviation "CUV_" can be created. These are individual for each customer installation.

Currently there are the following VIEWs in every installation: `AUW_POOL_TEILE` and `AUW_POOL_SZR`. The fields of these VIEWs are described in the database documentation.

*Figure 2-2 Field definition of the rough scheduling for fields from a VIEW*
```
Field Definition
Menu Group: Example VIEW
Menu Entry: Backcut
Column Title: Backcut
Description: Backcut
Format: Millimeter (1204)
Database Field: Open Selection
- AUW_POOL_SZR.RU
- AUW_BOM
- AUW_POOL_SZR
- AUFTNR
- KANTENINDIVIDUELL
- POS
- RAHMENSTAERKE
- RUECKSCHNITT1
- RUECKSCHNITT10
- RUECKSCHNITT11
```
An advantage of using a VIEW, you don't have to create a StoredProcedure in order to procure data. A VIEW works identically under SQLServer and INFORMIX. You can also use this VIEW like tables in a report.

### 2.3. Additional and surplus quantities
Additional or surplus quantities are necessary if for various reasons, production would like to start with a larger quantity than the customer has ordered. This larger quantity can be handled in different ways.

> **Caution**: The excess quantity dialog in A+W Production must not be used if the location-spanning PDC is used at the same time, as otherwise new label numbers would be generated which would not be known in all production locations.

#### 2.3.1. Commercial surplus
Commercial surplus and shortfall refers to a complete item. There is a minimum and a maximum quantity. Production of the maximum quantity is the goal. In case of a break, no remakes are done unless the quantity underruns the defined minimum.
Surpluses can be entered during the order entry or directly in A+W Production using a surplus editor. A+W Production reports the quantity produced to the ERP system (here, A+W Business)

*Figure 2-3 Commercial surplus*
