---
description: "EN-CONFIG-AW_Business-13"
---


This option can be enabled by ticking the checkbox Convert Date, and will be executed when the database pattern is created. Data type date is important for ALFAK capacity planning, no matter whether ALFAK Version 2011 or 2012 is used.

After that, the actual migration steps can be started.

First, select migration step Create Pattern and press OK. A script is created in the source database which is used to define the pattern on SQLServer. The database name is fixed in the script. For SQL Server, open the script in Management Studio (file/open/file). Use the Execute button to run the script. When the database has been created, the migration user has to be given access to the database (registration and database account), see 13.2.3. Important: For an SQL Base target database, the script already includes the creation of indices when this migration step has been executed. Load the script in SQL Talk and run it.

*Fig. 251: Database Migration Tool*

---
### Data migration
Choose migration step Data Migration and press OK. The table data will be transferred. Errors during data migration can be viewed in the log file afterwards (Migration.log). It is structured in such a way that the inserts can be done later. (troubleshooting provided).

*Fig. 252: Data migration – SQL Base → SQL Server with Unicode option*

### Enter foreign keys and indices
Choose migration step Create Foreign Keys (and Indices) and press OK. For an SQL Server target database, two scripts will be created which have to be loaded and run in Management Studio (file/open/file). The database requires no settings; this is part of the script. For a SQL Base target database, just one script will be generated for Foreign Key creation. This is loaded and run in SQL Talk. Unless data migration is running flawlessly, the foreign keys should not be added to the database. The script (for SQL Server target database) will delete all existing foreign keys before restoring them. This means that this process can be run as often as necessary. This also applies to the script with the indices.

### Defining or updating the ALFAK user
Porting SQL Base to SQL Server database generally requires no user migration. The following applies to database migration of ALFAK Version 2012 and higher: There is no real user migration for porting a SQL Server system to SQL Server. The migration tool defines the application role (Migration Step 4. Application Role) for the created database. A further script (SQLAuthorization.sql) is created in the A+W sub-directory of the Windows user [→ Application data for all users e.G. C:\Documents and Settings\All_Users\Application_Data\A+W\\<ALFAK_PRODUCTNAME>], to be executed in SQL Server Management studio.

If the target database is a SQL Base system, it will be first equipped with the standard ALFAK user. All others will be migrated thereafter.

Select migration step 4. User migration and press OK: the tool will trigger the commands.

### Loading SQL Base compatibility functions
To make sure that SQL Server can handle the special functions of SQL Base Datenbank (@ functions), run the script <Alfak Installationsverzeichnis>\Cmd\MS_SQLSERVER.SQL with the Management Console on the database. ATTENTION: You have to select the database; it is not fixed in the script. The database is now ready for use!

### 13.2.5. Time required
For the migration, all data records in the source database must be read in and stored in the target database. This is done using normal SQL commands. The porting of a 815 MG database on a virtual PC with 2.4 GHz requires approximately 15 minutes. A data migration with switched-on Unicode option on the same system requires approximately 20 minutes. From this, a factor of approximately 25% arises with respect to a non-Unicode to Unicode porting.

### 13.2.6. Tips and tricks
Until ALFAK2011, all text fields (long varchar) are saved as binary columns. These cannot be printed in Crystal Reports.
To print these text fields in the reports, you have to implement a function in Crystal Reports in SQL Expression Fields:
`{fn CONVERT (“BW_AUFTR_TXT”.”BEZ”,SQL_VARCHAR) }`

The error during the creation of indices (migration of a SQL Base database to SQL Server without Unicode conversion) is corrected with a repeated migration. The migration tool used to create indices which included the same columns as the primary key. One last essential aspect is that from ALFAK Version 2012 on, the Unicode option must be switched on for database migrations. The database will be automatically updated to Version 2012.

### 13.2.7. Note with activated change monitoring
If the change monitoring is active in the target database, due to the Unicode conversion, this must absolutely be reinitialized. Furthermore, the triggers for the change monitoring must be recreated. The previous database triggers still work with the ASCII data types. If one of the triggers is violated with an update of a data record, there will be a database error. This is prevented with this!

*Fig. 253: Change monitoring initialization after migration*

## 13.3. SQLBase Settings

**Performance Settings for Version 8.5**

| Selection | | |
|:---|:---|:---|
| Cache | 24000 | (min. recommended value for SQLBase 8.5 and 256 MB RAM) |
| Sortcache | 64000 | (min. recommended value for SQLBase 8.5 and 256 MB RAM) |
| Readonly | 0 | |
| Oracleouterjoin | 0 | |
| Logfileprealloc | 1 | (1= Login files are immediately created with a size of X MB) |
| Partitions | 0 | |
| Optimizerlevel | 2 | (2= current optimization technique, 1= old optimization technique) |
| Locktimeout | 275 | |
| secureapi | 0 | |
| sortlevel | 0 | (0 = activating the sort cache. For ALCIM, this parameter will cause the server to crash if the command Distinct is used in a query - it is therefore best completely deleted from SQL.ini) |
| threadmode | 1 | (1 = for NT/Win200/Win2003, 2 = for Win9x, ME) |
| workalloc | 5000 | (abhänig von der größe des Ram-Speichers des Servers Standard=1000) |

*Tab. 57: SQLBase Performance Settings*

## 14. Capacity planning

### 14.1. Description
A+W Business Capacity Planning offers the opportunity to calculate production date and costs for orders and items. The most important individual parts are described below.

### 14.2. Master data
So that the capacity planning can work correctly, a series of master data is required. This is described below.

#### 14.2.1. Work types
An activity is designated a work type, which is performed on a glass item during the value creation chain. Each production step calculated by the capacity planning is assigned a work type.
On the dialog, all settings can be changed that have a direct effect on the work types. These are, e.g. the sequence, which defines the sequence during the production process and whether the processing is only done on the main product (e.g. dispatch)

*Fig. 254 Work types*

#### 14.2.2. Allocations:
Allocations serve to assign the BOMs from the orders or quotations the required work types. Thus the capacity planning knows which work types must be performed for an item. The production sequence arises from the composition of the BOM and the sequence of the work type.

There are various types of allocations. These are evaluated in the following sequence for each BOM element. As soon as an allocation provides a match, the search is canceled and the work types in the allocation found are used.

Via the factor on some dialogs, the estimated time and costs of the work type can be adjusted again separately.

**14.2.2.1. Special allocation 4**
Here you can set that for a particular processing on a particular shape another work type (or several) than normal should apply if there is a particular follow-processing after the processing. Here you can specify on which edges which work type should be performed and calculated.

**14.2.2.2. Special allocation 2**
Here allocations can be created for edge processings on a shaped sheet. Various work types can be performed on different edges. In addition, different behavior can be set for different quantities.

**14.2.2.3. Special allocation 3**
With this allocation, you can define different work types for edge processings if they should only be done on particular edges.

**14.2.2.4. Special allocation 1**
Here you can define different work types for processings if a particular follow-up processing will be done.

**14.2.2.5. Combined product class**
On this dialog, you can allocate work types if a particular product is included in a product with a defined product class.

**14.2.2.6. Combined product type**
See combi product class, only with product type.

**14.2.2.7. Product**
Allocations of work types per product.

**14.2.2.8. Product group**
Allocations of work types per product.

**14.2.2.9. Good group / top group / main group**
Allocations of work types per goods group.

**14.2.2.10. Product type**
Allocations of work types per product type.

#### 14.2.3. Machine types
The type of a machine. This controls which restrictions are active for a machine and permit an entry.
For A+W Business Pro, there is an additional field in which the type of machine driver is set. Depending on the type, additional fields are then available on the machine dialog.

#### 14.2.4. Machines
Machines are the stations on which the required work types are performed. They are allocated restrictions, machine drivers, and costs. Here, the machine type and production area are also allocated.

#### 14.2.5. Default times
A default time is the allocation between a machine and a work type. Thus it is possible to store times for various combinations that determine how long performance of the work type takes on a machine. Here the time can be entered in hours per time unit as individual price, vector, matrix or cube.

Via the priority, you can control which machine is preferred by the scheduling for use of a work type. All other machines that were allocated the work type through a default time are entered as deviating machines, insofar as they are not declined due to restriction violation.

#### 14.2.6. Product areas
Here it is possible to group machines in order to allocate a common calendar, for example. This dialog can also be used to set which status is assigned if an item or an order has run through this production area completely.

#### 14.2.7. Transition time/matrix
Here times can be set for the transition between work types and production areas.
In the transition matrix, the duration is set in days, which must exist with a jump from a work type to the follow-up processing if here there is a change between particular production areas. Shifts can be set with specification of decimal numbers between 0 and 1.
In the transition times, the duration in shifts is specified, which must exist for the change between two work types.
On both cards, O can be used as wildcard in order to determine a transition from one or all production areas or work types.

#### 14.2.8. Calendar
The duration of the shifts is determined on the calendar. A calendar day can be assigned up to six different shift durations.
Calendars can be created for the combinations production area and site or work type and machine, whereby here O can also be used as wildcard. If a date is sought by scheduling for a work type on a machine, then the next day is sought on the appropriate calendar on which shifts are entered; there is then a check whether capacities are present.

### 14.3. Scheduling
In the scheduling, costs and time for documents are determined. Here, initially for the complete BOM of a document, the work types are sought via the allocations that are required for the production. For this work types, the possible machines are determined on which production is possible. Here, the times and costs are also calculated.
Then the production date is determined for each work type. Here, calculation is always backwards from the delivery date. The production date is thus always as close as possible to the delivery date; forward scheduling is not possible here.

#### 14.3.1. Programs
Orders can be scheduled by two programs:

**Manually**
- Single order by the user: Production > Capacity planning > Scheduling > Schedule order
- Complete number manager by the user: Production > Capacity planning > Scheduling > Schedule NM

**Create**
- through the ALFAK Interface Service (AIS)
- Standard transfer via workflow task, formula Workflow_TransferToALFAKCapacityPlanning.txt

**Configuration**
Status allocation always refers to the production transfer. In the following example, the minimum status for production transfer is status 37 which is allocated at automatic or manual scheduling as the scheduling result. Successfully scheduled orders can therefore be directly transferred - automatically or manually - to production.

**Status Points**
*Tab. 58: Status points - Capacity planning*

| No. | Required for | Designation | State Default | Min. | Lock |
|:---|:---|:---|:---|:---|:---|
| 37 | Scheduling | KAPA: scheduled (backgr) | 37 | X | X |
| 38 | Scheduling | Capacity planning: scheduled by time management | 37 | X | X |
| 39 | Scheduling | Error during automatic scheduling | 9 | X | X |
| 44 | Scheduling | No entry in TM | 37 | | |

**ERP Webservice**
Required for
- OrderXML production transfer using capacity planning data

Configuration in Master data > Company > Company data > tab Production > Order settings

#### Capacity status
- The scheduling status is shown in table BW_LOCK_KAPA, Feld KAPA_STATUS
- Used for formulas (scheduling) and order entry
- Reset to O at order entry by
	- Change of shipping or production date
	- all structural changes in an item (width or height, supply type,..)
	- BOM changes (shape, processing steps,...)
	- No reset because of price changes.

Possible values:
*Tab. 59: Capacity status*

| Value | Meaning | Application |
|:---|:---|:---|
| 0 | New order entered, or structural changes | Order entry |
| 1 | Scheduled | Scheduling |

### 14.4. Updating the old capacity planning to Patch July 2011
- **Differences from the old capacity planning:**
	- Scheduling, completion report, and control unit in program Production
	- Master data, allocations, and locks in program Capacity Planning
	- Automatic scheduling and transfer of residue by workflow tasks in AIS
	- Sql Server support
- **Procedure**
	- Unload tables KA_MENU and KA_FAVORITEN
	- Saving old programs
		- abcstamm.exe
		- abcfert.exe
		- abcstart.exe
		- abczeitw.exe
		- abcauftr.exe
		- abczwbatch.exe
		- abczwrestev.exe
		- abcreceive45.exe
	- Save capacity planning reports
		- bamasszu.qrp
		- zw_avb_st.qrp
		- zw_mar_st.qrp
		- zw_stati.qrp
		- zwaggtypen.qrp
		- zwauslastung_08.qrp
		- zwauslastung_12.qrp
		- zwbeatyp.qrp
		- zwprober.qrp)
	- Stop and delete planned tasks from the old, automatic scheduling (abczwbatch.exe) and residue transfer (abczwrestev.exe)
	- Delete the programs abczwbatch.exe and abczwrestev.exe
	- Database update (updating the menu, new database columns, creation of columns which were previously created by the program abczeitw.exe)
		- 20110328m.sql
		- 20110329a.sql
		- 20110330a.sql
		- 20110331m.sql
		- 20110401m.sql
		- 20110405a.sql
		- 20110429a.sql
		- 20110808a.sql
	- Update ALFAK installation
- Execute the ALFAK config tool to define the new TRACE switch Capacity Planning
	- **Automatic scheduling:** Add the formula Workflow_TransferToALFAKCapacityPlanning.txt as a task in AIS With this formula, from Version 10.8.2011, it is no longer necessary to schedule orders by hand which were entered BEFORE the change. This version of the formula also selects orders in the status area of automatic scheduling the entry BW_LOCK_KAPA.KAPA-STATUS of which shows NULL instead of 0. With older versions of the formula, orders have to be scheduled by hand, With older versions of the formula, orders have to be scheduled by hand,
	- **Automatic residue transfer:** Add the formula Workflow_RestManagement.txt as a task in AIS
	- Check the customizing formulas for scheduling of machine restrictions, dwell days, and priorities. The scheduling variables used in the formulas have to be converted to the new spelling (e.g. nAuftrag to m_nAuftrag). See section Customizing of scheduling
	- **OrderXML production transfer with capacity planning data**
		- Update the ERP Webservice to at least issue July 2011
		- Enable the switch Production transfer (OrderXML) with scheduling data in capacity planning settings
	- **Setup on an existing SqlServer system**
		- Migration of the existing SqlServer database (source/target SqlServer) using the migration tool and enabled option „Convert Date" to convert the existing data columns.

**Tool for checking the new capacity planning**
- `\\jupiter\ALFAK_Develop\Tools` includes the tool `abczwcompare45.exe` which can be used to compare the results of the old and new scheduling.
- This tool will work only if executed on a computer on which ALFAK 2011, issue patchday July 2011 has been installed.
- **We strongly recommend to execute the tool only on a test database and to delete the scheduling data from the database table ZW_AUFTR_ZEIT before loading the tool!**
- **Procedure - comparison**
Press the button Start old capacity planning.

*Fig. 255: Capa- Tool 1*

The old scheduling is loaded as a dialog; start it by pressing OK. The selected number manager is scheduled and scheduling is finished after that.

*Fig. 256: Capa - Start old values from ALFAK 1*

Press the button *Read old records*. The tool will read the scheduling results.

*Fig. 257: Capa- Tool 2*

Press the button *Start new capacity planning*. The new scheduling is loaded from the production program (abcfert.exe) of the ALFAK version installed; press OK to start it. The selected number manager will be scheduled. Production must be closed completely after scheduling is finished.

*Fig. 258: Capa- Start old values from ALFAK 1*

Press the button *Read new records*. The tool will read the new scheduling results.

*Fig. 259: Capa- Tool 3*

Press the button *Compare*. The tool will analyse the old and the new scheduling results.
If no differences are found, the message reads `No difference between old and new capacity planning`.

*260Fig.: Capa- Tool 4*

If differences are detected, the different records in table ZW_AUFTR_ZEIT will be listed on the spread sheet including order, item, BOM, work type, machine, time and costs. The programmer in charge will have to look into this matter.

*Fig. 261: Capa- Tool 5*

### 14.5. Configuring ALCIM with ALFAK capacity planning and OrderXML
ALFAK capacity planning with OrderXML transfer of scheduling data is possible with ALFAK 2009, patchday August 2011 and ALFAK 2011, patchday July 2011.

The correct allocation of the defining processing (e.g. cutting of a float sheet) of an element requires ALCIM version 2011, patch August!

ALCIM must be run in Professional mode without ALCIM Capacity Planning because the Compact mode includes other special features which are not taken into account by external time management!

**Procedure for new systems:**
Start with the ALCIM standard database and ALCIM in COMPACT mode. Machine allocation master data for the sections cutting, line, and spacer production have already been defined but only work via processes, not via external machine IDs.

Now enable the ALCIM Professional mode and disable ALCIM Capacity Planning. Delete the existing machine allocation master data via script and reinstall machine allocation. The result is the "old" machine allocation editor.

The script `\\jupiter\TECHSOFT Glasbaum\ALCIM\Projektierung\SQL\BereinigungMZOfuerALCIM Professional.sql` can be used to delete the machine allocation.

**Procedure for existing systems:**
In case of an update of a POOLASC system, you only need to set the element tree mode to 1 because machine allocation master data in this system are not based on ALCIM Compact structures. The above script must not be run.

To set/check the element tree mode, go to the following point in ALCIM master data:

*Fig. 262: Setting for existing system in ALCIM master data*

**Basic settings for existing and new systems**
As ALFAK knows no defining processing, the processed article must be marked by a defining processing in ALCIM (COMPACT and Professional) with the code internal processing.

Example: processing article 49000 cutting

*Fig. 263: ALCIM - Processing article*

To make sure that machine allocation during order import into ALCIM is successful, the machine numbers in ALFAK and ALCIM must be the same, or have to be allocated by means of a machine condition in ALCIM.
Machine allocation Professional - example: „Hegla cutting"

*Fig. 264: Machinery allocation ALCIM- ALFAK 1*

Select the corresponding production section (here: HEGLA cutting) and load the context menu „Modify condition“ for the condition for this production section.

*Fig. 265: Machinery allocation ALCIM- ALFAK 2*

Set the formula CUBLES-106-Zuschnitt Hegla ISO as a condition in dialog „Select condition“

*Fig. 266: Machinery allocation ALCIM- ALFAK 3*

New conditions can be defined by means of the graphics editor or the text editor by „New condition". Use „Edit" to change existing conditions. Example: Condition for allocating the ALFAK machine ID 106.

*Fig. 267: Machinery allocation ALCIM- ALFAK 4*

### 14.6. Customizing variables for machines, dwell days, priorities to be used for scheduling

*Tab. 60: Customizing- Variables*

| Meaning | Alt. | New | Example |
|:---|:---|:---|:---|
| Order number | nAuftrag | m_nAuftrag | |
| Item number | nPos | m nPos | |
| Element number (BOMID) | nBomid | m nBomid | |
| Date of entry | nErfdatum | m dtErfdatum | |
| Deliv. date | nLieferdatum | m dtLieferdatum | |
| Scheduled delivery date | dtLT Plan | m dtLT Plan | |
| Route | SATOUR | m SATOUR | |
| Customer number | nKDNR | m nKDNR | |
| Customer Name | skunde | m_skunde | |
| Priority | sRaster | m sRaster | |
| Lock code | sSperrkz | sSperrkz | |
| Document type | sDokTyp | m_sDokTyp | |
| Production preparation | | m sAvBereich | |
| Product type | nProduktart | m nProduktart | |
| Product group | nProduktgrp | m_nProduktgrp | |
| Quantity | nMenge | m_nMenge | |
| Width | nBreite | m nBreite | |
| Height | nHoehe | m nHoehe | |
| Area | nQM | m_nQM | |
| Linear meters | nLFM | m nLFM | |
| Thickness | nDicke | m nDicke | |
| Weight | nGewicht | m_nGewicht | |
| Item includes gas | nMitGas | m nMitGas | |
| Item includes shape | nlstModell | m_nlstModell | |
| Item includes Georgian bars | nMitSprossen | m_nMitSprossen | |
| Element product number | nProdukt | m nProdukt | |
| Element product group | strWGR | m sWGR | |
| Element super product group | strWOG | m_sWOG | |
| Default time - notes | sBemerkung | m_sBemerkung | |
| Processed edges | skanten | m_skanten | 01000000 = Edge 2 processed |
| Element supply type | nBeschArt | m nBeschArt | |
| Element color number | nFarbID | m nFarbID | |
| Stepped item | bStufe | m bStufe | |
| Max. glass thickness in item | nESmax | m_nESmax | |
| Min. glass thickness in item | nESmin | m_nESmin | |
| Total Width | nGes Dicke | m_nGesDicke | |
| Max. spacer thickness in item | nmaxSZR | m_nMaxSZR | |
| Min. spacer thickness in item | nminSZR | m_nMinSZR | |
| No. of film layers in item | nFolienzahl | m nFolienzahl | |
| The number of grid fields in item | nSPRFelder | m_nSPRFelder | |
| No. of grid edge connections in item | nSPR_RAP | m_nSPR_RandAnschlussPunkte | |
| Machine | nAgg | m_nAggregat | |
| Work type | nArbNr | m nArbNr | |
| Hierarchy code | nRFOZ | m nRFOZ | |
| Persons at machine | nPersonen | m nPersonen | |
| Machine runtime in hours | nStunden | m nStunden | |
| No. of shifts | nSchichten | m nSchichten | |
| Work type sequence | nFolge | m_nFolge | |
| Machine type | nAggtyp | m_nAggtyp | |
| Machine production area | nProber | m nProduktBereich | |
| Minimum time | nMinzeit | m nMinZeit | |

### 14.7. Calculation of time costs for quotes
To improve the profitability checks for quotes, you can now calculate the time costs by means of a workflow task in the ALFAK Interface Service (as from patchday September 2011). Automatic calculation will determine the material and time costs for a quotation, and purchase and sales prices can be compared.

The time costs of all quotes in the range of status point 990 „Capacity planning: Cost calculation" will be calculated automatically, and adopted for the quote. Successful calculation will raise the status of the quote to the user status of status point 990 „Capacity planning: Cost calculation" while an error (e.g. machine allocation missing) will reset the status of the quote to the user status of status point 991 „Capacity planning: Cost calculation error“.

Cost calculation only calculates the machine costs; unlike capacity planning, it does not reserve machine capacities.

To implement this function, run the database scripts 20110811a.sql and 20110812a.sql and allocate the new status points 990 „Capacity planning: Cost calculation" and 991 „Capacity planning: Cost calculation error“ to the corresponding user status in status allocation. Now enter the formula „Workflow_CostCalculationOffers.txt" as a workflow task in the ALFK Interface Service. The COM object abcreceive44.exe /abcreceive45.exe on the AIS computer must at least have version 'Patchday September 2011'.

### 14.8. Capacity information by customer
First, enter in master data the maximum production capacity in sqm, per weekday and product type. The data are entered in master data, in „Company - Company data“ on tab „13. Production“ in table „Total capacities". If no entries are made, there will be no validity check at the end of order entry.

*Fig. 268: Total capacity*

For all customers to be analysed separately (normally, the top customers or key customers), a reserved production capacity (in sqm) is entered in customer management, per product type and weekday. The corresponding table is found in customer management, tab „9. Production".

*Fig. 269: Reserved production capacity*

At the end of item entry, the capacities of the top customers are checked against the actual order data. If violations are detected for key customers or NON-key customers, the system issues a message and comes up with the overview. The fields that can cause production bottlenecks, are marked red.

To get an idea of the use of production capacity, open the menu „Functions – Capacity info by customer" in the order header.

Only articles with supply types cutting, production, and stock withdrawal with cutting will be checked. The system only checks the main items, not the bills of material!

## 15. Production data collection (barcoding)

### 15.1. Introduction
Online shop floor data collection via barcode scanner is done by a Windows-CE based scanner supplied by Datalogic (Scorpio). The actual program runs on a terminal server which connects with the scanner via remote desktop. The scanner sends all registered data to the currently active data field as keyboard entries.

To make sure that the barcoding program starts automatically when the scanner is registered at the terminal server, you need to copy a link to the barcoding program for the user to an autostart group. The program to be linked is called abcscanner.exe and is found in the Alfak program directory (e.g. C:\Program Files\A+W\ALFAK 2011\Program\German). Before starting the program, the Alfak start program must be run once on the computer, and the correct database connection must be entered in the login dialog. From that point on, the program will always connect to the database using the actual information.

The automatic start up of the program can be set by means of a configuration program (A+W Business 5 Scanner AutoStart Config) in the start menu ConfigTools from A+W Business 5.5 update 3 in the start menu Config Tools. In this program the scanner program (language dependent) can be selected for the currently registered user so that the program is started whenever the user logs in.

### 15.2. Settings

#### 15.2.1. Scanner
The scanner can be configured on any terminal. First, install the configuration software that comes with the scanner on a PC, then connect the scanner via USB. Now start the configuration software (Datalogic Configuration Utility). In the program, first set Postamble im Menü Hw Configuration > Laser > Parameters > Reader Parameters > Text Formatting. Just enter a tabulator. There are two ways of entering the tabulator. You can either enter a tabulator in an editor (e.g. Notepad or Word) and copy it to the data field by copy and paste. Alternatively, press the ALT key, and keep pressing it while entering on the number block the digits 0 0 9 before releasing the ALT key.

At the end of every scan, a [TAB] will be sent to the barcoding program to signalise that this barcode has been registered.

*Fig. 270: Completeness of barcode reading*

The second and last setting is CheckEvaluation in menu Hw Configuration > Laser > Parameters > Reader Parameters > Code39 > Standard. This must be set to Enabled so that the check digits of the Code39 barcodes will be checked instead of being sent to the program as valid data.

*Fig. 271: Code39 settings*

When all settings have been made, they can be transferred to the scanner. Select menu item Configuration > Send to Device to transfer all settings.

Alternatively, you can load the configuration file installed by the Setup/Auto-Update using the configuration program, and transfer it to the scanner. This configuration file (Datalogic Skorpio Configuration ALFAK BDE.cfg) includes all necessary settings and is found in the Config directory of the Alfak installation (e.g. C:\Program Files\A+W\Alfak 2011\Config\Datalogic Scanner Configuration).

#### 15.2.2. Master Data
The corresponding registration point type has to be entered in master data, in Production > Shop floor registration points in column 'barcode type'. This is required for the receipt of goods and for completion reports.

*Fig. 272: Enter registration point*

If the registration point has been clearly allocated to the barcode type (in the above illustration e.g. for receipt of goods), the user does not have to register the registration point at the scanner if the corresponding program point is selected.

In user management, you need to enter the personnel numbers of the users who are going to register with the scanner by means of their personnel barcode.

*Fig. 273: User management - User settings - Barcode for scanner*

#### 15.2.3. Interface Service
To book completion reports via scanner, the registered completion reports are buffered in the database before being processed by AIS. To make sure that AIS can assign these bookings, it is necessary to define the entity name of AIS as „sysadm“. This is default after installation. This setting must be checked if more than one entity of AIS is installed.

#### 15.2.4. Capacity planning
If completion reports are to be booked in Alfak capacity planning, a unique registration point must be entered for the machine in question. This is done in machine management, in Capacity planning > Master data > Organization > Machines. The work type to be used is always registered via barcode.

*Fig. 274: Machine allocation for registration point*

### 15.3. Functions
The individual barcoding dialogs and their function are listed below.

#### 15.3.1. Login
Scans can be made only after the user has scanned his personnel barcode.

*Fig. 275: Barcoding - Registration via employee barcode*

After the user has registered successfully, the program proceeds to the main menu. From there you can go to the corresponding dialogs to enter receipt of goods, inventory bookings, rack load, or completion reports.

*Fig. 276: Barcoding - Main menu*

#### 15.3.2. Receipt of goods
Scan the barcodes of the purchased items for which goods have been received.

*Fig. 277: Barcoding - Receipt of goods*

When the purchased item's barcode has been scanned, enter the quantity received (via keyboard). The program shows the full quantity for the purchased item by default; this has to be changed only if the quantity received is different. If no change is necessary, scan the barcode of the next purchased item. The program will collect these scans without actually booking them. This is only done if you press the ENTER key on the scanner or scan the barcode of another P.O. If you press the BACK key or the ESC key while there are purchased items in the memory which have not been booked so far, the program wil want to know whether these shall be booked now.

If the just scanned P.O. item is a box, you can scan a box ID barcode right afterwards and change the contents of the box if necessary. The program automatically enters a quantity of 1 piece which cannot be changed. For boxes with an ID you can enter different contents.

After a purchased item has been scanned, the bottom quantity field shows the number of articles ordered, and the number of articles received.

#### 15.3.3. Completion and breakage report
The production reports are found in the production report sub-menu, which replaces the previous completion report in the scanner main menu.

*Fig. 278 Production report menu*

The completion report dialog can be used to change the status of an order item. All scans which are made here are first saved in the database then processed by AIS as STSD reports. Status changes of orders will be made afterwards. For details on configuring the AIS for STSD reports please refer to chapter 3.5 Produktionsrückmeldung.

*Fig. 279: Barcoding - Completion report*

When an order item has been scanned, enter the quantity to be reported complete. The program will always preset the full item quantity. Press ENTER to save the completion report. The record is then processed by AIS, and the order status is amended if necessary. If only one piece is to be processed per scan, you can select the option "Quantity=1". If this option is enabled, when scanning a barcode 1 piece is immediately booked as complete. No additional quantity has to be entered nor the enter button pressed.

The breakage report dialog can be used to change the status of orders, but only negatively, in contrast to the completion report.

*Fig. 280 BDE breakage report*

Operating and booking work in the same way as the completion report, but it is possible to include the breakage reason and creator. These can be selected either by pressing the button on the scanner or by using the barcode. The barcodes can be printed out in the programs complaint reason and creator using the labels form.

After booking a record, the information on the last booking is shown as a summary on the scanner.

#### 15.3.4. Stock booking
Before starting an inventory booking, please define whether goods shall be added or withdrawn. In addition, the menu for boxes is accessible from here.

*Fig. 281: PDC - Stock movement*

*Fig. 282: PDC- Incoming stock*

*Fig. 283: PDC - Outgoing stock*

The next dialog works the same way for incoming and outgoing stock. After the stock location barcode has been read, the stock article bar code can be read and the respective quantity entered for the incoming or outgoing booking. By pressing the ENTER key, the booking is made directly.

**15.3.4.1. Transfer**
Under the stock movement menu element, there is now also the function transfer. If you select it, you must first scan a stock location bar code.

*Fig. 284: PDC - Select stock location*

After that, you land on the dialog for transferring stock items. Here the user must scan a stock item, that is, the stockID of a stock item, whereupon the current inventory is displayed. Now you should first define the quantity that should be transferred.

*Fig. 285: PDC - Transferring stock item*

Here the user can specify a new stock location and make the booking.

*Fig. 286: PDC - Successful transfer*

**15.3.4.2. Boxes**
Starting with version 12.5, there is also a Boxes submenu available. With this menu, you can call the following five functions:
1.  **Remove sheets**
    Use this function to reduce the sheet count in a box. For this, first a box bar code is scanned, and after that, the quantity displayed is set to the new value. By pressing the ENTER key, the booking is made.
2.  **Decomposing boxes**
    With this function you can decompose a box (that is, the box is deleted and the remaining sheets are booked to stock). For this, first a box is scanned and after that, its content can be edited. By pressing the ENTER key, the booking is made.
3.  **Change stock location of boxes**
    You can use this function to change the stock location of a box. For this, first a box is scanned and after that, the bar code of the new storage location is entered. The booking is then triggered immediately.
4.  **Put box on inventory list**
    Use this function to place a box on the current inventory list. After the box has been scanned, the new storage location can be scanned. After both scans have been completed, the current quantity of the sheets in the box can still be edited. By pressing the ENTER key, the booking is made.
5.  **Outgoing Goods Box**
    With this function, boxes with ident number can be assigned to an order item. Initially, an order item barcode must be scanned. After that, the number of lites in the box is determined by scanning the box barcode. It can be edited accordingly. By pressing the ENTER key, the booking is made.

#### 15.3.5. Racks
In order for racks to be able to be processed, the following conditions have to be checked beforehand:
1.  Rack numbers have to be unique. You can therefore not create a rack with the same number but a different rack type. If the same number is used, a letter should precede the rack number (for the rack type).
2.  When booking racks, the width and the height of the rack is checked and the loading weight is checked. These values can be adjusted per rack type.
3.  Rack booking was developed for shipping, i.e. only main items can be added to a rack.
4.  The only racks that can be loaded are those which are not booked for off site, have not been reported lost and are not locked.
5.  Point 5 ensures that the allocation of the rack is fully backed at rack exit.

Starting with version 6 there is also a rack submenu available. With this menu, you can call the following three functions:
1.  **Loading**
    For leading racks, the rack to be loaded first has to be selected. When scanning the rack barcode, you can add the order item to the rack in the next dialog. After the successful selection of a rack, you can add the order item to the rack. Two different modes are supported hereby, those with the buttons "Quantity = 1" and "Input quantity". The currently set mode is highlighted in green. The T2 bar code must be used to add order items. In the mode "Input quantity" after the item barcode has been scanned, the quantity that has not yet ben loaded onto the racks is shown. This can then be edited if a smaller number is to be loaded. Pressing the enter button on the scanner confirms the booking. In the mode "Quantity = 1", the booking is executed directly after scanning the order item barcode. Only 1 piece is booked hereby. The result of the last booking is always shown in the window "Last booking". To exchange the racks, press the Back button and then select a different rack.
2.  **Emptying**
    With this dialog, a rack can be reported empty. In this process, all allocations of the order items placed on the rack before are deleted. WARNING: There is no security query!!!
3.  **Display**
    With this dialog, the current allocation of order items on a rack can be displayed. If a rack barcode is scanned, the order items with the respective loaded quantity are shown in the allocation window. In addition, the customer number is also output. The list contains six entries. You can browse with the forward and backward button.

#### 15.3.6. Miscellaneous
The menu Miscellaneous includes the dialogs for order item information, registration information, and change of user. When an item barcode has been scanned, order item information will show the item name, item size, quantity, quantity delivered, price per price unit, and the delivery date.

*Fig. 287: Barcoding - Order item information*

The 'change user' dialog is explained in chapter 13.3.1 Anmelden. After scanning a valid user code, the present user will be signed out, and the new user registered.
The registration information dialog shows the currently registered user, the database, the database system (Microsoft SQL Server or Unify SQL Base), the registration point, the machine, and the work type.

*Fig. 288: Barcoding- Login information*

### 15.4. Barcodes
The individual dialogs and functions require certain barcodes. These are Code39 barcodes with check digit, with an asterisk at the start and at the end.

**Personnel barcode**
- **Prefix:** PE
- **User data:** `The personnel number` as per user management
- **Example:** *PE`000000199`F*

**Registration point barcode without work type for goods received**
- **Prefix:** RP
- **User data:** `Registration point ID`
- **Example:** *ES`0000000016`6*

**Registration point barcode and work type for completion report**
- **Prefix:** EA
- **User data:** `Registration point ID` and `work type ID` separated by a hyphen
- **Example:** *EA`0000000015`-`101`P*

**Order bar code for reporting finished and sheet-rack assignment**
- **Prefix:** T2
- **User data:** `Order number` + `item number (3-digit)` + `element number (3-digit)`
- **Example:** *T2`00000243``001``001`%*

**Order barcode for order information**
- **Prefix:** D2 or Präfix: T2
- **User data:** `Order number` + `item number (3-digit)` + `element number (3-digit)` (only T2)
- **Example:** *D2`00000243002`Q* or *T2`00000243002001`Q*

**P.O. barcode for receipt of goods**
- **Prefix:** D5
- **User data:** `P.O. number` + `item number (3-digit)`
- **Example:** *D5`000007065``001`.*

**Box barcode for stock additions and withdrawals**
- **Prefix:** BO
- **User data:** `Box ID`. Attention: ID must not start by zero!
- **Example:** *BO`BC00002`H*

**Warehouse barcode for inventory booking**
- **Prefix:** LA
- **User data:** `Warehouse ID`
- **Example:** *LA`0000000001`W* or *L`0000000001`W*

**Stock article barcode for inventory booking**
- **Prefix:** LP
- **User data:** `Stock article ID`
- **Example:** *LP`0000000164`E*

**Rack number**
- **Prefix:** GE
- **User data:** `Rack number`
- **Example:** *GE`9099`E*

**Reason for complaint**
- **Prefix:** BR
- **User data:** `Number of reason of complaint`
- **Example:** *BR`1`$*

**Cause of complaint**
- **Prefix:** BC
- **User data:** `Number of cause of complaint`
- **Example:** *BC`2`P*

### 15.4.1. Printing barcodes
In the following programs in A+W Business, a barcode printing functionality was implemented for the online plant data recording (via barcode scanner):
1.  Employee management (Master data>Company>Employees)
2.  Registration point in production (e.g. Master data>Production>Other>Registration points production)
3.  Default time (Capacity planning>Master data>Default times>Default times)
4.  Print program (e.g. Documents>Order>Print order)
5.  Stock definition (Master data>Stock>Stock definition)
6.  Stock management (Stock management>Inventory management)
7.  Racks (Production > Rack management > Racks)
8.  Reason of complaint (Master Data > Products > General > Complaint Reason)
9.  Cause of complaint (Master Data > Products > General > Complaint Cause)

If the useful data does not exceed the possible data length, the barcodes are filled up with zeros (0) (except rack barcodes). Furthermore, all barcodes received a final test digit. A general print functionality was also installed in the employee management (1). The barcodes contain the personnel number (here 199) of the employee (example: PE000000199F). The registration point barcode (2) is formed from the ID of the registration point (example: ES00000000166). In the default times program (3), the user now has the opportunity to print a registration point barcode with work type for the completion report in the online PDC. This is composed of the ID of the registration point and the ID of the work type separated by a hyphen (example: EA0000000015-101P). The print program for the form printing (4) can print an order barcode (order info in online PDC) or a purchase order barcode (incoming goods in online PDC), effective immediately. This barcode includes the document number, the 3-digit item number, and a 3-digit part number (always 000 since only main items are output here) (example order T200000243002000Q - example purchase order: D50000070650001.). For the stock booking in the PDC, the stock location must be scanned accordingly. For this, on the one hand the barcode printing on the stock definition dialog (5) was reworked and on the other hand, the online PDC was expanded. Effective immediately, the online PDC can process such storage location barcodes with an L-prefix. The barcode includes the ID of the storage location (example: *L0000000001W*). Then, barcodes of the stock items (5) are necessary for the stock booking. In the stock management, the appropriate barcodes, which include the ID of the stock item, can now be printed (example: LP0000000164E). For racks, a list of racks can be selected in rack management (7) and then printed for this barcode (Functions > Print Rack Barcode). As the racks are alphanumeric, they are not filled with leading zeros.

> **Note:** All bar codes are written to the report variable F_IDENT_C39 of the respective form/report.

### 15.5. Booking history
It is now possible to protocol the implemented completion and breakage reports. The switch "fill history table for completion reports" must be activated in the company master data on register 15. Capacity planning to activate the function.

If the switch has been activated, the edited reports are recorded in the table FS_BOOK_HISTORY. If the booking is active in the A+W Business capacity planning, the reports will also be recorded when booked in the same way. This also applies for reports performed via the dialog in A+W Business. Otherwise the bookings are recorded in PD_AWBAR.

The following data is hereby saved
- Order number
- Item number
- BOM element
- Time of scanning
- Mitarbeiter
- Registration point
- Work type (only for booking in capacity planning, otherwise 0)
- Breakage reason (only for breakage reports)
- Cause of breakage (only for breakage reports)
- Booked quantity
- Origin (BDE, manual, implicit)

Furthermore, there is an dialog on analysis of the booking history (Statistics > Booking history). Now the records to be displayed can be filtered via the QBE mode so that precise statistics, e.g. per employee, can be created.

*Fig. 289 Booking history*

By pressing, the displayed records can also be grouped according to two dynamic criteria, which can also be set in the dialog.

## 16. A+W CAD Designer (Shapes)

### 16.1. Print dimensioned sketches
Settings for the sketch size, fonts, etc. can be made in forms management of ALFAK Release 3.3.

*Fig. 290: Formula management - sketches*

The settings can be made for print item 544 - Shape sketches on a separate DIN-A4 sheet, and for sketches in the form (print items 100-499).

> **Attention:** In Releases 3.1 and 3.2, the ALFAK2000 setup program used to copy an SN.INI file automatically. This INI file contained settings to optimize the printout of sketches. However, these settings prevent those in Release 3.3 (see above) from becoming effective.
> As from 27.1.03, this INI file is no longer distributed by the setup; for all 3.3 installations before that date, the INI file must be corrected on the workstation as follows:
> DRAWINGEDGEZvmStyle = "TName = "Arial"; TScaleType = 1; TSize = 0.03; TColor = RGB(0,0,255); TBkColor = RGB(255,255,255); TULine = 0; TBold = 0; TItalic = 0; TCharSet = 0; TPFamily = 0; TWorldText = 1; LType = 0; LWidth = 1; LColor = RGB(0,0,255);"

Should the setup directory on the ALFAK server still contain an SNI.INI, this has to be deleted.

### 16.2. Copy SN files
With release 3.3, ALFAK2000 order entry allows to create SN files automatically.
We need to distinguish:

#### 16.2.1. Rectangles and standard shapes:

*Fig. 291: Create SN file name*

Press button to automatically create a serial number with suffix *.SN. The numbers are managed in number areas, per production area. The file will be saved in the directory defined for SN catalogue tables. The file will be updated whenever an item is saved.
Files created by Shaping & Nesting cannot be allocated (alpha-numerical file name).

#### 16.2.2. Shape 99 (free shape, Shaping Nesting file):

*Fig. 292: Assign available SN file*

*Fig. 293: SN file directory*

Button allows t o select a file created by Shaping & Nesting, to be allocated to an order item. This file will not be changed by ALFAK.
ALFAK can print true-to-scale sketches for these files.
