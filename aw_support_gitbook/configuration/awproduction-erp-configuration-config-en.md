---
title: "EN-CONFIG-A+W Production"
source: "EN-CONFIG-A+W Production.docx"
tags: ["A+W Production", "ERP", "Configuration", "Feedback", "Scheduling", "Rush Order", "Remake Handling", "Barcoding", "ALCIM", "A+W Cantor"]
version: "1.0"
last_updated: "2024-10-03"
short_description: "A technical configuration guide for the A+W Production software, detailing settings for order scheduling, rush orders, high-priority orders, and system feedback mechanisms. It covers integration with ERP systems, including fileless reporting, batch status updates, and rack allocation."
long_description: "This document, 'EN-CONFIG-A+W Production.docx,' serves as a detailed configuration manual for A+W Software GmbH's production management system. It outlines various switch positions and parameters that control the software's behavior in different scenarios, such as order scheduling, rush orders, and handling high-priority tasks. Key sections cover the logic for DD (Due Date) postponement, the use of a 'rush grid,' and how the system weighs costs to determine the most effective production path. The document provides in-depth information on the 'Feedback' module (Chapter 6), explaining the transition from file-based synchronization to a more streamlined, fileless reporting system. This includes the configuration of ALCIMBOOK services for reporting batch, production, and rack status directly to an ERP system. It details the necessary switches, parameters, and database tables (e.g., `ERP_RUECKMELDUNG`, `ERP_GEST_MELDUNG`) involved in this process. Furthermore, the guide explains how to configure remake handling for partial defects (Chapter 9), including the setup of PDC master data, status types, and parameter administrator dialogs. It also covers integrations with other A+W products like A+W Business, A+W Enterprise, and A+W Cantor, providing configuration steps for each."
---

---
### Switch DD postponement = YES, x days
### Switch use rush grid = NO

- Route date is known, for the scheduling, only the normal transitions (shifts + max. shifts) are drawn from the transition times.
- Program tries using the transition times and the flexible transition time to schedule without postponing the DD.
- If this does not succeed, then there is a postponement to the next possible DD if this is also in the range specified.
- Scheduling is only done in unlocked shifts and on bottleneck machines with free capacity in the shift.
- If this is not possible, then the order lands on the red card.

### Switch DD postponement = YES, x days
### Switch use rush grid = YES

- Route date is known, for the scheduling, only the normal transitions (shifts + max. shifts) and RUSH (shifts, max. shifts not relevant) are drawn from the transition times.
- Program tries using the transition times and the flexible transition time to schedule without postponing the DD.
- If this does not succeed, then there is a postponement to the next possible DD if this is also in the range specified.
- Both a conversion to rush grid, use of the flexible transition time, as well as a DD postponement are stored with internal costs.
- The program now weighs these internal costs and determines the most "cost-effective" way.
- Essentially, the program tries to place the rush grid at the start of the production chain.
- Scheduling is only done in unlocked (Version 5.5 to 6.1 also occupies shifts locked for normal orders, but this is an error) shifts and on bottleneck machines with free capacity in the shift.
- If this is not possible, then the order lands on the red card.
- Recommendation: Do not activate the use of the rush grid for normal orders.

## 5.1.2. Switch position rush order

### Switch DD postponement = NO
### Switch to rush grid = irrelevant since already rush order

- Route date is known, for the scheduling, both the normal and rush transitions are drawn from the transition times.
- Program tries using the transition times and the flexible transition time to schedule without postponing the DD.
- Here too, the program weighs between rush grid and flexible transition time.
- The specification is to maintain the DD.
- Scheduling is only done in unlocked shifts and shifts for rush orders and on bottleneck machines with free capacity in the shift.
- If this is not possible, then the order lands on the red card.

### Switch DD postponement = YES, x days
### Switch to rush grid = irrelevant since already rush order

- Route date is known, for the scheduling, both the normal and rush transitions are drawn from the transition times.
- Program tries using the transition times and the flexible transition time to schedule without postponing the DD.
- Here too, the program weighs between rush grid and flexible transition time.
- The specification is to maintain the DD.
- Scheduling is only done in unlocked shifts and shifts for rush orders and on bottleneck machines with free capacity in the shift.
- If the DD cannot be adhered to, then a new DD is determined, whereby this is already known to the system, as mentioned above.
- Now there is another calculation taking into account the "costs" for usage rush grid, flexible transition time, and DD postponement.
- Therefore, it is theoretically possible that not the next but the DD after the next is found, e.g., if the DD postponement is more "cost-effective" than the continuous use of rush transitions.
- If no DD is determined, then the order lands on the red card.

## 5.1.3. Switch position high-priority order

### Switch DD postponement = NO
### Switch to rush grid = irrelevant since already high-priority order

- High-priority order must go in
- Scheduling attempt with all grids, also minimal
- Scheduling attempt in shifts that are open for rush orders
- Scheduling attempt in shifts of bottleneck machines, even if these are already full
- Scheduling attempt of a processing in a shift, even if the duration is longer than the shift duration (error eliminated in Version 6.2)
- If this still does not manage to find the DD, then there is a second internal scheduling attempt.
- The second attempt ignores the campaign dates and can bring the production start forward.
- If no scheduling is possible, then the order lands on the red card.

### Switch DD postponement = YES, x days
### Switch to rush grid = irrelevant since already high-priority order

- High-priority order must go in
- Scheduling attempt with all grids, also minimal
- Scheduling attempt in shifts that are open for rush orders
- Scheduling attempt in shifts of bottleneck machines, even if these are already full
- Scheduling attempt of a processing in a shift, even if the duration is longer than the shift duration (error eliminated in Version 6.2)
- If this still does not manage to find the DD, then there is a second internal scheduling attempt.
- The second attempt ignores the campaign dates and can bring the production start forward.
- If no scheduling is possible, then the DD is postponed.

## 5.2. Collected information

This information came from a document from the market solution area, which was composed by NG in 2016.

### 5.2.1. Manual reprocessing (red card)
If an order is on the red card, then you can force the scheduling.

- **"Force scheduling"**
    - Shifts of bottleneck machines will be ignored, even if these are full.
    - A processing with a duration that is longer than the shift duration can be scheduled.
- **"Ignore scheduling"**
    - Order will be handled like high-priority order, see above.

### 5.2.2. Processing chains

- All processings that are done together should have activated the processing chain in the MA. These include arrissing, grinding, polishing, drilling, etc.
- Just not for processings that must be done one after another, that is, e.g., two times screen printing, two times sand blasting.

### 5.2.3. Alternative machine

- If an alternative machine is activated, then record times the time. Can take somewhat longer during import.
- Ensure that the processing is not brought forward.

### 5.2.4. CAPA_SETTING/MINIMUM_NORMALTRANSITIONS switch

- Specifies how many normal transitions are permitted between two machines.
- Should not be greater than value from "MaxSchichten".
- If a value in "MaxSchichten" is greater than this, then higher values will be ignored.

## 6. Feedback

In the past, many files were used to synchronize batch, order, item, and rack status between A+W Production and the ERP systems. This required a lot of configuration and caused many problems. To simplify the configuration, fileless reporting has been developed.

**Advantage:**
- Only a few settings are required for reporting of the basic status of an order/item/rack
- No files between the systems are required
- Direct view of the production database in order to get more detailed information

**Process:**
The process involves A+W Production systems (Realtime Optimizer, Terminal) filling the AWP-Datenbank. The AlcimBooking service then fills three special report tables. A webservice call is made to the ERP-Webservice, which then fills the ERP-System database.

ALCIMBOOK service saves changes to the batch/order/item or rack status in special report tables:
- **ERP_RUECKMELDUNG:** Reporting of batch and production status
- **ERP_GEST_MELDUNG:** Reporting of rack assignments, linked to production status messages
- **XOPT_RUECKMELDUNG:** Reporting of stock lites used during the cutting process

Two important time stamps are included in all three tables:
- **MELDEZEIT:** Time stamp when the report was generated
- **SENDEZEIT:** Time stamp when the report was transferred successfully to the ERP WebService

An individual thread in the ALCIMBOOK service calls the ERP WebService with the content of these tables as parameters. The ERP WebService transfers this information to the ERP system.

### 6.1. Activation

To switch on fileless reporting in A+W Production, the switch `[ALCIM_STATE / ERPFEEDBACK] = 1` must be set.
- `0`: Report via STSL files (default)
- `1`: Report via table ERP_RUECKMELDUNG and ERP-WebService

### 6.2. Reporting of batch status

This replaces the old reporting via STSL files. With the parameter `Status Registrations`, the A+W Production batch status is defined that should be reported. The parameter `[ALCIM_STATE / STATE]` is a comma-separated list of planning statuses (e.g., `0,10,100,150,200`).

The following status is sent to the ERP system:
- **100**: roughly scheduled
- **150**: scheduled in detail
- **200**: released
- **300**: in production

> **CAUTION:** The behavior of batch status 300 has been improved in Version 6.0 (#318353). As soon as the first process is booked for a lite, the batch status is set to 300 and the batch status in table FEIN_LOS is also updated. In addition, an entry is generated in table ERP_RUECKMELDUNG in order to trigger the fileless reporting in the ERP system. Before Version 6.0, the status and the reporting of the status 300 did not work right!

> **CAUTION:** If the batch status is set manually via the dialog, only a report for status 300 is written to the ERP system! Any higher status was not reported! This was corrected with two hot fixes in AWP5.4 (#341677). Manually settable statuses include: In Production, Produced, ready for shipment, Delivered.

### 6.3. Reporting of production status

This replaces the old reporting via STSD and STSB files. Only the stati "produced", "packed", and "sent" are reported.

The reporting is triggered if the processing on a lite is booked in the PDC system. For each item, the status is sent with the precise booked quantity depending on `POOL_BEARBEIT.FINAL_KZ`.

| Reporting status | Description | Condition POOL_BEARBEIT.FINAL_KZ | Condition BEARBEITSTAMM.AW_BEARBTYP |
| :--- | :--- | :--- | :--- |
| 700 | Produced | 1 | Processing before processing with AW_BEARBTYP = 1800 |
| 800 | Packed | 2 | 1800 |
| 900 | Sent | 3 | 1810 |

A correct configuration of the column assignment in the PDC system is required.

For breakage reporting, 3 entries in `ERP_RUECKMELDUNG` are triggered. For each status (700,800,900) an entry with the correct quantity of lites.

### 6.4. Reporting of intermediate production status

Intermediate production stati are stati between the production start and the final processing before packing:

- `Roughly scheduled, released, in production`: `xxx` = batch status
- `cutting, seaming, drilling, tempering`: `xxx` = intermediate production status
- `packing, delivery`: `xxx` = production status

Normally such stati are displayed in special views in the ERP system via the PPS WebService. For particular reasons, this information is not sufficient (e.g. in order to update the time management in A+W Business).

In order to switch on the intermediate production status, the switch `[ALCIM_STATE / ERP_DETAILED_FEEDBACK] = 1` must be set.
- `0`: ERP production reports just for status "Produced", "Packed", "Sent".
- `1`: Production reports also for intermediate status similar to STSP file.

In the master data for the registration points, a "tool for order entry" must be assigned and the "processing report" activated.

The value from "tool for order entry" is sent via `ERP_RUECKMELDUNG` as "machine" to the ERP system (`ERP_RUECKMELDUNG.MASCH`). The status of the intermediate product is always 300 (`ERP_RUECKMELDUNG.STATUS`).

> **CAUTION:** This function has been available since A+W Production Release 6.0 in combination with A+W Business!

> **CAUTION:** Watch out if you are working with "clean-up registration points" in order to book processings that were done but not booked. Example: the user has cut the glass but not booked it into the system. In the column assignment, the cutting processing is assigned to the registration point 16 (installed). If the IG is now produced on the A+W Production Terminal IG-In and IG-Assembly, the processing cutting is booked as completed. BUT: the registration point 16 is not configured for reporting (which is also not possible since various processings are assigned to the registration point, but only one “tool for order entry“!). This will cause different quantities in A+W Business and A+W Production!

### 6.5. Report of rack allocations

This replaces the old reporting via STSG files. To switch on rack feedbacks, the switches `[ALCIM_BDESETTINGS / FEEDBACKEMPTYRACKS] = 1` and `[ALCIM_SETTINGS / RACK_FEEDBACK] = 1` must be set.

It is also necessary to switch on the rack feedback for particular registration points in the master data, in order to ensure that the rack assignment is sent to the ERP system. In our standard system, this switch is set to registration point 2910 (dispatch).

The reporting is written to the table `ERP_GEST_MELDUNG` with the following status:

| Status | Description | Condition |
| :--- | :--- | :--- |
| 0 | Rack is back "OnSide" | If a rack with status "delivered" loses its status due to some booking, as with a "begin" booking to registration point dispatch |
| 900 | Rack assignment | If a rack is booked to a registration point with switched-on rack feedback |
| 950 | Delivered "Off-premises" | If status "delivered" is booked to a rack. If a rack is booked to a registration point that is linked to the status "delivered" (like 11-Off-Premises). If the delivery address is changed for a delivered rack via A+W Production Terminal |

> **CAUTION:** there is no rack feedback, only when booking a lite to a rack (regardless of which registration point) or booking of a processing!
> **CAUTION:** status 900 for rack feedback has a different meaning than status 900 for "production reporting"

#### 6.5.1. Rack feedback with extended workbench

With another switch, starting with booking version 13.04.5452, a restriction of the "packed" message (status 900) and the sent message (status 950) is possible. The switch is `[ALCIMBOOK / RACKPACKEDFEEDBACKFORPACKEDSHEETS]`.

If the switch is set, there is a rack feedback with status 900 (or 950) only if there are lites with already-booked packed processing on the rack (or packed processing). For the rack assignment, only the packed (or sent) lites are taken into consideration.

This switch is helpful if you are working with the extended workbench (EWB). Racks for the EWB are booked to the registration point dispatch and delivered; however, there may be no feedback for these racks. The lites on the racks of the EWB have the processing `pack EWB` (AW processing type 1805) or `send EWB` (if this processing exists), but not `pack` or `send`. Thus with the set switch, there is no feedback for racks of the EWB.

If there are processings `pack EWB` and `send EWB` on the header part too, it has to be prevented that during booking in dispatch (or to delivered) both processings `pack EWB` and `pack` (or `send EWB` and `send`) are booked simultaneously. This is achieved by including the processing types in the parameter `[ALCIMBOOK / BOOKONLYFIRSTPROCESSINGOFTYPE]`. Example list: `0, 1225, 1500, 1510, 1800, 1804`. If a rack is booked in dispatch, then with the first booking only the processing `pack EWB` is booked; with the next booking in dispatch, the processing `pack` is booked.

Starting with booking service version 13.04.8826 and ERP webservice 13.04.6030, a feedback for racks of the EWB is also possible. For this, a processing type `send EWB` has to be configured. The parameter is `[ALCIMBOOK / PROCESSTYPEFORDELIVEREDMESSAGE]`, with an example value of `1805`.

Using the booked processings of the lites on the rack it is decided whether a feedback for the EWB should occur. For the EWB, a function `AWCapacitySetRackInfoForPart()` is called in the ERP webservice. The tuple numbers of all lites on the rack are also transferred to this function.

The processing type `pack EWB` is recognized on the AW processing type 1805 or on the configured processing type pack EWB.

### 6.6. Reporting of stock lites

This replaces the old PRODDAZ/PRODDUZ file reporting. The reporting must be switched on in `XOPTON.CFG`:

```ini
[Cutting] WriteXoptRueckmeldung

0 = no feedback information for ERP
1 = feedback information for ERP if the pattern is shown by XTV.
2 = feedback information for ERP if the pattern is confirmed by XTV.
3 = feedback information for ERP if the transfer of the cutting code has been started for the pattern. You may use this mode if no XTV is installed.
```

Reporting is also possible for a cutting table without A+W Production Realtime Optimizer. Reporting is done during the first booking of a processing to a part of a batch and is done for all tables configured in the batch. So that this works, the detailed planning must fill the table `XOPT_USED_JUMBO`, switch `[FEIN_SPECIALS / USEDJUMBO]`. In the ALCIMBOOK switches `[ALCIMBOOK / TABLEIDSXOPTFEEDBACK]` the IDs of the cutting tables without A+W Production Realtime Optimizer must be configured for reporting in a comma-separated list.

> **CAUTION:** if the fileless reporting for stock lites is activated as described above, the reporting via files must be switched off in `XOPTON.CFG`. Otherwise, both reporting types will work, which causes doubled stock lite removals!
>
> ```ini
> [FeedBackFile] FeedBackFileType=0
> ```
> 0 = No feedback file will be created

### 6.7. Reporting from goods receipt

In A+W Production, under master data – configuration in the Parameter Administrator under A+W Production - PDC booking service under processing type for goods receipt, the value `9090` must be set; otherwise there is no reporting by the booking service to A+W Business. The parameter is `[ALCIMBOOK / PROCESSTYPEFORGOODSRECEIVED]`.

## 6.8. A+W Business

Using the fileless feedback it is possible to display the production progress of an order directly from A+W Production in A+W Business. The data for the new production overview come directly from A+W Production (online). The status for an Item / Order or Rack is updated by the result of the fileless feedback.

**Process:**
The ERP-Webservice fills the tables `FS_POOL` and `FS_POOL_KOPF`. The interface service (AIS or the new Exchange Service) processes both tables and writes the result in the A+W Business database, e.g.: `BA_GESTELLE_AUFTR` = rack content and customer.

> **ATTENTION:** some feedback takes several minutes to be processed. So you have to be a bit patient until the result arrives in the system. You can see in the field `FS_POOL.STATUS` whether or not the feedback has been processed by the AIS:

| FS_POOL.STATUS | Description |
| :--- | :--- |
| 0 | Not processed |
| 1 | Successfully processed |
| 2 | Error |
| 3 | Locked |

> **ATTENTION:** the fileless feedback is strictly necessary for the surplus function!

### 6.8.1. Configuration

To activate the fileless feedback, you have to set up some master data:
- In `A+W Business -> Master Data -> Company -> 1. Client`, activate "File-less report and online production overview".
- Set the `PPS-Webservice-URL` (e.g., `http://localhost/AlbwirAlcimDataService`).
- Set the `ERP Webservice URL` (e.g., `http://localhost/Albwir.Erp.Webservice2012`).
- In `Master Data -> Production -> Registration points`, configure status points that correspond to production statuses. The following color codes represent status groups:
    - **100-300** = batch status (e.g., planned, released)
    - **400-500** = intermediate production status (e.g., laminating started, IG started)
    - **700-900** = production status (e.g., produced, delivered)

### 6.8.2. FS_POOL

All feedback is stored in the table `FS_POOL`. The content depends on the type of feedback.

**Rack feedback:**

| Column | Content |
| :--- | :--- |
| **ID** | File number. All entries with the same ID coming from the same feedback. |
| **SEQUENZ_NR** | Sequence inside one feedback. Record with sequence=0 determines the customer who will get this rack (first lite from the rack). |
| **DATENSATZ** | Contains booking details such as Booking mode (1=rack entry, 3=rack load/content, 4=rack exit, 5=change of content), Rack name, Timestamp, Order number, Item, Quantity, Barcode, etc. |
| **STATUS** | 0 = not processed, 1 = successfully processed, 2 = error, 3 = locked |

### 6.8.3. Production overview

This feature allows viewing production progress directly in A+W Business.

**New view (based on a report):**
A modern, graphical overview showing the status of each processing step for an order item, including target and actual dates and the registration point.
- **Configuration:** Set in `Master data / Company / Company Data` under folder `13. Production`.
- **Report parameter:** `Report=//sr-db01/Trans/Reports/BDE/AUW_OrderList_Status.rpt&Unterteile_anzeigen=1&Auftrag=[OrderList]`

**Old view:**
A tabular view showing details for each part of an order, including batch, quantity, registration point, status, and timestamps.

**Classic view:**
A grid showing a matrix of registration points against production items, indicating the quantity at each stage.

### 6.8.4. Delivered racks

A+W Business provides a view to see racks that have been delivered, including details like rack number, type, customer, shipping date, and route.

## 6.9. A+W Enterprise

The fileless feedback is only available with A+W Enterprise <-> A+W Production. It is not possible to work with the fileless feedback with ALCIB/PMS.

**Process:**
The ERP-Webservice communicates with an RPC Dienst (Unix Process), which fills the AWE-Datenbank. This database is then updated.

### 6.9.1. Configuration

**PMXTVRLOESCHOPT**
In A+W Enterprise the information is required how long an optimization job may be valid, or when it is possible that a new job is be created with the same number. For this, activate the ALCIB parameter `PMXTVRLOESCHOPT` and assign a value indicating the number of days. If the parameter is not set, a default value of 30 days is applied. Read more information to ALCIB in Chapter 4.2 of `\\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity\Installation_Configuration\TU_090327_IstConfigListAlcibAlcimOrderXML_129902.doc`.

**AWC_ALCIM_ANBINDUNG**
This parameter has to be activated. Without this the complete function (communication with AWCapacity, OrderXML) will not work. Since ALCIB2011, no CommonBase is supported anymore, so the following parameter must be set:
- `AWC_ALCIB_SERVER_NAME`
- `AWC_PORT_RPC_DIENST`
- `AWC_PORT_CONTROL_SERVER` (you will find the ports in: `/etc/services`).

**AWC_FIXIERT_AB**
Specifies the ALCIM status from which on an order item is to be regarded as fixed in production, and hence cannot be edited anymore. Will lead to ALCIB status 300. Standard value 552.

**AWC_FREIGEGEBEN_AB**
Specifies the ALCIM status from which on an order item is to be regarded as released, and hence cannot be edited anymore. Will lead to ALCIB status 302, which cannot be reset anymore. Standard value 554.

**AWC_BUCHE_KPOSPROD**
If this flag is activated, the table `KPOSPROD` will be filled after each processing feedback.

**AWC_GESTZU_BUCHEN**
If this flag is activated the table `GESTZU` will be filled after each rack feedback.

**AWC_IGNORIERE_GESTELLMELDUNG**
If the parameter is set to ON, no rack feedback will be transferred into ALCIB table `BCBOCK`. The ALCIB parameters `GESTELL_BDE`, `MODUL_STAPELLOGIK` and `AWC_GESTZU_BUCHEN` are ignored. This is needed if ACLIM can't guarantee that the feedback of racks isn't numeric. ALCIB can't work with alphanumeric racks.

## 6.10. A+W Cantor

**Feedback Process:**
A+W Production systems generate an `OrderXml` file. This file is placed in a feedback directory. The A+W Cantor system calls `OrderXml` to fill its database.

For the feedback, a directory has to be defined, in which the XML file of A+W Production is stored. This is configured in the Cantor configuration under `[VERZEICHNISSE]`, entry `AlcimImport`.

In addition to the configuration of the directory, a system maintenance queue has to be set up. System queue 50 can import various formats. Parameter 4 is important for XML response. The following options are available here:

| Value | Description |
| :--- | :--- |
| 1 | A+W Pool STSY ASC |
| 2 | A+W Pool FEIN ASC |
| 3 | A+W Pool STSY ASC (Kunde) |
| 4 | Rack feedback from A+W Production |

## 6.11. A+W Cantor CIM

The following master data has to be set up in A+W Cantor CIM:

**Part Additions**
In the master data of terminal group configuration, the part additions 3 and 36 have to be entered.
- **Part addition 3:** Saves all rack information for a fitting field. If there are several lites in this field, the rack information is separated by commas.
- **Part addition 36:** Saves the rack information for a glass field. Which part addition is shown depends on the data procurement of the terminal group.

**Terminal group**
Both part additions have to be entered in the internal variables of the terminal group (e.g., `3;36`).

These variables are then available in the Designer to be placed on the terminal screen layout (e.g., `[Glasbock/-fach Glasfeld]`). When a worker scans a barcode, the corresponding rack information is shown on the terminal group.

The data of the feedback is saved in the respective CIM scheme in the table `CPB_TEILZUSATZ`.

### 6.11.1. Configuration in A+W Cantor

**PRODCONF**
| PRODCONF | Description | Possible values |
| :--- | :--- | :--- |
| 599 | Releases the system action for the feedback file of A+W Production. | 0.1 |

**CANTOR.INI**
| Section | Entry | Value Description |
| :--- | :--- | :--- |
| DIRECTORIES | AlcimImport | Here it is specified in which directory the feedback file of A+W Production is imported. |

### 6.11.2. Configuration in A+W Production

Rack feedbacks will only be created for out-of-house booking in A+W Production. To activate the file-less feedback in A+W Production you set the following parameter:
- `[ALCIMBOOK / CANTOR_RACKFEEDBACK] = 1`
- `[ALCIMBOOK / CANTOR_FEEDBACKPATH] = $SERVERDIR$\EXPORT\` (Standard)
- `[Data import (Item4Alcim) / CREATE SN FILES ] = 0`

### 6.11.3. Result

A file will be created with the name `RACK<timestamp>.XML` in the following format:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<RACK_RESPONSE>
  <RACK>
    <RACK_ID>...</RACK_ID>
    <SLOT>
      <SLOT_ID>...</SLOT_ID>
      <GLASS id="1">
        <GLASS_BARCODE>...</GLASS_BARCODE>
        <ORDERER_ORDER_NO>...</ORDERER_ORDER_NO>
        <ORDERER_REFERENCE_ITEM_NO>...</ORDERER_REFERENCE_ITEM_NO>
        <ORDERER_FIELD_NO>...</ORDERER_FIELD_NO>
        <ORDERER_PIECE_NO>...</ORDERER_PIECE_NO>
      </GLASS>
    </SLOT>
  </RACK>
</RACK_RESPONSE>
```

| Attribute | Data type | Length | Description | A+W source |
| :--- | :--- | :--- | :--- | :--- |
| **RACK_ID** | Char | 255 | Rack ID | `AWBAR_GESTELLE.GESTELLNAME` |
| **SLOT_ID** | Int | | Slot ID | `AWBAR_TEILE.FACHNR` or sequence |
| **GLASS_BARCODE** | Int | | Optional glass barcode | |
| **ORDERER_ORDER_NO** | Int | | Order number of purchaser. | `POOL_TXT.TEXT` (TYP 6009) |
| **ORDERER_REFERENCE_ITEM_NO** | Int | | Reference item number of purchaser. | `POOL_TXT.TEXT` (TYP 6010) |
| **ORDERER_FIELD_NO** | Int | | Field number of purchaser. | `POOL_TXT.TEXT` (TYP 6004) |
| **ORDERER_PIECE_NO** | Int | | Quantity of purchaser | `POOL_POS.MENGE` |

**Field Explanations:**
- **RACK_ID:** The rack name from the field `AWBAR_GESTELLE.GESTELLNAME`.
- **SLOT_ID:** For slot carts (rack with `AWBAR_GESTELLE.TYP_KZ = 1`), the slot number is filled from the field `AWBAR_TEILE.FACHNR`. If there are no slot carts, then `SLOT_ID` is filled with the sequence of the lites according to booking, beginning with 1.
- **ORDERER_ORDER_NO:** The values for the order and item number of a lite are read from the database field `POOL_TXT.TEXT`. The order number is taken from the data record with `POOL_TXT.TEXT_TYP = 6009`.
- **ORDERER_REFERENCE_ITEM_NO:** Same behavior as `ORDERER_ORDER_NO`, but `POOL_TXT.TEXT_TYP = 6010` is used.
- **ORDERER_FIELD_NO:** Same behavior as `ORDERER_ORDER_NO`, but `POOL_TXT.TEXT_TYP = 6004` is used.
- **ORDERER_PIECE_NO:** The total from `POOL_POS.MENGE` of all data records that belong to the same commercial item (`POOL_POS.AE_INTPOS`) of the lite.

> **Caution:** Feedback is only generated for lites where data records from `POOL_TXT.TEXT_TYP` 6004, 6009 and 6010 exist. The file is initially created with the extension `.TMP` and renamed `.XML` when it is written completely. The file name contains a time stamp. Errors that occur when writing the file are logged in the trace of the booking service.

## 7. A+W Realtime Optimizer

### 7.1. Multiple user login

In the A+W Realtime Optimizer, one or more users can be logged into the 'PDC' for evaluation for each configured cutting table. When closing the A+W Realtime Optimizer, all users must be logged out so that the A+W Realtime Optimizer can be closed. Registration is done via the main menu bar Settings > Tables > Login on a separate dialog. It can be configured that at least one user must be logged in to start the cutting process.

In order to activate the PDC user login in A+W Realtime Optimizer, the following requirements must be met:
- The PDC must be active.
- Open the Parameter Administrator in A+W Production via the menu `Master Data > Configuration`.
- In `A+W Production Terminal` both the parameters "Person for 'Logged off'" and the "Registration point for 'Logged off'" must be set in section 'Bookings'.
- The `"Albwir.Alcim.GlobalForms.dll"`, `"Albwir.Alcim.Designer.dll"` and the `"DataBaseReader.dll"` must be available in the program directory of the A+W Realtime Optimizer.
- In the `xopton.cfg` under `%AppData%\Roaming\A+W\TECHSOFT\Xopton` in the section `[BDE]`, the following switches have to be configured:
    - `Mode > 0`
    - `BdeUserSignIn=Y`
    - `BdeUserSignInMandatory=N / Y`
        - **N:** No user must be logged in to start the cutting process.
        - **Y:** At least one user must be logged in to start the cutting process.

## 8. A+W Barcoding

### 8.1. Background printing and e-mail dispatch

The booking service can be used to print reports and send e-mails.

The `ProcessManagerService` controls the report generation and sends e-mails. The CrystalReport runtime is required in order to create the reports. The booking service decides using the configuration whether a report should be created and sent and write the order into the table `PROZESSE`. `ProcessManagerService` evaluates the table `PROZESSE` and creates the reports and sends them.

The configuration and conditions that trigger the background printing are specified in the parameter administrator:

- In the section `'A+W Production -> General -> Mail Settings'` the connection data of the mail server used by the `ProcessManagerService` to send mails is stored.
- The section `'A+W Production -> Barcoding Booking Service -> General->Print of Report'` defines the conditions that must be met for a mail to be sent and the parameters of the mail stored.

The following mail parameters must be specified:
- **Report:** The file path to the CrystalReport file that will be attached as PDF attachment to the e-mail.
- **Recipient:** Address to which the generated e-mail should be sent.
- **Object Type:** Determines which object (lite, rack or registration point) is to be observed for changes in its properties.
- **Station group:** Specifies which instance of the `ProcessManagerService` executes the background printing and sending of the e-mail. The instances offered are specified in the section `'A+W Production-> Release Dialog-> Group of Executing PCs'`.

The following parameters are optional:
- **Printer:** If a printer is specified, in addition to the e-mail, the report will also be output on this printer.
- **Mail subject**
- **File path for mail content:** Path to a TXT file whose content will be copied into the e-mail.
- **Additional fields:** Field content of the booking record that can currently be evaluated by the booking service can be transferred to CrystalReport. The 'Additional fields' parameter specifies which fields from the table `AWBAR_BOOKING` should also be transferred to the report.

**Conditions that can be specified in order to generate a mail:**
If one of the parameters is configured, then only an e-mail is generated if the booking is of the corresponding parameter type.
- Stati
- Status Type
- Registration point
- Registration point type

**Report definition**
The report used must absolutely have a string transfer parameters with the name `"Barcode"`. In this, the bar code of the defined object type from booking is transferred.

### 8.2. 15-digit Gestellpool Europe barcodes

#### 8.2.1. Configuration in A+W Production

In order to be able to use 15-digit Gestellpool Europe barcodes in A+W Production, various adjustments must be made in the database.

The following DB update scripts must be present in `C:\Program Files (x86)\A+W\Techsoft\sql\XML`:
- `awupdate_alcim_2_626.xml`
- `awupdate_alcim_2_627.xml`
- `awupdate_alcim_2_628.xml`
- `awupdate_alcim_2_629.xml`
- `awupdate_alcim_2_630.xml`
- `awupdate_alcim_#389903_-1_-1.xml`

The standard scripts (2_626 to 2_630) enlarge database fields for the rack barcode. The customer-specific script enables alphanumeric barcodes and creates a new table for barcode recognition with regular expressions.

> **Attention!** With this solution, the master data dialog for racks and the one for barcode types do not work anymore. Production Terminals, label printing, etc. were not considered in this solution.

After the DB update, execute the following insert:
```sql
insert into awbar_barcodetypen (nummer, typ,name, laenge, pruefziffer,codetyp, [status], regex, praefix, ersetzungsmuster) values (1,3,'GESTELL',15,0,0,0,1,'([0-9]{15})$','');
```
The table `awbar_barcodetypen` will then contain a new entry for `typ=3` with `laenge=15` and the specified regex.

#### 8.2.2. Configuration in A+W Smart Companion

To process 15-digit Gestellpool Europe barcodes in the AWSOA database, a Regex adjustment must be made in the configuration of the infrastructure Web under `A+W Production -> CIMScannerSettings` in the Barcode Classification.

1. Download the current configuration.
2. Open the downloaded configuration with a text editor like Notepad++.
3. The entry for the "Regular Expression" for "Rack Barcode (Gestellpool Europe)" must be adjusted as follows:
   ```json
   {
       "$type": "AWSOA.Infrastructure.Config.ServiceContracts.DataTransferObject.BarcodeClassificationDto, AWSOA.Infrastructure.Config.ServiceContracts",
       "Sequence": 4,
       "BarcodeType": 3,
       "BarcodeSymbology": 16,
       "Application": 1,
       "RegularExpression": "([0-9]{15})$",
       "Substitution": "$1",
       "Description": "Rack Barcode (Gestellpool Europe_long)"
   }
   ```
4. After the entry has been adjusted, save it.
5. Upload the configuration file within the infrastructure web under `A+W Production -> CIMScannerSettings` in the Barcode Classification.
6. The configuration is saved automatically by the uploading. You can see the change under Barcode Classification 4.

### 8.3. Breakage booking with incomplete assembly message

If a unit (IG, LAMI or cast resin) is reported broken whose assembly has not been booked, no remakes are generated for the subparts. To prevent this, a new behavior can be activated. Instead of a breakage booking, a configurable state is booked to the unit, placing it in the remake handling. The breakage is not booked if at least one glass subpart has not been assembled.

In the remake handling, you can filter by the state for non-assembled lites. Any subpart can be assigned a still-available label number, and then the break can be booked after the fact.

This new behavior is activated by the switch `STATUSBARCODENOTASSEMBLED` in the booking service parameters. The state barcode for non-assembled lites is specified here. This state must not be a breakage reason and should be configured to cause a booking in the remake handling.

An update of the booking service is not sufficient. The display and bookings of the remake handling have also been changed. The dialog mode (expert mode) switch must be set to 1.

### 8.4. Consideration of the timestamp of bookings

By default, bookings are not executed if a newer booking already exists for the registration point, rack, or lite. The switch `[ALCIMBOOK / IGNOREOBSOLETETIMESTAMP]` allows ignoring the booking timestamp. Bookings are then made regardless of their timestamp.

### 8.5. Messages from bookings to the Smart Factory

Bookings to the Smart Factory can be reported from A+W Production Booking. This is activated with the switch `[ALCIMBOOK / PUBLISHBOOKINGS]` in the parameters for the booking service. If the switch is set, the following types of bookings will be reported:

#### 8.5.1. Lite at registration point

If the registration point of a lite changes, this is reported. The message includes the label of the lite, the number of the registration point, and the time stamp of the booking. This applies to any booking type that changes the registration point. The Smart Factory can be configured to react only to specific registration points.

#### 8.5.2. Booking of the processing "packed" or "sent"

If for the last lite of an order and a production item the processing "packed" or "sent" is booked, a message is issued. The message includes the order number, item number, and time stamp of the booking. This message can be used in the Smart Factory to initiate archiving.

#### 8.5.3. Fraction calculations

For a breakage booking, the label of the lite, the number of the registration point, and the time stamp of the booking are also reported. The reported registration point is the one before the breakage recording point 19.

#### 8.5.4. Booking of a state of the type "reuse"

Booking of a state of the type "reuse" ("prolonging") on a lite is reported. This state is for a lite that can be reused after a break. The booking service detects this state type via the field `AWBAR_ZUSTANDTYP.FUNKTIONTYP = 3`.

**Set-up of a state type "reuse":**
- In the master data for the state types, a new state type for "reuse" ("prolonging") must be created if it does not already exist.
- The decisive setting is that the "Function" is set to the value 3 (`Prolonging`).

**Set-up of the remake handling for the booking of "reuse":**
- In the parameters for remake handling (`AUW_PPSREMAKE`), a state for the booking of "reuse" can be specified with the parameter `_PPSR_REMAKEPROLONGINGBC`.

If for an IG from the remake handling "direct remake" is selected, then for the sub-parts of the IG, the original procurement type (cutting), reuse or prolonging can be selected. In case of reuse or prolonging, a registration point and a rack can also be specified.

## 9. Remake handling

This document describes how "partial defect" works. The partial defect should essentially fulfill two requirements:
a) The possibility to report only parts of an assembled product as broken (partial defect)
b) Via an editor, to decide what should be done with the individual parts of the remake (via a new item in the pool (OP remake) or immediate reproduction, etc.)

### 9.1. Mode of Operation / Operation

#### 9.1.1. Booking of a partial defect

The booking of a partial defect can be done via an A+W Production Terminal or a scanner. A status booking of the type `40=partial defect` must be made. The booked component is thus booked to the registration point `40=defectpool` and can then be processed further in the remake handling.

### 9.2. Configuration

#### 9.2.1. A+W Production parameters

- **Activation:** In `PDC Booking Service`, set `Activation Rough Planning Remakes=1`. The entry is under `Bereich=ALCIMBOOK` and `Eintrag = NACHLAUFPOS`.
- **Parameter Set:** Under `A+W Production/General/Parameter Record PPS Remake Dialog`, you can set which parameter set to use (Default = `AUW_PPSREMAKE`). The entry is under `Bereich=ALCIM_SETTINGS` and `Eintrag = PARAMETERSETREMAKEDIALOG`.

#### 9.2.2. PDC master data

**Registration point types**
- **Type 80: Defect Location:** All registration points assigned to this type are regarded as causing defect location.
- **Type 40: Defect Pool:** This type distinguishes the defect pool from "normal" registration points, ensuring correct display in terminal filters.

**Registration Points**
- **RPNO 5: Production:** Default outgoing registration point for lites that can be reused.
- **Type 40: Defect Pool:** Lites on this registration point are displayed in the remake handling.
- **RPNO 81/82: Defect Location 1-2:** Example defect locations.

**Status Types**
- **Type 40: Partial Defect:** This controls that all partial defects are booked to the registration point "Defect Pool". The status booking should book to RP `0040 Defect-Pool`.
- **Type 60: Re-Use:** This function ensures that the procurement types of the AV remakes are set correctly. The function should be set to `02-ReUse`.

**Stati**
- **Status 40: Partial Defect:** At least one status of type 40 is required. This status is booked by the break recorder to move the part into remake handling.
- **State 60: Re Use:** A status of type 60 is required for the re-use function.

#### 9.2.3. Parameter Administrator dialog

The main dialog and processing dialog for the remake handling feature are configured via a set of parameters, typically within a parameter set named `AUW_PPSREMAKE`.

**Parameters for the main dialog (misc)**

| Parameter | Value | Description |
| :--- | :--- | :--- |
| **Surface** | `AUW_PPSRemakeDialog_Main` | The designer form for the main dialog. |
| **Selected Tables** | (List of tables) | Tables from which data can be selected. |
| **FROM Clause** | (SQL FROM clause) | Defines table joins for the main query. |
| **Fixed SQL-Filter** | (SQL WHERE clause) | A fixed filter, e.g., to join on `awbar_stellen` to show the registration point name. |
| **Automatic Update** | `False` / `True` | Defines whether the dialog will be updated automatically. |
| **Update Frequency** | `180` | Interval in seconds to update the dialog. |
| **Edit Dialog** | `AUW_PPSRemakeDialog_Edit` | The designer form for the edit dialog. |
| **Rebook Dialog** | `AUW_PPSRemakeDialog_BookStateDialog` | The designer form for the rebooking dialog. |
| **Status type for broken parts** | `40` | Status bookings of this status type are moved to remake handling. |
| **Status barcode for „Rejects"**| `500000010` | Barcode for rejects. |
| **Status barcode for „Reuse"** | `500000060` | Parts that can be reused are booked with this status. |
| **Dialog Mode** | `0` / `1` | 0 = safe mode (only assembled parts displayed), 1 = expert mode (complete BOM displayed). |

**Parameters for processing dialog:**

| Parameter | Value | Description |
| :--- | :--- | :--- |
| **Types for Registration Point** | `200,300,600,...` | Limits the registration points that can be used for parts. |
| **Types for Reject Registration Point**| `80` | Limits the registration points for the defect location. |
| **Status Types for Reject Reasons**| `4` | Reasons for defect that are communicated with the part. |
| **Filter on Part Types**| `10` | Suppresses certain part types (e.g., films, frames) from the display. |

### 9.3. Operation of the remake handling

#### 9.3.1. Remake handling
The remake handling feature is accessed from the `Extras -> Nachläufer-Verwaltung` menu in A+W Production.

#### 9.3.2. Display

The remake handling dialog displays all lites that have a configurable state type (e.g., partial defect).

**Display in the detail list:**
- The detail list is filled when a lite is selected in the top list.
- A switch `_PPSR_PARTTYPEFILTER` can exclude certain part types (e.g., spacers, foils) from the detail list.
- **IG with installed lites:** The IG and its installed parts are displayed. All actions ("reuse", "scheduling remake", "direct remake") are possible.
- **Purchased IG:** Only the IG is displayed. All three actions are possible.
- **Non-produced IG:** Behavior depends on two switches:
    - **`_PPSR_SHOWPLANNEDBARCODES`:** If set, the IG and its planned parts (from detailed scheduling) are displayed. All actions are allowed.
    - **`_PPSR_EXPERTMODE`:** If this is set (and the above is not), the IG and its BOM sub-elements are displayed without assigned labels. All actions are possible.
    - If neither switch is set, only the IG is displayed, and only the "reuse" action is allowed.
- **Subelement of an IG or TG:** In expert mode, the sub-element, counter-lites, and header part are displayed. All actions are possible. If not in expert mode, only the sub-element is displayed, and "scheduling remake" is not allowed.

**Interface Breakdown:**
1.  **Menu Bar:** Top of the screen for future list attachments.
2.  **Overview Grid:** Top data grid showing parts with a partial defect (status type 40) or at the defect pool (RP 40).
3.  **Detail Grid:** If a lite is selected above, its associated BOM parts are displayed.
    - **Expansion (AWP5.4+):** The entire BOM is displayed, allowing decisions on all components.
    - **Expansion (AWP6.3+):** If components are assembled first and then reported broken, the system knows which BOM parts are affected.
4.  **Rebook Button:** Allows assigning lites to a different break reason (status) and adding an info text.
5.  **Filter:** Filters the remake handling list by status (e.g., "scratches").
6.  **Macros (F7-F9):** Buttons for rough decisions on the broken lite.

#### 9.3.3. Macros – the rough decision

- **Re-Use [F7]:** Used if the complete part can be reused. The procurement type is set to "reuse", and it disappears from the defect pool.
- **Re-Schedule [F8] (AV remake):** Creates a new production item in the order pool with original procurement types. The old item is reduced in quantity.
- **Direct Remake [F9]:** Creates a "normal" break. The parts are treated as for a direct defect booking and must be reproduced manually.

#### 9.3.4. Details – the fine-tuning

More precise settings can be made by double-clicking a part or using the "Edit" button (F3).

- **Procurement Type:** Change the procurement type between the original and "Reuse".
- **Registration Point:** If reusing, select the location to store the part.
- **Rack:** Specify a rack to store the reusable part.
- **Defect-Reason:** If not reusing, select the real defect reason for statistical evaluation.
- **Defect-Location:** Specify a defect location, regardless of where the break was booked.
- **Processes:** For processings like screen printing, you can choose to repeat only specific processings instead of remaking the entire lite.
- **Re-Schedule:** Placing a checkmark generates a new production item in the order pool.

#### 9.3.5. Assignment of real components (starting with AWP5.4)

This function is only available in "Expert Mode". If a subpart of an unplanned or planned product is broken, you can:
a) Reschedule the corresponding BOM components (counter-lites, spacer, header parts)
b) Reschedule the individual components in the capacity planning
c) Produce the product in a new batch

When a subpart is broken, the complete BOM is displayed in the remake handling. Components that are not yet clearly identified are shown without a barcode. If the user generates an OP remake, a new item is created.

**Example:**
An order has 4 insulated glass lites, unplanned. Label No. 13 is booked as a partial defect and an OP remake is created. In the new item, only the part with label No. 13 can be re-planned. The other BOM parts (with virtual labels) have the procurement type "11-Production in the original" and are ignored by planning.

