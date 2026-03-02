---
description: "EN-CONFIG-AW_Enterprise_Internal_Client_Separation"
---


---
## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2018-02-15 | Ina Seifert | Initial version | 1.0 |
| 2018-10-18 | Ina Seifert | Extension MP SITE EXACT | |
| 2019-03-20 | Elena Tempelfeld | Takeover of plant/RN for internal client separation | |
| 2019-08-03 | Alexander Weil | Environment variables parallel EDI import | |
| 2020-02-14 | Elena Tempelfeld | Global/local rights overview | |
| 2020-04-09 | Tobias Schierhuber | Extension of master data - installation restrictions | |
| 2022-09-26 | Ina Seifert | Multilingual operation - employees (Beta) | |

## Content

- **1. Notes on this Document**
- **2. Introduction**
    - 2.1. Checklist for the introduction/configuration of a multi-client system
- **3. System Configuration**
    - 3.1. Server
    - 3.2. Number ranges
        - 3.2.1. Site-specific number ranges (MP_SITE_EXACT)
    - 3.3. Configuration File
    - 3.4. Table xhaus
    - 3.5. Directory structure / required files
    - 3.6. Call Center // External Order Interface
    - 3.7. Scripts
    - 3.8. Status reporting (ID 135061-> rueckmeld)
    - 3.9. Messages
    - 3.10. Environment variables
    - 3.11. Error handling
        - 3.11.1. Error with nr_server
        - 3.11.2. PO generation does not start automatically
        - 3.11.3. Incorrect client in the mail subject
- **4. Multilingual operation – employees (Beta)**
    - 4.1. Introduction
        - 4.1.1. Checklist in start-up
    - 4.2. Master data
        - 4.2.1. Tax types
        - 4.2.2. Notes
        - 4.2.3. Article master data
        - 4.2.4. Article dimensioning
        - 4.2.5. Order entry
        - 4.2.6. Site change
        - 4.2.7. System
        - 4.2.8. Output
        - 4.2.9. Research help
- **5. A+W Enterprise Master Data**
    - 5.1. Master data at the dealer's
    - 5.2. Master data at production site
    - 5.3. Master data in stock
    - 5.4. Companies (MP_SITE_EXACT #333097)
    - 5.5. Key
        - 5.5.1. Due date conditions
    - 5.6. Product groups (#334944)
    - 5.7. Market partner master data
        - 5.7.1. Routes
        - 5.7.2. Limit check
        - 5.7.3. Client-specific data (MODUL_INTERNE_MANDANTENTRENNUNG)
        - 5.7.4. Client assignment MP_SITE_EXACT (#334703)
        - 5.7.5. Company assignment MP_SITE_EXACT (#333097)
    - 5.8. Item master data
        - 5.8.1. MP_SITE_EXACT (#331647)
    - 5.9. Employees / user rights
        - 5.9.1. MP_SITE_EXACT (#332946)
    - 5.10. Client-related company calendar
- **6. Texts**
- **7. Prices (MP SITE EXACT # 333913)**
    - 7.1. Requirements and configuration
        - 7.1.1. System / environment
        - 7.1.2. Employee master data
        - 7.1.3. Market partner master data
        - 7.1.4. Price master data
        - 7.1.5. Terms
        - 7.1.6. Evaluation in document entry
- **8. Sales**
    - 8.1. Limit check
    - 8.2. Transaction data
    - 8.3. Client-specific release pool
    - 8.4. Order corrections after successful client allocation
    - 8.5. Change of client allocation
    - 8.6. Company change in the order after transfer to AWP
    - 8.7. Reference
        - 8.7.1. Site assignment
    - 8.8. Expansion of the automatic invoice creation
    - 8.9. New supply type "not available"
    - 8.10. Document search via site number
    - 8.11. Total surface for objects
- **9. Call center solution**
    - 9.1. Configuration
    - 9.2. Initial version
    - 9.3. Manual PU price
    - 9.4. Supplier determination after client assignment
    - 9.5. Client-specific change of order after successful allocation
    - 9.6. Reference to an allocated order
    - 9.7. Failed allocation
    - 9.8. Total surface for objects
- **10. Purchase**
    - 10.1. Extension in PO pool
    - 10.2. Rack-related incoming goods
- **11. Information systems**
- **12. PMS/AWP**
- **13. Dispatch control**
    - 13.1. Interim goal for dispatch
- **14. A+W Enterprise - Barcoding**
- **15. Replications**
    - 15.1. Master data transfer (old master data replication)
    - 15.2. Key tables (old key replication)
    - 15.3. Item transfer (old item replication)
    - 15.4. Table distribution
    - 15.5. External Market Partner Interface
    - 15.6. External EDI
- **16. Corporation Statistics**
- **17. FinAc data**
    - 17.1. Transaction data for financial accounting
    - 17.2. Internal charging
    - 17.3. FinAc transfer of debtor data
    - 17.4. Vendors
    - 17.5. FinAc totals
    - 17.6. Transfer of cost centers
- **18. Message transfer**
    - 18.1. System message distribution
- **19. Construction site invoicing**
- **20. Racks**
    - 20.1. Rack transfer
    - 20.2. Rack (block transfer)
    - 20.3. Rack comparison
    - 20.4. Rack distribution
- **21. Project Information**
- **22. Distinction (Production - Distribution)**
- **23. Barcode Data**
- **24. Via plant / ViaPlant**
    - 24.1. Master Data
        - 24.1.1. Reg. No
        - 24.1.2. Route maintenance in master data
        - 24.1.3. Market partner master data
    - 24.2. Order Processing
        - 24.2.1. Determining the route for an order
        - 24.2.2. Shipment "via site" ("via plant")
        - 24.2.3. Calculation of the route date when shipping "via site"
        - 24.2.4. Changing the route and end route in the order
    - 24.3. Dispatch control
        - 24.3.1. Via site logic / Via plant
        - 24.3.2. Finished products stock
        - 24.3.3. Complex example
    - 24.1. Environment variables

## 1. Notes on this Document

> **Caution:** this documentation is not complete documentation of the entire variance of the configuration. It is only an A+W internal aid.
>
> In addition, use the current function description for this module.

There are two stages of expansion for the internal client separation. The second stage of expansion is activated with the environment variables `MP_SITE_EXACT`. Expansions that are only available in the second stage of expansion are marked with these variables.

10/18/2018: All expansions in this document have not yet been taken over. The main adjustments have been made via the project #343274 and can be seen in the appropriate release notes.

**Open**
- Statistics #334408
- List / Reports #334410
- Status reports #334475 / #349332
- Production transfer #334558 / 345567

## 2. Introduction

The internal multi-client system can handle several clients on one database. This has the following advantages:

1.  All internal clients use the same master data. No replication is necessary for adaptation. Client-related differences from the standard such as the supply type can be handled by means of new dialogs.
2.  A call center solution is possible. This means, all orders of the client system are entered for a call center client and are allocated to clients in the system by means of a "freely" defined logic. Allocation is followed by the automatic conversion of the client-related order data.
3.  A "rescheduling" of an order is easily transferred to another client by manually changing the client allocation at order entry.
4.  In such a system, it is possible to create reports and other analyses for all clients. Especially for sub-orders placed with another, internal client, you can determine e.g. PDC status information from the end customer order.

### 2.1. Checklist for the introduction/configuration of a multi-client system

This checklist serves to help make decisions about what kind of internal client separation and which basic configuration should be introduced. For the actual configuration, be sure to follow the section "System configuration – environment variables."

When planning the introduction of "internal client separation," you must absolutely pay attention that the main client is taken over first into the internal client separation. The main client is defined as the client that defines the database name.

| Function | Configuration | Note |
| :--- | :--- | :--- |
| Should different legal units (companies) be mapped? | `MP_SITE_EXACT` | Wide-ranging effects |
| Client-specific access rights for employees | `MP_SITE_EXACT` | |
| Are the main processes of the individual client identical? Or was it checked that the deviations can be configured client-specifically? | See this documentation and if necessary the documentation of the environment variables | |
| If an intermediate delivery via various production locations is required (ViaPlant) | `MODUL_INTERNE_MANDANTENTRENNUNG` | No `MP_SITE_EXACT` required |
| Do the clients have different local languages? | `MODUL_INTERNE_MANDANTENTRENNUNG_SPRACHE` | No `MP_SITE_EXACT` required |
| Do all clients have the same condition and prices for the same customers? | `MP_SITE_EXACT` | |
| How should the number ranges be created? Is it necessary to set these depending on the client? | Please consult the A+W Enterprise development manager | - Should a client change be possible for orders after the fact?<br>- If only invoices and credits should be separated MD-specifically, you should work with the determination of the invoice or credit number range per SP. |
| Are there operations that function only as trade client without AWP? | `PMSPURCHASETRIGGER` | |
| Is there a single system currency? | | Different currencies per client cannot currently be mapped. |
| Is the FinAc interface identical for all clients? | `FIBU_MANDANTENTRENNUNG` | FinAc interfaces must be adjusted individually if necessary |
| How should the limit check be done | `LIMITS_MANDANTENTRENNUNG` (Master data, Order entry) | |
| Should work be done with a central call center and an automatic distribution of the orders | `CALLCENTER` | |
| If a master data replication is also necessary | | Can only happen on the main clients.<br>No replication of client-specific data |
| Should the external market partner interface be used | `DFUE_MPDFUE_MANDANT` <br> **ATTENTION:** Only in exceptional cases for a short transitional period!! | This is only possible for the main client. The main client must be on the same computer (xhaus.host) |
| If within the internal EDI you are working with order coupling, this function cannot be used. | | This is not possible. It must be converted to order transfer. |

## 3. System Configuration

### 3.1. Server

All servers (`nr_server`, `ue_server`, `zu_server`) run just once on the main client. Other background processes (`ctrl_server`, `dfue_starter`, `rserv` etc) run per client (see "Scripts" section). For this, the corresponding entries must be made for the ports in `/etc/services`.

### 3.2. Number ranges

The number ranges are only evaluated for the main client and must therefore only be maintained for it.

With case #112491, a possibility was created for managing number ranges for invoices and credits in site-dependent fashion (independent of `SITE_DEPENDENT_NUMBERRANGES`)

Because this function is not a special function for internal site separation, it is documented in the document "EN-CONFIG-A+W Enterprise" - section "NR server".

If you are working with Callcenter, you may NOT work with this function for orders.

If you are working with this function, the site assignment can no longer be changed after the fact!

#### 3.2.1. Site-specific number ranges (MP_SITE_EXACT)

With case #334563, an enhancement was made in Version AWE 6. It is now possible to store particular number ranges client-specifically within the process entry. For this, the use of an internal client system is necessary in A+W Enterprise. Via a new dialog, it is possible with such systems to define different order number ranges for each client separately. If for one of the clients no separate number range is required, then the configuration for this client can be omitted. In this case, the associated number is pulled from the number range of the main client.

> **CAUTION:** The access key to the associated database tables was not changed. This means, during the configuration you must heed that the client-specific and global number ranges do not overlap.

This program logic is also bracketed via the switch `SITE_DEPENDENT_NUMBERRANGES`. If this switch is not active, then no client-specific numbers can be determined.

The following number ranges can be stored client-specifically:

- Quotations (angbex.mfo)
- Orders (kaufex.mfo)
- Invoices (rechex.mfo)
- Credits (gutsex.mfo)
- Supplier inquiries (anfrex.mfo)
- Purchase orders (baufex.mfo/bestex.mfo)
- Purchasing invoices (rechek.mfo)
- Purchasing credits (gutsek.mfo)

The number range dialog (System > Number ranges) serves to manage the client-specific number ranges. In order to be able to enter this dialog, the switch mentioned above (`SITE_DEPENDENT_NUMBERRANGES`) must be set to ON. Similarly, the switch `SITE_DEPENDENT_NUMBERRANGES_USER` is filled with the number of the employee who may use this dialog. To be noted is that the employee numbers must be stored separated with commas (e.g. 123,25,12). Last but not least, the employee right "SYNR" must be set for the employee in question in the employee management.

If this function is used, it is not possible to enter a process with reference to a process of another client and to retain the client number of the reference process. This means that if you are logged into client 1 and you refer to a process from client 2, the new process is created in client 1.

See also "EN-CONFIG A+W Enterprise" - NR server

### 3.3. Configuration File

In the file `/alcib/config/mandant.cfg`, all internal clients must be listed (for EDI environment establishment). Normally JG makes the adjustments to this file.

Parameters: `<Site> <$ALCIBPRG> <$INFORMIXDIR> <Instance> <FixVersion>`

Caution: for Pilkington (NSG), the file has a different path (e.g. `alcib***/config`)

### 3.4. Table xhaus

In all clients participating in the EDI, the table xhaus must be adjusted accordingly.

| Field | Description |
| :--- | :--- |
| `hnr` | Number of the client (in newer installations, haus and hnr are identical) |
| `kunr` | Customer number of the client in the market partner master data – **must be adjusted and possibly created in the master data** |
| `linr` | Supplier number of the client in the market partner master data – **must be adjusted and possibly created in the master data** |
| `kk` | |
| `hauptmandant` | is only evaluated for dbart!= -99 <br> `= hnr` - Main client <br> `!= hnr AND >0` internal client, the number is the number of the main client <br> `= 0` - external client (ID 135188) |

The table `xhaus` has been expanded to include the field `hauptmandant`.

This field is significant for internal client separation. It includes the site number of the client that corresponds to the main client within the internal client separation, that is, the client to which the database belongs.

The settings are as follows:

**Within the internal client separation: (here e.g. clients 42 and 142)**

- **Main client: `xhaus.hauptmandant = xhaus.hnr`**
    - e.g. client 42 => database name => alcib_42
    - `xhaus.hnr` = 42
    - `xhaus.hauptmandant` = 42

- **internal client: `xhaus.hauptmandant = xhaus.hnr` of main client**
    - e.g. client 142 => database name => alcib_42
    - `xhaus.hnr` = 142
    - `xhaus.hauptmandant` = 42

- **external client: `xhaus.hauptmandant = 0`**
    - e.g. client 242 => database name => alcib_242
    - `xhaus.hnr` = 242
    - `xhaus.hauptmandant` = 0

**Within an external client separation (here e.g. client 242)**

- **Main client: `xhaus.hauptmandant = xhaus.hnr`**
    - e.g. client 242 => database name => alcib_242
    - `xhaus.hnr` = 242
    - `xhaus.hauptmandant` = 242

- **internal client: `xhaus.hauptmandant = 0`**
    - e.g. client 142 => database name => alcib_42
    - `xhaus.hnr` = 142
    - `xhaus.hauptmandant` = 0

- **external client: `xhaus.hauptmandant = 0`**
    - e.g. client 42 => database name => alcib_42
    - `xhaus.hnr` = 42
    - `xhaus.hauptmandant` = 0

> **CAUTION:** if you are already working with internal client separation, you have to set the value for the field manually within the internal client separation after installation of the version !!

After each change to the table `xhaus`, the `ue_master` (or `ue_server`) and the `dfue_starter` must be ended and started again.

### 3.5. Directory structure / required files

In the directory `$DFUEDIR/proto` (e.g. `/usr1/alcibnet/proto`), there must be a subdirectory that has the same name as the client number (`xhaus.haus`) for each (!) client participating in the transfer (also internal clients!). For single-digit client numbers, a 0 must be placed in front of the directory name (e.g. site 2 => directory `$DFUEDIR/proto/02`). This subdirectory must have write and read rights for the user alcibnet.

In the directory `/usr1/alcibnet/bin` there must be an appropriate file `trm_ctrl_<mandantennummer>` for each client participating in the transfer (also internal clients!). This file must be created as a link to the file `trm_ctrl_<haus>`.

Per internal client, there must be a subdirectory in `$DBPATHEXT/proto`. If you are working with an A+W Production connection and ERP Webservice, there must also be a subdirectory for the main client for the alrpc process.

Per internal client, there must be a directory according to the A+W Enterprise env variable `IPCDIR`.

### 3.6. Call Center // External Order Interface

If the external order interface is used, it is absolutely necessary that call center (-> env variable) and main client match. (up to Version 2011 `trm_ctrl` build 1106 (ID 248261) => see next paragraph).

The variable `CALLCENTER_SP_ART` controls which SP is used for client determination. If this SP refers to the value 1, then an SP called `getproductionsite($kaufauftrnr)` (starting with Version 2012 additional parameter `$vorgang`) is called; it must return the following values:

- `sp_sql_haus` - assigned client (client)
- `sp_sql_frei` - 1 = release order, 0 = do not release
- `sp_sql_text` - "release note" (maximum 30 characters) is only taken over if order receipt via EDI (kauf.eingang = 4 or 14)

Starting with 2011 `trm_ctrl` build 1106 (ID 248261) it applies that:
- If `CALLCENTER` is defined, then scheduling only in `CALLCENTER`
- If `CALLCENTER` not defined, then scheduling on main client.
- Reason: most of the filters cannot run in parallel. Therefore, restriction to one client.

Starting with AWE 6 `trm_ctrl` build 13.04.2121 default interface i000filter build 13.04.2095 (ID 428675), external orders can be scheduled directly on an internal client if parallel processing is configured.

If you are working with the following interfaces in the appropriate versions, the configuration can be converted to parallel processing. In this case, scheduling can be done into each site directly. For this, the `trm_ctrl` in the Startscript must be called with the appropriate client number (see DE-CONFIG A+W Enterprise EDI)

| No | Filter | Parallel |
| :--- | :--- | :--- |
| 1 | `i000filter` | starting with 4.5 (2011) |
| 2 | `iskafilter` | starting with 4.3 (2008.2) |
| 3 | `iverfilter` | starting with 4.3 (2008.2) |
| 4 | `iegofilter` | starting with 13.0 (AWE 6) |
| 5 | `ifenfilter` | starting with 13.0 (AWE 6) |
| 6 | `ihuefilter` | starting with 13.0 (AWE 6) |
| 7 | `ivelfilter` | starting with 13.0 (AWE 6) |
| 8 | `iwirfilter` | starting with 13.0 (AWE 6) |
| 9 | `itelfilter` | starting with 13.0 (AWE 6) |
| 10 | `ikerfilter` | starting with 13.0 (AWE 6) |
| 11 | `iwinfilter` | starting with 13.0 (AWE 6) |

### 3.7. Scripts

In `$ALCIBPRG/spec`, the files `<mandant>_dfue_user`, `<mandant>_specs` and `<mandant>_user` must exist for all internal clients.

In the file `*_spects`, an adjustment must be made for the internal client analogous to the following:

```
case "${DBTYP}" in
[567][0-9][0-9])
    HPTHAUS=`expr ${DBTYP} % 100`
    DBNAME=alcib_${HPTHAUS}
    DBPATHEXT=/alcibdat/${HPTHAUS}
    IPCDIR=${DBPATHEXT}/ipc/${HAUS}
    DBTEMP=/alcib/dbtmp/${HPTHAUS}
    unset HPTHAUS
```

- `starterstart [<haus>]`: Starts the `dfue_starter` for the specified client. If no parameter is transferred, it is started for all clients for which in xhaus the `hauptmandant =$HAUS`.
- `starterstop [<haus>]`: Stops the `dfue_starter` for the specified client. If no parameter is transferred, it is stopped for all clients for which in xhaus the `hauptmandant =$HAUS`.
- `pmptrmctrlstart [<haus>]`: makes an entry according to `$DFUEDIR/wait` for the specified client for the start of the internal EDI. If no client is specified, the entry for `$HAUS` is created.

### 3.8. Status reporting (ID 135061-> rueckmeld)

The status reporting is started per client. However, true parallel operation is not implemented. During the configuration of the calls, attention must be paid to an appropriate time offset. Within the status reporting, it is ensured that with parallel start there is no data garbage (locking).

> **Caution:** with internal client separation, the rueckmeld script for the subclients cannot be started simply by hand from the shell, for it refers to the environment (that is the main client):

The status reporting is normally done via crontab entries. Attention must be paid that with internal client separation, the script must absolutely be called with 3 parameters.
`01,11,21,31,41,51 7-21 * * * /usr1/alcibnet/bin/rueckmeld 21 21 21`

### 3.9. Messages

You should absolutely work with e-mail and not with the A+W Enterprise internal reporting system.

Furthermore, the variable `ALMAIL_MANDANT_BETREFF` must absolutely be set so that you can see from which internal client a system message comes.

### 3.10. Environment variables

Environment variables are listed here that are important for the functioning of the internal client separation. In principle it applies that variables that are not listed here cannot be set client-specifically. For information about whether or not an environment variable can be set client-specifically, see the documentation of the variable itself (alenv.haus). Nevertheless, selected environment variables that cannot/may not be set client-specifically are listed here with appropriate commentary (e.g. MODUL_WAEHRUNG).

| Variable | Description |
| :--- | :--- |
| `DBTYP` | must be set in alenv client-specifically to the client (important for EDI). |
| `IBHAUS` | Disable. Check!! May not be set to an internal client number since otherwise the EDI will not work (see also `IB_ALLOWIB`). |
| `IB_ALLOWIB` | Disable. Check!! Should no longer be required in cooperation with AWP. s.a. `IBHAUS`. May not be set with internal client separation and configured `bestelldfü`. |
| `ALMAIL_MANDANT_BETREFF` | for system messages from internal clients. |
| `MODIFY_KAUFPARAUFTRNR` | ALT: must be set if you are working with purchase orders and EDI orders within the internal client separation. |
| `MODUL_INTERNE_MANDANTENTRENNUNG` | must be set to ON. |
| `CALLCENTER` | must be assigned the client number of the callcenter. |
| `CALLCENTER_SP_ART` | 1 use new client assignment logic. |
| `CALLCENTER_SP_DIRECTDELIV` | Number of parameters that must be transferred in addition to the keys `aufnr`, `posnr`. Currently implemented is 6: `getDirectSupplier(kpos.aufnr, kpos.posnr, default supplier (kpos.liefnr), kpos.artnr, postal code of the delivery address (kauf.lplz), kfzcode of the delivery address (kauf.lkfzcode), previous supplier, new client number)`. #99857 // [AW-147936] |
| `SOCKETMD` | must be set to the client number per internal client (not `$HAUS`, but rather the actual number). **Important:** so that the XX_server processes can be addressed correctly, an entry with `alenv.haus=0` must exist for the main client with the `SOCKETMD` of the main client (not `$HAUS`). If `SOCKETMD` sits on `$HAUS`, the processes that are assigned to a subclient establish no connect to `zu_server` or `nr_server`. |
| `IPCDIR` | must be set to the value `"${DBPATHEXT}/ipc/<Mandantennummer>"` per internal client whereby `$DBPATHEXT` should be entered resolved here. |
| `PROTOPFAD` | must be set to the value `"${DBPATHEXT}/proto/<Mandantennummer>"` per internal client whereby `$DBPATHEXT` should be entered resolved here and then must absolutely begin with `'/'`! |
| `PMXCOMM` | set to `"${DBPATHEXT}/xopt/<Mandantenummer"`. |
| `BESTELLDFUE` | With configured Bestelldfü, this variable must also be set (is evaluated by pms and in the kauf area). |
| `AWC_PORT_CONTROL_SERVER` | This variable must be set precisely for the site and there must be an entry with `alenv.haus=0` for the main client with the values for the main clients. |
| `AWC_PORT_RPC_DIENST` | This variable must be set precisely for the site and there must be an entry with `alenv.haus=0` for the main client with the values for the main clients. If the variable is not set client-specifically, the incorrect alrpc process of the ERPWebservice will be contacted. |
| `AWC_URL_PPS_WEBSERVICE` | This variable must be set precisely for the site. |
| `AWC_URL_PRODUKTIONSBERICHT` | This variable must be set precisely for the site. |
| `ORDERXML` | This variable must be set precisely for the site and there must be an entry with `alenv.haus=0` for the main client. |
| `FIBU_MANDANTENTRENNUNG` | Required if FinAc data should be transferred client-specifically. **CAUTION:** requires development adjustment #391254. |
| `MP_SITE_EXACT` | Controls the expanded internal client separation. This includes the client-site assignment and the expanded client-employee rights, as well as the client-market partner assignment. It applies system-wide! |
| `LIMITS_MANDANTENTRENNUNG` | #388239 allows a client-individual limit check. |
| `MODUL_WAEHRUNG` | The system and company currency can only be set database-wide. Therefore, it is absolutely necessary that all sites within the internal client separation work with the same company currency. |
| `PRICE_MASTER_HOUSE` | In this variable, the client number of the so-called "Price master clients" is entered. This client must have the `dbart=-99` in the table xhaus. By setting this variable, the logic is activated for Local and global price lists. |
| `DFUE_TRM_SIMULTAN` | This variable enables simultaneous `trm_ctrl` for external order saving. For further information please read the following configuration instruction: EN-CONFIG-A+W Enterprise EDI.docx. |
| `DFUE_JOBCTRL` | With an activated variable, the parallel execution of several filters is possible. For further information please read the following configuration instruction: EN-CONFIG-A+W Enterprise EDI.docx. |
| `DATEI_REF_PFAD` | Basic path for file attachments in document and notif, macro, and other master data files. For the file attachments in the document, the variable on May 2020 is evaluated client-specifically. For the master data, there must be an entry with `alenv.haus=0` for the main client. **CAUTION:** if the variable is changed from global to local after the fact, existing file attachments must be shifted independently to the new base path. |
| `DFUE_DATEI_REF_PFAD` | Analogous to `DATEI_REF_PFAD` for internal PO transfer and external order transfer. |
| `INTAUF_KALKKUNR` | If within the expanded internal site separation you are working with different condition debtors, this environment variable has to be enabled so that the price calculation determines the correct conditions during the internal PO transmission. |
| `INVOICE_IMPORT_FORALL` | If no site number is entered for the data import (invoices), then all data from the sites is retrieved where the user VORE=W. |

### 3.11. Error handling

#### 3.11.1. Error with nr_server

**Problem:** When starting the A+W Enterprise front end and also within the background processes (e.g. `intauf`), there are errors during the connect or starting of the number server (`nr_server`).

**Solution:** checking of the environment variables `SOCKETMD` (System configuration - environment variables)

#### 3.11.2. PO generation does not start automatically

**Problem:** if POs are written directly by the ERPWebservice to the table `intbest`, they remain there and are not processed. If you call a `pmptrmctrlstart <haus>` manually, then the records are processed without a problem.

**Research:** the order is not in the alrpc log of client 1, but in the log of client 2.

**Solution:** checking of the environment variables `AWC_PORT_RPC_DIENST`

`AWC_PORT_RPC_DIENST` - This variable must be set precisely for the site and there must be an entry with `alenv.haus=0` for the main client with the values for the main clients. If the variable is not set client-specifically, the incorrect alrpc process of the ERPWebservice will be contacted.

#### 3.11.3. Incorrect client in the mail subject

**Problem:** The environment variable `ALMAIL_MANDANT_BETREFF` is active. An order is entered in client 1 and released. However, the user receives the mail from site 2 that the delivery date of the order was shifted.

**Research:** the order is not in the alrpc log of client 1, but in the log of client 2.

**Solution:** checking of the environment variables `AWC_PORT_RPC_DIENST`

`AWC_PORT_RPC_DIENST` - This variable must be set precisely for the site and there must be an entry with `alenv.haus=0` for the main client with the values for the main clients. If the variable is not set client-specifically, the incorrect alrpc process of the ERPWebservice will be contacted.

## 4. Multilingual operation – employees (Beta)

### 4.1. Introduction

QR 22/09

Since this upgrade is an extensive system upgrade, this function may currently only be activated in consultation with your A+W planner and deployed on test systems. Deployment in productive sites is currently not approved.

This module enables several sites with different languages to map an internal site system for the employees.

In the new table "alsysinfomd" the respective languages for the sites are set. This is done during the activation of the functionality directly on the database.

For this, different front-end links per language and in the employee master data as login site one site with the appropriate local language must be assigned. All menu elements and most field names will now be displayed in this language. Thanks to a global setting in the current database connection, it is achieved that selection functions for multilingua key tables are also displayed in the language of the employee's login site.

There are a few pieces of language-dependent data that are assigned depending on the login sites. In addition, there are additional language-dependent data, such as the texts in the order, which depend on the site assignment of the order and the customer's language. They must always be generated in the language of the order since these texts are also transmitted to production and printed on customer papers.

#### 4.1.1. Checklist in start-up

- Import complete current QR
- Checking of CUSTOMIZING, EDI, Adhoc_SQL and Reports
    - E.g. selos that depend on configurable fields must exist in all language environments (artcomfld.selo, mpcomfld.selo, kflddef.selo) `$ALCIBPRG/cust/...`
    - On reports, check if necessary from which tables the data comes, e.g. is the country name in mp.land in the language of the employee who last saved it. The respective correct name is in xland (in the correct environment) or xsprbez.
    - Check `$DFUEDIR/bin/trm_ctrl*` for `$ALCIBPRG`
- Master data maintenance (keys, article master, employee master, etc.)
- Configure sites in alsysinfomd
- Create front-end links per language
- `$AWROOT/config/mandant.cfg`: the language environment must be entered here per site
- For this, there are the following scripts under `$ALCIBPRG/install/xsql/cust/sy`:
    - `alsysinfo.sql` - conversion of alsysinfo to a view on alsysinfomd
    - `updlangspecviews.sql` - script for new creation of all views with respect to the updlangspec logic
    - `xsprbezviews.sql` - script for new creation of all views with respect to the xpsrbez logic
- Activate environment variable `MODUL_INTERNE_MANDANTENTRENNUNG_SPRACHE`
- Restart server

### 4.2. Master data

In order to guarantee this function in as many places as possible, additional master data must be maintained language-specifically in addition to the already familiar language-dependent master data.

- Master data - Department
- Master data - cost master data (cost types, cost units, cost centers)
- Notes (article, market partner, process)
- Master data - Article - Article dimensioning (parameters)
- Master data - Keys - Market partner - Bonus
- Master data - Keys - Market partner - Process discounts - Discount methods
- Master data - Keys - System - Dispatch - Routes
- Master data - Keys - System - Dispatch - Packaging types
- Master data - Keys - System - Dispatch - Delivery types
- Master data - Keys - System - Currency
- Master Data - Keys - System - Taxes (Tax Types)
- Logistics - Rack management - Rack types

If key data is not maintained in the respective user language (this also applies for existing language-dependent data), then the user will not have these displayed with a search (e.g. Selo F9).

This does not yet include all data available in the system. If relevant data is still missing, this is converted on request insofar as this is possible.

**26/09/2022: Not yet converted keys (not complete):**

- Language
- Document types
- Vehicles
- Exit customs office
- Customs office of destination
- Dispatch groups
- Bending strength (technical values)
- Declaration of performance (documents)
- Production types
- Patterns
- Prices (vectors, price lists, etc.)
- Product sets
- Configurable fields
- Report management (report name and parameters)
- Adhoc_Sql
- Printer
- Individual programs (parameters)
- Stockroom
- Forms and lists
- Text Formulas
- Logical PC grouping (terminal)
- Packing BOM
- Machine (display in the cost calculation, no maintenance dialog available)
- Work processes (display in the cost calculation, no maintenance dialog available)

#### 4.2.1. Tax types

It must be checked that all tax types as key (tax type) > 0 since key = 0 is no longer allowed for the default logic. If from the past a tax type=0 exists, it must be adjusted to the new type in the master data and in the active processes. Only the key number must be adapted. Another calculation is not necessary.

If the external market partner interface is used, then an appropriate adjustment when writing the interface must be made here.

In case of questions, please contact A+W Service.

The conversion can be done before the start-up of the new login. Affected are the following tables and fields:

| Table | Field | Description |
| :--- | :--- | :--- |
| xkukz | kukz | key table => xsprbez.id2 where tab='xkukz' |
| kauf | kukz | Processes => Reference to xkukz.kukz |
| mp | mwst | Market partner master data => reference to xkukz.kukz |
| mpmdzu | mwst | Market partner master data => reference to xkukz.kukz |
| xmwst | kukz | VAT rates => reference to xkukz.kukz |

With these fields, the concern is NOT the VAT tax rate. This is saved in a separate field and therefore does not have to be adjusted.

#### 4.2.2. Notes

All notes for master data (market partner, article, employee) can now be entered in multiple languages.

If an employee enters a document for a market partner for whom a note is present, but not in the language of the active site, then the employee is asked whether he would like to see the note in the other language.
"There are important notes stored, however in a different language. Would you like to see these?". If the question is answered with yes, the note is displayed. Otherwise not.

Document notes cannot be entered language-dependently.

#### 4.2.3. Article master data

The texts for the article names (main description, etc.) must be present in all site languages ("Master data - Article - F4 - Other names"). If the translations are not present, no data will be displayed in the article search, for example.

#### 4.2.4. Article dimensioning

The texts for the processing parameters must absolutely be present in all site languages ("Master data - Article - F4 - Dimensioning article dimensioning - 'Texts'''). If the translations are not present, no field labels will be displayed in the document entry on the dialog for processing parameters.

#### 4.2.5. Order entry

If an order is obtained from another language site for viewing, then the data on the document header level (country, packaging type, delivery type, etc.), footer (discount names), and also on the item level (article name for product and BOM element, packaging type, etc.) will be displayed in the language of the login site. If the site is left this way in the order, then the texts for the existing items will not be regenerated on loading.

If an order is obtained from a site with another language for viewing and the site changes to the site number of the login site, then the data will be visualized as described above. In addition, the texts will be regenerated for the existing item. Here, it is considered which language is the customer language in the order (customer papers) and the language of the new site for the production papers.

If a new document is entered as reference to a document for a site in another language, then the data is obtained and a question posed, in which site the new order should be placed. If the new order should remain at the third-party site, then the data will only be visualized. If the new order should remain on the login site, then the data will be visualized and the texts re-generated.

If the environment variable `MODUL_INTERNE_MANDANTENTRENNUNG_SPRACHE` is enabled, for discount records that come from the discount master data, the discount name may not be overwritten. In the order, the discount name is displayed in the client language. If a change of the name is required in an individual case, the discount must be disabled and there must be a new manual discount with the new discount name in the customer language. Manually entered discounts must absolutely be entered with a discount text in the customer language. The forms on which discount texts are printed must be adapted accordingly.

#### 4.2.6. Site change

If via the menu element "Site change" on the "System menu" (Ctrl+F4 => "User configuration") a site change is undertaken, the user language will not be changed. The language of the original site - assigned in the employee master data - is retained.

#### 4.2.7. System

The logic must be activated with the switch `MODUL_INTERNE_MANDANTENTRENNUNG_SPRACHE`.

Only for customers who need this logic will the table `alsysinfo` be replaced with a view (see below for script).

Depending on a session-global variable, which refers to the current site, this shows the entry belonging to this site as alsysinfomd. With `setakthnr(HAUS)`, this variable can be converted for a session. With `getakthnr()`, the current site can be queried.

**Conversion of the "al tables" in views**

During the version update, the contents of particular tables from A+W are also delivered. After this action, previously the local language of the associated site was entered in the name fields in the course of the setup. For a multilingual environment within a database, this is no longer possible, since several languages are required here. For this reason, the following tables were converted to views:

- alatyp
- albestart
- alkaufart
- alsprpart
- alprsart
- alsprtypen
- alvkptyp
- albeschaffart
- aledvmodule
- xvorgang
- alenvgrp
- swaehrdru
- alzaart
- alvkzweig
- awbeaparam
- awbeatyp
- alkqual
- aldfuectrl
- aldfuetyp
- alkfldrefdef
- alvsgberechart

**CTRL server and background processes**

In order to send system mails in the correct language, for example, for the `MODUL_INTERNE_MANDANTENTRENNUNG_SPRACHE` module, the CTRL server is started in the appropriate language environment. This way these, as well as the background processes started this way, can access the messages of the appropriate language environment. Here, the subject lines and message texts of the system messages can be read in.

Switching the environment it done with the script `switch_site_env` within the call `ctrlservstart`.

Switching of the environment is done with remoshell. Here, the environment variables are set according to profile chain.

The SP `setakthnr` is called for background processes with the content of the variables `$HAUS`!

> **Note:** Messages that are sent by A+W Production (e.g. note about incorrect scheduling) are sent in the language of the production system.

**DFUE**
- Script `starterstart` was adjusted analogous to `ctrlservstart`. (switching the environment)
- EDI scripts must be checked.
    - In the scripts `$DFUEDIR/bin/trm_ctrl*`, `$ALCIBPRG` is assigned. Standard is a config file `"$AWROOT/config/mandant.cfg."`

**New DB connects**

For new DB connects in customimzing or in the reports, the language of the default site is always used. If another one is required, there must be a switch with `setakthnr()`.

#### 4.2.8. Output

Via the normal update logic, the following DB elements are output or changed:

- Table `alsysinfomd`
- Stored Procedures `getakthnr` and `setakthnr`
- `updlangspecviews` - conversion of all tables to views, which were converted earlier to the local language with updlangspec.
- View `artikelspr`: View of the articles, artbezfremd and alsysinfo joined. It delivers all fields of the table artikel in the local language of the current site.

**Adjustments that must be made if a multisite site requires multilingual logic**

- Since the conversion of the table alsysinfo can be problematic in a view at the customer's, all views based on it must be re-generated; therefore, this adjustment is only undertaken dedicated.
- For this, there are the following scripts under `$ALCIBPRG/install/xsql/cust/sy folgende`:
    - `alsysinfo.sql` - conversion of `alsysinfo` to a view on `alsysinfomd`
    - `updlangspecviews.sql` - script for new creation of all views with respect to the `updlangspec` logic
    - `xsprbezviews.sql` - script for new creation of all views with respect to the `xpsrbez` logic
- `$AWROOT/config/mandant.cfg`: the language environment must be entered here per site.

In the `vorgangs_sql` and also with other customizing, the site must be converted after the connect. Otherwise the main site is used as default.

#### 4.2.9. Research help

Check data not via select via shell or external database tools, but rather via `Adhoc_sql` in A+W Enterprise since the appropriate data for the site is assigned there. However, this assumes that you log into the correct site.

## 5. A+W Enterprise Master Data

### 5.1. Master data at the dealer's

For the internal document transfer, it is necessary that the production site be created as supplier in the market partner master data. Decisive for the internal document transfer is the "EDI type" field on the "Delivery" tab. This field has to be set to "SA Coupling" or "PU 1:n" or "PU 1:1".

Moreover, the production site has to be entered in table `xhaus` with the same supplier number. Special attention has to be paid to the correct setting of the fields `kunr`, `linr`, `host`, `hausart`, `vers`, `subvers`, and `patch` as well as `iboffset`, `bytevektor`, and `dfuedirpath` since these have a central effect on the internal document transfer.

In all clients participating in the internal document transfer, the table `xhaus` has to be adjusted accordingly.

| Field | Description |
| :--- | :--- |
| `haus` | Number of client (matches `$HAUS`) |
| `hnr` | Number of client (only in really old installations `haus` and `hnr` are different) |
| `hname` | Short name of the client |
| `kunr` | Customer number of client (corresponds to the customer number in the market partner master data). A client's customer number should be identical in all connected clients. If a company has 3 branch offices in Berlin, Dresden, and Munich, the Berlin branch office should be kept with the same customer number in the Dresden branch office as in Munich. It is possible to deviate from this recommendation, but the result is more configuration and management work. |
| `linr` | Supplier number of client (corresponds to the supplier number in the market partner master data). A client's supplier number should be identical in all connected clients. |
| `host` | Host name of the server on the network on which the client was installed and to which the transfer files should be sent. |
| `hausart` | For new installations always 10 or 11. The difference between 10 and 11 lies in the evaluation of the field `iboffset`. With `hausart=11`, the field is not evaluated. |
| `vers` | ALCIB version (e.g. ALCIB version 2.12.1 => vers = 2) |
| `subvers` | ALCIB subversion (e.g. ALCIB version 2.12.1 => subvers = 12) |
| `patch` | ALCIB - Patch (e.g. ALCIB version 2.12.1 => patch=1) |
| `dbart` | Identification of the master database for master data replication<br>2 - Master-Master database for 2-stage replication<br>1 - Master database<br>0 - Client database<br>-99 Sub client for self-transfer (environment variable IBHAUS) |
| `region` | The association of a client with a region (is evaluated, e.g. in the FinAc interface) |
| `shmoffset`| Shared memory offset of the client |
| `servmaster`| Name of the computer on which the server processes are running |
| `netz` | Network recognition |
| `sprkz` | Language ID (local language of the client) |
| `informixserver` | Name of the database server on the net. |
| `iboffset` | Offset for the generation of the order number for orders received via internal EDI |
| `bytevekt` | 1 - Database works byte vector (`BYTE_VEKTOR=ON`)<br>0 - Database works with bit vector |
| `dfuedirpath` | `$DFUEDIR` of the corresponding client. If the field is not filled, it is assumed that it is identical with `$DFUEDIR` of the sender. Important is the maintenance of this field if EDI should take place between Windows sites and UNIX sites or between 2 Windows sites on different installations. The path for the Windows sites must be entered in SFU notation. |
| `main site` | `=hnr` - main client<br>`!= hnr AND >0` internal client, the number is the number of the main client<br>`=0` - external client (#135188) |

### 5.2. Master data at production site

For the internal document transfer, it is necessary that the distributor be created as customer in the market partner master data. Decisive for the internal document transfer is the "EDI type" field on the "Delivery" tab. The field has to be set to "SA connection", "PU 1:n" or "PU 1:1". This has to correspond to the settings for the supplier at the distributor.

Moreover, the dealer has to be entered in table `xhaus` with the same customer number.

If the customer number of the distributor at the production site is not the same as the customer number that was entered in the `xhaus` entry for the production site at the distributor, the environment variable `IB_KUEMPF` has to be set at the production site.

### 5.3. Master data in stock

The client number throughout the stock module is evaluated if internal client separation is configured.

The system checks whether each of the articles to be booked has been defined as an inventory article for the client to which the inventory is allocated. If not, the booking will be rejected.

Client allocation is also checked when size- and color variants or the supplier is selected. Available for selection are only master data entries that match the current inventory in the client number or master data that have been defined without client allocation.

Irrespective of the configuration, the inventory selos now show the allocated client.

### 5.4. Companies (MP_SITE_EXACT #333097)

The key master data for companies is stored under Master data > Keys > System > Companies > Companies. In the Market partner field, an "Other" market partner can be selected, which must be assigned the value "1" in the `private_long1` field.

Under Master data > Keys > System > Companies > Company assignment, a company is assigned to all companies. On this dialog, it is not possible to enter new companies; it is only possible to make an assignment for existing companies. Please note that a site without company assignment counts as non-existent. Any change of the assignment will be logged in the DB table `site2compprot` with the following data: site, old site number, new site number, employee number, and date of the change. Since a change of the assignment can have massive consequences for the calculation, there is a security query for each change, asking whether you really want to do this.

For all companies, customer and supplier numbers are stored in the table `xhaus`. These count as **internal market partners**. Internal market partners must absolutely be maintained in the master data.

The company assignment of an internal market partner cannot be changed if the market partner is also assigned to other internal market partners as FINAC debtor. In this case, the dependency must first be resolved (that is, the FINAC debtor of the affected other internal market partners changed) before a new company assignment can take place. (see Also market partner master data - `MP_SITE_EXACT`)

**Process recording**

Via the site assignment, the company association is determined in each process and this company saved in the field `kauf.company`. If a company assignment is changed, then effective as of this time, the following rule applies for the existing processes:

- There is no automatic conversion of all existing processes.
- If an order is retrieved for correction, the company is adjusted in the configurable field. If this is an internal market partner, then the VAT is retrieved again and there is another calculation of the gross amount.
- If an order is entered with reference to an old older, then the company is determined again. If this is an internal market partner, then the VAT is retrieved again and there is another calculation of the gross amount.
- If an invoice is recorded for a process that was recorded before the change of company association, then the order itself will not be corrected. However, the invoice is generated for the new company and for internal market partners the VAT is retrieved again and the gross amount calculated. For the booking of the open orders/open items, it applies in this case: OA (gross values) are booked with the VAT valid before the change, the OPs (gross values) with the VAT valid after the change. Since the booking of the open orders takes place at the same time as the booking of the open items, there can be temporary differences in the data if the charging of an order is done via partial invoices. With the final invoice, the status of the open orders is balanced.
- Since due to the change of the company association it can happen that partial invoices are recorded and booked (gross values) for an internal market partner with different VAT rates, credits for internal market partners can only be recorded freely or with reference to invoices. The VAT in credits with reference is not determined anew; instead, it is always taken over from the invoice.

In the process (order) it is also possible to change the FINAC debtor. For internal processes, the same restrictions apply for the FINAC debtor as in the master data.

### 5.5. Key

For the expanded internal client separation, additional key data must be created.

#### 5.5.1. Due date conditions

Under the menu element Master Data > Keys > Cash Discount Groups, you store a payment condition with the type Due date. All date-related data will be maintained precisely as for cash discount conditions, only the cash discount record has no meaning in this case.

The number of due date dates can be determined by following records.

Depending on the number of following records, the amounts can also be divided. The due dates are thus not independent records, but rather chained to one another. The calculation of each additional due date in the chain is done relative to the due date record before.

This must absolutely be heeded when creating the dates or invoicing dates of the due dates.

**Example 1:**
An invoice for 1234,- € was booked on 05/25/2007.
- Due date 300: 1 month from invoice creation. Following condition 200.
- Due date 200: 1 month from 1st due date (2 months from invoice creation). Following condition 100.
- Due date 100: 1 month from 2nd due date (3 months from invoice creation). No following condition.

For each due date record, a 1 should be entered in the months field (in addition to the invoice date) and a corresponding following due date defined.

Due date 300 corresponds to a 3-way due date chain with division of the invoice amount in three equal parts:
- 411.33- € due on 06/25/2007
- 411.33- € due on 07/25/2007
- 411.33- € due on 08/25/2007

**Example 2:**
An invoice for 1234,- € was booked on 05/25/2007.
- Due date 401: period 15 days
    - Creation date 1: 15
    - Creation date 2: 30
    - Following record : 301
- Due date 301: period 15 days
    - Creation date 1: 15
    - Creation date 2: 30
    - Following record : 201
- Due date 201: period 15 days
    - Creation date 1: 15
    - Creation date 2: 30
    - Following record: 101
- Due date 101: period 15 days
    - Creation date 1: 15
    - Creation date 2: 30
    - Following record: none

- Due date 401 corresponds to a 4-way due date chain with division of the invoice amount in 4 equal parts:
- Due date 301 corresponds to a 3-way due date chain,
- Due date 201 corresponds to a 2-way due date chain.

Each of these due dates can be stored for the market partner if necessary.

If for the invoice due date 401 is entered, the invoice amount will be distributed as follows:
- 308.50- € due on 06/15/2007
- 308.50- € due on 06/30/2007
- 308.50- € due on 07/15/2007
- 308.50- € due on 07/31/2007

For due dates, a date rounding can be activated in the master data. Here, however, the rounding is only considered for the first element of the due date chain.

> **Note:** The handling of cash terms with activated date rounding and the consideration of vacation days for due dates are described in separate texts.

**Booking invoices**

When booking an invoice for which the cash term was replaced by a due date condition, data is generated according to the number of due dates in a separate table `zahlplan`. This data is available when printing the invoice. However, it can also be viewed in a generated invoice via Menu > Payment plan. The data cannot be changed there.

Also when booking a collective invoice, the data is generated in the table `zahlplan`. And this for each part of the collective invoice with specification of the reference. In addition, a total record for the entire collective invoice is generated, in which the reference fields are not assigned.

A due date condition replaces a cash discount term and is applied to the entire invoice amount.

### 5.6. Product groups (#334944)

It is now possible to maintain the procurement types for products (incl. the procurement parameters) right in the goods groups / subproduct groups / product groups level.

**Master data**

In the goods group master data, you can now maintain globally and also site-specifically the procurement types for all products that belong to the appropriate goods group. The global procurement type data (standard supplier, production time, stock) can be stored using the "Procurement type" tab for goods group. All entries are possible both on the goods group as well as on the subproduct group level (here the first 4 places are defined) as well as on the product group level (here only the first 2 places are defined). If for individual companies/sites deviating data should be necessary, then it must be maintained via "Details (company) or <F5>". These company-specific details are also on the Master data->Keys->Products->Company-specific details->Product groups. The prerequisite is the existence of the STWM right for the employee or master data administrator rights.

The entry of the procurement type in the master data itself is now no longer absolutely necessary. When exiting the dialog, there is only a check as to whether the procurement type could be found via this itself, the subproduct or product group. If this is not the case, an appropriate message is output.

**Evaluation in the process**

When entering orders, a procurement type is always determined for each product from master data. This is a component of the shared memory article. The determination is done in several stages in the sequence:

1.  Procurement type of the color or dimensional variant with respect to the current site (DB tables `artfarbmdzu`/`artvarmdzu`)
2.  Procurement type of the product itself with reference to the current site (DB table `artmdzu`)
3.  Procurement type of the goods group (all 6 places) with respect to the current company (DB table `wagrpmdzu`)
4.  Procurement type of the subproduct group (the first 4 places) with respect to the current site (DB table `wagrpmdzu`)
5.  Procurement-type of the product group (the first 2 places) with respect to the current site (DB table `wagrpmdzu`)
6.  Procurement type of the global color or dimensional variant (DB tables `artfarbzu` / `artvarzu`)
7.  Procurement type of the product itself global (DB table `artikel`)
8.  Procurement type of the product group (all 6 places) global (DB table `wargrp`)
9.  Procurement type of the subproduct group (the first 4 places) global (DB table `wargrp`)
10. Procurement type of the product group (the first 2 places) global (DB table `wargrp`)

As soon as a procurement type has been found, the search ends.

**Evaluation in other modules**

In Stock, the determination of the procurement types is done in accordance with the logic described above.

ENV switch `WARENGRUPPEN_BA = ON` must be active.

### 5.7. Market partner master data

For the new sites, the appropriate customers and suppliers must be created according to `xhaus`.

#### 5.7.1. Routes

If within the internal site separation you are not working with uniform route master data, then you have to work with `MODUL_REGIONALROUTEN`. See “DE-CONFIG-A+W Enterprise.pdf" section "Shipping regions/routes."

> **CAUTION:**
> If the switch `MODUL_REGIONALROUTEN` is set to ON, the fields for alternative routes, routes 2-4, cannot be accessed. If before an activation of the environment variable there are already alternative routes in the market partner master data, it absolutely has to be deleted **manually** with activation. Thanks to the activation of the environment variable, the alternative routes for the market partner are not removed automatically from the system.

#### 5.7.2. Limit check

Within the internal client separation a client-specific limit check is possible. The environment variable `LIMITS_MANDANTENTRENNUNG = ON` activates the logic.

If client-specific limit check is activated, the entry of the limit values is no longer done directly in the fields for the market partner master data. Directly after the field "Limit check via" on the appropriate "Limits" tab, a separate dialog opens on which you can enter the limit data site-specifically. This deletes the "general" data on the MP dialog.

#### 5.7.3. Client-specific data (MODUL_INTERNE_MANDANTENTRENNUNG)

**Master data**

For each market partner of the type "Customer," "Supplier" or "Object," you can maintain different data per client via Menu > p.Company-related details.
- Representative (sales revenue)
- Conditions debtor
- VAT code

**Addresses**

QR22/11

If an address is entered, with internal client separation, you should always enter the distance and driving time per client. Therefore, on the address dialog, when you enter the Distance field, you are taken to a separate dialog for the entry per client. The data is entered client-specifically on this dialog.

If you enter a new address, the entry of the distance without client reference is not possible. If you change an existing address with entered distance, then a record on the new dialog for the current site is generated right away.

The entry of this data is only possible in correction mode (master data) or new entry mode (master data or document entry). For the display of the existing addresses in sales, this data is obtained client-specifically if it has been maintained client-specifically.

If the system is configured so that the driving time should be obtained from the route, the entry of the driving time in the addresses is not possible.

**Process recording**

If in the document a client assignment is changed, then the distance and the driving time from the delivery address are obtained taking into consideration the new client assignment (if data about this is present). If km-specific discounts are present in the document, these are recalculated.

In case of a change of the client within the transaction entry, the route and the VAT key for the customer are pulled client-specifically. If the client change occurs when all items have already been entered in the transaction, the supply types for the products are pulled again. The transaction is recalculated completely if the VAT has changed.

**Company change in the order after transfer to A+W Production**

If in an already-released order a client change is desired, then you can enter a new client number via the menu or with `<F5>` from the Input field in the transaction header. If the transaction is already locked (local correction), a client change is no longer possible. After the new client number has been taken over into the order header, the user can decide whether the new procurement type according to the stored master data should be pulled into the new client. A new route is searched for and the order is re-calculated.

Client change is always considered production-relevant! If the transaction was already released in Company 1, the release in the company is assumed as a "must." When saving, first a query is sent to A+W Production whether a cancellation in Company 1 would still be possible. If the cancellation query is accepted, then all other data in Company 1 is cancelled (dispatch, stock, purchase orders) and the order is released in Company 2. If the cancellation is rejected, then the order cannot be saved in this form. The user must contact an employee in the production area and then eliminate the possible blockage reasons. Then, the client change must be carried out again. If this is not possible, the client change must be discarded. We recommend executing the client change quickly and not in connection with other changes. Since the lock from production can come at the time of the change and then the changes must be discarded completely.

A client change in connection with cancellation to A+W Production is also logged in the order status (`kaufstat`). If the purchase orders are thus also canceled, you can see this information in the change log.

**Export Service**

In the config tool of the export service, several databases can now be configured. With internal client separation, the DB configuration can be done subclient-precisely if needed. Polling interval and the maximum number of transmission attempts are specified across DBs.

In the service, after expiration of the polling interval for all configured and active databases, it is checked whether trigger records are present in the table `EXPORTINFO`. Existing records are worked through. The databases are checked one after another, the sequence of the checking is arbitrary.

With subsite-precise configuration of a DB connection, only the `exportinfo` records are processed that contain the configured subsite in `EXPORTINFO.HAUSNR`.

**Export Service: New interface "CANCELORDER"**

Order cancellations are transferred to A+W Production using this interface.
The interface records in table `EXPORTINFO` are generated by the back end.Records with the new interface are preferably processed by the export service. Attention! For this, the polling interval in the config tool must be configured so that it is appropriately short.

The export services calls a PPS Webservice method, which executes the order cancellation in A+W Production. The return value of the method indicates whether or not the order cancellation was executed successfully in A+W Production:

- Return value > 0 indicates that the cancellation was executed successfully.
- The value -1 indicates that the action could not currently be executed due to content problems (e.g. OrderXML is being imported now).
- The value -2 indicates that the order was neither found in the database nor as OrderXML.
- The value -3 indicates that there are technical problems (e.g. DB connection problem, program error).

Successfully processed records are transferred to the table `EXPORTINFOOK`, in the process the long value from `EXPORTINFO.IZEIT` (insert-time) is transferred after `EXPORTINFOOK.LONGWERT1`, so that records for the same order can be distinguished using the time stamp.

Records that encounter an error stop with `STATUS < 0` in `EXPORTINFO`. In `EXPORTINFO.FEHLERTEXT` the error that occurred is described and the error code specified.

In the PPS Webservice, the new method for order cancellation is available starting with Version 13.04.1330.

**OrderXML Service**

In the config tool of the OrderXML Service, you can maintain a site number. Effective immediately, it is also evaluated by the OrderXML service, so that only such transactions from the `OTTRANSFER` table are read that fit the configured client number. If in the configuration the site number was assigned the value 0, as previously, all data records will be processed.

The entries in the table `OTTRANSSAV` will serve only research purposes in the future. The previous logic of sending a special OrderXML to the previous sites in case of a site change was deactivated since it was causing problems.

#### 5.7.4. Client assignment MP_SITE_EXACT (#334703)

With the introduction of the multi-client logic, the market partners (customers, suppliers, objects) are now also maintained client-specifically. Each market partner can be assigned to a single client, but also to several. For the use of all market partners, however, an assignment to at least one client is necessary. **IMPORTANT!** Without assignment, the existing market partners cannot be used.

**Master data**

For each market partner of the type "Customer," "Supplier" or "Object," you can maintain an assignment to the existing clients via Menu > p.Company-related details. Since this assignment is necessary for the further use of market partners, when exiting the market partner dialog, it is checked whether the assignment has already been made. If there is no assignment and the employee also has the rights for the market partner - site assignment (MPMA) or if he is a master data administrator, then the user is led automatically to the assignment dialog. If the employee has no rights to maintain the assignment, then he is only informed of the missing assignment.

On the same assignment dialog, it is possible to assign each market partner a deviating revenue representative and a deviating condition debtor site-specifically. However, these details are not absolutely mandatory. If no site-specific data was stored, then the data from the market partner itself is used. The prerequisite for the takeover of the "global" representative is the appropriate site assignment for this in the employee master data (representative = employee with representative option) for appropriate companies.

The assignment is also possible via Master data->d Keys->a Market partners-> n Company-related details.

You can maintain 2 VAT keys directly in the master data. The internal VAT is pulled if the customer is an independent company within a company.

**Process recording**

During the entry of each process, in advance via the employee assignment or the global manual setting in the current session (System menu > Company change), the site is defined for each new process. For users for whom the right "VOKU" has been revoked, the customer selection (manual or via the search dialog) is then only limited to the customers who have an assignment for the current site of the process. This restriction applies generally regardless of this right, also for objects and suppliers on all sales dialogs and for suppliers and objects in the purchasing processes. Only for automatic processes generated by the EDI is the existing data not checked and generally assumed to be "applicable."

A site change is only possible as long as the transaction has not yet been saved. For transactions that have already been saved, no more site change is possible. This is because with extended internal site separation, it is possible to work with site-specific number ranges.

If during the company entry there is a site change after entry of the market partner, there is a check whether this is permissible for the new site and if not, a site change is declined. If this is an order with an object assignment, then there is also a check of whether the existing object is permissible for the new site. If not, the site change is also declined. The procedure is different if the order items in the process or ordered parts from the BOM have a supplier who is not known in the new site. Here the site change is not declined; however when saving the order, all suppliers are checked and the order cannot be saved until all suppliers not permissible for the new site have been changed. The checking of the suppliers is done for all items first on the item level and after that also for all levels of the BOM, so that the product itself if not ordered or removed from the warehouse. In case of a failed check, a message appears indicating which item or which BOM and item had incorrect suppliers.

During the entry, the fields "Representative(revenue)" in the header dialog ("Properties" tab) and Condition debtor (visible on the "Order conditions" dialog) are obtained site-specifically. If the logic of the takeover of the object data (`ALL_OBJ_INFO`) is active, then the data is always re-determined after the object assignment; it applies for this order. Here, however, the rule is that if the data was taken over from object and for the site, no site-specific condition debtor or revenue. Representatives entered, then the global data from the object applies. If the global data from the object is unsuitable for the current site, then the object itself applies as condition debtor and the rev. representative is deleted.

If the `OBJ_ALL_INFO` logic is not active, then the data from the object plays no role and the condition debtor and the revenue-proportionate representatives are obtained from the customer data. In the purchasing processes, no data is taken over from objects.

If `MPPROJEKT` is active, then here too the rule applies that in a site only the data can be viewed and entered that is also assigned to this site.

**Market partner search**

The dynamic market partner search now supports a site-specific search for customers, suppliers and objects. If you start the search from the areas where the site assignment is already defined (e.g. in the procedure entry), then the search field "company number" is pre-populated and cannot be changed. From the areas where market partners are sought across boundaries (e.g. in the master data), you can enter the search criterion "site" in order to have displayed only the market partners who have the appropriate site assignment or leave the field empty in order to see all market partners of the selected type. In the overview column "Site," either the site number is visible or with a cross-site search a specification of the form (X), whereby X corresponds to the number of assigned sites. If you position yourself on this field and press the `<F5>` button, then you will see a list with the assigned companies.

> **IMPORTANT!** The search is always associated with the rights of the employee for the current module and the current area. If the employee, e.g. only has rights for the market partner master data in site 1 and 6, then he will only see market partners from the site 1 and 6 even in the cross-site search. Only the master data administrator is responsible for new site assignments.

#### 5.7.5. Company assignment MP_SITE_EXACT (#333097)

For all companies, customer and supplier numbers are stored in the table `xhaus`. These count as **internal market partners**. Internal market partners must absolutely be maintained in the master data. If you enter these market partners on the Master data > Market partner menu, then the title changes to "internal market partner." For internal market partners, it is also possible to store a deviating FINAC debtor. However, stricter restrictions apply here: permissible are only internal market partners that belong to the same company/corporate group. If for an internal market partner a deviating FINAC debtor has been entered, then starting from this point, there is also increased checking of the change of the company assignment.

The company assignment of an internal market partner cannot be changed if the market partner is also assigned to other internal market partners as FINAC debtor. In this case, the dependency must first be resolved (that is, the FINAC debtor of the affected other internal market partners changed) before a new company assignment can take place.

In the process (order) it is also possible to change the FINAC debtor. For internal processes, the same restrictions apply for the FINAC debtor as in the master data.

**Example:** MP 2 should be assigned company B. In this case, first the FINAC debtor of MP 1 must be set to 1.

| MP | Finac debtor | Company |
| :-- | :-- | :-- |
| 1 | 2 | A |
| 2 | 2 | A |
| 3 | 3 | B |

The same applies if an internal market partner with deviating FINAC debtor should be assigned a new company (in the example: MP 1 should be assigned company B). In this case, the assignment to the FINAC debtor must also be resolved before the assignment can be made (that is, the FINAC debtor set from MP 1 to 1).

We would like to point out that the invoices are always recorded and booked to the FINAC debtor. If for internal market partners a deviating FINAC debtor is entered, then there can be no detailed site-specific internal charging.

For the internal market partners (customers and suppliers), on the "Limits" tab there is now the possibility to specify two different VAT keys (records). The first one is used if you record a process for an internal customer who belongs to another company than the main company for which the process is recorded. The second internal VAT applies for processes of internal customers that belong to the same company.

### 5.8. Item master data

The following article master data can be stored client-specifically:
- Menu > Client-related details > Variants
- Menu > Client-related Details > Variants
- Menu > Client-related Details > Colors/Sizes
- Procurement type
- Supplier
- Delivery time
- Production duration
- Standard stock
- Size restrictions (only on article level)
- Installation restrictions

#### 5.8.1. MP_SITE_EXACT (#331647)

The following item master data, which affects the cost calculation and prices, can now be stored site-specifically:

- cost calculation (yes/no)
- Loss of material
- Correction factor (calculational loss)
- Standard price (FinAc-spec. entry)
- Price type (FinAc)

**Maintenance of the master data:**

This data is, as earlier, maintained directly in the item master data. Should the data in one of the companies deviate, then you can create it on the Menu -> Site-related details -> Item on the "Details" tab. When creating site-specific data, first the details from the item itself are taken over. **Note:** subsequent changes of the data on the item level do not automatically change the site-specific data. It is only reported that the data must be checked. On the dialog for site-related item details, it is possible to take over the changed calculation data from the item for all or for individual sites.

**Evaluation**

The item data determination in AWE modules is done on two levels: first site-specifically and with missing site-specific data then from the global item level.

Thus for the cost calculation, the material loss is determined first for the current site (database table `artmdzu`). If there is no data here, the data is then obtained from the item master data (database table `artikel`). The same applies for the stock forecast - first the correction data is sought site-specifically and taken over, but if no data is found there, then the correction data is taken over from the item master data.

### 5.9. Employees / user rights

#### 5.9.1. MP_SITE_EXACT (#332946)

In internal site systems where employees of companies with different legal status work simultaneously, it is important to be able to limit both the module rights as well as the data access on the site level. Thus you can prevent any employee from accessing the data for all clients as soon as he has been created in the system.

**User rights**

A site assignment must be specified for all employees. If he may only operate the program in one site, then it is sufficient to make an assignment in the "client" field. If an employee works in several sites, then there must be a site assignment made using the "Site assignment" button or `<ShF5>`. Since only the companies are offered for selection for which the person entering the order has rights, this assignment should be made by one of the master data administrators (MASTER_DATA_ADMIN). (right STMM) (for a list of the affected dialogs, see also "EN-CONFIG-A+W Enterprise EDV Moduleabbreviation")

After the employee is assigned to the different sites, site-specific rights can also be assigned or revoked. To do this, you enter the rights on the lower part of the dialog with entry of the site number. If the site number remains blank, then this right rule applies for all companies to which the employee is assigned.

For rights groups, it is NOT possible to assign a site since these are always defined generally. If for an employee a rights group is selected, then you can limit this only to particular sites. If no site is specified for the rights group assignment, then the rights of the group apply in all sites to which the employee is assigned.

If a user assignment to a site is deleted, first there is a check whether for this user there are explicitly some module rights for the site via direct assignment or via group rights. If such are found, this is reported to the person entering the data and the deletion is declined.

**Global/local rights**

The division into global and local settings is referred to in the description of the EDP module codes. It is described in the documents DE-CONFIG-A+W Enterprise EDV Modulkuerzel.docx and EN-CONFIG-A+W Enterprise EDP Module Codes.docx

Note that not every right is maintained site-specifically and can be evaluated.

**Copying module rights and rights groups**

A copy function was added to the sub-dialogs for Rights and Rights groups with which it is possible to transfer existing rights to additional clients.

The function is only available for such records that already have a client assignment. This client applies as source client for the copy action. Trigger the copy function with the key combination `<CTRL>+<F9>`. A dialog appears on which the target client can be selected. Only such clients are available for selection that were assigned to the employee. If the dialog is triggered with `<F3>` or the `<Start>` button, all data records of the source client are copied to the target client.

If there were already records for the target client, these are deleted before the copy action in order to prevent doubled records and ensure that source rights and target rights are identical after the copy action. With an appropriate query before deletion, the user can prevent the deletion of the rights by canceling and copy action.

In order to copy the configured rights of a source client to all possible target clients for an employee, you can simply leave the field for the target clients blank on the selection dialog.

Additional prerequisites for the copy mechanism are: the employee must have more than one client assignment and the employee type must be 'Employee.'

**Evaluation of the rights in the modules**

The site that was entered directly in the employee master data applies as main site for the employee and is pre-populated as current site. However, after the start of the program, you can change the site assignment for this session. This is possible using `<CTRL>+<F4>` > a user configuration > a site change. Naturally this change is only possible if the employee has more than one site assignment. With the start of all menu items (if these are protected with an individual right), user rights are then checked site-specifically. In the process entry, first there is only a general check whether the user has a right to enter orders in at least one site. With a call of an existing process, the site number assignment is then made concrete and then the appropriate rights are checked. For the new entry, the right is checked according to the site number on the process entry dialog. With the `<START>` button, you can change the site assignment directly in the process during the new entry. Here only the sites are available for selection to which the employee is assigned. After the selection of a site, the appropriate entry rights are checked again for this site.

**Evaluation hierarchy for user rights**

It is currently possible to store user rights on different levels. Thus even today, you can combine rights into rights groups, in addition there are rights to module groups and directly on the module level. The site level has now been added to these levels. The evaluation of the different hierarchy levels is done as follows here:

| Priority | Site allocation | Module/Module Group | User/Group |
| :--- | :--- | :--- | :--- |
| 1 | H | M | B |
| 2 | H | M | G |
| 3 | H | MG | B |
| 4 | H | MG | G |
| 5 | * | M | B |
| 6 | * | M | G |
| 7 | * | MG | B |
| 8 | * | MG | G |

- **H** = Rights with site allocation
- **\*** = Rights independent of the site
- **B** = User rights
- **G** = Group rights
- **M** = Module rights (e.g. VOKA)
- **MG** = Module group rights (e.g. VO*)

Here it is so that rights that are assigned to a site generally have a higher priority than rights that were assigned regardless of the site. Module-specific rights have a higher priority on the next hierarchy level than rights from module groups. In addition, rights that are assigned directly to the user have a higher priority than rights that were assigned via user groups.

The rights are saved in the temporary table `nlogin` and evaluated via the `SP syget_zugang_site`.

**Restriction of data access**

Since the various sites may be legally independent companies, it is important to ensure that employees who are only assigned to one or more clients can only view the data of the assigned sites as early as the selection dialogs (transaction search, product and market partner search and other SELOs). This restricted data view is relevant to all client-specific master and transaction data. For example, an employee who is assigned only to site 11 can only view orders that are allocated to site 11 in the order search window. All other orders remain hidden.

Such restricted data views are only possible at those points in the program at which the associated data has been assigned to a site. As a result, no site allocations will exist for the Salutation keys, since they are maintained globally across all sites. Therefore it is not possible to implement a restricted data view or site-specific rights check at this location.

**Restriction of SQL queries (adhoc-sql)**

Since data access for SQL queries is controlled via the saved SQL, it is unfortunately not possible to make general program adjustments that would automatically allow for restricted views in accordance with the user's rights. To nevertheless achieve such restricted access, a temporary `nxhaus` table is created when the program starts. It contains all of the fields of the `xhaus` table; but it is reduced to the sites to which the employee registered with A+W Enterprise has been assigned. Hence all tables with a site allocation would be joined with this table, so that only the data from the table for which the employee has access rights (via the site allocation) is displayed. All SQL queries of Group 1 (SQL queries delivered by A+W) were already converted. They will be supplied with the version update.

The tables `nxhaus` and `nlogin` can be checked via a SQL query (ahoc-SQL) in the program.

### 5.10. Client-related company calendar

For each internal client, individual data can be stored on the operating calendar. That is, client-specific distribution, production, and holidays can be stored.

The client calendar is accessible via System menu > Info services > Calendar > Client calendar.

## 6. Texts
(#437335)
A house number can now be stored for master texts, current texts, group texts and product group texts in Master data > Text management in order to store house texts in a multi-client system.

Whether a text is used is controlled by the house number in the respective document.

The current texts and the group texts are evaluated in the programs that generate the texts, `repmix` and `reptzui`. To adjust the evaluation of merchandise category texts, the reports must be adjusted accordingly.

The product group texts are loaded and evaluated in both the REPGO and CRYSTAL environments within the report. The evaluation of the house number must be solved individually for the customer on request, this was not part of this development. To control the evaluation of the house number in the reports, you can use the new environment variable `REP_WARGRPTXT_MULTISITE` (ON/OFF).

## 7. Prices (MP_SITE_EXACT # 333913)

Starting with Version A+W Enterprise 6.0, it is possible to control the price calculation via global and local price lists. This new feature is only possible for operation with the extended internal client separation since only in this configuration is there a separation between global (company-spanning) and local (company-specific).

### 7.1. Requirements and configuration

#### 7.1.1. System / environment

In order to be able to define global price lists, a pseudo price master company must be defined. It is stored in the table `xhaus` with `xhaus.dbart=-99`. With the dbart flag, the price master company for manual use is excluded within the transaction entry, the EDI, and for various evaluations. Furthermore, the company must be kept in the appropriate ENV switch. Via whose activation the new logic is also enabled. With the current program version, several price master data tables were also expanded. With a script provided by A+W, you can assign the existing keys in the price sector to the price master company. In `<$ALCIBPRG>/cmd` a script `preisstamm <Target site number> <Current site number>` is stored that converts the existing data. Here, target - company number should be the company number from environment variable `PRICE_MASTER_HOUSE`.

#### 7.1.2. Employee master data

The price master company must be assigned to the employees who are responsible for the maintenance of the prices and condition master data in the master data, as well as the appropriate rights from the prices/conditions area.

#### 7.1.3. Market partner master data

In the market partner master data (Master data > Market partner) under the References tab, it can be specified for a market partner whether it is a company-specific debtor. For this, the 2 data fields `Debitor` and `Debitor-Hausnr` have been added. With the Debitor data field, you mark the market partner as debtor. If the market partner should be set as debtor, the data field `Debitor-Hausnr.` becomes active and you can enter the associated company. On the data field `Debitor-Hausnr.` you can use F9 to call up a search dialog for the existing companies.

For the assignment of the conditions for this customer, for all areas (IG, TG, base glass, etc.) the local price lists of the company from the `Debitor-Hausnr` field and also the general price lists are available.

For all other customers, it is possible to use Market partner->F4->Company-specific details to store a new record in the table `mpmdzu` with the condition debtor for the local price lists and corresponding company.

**Example:**

Customer 500 is marked as debtor for the company 5130 via the `Debitor-Hausnr.` Field marked (debtor: 1/debtor for the company: 5130). In addition, it can be assigned to additional companies (e.g. 6130) via the company-specific details.

The price lists from the company 5130 are now assigned to the customer 500 via the debtor company number.

If customer 4711 is assigned to the companies 5130 and 6130 via the company-specific details. If in both assignments the condition debtor `mpmdzu.konddebnr=500` is entered on the dialog, then the price lists of the company 5130 apply for the customer 4711 at both companies.

For suppliers, the master data maintenance is done the same way:

A pseudo supplier can be defined via the new data fields `Debitor` and `Debitor-Hausnr.` as condition debtor for a local company. The local purchasing price lists can then be assigned for this supplier. Via company-specific entries (table `mpmdzu`) this condition debtor can be stored for a particular company.

The deviating delivery time can thus also be maintained per client.

With maintenance of the conditions, only the global price lists are available to all customers/suppliers. For the market partners who are specified as local condition debtors for the individual companies via the new data fields, the global price lists and the local price lists are available for selection.

#### 7.1.4. Price master data

The maintenance of the price key and price assignments is now only possible after entry of the company.

**Price lists:** As default value on the price key dialogs, the price master company is always suggested first. Using a selo or with manual company number entry, it is possible to store the local price lists (PLKZ/PKZ) for the appropriate company.

**Price list control:** The global price lists for the price master company continue to support all types of price control, such as:
- only PLKZ
- PLKZ + base
- starting with PLKZ
- starting with PLKZ + base.

For the local price lists, there are only 2 possibilities:
- only PLKZ, or
- PLKZ + base.

A local price list or a global price list can be specified as base price list. For the pricing via price lists with the "starting with PLKZ" or "starting with PLKZ+base" logic, the valid data is always determined using the price lists for the current company. Thus the local price lists do not absolutely have to be in a completely different number range. A prerequisite here is that the base price list number is smaller than the numbers of the local price lists.

#### 7.1.5. Terms

**Assignment of the local price lists:** The assignment of the local price lists is done via the assignment of the general conditions to a company-specific debtor.

Within the special conditions, you can assign the local price lists of the site to which the condition debtor is assigned. Starting with Build 13.04.3884 (January 30, 2020), it is also possible to assign a global price list to a local condition debtor in the special conditions. This is possible in
- Special general conditions
- Special product group conditions
- Special article conditions
- Special shape surcharges
- Special AIR surcharges
- Special exchange list factors

Within the special prices, you can also assign special prices for the global price lists.

The prerequisite for assigning the global price lists in the conditions is that the employee is assigned to the price master site and has the appropriate employee rights.

**Purchase price list control for cost calculation for multi-client configuration**

Currently, you can only enter one material cost list in the general daily conditions. It is not client-specific. The average stock values can already be evaluated client-specifically if you define client-specific standard stocks in the item master data.

Now it is also possible to create local material cost lists.

In order to define client-specific material cost lists, the program has been adjusted so that in the market partner-specific general conditions for the supplier/condition debtor "own site" (`xhaus.linr`), a material cost list can also be stored. Here it is checked whether the price list is allowed for this client (price list master data). If the price list assignment or the site assignment of the price list is changed after the fact, there is no further check whether the price list is valid for the client.

The evaluation is done so that first there is a search for the client-specific cost list. If a cost list is entered, it is used. At the same time, the piece price rounding from this condition record is used. Then there is no check whether general day conditions exist.

If no client-specific cost price list was defined, it is checked whether a general cost price list was defined in the general day conditions. If this is the case, this cost list and the piece price rounding from this condition record are used. It is not checked whether in the site-specific conditions a deviating piece price rounding is stored.

#### 7.1.6. Evaluation in document entry

For the entry of SA transactions, the company-specific condition debtor is determined and the prices pulled from the appropriate price lists. For the determination of the PU prices of ordered items, the condition debtor of the supplier (if present) is used as the basis for finding the price lists.

Which price lists are available for the change in the order is determined by the customer's condition debtor. If this is a condition debtor with local price lists, then global and local price lists are available for the change in the order. You can select the global price lists using a selo with `<F9>`. You select the local price lists of the company in which the order is entered (`kauf.hausnr`) using `<F8>`.

If the local price lists of the company are not stored generally using a standard condition debtor with local price lists for the customers in the master data, you can nevertheless assign the local price lists in the order. However, the user must have the right for this (VOLP). Here it must be noted that the rights can only be revoked. If users may not make the decision about the assignment of local prices, the right must be revoked (Recht != 'w').

If the separation depicted here according to general and local price lists is not active, then nothing about the old price calculation changes despite the expansion of the price key table. The company number is pre-populated with 0. It is neither required as entry nor is it evaluated anywhere in the system.

The evaluation of the old right VOAU (edit order conditions) was expanded. The old evaluation "no W-right - no access right" was expanded to R-right. If the user has only a read right, then he may enter all condition dialogs in display mode. For site-specific separation, the right can be set purposefully for different companies.

## 8. Sales

### 8.1. Limit check

Within the internal client separation a client-specific limit check can be configured (#388239).
The environment variable `LIMITS_MANDANTENTRENNUNG = ON` activates the logic.
`LIMITS_ANZEIGE = ON` activates the new display on the dialog edge
The environment variable `LIMIT_FREI` must **not be set**.

See Master data - Market partner

### 8.2. Transaction data

The values for open orders and receivables from the orders/invoices are now booked company by company in the "limits" table.

If there is a company change, the limit data is obtained anew and the order value is checked against the new limits values. The user's rights are still checked. If an order was entered in a company and release and then the company assignment changed, this order can no longer be blocked in the release pool. This change is rejected if the user does not have sufficient rights for changes that extend beyond the customer limit.

The market partner information from the transaction is always obtained in this case for the current company.

### 8.3. Client-specific release pool

The release pool is client-related, therefore the data is only obtained after entry of the desired clients. The field site number is pre-populated with the current site number, but it can be changed. If the site number is deleted from the input screen, then an overview of all non-released orders in all sites is granted. From the release pool of all production clients, you can also release the orders directly by marking them and pressing `<F3>`.

### 8.4. Order corrections after successful client allocation

If the order is obtained after successful client allocation, the site determined will be retained. Also in the case if the following corrections would have had an effect on the new allocation in case of initial entry. Automatic reallocation is impossible because - under certain circumstances - the system will not be able to cancel already created purchase orders and orders.

### 8.5. Change of client allocation

If - in case of internal client separation - the allocation of the production client cannot be done in the background, the order remains in the release pool of the call center, with a note: "No client allocation."

The user can only forward orders from the call center's release pool to the system with a manual change of the order. This can be a change of the criteria that enable another allocation or also a manual allocation of the production client. To make such a change, the user must have particular employee rights.

Also directly during the entry, an employee with appropriate authorization can allocate the order to a particular production site. In this case, the order will not be transferred to the automatic site assignment of the call center. There will be no restriction check of the order. The user is responsible for ensuring that the order data fits the manually selected site.

Site allocation should be changed manually only in exceptional cases, which is why the field Site number cannot be accessed directly but only via `<F5>` from the Receipt field.

With the change of the site allocation, the route is adjusted immediately, even if a shipping site was entered in the order. If the new site is identical with the former shipping site, the system will realize this; the internal route will be replaced by a direct customer route and shipping site and end route to the customer will be deleted. The delivery date will be recalculated after the fact.

The site allocation cannot be changed if the order has been locked because of a PO, receipt of goods, or production at the former site. If the order has been locked at the former site only by dispatch planning, the user will be informed and asked if this change shall still be made. An after-the-fact allocation to call center if the order was already allocated to a production client is not possible because it can mean that with the change, no new allocation can be found and so no further processing of the transaction takes place, thus also no cancellation in the production or for data from the order from the initial entry.

> **IMPORTANT!** In case of after-the-fact changes of the site in an order, which was already booked in dispatch in the old site, there is an immediate adjustment of the data in dispatch. Such a change can no longer be discarded.

A change of site (new input as well as order correction) is recorded in a special table `hausprot`.

### 8.6. Company change in the order after transfer to AWP

If in an already-released order a company change is desired, then you can enter a new company number via the menu or with `<F5>` from the "Input" field in the transaction header. If the transaction is already locked (local correction), a company change is no longer possible. After the new company number has been taken over into the order header, the user can decide whether the new supply types according to the stored master data should be pulled into the new company. A new route is searched for and the order is re-calculated.

The company change always counts as production-relevant and if the transaction was already released in Company 1, the release in the company is assumed as a "must." When saving, first a query is sent to A+W Production whether a cancellation in Company 1 would still be possible. If the cancellation query is accepted, then all other data in Company 1 is cancelled (dispatch, stock, purchase orders) and the order is released in Company 2. If the cancellation is rejected, then the order cannot be saved in the form. The user can contact employees in the production area and then eliminate the possible blockage reasons on this side and make the change again. If this is not possible, he must discard the change. We recommend executing the company change quickly and not in connection with other changes since the lock from production can come at the time of the change and then the changes must be discarded completely.

A company change in connection with cancellation to A+W Production is also logged in the order status (`kaufstat`). If the purchase orders are thus also canceled. you can see this information in the change log.

**Export Service**

In the config tool of the export service, several databases can now be configured. With internal site separation, the DB configuration can be done subsite-precisely if needed. Polling interval and the maximum number of transmission attempts are specified across DBs.

In the service, after expiration of the polling interval for all configured and active databases, it is checked whether trigger records are present in the `exportinfo` table. Existing records are worked through. The databases are checked one after another, the sequence of the checking is arbitrary.

With subsite-precise configuration of a DB connection, only the `exportinfo` records are processed that contain the configured subsite in `exportinfo.hausnr`.

**Export Service: New interface "CANCELORDER"**

Order cancellations are transferred to AWP using this interface.

The interface records in `exportinfo` table are generated by the back end.

Records with the new interface are preferably processed by the export service. Attention! For this, the polling interval in the config tool must be configured so that it is appropriately short.

The export services calls a PPS Webservice method, which executes the order cancellation in AWP. The return value of the method indicates whether or not the order cancellation was executed successfully in AWP:

- Return value > 0 indicates that the cancellation was executed successfully.
- The value -1 indicates that the action could not currently be executed due to content problems (e.g. OrderXML is being imported now).
- The value -2 indicates that the order was neither found in the database nor as OrderXML.
- The value -3 indicates that there are technical problems (e.g. DB connection problem, program error).

Successfully processed records are transferred to the `exportinfo` table, in the process the long value from `exportinfo.izeit` (insert-time) is transferred after `exportinfook.longwert1`, so that records for the same order can be distinguished using the time stamp.

Records that encounter an error stop with status < 0 in `exportinfo`. In `exportinfo.fehlertext` the error that occurred is described and the error code specified.

In the PPS Webservice, the new method for order cancellation is available starting with Version 13.04.1330.

**OrderXML Service**

In the config tool of the OrderXML Service, you can maintain a site number. Effective immediately, it is also evaluated by the OrderXML service, so that only such transactions from the `ottransfer` table are read that fit the configured site number. If in the configuration the site number was assigned the value 0, as previously, all data records will be processed.

The entries in the table `ottranssav` will serve only research purposes in the future. The previous logic of sending a special OrderXML to the previous sites in case of a site change was deactivated since it was causing problems.

`EXPORTSERVICE_WAIT_CANCEL = X`

Here you should enter the max. wait time for the response from AWP. If within this time there is no response, then the user is informed that it did not work. If the switch is not active, the wait time is 5 min.

> **CAUTION:** This functionality cannot be used together with the logic `SITE_DEPENDENT_NUMBERRANGES`.

### 8.7. Reference

#### 8.7.1. Site assignment

If a new order with reference to an order from another client is entered, then the new order receives the current client into which the employee entering the order is logged in.

However, the system can be configured so that for the reference of the client, the reference process is retained.

`BEZUG_ALTES_HAUS` (client reference: no)
(Case #221522): If this environment variable is set, the site is copied from the reference document when the sales transaction is generated manually and is not reoccupied.
This variable is only evaluated for systems without internal client separation.

### 8.8. Expansion of the automatic invoice creation

The menu for automatic issue of delivery notes and sales invoices now shows the client number.

Furthermore, the import functionality was also, if the internal client separation is activated, expanded to include the client number.

For a collective invoice, only transactions with the same client number are grouped.

### 8.9. New supply type "not available"

An article or an article variant (color, size, or thickness variant) can be set - for one or more clients - to supply type **not available**. This means that this article is neither produced, ordered, nor taken from stock; this article can therefore not be sold by certain clients.

However, setting this supply type for the client "Callcenter" should be avoided.

After allocation of a transaction to a production site, under some circumstances it can happen that the redetermination of the client-specific supply type causes a product in the order or an element in the BOM to be "not available." The checking on the BOM level is only performed if the item itself is not ordered. Such an order is not automatically forwarded to the system, but rather remains in the release pool of the allocated site with the note "item not available."

Which items in the order in question are affected can be seen on the release screen with `<F5>`; alternatively, you can click the mouse or press `<SHIFT+F5>` to jump directly to the order. The information is displayed in the form of order notes.

> **Caution:** It is IMPOSSIBLE to change the supply type not available simply by a toggle or by entering a supplier!

Because, however, the saving of the order with non-available products is not allowed, you can only achieve the change of the supply type by selecting another variant or force it through another allocation of the production client.

If a product with the supply type not available is the result of an order amendment, you can change it by allocating a new site only until the order is locked due to production or PO. The item has to be removed from the order in this case.

The same applies to BOM parts.

Manually changing another supply type to `not available` is not permitted for the item nor for the BOM.

> **Important:** If a BOM article has been set to Included at the call center, this supply type will not be changed.

### 8.10. Document search via site number

The hit screens of some transaction selos were expanded to include the site number. Both for the expanded transaction selos as well as for purchasing, the site number can be entered as search criterion. The hit screens also include the site number. Furthermore, these screens were enlarged and equipped with tabs and buttons, which greatly increases the operating comfort and clarity of the screens.

Also in the transaction research, the user can now restrict the hit quantity with the site number.

### 8.11. Total surface for objects

For each object, under the menu element Sales > Object Budgeting > Object Accounts, a surface can be defined that is provided for the object.

When entering orders for the object, the surface is always booked to the object account and when saving the order, there is a check whether the total of the surfaces exceeds the defined total surface. If the check indicates that the total surface is exceeded, then a message is output to inform the user. If no total surface is defined for the object account, there is also no check.

## 9. Call center solution

It must be noted that the CALL CENTER solution cannot be regarded separately from other configurations. It also works with A+W iQuote, so that the configuration may also be included there or in the general A+W Enterprise documentation.

### 9.1. Configuration

**`CALLCENTER`** (site reference: no)
With these environment variables, the call center logic is switched on within the multi-site configuration. The environment variable contains the site number of the call center site.

**`CALLCENTER_BY_USER`** (client reference: no)
[AW-131360]
If the entry of documents is handled via the call center logic, then by default, the call center is also the client on which the documents are entered.
With a new configuration, the employee's master data is evaluated during determination of the client. The assignment to the call center must also be done via assignment in the employee master data.

**`CALLCENTER_SP_ART`** (site reference: no)
In these environment variables it is defined how the site assignment and approval of orders works within the call center.
- `0` - Stored Procedure get_md (Vitro)
    - Parameter: Order `<auftrnr>`
    - Return: target site
- `1` - Stored Procedure getProductionSite (NSG)
    - Parameter: Order `<auftrnr>` and starting with version ALCIB 2012 procedure `<vorgang>`
    - Return: target site, approval 1- Yes / 0 - No, comment (maximal char(30); the approval mark is only taken over if the order entry is done via EDI (kauf.eingang = 4 oder 14)
- `>1` - Target site (e.g. for tests)

**`CALLCENTER_SP_DIRECTDELIV`**
The number of additional parameters in addition to the keys `aufnr` and `posnr` that should be sent to SP)
Currently implemented is 6:
`getDirectSupplier(kpos.aufnr, kpos.posnr, default supplier (kpos.liefnr), kpos.artnr, postal code of the delivery address (kauf.lplz), kfzcode of the delivery address (kauf.lkfzcode)).`
[AW-156214] (September/2023)

**`DFUE_CALLCENTER_STAY`** (client reference: no)
EDI orders (external and internal) in the release pool of the call center can get a site assignment directly in the pool and be released. With this assignment, the assignment via SP no longer applies.
Whether the EDI orders remain in the call center release pool is decided via `mpdfuectrl` ID 65.

**`IQUOTE_CALLCENTER_STAY`** (client reference: no)
If this environment variable is active, online orders (entered in A+W iQuote) that are entered in the CALLCENTER remain in the call center. There is no automatic site assignment.
(see also "EN-CONFIG-A+W Enterprise" section "Release pool")

### 9.2. Initial version

The order is usually entered as an order in the call center. If the production client is not allocated manually, the system will check whether an allocation shall be made when the order is saved. This is important in case of major additions to the order in which case a premature allocation of the production client would not make sense. If an allocation is not desired at that point, a window pops up that allows entry of the reason why the order shall remain in the call center's release pool. The input field is preset with "Order to be changed"; this can be overridden or completed. When you save this order again, there will be no additional check regarding a possible release of this order; the order is transferred to the release pool of the call center.

If the question regarding allocation is answered by YES, all other criteria for releasing this order will be checked. If there is a hindrance (e.g. cash in advance or if the user is not entitled to release orders), the order is passed on to the background process `intauf` in the call center to be allocated to a production site. If company XX has been determined, the order is processed by the background process `intauf` at the allocated site XX and will remain in the release pool of the new site XX. If the order is suitable for release, then comes the question whether the order should be released. If you decide in favor of the release, then after the successful production client allocation in the site "Callcenter" and editing of `intauf` in the new site XX, there is a transfer to the production module PMS and additional system modules in site XX. If you do not want a release, then after successful allocation, the order lands in the pool of the site XX.

**[AW-149678] // September 2023: releasing of call center orders**

If an order is entered in the call center and automatic site assignment is desired, then comes the question whether this order should also be released. For EDI orders via call center, for the automatic site assignment via SP it was decided at the same time whether or not the order is released.

The logic of the release was now also expanded to the orders entered manually in A+W Enterprise. If for the entry a release was desired, it was checked nevertheless via SP and possibly then stopped and put in the pool. The reason for the rejection is also reported via SP and is visible in the pool.

**[AW-145848] // September 2023: releasing and site assignment of A+W iQuote orders in the call center**

See also "EN-CONFIG-A+W Enterprise" section "Release pool"

**[AW-156214] alcib - 13.04.14857 (April/2023)**
EDI orders remain in the release pool of the call center

See also "EN-CONFIG-A+W Enterprise" section "Release pool" and EN-CONFIG-A+W Enterprise EDI"

### 9.3. Manual PU price

Manual purchase prices and conditions are not taken over from the call center into the production clients.

**[AW-157824] // October 2023**
If an order is entered in the call center and a manual purchase price is entered for an item to be ordered completely (item - "Prices" tab), this price is also retained after the client assignment. This does not affect a manual change of the purchase conditions (item - price field - Shift+F9, F4 Price details - Order conditions - F2). A manual change of the conditions is overwritten in the production client with the values valid there.

### 9.4. Supplier determination after client assignment

If an order was entered in the CALL CENTER, it is assigned a client directly after entry according to customer-specific rules. After the assignment, the procurement types of the assigned site are determined for all products and BOM elements. This also affects the supplier assignment for ordered articles.

If the order is of the delivery type "drop shipment", then with appropriate configuration a customer-specific stored procedure (SP) can be called for an individual supplier assignment. This can help optimize the delivery paths, for example. The SP is called for each item with the procurement type "PO" with the appropriate parameters. As parameters, the following parameters are passed:

1.  `interneAuftragsnummer` (kpos.aufnr)
2.  `interne Positionsnummer` (kpos.posnr)
3.  Default supplier of the item article in the newly assigned client (kpos.liefnr)
4.  Item article number (kpos.artnr)
5.  Postal code of the delivery address (kauf.lplz)
6.  Country code of the delivery address (kauf.lkfzcode)
7.  Previous item supplier from the call center
8.  Client number to which the order was assigned

The call is only made with change of the item article number, of the default supplier or of the previous item supplier.

The SP must return a valid or deviating supplier number for the item. Here, A+W Enterprise does not check whether this supplier is also assigned to the site to which the order is assigned. This check is the responsibility of the customer within the SP. A+W Enterprise only checks whether the supplier exists in the master data and is not shut down.

**`CALLCENTER_SP_DIRECTDELIV`**
The number of additional parameters in addition to the keys aufnr and posnr that should be sent to SP
Currently implemented is 6:
`getDirectSupplier(kpos.aufnr, kpos.posnr, default supplier (kpos.liefnr), kpos.artnr, postal code of the delivery address (kauf.lplz), kfzcode of the delivery address (kauf.lkfzcode), previous supplier, new client number).`

### 9.5. Client-specific change of order after successful allocation

The allocation is only made for orders that are entered with site = Callcenter. If a production site is determined, all client-related data will be adapted.

For all articles, both in the item and in the BOM, the supply types, suppliers, stock, delivery times, will be re-pulled. After the fact, the order is completely recalculated.

Allocation of a new site also results in a recalculation of the customer route (or the route to other clients if another destination is entered) and a possible correction of the delivery date.

### 9.6. Reference to an allocated order

If a successfully allocated order is used as a reference for a new order, the site allocation will be lost. Right after loading the order data, the site is automatically reset to 'actual site' (call center); all client-related data for all articles will be reloaded, and the order will be recalculated. The route and the date will also be obtained for the current site.

This does not apply if an invoice is entered referring to an allocated order. All direct following transactions retain the allocated site.

### 9.7. Failed allocation

If the orders could not be allocated to a site (for whatever reason), they will remain in the release pool of the current site (call center). These are marked in the pool with the note "No site assignment." The orders from the release pool of the call center cannot be released directly from the pool. The renewed transfer to the system is only done through a manual change of the order. You can move from the pool to each individual order with `<Shift+F5>` or by clicking the order field.

### 9.8. Total surface for objects

For each object, under the menu element Sales > Object Budgeting > Object Accounts, a surface can be defined that is provided for the object.

When entering orders for the object, the surface is always booked to the object account and when saving the order, there is a check whether the total of the surfaces exceeds the defined total surface. If the check indicates that the total surface is exceeded, then a message is output to inform the user. If no total surface is defined for the object account, there is also no check.

## 10. Purchase

### 10.1. Extension in PO pool

In contrast to one-client operations for which from the PO pool, the dispatch notification, and the invoice check the supplier can be taken over directly in the item master data as standard supplier, with internal client separation this is no longer permitted and the takeover is refused with a message.

### 10.2. Rack-related incoming goods

With #344831, the function "rack-related incoming goods" was expanded for the multi-site logic. The description of the overall function is in the A+W Enterprise Configuration Guide.

## 11. Information systems

The call "Customer" in the information systems was expanded with entry of the company number.

## 12. PMS / AWP

For clients who order all products and do not have their own production, a special configuration with the environment variable `PMSPURCHASETRIGGER` is required. The detailed description is in the "EN-CONFIG-A+W Enterprise EDI" configuration guide. The function is also called "PMSO".

The variable `PMACLEANUPMANDANT` must be set to the site number (HNR) of the site that should delete old data from the tables. Note: also locked for the other sites are the tables in the time. Therefore, the values for `PMZARBEITSBEGINN` and `PMZFEIERABEND` (they determine when the clean-up may take place) should be selected so that all sites are not working at this time.

For reporting from other programs via file interface, it must be noted that the path specifications must be set site-specifically. Most easily via the switch `PMXCOMM`.

For more information about the configuration of the direct data import from ALCIM from PMS, see the document `\\jupiter\DOKU_DocuWare\ALCIM2000\Import\DirekterDatenimport\User_Manuals\TU_030218_DirekterImport_58749.doc` (chapter "Information collection /> Internal Client Separation").

For reporting from ALCIM, heed the document `\\jupiter\DOKU_DocuWare\ALCIB-PMS\PMS-Schnittstellen\User_Manuals\ALCIM_Rückmeldungen_im_PMS.doc`.

Site separation currently takes place functionally only within the rough scheduling. The detailed scheduling does not distinguish, however the separation can be achieved through suitable site assignment of all resources.

## 13. Dispatch control

### 13.1. Interim goal for dispatch

ALCIB dispatch control shall offer functions that allow a company (site A) to organize shipment via a second site ("via plant"), i.e. the goods will be shipped from site A to the "via plant" site and from there on to the customer. That is, the goods are first transported from site A to the "via plant" site and from there to the customer.

This logic is documented in a separate Section.

## 14. A+W Enterprise - Barcoding

Is currently not prepared for site assignment. However, the barcode background process would be able to run in such an environment assuming that there is only one background process for all sites.

## 15. Replications

### 15.1. Master data transfer (old master data replication)

With 2008 for 2009 termination - no adjustments with respect to internal client separation and UTF8.

### 15.2. Key tables (old key replication)

With 2008 for 2009 termination - no adjustments with respect to internal client separation and UTF8.

### 15.3. Item transfer (old item replication)

With 2008 for 2009 termination - no adjustments with respect to internal client separation and UTF8 - no availability with internal client separation.

### 15.4. Table distribution

Is initially not active with internal client separation.

### 15.5. External Market Partner Interface

Cannot run simultaneously on several sites since with each scheduling, first the working table `impdfue` is emptied and then filled per load. Thus it could happen that a table just filled is emptied right away by the next process. However, it is possible to ensure via configuration that scheduling may only occur on one main site => Where we would be with `xhaus.intern_md` again.
=> taken care of, may only be started on main sites.

> **Attention:** The defined main client may not be on another server (`xhaus.host`). You must pay special attention to this if clients are taken over step by step into internal client separation and during this transition time, internal EDI should run on the old computers with other clients (keyword "status reporting").

A+W Enterprise 6: `trm_ctrl` BUILD :8498 DATE :2023-01-16 10:45 buildentry 13.04.8498

Within the internal client separation, it is defined that the external market partner interface can be started exclusively on the main client.

In the course of update projects, it can happen that the main client is not yet available in the system of internal client separation. For this case, as an exception and for a limited time, the environment variable `DFUE_MPDFUE_MANDANT` can be activated with the client number to which the external market partner interface should transfer.

### 15.6. External EDI

Only to be started on main site!

**Starting with 2011 `trm_ctrl` build 1106 (ID 248261) it applies that:**

- If `CALLCENTER` is defined, then scheduling only in `CALLCENTER`
- If `CALLCENTER` not defined, then scheduling on main site.
- Reason: most of the filters cannot run in parallel. Therefore, restriction to one site.

If you are working with the following interfaces in the appropriate versions, the configuration can be converted to parallel processing. In this case, scheduling can be done into each site directly.

| No | Filter | Parallel |
| :--- | :--- | :--- |
| 1 | `i000filter` | starting with 4.5 (2011) |
| 2 | `iskafilter` | starting with 4.3 (2008.2) |
| 3 | `iverfilter` | starting with 4.3 (2008.2) |
| 4 | `iegofilter` | starting with 13.0 (AWE 6) |
| 5 | `ifenfilter` | starting with 13.0 (AWE 6) |
| 6 | `ihuefilter` | starting with 13.0 (AWE 6) |
| 7 | `ivelfilter` | starting with 13.0 (AWE 6) |
| 8 | `iwirfilter` | starting with 13.0 (AWE 6) |
| 9 | `itelfilter` | starting with 13.0 (AWE 6) |
| 10 | `ikerfilter` | starting with 13.0 (AWE 6) |
| 11 | `iwinfilter` | starting with 13.0 (AWE 6) |

## 16. Corporation Statistics

Always worked only for Schwabenglas - questionable whether we should still maintain the logic. Now in any case I would not make any active changes for internal client separation and UTF8.
=> Commented out but not thrown away yet.

## 17. FinAc data

See #135123

**`FIBU_MANDANTENTRENNUNG`** Required if FinAc data should be transferred client-specifically.
**CAUTION:** requires development adjustment #391254

### 17.1. Transaction data for financial accounting

If internal client separation is configured, every internal client can transfer the invoice data to financial accounting. However, this function must be synchronized with the booking function of the invoices. The booking function must book the field for the client number accordingly in the interface table.

### 17.2. Internal charging

No longer available starting with 2008!

### 17.3. FinAc transfer of debtor data

The transfer of data can only be called up in main sites (only relevant for CSS and XAL).

An individual transfer of debtors is possible if the client-specific limit check is configured.

In the CSS FinAc (environment variable `FIBU_ART = 2`) the debtor transfer has been adjusted.

Now the environment variable `LIMITS_MANDANTENTRENNUNG` is evaluated. If the variable is activated with "ON," a MP record is not written in the table `CSSDUE` as previously, instead for each company-specific record in the `LIMITS` table, a record is written to `CSSDUE`.

The relevant data records from `LIMITS` are determined using the customer (MP.MPNR and MP.KULIFLAG). Per entry in `CSSDUE`, `LIMITS.HAUSNR` and `LIMITS.AKVLIMIT` are taken over from the corresponding `LIMITS` record. All other `CSSDUE` fields remain the same in all data records of a customer.

The transfer of the debtors to the FinAc must be done in temporal sequence otherwise there are table blocks.

### 17.4. Vendors

Can only be called up in main sites (only relevant for XAL).

### 17.5. FinAc totals

s.a. EN-CONFIG-A+W Enterprise EDI

**Standard**

There is an environment variable that specifies which is the FINAC central office. The variable is currently not read out site-specifically. Here, the question is (and we have to clarify this with the customer and/or GV) what makes sense here. Also with respect to the limit check. Which table is used `kuplus` as default for normal sites without central limit check (has no site number - key is kunr) or `limits` for client-master structure with central limit check. Currently, without adjustment it would run so that all totals on the main site must be sent and point to the site on the `FIBU_ZENT` (may not be `$HAUS`!!). Otherwise, a scheduling of the totals does not currently work client-specifically with internal client separation since the table `salden` as central table is emptied at beginning of the scheduling and then filled via load.
=> Inquiry with MKA / GV

**Upgrade**

The balance files must be imported client-specifically if the client-specific limit check is configured (environment variable `LIMITS_MANDANTENTRENNUNG`). The correct site number must be in the `salden.dat` file. As previously, there is also an appropriate implementation via the control file `$ALDATPFAD/cssmandant.par`.

If the environment variable `LIMITS_MANDANTENTRENNUNG` is set, the environment variables `LIMIT_ZENTRALE_DB` and `BUCHE_SALDEN_ZENTRAL` may not be active.

For the site-individual balance scheduling, the open items from the FinAc are written and if configured the limits in the limits table. If a customer is only in the mp table, but not created in the limits table, then there is no takeover of the open items for this site.

### 17.6. Transfer of cost centers

If internal client separation is configured, these functions will not be available.

Starting with Version 2011 (build 1087), the cost center transfer on the main site (= site to which the database belongs) can be started.

> BEFORE putting into operation, it must be checked whether this is suitable for the special financial accounting since under some circumstances data from several companies (internal sites) is transferred in a transfer file.

## 18. Message transfer

With internal client separation, it is already ensured in the message system that messages are only written for the main clients. Nevertheless, it is urgently recommended that you work with e-mail.

The messages system will only be called for the main site.

### 18.1. System message distribution

The system message distribution was also adjusted for internal client separation. It is now possible to store the mail distribution client-specifically. Furthermore, the screens on the system menu for maintenance of the mail distribution were reworked.

## 19. Construction site invoicing

No longer available starting with 2008.

## 20. Racks

### 20.1. Rack transfer

If internal client separation is configured, these functions will not be available.

### 20.2. Rack (block transfer)

If internal client separation is configured, these functions will not be available.

### 20.3. Rack comparison

If internal client separation is configured, these functions will not be available.

### 20.4. Rack distribution

If internal client separation is configured, these functions will not be available.

## 21. Project Information

No longer available starting with 2008.

## 22. Distinction (Production - Distribution)

No longer available starting with 2008.

## 23. Barcode Data

I have not simply done so that the barcode EDI can only be started on the main site and data transferred only to external sites (`xhaus.hauptmandant=0`).

## 24. Via plant / ViaPlant

A+W Enterprise dispatch control offers functions that allow a company (site A) to organize shipment via a second site ("via plant"), i.e. the goods will be shipped from site A to the "via plant" site and from there on to the customer. That is, the goods are first transported from site A to the "via plant" site and from there to the customer.

Another special feature is the dispatch via a second production site. Basically, there are three different cases:

1.  An order is produced by site 1 but the customer calls and asks for a truck with a crane. This kind of vehicle is only available at site 3 however. The order is therefore first shipped from site 1 to site 3 and from there to the customer. Since the customer is asking for a special service, he will basically agree to a change of delivery date.
2.  With some customers, it is clear already at the start (via the route number) that the shipping has to be "via city XY" because the order must be delivered by plant 3 (city XY) because the customer has asked for a crane when placing the order.
3.  The shipping coordinator decides at short notice that one (or more) orders will be shipped via city XY because other orders of this customer will be produced in city XY anyway so that they can be shipped together on a smaller truck.

The „rescheduling" described in 1. and 3. may happen until shortly before the actual delivery which means that the orders are already in local correction.

To handle these requirements, A+W have created a so-called „interim destination logic" (similar to an interim destination in a navigation system). The new route type „internal" has been implemented in ALCIB route data for this purpose. With specification of such a route, a screen opens on which the shipper enters the site number of the "interim destination." This site number is allocated to a route. In addition, the number of the route leaving from the interim destination is entered. This entry means that the shipping data of the original route is copied to the new route. An additional flag with the values:
- `0` = default
- `1` = data copied, glass not available at the interim destination
- `2` = target quantity is available at the interim site

Due to the "packed" message at the interim destination, the goods removal is booked.

If the site/area allocation is not clear (because every site has local routes as well, e.g. city XY – East, XY -West, XY -North, City XY -South), the „Priority flag" defines the route to be copied to.

The delivery note is issued at the producing site and accompanies the shipment.

Losses (breakage) occurring between the two sites will be handled in the same way as losses/breakage occurring between shipping site and customer.

A database-wide solution is impossible at present; shipping via country XY (and vice versa) has to be handled by organizing.

### 24.1. Master Data

#### 24.1.1. Reg. No

In MASTER DATA => KEYS => SYSTEM => DISPATCH => DISPATCH REGIONS, for all internal sites that can function as intermediate destination, a region must be created that has the site number as key number.

Furthermore, the delivery areas should be broken down into regions. There can be several routes for a region. However, a route can always only be assigned to one region.

#### 24.1.2. Route maintenance in master data

Each route in the Master Data > Keys > System > Dispatch > Routes > Routes must have a site allocation.

With internal client separation, there is a distinction between the known routes to customers (common, pick-up-, or direct delivery route), and purely internal routes, between sites only. These routes must be set to type internal. For a route between client X and client Y, enter the client number X in column `site` and the client number Y in column `Area/Site`. For every client, there should be a 1:(n-1) allocation of internal routes to all other internal clients.

**Example:**

**In site 20**
- Route 23: internal route from site 20 to site 30 -> site: 20 area/site: 30
- Route 24: internal route from site 20 to site 40 -> site: 20 area/site: 40
- Route 25: internal route from site 20 to site 50 -> site: 20 area/site: 50
- etc.

**In site 30**
- Route 32: internal route from site 30 to site 20 -> site: 30 area/site: 20
- Route 34: internal route from site 30 to site 40 -> site: 30 area/site: 40
- etc.

The other customer routes at site X are entered in column `site` X; in column `area/site`, an internally defined area number is entered.

**Example:**
The delivery area is divided into 4 regions, the distribution and numbering of the regions can be selected freely.
- 100 - South
- 200 - West
- 300 - North
- 400 - East.

For site 20 (Linden), there are the following routes for instance:
- Route 211 (LI - Berlin) => allocation: route 211 to site 20 and area 400
- Route 212 (LI - Hamburg) => allocation: route 212 to site 20 and area 300
- Route 213 (LI - Munich) => allocation: route 213 to site 20 and area 100
- etc.

You have to make sure that at least one route exists per area for each site with a priority > 0.

For site 30 (Frankfurt), the routes are:
- Allocation: Route 311 FR- Berlin to site 30 and area 400 priority 1
- Allocation: Route 312 FR -Halle to site 30 and area 400
- Allocation: Route 321 FR-Hamburg to site 30 and area 300
- Allocation: Route 335 FR-Munich to site 30 and area 100 priority 1
- Allocation: Route 338 FR -Stuttgart to site 30 and region 100

If you define several routes per site and area, you should define one with the highest priority so that this one can be used for automatic route determination if the site is changed.

#### 24.1.3. Market partner master data

A route must be entered for each address of a market partner.

### 24.2. Order Processing

#### 24.2.1. Determining the route for an order

For each customer, one default and up to three alternative routes can be stored in the master data.

During entry, the system first checks if one of the defined routes is suitable for the site in which the order has been entered. If the default route for the current site is not permitted, then the stored alternative routes are checked.

If none of the existing routes is permitted for the current site, then the route to the customer is determined as follows:
From the stored default route, the allocated area is pulled; after that, there is a search in the current site for routes for this area. If there are several valid routes, the route with the highest priority will be chosen.

Please note that the customer route can be overwritten with the route from the default address. In this case, the alternative routes will not be considered.

**Example 1:**
For customer 11111, the standard route 335 and alternative route 338 are defined.
An order is entered in site 20 for customer 11111.
Route 335 does not exist in site 20, neither does the alternative route 338, therefore, the area of the route 335 is determined: Region 100 (South).
After that, the system searches for a route for site 20 and area 100. It finds route 213 which will be used for this order.

**Example 2:**
For customer 11111, the standard route 335 and alternative route 238 are defined.
An order is entered in site 20 for customer 11111.
Route 335 does not exist in site 20, but the alternative route 238 does. Route 238 is taken over into the order.

**Example 3:**
For customer 11111, the routes exist as in example 2, but there is also a default delivery address with route 338.
In this case, the alternative route 238 is not taken over, but instead, the route is pulled from the address data. After that, the route is determined as in example 1 via the area 100 in site 20; the route 213 is allocated.

#### 24.2.2. Shipment "via site" ("via plant")

During entry of an order, the user can already determine that the order will be shipped via another site. In field Route in the order header use `<F5>` to select or enter another internal shipping site.

With selection of a shipping site, the route will be determined according to the logic described above. The new route for the shipping site is written in field `Shipping route` however; this field belongs to the first MODE menu in the order header. The original customer route is replaced by an internal route which is determined based on the data current site - shipping site.

To signal that shipment will be effected by another site, the route field is marked `*`.

Alternatively, you can enter the shipping site directly on the 1.MODE screen of the order header. Deleting the shipping site can only be done via another allocation of the route, by replacing in the order header the internal route determined for the shipping site with a route directly to the customer.

**Example 4:**
In example 1 for customer 11111, route 213 was determined for site 20. If you decide to ship via site 30, the end route for customer 11111 and site 30 is determined first:
a. area for route 213 in site 20 is 100. Route for site 30 and area 100 is 335. Therefore, the shipping route is 335.
b. Now, the system determines the internal route from site 20 to site 30 => route 23, the route is set to 23.

#### 24.2.3. Calculation of the route date when shipping "via site"

The delivery date is determined in two steps. After entering the required date, the system first calculates the delivery date for the shipping site. This calculation is based on the shipping route of the shipping site. The new date is first corrected by the handling time for the internal route (only to be maintained for internal routes in route master data) and is then assumed as the required data for calculating the delivery date for the present site and the internal route.

**Example 5:**
Route 335 in site 30 in example 4 is done only on Wednesdays, the internal route 23 from site 20 to site 30 only on Wednesdays and Fridays, with one day handling time.

**Calculation:**
- The date requested by the customer is 24.9.2007 - Monday. (`kauf.ltideal`)
- Delivery date for shipping site 30 would be 19.09.2007 – Wednesday.
- Correction by handling time 19.09.2007 - 1 day: 18.09.2007 - Tuesday
- Delivery date for current site, route 23: 14.09.2007 - Friday
- The date 14.09.2007 is entered in `kauf.ltplan`.

**For comparison:**
If the site (20) had not been changed and the route 213 remained valid, the delivery date would have been determined based on the required date (24.09.2007) and the plan of the route 23 determined and thus specified as 21.09.2007.

#### 24.2.4. Changing the route and end route in the order

Field Route can be changed at order entry. You can only enter routes belonging to the present site however. Selection via Selo `<F9>` only shows the routes allocated to the present site.

This rule also applies for the call center. Since the allocation to the production client is done at a later point in time, initially only the routes allocated to the call center can be selected.

The route cannot be changed at random. A normal customer route cannot be replaced by an internal route between two sites unless the customer itself is one of the shipping sites.

When you try to replace a common route with an internal one, the system will inform you that this change is invalid, and can be made only by selecting the shipping site. The middle column of the first mode menu in the order header shows the shipping site and route for the customer, which can be changed there if required. If no shipping site is selected, you cannot choose a shipping route, neither manually nor via selo.

When you open the route selo, the system will only show the customer routes for the shipping site. Internal routes are not displayed. Confirm your selection of the marked route with `<ENTER>`. If no route is chosen and you exit the selection menu using `<END>` or `<POS1>`, the new route will not be adopted.

### 24.3. Dispatch control

The tree structure for the shipping data offers the following options:
- Input from date to date, i.e. overview of several shipping days
- Input by client and overview of all clients
- Left side of the shipping explorer is active, right side of the shipping explorer inactive (view only)
- Shift routes, orders, items via right mouse key:
    - The shift menu has been completed by the fields via site and final route for this purpose.
    - In the shipping department, changes can be made by route and order (complete orders).
- Splitting an order into parts, which should be delivered on the one hand directly to the customer, on the other hand via a site is not possible.
- By shifting an order from an internal route to a direct route to customers, the data in the shipping of the earlier shipping site is finally deleted and only remains in the producing site with allocation to the new route.
- Shifting of orders from one shipping site to another is impossible at present. Shipping of goods via another site is limited to two sites.
- Access the orders by clicking on the route on the left side
- Access the items by clicking on the order on the left side
- Global search including all clients.

#### 24.3.1. Via site logic / Via plant

Define the Via site logic by pressing `<F5>` in the order header, field Route.

**Data and shipping status in case of "via site" shipment**

If you choose shipment "via site" for an order, two records per item will be created in the shipping department: one record for producing subsidiary (site 20) and one record for delivery (site 30). As described in example 5 in point 3.1, the records per item in site 20 and site 30 will be created as follows:

- **Record1:** Order: XXXX, Itm: 1, Site: 20, Delivery date: 14.09.2007, Route: 23, Status: 0, ...
- **Record2:** Order: XXXX, Itm.: 1, Site: 30, Delivery date: 19.09.2007, Route: 335, Status: 1, ...

The status value of an item record in shipping provides important information.
In case of "normal" shipment directly to the customer, all records always have the status=0 which means that these records can be changed at random in the shipping department (based on the shipping progress).
In case of "via plant" shipments, the record is immediately created and visible at the shipping site, but has status 1 and is therefore in lock mode. In lock mode, data can be changed only to a certain extent. The data serve primarily an informational purpose, however shifts can also be undertaken.

When you shift the data to "via site" or split it, the system will tell you that this may cause problems regarding the connection of communicating records because data are not yet available or cannot be allocated at the production site later on.

Whenever data is shifted by a production site, no matter if this is done manually or triggered by the production module for capacity reasons, the system will always try to shift the data at the shipping site as well. If the linked shifting at the shipping site does not succeed, the shifting at the producing site will be executed nevertheless and the user informed that the data in the "via" site must be adjusted manually.

When an order has been reported complete and packed at the producing site (site 20), either by the system or manually and a delivery note has been created, the order is also set to status 3 (delivered) in site 20. With the message about the information, the corresponding records in site 30 are set to status 2. The available and packed quantities are updated. All shipping functions are available again for this order. The corresponding records in site 20 with the status 3 are locked for further processing. It counts as fully delivered.

A delivery receipt of goods at the shipping site is reported booked via the Delivery receipt menu. The input menu serves to enter the search criteria to restrict the number of hits to a certain order, a complete route, or a certain production site. Depending on the search criteria, the data is fetched from one or all sites. For one or all orders on a route searched for, the anticipated delivery quantities and receipt quantities that count as "under way" are displayed.

Goods are considered to be "under way" if the production site has issued a delivery note. (For additional information about this topic, see the transaction for finished goods stock.) The quantities are obtained from the delivery note of the producing site and the quantities of the shipping site are adjusted.

If site 1 has reported 200 pcs. for item 1 shipped to site 2 on 10.09.2007 and the data have been split at site 2 for customer delivery so that for 13.09.2007 and 14.09.2007, 100 pcs. are scheduled for shipment, shipment of item 1 on 13.09.2007 (100 pcs.) and 14.09.2007 (100 pcs.) will be suggested when receipt of the goods has been reported.

If just the shipping site is entered in the input menu for the 'receipt' report, the system will show all order items to be expected from the production site. Their status at the production site is "not arrived" (`lapool.status=1`).

The Receipt field shows the quantities that are on their way to the shipping site (for which the production site has issued a delivery note). You can take over or reduce the quantities. In order items for which the Receipt field has been filled, the code `Book` is automatically set as `YES`. By removing the Book code, you can keep one or more complete items as "not received" in the system, and report them as "received" later on.

Here's another overview of all possible shipping status:
- `0`: order is free, original record in the producing site
- `1`: one record in the shipping site, not yet arrived, not changeable (except for shift), record locked
- `2`: the record in the shipping site, which is reported as arrived, no lock
- `3`: the original after delivery, record locked

#### 24.3.2. Finished products stock

The finished goods stock provides an overview of the whereabouts of the goods at all times:
- in the finished goods stock of site A
- on the way between A and the „via site" plant
- in the finished goods stock of the "via site" plant
- on the way to the customer
- completely delivered by "via site" plant

Data is stored in tables `lapfertwb` (finished goods stock) and `lapfertwbprot` (booking log for the finished goods stock).

**Handling for the search for an order:**
1. Search for an order by `<Ctrl> + <K>` or press button [Skip] for an order in the shipping explorer as described above.
2. After entering the order number, press `<F3>` or the [Release] button.
3. The following view appears for via site shipments:
This view gives an overview of the delivery of the order in question. All items of the order are displayed twice: 1. for the site producing the goods and 2. for the site used as a stopover for delivery. The articles marked in white (status: open) are available at the Starting site as well as at the via site plant. There, the marking is red (status: locked) because the goods have not actually reached the via site plant. The status changes in the process of events to show the whereabouts of the goods at all times.
4. If you enter another order number and press [Skip] you will move from this view to the defined order; from there, you can also load the order view for the other "via site."
5. Once the goods are complete in site 542 for instance, they have to be reported packed. This report can be released by production, barcoding, or manual packing in the shipping area (depending on the system configuration). You can load the menu for manual packing on item level by pressing `<F4>` Check missing quantities.
6. The missing quantity check is released by pressing [Book]. This action gives the goods the status `Completely packed`; check box `cmp`. is ticked. Use `<Ctrl> + <K>` to get information on the statuses at the different sites, and to view the finished goods stock.
    - Yellow: goods completely packed
    - Red: goods locked
7. At that point, the finished goods stock only shows the order items for site 542 as the goods are actually available only at 542 and are not on its ways to site 642 yet.
8. Status `Completely packed` at site 542 allows to book the entire order to 'transport'. This is done in menu `<F4>` Book to transport on order level. At the same time, preliminary delivery notes are released for printing, and the order status changes. This booking provides further information in the finished goods stock because the goods are now on their way to site 642. You can see this from the destination site's entry in the finished goods stock of 542. This information is also available at 642 so that the via site plant already knows that the goods from 542 can be expected.
9. Press [Skip] to get right to via-site 642. Use `<F3>` to trigger this action; the order appears on item level for site 642. Once the truck has reached site 642, the system expects the receipt of goods so that the goods are actually booked for 642. At site 642, this receipt of goods is booked on item level via menu F4 Receipt of goods, triggered by `<F3>` or via button [Trigger] and `<End>`.
10. This sets the goods at site 642 to `Completely packed` and they are now available for shipment from the via site plant to the customer. Use `<Ctrl> + <K>` to call up additional information about the order. Status Transport shows that the goods are no longer available in site 542 but have not reached the customer yet. Status `Completely packed` in site 642 means that the goods are actually available there, and can be shipped on.
11. When the truck has been loaded for the customer, site 642 has to set the goods to 'transport'. This is done in menu `<F4>` Book to transport on order level. Preliminary delivery notes can be issued and printed; the order status changes. The destination site is set to -1 in the finished goods stock. This means that the goods are on their way to the customer.
12. If the goods are shipped with a preliminary delivery note, this would be signed and returned to site 642 in real life. This again would be the trigger for a delivery note. This action therefore relieves all shipping information in sites 542 and 642; the goods are considered completely shipped. The delivery note is issued in menu `<F4>` Deliv./receipt of goods Release + print, `<F3>` or button [Release]. All items in sites 542 and 642 have now got the status `Completely shipped`.

#### 24.3.3. Complex example

If an item or part of an item does arrive on time when being shipped from a subsidiary via plant (not completed on time, broken on the way...), only the quantity actually received can be booked. The rest still remains at the subsidiary because the missing quantity has to be remade and shipped. The status of the goods therefore differs. The packed goods are marked as `Completely packed`. The open item still remains open but gets a different date due to the delay. Both show the site number 542. The status of the goods ready for 642 does not change.

After the 'packed' report, the goods have to be booked to 'transport' which triggers printout of the preliminary delivery notes.

The status only changes for the goods that have not been moved. The goods at the starting site are marked as 'under way'. At the 'via plant', the goods are still locked because they have not been received. The moved item is still marked as "open".

When the goods arrive at the 'via plant' they are booked as receipts.

Receipt of goods immediately changes the status of the goods received to 'completely packed'. The goods are now at the customer's disposal. The via plant can now ship these goods, or wait for the open item.

- Item 1 is still open at 542 and locked at 642
- Items 2-5 are marked as under way at site 542 and as completely packed at 642

> **Please note:**
> When the goods are returned, manual intervention in the production process is required; the information is available everywhere but the person in charge has to react accordingly. Example: a sheet damaged at the customer's has to be moved in shipping control as well (with the corresponding explanation). Production of the sheet is based on the manual input of an order. This new order passes the whole production chain to fulfil the customer's order. Booking the non-shipped goods will trigger no new order in ALCIB!!!

### 24.4. Environment variables

**`RABATT_AUS_ENDROUTE`** (site reference: no) (starting with ALCIB 2012)
If this environment variable is set, for "via plant" deliveries, the final route is used as discount criterion instead of the route.
