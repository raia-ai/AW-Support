---
title: "EN-CONFIG-AW_Enterprise_EDI"
source: "EN-CONFIG-AW_Enterprise_EDI.pdf"
tags: ["A+W Enterprise", "EDI", "Configuration", "Software", "Glass Industry", "PO Transfer", "Order Linking", "Master Data Replication", "SAP Coupling", "System Integration"]
version: "1.0"
last_updated: "2025-10-08"
short_description: "This document provides comprehensive configuration instructions for the A+W Enterprise EDI (Electronic Data Interchange) software. It details the setup and management of various data exchange functions within a company, including master data replication, order processing, and system integration."
long_description: "The A+W Enterprise EDI configuration manual is a detailed technical guide for system administrators and planners responsible for setting up and maintaining data exchange processes in the A+W Enterprise software, which is tailored for the glass industry. The document covers a wide range of functionalities, including the replication of master data (articles, market partners, keys), the transfer of purchase orders (PO transfer) and sales orders (order linking), and the generation of invoices. It outlines the basic configuration prerequisites, such as setting up the 'xhaus' table for site management, defining directory structures, and configuring environment variables. A significant portion of the manual is dedicated to error research and troubleshooting, providing detailed status codes, problem descriptions, and remedies. It also explains the processes for purchase order generation, including configurations for pure trade sites, handling of delivery addresses, and document takeovers. The manual differentiates between internal PO transfers and external PO exports, and provides in-depth instructions for both. Furthermore, it covers advanced topics like status reporting from production clients, balance scheduling, external order interface/EDI import, and coupling with external systems like SAP Oxygen. The document is intended to ensure seamless, automated, and company-wide data communication between different branch offices or with external partners."
---

---
## Change history

| Date | Author | Comments | Version |
| :--- | :--- | :--- | :--- |
| 2018-02-15 | Ina Seifert | Initial version | 1.0 |
| 2019-02-18 | Alexander Weil | **6.8.19. Rabatte**<br>Wenn die Umgebungsvariable RABATTLOGIK_2005 aktiv ist, werden die Vorgangsrabatte innerhalb der Bestellübertragung NICHT übertragen. Im Empfangshaus werden für den Auftrag die Rabatte für den Kunden „Sendendes Haus“ neu aus den Stammdaten ermittelt. Der Endkunde des Auftrages wird dabei nicht ausgewertet.<br>Standortübergreifende BDE | 1.1 |
| 2019-06-12 | Alexander Weil | 6.8.5 SN-Datei Übertragung | 1.2 |
| 2019-12-17 | Alexander Weil | 6.8.5 SN-Datei Übertragung - Upgrade | 1.3 |
| 2020-01-28 | Ina Seifert | Product set transfer<br>Private fields retained | |
| 2020-06-23 | SVH | #422752-A+W EDI Export | |
| 2020-09-16 | Ina Seifert | E/Z rules for frame exchange | |
| 2020-12-15 | Ina Seifert | Extension of MP interface | |
| 2022-05-06 | Elena Tempelfeld | Format adjustment, receipt of goods section inserted | |
| 09.10.2023 | Ina Seifert | New message 95 | |
| 2024-07-16 | André Münch | Connection to Oxygen | |
| 2024-09-05 | SVH | [AW-169965] – PO export to A+W Business | |
| 2025-03-11 | André Münch | Oxygen Change for Purchase Order and Purchase Requisition | |

## 1. General

Frequently, there is a desire for a company-wide, central master data management, automatic order processing within a company with several branch offices, and automatic order scheduling for external orders.

A+W Enterprise provides special transfer functions that allow these various requirements to be fulfilled.

Central components of all transfer are the program trm_ctrl and the table xhaus, which includes all necessary information about the clients for data exchange.

Without trm_ctrl (but with the table xhaus), only the online master data replication and the goods receipt and invoice transfer work.

### 1.1. Overview of the supported transfer types

*   Master data replication (article, market partner, key, product sets)
*   Transfer of Orders and Purchase orders
*   Transfer of External purchase orders
*   Takeover of incoming goods and purchase invoices for existing orders
*   Reporting of order status values
*   Distribution of messages
*   Transfer of invoice data to external FinAc systems

### 1.2. PO transfer vs. PO export

What are the basic differences between internal PO transfer and PO export?

| Function/area | Internal PO transfer | PO export |
| :--- | :--- | :--- |
| **Article master data** | Must be identical between the two clients. Rudimentary evaluation of the replacement/addition rules | Different item master data |
| **Item referencing** | Does not take place | Takes place via customer article and replacement/addition rules |
| **Status reports** | Detailed status messages from the production site. | No status reports |
| **Local correction** | Configuration via DFUE_IB_BESTELLSPERRE | Configuration via BESTELLFREIGABE |
| **Program file** | trm_ctrl | Export: A+W B2B Service<br>Import: i000filter; trm_ctrl |

## 2. Basic configuration

### 2.1. Checklist

| | |
| :--- | :--- |
| **Housekeeping** | Individual script for cleaning up individual directories, especially also $DFUEDIR/proto/* |
| **Tabelle xhaus** | **Versions** check/set all clients.<br>**bytevektor** check/set all clients.<br>This must be set correctly in the sender and in the recipient. |
| **Directory structure** | $DFUEDIR<br>The subdirectory $DFUEDIR/proto/<Mandant> is important |
| **Market partner master data** | Type of the EDI/direct order |
| **Connection (FTP)** | It's important that alcibnet has the right for ftp on the xhaus.host of the other sites. |
| **PMSPURCHASETRIGGER** | Has to be set if this is purely a distributor. |

### 2.2. Table Xhaus

#### 2.2.1. General

In the table xhaus, data for all clients that communicate with one another via A+W Enterprise is saved.

xhaus can thus be called a site management table from which A+W Enterprise draws all data required for communication.

In all connected sites, the table xhaus must be maintained accordingly. Sites that are not entered in the table xhaus are not available to the system for automatic data exchange.

After each change to the table xhaus, the ue_server and the dfue_starter must be ended and started again.

Special attention must be paid to the correct creation of the fields kunr, linr, host, hausart, vers, subvers, and patch, as well as iboffset, bytevektor, and dfuedirpath since these have a central effect on order linking and PO transfer.

In all sites participating in the order linking and PO transfer, the table xhaus must be adjusted accordingly.

#### 2.2.2. Table structure

| No. | Table field | Description | Reference to remarks | from version |
| :--- | :--- | :--- | :--- | :--- |
| 1 | haus | Number of the site/sub-site | haus | < 4.0 |
| 2 | hnr | Number of the site/sub-site | hnr | < 4.0 |
| 3 | hname | Short name for the site | hname | < 4.0 |
| 4 | kunr | Customer number of the site | kunr | < 4.0 |
| 5 | linr | Supplier number of the site | linr | < 4.0 |
| 6 | host | Host name of the server | host | < 4.0 |
| 7 | hausart | Flag for evaluation of iboffset and environment variables | hausart | < 4.0 |
| 8 | vers | ALCIB Version | vers | < 4.0 |
| 9 | subvers | ALCIB Subversion | subvers | < 4.0 |
| 10 | patch | ALCIB Patch | patch | < 4.0 |
| 11 | dbart | Flag for replication | dbart | < 4.0 |
| 12 | region | Region affiliation | region | < 4.0 |
| 13 | socketmd | SOCKETMD from alenv | socketmd | < 4.0 |
| 14 | shmoffset | Shared memory offset of the site | | < 4.0 |
| 15 | servmaster | Name of the computer on which the server processes are running | | < 4.0 |
| 16 | netz | Network recognition | | < 4.0 |
| 17 | sprkz | Local language of the site | | < 4.0 |
| 18 | informixserver | Name of the Informix server | informixserver | < 4.0 |
| 19 | iboffset | Offset of the document numbers of the site | iboffset | < 4.0 |
| 20 | bytevekt | Byte vector flag | bytevekt | 4.0 |
| 21 | dfuedirpath | EDI directory of the site | dfuedirpath | 4.2 |
| 22 | hauptmandant | Client ID within the internal client separation | hauptmandant | 4.2 |
| 23 | clientlocale | Value of the CLIENT_LOCALE system variables of the site | clientlocale | 4.4 |
| 24 | vers_seqnr | AWE database version of the corresponding client | vers_seqnr | 6.0 |

#### 2.2.3. Field description

**haus**
Number corresponds to the system variables $HAUS (site)

**hnr**
At least since Version 4.0, haus and hnr are always assigned the same value (the site number). In older versions, these values can deviate from one another.

**hname**
Name of the site. This is displayed, among other things, on the title line of the A+W front end. In addition, it can be displayed in the subject line of system e-mails (ALMAIL_MANDANT_BETREFF) or for the establishment of the mail domain server (AWMAIL_XHAUS_DOMAIN).

**kunr**
The number corresponds to the customer number in the market partner master data. A site's customer number should be identical in all sites.

If a company has 3 branch offices in Berlin, Dresden, and Munich, the Berlin branch office should be kept with the same customer number in the Dresden branch office as in Munich. It is possible to deviate from this recommendation, but the result is more configuration and management work. (see environment variable IB_KUEMPF).

Depending on the configuration, this number is also used to determine the sender address for the form dispatch. See section "Determination of the sender address" in "EN-CONFIG-A+W Enterprise Print Service"

**linr**
The number corresponds to the supplier number in the market partner master data. A site's supplier number should be identical in all sites. The supplier number is used within the order coupling and the PO transfer as well as internal accounting and automatic goods receipt generation. In particular in the course of internal accounting, there can be problems if the supplier numbers are not unique company-wide.

QR 2406:
The supplier number is also used in the course of "XRechnung" to identify the seller. If you want to work with "XRechnung" but not with internal EDI, the supplier number can also be entered negative.
"XRechnung" see "EN-CONFIG-A+W Enterprise B2B Service"

**host**
Host name of the server on the network on which the site was installed and to which the transfer files should be sent.

**hausart**
For installations, the field is always assigned 10 or 11.
The difference between 10 and 11 lies in the evaluation of the field iboffset. With hausart=11, the field is not evaluated.
Site types between 0 and 10 are no longer supported and will cause errors.

**vers**
Version number (for example 4 in Version 4.3.2)
All version fields must be set correctly in all participating sites. E.g.
Site 1 and site 2 work with internal order transfer
Site 1 works with Version 4.5.1
Site 2 works with Version 6.0.4

In site 1:
In the xhaus record for site 1, vers=4;
In the xhaus record for site 2, vers=6;

In site 2:
In the xhaus record for site 1, vers=4;
In the xhaus record for site 2, vers=6;

**subvers**
Subversion (for example, 3 in Version 4.3.2)
All version fields must be set correctly in all participating sites. E.g.
Site 1 and site 2 work with internal order transfer
Site 1 works with Version 4.5.1
Site 2 works with Version 6.0.4

In site 1:
In the xhaus record for site 1, subvers=5;
In the xhaus record for site 2, subvers=0;

In site 2:
In the xhaus record for site 1, subvers=5;
In the xhaus record for site 2, subvers=0;

**patch**
Patch (for example, 2 in Version 4.3.2)
All version fields must be set correctly in all participating sites. E.g.
Site 1 and site 2 work with internal order transfer
Site 1 works with Version 4.5.1
Site 2 works with Version 6.0.4

In site 1:
In the xhaus record for site 1, patch=1;
In the xhaus record for site 2, patch=4;

In site 2:
In the xhaus record for site 1, patch=1;
In the xhaus record for site 2, patch=4;

**dbart**
ID for the master and client database for item, market partner, and key replication.
2 - Country or sub-master database for 2-stage master-client logic
1 - Master database
0 - Client database
-99 - Pseudo site (not a regular site)
- is required as price client for internal client separation starting with version AWE 6.
- is used as pseudo site for self-transfer (environment variable IBHAUS)
- Used as pseudo client for several call centers due to multilingualism (capacitative client assignment) - **work in process**
- For these sites, no background processes are started.
- One employee-client assignment is possible

The value "2" for sub-master only plays a role in the sub-master itself. It identifies for itself that dbart=2 is entered in its xhaus record.

Example:
The sites 70, 80, and 90 exist.
90 is master (for site 80)
80 is sub-master (for site 70)
70 is "only" client

xhaus entries in site 90:
*   haus 90, dbart 1
*   haus 80, dbart 0
*   haus70, dbart 0

xhaus entries in site 80:
*   haus 90, dbart 1
*   haus 80, dbart 2
*   haus70, dbart 0

xhaus entries in site 70:
*   haus 90, dbart 0
*   haus 80, dbart 1
*   haus70, dbart 0

**region**
The association of a site with a region is evaluated, e.g. in the FinAc interface.

**Socketmd**
The respective SOCKETMD of the client from alenv. Important for central number assignment.

**shmoffset**
Shared memory offset of the site

**Servmaster**
Name of the computer on which the server processes are running. Important for central number assignment.

**Netz**
Network detection

**sprkz**
Language ID (local language of the site)

**Informixserver**
Name of the database server on the net. This is required for the master data replication.
Order entry also uses this for the database access.

**iboffset**
If iboffset is greater than 0, then the new order number for documents that are sent by this site via order linking or order EDI is the document number sent plus iboffset.

**bytevekt**
If the site works with byte or bit vectors (1 - byte vector => environment variable BYTE_VEKTOR is set).

**dfuedirpath**
The value of $DFUEDIR for the corresponding site is set. If the field is not filled, it is assumed that the directory is identical with $DFUEDIR of the sender.
Important is the maintenance of this field if EDI should take place between Windows sites and UNIX sites or between 2 Windows sites on different installations. The path for the Windows sites must be entered in SFU notation.

**hauptmandant**
The field must be maintained due to the internal site logic.
If the value stored here is equal to hnr, it is a main site.
If the value stored here is not equal to hnr, but is greater than 0, it is an internal site whose main site is specified in this field.
The main site defines the database name (alcib_<hauptmandant>)
For pseudo sites (e.g., IBHAUS) for which no background processes, especially no ctrl_server must run, a 0 must be entered here.

See case 135188

All xhaus entries with the same main client will be updated accordingly with a QR update (version information). If there is something incorrect here (e.g, in preparation for a future move or because you just copied another record), it can happen that an internal EDI no longer works after a QR update.

A+W Enterprise 6: Apparently now for the Singlesite_Installations the main client must be set equal to the client number so that the order entry works.

**clientlocale**
The valid Informix client country setting must be saved for each site entered. With internal EDI, a code set conversion is done if necessary using this data.
In the new field clientlocale of the table xhaus, the CLIENT_LOCALE value of the appropriate site must be stored (upper and lower case plays no role).
If no value is stored for a site in xhaus.clientlocale, the EDI assumes that conversion should be to the code set ISO8859-1.
See case 168856

**vers_seqnr**
The EDI must know in the respective client which database structure exists in the site connected via EDI. Since database changes are no longer attached solely to the A+W Enterprise Version (fields vers,subvers, and patch), there is now another field vers_seqnr.
The seqnr of the last SQL file listed on the database is entered in this field. Therefore, it is important that the SQL scripts are always executed seamlessly in the correct sequence.
This information controls central functionalities within the internal document transfer.
The update routine tries to update these values for accordingly all relevant xhaus entries. For this, however, it is necessary that all databases be available to one another for SQL commands. If this is not the case, the update must be done manually after an update.

> **After each change to the table xhaus, the ue_master (or ue_server) and the dfue_starter must be ended and started again.**

### 2.3. Directory structure / required files

*   In the directory $DFUEDIR/ proto (e.g. /usr1/alcibnet/proto), there must be a subdirectory that has the same name as the site number (xhaus.haus) for each site participating in the transfer (also internal sites!). For single-digit site numbers, a 0 must be placed in front of the directory name (e.g. site 2 => directory $DFUEDIR/proto/02) This subdirectory must have write and read rights for the user alcibnet.
*   In the directories $DFUEDIR/dat (e.g. /usr1/alcibnet/dat) and $DFUEDIR/wait (e.g. /usr1/alcibnet/wait ) there must be one subdirectory per .testmount (the dot is important). Parallel to the directory $DFUEDIR/wait, there must also be a subdirectory $DFUEDIR/waitx. All directories must have write rights for the user alcibnet.
*   In the directory /usr1/alcibnet/bin there must be an appropriate file trm_ctrl_<mandantennummer> for each site participating in the transfer. This file must be created as a link to the file trm_ctrl_<haus>.
*   To enable a transfer between 2 servers, the file.netrc must have a corresponding entry for the user alcibnet in the directory /usr1/alcibnet.
*   In the directory $ALCIBPRG/cmd, there must be a script "FT". It must be possible to execute the script with the user alcibnet.
*   It must be possible to execute the system commands compress / uncompress, uuencode / uudecode and tar from alcibnet.
*   The database settings DBDATE and DBMONEY must be identical for all participating sites.

### 2.4. Master data

#### 2.4.1. Market partner

Within the market partner (xhaus.linr, xhaus.kunr) the field "Type of the EDI" and the field "Direct order" must be set accordingly.

Direct order "yes" means that the order is generated immediately and not via the order pool.

### 2.5. Environment variables

**DFUE_IB_BESTELLSPERRE (version 2007):**
The variable controls when internal POs go into local correction.
0 - print; 1 - send; 2 - receipt; 3 - scheduling; 4 - job created; 5 - job confirmed

**DFUE_IB_OWN_AHAM (client reference: no)**
For the internal DFUE it is assume that the item master data is identical in its essential properties. Therefore, the AHAM is transferred unchanged by default. To achieve that the local SR is used in the receiving site and the dependent data (spacer and muntin size) is recalculated, the variable must be activated. ID 134840
The logic works starting with Version 4.2 also for triple and quadruple IG, see case 204646.
This function may not be configured together with an MD_MIN_AHAM.

**DFUE_PROTO_NOBUFF**
Normally for performance reasons, the EDI logs are written buffered. This can mean that with crashes due to program errors, not all messages are found in the log. With the setting of these variables, all logs of the EDI are written unbuffered. For differentiated treatment, see DFUE_RESEARCH.

**DFUE_RESEARCH**
With these variables, various research modes of the trm_ctrl can be switched on. Up to 10 areas are separated by | (pipe). Currently available:

*   **trm_ctrl**
*   **ibout** - export of the data (also for PO generation) to the distributor
    - Protocol $DFUEDIR/proto/[<hausnr>/ibout>/]ibout*
*   **ibin** - storage of the data (also PO generation and external EDI)
    - Protocol $DFUEDIR/proto/[<hausnr>/ibin/]ibin*
*   **filter** - reading in of external interfaces via interface filter (external EDI)
    - Protocol $DFUEDIR/proto/[<hausnr>/edi/]<filter>*
*   **mp_replicate** - Market partner replication
    - Protocol $PROTOPFAD/MP_replic<mmdd> (in client)
*   **art_replicate** - Article replication
    - Protocol $PROTOPFAD/ArtReplik_replic<mmdd> (im Client)
*   **rechrueck** - report from financial accounting
    - Log $PROTOPFAD/Rechrueck_<mmdd>_<hhmm>
*   **rueck, mp, fibu, ibi_unl** - moves unload files of the _i-tables to $DFUEDIR/proto
*   **ibout_unl:** moves unload files of the _-tables to $DFUEDIR/proto/unl_ .res ATTENTION:
*   **ON:** extended recording for all EDI areas.

If this variable is set, the log for this area will be unbuffered (s.a. DFUE_PROTO_NOBUFF, REPLICATE_PROTO)

**DFUE_TRM_SIMULTAN**
Simultaneous trm_ctrl for external order scheduling and PO generation.

**IB_ALLOWIB (client reference: no)**
Allow orders to your own site via pseudo supplier. In addition, the environment variable IBHAUS has to be activated (see section "generating suborders")

**IB_DFUE_NACHBEARB (data transfer)**
From trm_ctrl, after booking an entry, a script is started with set variables. Here, another script can be called per order customer (kauf.kunr). The definition is stored in the table dfue_nachbearb. The script itself must be in $ALCIBPRG/cmd or $ALCIBPRG/spec/cmd.

Parameter: paknr, exaufnr, auftrnr, hausnr, parhausnr
Is overwritten for external order scheduling of EDI_SQL.

If with external EDI neither of the two variables is set but there is an entry in dfue_nachbearb, then the reprocessing is done.
Attention: see "Post-processing" section

**IB_EXREF (client reference: no)**
The variable influences the structure of kaufexaufnr (external reference) for the document transfer (NOT for order generation!)
0: exaufnr=auftrnr sender's order no (PO number for PO EDI)
1: exaufnr=bestnr the sender's PO number appears at the target site
2: exaufnr=auftrnr/bestnr both numbers appear at the target site
3: exaufnr=bestnr/auftrnr both numbers appear at the target site
4: exaufnr is transferred unchanged
> Caution: not set or 0 corresponds to the previous logic (see also PILK_51922)

**IB_EKVK_SHIFT**
For the internal order transfer, it is also possible by setting this variable that one of the price fields of the original order from poskost is written to kpos.dfuenstpreis and transferred. The name of the field to be used has to be entered in the variable; the only valid fields are "stkprs" and "stkprsfw." With entry of "nstpreis," kpost.nstpreis is written to kpos.dfuenstpreis and transferred.

**IBHAUS (client reference: no)**
Site number from xhaus for the internal pseudo suppliers for production suborders. The client number may not be the same as the own client number.
In addition, the environment variable IB_ALLOWIB has to be activated. (see section "Generating suborders")

**IB_KUEMPF:** must be set if the customer number of the distributor at the production site is not the same as the customer number that was entered in the xhaus entry for the production site at the distributor. With a set variable, when scheduling an order at the production site, used as customer number, default debtor and calculation debtor from the local xhaus entry. If the variable is not set the customer number sent from the distributor is used as customer number.

**IB_NOBESTINTBEST (client reference: no)**
For internal orders and in active ordering, since 2.7 except for the order in the receiving system, an order is also generated in the sending system. This is not always desired! (additional document, data, goods receipt, etc.) With this variable, the generation of the local order document can be switched off.

**IB_NO_IN_DOCUCHECK:** Within the order scheduling for PO transfer, documents to be transferred are copied from a temporary directory of the EDI on the document server. After that, the program checks whether all defined documents have arrived there. If a document is missing, the order is not released. If this variable is set, the check does not take place.

**IB_NO_OUT_DOCUCHECK:** Within the order scheduling for PO transfer, documents to be transferred are copied from the document server to a temporary directory of the EDI. After that, the program checks whether all defined documents for the PO are available in this directory. If a file is missing, the transfer is cancelled. If this variable is set, the check is not done.

**IB_XUSR (client reference: no)**
The employee who made the entry is retained by the EDI.
> Caution: the employee must be present in the target system!
> Caution: INTAUF_MANEU overrides these variables
Attention: In combination with IB_EUSR.
IB_EUSR for purchase orders, IB_XUSR: for orders (in the receiving site)

**IB_ZVERS (client reference: no)**
This variable is used to activate the order postponement to a test client. If this variable is set, the column intver in intbest is evaluated by trm_ctrl. Using the shell script "intver," orders for postponement can be placed in intbest.
Attention: No other activity should be booked to intbest!
The orders are registered in the target system with parhausnr+=100 so that no messages are sent to the sending system!
In addition, the orders in the target system are not transferred to intauf with still -1 (NEUKAUF), but rather with still -3 (TXT_KOMPL), which means that some functions (e.g. E/A rules, price calculation) will not take place during the import. (see section "Order shifting")

**INTAUF_ALTEK**
*   **active:** After an order transfer, the PU prices transmitted in advance in the sender are taken over in the recipient as SA prices
*   **inactive:** After an order transfer, the SA prices in the receiving site are determined anew
*   **x|y|z:** if site numbers are entered separated by | (pipe) for these sites in advance after an order transfer, the PU prices are taken over in the recipient as SA prices.
For all other sites, the prices are not taken over.

**INTAUF_CHECK_DFUE_RESTRIKT:** If this variable is set, for all incoming EDI orders (external and internal), there is a dimension restriction check. If an existing restriction is violated, then the order is not released, but placed in the release pool with an appropriate notation. In addition, an appropriate entry in the document notes is generated for the dimension restriction violated.
Processing restrictions (article dimensioning) are always checked.
Starting in July 2025: BOM restrictions will also be checked

**INTAUF_DFUE_WUNSCHLIEFERANT (client reference: no)**
For ext.DFÜ, the desired supplier is taken over (item) if a BA is of the type "PO".
Std logic: only if 1st procurement type is "PO"

**INTAUF_FREITEK:** This variable controls whether and which orders scheduled via EDI are released directly and which are put into the release pool.
*   **EXTERN:** The orders from external order input interfaces are not released directly, but rather placed in the release pool.
*   **INTERN:** The group-internal EDI orders (order linking and order transfer) are not released immediately, but rather placed in the release pool.
*   **ON :** All EDI orders are placed in the release pool

**IB_EUSR (client reference: no)**
If set, the eusr in kauf (user) is no longer set to -1 (System) for orders transferred. (ON, RELEASE, UNCHANGE, ORDER)
> Caution: then all employees have to be present everywhere on the network!
Attention: In combination with IB_XUSR.
IB_EUSR for purchase orders, IB_XUSR: for orders (in the receiving site)
> Caution: INTAUF_MANEU overrides these variables
Value RELEASE see AWDesk 198581, UNCHANGE #358345
\\jupiter\DOKU_DocuWare\ALCIB-PMS\DFUE\Bestellübertragung_Uebersicht.doc Note:
The variable BESTPOOL_INTERN must be deactivated, for the variable creates chaos with active BESTELLDFUE. BESTELLDFUE already includes the logic of collective POs for internal supplier via PO pool (see case 240821).

**INTAUF_BEARBCOPY_BA_HALTEN = ON:** If this switch is active, the processing steps marked as 'can be passed on' in master data will adopt the processing type from distribution instead of loading it from the production site's master data as for all other elements.

**INTAUF_VSGLM_BA_HALTEN=ON:** If this switch is active, the processing steps marked as 'can be passed on' in master data will adopt the processing type from distribution instead of loading it from the production site's master data as for all other elements.

**INTAUF_MANEU (client reference: no)**
If this variable is active, all EDI orders are assigned user -1 (that is the system service).
Otherwise, the user of the sending site is retained.
> Caution: this variable overrides the variables IB_EUSR and IB_XUSR

**INTAUF_LIEFERART (client reference: no)**
If variables are set, the delivery type is redrawn for internal EDI:
*   ON = for order generation at the production site and PO generation at the distributor
*   1 = Only for order generation at the production site
*   2 = For PO generation at the distributor

**INTAUF_VERPACKART (client reference: no)**
If the variable is set, with internal EDI, the packaging type is re-transmitted for rack planning):
*   ON = for order generation at the production site and PO generation at the distributor
*   1 = Only for order generation at the production site
*   2 = For PO generation at the distributor

**MD_MIN_AHAM (client reference: order)**
For the internal EDI it is assume that the item master data is identical in its essential properties. Therefore, the SR is transferred unchanged by default. Local production lines can require that a particular SR not be underrun. To achieve this, a minimal SR can be defined client-specifically.
This function may not be configured together with DFUE_IB_OWN_AHAM.

**PMSPURCHASETRIGGER (client reference: no)**
If ALCIB works with a different production system than PMS, PMS can continue to be used as an order switch, i.e. to trigger internal and external order proposals. In this case, however, no statuses, such as incoming goods messages, may be booked on the PMS side. The order blocking may only be carried out from ALCIB or the other production system. Requirements for the background process - with the exception of order scheduling - are therefore ignored when variables are active, and feedback messages are prevented as far as possible.

### 2.6. Housekeeping

Under the stipulation that the external and internal EDI can run in parallel in principle and that the attached files can be used several times, the scheduling process cannot clean up the incoming directory and the intermediate directories for additional files. This has to be done in a housekeeping script that runs at night. The script has to check whether scheduling is still open (table ialf_jobctrl.status != 30). If there is no more scheduling to be processed, then the incoming directory and the directory /usr1/alcibnet/dat/EDI/<dfuetyp> can be cleaned up.

Status in ialf_aufctrl and ialf_jobctrl
*   10 - Order generated for job
*   20 - Order complete, but not the whole job
*   30 - Order and job complete
*   40 - Order will be processed by trm_ctrl
*   50 - aufnr was assigned in ibin
*   300 - Error in the interface
*   310 - Error in the interface, but nevertheless processed by trm_ctrl
*   320 - Error in exbin()
*   330 - Error in ibin()
*   340 - Error in filter post-processing

## 3. Error research

### 3.1. Reports

The DFÜ reports are primarily in $DFUEDIR/proto. Depending on the configuration, in this directory there are subdirectories for the individual clients installed on the server ($DFUEDIR/proto/<xhaus.hnr>). In the precise client directory, there are, in turn, thematic subdirectories
global, edi, ibin, ibout, exbin, edi_misc.
Environment variable: DFUE_TRM_SIMULTAN, DFUE_JOBCTRL

**QR22/02**
Since A+W Enterprise release 6 December 2019, the master data replication can log in its own tables and generate from this a log e-mail for the end user (#377851 // [AW-7851]). With the further expansion of this function in other modules of the EDI, it became necessary that in addition to the log tables dfue_protokopf and dfue_protodetail, there must also be back-up tables and a function to delete old data.

When the process to be logged is done and the e-mail for the end user was generated, the relevant records (key: dfue_protokopf.id) is pushed out of the tables dfue_protokopf and dfue_protodetail to dfue_protokopfok and dfue_protodetailok. There, they are still available for searches. However, it can happen in these tables that the original key dfue_protokopf.id is no longer unique.

Old data records can be deleted from the *ok tables with the normal A+W Enterprise deletion function for unreferenced records. By default, the records are deleted after 365 days. This deadline can be defined with the environment variable DFUE_PROTOTAB_INTERVAL.

*   If the environment variable is not active, the deletion deadline is 365 days.
*   If in the environment variable a value less than zero is entered, the data will never be deleted.
*   If in the environment variable a value between 0 and 14 is entered, the deletion deadline is 14 days.
*   If in the environment variable a value greater than 14 is entered, the deletion deadline is this number of days.

#### 3.1.1. Article replication

The log `$PROTOPFAD/ArtReplik<mmdd>` writes the article replication. The logging is done in English. The logging level can be switched with the environment variable `DFUE_RESEARCH=art_replicate` to an expanded mode, a so-called developer mode. The log is written buffered by default. If the expanded log is switched on, then it is written unbuffered. If you would like the default protocol to be written unbuffered as well, then the environment variable `DFUE_PROTO_NOBUFF` has to be set.

#### 3.1.2. Market partner replication

The log `$PROTOPFAD//MP_replic<mmdd>` writes the market partner replication. The logging level can be switched with the environment variable `DFUE_RESEARCH=mp_replicate` to an expanded mode, a so-called developer mode.

#### 3.1.3. Key replication

The key replication writes a log to `$PROTOPFAD/Key_replic_<date>_<time>`. If the environment variable `REPLICATE_PROTO` is set, an expanded logging can be switched on.

### 3.2. Research options

In the reports, especially the document transfer, errors are marked with the keyword "ERROR" and warnings with the keyword "WARNING." If a possible error cause and remedy are known, appropriate instructions are provided with the keyword "HELP."

With the environment variable `DFUE_RESEARCH`, it is possible to place the individual logs on a higher degree of detail (see "Environment variables").

The system can be configured so that a special error is generated. This is primarily intended for tests within development.

**DFUE_ARISE_ERROR (client reference: no)**
If this variable is set and has a value greater than 0, an error is provoked at a particular point in the EDI.

1 - after converting the aufnr in * tables (ibout)
100 - end kauf_insertgroup (ibin);
101 - after insert into aufint (ibin)
102 - after script call in dfue_nachbearb (ibin)
103 - all the way at the end (ibin)
104 - simulation of active MODUL_STAPELLOGIK (ibin and ibout)

#### 3.2.1. Status in the table intbest

The error status of the EDI is entered in the table intbest in the field sendeseq:
Positive values in the sendeseq field mean that the document has already been sent, however the receiving site has not sent confirmation of the receipt.

The procedures specified here for eliminating a problem currently represent the best knowledge as recommendation and do not absolve you of the obligation to prior research and weigh all possible consequences (especially in case of data manipulations).

| Error status | Cause | Remedy |
| :--- | :--- | :--- |
| 0 | New entry | Please check whether the EDI was started (process: dfue_startert $HAUS). If the process is not running, it can be started with 'starterstart'.<br>For additional notes, see the logs $DFUEDIR/ueber_err$HAUS and $DFUEDIR/proto/ibout_proto$HAUS. |
| -1 | Entry is being processed | This is a temporary state when the EDI begins to process a dataset. If this state should last longer, it must be checked whether a process trm_ctrl 10 ...$HAUS ... is running. If this is the case, it must be checked in the log $DFUEDIR/proto/ibout_proto$HAUS why and where the process is hanging. It is possible that the process must be ended.<br>If no abovementioned process is running, the sendeseq can be reset to 0. Here it must be heeded that no doubled records arise in the table. Key on this table is "kaufnr, gruppe, poskonr, posnr, tupnr, sendeseq, storno". |
| -2 | There can be several causes of this error. The EDI classifies the various errors as temporary errors (e.g. locking of an order by an employee) | For the precise cause, see the log $DFUEDIR/proto/ibout_proto$HAUS. If the following line is in the ibout log, then you have to check the ibin log for the cause.<br>`called ibin(pknr,-2,dest) for purchase order! (rc=-2)`<br>`23.03 17:18:28: ERROR -2 in create PO/Enquiries (ibin)`<br>With each start of the EDI, there is an attempt to re-process these records. Starting the EDI can be forced with the script pmptrmctrlstart. |
| -3 (only with BESTELLDFUE) | Error during update of the sendeseq to 0 by the report ekueb.rep | Only for BESTELLDFÜ: The error cause could be in REPERROR or in the file that was generated from the form printing during file printing.<br>After checking the data, either delete entries from intbest and transfer the purchase order again via Purchasing - Form printing or set sendeseq = 0 (WARNING: Here you must heed that no doubled records arise in the table. Key on this table is "kaufnr, gruppe, poskonr,posnr, tupnr, sendeseq, storno") |
| -15 | IO_LOAD_ERROR: An error occurred when loading the data in the receiving site | For the more precise cause, see the log $DFUEDIR/proto/ibin_proto$HAUS.<br>Up to version 2007:<br>`e.g. insert_ikuaz fehlgeschlagen SC=-206, CISAM=-111`<br>`Load from_tables: SC=-206`<br>=> generation of the parallel tables _kuaz and _ikuaz from the regular table kuaz mittels ',alias_temp kuaz'<br>WARNING: This may only be done if no EDI order and no order generation is being processed by intauf.<br>Starting with Version 2007, the tables are generated dynamically in the program. |
| -1007 | MASTERDATA_ERROR: Items are contained in the sent document that are not included in the master data at the receiving site. | Create master data at the receiving site or adjust document at the sending site. Can also be informed about messageID 68 |
| -1100 | Select on kpos produces error | For the precise cause, see the log $DFUEDIR/proto/ibout_proto$HAUS (older versions < 3.2 $DFUEDIR/ueber.err).<br>"ERROR: SC 100 CISAM 0 during search item!" there is another aufnr in intbest.internr than in kpos for the document. The cause can be that a PO was re-generated before the transfer. This should have been caught, except ...<br>If necessary more precise examination of how the data inconsistency occurred is required.<br>Solution: remove intbest entry and set document again. |
| -2002 | IO_NOT_FOUND_ERROR at the sender. Required data was not found for export. | For the precise cause, see the Log ibout_proto* (older versions < 3.2 $DFUEDIR/ueber.err).<br>Previously occurred causes: In the order, special items were entered that require additional data. Therefore, the field kpos.gvkz!=0. However, the relevant item of the corresponding record does not exist in the table kposgv. It must be examined how the order was entered or has been changed in order to determine the cause of the missing record within the order entry.<br>If necessary, the relevant item must be re-entered.<br>Remove the order from the table intbest and after the correction, it is provided anew by the system for transfer. |
| -2003 | Database error when exporting an order | Please check in the Log ibout_proto<haus> which error is the one in question (table, error number). Using the error number listed there, the corresponding causes must be researched and measures taken to eliminate these (e.g. data correction for SC = -284; adjustment of the database structure with SC = -217; order correction with SC=100 (expected files are missing)) |
| -2020 | Different suppliers for the same group/PO number | A PO in the PO pool was generated with different suppliers. This should actually not be possible. In case of this error, message 47 is sent. Please ask the user how he generated the PO. How is BESTPOOL_GRUPPIEREN set? |
| | Different number of records to be processed | sendeseq=0 is still in intbest, but -2020 is in the ibout* log. Get data from intbest (2 rows copied) ... `ERROR (-2020): Intbest fetch (1) > count (1)` ... `==> !! EXIT !!`. Checks the field intever; it must be between 0 and 4. Is the variable IB_ZVERS set? If so, see section "Order shifting" |
| -2025 | Error when accessing files or writing files | FOPEN_ERROR, that is,<br>- the log file for status exchange between the clients could not be written. The file is written to $DFUEDIR/dat<br>- or the packing of the sn files did not work<br>- or the packing of attached files or ...<br>without ibout log, you will not find the precise cause. |
| -2028 | Purchase order not yet released or already transferred. | Check whether the purchase order is already in the status "local correction - ordered" or in the status "local correction - transferred". If the status "ordered" does not yet exist or if the status is already "transferred", a transfer of the purchase order is not possible. Please correct the status of the purchase order. For this case, the message No. 46 can be sent.<br>Please check the setting `DFUE_IB_BESTELLSPERRE`. |
| -2029 | Starting with QR 2406 – incorrect transfer type | If the supplier is VKKopplung, but a PO is provided for transfer |
| | Missing delivery date (field intbest.termin) | **Attention:** Delete the relevant record from intbest and possibly bestpool and re-do the date calculation in the PMS. Or set a known date in the table intbest. |
| -2030 | For purchase order transfer, sender≠recipient | Check the data and configuration. See also #447449<br>NO_LAGERBEST is probably not set and internal order transfer configured. Why is NO_LAGERBEST not set. Why do you need the PO. The recommended workflow is to generate only a stock-filling order without PO and then to trigger the incoming stock booking via the packed message from production. |
| -2040 | During the order scheduling, it is checked whether all item and BOM articles also exist in the article master data | The status is transmitted back during the order transfer to the distributor as status -1007 |
| -2041 | Address not present | The delivery address of the retail order no longer exists in the master data. Please correct the order. |
| -2042 | Doubled records in awc_bestetikett | To eliminate the problem, it must be clarified with production which labels/glass should actually be ordered in which quantities. Then the data must be corrected/deleted in the tables "awc_bestetikett", "intbest", and if necessary, "bestpool".<br>Should not happen anymore starting with "A+W Enterprise 6 Export Service - 13.4.12027" (June 2025) |
| -2050 | General SN file FTP transfer error. | Please check ibin log.<br>Possible causes:<br>- No FTP active on the Windows computer Please check the ftp connection with the user alcibnet manually<br>- Is the Windows computer correctly on the .netrc of the user's alcibnet. On the .netrc, it has to be precisely as in the environment variable `DFUE_DATEI_REF_PFAD` or `DATEI_REF_PFAD` (including or excluding domain specification)<br>- FTP log in `/tmp/ftp*`<br>- It has to be heeded that in the `DFUE_DATEI_REF_PFAD` variables, `/` instead of `\` are to be used for the path specification. |
| -2051 | Check failed, whether SN file is present in the article master data for transfer. | Please check ibin log.<br>A fixed subpart should be ordered. In the article master data (master data - article - F4 - article dimensions), no valid SN file is entered or the copying of the SN file failed<br>Possible causes:<br>- No FTP active on the Windows computer Please check the ftp connection with the user alcibnet manually<br>- Is the Windows computer correctly on the .netrc of the user's alcibnet. On the .netrc, it has to be precisely as in the environment variable `DFUE_DATEI_REF_PFAD` or `DATEI_REF_PFAD` (including or excluding domain specification)<br>- FTP log in `/tmp/ftp*`<br>- It has to be heeded that in the `DFUE_DATEI_REF_PFAD` variables, `/` instead of `\` are to be used for the path specification. |
| -2052 | Copying the SN files via FTP failed | Please check ibin log.<br>Possible causes:<br>- No FTP active on the Windows computer Please check the ftp connection with the user alcibnet manually.<br>- FTP log in `/tmp/ftp*`<br>- Is the Windows computer correctly on the .netrc of the user's alcibnet. On the .netrc, it has to be precisely as in the environment variable `DFUE_DATEI_REF_PFAD` or `DATEI_REF_PFAD` (including or excluding domain specification)<br>- It has to be heeded that in the `DFUE_DATEI_REF_PFAD` variables, `/` instead of `\` are to be used for the path specification. |
| -2053 | Check failed, whether file is present for transfer. | Please check ibout-log and `copy_docu_files*`.<br>Start transfer with `DFUE_RESEARCH=ibout`. Then a lot of the ftp connection is also written in `/tmp/ftp*`.<br>Possible causes:<br>- No FTP active on the Windows computer Please check the ftp connection with the user alcibnet manually<br>In the ftp log, there is an attempt to open the connection with the USER "bin". FTP log in `/tmp/ftp*`.<br>Possible cause<br>- Is the Windows computer correctly on the .netrc of the user's alcibnet. On the .netrc, it has to be precisely as in the environment variable `DFUE_DATEI_REF_PFAD` or `DATEI_REF_PFAD` (including or excluding domain specification)<br>- It has to be heeded that in the `DFUE_DATEI_REF_PFAD` variables, `/` instead of `\` are to be used for the path specification.<br>For research also the log |
| -2701 | During the purchase order generation it was determined that more than one purchase order exists for an order and a supplier, split | The purchase order generation tries to change an existing purchase order for the order and supplier. If, however, there are already several purchase orders for an order and supplier, the system can no longer decide which purchase order may be changed. Here, manual intervention is necessary (e.g. cancellation of existing purchase orders) |
| -9000 | Provoked errors within the program | Deactivate environment variable `DFUE_ARISE_ERROR`. |

#### 3.2.2. -2041: Missing shipping address

[AW-109920]: trm_ctrl - 13.04.9110 // 05.2023
If a PO is generated and/or transferred for an order with an invalid shipping address the generation of the new document is interrupted with the temporary error -2 and the system tries again later. This could cause a high number of error e-mails and a high system load. Therefore, this error is now set to its own, new error status -2041.

In this case, the shipping address in the order and/or in the market partner must be corrected. Then the error status can be reset in the table "intbest" and the generation/transfer started again (pmptrmctrlstart).

### 3.3. Additional problems and their possible cause(s)

| Problem | Cause | Remedy |
| :--- | :--- | :--- |
| The send purchase orders remain in the table intbest with sendeseq = 0. | The dfue_starter of the relevant site is not running (check with the command: "ps -ef \| grep dfue_starter" or "ps -ef \| grep alcibnet") | Check in the directory $LOCKDIR whether a file starterlock$HAUS is present. If this file is present, but the corresponding dfue_starter is not running, this file must be deleted.<br>If the dfue_starter is not running, it must be started with the command "starterstart" in the environment of the affected site.<br>Log: $DFUEDIR/proto/start_proto<$HAUS> |
| The send orders remain in the table intbest with sendeseq = 0, although the corresponding dfue_starter is running | The directory $DFUEDIR/wait contains too many files. | The processing files for the dfue_starter are in the directory $DFUEDIR/wait. The files to be processed end with .r$HAUS. All files can be deleted that are older than one day and only end with the ending .$HAUS. The content of the .r$HAUS files must be checked. Of the files that can only call trm_ctrl_* <Parameterlist>, all files but for one with an identical parameter list can be deleted.<br>For all other files, an individual case check in cooperation with the customer is required. |
| The records for PO generation remain in intbest with positive sendeseq. No PO is generated | No *.r<hausnr> file is generated in $DFUEDIR/wait, but rather a file *.rh or *.rp | In the table xhaus, the hausart has a value less than 10. In addition, the environment variable(s) DFUE_DBTYP_* are activated.<br>The xhaus. hausart< 10 is no longer supported. Please update the hausart in xhaus to 10 or 11 and restart the ue_server and the dfue_starter |
| Error -206 in loadext() in ibin_proto<haus> | An absolutely necessary table does not exist | A _ and/or _i table is missing. (only up to Version < 2007)<br>In the script $ALCIBPRG/install/cmd/prep_dfuetabs (älter prep_ibtabs) all tables are listed for which the underscore tables must exist. In case of doubt, this script must be updated at the customer with the one from Linden.<br>After that, the script or an alias_temp <Table> can be executed. Here, attention must be paid that there is an OK next to each "create ...".<br>WARNING: This may only be done if no EDI order and no purchase order generation is being processed by intauf since the intermediate files are deleted (drop tables)<br>Starting in Version 2007, the - and i-tables are generated dynamically as TEMP tables and they are no longer present after ending of the trm_ctrl. |
| The transfer works, but the table intbest will not be emptied in the sending site. | Error in uudecode | Install Uudecode on a computer where it works. |
| The entries from the table intbest for generating a purchase order disappear, however no purchase orders are generated | The environment variable IB_MKBEST is not set. | There are only entries in $DFUEDIR/proto/ibout_proto<$HAUS>, however none in ibin_proto<$HAUS>.<br>In the extended log mode (DFUE_RESEARCH=ibout), the variable definitions are at the beginning:<br>`: ** IB_GRUPPE using groups during processing: NO`<br>`: ** IB_MKBEST create purchase orders: NO` |
| After saving the purchase orders from the order pool, these are not processed automatically although the dfue_starter is running | No start file *.r<$HAUS> nach $DFUEDIR/wait is written | The environment variable PMPTRMCTRLSTART contains the script for the automatic start of the trm_ctrl. In general, the script is also called pmptrmctrlstart.<br>PMPTRMCTRLSTART=“pmptrmctrlstart" |
| After generation of an order at the sending site, no purchase order/work plan is generated | The order was not released automatically (kauf.tekapkz=0) | **INTAUF_CHECK_DFUE_RESTRIKT:** If this variable is set, there is a restriction check for all incoming EDI orders (external and internal). If an existing restriction is violated, then the order is not released, but placed in the release pool with an appropriate notation. In addition, an appropriate entry in the document notes is generated for the restriction violated.<br>**INTAUF_FREITEK:** This variable controls whether and which orders scheduled via EDI are released directly and which are put into the release pool. |
| A transferred order cannot be processed at the receiving site. The information is in the ibin log that the file with the name <xxx> could not be found/opened | Different logic for generation of file names. | Check DFUE_PAKID_HOSTBASE. The value of the variables must be identical in the sending and receiving sites. |
| A transferred document cannot be processed at the receiving site. The information is in the ibin log that the load has failed.Log intbest Einlagern (kposp) LOAD fehlgeschlagen Error Code: -1 | Data structure and structure of the load file to not fit together. | The version information in the respective data records of the table xhaus must be checked. These must be consistent in the sender AND in the recipient (xhaus) In particular, the field vers_seqnr hast to be correct for all participants.<br>Site A orders in site B. Thus, in site B the data record for site A has to be identical to the data record of site A in site A. |
| SC=0 CISAM=0,ERRM:><br>A change transmission does not result in a change of the order at the production site even though it is not in local correction. The message 55 fx_texte 23030: "Caution: order %d=%d from site %d change failed - already released!" is sent | The status delivery planning exists | In the EDI, this status must be checked since her no question can be posed as in the foreground. |

### 3.4. Checking the transfer

All PO generations and document transfers to another site (internal EDI) will be written to the table intbest and processed there by the trm_ctrl.

For this, various State flags are written to the table in the course of the processing. In addition, messages are sent for successful and/or faulty processing. Which messages are sent to whom can be configured (see section "Messages")

In the application, you can use the menu element "System - Data Transfer - Document Transfer - Check Transfer" to view the faulty and successful transfers.

When the dialog opens, a selection menu appears:
a) **Orders whose transfer is in progress**
All transfers are displayed here that have a positive send sequence. This means that the transfer was made, but the recipient has not yet sent confirmation of the receipt.

b) **Orders with faulty transfer**
All transfers are displayed here that have a send sequence less than -2. This means that an error occurred during the transfer. The send sequence specifies which error occurred. (see section "Status in the table intbest")

c) **Orders that have not yet been transferred**
All transfers are displayed here that have not been started yet.

d) **Transferred orders**
All transfers are displayed here that are in the table "intbestok". This means that the transfer was processed successfully.

## 4. Purchase order generation

Within an order, it can be decided using the supply type of an item or a BOM part whether this part should be ordered. After the order has been scheduled and analyzed by the production system, order proposals are created according to the master data and configurations.

The order proposals are ALWAYS created by the production system!
For clients with own production, the order proposals are created by A+W Production.

### 4.1. Pure trade site

If an A+W Enterprise site is a pure trade site without its own production, the PMS production system can function as an order gate. For this, the environment variable `PMSPURCHASETRIGGER` has to be activated. This variable can only be activated globally. This process is also called "PMS0".

With use of an internal client separation, it is now possible for individual clients (trade operations) to have the orders created via the ALCIB order gate. For this, for the appropriate clients the environment variables `ORDERXML` and `AWC_ALCIM_ANBINDUNG` have to be deactivated and the environment variable `PMSPURCHASETRIGGER` has to be global.

The environment variable `MODUL_PROD_SPAETE_AENDERUNGEN` may not normally be active. Since this can be necessary for other clients of a multi-site system, however, starting with build pms - 13.04.8431, this no longer disturbs the processing in the retail clients.

#### 4.1.1. Postponement

If within A+W Enterprise the order gates (without connection to A+W Production) were used, previously the delivery date of an order was not shifted if the delivery date of the PO was before the delivery date of the order.

Within the order gates, the delivery date is calculated for an order including customer and supplier handling time. If the incoming goods date calculated this way is later than the delivery date of the order, now with appropriate configuration, the delivery date of the order is shifted to the next possible delivery date.

#375089: environment variable for the order `PMEKAUF` and in dispatch `PMEMELDTERMINVER`

#### 4.1.2. Special checking of the environment variables

| | | |
| :--- | :--- | :--- |
| **PMSPURCHASETRIGGER (client reference: no)** | ON | Has to be active for pure trade sites (without AWC connection) |
| **MODUL_KOSTENKALK** | 2 | May absolutely not be 3. Is not evaluated client-specifically |
| **PMEINLASTUNG** | disable | |
| **PMEINLASTUNGNEU** | disable | Not "OFF" und enable =1 but rather enable=0, otherwise no update of the shipping date in kauf |
| **PMPGLASALL** | disable | PF [AW-138928] |
| **PMXAWPOOL** | disable | |
| **PMQCIMIN** | disable | |
| **PMPHPOSANZ** | disable | |
| **PMETERM** | check | 4, otherwise no update of the shipping date in kauf |
| **PMPGLASALL** | disable | |
| **ORDERXML** | disable | Can also be deactivated for multisite client-specific. |
| **AWC_ALCIM_ANBINDUNG** | disable | Can also be deactivated for multisite client-specific. |
| **PMEKAUF** | check | Writes new date back to the order (only if PMETERM=4 and PMEINLASTUNGNEU is deactivated (enable=0)) |
| **PMEMELDTERMINVER** | check | |
| **PMEGESCHART** | Check | May be necessary if for drop shipments no handling time should be considered. |
| **PMPBESTTERMIN** | Check | May be necessary if for drop shipments no handling time should be considered. |
| **PMELTPLANMAXDIFF** | Check | |
| **PMENEXTTOURTERMIN** | Check | |
| **PMHSLEEΡΤΙΜΕ** | 5 | Was on 30 for AGC. Causes with a lock via the NR_Server, so that it waits this number of seconds before it tries to set the lock again. |

#### 4.1.3. Logs

The process PMS is used for the date calculation. The logs are largely written in Alcib language.

**PMEPROTOBASIS (client reference: no)**
Detail degree of the log generation in the general service functions in the scheduling area (rough scheduling).
0 = no messages at all
1 = only report errors
2 = normal user log
3 = expanded log for development
4 = excessive log with all messages

**PMEPROTOBAUM (client reference: no)**
Detail degree of the log generation in the tree management functions in the scheduling area (rough scheduling).
0 = no messages at all
1 = only report errors
2 = normal user log
3 = expanded log for development
4 = excessive log with all messages

**PMEPROTODASCH (client reference: no)**
Degree of detail of log generation in the functions surrounding the date determination (date and shift) in the scheduling.
0 = no messages at all
1 = only report errors
2 = normal user log
3 = expanded log for development
4 = excessive log with all messages

**PMEPROTOENTRY (client reference: no)**
Detail degree of the log generation in the general external service functions in the rough scheduling area.
0 = no messages at all
1 = only report errors
2 = normal user log
3 = expanded log for development
4 = excessive log with all messages

**PMEPROTOVGZ (client reference: no)**
Detail degree of the log generation in the general functions default time calculation in the rough scheduling.
0 = no messages at all
1 = only report errors
2 = normal user log
3 = expanded log for development
4 = excessive log with all messages

**PMHTESTLEVEL (client reference: user)**
The variable contains the test level for a test message log for the background process PMS. This corresponds to the test protocol in the foreground when you type "ESC f t". In the foreground the test level is queried.
The test messages are written to the file "<Process-ID>.test". This is located in the folder that can be reached with "gft" from a UNIX shell.
A test level 3 generates a message each time a function is entered or exited. A test level of 9 (maximum) also generates a message for each event.

### 4.2. Environment variables

| | | |
| :--- | :--- | :--- |
| **RAHMEN_BESTELLUNG_GLASMASS (client reference: no)** | check | For active A+W Production, replaces the variable PMFZKRAHMENAHAM, which was evaluated by PMS. When ordering spacers/grids/muntins, data is calculated according to glass dimensions. |
| **PMSPURCHASETRIGGER (client reference: no)** | ON | Has to be active for pure trade sites (without AWC connection) |
| **EK_REKLAMATION** | check | **EK_REKLAMATION (client reference: no)**<br>A complaint order does not automatically result in a complaints PO. If this environment variable is active, old logic is reactivated, that is, a complaint orders creates a complaint PO. This only applies to Purchasing without prior grouping in the purchase order pool. |
| **DFUE_IB_ADDITIONALGRP** | check | **Client reference: no**<br>If POs are generated without the PO pool, parts to be ordered are combined per order, supplier, and delivery type.<br>If this variable is activated, the "splitcode" field for the grouping is also evaluated. The "splitcode" field in the table intbest is populated individually by the SP "cu_pogetsplitcode". The SP is called by the ERP Webservice.<br>See "EN-CONFIG-A+W Enterprise EDI" [AW-157565] |

### 4.3. Configuration Options

The definition of the individual settings is made under
`System > Data Transfer > Transfer Document > Configuration`
Or in the market partner master data via the "EDI configuration" menu or F5 on the field "Type of EDI."

With "Type of EDI" - 102 "PO generation," currently the following settings are possible:

| Control type | Name | Description |
| :--- | :--- | :--- |
| 4 | Local Notification | If there is a notification for a PO, but the PO is not in local correction and this PO is corrected via order change, the notification's data is retained. Otherwise it is deleted. The control type is created for the supplier for which the PO is generated. Precise specification: ID 126756 |

### 4.4. PO grouping for direct orders

[AW-157565] // March 2024

If POs are generated without the PO pool, parts to be ordered are combined per order, supplier, and delivery type. If this grouping is not sufficient, but you don't want to work with the PO pool, there is now an additional customer-specific grouping criterion.

The function is activated with an environment variable. In addition, there must be a stored procedure "cu_pogetsplitcode". This SP receives the parameter `<Auftragsnummer (kauf.auftrnr)>`, `<Vorgang (5)>`, `<Stücklistennummer (kpos.poskonr)>`, `<interne Positionsnummer (kpos.posnr)>`, `<Stücklistenelement (aufstrukt.tnr)>`, `<Lieferant (aufstrukt.linr)>` and returns a 2-digit character string as additional grouping criterion.

For this, the tables "awc_bestproto", "intbest" and "intbestok" were expanded to include the field "splitcode". The "splitcode" is the additional grouping criterion. Via the SP mentioned above, the "splitcode" field is populated in the table "intbest" and "awc_bestproto" (return value of the SP). It is taken over in the PO, but it is not visible there.

> **It is mandatory that the splitcode for an order part is always identical; otherwise PO changes cannot be made correctly.**

This function is only supported for direct POs (ID in the supplier master data).

If within the internal EDI you are working with order coupling, this function cannot be used.

If within the internal EDI you are working with this function, it must be activated for all participating clients. However, it is possible that the SP returns no (or an empty) splitcode for the parts to be ordered.

The function cannot be used if you are using one-type documents (article group) with the function.

`DFUE_IB_ADDITIONALGRP=ON`

Cannot be used if `PRODTYP_TEST` is active.

### 4.5. Delivery Address

#### 4.5.1. No direct shipment

If this is not a direct shipment, the delivery address in the PO is determined according to the following sequence:

*   Default delivery address of the supplier of the PO
*   Default delivery address of the sending site
*   Invoice address of the sending site
    => This way, there is no PO without delivery address!
The delivery address from the order is taken over in the end customer address.

If one of the addresses should be cancelled, this cancellation code is not considered within PO generation. If a cancelled address is in an existing order, then it is also taken over into the PO and a resulting order.

#### 4.5.2. Direct shipment

If in the order there is a delivery address, the delivery address is taken over into the PO.

If the order contains no explicit delivery address, the delivery address in the PO is determined according to the following sequence:

-   Default delivery address of the supplier of the PO
-   Default delivery address of the sending site
-   Invoice address of the sending site
    => This way, there is no PO without delivery address!

If one of the addresses should be cancelled, this cancellation code is not considered within PO generation. If a cancelled address is in an existing order, then it is also taken over into the PO and a resulting order.

### 4.6. Document takeover

[AW-66053] - Release April AWE 6

Within the order entry, it is possible to attach files manually on the order and item level. However, these files were not taken over into an order-related PO.

With the current version of A+W Enterprise, you can define both in the master data (Master Data - Keys - System - Dokumententypen) as well as in the order entry on the "Document assignment" dialog that a document should be taken over into the PO. To do this, you need to place a checkmark in the "Best" field. If the checkmark is already set in the master data for the document type, this is taken over into the order; however it can also be changed there.

