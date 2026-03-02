---
description: "AUW_Description_File-less_Feedback"
---

# File-less Feedback

> Document is transferred into configuration manual!

## History
| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 11.06.2012 | Dirk Langwald | First Release | 1.0 |
| 11.03.2015 | Peter Kühn | New structure, news from Release SP55 | 2.0 |
| 31.03.2015 | Peter Kühn | Changes (manual setting of batch-status) after Hotfix in SP54 ff. | 2.1 |
| 26.06.2015 | Peter Kühn | Correction in intermediate-status | 2.2 |
| 29.10.2015 | Peter Kühn | Add new production-overview in AWB | 2.3 |
| 27.01.2016 | Peter Kühn | Add new information for AWP-Release 6.0 | 3.0 |
| 18.02.2016 | Peter Kühn | Change settings for intermediate feedback for Release 6.0 | 3.1 |
| 15.03.2016 | Peter Kühn | Add Classic view in AWB; and remarks to the intermediate feedback | 3.2 |
| 07.11.2016 | Peter Kühn | Add information about connection to Cantor | 3.3 |
| 01.06.2017 | Anja Grünbacher | Add information about connection to Cantor | 3.4 |
| 11.07.2017 | Peter Kühn | Add information about stockplate feedback | 3.5 |
| 30.07.2018 | DLA | Changes of document now in CONFIGURATION manual!!! | - |

## Motivation

In the past we used a lot of files between the PPS-System and the ERP-Systems to synchronize batch-, order- and item-states or rack-states. This needs a lot of configuration and cause a lot of troubles.
To make the configuration simpler, the file-less-feedback was developed.
Benefit:
- There are just a very few settings necessary to feedback the basic states of an order/item/rack
- There are no files between the systems necessary
- Direct view into the production-database to get detailed order-information
Disadvantage:
- There are only basic information’s transferred between the systems, such as: batch scheduled or released, production started, sheet produced, packed and shipped.
- To get intermediate-states from the production, there is additional configuration necessary
## A+W Production

### Process

Changes of Batch/Order/Item or Rack-states are stored by AlcimBooking in special feed-back-tables:
- `ERP_RUECKMELDUNG` — feedback batch and production status
- `ERP_GEST_MELDUNG` — feedback of rack layout, linked to feedback of production status
- `XOPT_RUECKMELDUNG` — feedback of used stock plates during cutting process
A separate thread in Alcimbooking calls the ERP-WebService with the content of these tables as parameter. The ERP-WebService will transfer this information to the ERP-System.
### Configuration and Conditions

**Activate the file-less feedback in AWProduction**

To activate the file-less feedback in AWProduction you set the following parameter:
`[ALCIM_STATE / ERPFEEDBACK] = 1`
**Feedback of batch status**

This is the replacement for the old feedback via STSL-file. No new or additional configuration is necessary.
`[ALCIM_STATE / STATE] = 0,10,100,150,200`
The following status will be send to the erp-system:
| Feedback-Status | Description | Batch-Status |
| --- | --- | --- |
| 100 | Roughly scheduled | 100 |
| 150 | Scheduled in detail | 150 |
| 200 | Released | 200 |
| 300 | In Production | 300 |

> ATTENTION: the behavior of batchstatus 300 was improved in AWP6.0 (#318353). As soon as the first process on any sheet is booked, the batchstatus is set to 300 and also if there is a lot the status in fein_los is updated. Additionally there is an entry in erp_rueckmeldung created to trigger the file-less feedback to the erp-system.

Before AWP6.0 the status and feedback for status 300 is not correctly working!
> ATTENTION: if the status of a batch is set manually via this dialog:

There is only a feedback written to the ERP-system for status 300-in production! All other higher states are not reported!
This was fixed with two hotfixes in AWP5.4 (#341677 SGDG: Erweiterung Laufstatusrückmeldung) \\jupiter\SW_Install\Hotfix\0_A+W Production 5 Booking_1822.zip and
\\jupiter\SW_Install\Hotfix\0_A+W Production 5 Booking_1823.zip
**Feedback of production status**

This is the replacement for the old feedback via STSD- and STSB-file. Only the states “Produced”, “Packed”, and “Shipped” will be reported.
The feedback is triggered, if the process of a sheet is booked with the barcoding system. The Status will be send for each line item with the exact booked quantity, depending of pool_bearbeit.final_kz.
| Feedback-Status | Description | Condition
POOL_BEARBEIT.FINAL_KZ | Condition
BEARBEITSTAMM.AW_BEARBTYP |
| --- | --- | --- | --- |
| 700 | Produced | 1 | Process before process with AW_BEARBTYP = 1800 |
| 800 | Packed | 2 | 1800 |
| 900 | Delivered | 3 | 1810 |

It is also necessary to setup the correct column-assignment in the tracking system.
In case of a breakage, there will be 3 entries in the erp_rueckmeldung triggered. For each status (700,800,900), one entry with the correct amount of sheets.
**Feedback of intermediate production status**

Intermediate production states are states between the start of production and the final process before packing:
roughly scheduled, released, in production, cutting, seaming, drilling, toughening, packing, delivery
xxx = batch status
xxx = intermediate production status
xxx = production status
Normally those states can be displayed via the PPS-WebService in a special view in the erp-system. For some reasons this information is not enough (e.g. to update the capacityplanning in AWBusiness, …).
To activate the intermediate production status, you have to set the following parameter:
`[ALCIM_STATE / ERP_DETAILED_FEEDBACK] = 1`
You also have to assign a “Machine of the Order Entry” and activate the “Processing Feedback”:
The value in “Machine of the Order Entry” is send via erp_rueckmeldung as a “machine” to the erp-system (erp_rueckmeldung.masch). The status for the intermediate is always 300 (erp_rueckmeldung.status).
> ATTENTION: this functionality is only available with AWProduction Release 6.0 and AWBusiness!

> ATTENTION: take care if you are working with “cleanup-registrationpoints” to book processes which are done, but not booked. Example: the user has cut the glass but not booked into the system. In the column-assignment, you assign to the Registrationpoint 16 (assembled) the process “cutting”. When you now produce the IG via Productionterminal IG_In and IG-Assembly, the process “cutting” is booked as done in A+W Production. BUT: the Registrationpoint 16 is not configured to send a feedback (which is not possible, because: several processes are assigned to reg.-point 16, but only one “machine of the order entry”)! This will cause different quantities in AWB and AWP!

**Feedback of rack-assignment**

This is the replacement for the old feedback via STSG and STSK-files. To use that rack-feedback, you have to enable the following parameters in AWProduction:
`[ALCIM_BDESETTINGS / FEEDBACKEMPTYRACKS] = 1`
`[ALCIM_SETTINGS / RACK_FEEDBACK] = 1`
It is also necessary to enable the rack-feedback for certain registrationpoints in the AWProduction masterdata…
… to make sure that the rack-content will be send to the erp-system. In our standard-system, this flag is set for Registrationpoint 2910-dispatch.
The feedback is written into the table erp_gest_meldung with the following status:
| Status | Description | Condition |
| --- | --- | --- |
| 0 | Rack is back “OnSide” | If a rack with the state “delivered” loose this status by any booking, such as “begin” or book on Registrationpoint dispatch |
| 900 | Rack content | If a rack is booked to a Registrationpoint, where the rack-feedback is enabled |
| 950 | Delivered
“OffSide” | If the state “delivered” is booked to that rack
If the rack is booked to a Registrationpoint, which is linked to the state “delivered” (such as 11-OffSide)
If the delivery address is changed for a delivered rack via AWProductionterminal Edit |

> ATTENTION: there is no rack-feedback triggered just by booking a sheet to a rack (no matter on which Registrationpoint) or after booking a process!

> ATTENTION: the status 900 in the rack-feedback has a different meaning then status 900 in the production-feedback!

**Feedback of stockplates**

This is the replacement for the old PRODDAZ/PRODDUZ feedback files. The feedback has to be activated in the Xopton.cfg:
[Cutting]
WriteXoptRueckmeldung
0 = no feedback information for ERP will be written to
1 = feedback information for ERP will be written if the pattern is shown by XTV.
2 = feedback information for ERP will be written if the pattern is confirmed by XTV
3 = feedback information for ERP will be if the transfer of the cutting code has been started for the pattern. You may use this mode if no XTV is installed.
For all cutting tables without XOPTON a feedback is also possible. The feedback happens during the first booking of a processing on a part of a batch. The feedback happens for all configured tables in the whole batch. To make it work detailed scheduling has to fill table XOPT_USED_JUMBO, parameter [FEIN_SPECIALS / USEDJUMBO]. In ALCIMBook parameters [ALCIMBOOK / TABLEIDSXOPTFEEDBACK] the cutting table IDs for the feedback without XOPTON has to configured in a comma separated list.
[ALCIMBOOK / TABLEIDSXOPTFEEDBACK]
> ATTENTION: If you enable the fileless feedback for the stockplates as shown above, you have to disable the feedback via file in the xopton.cfg. Otherwise both feedbacks are working which cause double stockplate reduction!

; ............. Section for FeedBackFile ...................................
[FeedBackFile]
FeedBackFileType=0
; 0 : No feedbackfile will be created
### Result

Each feedback from AWProduction is stored in the table’s erp_rueckmeldung, erp_gest_meldung or xopt_rueckmeldung. In all three tables there are two important timestamps:
MELDEZEIT: Timestamp of feedback creation
SENDEZEIT: Timestamp when the feedback is successful transferred to the erp-webservice
All other fields are documented in the A+W Production Table-documentation
## A+W Business

### Process

Using the file-less feedback it is possible to display the production progress of an order directly from A+W Production. The data for the new production overview come directly from A+W Production (online). The status for an Item / Order or Rack is updated by the result of the file-less feedback.
The ERP_WeBService fill the tables FS_POOL and FS_POOL_KOPF. The Alfak-Interface-Servcie (AIS) process both tables and write the result in the A+W Business database. Some example:
BA_GESTELLE_AUFTR = rack-content and customer
> ATTENTION: some feedbacks take several minutes to be processed. So you have to be a bit patient until you expect a result. If the feedback is processed by the AIS or not, you can see at the field FS_POOL.STATUS:

| FS_POOL.STATUS | Description |
| --- | --- |
| 0 | Not processed |
| 1 | Successful processed |
| 2 | Error |
| 3 | Locked |

> ATTENTION: the file-less feedback is strictly necessary for the surplus function!

### Configuration and Conditions

To activate the file-less feedback you have to setup some master data:
100-300 = batch status
400-500 = intermediate production status
700-900 = production status
### Result

**FS_POOL**

All feedbacks are stored in the table FS_POOL. The content depends on the type of feedback.
Rackfeedback:
| Column | Content |
| --- | --- |
| ID | Filenumber. All entries with the same ID coming from the same feedback |
| SEQUENZ_NR | Sequence inside one feedback. Entry with the Sequence=0 determine, the customer who get this rack (first sheet from the rack) |
| DATENSATZ | Bookingmode: 1= rack entry (return), 2 = Nothing, 3 = rackload / rack-content, 4 = rack exit (delivery), 5 = change of rack content
Rackname
Timestamp of booking
Ordernumber
Item
Quantity
Barcode
Equipment |
| STATUS | 0 = not processed
1 = successful processed
2 = error
3 = locked |

**Production Overview**

Old view:
New View (based on a report):
To be configured here:
Masterdata / Company / Company Data – here use Folder “13. Production”:
Classic view:
**Delivered Racks**

## A+W Enterprise

### Process

The file-less feedback is only available with AWEnterprise <-> AWProduction. It is not possible to work with the file-less feedback with Alcib/PMS!
### Configuration and Conditions

PMXTVRLOESCHOPT
In ALCIB the information is required how long an optimization job may be valid, or when it is possible that a new job is be created with the same number. For this, activate the ALCIB parameter PMXTVRLOESCHOPT an assign a value indicating the number of days. If the parameter is not set, a default value of 30 days is applied. Read more information to ALCIB in Chapter 4.2 of .
AWC_ALCIM_ANBINDUNG
This parameter has to be activated, without this the complete function (communication with AWCapacity, OrderXML) are not working. Since ALCIB2011 no CommonBase is supported anymore, so the following parameter must be set: AWC_ALCIB_SERVER_NAME, AWC_PORT_RPC_DIENST, AWC_PORT_CONTROL_SERVER (you will find the ports in /etc/services).
AWC_FIXIERT_AB
Specifies the ALCIM status from which on an order item is to be regarded as fixed in production, and hence cannot be edited anymore. Will lead to ALCIB status 300. Standard value 552.
AWC_FREIGEGEBEN_AB
Specifies the ALCIM status from which on an order item is to be regarded as released, and hence cannot be edited anymore. Will lead to ALCIB status 302, which cannot be reset anymore. Standard value 554.
AWC_BUCHE_KPOSPROD
If this flag is activated, the table „kposprod“ will be filled after each processing-feedback (#180809).
AWC_GESTZU_BUCHEN
If this flag is activated the table „GESTZU“ will be filled after each rack-feedback.
AWC_IGNORIERE_GESTELLMELDUNG
Is the parameter set to ON, no rack feedback will be transferred into ALCIB table BCBOCK. The ALCIB parameters GESTELL_BDE, MODUL_STAPELLOGIK and AWC_GESTZU_BUCHEN are ignored. This is needed if ACLIM can’t guarantee that the feedback of racks isn’t numeric. ALCIB can’t work with alphanumeric racks.
### Result

???
## A+W Cantor

### Process

### Configuration and Conditions

**A+W CANTOR AV System (AV=Arbeitsvorbereitung, transl. work preparation)**

For the feedback, a directory has to be defined, in which the XML file of A+W Production is stored.
In addition to the configuration of the directory, a system maintenance queue has to be set up.
System queue 50 can import various formats. Parameter 4 is important for XML response.
The following options are available here:
| Value | Description |
| --- | --- |
| 1 | A+W Pool STSY ASC |
| 2 | A+W Pool FEIN ASC |
| 3 | A+W Pool STSY ASC (Customer) |
| 4 | A+W Production Rack Response |

**A+W CANTOR CIM**

The following master data has to be set up in the A+W CANTOR CIM:
Part Additions
In the master data of terminal group configuration, the part additions (Teilzusätze) 3 and 36 have to be entered.
Part addition (Teilzusatz) 3 saves all rack information for a fitting field. If there are several lites of glass in this field, the rack information is separated by commas. Part addition (Teilzusatz) 36 saves the rack information for a glass field. Which part addition (Teilzusatz) is shown, depends on the data procurement of the terminal group.
Terminal group (Arbeitsplatzgruppe)
Both part additions (Teilzusätze) have to be entered in the terminal group (Arbeitsplatzgruppe):
Therefore, these two variables are available in the Designer:
Result
If the worker now scans a barcode, the rack information is shown on the terminal group:
Note:
The data of the feedback is saved in the respective CIM scheme in the table CPB_TEILZUSATZ.
**Activate the file-less feedback in A+W Cantor**

Prodconf
| Prodconf | Description | Possible values |
| --- | --- | --- |
| 599 | Releases the system action for the feedback file of ALCIM/A+W Production. | 0.1 |

Cantor.ini
| Section | Entry | Values | System Behavior |
| --- | --- | --- | --- |
| VERZEICHNISSE | AlcimImport |  | Here it is specified in which directory the feedback file of ALCIM/A+W Production is imported. |

Configuration of A+W CANTOR rack feedback for out-of-house booking in A+W Production.
**Configuration of A+W CANTOR rack feedback for out-of-house booking in A+W Production**

To activate the file-less feedback in A+W Production you set the following parameter:
`[ALCIMBOOK / CANTOR_RACKFEEDBACK] = 1`
[ALCIMBOOK / CANTOR_FEEDBACKPATH] set (Standard $SERVERDIR$\EXPORT\)
`[Data import (Item4Alcim) /CREATE SN FILES ] = 0`
### Result

A file will be created with the name RACK<timestamp>.XML (P:\Export\Work) in the following format:
| Attribute | Data type | Length | Description | A+W source |
| --- | --- | --- | --- | --- |
| <?xml version=”1.0” encoding=”UTF-8”> | <?xml version=”1.0” encoding=”UTF-8”> | <?xml version=”1.0” encoding=”UTF-8”> | <?xml version=”1.0” encoding=”UTF-8”> | <?xml version=”1.0” encoding=”UTF-8”> |
| <RACK_RESPONSE> | <RACK_RESPONSE> | <RACK_RESPONSE> | Root level | Root level |
| <RACK> | <RACK> | <RACK> | Rack element | Rack element |
| RACK_ID | Char | 255 | Rack ID |  |
| <SLOT> | <SLOT> | <SLOT> | Slot element | Slot element |
| SLOT_ID | Int |  | Slot ID |  |
| <GLASS id=”1”> | <GLASS id=”1”> | <GLASS id=”1”> | Glass element
The attribute ID is optional: if several lites are found in one location.
First pane in slot ID=1, second pane in slot ID=2 etc. | Glass element
The attribute ID is optional: if several lites are found in one location.
First pane in slot ID=1, second pane in slot ID=2 etc. |
| GLASS_BARCODE | Int |  | Optional: If several lites are found in one location. |  |
| ORDERER_ORDER_NO | Int |  | Order number of purchaser. | CANTOR:
AUFPOS.AufNr (transl. orderitem.order#)
OrderXML: Textid 6009 |
| ORDERER_REFERENCE_ITEM_NO | Int |  | Reference item number of purchaser. | CANTOR:
AUFPOS.RefPosNr (transl. orderitem.referenceitem#)
OrderXML: Textid 6010 |
| ORDERER_FIELD_NO | Int |  | Field number of purchaser. | CANTOR:
AUFART.LfdNr (transl. orderarticle.sequence#)
OrderXML: Textid 6004 |
| ORDERER_PIECE_NO | Int |  | Quantity of purchaser | CANTOR:
AUFPOS.Stck (transl. orderitem.pieces)
OrderXML: UDX.AW -> Amount |
| </GLASS> | </GLASS> | </GLASS> |  |  |
| </SLOT> | </SLOT> | </SLOT> |  |  |
| </RACK> | </RACK> | </RACK> |  |  |
| </RACK_RESPONSE> | </RACK_RESPONSE> | </RACK_RESPONSE> |  |  |

RACK_ID: The rack name from field AWBAR_GESTELLE.GESTELLNAME.
The following information is created for each lite:
SLOT_ID: The slot ID from field AWBAR_TEILE.FACHNR, if the rack is a harp rack. Harp racks are racks with AWBAR_GESTELLE.TYP_KZ = 1. If the rack is not a harp rack, the SLOT_ID will be inserted into the field, beginning with 1 in the sequence in which the lites are booked.
ORDERER_ORDER_NO: The value for the order and the position of the lite is determined from the field POOL_TXT.TEXT with TEXT_TYP = 6009. If a data record for the position does not exist in table POOL_TXT with TEXT_TYP = 6009, a feedback file will not be created for this lite. If several data records exist with TEXT_TYP = 6009, the POOL_TXT.TEXT is determined for any one of these data records and written into the element ORDERER_ORDER_NO.
ORDERER_REFERENCE_ITEM_NO: Same as ORDERER_ORDER_NO, only that TEXT_TYP = 6010.
ORDERER_FIELD_NO: Same as ORDERER_ORDER_NO, only that TEXT_TYP = 6004.
ORDERER_PIECE_NO: The sum of POOL_POS.MENGE from all data records that belong to the AE_INTPOS of the lite. This means that the quantities of several items are summed up in the case an item-split.
Please note that a feedback is only created for lites where the text types 6009, 6010 and 6004 exist in the table POOL_TXT. The file is initially created with the extension "tmp" and renamed to "xml" after is has been written completely. The filename contains the timestamp. Errors that occur while writing the file are logged in AlcimBook.log.