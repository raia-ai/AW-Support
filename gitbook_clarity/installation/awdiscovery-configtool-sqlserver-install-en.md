---
description: "EN-INST-AW_Discovery"
---


# Description of the Config Tool: A+W Discovery

---
## Change history

| Date       | Edited by | Remarks         | Version |
| :--------- | :-------- | :-------------- | :------ |
| 2013-08-16 | MISC      | Initial version | 1.0     |
| 2013-09-10 | RI        | Addition        | 1.1     |

## Content

1.  **Description**
    1.1. Configuring A+W Discovery
    1.2. Available parameters
2.  **Error handling**
    2.1. Configuration of the SQL Server services

## 1. Description

The following chapter discusses the working method of the A+W Discovery config tool and it explains the individual steps for configuring A+W Discovery successfully. Here, A+W Discovery assumes that an appropriate Microsoft SQL Server is installed on the target computer.

### 1.1. Configuring A+W Discovery

The A+W Discovery installation is handled by the A+W SetupLauncher. It ensures that all resources required by the config tool are installed on the target computer. After this has happened, the SetupLauncher starts the A+W Discovery config tool. The first interface that appears looks like this:

_Figure 1: Start dialog_

In the beginning, the user is asked to specify the instance of the local SQL Server. If only the standard instance (unnamed instance) of the SQL Server is on the computer, this field must remain empty. This is due to the fact that in the SQL Server, the standard instance is not addressed by its instance name.

> **Note:** Currently in the config tool there is **no** remote configuration supported, so that no host can be entered here. Furthermore, it must be noted that – if there are several SQL Server instances on the computer – the SQL Server browser must be started since otherwise no connection to an instance can be established.

In the second step, the entry of a user with administrative rights is requested. This user must be in the local administrator group of the computer. Furthermore, this update task also writes to the event log of the computer, which is only possible with such rights.

If you click "Next" on the following two pages, the config tool checks whether:
*   The specified user and password are correct and it is possible to log on with these.
*   The user is in the administrator group.
*   The instance can be found and a connection is possible.

All three points must be fulfilled so that you can move to the next page. Here, the following is displayed:

_Figure 2: Optional de-installation_

Now it is possible to remove an optional A+W Discovery installation. It must be mentioned that A+W Discovery is not a normal "installation" of a program; instead, it is more the case that only the services of the respective SQL Server must be configured appropriately. Since the set-up for this must recognize the instance of the SQL Server, it runs within the config tool.

A deinstallation checks and removes the following:
*   All SQL Server tasks that start the data import and all previously-required authorizations (log-ins, proxy, etc.).
*   The SQL Server databases (DWH and Import).
*   The SSIS packages within the integration services.
*   The cube within the analysis services.

Finally, the SQL Server is reset to its original state before installation.

Next you will see the installation dialog:

_Figure 3: Installation dialog_

As soon as this view appears, there is an automatic background check as to whether A+W Discovery is installed correctly or whether an update is required.

The update performs the following steps:
1.  The existing SSIS packages for the data import are updated.
2.  The existing cube is deleted and replaced with the current, empty cube. **Important:** all data previously in the cube is lost and therefore the cube must be processed anew. A complete new import of the data is not necessary since the DWH database is not deleted during an update.

In case of a first installation, the following steps are performed:
1.  The database login is generated (SQL user `"AWDiscovery_USR_SQL"` with the server roles `public` and `bulkadmin`).
2.  The DWH and import databases are generated and added to the SQL user.
3.  Generation of a credential and proxy with the administrative user specified on the first dialog window.
4.  Creation of the two SQLServerAgent tasks for the daily import of the data. The tasks are performed under the previously-created proxy.
5.  If necessary, deletion of an already-existing A+W Discovery cube.
6.  Generation of the cube.
7.  Initialization of the databases (with statistical data).
8.  Initialization of the SSIS packages.

Both for an update as well as for an installation, there is always a check in advance whether a connection to all services is possible and furthermore, whether these are configured correctly (start mode). Furthermore, the `"FILESTREAM"` option within the SQL Server is also read out and checked. If it is not active, this is indicated to the user in the config tool. During the installation in Figure 3, for example, you can see that the SQL ServerAgent is not configured appropriately. Here, however, the correct installation is not influenced. However the SQL ServerAgent must be configured manually after the fact since otherwise the future daily update cannot be performed successfully within the ServerAgent.

For the update task with the designation `"AWDiscovery_Update"` it must also be mentioned that by default, it is performed daily at 3:00 am. Here, the data import is started and then – if no errors occurred during the import – the cube is built up again with the updated data. At the beginning and during the individual steps, there is also writing to the event log. If, due to network problems or similar, the task must be shifted to another time, then this must be set manually in SQL Server Management Studio.

Furthermore, a second task called `"AWDiscovery_CleanLogAndUpdateDate"` is created, which cleans the internal data and keeps it consistent. This task is performed once on the last Sunday of the month at 10:00 pm. Here too, the manual time change applies.

After the installation of A+W Discovery has been performed successfully, on the following dialog window, the following must be edited:

_Figure 4: Global settings_

The parameters listed here are necessary in order to ensure the data flow in the import and DWH databases. However, most of these are already specified and cannot be edited. Both variables `Start year` and `Days in advance` serve the internal date creation. Here, it is necessary to ensure that the configured interval (`Start year` until today + `Days in advance`) always covers the time period that the connected sites manage. If, for example, a site should be added that contains older data than the `Start year`, the `Start year` must be set back. The year specification is sufficient here since the beginning is always 01/01 of the year. The variable `Days in advance` ensures that future data values are also present. This variable may not be less than 31. Recommended here is the value 365.

The (DWH) password can also be changed here that the `AWDiscovery_USR_SQL`-user should use to log on. By default, a default password is assigned here. After a password entry, there is a check to be sure the new password is valid and it does not violate any active password guideline. If this is the case, then this is indicated to the user with a warning messages on the lower part of the config tool. The SQL login applies for the DWH and import database. **Important:** if the password is changed after the fact, then you must ensure that change is also applied for already-existing sites.

After a valid password entry, it takes a little while until the config tool has made all necessary changes. Here, the following steps are performed:
1.  The SQL login is assigned the new password (continue only if successful).
2.  The new password is transferred internally to all SSIS packages.
3.  The new password is set in the cube.

After that, click "Next" to define the groups for sites that are created in the next step. However, this group definition is optional. For example, sites to be created here can be divided into regional groups or industries.

_Figure 5: Optional creation of groups_

After this step has been performed comes the actual creation of the various sites.

_Figure 6: Creation of sites_

Here, sites to be imported (Business, Enterprise, and Production) can be created with "Add." Editing, copying, and deletion is also possible. When copying it must be noted that all values – but for the ID – are taken over from the original site. The following dialog appears:

_Figure 7: Selection of the module type_

First you must select what the type of the new site to be created should be. After you have made a selection here, the type-specific, configurable parameters are loaded automatically.

_Add new Remote Database (Detailed View)_

There is a listing of these parameters in Chapter 1.2. Here, the point is to explain in brief which parameters must absolutely be set for a successful import. In the beginning, the user can set a different ID than the one automatically specified. This option makes sense if for a site with e.g. ID = 3 and type Production there is an additional type Enterprise. In this case, an additional Enterprise site with the same ID must be created. **But:** for one ID, the same type cannot be created several times.

Next comes the specification of the database parameters. Here there is a distinction among the various supported database types Informix, SQLBase, and SQLServer. Depending on the type specified, the corresponding fields are adjusted or set to non-editable. For Informix, it must also be mentioned that here, its internal configuration (by Informix's own program SetNet) is executed automatically. Thus the user does not have to perform any additional Informix configuration in advance. **But:** if the site to be created is a SQLBase database, then the SQLBase "Connectivity Administrator" must be called in advance and the database server defined. **Attention:** for SQLBase it must also be noted that all required databases must have different names since the databases are only addressed using these.

The correct entry of the database parameters in the config tool is indicated to the user after each editing and addition in the lower area with a connection test to the corresponding site.

Another mandatory entry is the selection of the import database. If the import should always be up to the current day, then for `"End date"` only `OFF` should be specified (by setting `disable` in the date field). Later on, this causes the import to always import up to the current day. The `start date` causes processes to be imported that were changed since `start date`. But not recorded earlier than `first date`. Generally the specification of the correct date format through the `"Date format"` variable must be heeded since especially with the Informix driver (under DBDate), a date format can be specified that is used in the end. The `"Import interval"` variable handles the import of larger quantities of data and can be used in such a case to set the number of days (value > 0) that should be imported in a run. If, for example, data should be imported over a period of 2 years data, the import can be divided up into intervals of 100 day-steps. For this, you must only enter the value 100 in the variable. Thus – starting from `start date` – the data is imported in 100-day steps.

**Important:** should the data for a site be imported in several import intervals, you must ensure that for this site there is one master data site (`RunLevel` on 1).

In the end, for the import of a site it should be mentioned that this is always attempted several times or three times e.g. in case of network problems. The number of failed attempts is always documented in the event log.

Next comes the `"General,"` section where a definition and so-called `RunLevel` are defined. The latter is significant if, for example, there is a master data site that contains only the global master data for all sites. Such a one must contain the `RunLevel` 1 so that it is imported first. After all sites have been imported completely with such a `RunLevel`, then the sites with `RunLevel` 2, 3, etc. follow. Here it is generally sufficient to leave all other sites at `RunLevel` 2. Here too, it should be mentioned again that only for sites with `RunLevel` 1 can an `ImportInterval` be set.

The `"Global"` rubric includes all parameters that are unique for a site. If for a site (ID) there should be several modules, then these parameters are the same for all modules and they are unique per site. Among other things, it is possible to specify an optional group from the previous dialog window here (if created). Important here, however, is the name of the site since it is used to create a corresponding local group on the computer and in the cube. The name of this group follows the following convention: `"AWDiscovery Site <ID> <Name of the site>."` If this name changes in a module, then the name is also changed for any other existing modules (with the same ID). The consequence of this is that the roles in the cube and in the Windows group are also renamed. By default, the role in the cube receives the limitation that only data for the respective site ID are visible and the corresponding, previously-created Windows group is assigned to it. Thus appropriate administrators can add the users (or groups) to the created Windows groups. The config tool creates **only** the corresponding groups.

The last category is the `"Master data,"` which is of special significance for customers with a central master data site. If, for example, there is a master data site with an ID = 1, then for the creation of another local site (ID = 2) there must be a reference to the first one:

_Figure 8: Configuration of master data_

Here, it can be specified individually for individual master data (item, models, etc.) where their reference should be sought. In the figure above, you can see that all master data refers to the master sites since all of these are set to its ID 1. If all master data is set to another ID, then the `"ImportMasterData"` option can be set to `false`. The effect of this is that no master data is imported for the current site.

The field `"House no."` serves the internal site capability of the individual modules. Thus, for example, Enterprise is in a position to manage several internal houses within a site. Such a constellation must be created within the config tool as follows:
*   Each internal house is created as an individual site (each has its own ID), whereby each site has its own module-specific house no.
    *   **And:** for the first site created, the `"ImportMasterData"` switch is set to `true` and for all others to `false`. Furthermore, for the latter the reference of the individual master data must be set to the ID of the first site created.

After these steps have been performed, a new site is successfully created and the configuration is complete.

Now end users can use Excel to access the cube and its contents. These A+W Discovery reports are in `...\A+W\A+W Discovery\Resources\Documents` and on first opening, the data connection must be adjusted to the cube, since here by default the correct connection character string is not defined.

### 1.2. Available parameters

Below is a list of all the parameters, only some of which may be edited by the user.

**Global Variables**

_Figure 9: Description of the available, global variables_

| Display name            | Description                                   | Category         | Default value                                             | Read only | Extended property |
| :---------------------- | :-------------------------------------------- | :--------------- | :-------------------------------------------------------- | :-------- | :---------------- |
| Max. Parallel Packages  | Count of concurrently running packages        | General          | 1                                                         | 1         | 1                 |
| Import Connection Appendix | Opt. Appendix for import connection           | Import Connection | `Persist Security Info=True;Auto Translate=False;`          | 1         | 1                 |
| Import DB Provider      | DB Provider for import Connection               | Import Connection | `Internal set`                                            | 1         | 1                 |
| Import Database         | Name of database for import                   | Import Connection | `AWDiscovery_Import`                                      | 1         | 0                 |
| Import Server Name      | Server (Host\Instance) for import             | Import Connection |                                                           | 1         | 0                 |
| Import Username         | Username for Import Connection                | Import Connection | `AWDiscovery_USR_SQL`                                     | 1         | 0                 |
| Import Password         | Password for Import Connection                | Import Connection | `AWdiscovery!`                                            | 1         | 0                 |
| DWH Connection Appendix | Opt. Appendix for DWH Connection              | DWH Connection   | `Persist Security Info=True;Auto Translate=False;`          | 1         | 1                 |
| DWH DB Provider         | Provider for DWH Connection                   | DWH Connection   | `Internal set`                                            | 1         | 1                 |
| DWH Database            | Name of database for DWH                      | DWH Connection   | `AWDiscovery`                                             | 1         | 0                 |
| DWH Server Name         | Server (Host\Instance) for DWH                | DWH Connection   |                                                           | 1         | 0                 |
| DWH Username            | Username for DWH Connection                   | DWH Connection   | `AWDiscovery_USR_SQL`                                     | 1         | 0                 |
| DWH Password            | Password for DWH Connection                   | DWH Connection   | `AWdiscovery!`                                            | 0         | 0                 |
| Installed Version       | AWDiscovery Version No.                       | General          |                                                           | 1         | 0                 |
| Language ID             | Language ID                                   | General          | 4                                                         | 1         | 1                 |
| Start year              | Start year for insert data stamp into db      | General          | 2008                                                      | 0         | 0                 |
| Days in advance         | Days in advance for insert data stamp into db | General          | 365                                                       | 0         | 0                 |
| SSIS Package            | AW Discovery Package                          | General          |                                                           | 1         | 1                 |
| SSIS Date               | AW Discovery                                  | General          |                                                           | 1         | 1                 |

**Site Creation Parameters**

| Display name          | Description                         | Category      | Module | Default value | Read only | Extended |
| :-------------------- | :---------------------------------- | :------------ | :----- | :------------ | :-------- | :------- |
| Module                | Kind of module                      | Identifiers   | E,B,P  |               | 0         | 0        |
| SiteID                | ID for subsidiary                   | -             | -      |               | 0         | 0        |
| Database Type         | Database Type                       | Connection    | *      | null          | 0         | 0        |
| Database              | Name of database                    | -             | *      | null          | 0         | 0        |
| Server Name           | Host@server or db name              | -             | *      |               | 0         | 0        |
| Username              | User for database                   | -             | *      | alcimdb       | 0         | 0        |
| Password              | Password                            | -             | *      |               | 0         | 0        |
| Connection Appendix   | Opt. appendix for connection        | -             | *      |               | 0         | 1        |
| Servicename \ Port    | Servicename \ Port (Informix)       | -             | *      |               | 0         | 0        |
| Client Locale         | Client Locale                       | -             | *      | en_US.1252    | 0         | 0        |
| DB Locale             | Database Locale                     | -             | *      | en_us.CP1252  | 0         | 0        |
| DB Provider           | Provider                            | -             | *      | internal set  | 1         | 1        |
| Date Format           | Format of date                      | Date and Time | *      | yyyy-MM-dd    | 0         | 0        |
| Start date            | Start date for import               | -             | *      |               | 0         | 0        |
| End date              | End date for import                 | -             | *      | OFF           | 0         | 0        |
| First date            | Import date for changed orders      | -             | *      |               | 0         | 0        |
| Import interval       | Import interval (in days)           | -             | *      | 0             | 0         | 0        |
| End interval date     | Only relevant in case of failure    | -             | *      |               | 1         | 1        |
| Description           | Description                         | General       | *      | Description   | 0         | 0        |
| RunLevel              | RunLevel                            | -             | *      | 2             | 0         | 0        |
| Group                 | Group                               | Global        | *      |               | 0         | 0        |
| Name for site         | Unique name for site                | -             | *      | SiteName      | 0         | 0        |
| Symbol for site       | Symbol for site                     | -             | *      | SiteName short | 0         | 0        |
| Locale ID             | Locale ID for site                  | -             | *      | Null          | 0         | 0        |
| House No.             | Internal house no                   | Master data   | E, B   | -1            | 0         | 0        |
| ImportMasterData      | Master data import for site (replication) | -             | E      |               | 0         | 0        |
| Site for articles     | Site for master articles            | -             | E,B    |               | 0         | 1        |
| Site for claim place  | Site for master claim place         | -             | *      |               | 0         | 1        |
| Site for claim reasons| Site for master claim reasons       | -             | *      |               | 0         | 1        |
| Site for claim type   | Site for master claim type          | -             | E      |               | 0         | 1        |
| Site for cost centers | Site for master cost centers        | -             | E, B   |               | 0         | 1        |
| Site for customer     | Site for master customers           | -             | *      |               | 0         | 1        |
| Site for customer delivery | Site for master customer delivery | -             | *      |               | 0         | 1        |
| Site for economic region | Site for master economic region    | -             | E      |               | 0         | 1        |
| Site for kind of order| Site for master kind of order       | -             | B      |               | 0         | 1        |
| Site for model        | Site for master model               | -             | *      |               | 0         | 1        |
| Site for object       | Site for master object              | -             | B      |               | 0         | 1        |
| Site for product groups | Site for master product groups    | -             | E, B   |               | 0         | 1        |
| Site for rebate method| Site for master rebate method       | -             | E      |               | 0         | 1        |
| Site for sales representatives| Site for master sales rep.   | -             | E, B   |               | 0         | 1        |
| Site for status       | Site for master status              | -             | B      |               | 0         | 1        |
| Site for supply       | Site for master supply              | -             | B      |               | 0         | 1        |
| Site for type of dispatch | Site for master type of disp.     | -             | E, B   |               | 0         | 1        |
| Site for type of package | Site for master type of pack.      | -             | *      |               | 0         | 1        |

## 2. Error handling

If an error should occur during data import or cube construction, these are always stored permanently under the following components:
*   Table `sysssislog` (present both in AWDiscovery as well as in AWDiscovery_Import database)
*   Event log ("application") of the computer under "AWDiscovery"

Errors within the config tool and the A+W Discovery set-up are logged as follows:
*   On each start, the config tool writes to a log file with an appropriate date stamp. The log file is usually written away under the `LogDir` registry entry (usually: `"C:\Program Files(x86)\A+W\Installation Log"`). If this entry is not present, then it is in the installation folder of A+W Discovery (usually: `"C:\Program Files (x86)\A+W\A+W Discovery"`). There, under `\Resources\Log` there is also a log file of the set-up, which is written continuously.

### 2.1. Configuration of the SQL Server services

The following table shows all required services with their start mode and "log on as" status. To be heeded is also that the start mode does not prevent a successful starting of a service.

| Name                 | Start Mode | Log On As                     |
| :------------------- | :--------- | :---------------------------- |
| Integration Services | Automatic  | NT AUTHORITY\NETWORKSERVICE   |
| Analysis Services    | "          | .\awsqlsvradmin               |
| SQL Server           | "          | LocalSystem                   |
| SQL Server Agent     | "          | .\awsqlsvradmin               |
| SQL Server Browser   | "          | LocalSystem                   |

For the SQL Server service, it must also be mentioned that here too attention must be paid to the respective instance (if there are several instances on the system).
