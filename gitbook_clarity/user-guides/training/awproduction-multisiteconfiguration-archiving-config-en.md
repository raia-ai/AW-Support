---
description: "AWProduction MultiSiteConfiguration Archiving Config EN"
---



title: "EN-CONFIG-AW_Production_4"
source: "EN-CONFIG-AW_Production_4.pdf"
tags: ["A+W Production", "Multi-Site Configuration", "Software Manual", "Archiving", "PDC", "Database Configuration", "Technical Documentation", "A+W IoT Smart Trace", "Production Monitor"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This technical document details the configuration and operation of A+W Production in a multi-site environment. It covers the setup of services and web services using the MultiSite CONFIG tool, application startup procedures, and special considerations for updates and database management."
long_description: "This comprehensive guide provides in-depth instructions for setting up, configuring, and managing the A+W Production software in a multi-site architecture. The document begins by explaining how to use the A+W Production MultiSite CONFIG tool to create and manage services and PPS WebService instances for each site. It walks through the application startup process, including site selection for users assigned to multiple sites. Key sections are dedicated to special features and the update process, outlining manual steps required in a multi-site environment that are typically automated in a single-site setup, such as database updates, designer screen updates, and managing the TRANS release. A major portion of the document is dedicated to data archiving, covering both manual and automatic archiving procedures. It explains how to configure archiving modes, set up archive databases (for both Informix and SQL Server), manage the deletion of associated files, and utilize expanded archiving methods for greater flexibility. The guide also introduces the A+W IoT Smart Trace feature for sending data to external systems, detailing gateway connection settings and PDC (Production Data Collection) configuration. Finally, it covers other functions like the Parameter Administrator for general and station-dependent settings, the management of document links across different A+W modules, and an overview of the Production Monitor for visualizing workloads and backlogs."
---

## A+W Production Multisite Config

*Figure 13-11 A+W Production MultiSite CONFIG tool services*

The following is a representation of the A+W Production Services - Multi Site configuration screen.

| Site | Service | Display Name | Service Name | User Name | Port | Existing Service |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | ☑ | A+W ALCIM Items4ALCIM (1) | 14Asvc_C1 | TSE\QMService B1 | 2100 | ☑ |
| 1 | ☑ | A+W ALCIM Booking Engine (1) | Alcim Book_C1 | TSE\QMService B1 | 2110 | ☑ |
| 1 | ☑ | A+W ALCIM Process Manager (1) | Process Manager_C1 | TSE\QMServiceB1 | 2120 | ☑ |
| 1 | ☑ | A+W ALCIM Server (1) | AlcimServer_C1 | TSE\QMService B1 | 2130 | ☑ |
| 10 | ☑ | A+W ALCIM Items4ALCIM (10) | 14Asvc_C10 | TSE\QMService E1 | 2200 | ☑ |
| 10 | ☑ | A+W ALCIM Booking Engine (10) | AlcimBook_C10 | TSE\QMService E1 | 2210 | ☑ |
| 10 | ☑ | A+W ALCIM Process Manager (10) | Process Manager_C10 | TSE\QMService E1 | 2220 | ☑ |
| 10 | ☑ | A+W ALCIM Server (10) | Alcim Server_C10 | TSE\QMService E1 | 2230 | ☑ |
| 20 | ☑ | A+W ALCIM Items4ALCIM (20) | 14Asvc_C20 | TSE\QMService E20 | 1800 | ☑ |
| 20 | ☑ | A+W ALCIM Booking Engine (20) | AlcimBook_C20 | TSE\QMService E20 | 1810 | ☑ |
| 20 | ☑ | A+W ALCIM Process Manager (20) | Process Manager_C20 | TSE\QMService E20 | 1820 | ☑ |

**Action Log:**

| Category | Action | Result |
| :--- | :--- | :--- |
| ✔Multi Site Mode | Enabled | ok |
| Connecting to A+W Infrastructure | success | |
| Creation of ODBC connection (1) | success | DSN:alcimdb_v6_b1, Host Name:QM-DBSRV TSESQL2016EXP, DB:alcimdb_v6_b1 |
| Creation of ODBC connection (10) | success | DSN:alcimdb_v6_e1, Host Name:qm-dbsrv, DB:alcimdb_v6_e1 |
| Creation of ODBC connection (20) | success | DSN:alcimdb_v6_e20, Host Name:qm-dbsrv, DB:alcimdb_v6_e20 |
| Creation of ODBC connection (21) | success | DSN:alcimdb_v6_e21, Host Name:qm-dbsrv, DB:alcimdb_v6_e21 |

In the next step, the CONFIG tool creates one PPS WebService instance per site if the tool is running on the server to which the WebService address is pointing.

*Figure 13-12 A+W Production MultiSite CONFIG tool services*

**A+W Production PPS Web Services - Multi Site**
Your A+W Production PPS Web Services will be configured for your multi site settings.
For each A+W Production PPS Web Service will be created a specific Application Pool running under your site specific service user.
A Web Site for each of the service will be created under the name PPSWebService_C<ClientID>.
You can access it under the URL: `http://localhost/PPSWebService_C<ClientID>/Albwir.Alcim.Dataservice.asmx`

**Action Log:**

| Category | Action | Result |
| :--- | :--- | :--- |
| ✔ Serviceinstall Process Manager_C21 | success | |
| Serviceinstall AlcimServer_C21 | success | |
| Serviceinstall 14Asvc_C22 | success | |
| Serviceinstall AlcimBook_C22 | success | |
| Serviceinstall Process Manager_C22 | success | |
| Serviceinstall AlcimServer_C22 | success | |
| Validate User | check user credentials | Success |

The MultiSite CONFIG tool must run on the process and terminal server.

*Figure 13-13 Services according to A+W Production MultiSite CONFIG tool*

The following table represents the list of services as seen in `Services (Local)`.

| Name | Description | Status | Startup Type | Log On As |
| :--- | :--- | :--- | :--- | :--- |
| A+W ALCIM AWPort | Scanner Access Point | | Manual | Local System |
| A+W ALCIM Booking Engine | ALCIM Booking Engine | | Disabled | TSE QMServiceB1 |
| A+W ALCIM Booking Engine (1) | ALCIM Booking Engine | Running | Automatic | TSE QMServiceB1 |
| A+W ALCIM Booking Engine (10) | ALCIM Booking Engine | Running | Automatic | TSE QMServiceE1 |
| A+W ALCIM Booking Engine (20) | ALCIM Booking Engine | | Manual | TSE\QMServiceE20 |
| A+W ALCIM Booking Engine (21) | ALCIM Booking Engine | | Manual | TSE QMServiceE21 |
| A+W ALCIM Booking Engine (22) | ALCIM Booking Engine | | Manual | TSE\QMServiceE22 |
| A+W ALCIM Datalmport | Provides interface to ALCIM master data. | Running | Automatic | TSE\QMServiceB1 |
| A+W ALCIM Items4ALCIM | Provides order data from ERP-System to AL... | | Disabled | TSE QMServiceB1 |
| A+W ALCIM Items4ALCIM (1) | Provides order data from ERP-System to AL... | | Manual | TSE\QMServiceB1 |
| A+W ALCIM Items4ALCIM (10) | Provides order data from ERP-System to AL... | | Manual | TSE QMServiceE1 |
| A+W ALCIM Items4ALCIM (20) | Provides order data from ERP-System to AL... | | Disabled | TSE QMServiceE20 |
| A+W ALCIM Items4ALCIM (21) | Provides order data from ERP-System to AL... | Running | Automatic | TSE\QMServiceE21 |
| A+W ALCIM Items4ALCIM (22) | Provides order data from ERP-System to AL... | Running | Automatic | TSE\QMServiceE22 |
| A+W ALCIM Process Manager | Provides automatic executing of processes | | Manual | TSE QMServiceB1 |
| A+W ALCIM ProcessManager (1) | Provides automatic executing of processes | Running | Automatic | TSE\QMServiceB1 |
| A+W ALCIM ProcessManager (10) | Provides automatic executing of processes | Running | Automatic | TSE QMServiceE1 |
| A+W ALCIM ProcessManager (20) | Provides automatic executing of processes | | Manual | TSE QMServiceE20 |
| A+W ALCIM ProcessManager (21) | Provides automatic executing of processes | | Manual | TSE QMServiceE21 |
| A+W ALCIM ProcessManager (22) | Provides automatic executing of processes | | Manual | TSE OMServiceE22 |
| A+W ALCIM Server | A+W Production background services | | Disabled | TSE\QMServiceB1 |
| A+W ALCIM Server (1) | ALCIM background services | Running | Automatic | TSE QMServiceB1 |
| A+W ALCIM Server (10) | ALCIM background services | Running | Automatic | TSE QMServiceE1 |
| A+W ALCIM Server (20) | ALCIM background services | | Manual | TSE\QMServiceE20 |
| A+W ALCIM Server (21) | ALCIM background services | | Manual | TSE\QMServiceE21 |
| A+W ALCIM Server (22) | ALCIM background services | | Manual | TSE OMServiceE22 |

The configuration is thus complete, the applications can be started.

### 13.3. Starting the applications

If a Windows user is assigned to several sites, a dialog for selecting the site appears at the start of A+W Production and A+W Realtime Optimizer. So that this works, the AWSOA environment must be accessible. If this should be running on the process server, the applications will not start should this server not be accessible, e.g. due to maintenance work. This was different in the SingleSite.

When starting, the TRANS drive is connected to the configured drive, e.g. P. The connected drive is still required for various older features (e.g. in the area of drivers), which cannot be worked around with the UNC path of the TRANS drive.

*Figure 13-14 A+W Production site selection*

| Name | Description | Site |
| :--- | :--- | :--- |
| C1 (AWB 1) | A+W Business Mandant 1 | 1 |
| C10 (AWE 1) | A+W Enterprise Mandant 1 | 10 |
| C20 (AWE 20) | A+W Enterprise Mandant 20 | 20 |
| C21 (AWE 21) | A+W Enterprise Mandant 21 | 21 |
| C22 (AWE 22) | A+W Enterprise Mandant 22 | 22 |

A+W Realtime Optimizer can change sites, but in the productive system there must be one Windows user per site for each A+W Realtime Optimizer. This is due to the direct coupling to a cutting table. This cannot simply be changed. The basic settings (XOPTON.CFG) are also unique per Windows user and cannot be changed.

A+W Production Terminal has no appropriate function for changing the site. Here, the correct PPS WebService must be used; this is configured as usual. When starting A+W Production Terminal, hold down the `<SHIFT>` key to reach the PPSWebService selection dialog. Enter the appropriate PPS WebService there:
`http://<ProcessServer>/PPSWebService-C<Client Number>/Albwir.Alcim.DataService.asmx`

*Figure 13-15 A+W Production Terminal selection of PPSWebService*

In order to call up the CapaView from the planning domains, the site number must be specified in the address:
`http://<Server for AWSOA Planning>/Planning.Web/<Client Number>/Capaview`

The same applies for the scanner solutions from the AWSOA CIM domains:
`http://<Server for AWSOA CIM>/CIM.Web/<Client Number>/SmartTerminalBooking`
`http:// <Server for AWSOA CIM>//CIM.Web/<Client Number>/barcodereading`

### 13.4. Special features

So that the sites have their own environments, all settings that do not come from the database are on the TRANS release of the site. Dependent applications, e.g. A+W CAD Designer (Shapes) must be configured so that these use their configurations from the TRANS release. This means with direct use of these dependent applications, these use the configuration of the last started A+W Production site. Since generally one user is assigned to just one site, there should be no problems. If this is not the case, this must be noted.

Configurations that cannot be shifted to the TRANS directory must be created in the MultiSite so that there are no overlaps. In A+W Production this affects the machine drivers that are called with batch release. Especially cutting code drivers, but also old bender and sealer drivers and new ones with special configurations. Some of the configuration of these drivers is in the programs directory. Thus it must be heeded that the configurations, directories for the drivers are unique across sites.

### 13.5. Update

In case of an update of the A+W applications in the MultiSite, additional steps must be performed per site, which happen automatically with SingleSite.

To perform these steps, it is recommended that you dial in on the ProcessServer under each of the services users since these are assigned only one site, and to perform the steps there.

**Databases**

The A+W Production database must be updated manually. This happens manually with the DBUpdateTool. In the Multisite, make sure to update all databases of all sites (also archive databases!).

**Designer screens**

The updating of the designer screens (release dialog, A+W Production Terminal screens, etc.) is done in the SingleSite automatically by the SetupLauncher. In the MultiSite, this must be done manually since the SetupLauncher does not recognize the sites.

Execute the DesignerFormsUpdater.EXE in a DOS box under each Windows services user on the ProcessServer.
`C:\Program Files (x86)\A+W\Techsoft\Tools\DesignerUpdater\DesignerFormsUpdater.EXE`

**TEXTE table**

The updating of the TEXTE table is done in the SingleSite via the A+W Production CONFIG Tool. In the future, this should be done by the A+W Production MultiSite CONFIG Tool; until this works, we must take advantage of a trick.

1.  On the ProcessServer, stop all services and end all applications
2.  Temporarily set the MultiClient switch to 0 in the registry
3.  Under each Windows services user, start the A+W Production CONFIG Tool and there, execute only the update of the TEXTE table
4.  Set the MultiClient switch back to 1

**TRANS release**

The "Shared Folder" diskset updates the data to the TRANS release. In the process, the SetupLauncher takes the directory that was configured for it; it does not recognize the configuration of the MultiSite.

The current solution for updating all TRANS releases would be to uninstall the "Shared Folder" diskset again (this should not delete any data) and reinstall it, while setting the next TRANS release in the SetupLauncher. Repeat this until you have done all sites.

Alternatively, the data from the updated TRANS release can be copied to the other releases. For this, however, you have to know exactly what is updated and what is not. If you simply copy the whole directory, the configuration will destroy the site.

## 14. Archiving

### 14.1. Manual archiving

Batches that are no longer needed in the production system can be archived. For this, the batch to be archived must be set to "archivable" in A+W Production via the batch display (batch status 2000).

*Figure 14-1 Archiving a batch in A+W Production*

As soon as the archiving has access to this batch, the status is set to "in archiving" (batch status 2001). The status 2001 marks the batches for further processing (archive or delete). With the parameter "DELETIONDELAY", you can define a delay in days between the transfer of the status 2000 and 2001. The delay refers to the database field "pool_lauf.lastmodzeit".

Archiving is done via the ALCIMServer that is installed on the ProcessServer. There are 2 ways to do this. With the first one, the batches are simply deleted; with the second, the batches are shifted to archive databases. The procedure is controlled with the switch `[ALCIM_ARCHIV / NOARCHIV]`: 0 = archive databases; 1 = delete.

*Figure 14-2 Archiving or deleting configuration batches*

**Parameter: Delete Instead of Archive**
Indicates whether the ALCIMServer removes deletable batches/orders directly. Caution: deleted data can not be restored! 0 - Default, archiving in archive databases 1-No archiving, data will be deleted. It is not necessary to configure an archive database.
- Permitted values: 0, 1
- Default value: 0
- Range: ALCIM_ARCHIV
- Entry: NOARCHIV

If batches should be archived in archive databases, then the appropriate databases and an ODBC data source must exist. One database per year and one additional database that is used for problems are required. By default, this database has the name ALCIMQRT and the annual databases have the year at the end of their names (e.g. ALCIMQRY2019). The ODBC data source must be set up on the ProcessServer on which the ALCIMServer service is running.

The ODBC connect string for the archive database must be configured in A+W Production (`[ALCIM_ARCHIV / DATABASE]`), here the syntax is different for INFORMIX and SQLServer. For SQLServer, the database user and password must be stored here for the person who has the right to delete data from the production database and write it in an archive database. This information is stored under INFORMIX directly in the IDBC data source.

**Informix:**
`DSN=<ODBC data source>; DATABASE=<archive database without year>;`

**SQLServer:**
`DSN=<ODBC data source>; DATABASE=<archive database without year>; UID=<user>; PWD=<password>;`

*Figure 14-3 Configuration of DSN for archive database*

In addition to the data in the database, files can also be deleted during archiving. These can be file with batch reference (`[ALCIM_BDESETTINGS / DELETE_FILE_WITHSCHEDULE]`), e.g. optimization results, or files with order references(`[ALCIM_BDESETTINGS / DELETE_FILE_WITHORDER]`), ORDERXML files. It is also possible to set whether SN files that are assigned to the items should be deleted (`[ALCIM_BDESETTINGS / DELETE_SN_FILES]`).

*Figure 14-4 Configuration deletion of files during archiving*

| Parameter | Value |
| :--- | :--- |
| Files to be Deleted while Archiving Batches | `$SERVERDIR$\RELEASE\SAVE #SAVE.*.` |
| Files to be Deleted while Archiving Orders | `$SERVERDIR$\Import\Archive\archived_order#* XML` |
| Deleting SN Files | 1 |

### 14.2. Automatic archiving

Since July 2020 (#45912), there are additional archiving modes that can be activated with the parameter (`[ALCIMSVR] / [BATCH_ARCHIVING_MODE]`).

-   **0** = previous behavior, status must be set manually to 2000
-   **1** = batches with the status 700 (produced) or higher are archived
-   **2** = batches with the status 800 (packed) or higher are archived
-   **3** = batches with the status 900 (delivered) or higher are archived

The batch statuses 700 – 900 are set automatically by AlcimBooking based on pool_bearbeit.final_kz:
-   All header parts in the batch with `pool_bearbeit.Final_KZ = 1` -> 700 produced-> `pool_teile.bdefertig > 0`
-   All header parts in the batch with `pool_bearbeit.Final_KZ = 2` -> 800 packed -> `pool_teile.bde_verpackt > 0`
-   All header parts in the batch with `pool_bearbeit.Final_KZ = 3` -> 900 delivered -> `pool_teile.bde_versendet > 0`

> **CAUTION:** If one of the new Archivierunsmodi (1, 2 or 3) is used, it is necessary that the delay of the archiving be set to at least one day in order to prevent immediate archiving (e.g. in order to book breaks after the fact). For security reasons, therefore, always use one day delay as soon as BATCH_ARCHIVING_MODE > 0 and DELETIONDELAY < 1.

**Booking discipline**

The automatic archiving is based on PDC bookings and therefore depends on the booking discipline. As soon as a header part in a batch does not reach the appropriate status, the batch status cannot be set and thus the automatic archiving is initiated. Therefore, attention has to be paid that especially the header parts are booked completely.

AlcimBooking takes care of forgotten bookings for subparts as well as it can automatically. This is controlled via the fields "bdefertig“, "bde_verpackt" and "bde_versendet“ in the table "pool_teile." Each of these fields can assume the following values:

-   **0** = not yet complete
-   **1** = PO quantity was reached
-   **2** = PO quantity plus the surplus (=maximum quantity) was reached

If you are working without surplus, the value changes directly from 0 to 2 as soon as all lites are in the appropriate condition (available, packed or sent).

As soon as all header parts are booked packed (that is, all processing on the header parts with `pool_bearbeit.Final_KZ = 2` were booked), `pool_teile.bde_verpackt` is 1 or 2 and AlcimBooking ensures that this value is also inherited by all subparts. This achieves the following:

a)  Forgotten bookings on subparts are "corrected"
b)  Batches that only include subparts or subparts whose header parts are in other batches can nevertheless receive a status for automatic archiving

Essentially it applies that: a complete archiving of a batch can only be done when dependent batches (which contain common order items) are also in this status. Since you can never assume 100% booking reliability, you can support customers with helpful views or reports.

### 14.3. Expanded automatic archiving

A new configuration switch **"Archiving method"** has been introduced in order to switch between the old archiving method (which is set and used by default) and the new "expanded" method, which is less restrictive and allows the archiving and releasing of more batches.

-   **0 = Standard archiving method**
-   **1 = expanded checking of the batches.** Here additional flags of the orders are considered in a batch in order to check whether an order can be archived. This method is less restrictive than the standard method.

The parameter **"BATCH_ARCHIVING_MODE"** tells the AlcimServer starting with which status a batch should be regarded as "ready for archiving". The value of "Automatic batch archiving" can be 1=Status 700 (produced), 2=Status 800 (packed), 3=Status 900 (delivered) or 0=Status 2000 (set manually as archivable).

#### 14.3.1. How "standard method" works

Example for batch 1000, whose status is set to 900 and the configuration parameter "archivable status" is set to 3 (status 900, delivered).

| Batch | Status | Orders | | Batch | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1000 | 900 | -> 2000001 | -> | 1001 | 900 |
| | | | | 1002 | 700 |
| | | 2000002 | -> | 1001 | 900 |
| | | | | 1003 | 2000 |

If AlcimServer processes the batch 1000 [column A] with a status equal to or greater than "archivable status" (900 in the example), it checks all orders of the batch 1000 [column D] and then checks in which other batches contained [column F] and whether they all have a status equal to or greater than "archivable status".

In this example, the order 2000001 cannot be archived because there is another batch 1002 that also contains this order and this batch only has the status 700. Since this is less than "archivable status," batch 1000 cannot be archived.

#### 14.3.2. How "expanded method" works

The new method was invented in order to be able to archive more batches.

The new method enables the archiving of orders that can be regarded as completed, even if they are included in another batch with a status less than "archivable status" but with a status equal to or greater than 700 (= produced).

Example: batch 1000 has the status 900 and the parameter "archivable status" is set to 3 (900, delivered).

| Lauf | Status | | AuftNr | -> | Lauf | Status | -> | pos | teile_nr | bdefertig | bde_verpackt | bde_versendet |
| :--- | :--- | :- | :--- | :- | :--- | :--- | :- | :-- | :--- | :--- | :--- | :--- |
| 1000 | 900 | -> | 2000001 | -> | 1001 | 900 | -> | 1 | 0 | 2 | 1 | 1 |
| | | | | | | | | 1 | 1000000 | 2 | 1 | 1 |
| | | | | | | | | 1 | 2000000 | 2 | 1 | 1 |
| | | | | | | | | 2 | 0 | 2 | 1 | 1 |
| | | | | | | | | 2 | 1000000 | 2 | 1 | 1 |
| | | | | | | | | 2 | 2000000 | 2 | 1 | 1 |
| | | | | -> | 1002 | 700 | -> | 3 | 0 | 2 | 0 | 0 |
| | | | | | | | | 3 | 1000000 | 2 | 0 | 0 |
| | | | | | | | | 3 | 2000000 | 2 | 0 | 0 |
| | | -> | 2000002 | -> | 1001 | 900 | | | | | | |
| | | | | | 1003 | 2000 | | | | | | |

If the status of the batch is 700 or larger and smaller than "archivable status," then other data records from `pool_teile` and `pool_auftrag` also have to be analyzed.

Part of an order 2000001 [column D], which is included in the batch 1001 [batch F] does not have to be analyzed since the status [column G] of this batch is equal than or greater to "archivable status".

But another part of the order 2000001 [column D] that is included in the batch 1002 [column F] has to be analyzed because the status [column G] of this batch is 700 or greater and less than "archivable status".

The condition that this part of the order 2000001 [column D] counts as archivable is that all `pool_teile` data records for the specified batch and given order have set at least one of `bdefertig` | `bde_verpack` | `bde_versendet` flags [columns K,L,M] to a value not equal to zero or that the `auftkz` value of the `pool_auftrag` has to be greater than zero (canceled).

As you can see in comparison to the standard method, the new method considers the order 2000001 [column D] as archivable and thus the batch 1000 can be archived.

### 14.4. Archiving via customizing

With customizing, orders can be marked in the database as archivable. The booking service checks the status of all batches that are at least released once a day at 12:00 AM. Here the batch status is increased if this is possible. If, for example, a batch contains an archivable order that is not dispatched and a dispatched order, the batch status is set to dispatched (900). The check by the booking service is only done if the automatic archiving is configured by the AlcimServer. Thus, the batch is archived, even if not all orders are booked accordingly.

The archiving of orders can be identified via a customizing in that you enter a value > 0 in the `pool_auftrag.force`.

### 14.5. How is archiving done?

By default, archiving is done year by year, one archive database per year. The year in question and the associated archive database is determined with the following stored procedures. If these are changed, the default behavior can be changed, but this is not recommended.

-   `cu_alcsv_arcord` (archiving of the orders)
-   `cu_alcsv_arcsched` (archiving of the batches)
-   `cu_alcsv_arcopt` (archiving of the PMO data)

An order is only archived if all items of this order are completely planned in archivable batches. If this is not the case, the batch remains with the status "in archiving" (2001) until the condition is fulfilled and the batch can be archived completely.

In addition to the manual possibilities for archiving a batch, there is also the archiving pot 12600. Cancelled orders are shifted to it and archived automatically by the ALCIMServer service.

The archiving of batches marked for archiving starts X days after marking. The time in days can be configured with the switch `[ALCIM_SETTINGS / DELETIONDELAY]`. If the switch is set to the value 0, the archiving begins immediately. The day of marking comes with the time stamp `POOL_LAUF.LASTMODZEIT`.

*Figure 14-5 Configuration of deletion delay*

### 14.6. Archive databases

Archive databases have the same data structure as the production database. On first access by the ALCIMServer service, it adds the field XXXARCTIME to each table.

For an update of the structure of the production database, the structure of all archive databases must also be updated accordingly.

To generate a new, empty archive database, the data structure of the production database must be backed up. A new archive database is created and this data structured loaded. The data structure may not include any TRIGGERs; functions, stored procedures, and VIEWs are not required. Required are the indexes of the tables.

After the structure is loaded, a data record with the version of the data structure must be entered in the PARAMETER table. This data record can be unloaded from the production database and loaded into the archive database or you can add it directly to the archive database with INSERT:

**INFORMIX:**
```sql
INSERT INTO parameter (lastmodstation, lastmodzeit, bereich, eintrag, nummer, typ, text) 
VALUES ('INIT', TODAY, 'DATENBANK', 'ALCIM',0,1,'<DB Version>');
```

**SQLServer:**
```sql
INSERT INTO parameter (lastmodstation, lastmodzeit, bereich, eintrag, nummer, typ, text) 
VALUES ('INIT', CURRENT_TIMESTAMP,'DATENBANK','ALCIM',0,1,'<DB Version>');
```

**INFORMIX (Windows)**

To be executed on the database server in the DOS boxes of the environment. It may be necessary to adjust the commands to the environment in question.

**Load data from production database:**
```bash
DBSCHEMA -d alcimdb C:\Temp\dbschema.sql

ECHO unload to 'c:\Temp\parameter.uld' select * from "alcimdb".parameter WHERE eintrag = "ALCIM" AND bereich = "DATENBANK" | dbaccess alcimdb
```

**Generate archive database:**
```bash
ECHO create database alcimqry2019 in alcimqry with buffered log | dbaccess

DBACCESS alcimqry2019 C:\Temp\dbschema.sql

ECHO load from 'c:\Temp\parameter.uld' insert into "alcimdb".parameter | dbaccess alcimqry2019

LOMOSET -isvalcimqry -dbnalcimqry2019
```

**SQLServer**

With the SQLServer Management Studio, the structure can be created with the script wizard in a SQL file (Select database → Tasks → Generate Scripts...). Select all tables and activate the option that indexes should be taken along.

Then execute script generated on a generated archive database and then transfer the version to the parameter table.
```sql
USE alcimqry2019
INSERT INTO parameter SELECT * FROM alcimdb..parameter WHERE bereich='DATENBANK' AND eintrag='ALCIM'
```

### 14.7. Tables used

The ALCIMServer service analyzes the tables to be archived dynamically. Thus it is possible to create customer-specific tables and also to have them processed by the archiving. Of course these tables also have to exist in the archive databases.

For the analysis of the tables, the ALCIMServer service proceeds in the following steps:

**Order tables**
The table is an order table if the following is fulfilled:
-   Table includes an `AUFTNR` column
-   Exceptions are tables...
    -   `AWBAR_CHARGE`, `ERP_RUECKMELDUNG`, `AWINFO_TEMP_ORDER`
    -   whose names begin with `BDESTAT_`

**Batch tables**
The table is a batch table if the following is fulfilled:
-   Table contains a `LAUF`, `JOB` or `JOBID` column
-   Table includes no `AUFTNR` column
-   Exceptions are tables...
    -   `XOPT_STATISTIK`, `XOPT_STATISTIK_JUMBO`, `CU_IP_STATISTIK_KOPF`, `CU_IP_STATISTIK_PROD`
    -   whose names begin with `BDESTAT_`

**PMO tables**
The table is a PMO table if the following is fulfilled:
-   Table includes an `OPTI_ID` column
-   Table name begins with `PMO_`
-   Exception is the table `PMO_ITEMS`

### 14.8. Archiving the SKIZZEN table

The SKIZZEN table contains images of the individual lites. Data from this table is archived if the time stamp of the data records is older than a configured number of days. This is controlled via the configuration file LABELPRINT.INI. Also controlled via this configuration is that you should not delete the image files. These exist in addition to the SN drawings and are copied into the SKIZZEN table with the batch release. The JPG files are deleted by the archiving on the ALCIMServer. If the SKIZZEN of a batch are deleted although lists with sketches should be printed again, these can be copied again into the SKIZZEN table by repeating the sketch generation in the batch release.

```ini
[ALCIM_Skizzen]
CleanRecordsAfterDays=5
DoNotDeleteAlcimSNDrawFiles=Yes
DoNotDeleteAlcimSNDrawFilesAtAll=Yes
```

The switches `ACCESS_DSN` and `CompactDatabase` have no more significance; they come from the times when sketches were saved in an individual Access database.

## 15. A+W IoT Smart Trace

### 15.1. Basic configuration

#### 15.1.1. Gateway connection settings

So that data and documents can be sent via the gateway service to external systems such as Actiware, connection points are configured under A+W Infrastructure Web.

For this, start the web interface of the Infrastructure Services using the following URL:
`http://servername/infrastructure.web`
or open via the A+W folder on the desktop. Now select the configuration dialog.

*Figure 15-1 Infrastructure Web start page*

Now enter the gateway connection settings under the Gateway point:

*Figure 15-2 Configuration of the gateway connection settings*

**Gateway Verbindungseinstellungen**

| Setting | Value |
| :--- | :--- |
| Nutze verschlüsselte Verbindung (https) | OFF |
| Server Name | 192.168.206.7 |
| Port | 31003 |
| Update Pfad | /api/v1/process/awdemo/TERMINAL/collect/start |
| Benutzer | toso |
| Passwort | ****** |

In the current version of the Actiware modules, NO encrypted connection is possible; the switch must remain in the default value OFF. Similarly, neither user nor password is evaluated.

#### 15.1.2. PDC configuration

So that PDC data is sent to the gateway service, the master data in A+W Production must be adjusted as follows:

Via Master Data > Configuration, you can reach the Parameter Administrator. Search here in the barcoding booking service for "gateway" and set the switch Barcoding Statistics > External Barcoding Statistics to 1.

*Figure 15-3 Activating the PDC data transfer to the gateway service*

Setting this value causes the booking data to be written to the `awbar_gateway_data` table. It can then be forwarded by the gateway service to external services.

### 15.2. Sending reports

This function was previously realized for the A+W Production Terminal screens Order and xxx-Out.

If reports are printed in the production environment, for example from an A+W Production Terminal, it is possible to send these to external systems. For this, the following settings must be made:

-   Press [Ctrl] + [F12]
-   Insert an output field with the action `REGPOINTOUT`. For example, this field can be placed behind the SNLive view. This field is required so that the registration point number can be included with the report.
-   Open the script processing with the "Script and Reports" rubric
-   Set the "Archive report" switch to [True]
-   Confirm with OK

This configuration must be done per screen and then applies automatically to all reports.

## 16. Other functions

This section describes functions that cannot be assigned clearly to any other section.

### 16.1. Parameter Administrator

In A+W Production, the Parameter Administrator serves to make general and station-dependent settings in A+W Production. The Parameter Administrator can be reached in A+W Production via the menu Master Data → Configuration. From dialogs with Designer technology (A+W Production Terminal, release dialog, etc.), the Parameter Administrator can be reached with the key combination `<CTRL><F9>`.

When creating a new station in A+W Production, station parameters in the "General" area must always be present. In other areas, these are only necessary if the corresponding functions are used. For this reason, you can only enter new stations in this area. A station in A+W Production has a length of 2 digits or letters.

*Figure 16-1 Parameter Administrator: Creating a new station*

In other areas, you can only select a station that already exists under "General" from a list when creating a new station.

*Figure 16-2 Parameter Administrator: Transferring a new station*

The same behavior occurs if in an area you mark a station and want to copy it. Then in the "General" area you have the opportunity to enter a new station and in other areas the selection of a station already present in "General".

### 16.2. Document links

It is possible to attach external documents (e.g. a PDF) to an order or individual items of an order. These documents can be displayed and printed using various functions in A+W Production.

#### 16.2.1. A+W Production

Document links are stored in A+W Production in the database table `POOL_DOKUMENTE`. Documents that are assigned the item 0 apply for the entire order.

From the POOL views, document links can be managed with the [Belonging documents] context menu. Existing document links can be opened, deleted, created anew or edited.

*Figure 16-3 Management of document links*

| Order | Item | Type | Document |
| :--- | :--- | :--- | :--- |
| 700072 | 0 | 0 | `\\Sr-db01\trans\User_Manuals\US-ALCIM-UM-Complete-1.0.pdf` |
| 700072 | 1 | 5 | `\\Sr-db01\trans\User_Manuals\US-ALCIM-UM-Informix.pdf` |
| 700072 | 1 | | |
| 700072 | 2 | | |
| 700072 | 3 | | |
| 700072 | 4 | | |
| 700072 | 5 | | |

With batch release, there is a function for printing the document links of a batch.

*Figure 16-4 Print document links on release*

By default, this prints all documents of an item for all end products found in the batch. If an item is split into several batches, the documents are only printed in the batch where the end product is located. Order-related documents are not printed.

Printing is controlled by the script `DocumentLink.vb`. Customer-specific adjustments incur costs; for this, a copy of the file with the customer abbreviation must be created.

> **Caution:** Opening is only possible if there is a link to the Doculink from the A+W Production station (ideally always use the UNC path) and the file format can be started by an application linked in Windows.

#### 16.2.2. A+W Production Terminal

In A+W Production Terminal, the link is displayed in the element "Linkeddocuments":

*Figure 16-5 Document links in A+W Production Terminal*

This element is available on all screens. The links displayed can be filtered for each screen using a parameter via the type The link.

*Figure 16-6 Switch filter document links in A+W Production Terminal*
To filter documents, use the parameter `PRODTVDOCUMENTTYPES` in the `@PROPERTY_LOGICAL` area. This is a list of document types from the `POOL_DOKUMENTE` table to be displayed. If nothing is specified, all document types are shown.

> **Caution:** Opening is only possible if the WebService can establish a link to the Doculink (ideally always use the UNC path) and the file format can be started by an application linked in Windows to the A+W Production Terminal Client.

#### 16.2.3. Entry in A+W Business

In the document entry, item entry, and in the product, customer, supplier, and partner master data, there is a storage possibility for any file attachments, e.g. Word files, Excel files, JPEGs, and e-mails. These are simply saved in the corresponding field via the usual Windows drag & drop function. Here it is also possible to copy elements from Outlook, Outlook Express, and Windows Live Mail directly via drag & drop. Supported are mails, contacts, attachments, and calendar entries.

*Figure 16-7 File attachment in A+W Business*

A+W Business copies the files into a directory stored in the company master data (Master Data > Company Data > 4. Documents):

*Figure 16-8 Configuration directory for file attachment in A+W Business*
The path is configured as: `\\10.4.9.11\ERP-attachment\AWB\`

The directory stored there is completed with the document type, document number and (if applicable) item number or master data type, and is saved. Only the relative path is saved in the database.

*Figure 16-9 Directory for file attachment in A+W Business*

Click on such an attached file in A+W Business to start the corresponding application, and to open the document linked to the file type.

All file attachments can be grouped by type now. This helps to control which file attachments will be taken over for the transfer to production (OrderXML), copying quotations into orders, and PO transfer (e.g. product information) and which shall not (e.g. calculation information).

*Figure 16-10 Types for file attachment in A+W Business*

For the setup, the required attachment types have to be defined in text master data (Master Data > Text > File Attachment Types) before they are activated in the settings dialogs for transfer to production (Production > Production > Production Transfer > Function Settings), Copy documents (Documents > Quote > Quote NM > Copy Documents), and PO transfer (Documents > Order > P.O. transfer).

*Figure 16-11 Configuration transfer file attachment from A+W Business*

By default, all attachments are initialized with type A (all) and will always be transferred (exception: PO transfer).

**File attachments in the document order entry**

Essentially, an attachment can only be assigned to a document if the document has already received a valid document number.

In item entry, an attachment is visualized with an appropriate icon.

*Figure 16-12 File attachment in item entry in A+W Business*

In the document view, the document links can also be displayed on an individual tab. This is possible even for archived documents.

*Figure 16-13 File attachment in document view in A+W Business*

When importing orders via EDI interface (Documents > Order > Import), document attachments can also be imported. These are pre-populated with the document link type A.

When you copy documents, only the file reference will be copied, not the file itself. When you enter series at item entry, the annexed file will not be kept.

During the saving of items as macros, existing document links are also saved.

An overview of the attachments to the product is found on the item info dialog on tab 3. Attachments, from which they can be opened with a double-click. Thus, this data can be accessed quickly at any time in the document entry.

**Affected database tables**

File attachments in A+W Business databases are saved in the following tables:

| Table Name | Description |
| :--- | :--- |
| KA_ATT_TYPE | File attachment types |
| BA_MAKRO_ATT_POS | File attachments for macros |
| BW_ANFR_ATT_KOPF | Inquiry file attachment header |
| BW_ANFR_ATT_POS | Inquiry file attachment items |
| BW_ANGEB_ATT_KOPF | Quotation file attachment header |
| BW_ANGEB_ATT_POS | Quotation file attachment items |
| BW_AUFTR_ATT_KOPF | Order file attachment header |
| BW_AUFTR_ATT_POS | Order file attachment items |
| BW_GUTSCH_ATT_KOPF | Credit note file attachment header |
| BW_GUTSCH_ATT_POS | Credit note file attachment items |
| BW_BEST_ATT_KOPF | Purchase order file attachment header |
| BW_BEST_ATT_POS | Purchase order file attachment items |
| BA_PRODUKTE_ATTACH | File attachment for products |
| KU_ATTACH | File attachment for customers |
| LI_ATTACH | File attachment for suppliers |
| PA_ATTACH | File attachment for partners |
| FS_ATT_KOPF | File attachment on header level from external interface |
| FS_ATT_POS | File attachment on item level from external interface |

## 17. Production Monitor

### 17.1. Overview

*Figure 17-1 Production Monitor*

The Production Monitor provides a visual overview of production resources and their status over several days.

**Legend:**
-   **Green circle:** No backlogs
-   **Yellow circle:** Backlogs, but you can finish them today
-   **Red circle:** Backlogs, and it is not possible to finish them today
-   **X:** Closed shift
-   **White bar:** Free capacity
-   **Striped bar:** Reduced shift
-   **Green bar in shift:** Already done

A tooltip provides detailed shift information, such as start/end times, load, completion time, and reservations.

### 17.2. Detail view

With the icon (upper left corner of the Production Monitor), you can switch to a detailed view for a day. Here, the various planning states of the orders are depicted with different colors:

-   **Yellow:** In the pool
-   **Blue:** Rough and detailed scheduling
-   **Green:** Released

*Figure 17-2 Tooltip display in Production Monitor*
The tooltip in this display indicates the precise data for a shift, including load times, production release, and planned durations.

### 17.3. Backlogs and workload

#### 17.3.1. Display

Backlogs are displayed when you move the mouse over a traffic light display:

*Figure 17-3 Display of backlogs*

Here, all lites are regarded that must still be produced in the period Today-30 days - until today (incl. - changed starting with 5.3; see below)(and are not yet finished).

If only values (that is, no times) will be displayed for the backlogs (see figure), then no specified times are stored for this machine.

The data displayed (status A+W Production 5.1) will be determined with the following SQL (SQL Server):
```sql
SELECT
    SUM((pt.menge_nach - pt.mindermenge_nach) * pb.dauer) AS backorderAmount,
    SUM(pb.dauer * (CASE pb.menge WHEN 0 THEN pt.menge
        ELSE pb.menge_gut/pb.menge END)) AS backorderAmountDone,
    SUM((pt.menge_nach - pt.mindermenge_nach)) AS backorderCount,
    SUM(CASE pb.menge WHEN 0 THEN pt.menge
        ELSE pb.menge_gut/pb.menge END) AS backorderCount Done
FROM pool_bearbeit pb, pool_teile pt, pool_pos pp
WHERE pb.auftnr = pt.auftnr
    AND pb.pos = pt.pos
    AND pb.u_pos = pt.u_pos
    AND pb.teile_nr = pt.teile_nr
    AND pb.prod_term >= convert(date, dateadd(d,-30, getdate()))
    AND pb.prod_term < cast(getdate() as date)
    AND pb.auftnr = pp.auftnr
    AND pb.pos = pp.pos
    AND pb.u_pos = pp.u_pos
    AND pp.auftkz = 0
    AND pb.mzo_id_phys = 110
```
Starting with Version 5.3, the new fields from `pool_bearbeit` are used.

You can reach the backlog display by clicking the right mouse button on the traffic light symbol and selecting "Display backlog".

In the following display, 2 filters should be set:
-   **"Max backlogs (-30)"**: `cast(pool_bearbeit.prod_term as date) >= convert(date, dateadd(d,?, getdate()))` with a standard parameter of -30 filters the backlogs to a maximum of 30 days in the past. Without this filter, all backlogs are drawn from the database.
-   **"Only production orders"**: `POOL_POS.AUFTKZ<>90 and POOL_AUFTRAG.AUFTKZ<>90` filters out the quotation orders.

This display also displays the backlogs starting 30 days in the past, however **WITHOUT** today.

The weight should be calculated in the work plan from `pool_teile.flaeche * pool_teile.dicke / 1000 * 2,5 * pool_bearbeit.menge_prod`. Then the data will match the figures from the Production Monitor. For insulated glass, this does not hold true, but there a display in weight makes no sense.

`Pool_teile.flaeche` is important in this formula since this way, shapes are also taken into account. `Pool_bearbeit.menge_prod` is important since with it, cancellations are displayed correctly (in case of cancellation, reduces in contrast to pool_teile.menge).

#### 17.3.2. Workload

You can display the workload of a shift by moving the mouse over a shift in the Production Monitor:

*Figure 17-4 Utilization of a shift*

The data for this is gathered with the following SQL. Starting with Version 5.3, the new fields from `pool_bearbeit` are also used:
```sql
SELECT
    pb.prod_term AS prod_term,
    pb.schicht AS schicht,
    pb.mzo_id_phys AS mzo_id_phys,
    pb.mzo_technologie1 AS mzo_technologie1,
    COUNT(*) AS rcount,
    SUM(pb.dauer * (CASE pb.menge_prod WHEN 0 THEN pt.menge 
        ELSE pb.menge_prod END)) AS wload,
    SUM(pb.dauer * (CASE WHEN pb.menge = 0 THEN pb.menge
        WHEN pb.menge_prod = 0 THEN (pb.menge_gut/pb.menge)
        WHEN pb.menge_gut > pb.menge_prod THEN (pb.menge_prod/pb.menge)
        ELSE (pb.menge_gut/pb.menge) END)) AS wloaddone,
    SUM(CASE WHEN pb.menge = 0 THEN pb.menge
        WHEN pb.menge_prod = 0 THEN (pb.menge_gut/pb.menge)
        WHEN pb.menge_gut > pb.menge_prod THEN (pb.menge_prod/pb.menge)
        ELSE (pb.menge_gut/pb.menge) END) AS wdone,
    SUM(CASE pb.menge_prod WHEN 0 THEN pt.menge ELSE pb.menge_prod END) AS squantity,
    MAX(pb.sequenz) AS maxSequenz,
    pt.status AS pt_status
FROM pool_teile pt, pool_bearbeit pb, pool_pos pp
WHERE pb.prod_term >= @start_prod_term
    AND pb.prod_term <= @end_prod_term
    AND pb.mzo_id_phys IN (110,120,130)
    AND pt.auftnr = pb.auftnr
    AND pt.pos = pb.pos
    AND pt.u_pos = pb.u_pos
    AND pt.teile_nr = pb.teile_nr
    AND pt.auftnr = pp.auftnr
    AND pt.pos = pp.pos
    AND pt.u_pos = pp.u_pos
    AND pp.auftkz = 0
GROUP BY pb.prod_term, pb.schicht, pb.mzo_id_phys, pb.mzo_technologie1, pt.status
```

#### 17.3.3. Known problems (in A+W Production 5.1/5.2):

-   Tooltip of the backlogs takes today into account, the display does not → #286367 (eliminated in 5.3 or with Hotfix „0_A+W Production 5_1976.zip")
-   Tooltip for the backlogs and work plan do not consider PDC cancellations (that is, still occupy the capacity) → #286365 (eliminated in 5.3 or with Hotfix „0_A+W Production 5_2113.zip")
-   No PDC tables should be used in the workplan. Here, please use only the pool tables since otherwise there will be undesired effects: a) the "figures" will not be correct b) for quotation orders, no data will be displayed (since not PDC-initialized)

### 17.4. Manual completion notification

Backlogs cannot be reported completed directly from the workplan.

#### 17.4.1. The process

For this, you select a machine/shift from which the lites should be reported completed:

*Figure 17-5 Display in the Production Monitor*

Then you open the workplan (double-click or right mouse-click). Here, you then mark the orders/processings that should be reported completed and select the "Report completed" option on the context menu:

*Figure 17-6 Batch overview*

After that, another confirmation message appears:

*Figure 17-7 Program message*

> Bei einer manuellen Fertigmeldung werden alle unterliegenden Bearbeitungen mit gebucht.
> Wollen Sie die ausgewählte Bearbeitung sowie alle darunterliegenden Bearbeitungen wirklich fertig melden?
> (With a manual completion notification, all underlying processings will be booked. Do you really want to report the selected processing and all underlying processings as completed?)

and here we go. That is, all lites from the selection (with their components that you have searched for) and are booked to the planned `esnr_soll`.

#### 17.4.2. Limitations

-   The lites will be booked normally. That is, also in `awbar_teile`, they are suddenly on a registration point where they never were before.
-   In `awbar_teile`, you cannot detect that this is a manual booking (except that no person is specified; in `awbar_booking`, the station is "DEBKMO"). That is, the statistics are "mucked up" and you must take this into account. Therefore, should only be used only in case of emergency and if you are sure that the lites are truly complete.
-   the subparts are not "married". That is, you do not see which subparts are installed in a header part. The defect management then does not work with such parts!
-   in the MZO and in the column assignments, the same registration points must be used. That is, if the MZO calculate an ESNR-target 1610 and the ESNR 1612 is responsible in the column assignment for the processing booking, the lites are booked to the 1610, but they do not disappear from the backlog list!

#### 17.4.3. Known Problems

For the booking, broken lites are also written to `awbar_booking`, which causes error messages in the PDC post-processing → 286361: is solved with Hotfix 0_A+W Production 5_1791.zip.

## 18. Table of Figures

-   Figure 1-1 Parameter administrator: specification of the sequences in O4P
-   Figure 1-2 Parameter administrator: Specification of the sequences in O4P - example of Resolve MacroProcessing.
-   Figure 1-3: ALLOW_LATE_POSTPONE_TO_PAST
-   Figure 1-4: IGNORE_TEXTCHANGES_IN_LATEORDERCHANGE
-   Figure 1-5: IGNORE_COMISSION_CHANGES.
-   Figure 1-6: CHANGE_POS_LIEFTERM
-   Figure 2-1 Pool display - selected filters
-   Figure 2-2 Field definition of the rough scheduling for fields from a VIEW.
-   Figure 3-1 ProcessManagerControl...
-   Figure 3-2 Parameter group
-   Figure 3-3 Parameter leading group
-   Figure 3-4 Configuration of report mode INTERNAL.
-   Figure 3-5 Parameters PDF output directory
-   Figure 3-6 Parameter [POOL_SETTINGS / SCHEDULE_RELEASE_STORNO].
-   Figure 4-1 Parameter administrator: specification of the version of the Crystal Report runtime
-   Figure 4-2 Crystal Report Designer - Parameter field dialog
-   Figure 4-3 Example of true to scale sketch
-   Figure 4-4 Switch [ITEMS4ALCIM_SPECIALS / CREATE_SN_FILE_BY_ORDERXML]
-   Figure 4-5 Switch [POOL_SN / DATAFILEPATH]
-   Figure 4-6 Switch [ALCIM_SHAPE / SNCUTASSTANDARDFRM]
-   Figure 4-7 Switch [ALCIM_SN / SKETCHPRINTINGVIEWS]
-   Figure 4-8 Sketch configuration dialog
-   Figure 4-9 Switch [ALCIM_BDESETTINGS / DELETE_SN_FILES]
-   Figure 4-10 Sketch with profile
-   Figure 4-11 Switch [ALCIM_SHAPE / SN_FLIPMODE].
-   Figure 4-12 AWPLogoTableEditor
-   Figure 4-13 AWPLogoTableEditor - configuration of database.
-   Figure 4-14 AWPLogoTableEditor – Trace display
-   Figure 4-15 AWPLogoTableEditor - adding a logo..
-   Figure 4-16 AWPLogoTableEditor – image file selection
-   Figure 4-17 AWPLogoTableEditor - editing a logo......
-   Figure 4-18 AWPLogoTableEditor – deleting a logo.
-   Figure 4-19 AWPLogoTableEditor – saving a logo...
-   Figure 6-1 Reporting process
-   Figure 6-2- Switch [ALCIM_STATE / ERPFEEDBACK]
-   Figure 6-3 Parameter Status Registrations
-   Figure 6-4 Switch [ALCIM_STATE / ERP_DETAILED_FEEDBACK]
-   Figure 6-5 Master data registration point for processing reporting.
-   Figure 6-6 Switch rack feedbacks
-   Figure 6-7 Master data Registration point for rack feedback.
-   Figure 6-8 Switch [ALCIMBOOK / TABLEIDSXOPTFEEDBACK]
-   Figure 6-9 A+W Business Feedback Process
-   Figure 6-10 A+W Business Configuration Feedback
-   Figure 6-11 A+W Business Open production overview..
-   Figure 6-12 A+W Business Old production overview..
-   Figure 6-13 A+W Business Production overview based on a report.
-   Figure 6-14 A+W Business Configuration Production overview based on a report.
-   Figure 6-15 A+W Business classic product overview
-   Figure 6-16 A+W Business view delivered racks
-   Figure 6-17 A+W Enterprise feedback process
-   Figure 6-18 A+W Cantor feedback process.
-   Figure 6-19 A+W Cantor configuration feedback directory.
-   Figure 6-20 A+W Cantor configuration system queue...
-   Figure 6-21 A+W Cantor configuration part additions..
-   Figure 6-22 A+W Cantor configuration terminal group
-   Figure 6-23 A+W Cantor rack group designer
-   Figure 6-24 A+W Cantor rack group result.
-   Figure 6-25 A+W Production parameter for A+W Cantor rack feedback
-   Figure 8-1 Connection data of the e-mail server
-   Figure 8-2 Configuration of the booking service for e-mail dispatch and background printing
-   Figure 8-3 Parameter configuration in Crystal Reports
-   Figure 8-4 DB table awbar_barcodetypen
-   Figure 8-5 CIM Server Settings
-   Figure 8-6 Regex configuration
-   Figure 8-7 Regex adapted
-   Figure 8-8 Uploading the new configuration
-   Figure 8-9 New configuration....
-   Figure 10-1 Parameter Administrator with parameter "Use dialog QA".
-   Figure 10-2 Global formatting.
-   Figure 10-3 Formatting of data columns...
-   Figure 10-4 Configuration of synchronous booking..
-   Figure 10-5 Configuration of the rack comparison with the A+W Rack Manager
-   Figure 10-6 - Keyboard scanner parameters..
-   Figure 10-7 - Scanner ID
-   Figure 10-8 Furnace bed
-   Figure 10-9 Action for the foil preview
-   Figure 10-10 SQL expression for the foil preview
-   Figure 10-11 Parameter Administrator with parameter "Automatic Batch Creation"
-   Figure 10-12 Configuration for provision of PMO data.
-   Figure 10-13 Configuration for transfer of PMO data via XML file
-   Figure 10-14 Parameters for quality scanner.
-   Figure 10-15 Parameters for quality scanner..
-   Figure 10-16 Parameters for individual lite booking.
-   Figure 10-17 Parameter Administrator with dialog selection for racks that can be called up
-   Figure 10-18 Select lot types
-   Figure 10-19 Parameter Administrator for the filter possibility by cutting tables.
-   Figure 10-20 Configuration of tables for filter selection.
-   Figure 10-21 Designer with new action button [Racks that can be called up]
-   Figure 10-22 selection of a fine planning rack
-   Figure 10-23 Dialog for loading a lot
-   Figure 10-24 SN driver call
-   Figure 13-1 Multisite infrastructure.
-   Figure 13-2 Infrastructure configuration sites
-   Figure 13-3 Infrastructure site assignment.
-   Figure 13:4 Infrastructure configuration...
-   Figure 13-5 Infrastructure A+W Production configuration
-   Figure 13-6 Infrastructure A+W Production configuration basic settings
-   Figure 13-7 Infrastructure A+W Production configuration database connection
-   Figure 13-8 Infrastructure A+W Production configuration PPS WebService URL.
-   Figure 13-9 Infrastructure A+W Production configuration Service Monitor
-   Figure 13-10 A+W Production MultiSite CONFIG Tool.......
-   Figure 13-11 A+W Production MultiSite CONFIG tool services.
-   Figure 13-12 A+W Production MultiSite CONFIG tool services.
-   Figure 13-13 Services according to A+W Production MultiSite CONFIG tool
-   Figure 13-14 A+W Production site selection....
-   Figure 13-15 A+W Production Terminal selection of PPSWebService..
-   Figure 14-1 Archiving a batch in A+W Production
-   Figure 14-2 Archiving or deleting configuration batches.
-   Figure 14-3 Configuration of DSN for archive database
-   Figure 14-4 Configuration deletion of files during archiving
-   Figure 14-5 Configuration of deletion delay
-   Figure 15-1 Infrastructure Web start page
-   Figure 15-2 Configuration of the gateway connection settings.
-   Figure 15-3 Activating the PDC data transfer to the gateway service
-   Figure 16-1 Parameter Administrator: Creating a new station.
-   Figure 16-2 Parameter Administrator: Transferring a new station
-   Figure 16-3 Management of document links..
-   Figure 16-4 Print document links on release
-   Figure 16-5 Document links in A+W Production Terminal.
-   Figure 16-6 Switch filter document links in A+W Production Terminal
-   Figure 16-7 File attachment in A+W Business...
-   Figure 16-8 Configuration directory for file attachment in A+W Business.
-   Figure 16-9 Directory for file attachment in A+W Business.
-   Figure 16-10 Types for file attachment in A+W Business
-   Figure 16-11 Configuration transfer file attachment from A+W Business
-   Figure 16-12 File attachment in item entry in A+W Business.
-   Figure 16-13 File attachment in document view in A+W Business
-   Figure 17-1 Production Monitor
-   Figure 17-2 Tooltip display in Production Monitor
-   Figure 17-3 Display of backlogs.
-   Figure 17-4 Utilization of a shift ....
-   Figure 17-5 Display in the Production Monitor.
-   Figure 17-6 Batch overview.
-   Figure 17-7 Program message...

