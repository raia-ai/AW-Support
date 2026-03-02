---
description: "EN-CONFIG-AW_Enterprise_PMO"
---


# A+W Configuration
# A+W Enterprise PMO

- -INTERNAL-
A+W - Software for Glass

---
## Change history
| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2006-02-24 | svh | Original version | 0.0.1 |
| 2006-05-31 | T.H. Schmidt | Automatic Installation on client PCs from O:\PMO | 0.0.2 |
| 2006-06-13 | svh | Addition | 0.0.3 |
| 2017-07-24 | Silvia Höpp | Addition: 64-bit | 0.0.4 |

## 1. Requirement

### 1.1. Configuration of the env variables

#### 1.1.1. GESTPLAN_PMO
Has to be activated with the value PO or PV.

#### 1.1.2. GESTPLAN_PMO_SENDCTRL
Connection parameters (host, socketmd) are stored in the variables so that the intauf can be initiated from the vbs script pmodatout.vbe.
**Caution:** this variable must ALWAYS be created generally (manr = 0).

#### 1.1.3. GESTPLAN_PMO_SERVER
The server name is entered here if the PMO should be installed as server solution. If the PMO is running locally, the variable must be deactivated.

#### 1.1.4. GESTPLAN_PMO_ERROR
In the variables, the path specification for a directory can be given in which the PMO log files are stored as zip file if an error occurs in the script processing or during the optimization.
Format: `\\[Computername]\[Directory]...`
**Caution:** The path specification must absolutely begin with a double backslash and may NOT have a backslash at the end.
**Caution:** this variable must ALWAYS be created generally (manr = 0).

### 1.2. SQL scripts
The following sql scripts must be executed:
1. `pmo_offile01.sql`
2. `pmo_ofgrp01.sql`
3. `pmo_ofrack01.sql`
4. `pmo_oftxt01.sql`
5. `pmo_ins_alsysab02.sql` (creation of the message number 64 for system message in case of flawed rack planning)

**CAUTION:** `pmo_env` is a VIEW! (All entries from alenv with group = 490) In order to avoid problems, it should be clarified explicitly whether for the user there is read access (SELECT) for this VIEW.

All env variables to be evaluated in the PMO must be assigned to the group 490 ("rack management").
For security, this group assignment should be checked, in particular for the variables:
- GTYPEN_GLEICHE_MASSE
- GTYPEN_OHNE_MODELLE
- MASSVARIANZ_NEGATIV
- MASSVARIANZ_POSITIV

Helpful SQL statement:
```sql
SELECT name, manr, gruppe, enable FROM alenv WHERE (name LIKE 'GTYPEN_%' OR name LIKE 'MASSVARIANZ_%' OR name LIKE 'GESTPLAN_%') AND gruppe=0 AND manr=0
```
If this group assignment is missing, the following UPDATE statement must be executed:
```sql
UPDATE alenv SET gruppe=490 WHERE (name LIKE 'GTYPEN_%' OR name LIKE 'MASSVARIANZ_%' OR name LIKE 'GESTPLAN_%') AND gruppe=0 AND manr=0
```

### 1.3. Settings on the system menu
System menu (CTRL+F4)->Mail system->System messages->Message assignment:
As desired:
- Add employee for meldid 61 (notification for successful PMO)
- Add employee for meldid 64 (notification for PMO scheduling error)

**Note:** Errors during the vb script execution and during the optimization run do NOT cause a system message. These errors must be read from the log files.

### 1.4. System requirements

#### 1.4.1. Windows Script Host
Windows Script Host is built into Microsoft Windows 98, 2000, and Millennium Editions. If you are running Windows 95, you can download Windows Script Host 5.6 from the Microsoft Windows Script Technologies Web site (http://msdn.microsoft.com/scripting).

#### 1.4.2. Script Encoder
http://msdn.microsoft.com/library/default.asp?url=/library/en-us/script56/html/seconscriptencoderoverview.asp

Script Encoder is a simple command-line tool that enables script designers to encode their final script so that Web hosts and Web clients cannot view or modify their source. Note that this encoding only prevents casual viewing of your code; it will not prevent the determined hacker from seeing what you've done and how.

Web designers use scripting on Web pages and server-side active server pages (.ASP) to add virtually every kind of feature you can imagine. In addition, scripting is used by the Windows® Scripting Host (WSH) and in a number of other applications with equally impressive results.

Up to now, one of the shortcomings of using scripts is that they afford no protection of the intellectual property contained within, nor do they provide any assurance that what users get is what you created. Clever algorithms and carefully designed scripts were always completely visible because they were stored as plain text. As a result, script users at every level could see the script designer's code and could then take it, modify it, and make it their own. Obviously, this is not good if you're trying to get an edge in a very competitive environment.

With the introduction of scriptlets, protecting the source code becomes even more important. Script designers want to use this simple component architecture, but they don't necessarily want to share their source code with the world. After a script is encoded, changing any part of the resulting file will render it inoperable, thus ensuring the absolute integrity of your encoded script.

Supported Operating Systems: Windows 2000; Windows 98; Windows ME; Windows NT; Windows XP

The Script Encoder is included in the Alcib-PMO installation package.
The Script Encoder must be present on each PC on which the PackView should run, in the usual directory structure: `$ProgramFiles\A+W\techsoft\PackOpti\Alcib\run\exe`.

#### 1.4.3. Miscellaneous
**IMPORTANT:**
services have to be maintained (due to AlSendCtrlCmd)

**CAUTION for remote connections:**
The terminal simulation program FIXWIN has the following property: if ALCIB is started on a remote computer, FIXWIN determines as computer name the host name from which you have established the connection. This creates problems with the PMO because this undertakes a comparison between the ALCIB computer name and the name of the PC on which the PMO polling process is running.
The only solution right now is to "pre-start" A+W Enterprise directly on the computer. If AWE was already started, the subsequent remote access is unproblematic.

### 1.5. Installation on 64-bit systems
The PMO was reworked with AWDesk #391235 for the operation on 64-bit computers.

#### 1.5.1. VB scripts (AWDesk #391235)
The VB scripts were reworked for 64-bit operation. The following scripts are required in the current version:
- `PMOkonfig.vbs`
- `PMOdatIn.vbs`
- `PMOdatOut.vbs`
- `OFrelease.vbs`
- `OFstore.vbs`
- `PMOtest.vbs` (this file is a new addition)

The file `OFkonfig.vbs`, which was previously used for the configuration of the scripts `OFrelease.vbs` and `OFstore.vbs`, is no longer needed.
From now on, the configuration of all scripts will be done via the `PMOkonfig.vbs`.

Previously, you had to enter the AWE version used during the configuration. This is no longer necessary. The script `PMOdatOut.vbs`, which requires the version specification, determines the version by itself through a query of the table `alcibversion`.

The file `PMOtest.vbs` is a small test script with which you can test after the configuration whether via the encrypted file `PMOdatOut.vbe` a database access is possible. With this test, the current AWE version is read out from the AWE DB table `alcibversion` and output.

The files `PMOkonfig.vbs` and `PMOtest.vbs` write log messages to the file `PMOkonfigLog.txt` during their execution (in the same directory as the scripts themselves).

All scripts listed above include a logic that ensures that the scripts are ALWAYS executed on the 32-bit script host, so that there are no problems with the access to the Informix DB (on the AWE side, the Informix client SDK is used in the 32-bit version, because only an Informix ODBC Driver 32-bit is available).

So that the outputs of the scripts (stdout) can be written to the log files that specify the batch scripts to be called, the call of the script must be made explicitly via the 32-bit script host.

### 1.6. DB connection
On each PC or the server on which the PMO is installed, AND on every PC on which PackView is installed, the following must also be installed:

#### 1.6.1. Informix Client

#### 1.6.2. ODBC data source (32-bit)
For the access of the vbs scripts to the pmo tables of the alcib database:
- Create System DSN
- Create users for the DB access of the vbs scripts

### 1.7. Automatic installation of the rack optimization on client PCs from the directory O:PMO
The central directory `O:\PMO` must contain all ALCIB/PMO files, that is `O:\PMO\ReadMe.txt`, `O:\PMO\PMOkonfig.vbs`, `O:\PMO\run\PMOdatOut.vbs`, ...etc. If necessary, you unpack these from the archive `ALCIB.ZIP`. With an update of the central directory, initially first all files there are deleted, so that it is certain that no out-of-date files remain there. During the update of the central directory, the PMO should not be started on any client PC. Otherwise it would be possible that during the provision of the new files, a client PC undertakes an update with `StartpollPMO.bat`, which then does not (yet) contain all current files. During the update of the central directory, you could also rename the directory name `O:\PMO` (to `O:\PMOupdating`, for example), in order to prevent such an incomplete update.

On each client PC, the directory `C:\Programme\A+W\techsoft\PackOpti\Alcib` is created and `StartpollPMO.bat` is copied there from `ALCIB.ZIP`. (Alternatively, `C:\techsoft\alcim\PackOpti\Alcib` can also be used as the target directory). `StartpollPMO.bat` is deleted (automatically) from `O:\PMO` and is therefore only present in `ALCIB.ZIP`. For the convenience of the user, you should set up a START link on the desktop with which you can reach `StartpollPMO.bat` easily.

The call of `StartpollPMO.bat` on the client PC installs and then starts the PMO. If it has not yet happened, here (once) the configuration of the scripts for the database access is executed automatically. (*) (**) The scripts in plain text (*.VBS) are deleted after the configuration from the central directory (only the configured and compiled *.VBE scripts remain on the server - these are then taken over for each client PC on the next start of the PMO). As long as this configuration of the *.VBS scripts is not yet completed, only an appropriately authorized user should execute `StartpollPMO.bat` for initially the configuration of the *.VBS scripts is always started.

After an update of the central directory, the update of each local PC is done automatically as soon as `StartpollPMO.bat` is executed. According to our experiments, there are no conflicts if several processes execute the update at the same time. However, the update is only executed reliably if the times of the participating computers are correct, for in each case only newer (or if necessary files previously not yet present) are copied. However, it doesn't hurt if you delete all PMO files on the client PC and only leave `StartpollPMO.bat`. The call of `StartpollPMO.bat` installs and starts the PMO.

### 1.8. Manual installation of the rack optimization
Either on all client PCs or on a server through unpacking of the files from `Alcib.zip` after `$ProgramFiles\A+W\techsoft\PackOpti\Alcib`. (Alternatively, `C:\techsoft\alcim\PackOpti\Alcib` can also be used).

#### 1.8.1. Configuration of the PMO-vb scripts
Adjustment of the vbs scripts for the db access and encryption of the vbs files with ScriptEncoder.
There is a script available: `$ProgramFiles\A+W\techsoft\PackOpti\Alcib\PMOkonfig.vbs`
When calling the script, the configuration parameters for the ODBC connection (DNS + USER + PWD) for the files:
- `$ProgramFiles\A+W\techsoft\PackOpti\Alcib\PMOdatIn.vbs` and
- `$ProgramFiles\A+W\techsoft\PackOpti\Alcib\run\PMOdatOut.vbs`
are queried and an encrypted version of the scripts with the parameter specifications is generated automatically.

Resulting are the files:
- `$ProgramFiles\A+W\techsoft\PackOpti\Alcib\PMOdatIn.vbe`
- `$ProgramFiles\A+W\techsoft\PackOpti\Alcib\run\PMOdatOut.vbe`

#### 1.8.2. AlSendCtrlCmd.exe
`AlSendCtrlCmd.exe` must be present in the directory `$ProgramFiles\A+W\techsoft\PackOpti\Alcib\run\`. The program is used to initiate the `intauf` process:
- The path to the bin directory of the Informix client must be entered in the PATH variable on the PC, otherwise AlSendCtrlCmd.exe will not find isqlt09a.dll.
- the msvcr71.dll must be present

### 1.9. Installation of the graphic box display PackView
PackView must be installed on this PC for the three-dimensional display of the boxes on the PC screen. This is easiest to do with the appropriate setup (PVSetup.exe). Alternatively, you can also copy the necessary files "by hand." The file extension OUT must be registered for PackView. You can either have this done by the PackView setup or do it "by hand." After the setup, the file `Packopt.exe` has to be copied into the same directory as PackView.exe (otherwise error message "Could not execute PACKOP.EXE/GS"). For the test, you should check before starting the PMO with a double-click on the sample file `123456auf.csv.out` that PackView displays this result file as desired.
In rare cases, it happens that the PackView does not start, but rather no display at all appears. In this case, you call up the DirectX diagnostic program `DXDIAG` and deactivate the AGP interface acceleration on the "Display" tab.

If at the start of the PackView you want to switch off the box display "from above," you can set the following entry in the registry:
```reg
Windows Registry Editor Version 5.00
[HKEY_CURRENT_USER\Software\ALBAT + WIRSAM\PackView\Views\TopView]
"Visible"=dword:00000000
```

#### 1.9.1. Configuration of the PackView vb scripts
(section updated 24.07.2017, AWDesk #391235)
On each PC on which the PackView should be called up, the scripts `OFstore.vbs` and `OFrelease.vbs` in the directory `$ProgramFiles\A+W\techsoft\PackOpti\Alcib` must be present.
The scripts are configured precisely like the PMO*.vbs files by calling the `PMOkonfig.vbs`.

### 1.10. Ongoing operation of the PMO
For processing of optimization orders from Alcib, the PMO must be switched to ready with `StartpollPMO.bat`. This has to be done once when the user logs in on the PC (for example, in the autostart). You can see that the PMO is active in a window "pollPMO" (visible on the start bar).
Before logging off, `StoppollPMO.bat` must be called so that any existing PMO tasks are completed regularly. Possibly `StoppollPMO.bat` must also be called several times until the "pollPMO" window disappears.
For the convenience of the user, you should set up START and STOP links on the desktop with which you can reach `StartpollPMO.bat` and `StoppollPMO.bat` easily.

If during the optimization or during data transfer from or to ALCIB there is an error, a ZIP archive with all required data is stored in a defined directory (example Pilkington Fireprotection: `\\sdeaw02\usr1\awserv\pmo_fehler`). If you would like to configure a directory, you can create a file `AlcibFailFolder` (`C:\Programs\A+W\techsoft\PackOpti\Alcib\AlcibFailFolder`) the first line of which contains the desired directory name (without final backslash).
Starting with ALCIB Version 4.0, the environment variable `GESTPLAN_PMO_ERROR` (see above) is available, in which you can enter and activate the desired directory path.
If at the same time an `AlcibFailFolder` entry and final variable entry exist, the variable entry will be handled with priority.

## 2. Planning Web

### 2.1. Rack types
For configuration of the rack types, you must take the following steps:
1. Open the A+W Planning Web, for example via the A+W folder on the desktop. Normally this page is hosted under `http://[processserver]/Planning.Web`. Then the browser opens with the start page of the A+W Planning Web.
2. Press the **Stock** button.
3. Then click the **Master data** menu and there, the **[Rack properties]** button.
4. New rack types can be created and configured here. For this, either change values of an existing rack type directly or create a new rack type with the **[+ Add]** button. The following fields must be configured:
    - **Description:** unique name for identification of a rack type
    - **Access type:** describes how glass can be stacked up or down. Available options:
        - **Free:** random access to the glass (e.g. harp racks)
        - **First in, First out (FiFo):** only the first glass stored can be removed (e.g. through passage)
        - **Last in, First out (LiFo):** only the last glass stored can be removed (e.g. A-rack)
    - **Maximum weight:** maximum weight in kg
    - **Maximum height:** maximum height of the glass that can be placed on this rack type.
    - **Maximum width:** maximum width of the glass that can be placed on this rack type. In the case of several stacks, this value describes the maximum width of all stacks together.
    - **Maximum depth:** maximum depth of the rack. With a glass stack, all thicknesses of the glass in a stack are added together. For harp racks, the maximum depth is set equal to the width of a single slot.
    - **Minimum height:** minimum height of the glass that may be placed on this rack type.
    - **Minimum width:** minimum width of the glass that may be placed on this rack type.
    - **Maximum number of stacks/slots:** maximum permissible number of stacks on this rack type. For a harp rack, this is the number of slots. If the value -1 is set, the number is unlimited; then only the other values such as maximum height, width or depth are consulted for restrictions.
    - **Segment type:** the type of this rack type. Available options:
        - **HarpRack:** Harp racks
        - **LRack:** L-rack
        For configuration of an A-rack, two L-racks must be created.

### 2.2. Stock incl. rack
After the rack types were created as described under 2.1, the Stock, Stock areas, and Rack can be configured in the Master data. The following steps are required for this:
1. Call of the configuration page of the stock starting from the start page via Stock > Master data.
2. Change of the values of already existing stock or addition of a new stock via the **[+ Add]** button. The following fields must be configured:
    - **ID:** unique numeric key; if a new stock is created, the next ID not yet assigned will be suggested. Any previous IDs that have been freed up through the deletion of a stock will not be taken into account and therefore not suggested. It is possible to select the ID manually. If the ID already exists, a corresponding message will point this out and prevent saving.
    - **Description:** a unique name of the stock area
3. If a new stock was created, **[Save]** must be pressed so that the changes are taken over.
4. Open the settings for the storage location of this stock with a click on **[Edit]**.
5. Either change values of existing storage locations directly or add a new storage location with the **[+ Add]** button. The following fields must be configured:
    - **ID:** Unique numeric code, this code must be unique across all stocks. If a new storage location is created, the next ID not yet assigned will be suggested. Any previous IDs that have been freed up through the deletion of a storage location will not be taken into account and therefore not suggested. It is possible to select the ID manually. If the ID already exists, a corresponding message will point this out and prevent saving.
    - **Description:** A unique name of the storage location
    - **Stock types:**
        - **Storage location:** simple stock
        - **Stock receipt:** a receipt/removal for the other stock
    
    > For each table with the corresponding table ID, a stock and a storage location with the type Stock receipt should be created so that new residual plates can be created manually and can be stored in other stock locations.
    
    > The other stock types are conceived for a sortjet and are not used in the RSM. Available types include: Stock location, Loading, Buffer, Loading station, Shuttle, Stock receipt.

    - **Allocation status:** here you can set whether the storage location can be used with racks or is locked. A manual lock would make sense, for example, if the area is blocked due to a goods delivery. Here, storage locations that were locked by the system can be re-enabled.

6. Save change with a click on **[Save]** so that the changes are taken over.
7. If for the respective storage locations you click **[Edit]**, the allocated rack one level below opens. Lites can only be booked on racks, therefore it is advisable to configure at least one rack for each storage location.
8. With the **[+ Add]** button, you can create a new rack. The following fields must be configured:
    - **ID:** unique numeric code, this code must be unique across all racks. If a new rack is created, the next ID not yet assigned will be suggested. Any previous IDs that have been freed up through the deletion of a rack will not be taken into account and therefore not suggested. It is possible to select the ID manually. If the ID already exists, a corresponding message will point this out and prevent saving.
    - **Description:** a unique name of the rack
    - **Allocation status:** here you can set whether the rack can be used for lites or if it is locked. A manual lock would make sense, for example, if the area is blocked due to a goods delivery. Here, racks that were locked by the system can be re-enabled.
    - **Properties:** the rack type can be selected from among all the previously created rack types. How rack types are created is described in 2.1.

## 3. Realtime Optimizer

### 3.1. Xopton.cfg
So that the A+W Residual Stock Manager and A+W Realtime Optimizer can communicate with one another, the configuration file of the A+W Realtime Optimizer, `xopton.cfg`, must be adjusted. This file is under:
`%appdata%\A+W\TECHSOFT\Xopton`

Basically, for this file:
- all lines that start with a semicolon are commented out and will not be considered. It can be necessary to remove semicolons in order to activate the configuration.
- Between parameters, assignment operator `=` and the value assigned, there may be no empty spaces. That is:
    - False: `Table = TB1`
    - True: `Table=TB1`
- At the end of the document, there is a description of all parameters and their assignment possibilities.

In the `Remaster` section, the following parameters must be set:
```ini
; ....... Section for Hegla Remaster .................
[Remaster]
Remaster=Y
NumberOfRemasters=1
Remaster1=Tablename,StockID
RemasterMode=6
MinRemasterLength=1000
```
The table must be entered in the `Table name` field that should work with the stock in question in the A+W Residual Stock Manager. The possible tables are in the `xopton.cfg` under:
```ini
; ....... Section for cutting .................
[Cutting]
Table=Table name
```
Also configured in the `xopton.cfg`. The `StockID` is the ID of the stock that the table can access. For the ID, consult the A+W Planning Web. It is possible to configure several manual residual stocks, then the parameter `NumberOfRemasters` must be adjusted accordingly and a new line with `RemasterX=Table name,StockID` inserted for each residual stock.

### 3.2. Settings directly in the program
In addition to the `xopton.cfg`, the use of a residual stock must also be activated in the A+W Realtime Optimizer. For this, the following steps are required after the start of the A+W Realtime Optimizer:
1. Click the **Settings > Tables** menu element, this will open the Settings window.
2. Place a checkmark in the 3 boxes in the **Residual plate stock** section. Here it is also possible to define the minimum storage length and decide whether residual plates should only be placed in or used from the stock. The settings here override the configuration in the `xopton.cfg` file.
    - **Residual Warehouse**
        - `[x] Active`
        - `[x] Store Plates`
        - `[x] Use Plates`
        - **Minimum Storage Length**: 100
    - **Cutting**
        - **Edit Residual Plate**
        - **Minimum Storage Length**: 0

## 4. Configuration of the infrastructure web
In order to print labels for residual quantities, the following adjustment must be made in the configuration of the infrastructure web under **Stock label Print**.

- In the **Stock Id** field, enter the stock number that should be printed. You can configure one printer per created stock.
- In the **Printer** field, specify the printer on which the labels should be printed.
- In the **Report Name** field, the name of the report.
- Printer and Report Name must be specified as absolute paths.
- The **Station Group** field refers to the groups defined in A+W Production (A+W Production > Parameter Administrator > Release dialog, Group of executing computers area). The job service writes this entry to the process table.

**Example:** If the ProcessManager that is entered in `Group 1` should print the report, then in the Web interface, `1` should be entered in the **Station Group** field. `Group 0` is reserved for the release dialog.

The **Stock Connection Settings** and **Table to Stock Assignment** areas contain parameters for the Stock Service, so that it can communicate with an external stock, e.g. the Hegla ReMaster.

### Stock Connection Settings
In this area, you make the settings for the stock connection.
- In the **Stock Id** field, enter the stock ID to be incorporated.
- In the **IP Address** field, enter the appropriate Hegla (stock) IP address.
- In the **Port** field, the port number to be used must be entered.
- In the **Stock Interface Version** field, the interface or interface version that is used.
To add a new stock connection, click the **+** and fill out the fields described above accordingly.

### Table to Stock Assignment
In this area, you can assign cutting tables to individual stocks.
- In the **Table Id** field, enter the appropriate table number.
- In the **Stock Id** field, the appropriate stock number.
- The combo box in the **Stock Type** field contains the entries **External** and **Internal**.
    - Here, the Stock ID of an **internal** stock corresponds to an internal storage of the warehouse ID in the planning web (RSM).
    - The Stock ID of an **external** stock corresponds to the ID in the Stock Connection Settings (e.g. Hegla, ReMaster, other manufacturers are also possible).

With a click on **X**, the corresponding entry is removed.

After the settings were made, you should ensure here that the Stock Service is restarted. This is necessary since otherwise the service will not connect to the ReMaster.

## 5. Optimization kernel: Xopt.cfg
In addition to the configuration in the `xopton.cfg`, various parameters for the optimization kernel can be overridden. Usually this is not necessary, but it can be appropriate for test scenarios or other fine-tuning. The parameters listed here should only be activated if the person activating them is aware of the changes they will cause. In the worst case, the use of residual plates can be deactivated completely or the use of an excessive number of residual plates can slow down the production flow.

Since the parameters in the `xopt.cfg` file override parameters from the file `opt2par.dat`, a check of these entries in advance makes sense. The `opt2par.dat` file can be opened with the A+W Tool DebNET.exe. For this, just copy the program `\\jupiter\TECHSOFT Glasbaum\XOPT\TOOLS\DEBUG\DebNET.exe` into the directory with the individual opt2 files (for example, in the directory for table optimization listed below) and open it with a double-click. Editing of the opt2 files is not possible.

The `xopt.cfg` master file is under `P:\Release\Save`.

This `xopt.cfg` file is copied for each table optimization into the directory `%appdata%\A+W\TECHSOFT\Xopton\TOPT01`.

The individual opt2 files can also be copied here for each table optimization. If the master file is changed, this change takes effect with the next optimization. No restart of the A+W Realtime Optimizer is required. The following parameters influence the use of the residual plates from the A+W Residual Stock Manager and replace individual parameters from the `opt2par.dat` file:

- **ForceStockplateSequence**
This parameter can be used to override the `StockInSequence` entry in the `opt2par.dat` and controls the processing of the stock dimension.
    - **`=0` (Default)** All entries for stock plates are treated the same. There is no special logic for residual plates. Control via prices is possible now as before.
    > **Caution:** if everything is configured for the A+W Residual Stock Manager, then the access sequence (>=1) is entered in the price field for the residual plates. Since in this case, the dimensions have a 0 in the price field, no residual plates will be used since they have a higher price.
    - **`=1`** All stock plates are processed strictly in the order of their entries. The field `PRICE` in the `opt2par.dat`, record 3 is used as sort index in ascending order. If no prices are specified, then procedure is automatically as in the case `= 0`. If prices exist, the least expensive stockplate is necessarily processed first. The next stockplate in the sequence is only begun once all plates of the previous stage are completely used up. If there are two residual plates with sequence 1 and a residual plate with sequence 2, then first both residual plates with sequence 1 must be used before the residual plate with sequence 2 can be used. This ensures that residual plates used are also accessible. The sequence is visible on the table optimization dialog or it can be checked with the A+W tool Deb.NET in the `opt2par.dat` file.
    - **`=2`** This is the default setting for use of the A+W Residual Stock Manager. The stockplates and residuals are categorized using the entries in the `RESTLAGER` field in the `opt2par.dat`, record 3. Here, the entry 0 means that this is a normal stockplate; 1 that this is a residual plate from an automatic stock, and 2 that the residual plate is stored in a manual stock. Depending on the entry, the residual plates are planned as follows:
    Residual plates from an automatic stock are preferred if they can be occupied (a plate may be too small for the current order dimensions). If these residual plates have been processed or cannot be processed, normal stockplates and manual residual plates are checked and used depending on the achievable yield. A manual residual plate is therefore only used if a better yield is achieved as a result (which will automatically be the case, for example, with small order quantities). In the case of manual residual plates, additional attention is paid to whether they may stand on a stack and can only be used in a certain sequence.
    - **`=3`** Precisely as with `ForceStockplateSequence=2` with the following deviation: The residual plates from the automatic stock are not preferred, but rather only used according to the yield.

- **ConsumeResidualsFirst=1**
If this parameter is set, all residual plates are used before the stockplates, regardless of the yield or whether the stock is manual or automatic. This happens until either all residual plates are used up or a residual plate to be processed manually cannot be used. A manual residual plate cannot be used if it is not in the first position on an A-rack stack or if it is too small for the lites to be cut. As soon as the optimization kernel encounters a residual plate that is not accessible, only stockplates are used. In this case, starting at this time, all residual plates are ignored for the rest of the current optimization batch (background: the other residual plates are then not accessible).

- **IgnorePricemarkeForResiduals=1**
If this parameter is set, residual plates are only used if the yield increases with their use. Thus, residual plates are not preferred and it can happen that the residual plate stock is overloaded or completely loaded.

- **InvertMIMResidueSetting=1**
If residual plates are used for a table optimization, all available residual plates are locked until the optimization is either saved or cut. Only then will the residual plates not used be released for a new optimization. This prevents double use.
With the parameter `InvertMIMResidueSetting`, parameters set by the A+W Realtime Optimizer within the `opt2par` file are modified so that the save files can be used for additional tests directly with the optimization kernel. Therefore, setting this parameter makes sense only if the A+W Realtime Optimizer should use save files modified by a table optimization for tests with the optimization kernel. **This parameter may not be set in live operation!**

## 6. Examples
In A+W Enterprise, an order-precise rack optimization can be executed from the order entry.

### 6.1. Master data
The restrictions of the PMO that are specified by A+W Enterprise include the rack main group (packaging type) and the maximum weight per rack. Both specifications are stored customer-specifically in the master data.

#### 6.1.1. Packaging type
The packaging type stored in the customer master data (field `Verpackart`) must correspond to the desired rack main group.

#### 6.1.2. Maximum weight per rack
The maximum weight per rack is set in the customer master data in the production-specific tab (field `Gestellgewicht (max)`).

#### 6.1.3. Rack types
All rack types that should be available to the PMO must be created in the master data with the correct main group. The field "Number of places" must be assigned 1 or 2.

#### 6.1.4. Priority sequence
The priority of the rack types must be stored in the master data under `Prioritätssteuerung Gestelle` (Rack Priority Control).

#### 6.1.5. Restrictions from environment variables
The restrictions from the following A+W Enterprise environment variables are taken over from the PMO:
- GESTPLAN_MASS_FAKTOR_BREITE
- GESTPLAN_MASS_FAKTOR_HOEHE
- GTYPEN_GLEICHE_MASSE
- GTYPEN_OHNE_MODELLE
- MASSVARIANZ_NEGATIV
- MASSVARIANZ_POSITIV

### 6.2. Execution of the PMO

#### 6.2.1. Rack planning dialog
The rack planning is accessed from the order footer with `<CTRL+G>`. The algorithm is set to "PO" in the `Sort` column for the relevant items. After pressing `<F5>` (Start Packm.planung), a confirmation dialog appears to start the optimization.

The transfer to the PMO only takes place if the order is saved and exited. The PMO is done asynchronously. Until the optimization result was written back successfully by A+W Enterprise, the order remains locked with `still= -29`.

#### 6.2.2. PMO result
The PMO result can be viewed in A+W Enterprise with renewed call of the rack planning (in the order footer), then with `<CTRL+F10>` to change to the results dialog. The dialog will show the items assigned to specific rack numbers (`Gestellnr`).

#### 6.2.3. PackView call
The PMO result can also be viewed and edited from the rack planning with the PackView program. For this, you must press the key combination `<SHIFT+F9>` on the Rack planning dialog.

PMO results can be edited at will via PackView. The result is taken over into A+W Enterprise after exiting PackView. A+W Enterprise provides special `pmo_of*` data structures for this. From these data structures, the appropriate out file is generated before opening PackView.

The rack sequence (`pmo_ofrack.rackid`) determined by the PMO is also reflected In the `pmo_of*` data structures.
An order that was replanned manually after PMO or that was planned after the fact via an A+W Enterprise sort algorithm can no longer be displayed in PackView.

### 6.3. Special specifications for the PMO

#### 6.3.1. Grouping
On the Rack planning dialog, a grouping of the items can be specified for the PMO by entering the same number in the `Gruppe` (Group) column for items that should be kept together. Grouped items are kept together on racks.

#### 6.3.2. Grouping with number
On the Rack planning dialog, the number of lites of an item can be specified in addition to the grouping for the PMO. By using the `Anzahl` (Number/Quantity) column, you can specify that a certain quantity of an item should be kept together within a group. Grouped item quantities will be kept together on racks.
