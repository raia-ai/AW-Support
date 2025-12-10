---
description: "EN-CONFIG-AW_Defect_Optimizer"
---


# A+W Configuration
# A+W Defect Optimizer

**INTERNAL**

**A+W - Software for Glass**

---

---
## Change history

| Date | Author | Changes/Comments | Version |
| :--- | :--- | :--- | :--- |
| 08/24/2015 | KM | Release (#279490) | 1.0 |
| 09/02/2015 | KM/DC | Some corrections | 1.1 |
| 10.03.2016 | KM | Version after the first test at VIO | 1.2 |
| 17.05.2016 | KM | Version after tests at Glassver | 1.3 |
| 08.12.2016 | KM | Fine coordination | 1.4 |
| 06.02.2017 | SFR | Version after installation at SGG-Auvergne | 1.5 |
| 29.11.2017 | FDR | Version after installation at SGG-Rietberg and SGG-Glassverwaltung | 1.6 |
| 20.01.2018 | SFR | Version after several installations at SGG-F with new Hegla interface | 1.7 |
| 29.06.2018 | SFR | Version after installation at SGG-Jaroszowiec | 1.8 |
| 28.09.2018 | SFR | For the installation at SGG-Jaroszowiec (part 2) | 1.9 |
| 04.04.2019 | SFR | For the latest Hegla interface (TCP/IP), clarification of the StationID - parameters | 1.10 |
| 26.04.2019 | SFR | Determination of the configuration difference for systems with and without TCP/IP communication | 1.11 |
| 02.07.2019 | SFR | Section XTV | 1.12 |
| 02.07.2019 | SFR | Restructuring/abbreviation of the installation instructions as preparation for translation and integration into setup. | 1.13 |

This document describes the necessary steps for the installation and activation of the A+W Defect Optimizers in a completely configured A+W Realtime Optimizer environment.

Starting with Version 5.4, the A+W Defect Optimizer is an integral component of the A+W Realtime Optimizer and thus part of the setup.

For details, see: `\\hausi\awdcasedoc\279\279490\20130609_Defect_handling_279490.docx`.

## 1. Requirements

### 1.1. Hardware
No requirements from the A+W side.

So that the E-marking on stockplates can be detected and transmitted to the SGG-box, a camera must be mounted on the cutting table. The installation will be organized by the location or the SGG E-marking team.

### 1.2. Network
Ports for the communication must be released on the network in advance. The following information must be communicated by the customer or the SGG E-marking team:

- IP of RTO or TS and user
- IP of the cutting table (Hegla)
- IP of the box
- ID of the box
- Port for statistics (400x)

For an unambiguous connection between box and A+W Realtime Optimizer, either each A+W Realtime Optimizer must have an individual IP address (local installation) or the port for the statistics must be unique (terminal server installation).

### 1.3. Software
- A+W Realtime Optimizer 5.4 or newer
- Planedit
- License server 5.4 or newer
- License client 5.4 or newer

If the A+W Defect Optimizer should only run in simulation mode, the XoptKernel.dll and XoptsCom.exe must have the product version 12.5.0878.0 or higher or 13.0.0878.0000 or higher.

### 1.4. Database
The two new database tables
- `XOPT_FEHLSTELLEN_JUMBO`
- `XOPT_FEHLSTELLEN_DETAIL`

are required, as are both fields
- `DEFECTAREABEFORE`
- `DEFECTAREAAFTER`

in table `XOPT_STATISTIK_JUMBO`.

## 2. Installation
This chapter serves as a check list for all preparations that must be made for the go-live.

### 2.1. Preparation for the remote test

**1 month in advance:**
- Agree directly with your customer and/or David Aout on the date for the tests.
- Gather all the necessary information (analogous to step 1.2):
    - IP of RTO or TS and user
    - IP of the cutting table (Hegla)
    - IP of the box
    - ID of the box
    - Port for statistics (400x)
- Please ask the branch office to order sufficient E-marking glass for the installation. 50 jumbos per cutting table are sufficient.

**1 week in advance:**
- Update the A+W Realtime Optimizer with hotfixes, XTV (Planedit), LicenseServer, and client to the latest version
- Update the license for the A+W Defect Optimizer (see section 3)
- Update and check the database tables
- Test the access to the A+W Realtime Optimizer-PC.
- Test the access to the TSE server (DB, logs, config, etc.)
- Prepare xopton.cfg (see section 4.3)
- Prepare cutting_TB1.bat
- Prepare cutting table-specific changes (driver, downloads in opt2txt.dat, etc.)
- Create the defect opti environment (see section 4.1)
- Activate the prioritization of rush lites for the acceptance test (see section 2.5.2)

**15 minutes before beginning of the remote test:**
- Increase the log level of the Realtime Optimizer to Infolevel
- Activate the prepared xopton.cfg
- Activate the prepared cutting table-specific changes
- Restart the Realtime Optimizer, so that the new configuration and the log level are read in
- Check the xopton log file to see whether the license was read in (see section 3.2)
- Check socket (Hegla socket on port 10000 is only available if the new Hegla software is installed and running.)

### 2.2. Remote test
- Open the cutting dialog (go to the top area Cutting>Panorama>Cutting dialog) and check under Panorama > Communication whether the light is green.
- Load an old batch with 3-6 samples.
- Follow the instructions and requirements of Hegla. (Start cutting, check whether all lights are green. Follow the instructions and requirements of Hegla. (Start cutting, check whether all lights are green. Hegla checks whether the cutting code was received...])
- Alternative: entry of rush lites and table optimization.

**CAUTION:** Do not report any breakage. Alternatively, you can go to the breakage pool and delete the appropriate glass.

### 2.3. Reworking
- Save the batch and change the status to **produced** in the A+W Realtime Optimizer in order to prevent a batch from being cut again.
- Set log level back to previous level
- Keep log files in case of problems after restart
- Delete machine status under `%appdata%\Roaming\A+W\Techsoft\Panorama\SavedMachineStatus`
- Switch the cutting table-specific changes to the old version
- Reset xopton.cfg back to the old version
- Restart the A+W Realtime Optimizer

### 2.4. Acceptance test on-site

**Connection with the box: visual check**

You can see from the user interface of the box with which systems the box is connected. The field **OPTIM SOFTWARE** displays the connection to our A+W Realtime Optimizer. Only if this field is green has the box established a connection to our software.

In the **CAMERA** field, the last detected E-marking ID is displayed (DataMatrix number). If you click the **PARSER** field and update it, the associated default map of the current plate is displayed. By clicking the top button (Java Cup), it is possible to see the image and course of the last scan.

**Pre-defined tests**

For acceptance, there are a series of pre-defined SGG tests that must be conducted. Two of these tests are to create a particular pattern and get a pre-defined defect map in order to check the results of the re-optimization of the A+W Defect Optimizer.

For these 2 tests, enter a defined number of lites with a particular priority in order to get the desired pattern with the table optimization. After you have created the appropriate pattern, the E-marking team sends Defect Map coordinated with this in order to check the functionality of the A+W Defect Optimizer.

For the tests, please enter the following data as rush lites. Make one table optimization with trim = 10mm on each side and transfer this pattern to the cutting.

- **Test 1:**
    - 1495 x 3100 (prio 0, 2 pieces)
    - 1495 x 775 (prio 1, 8 pieces)
- **Test 2:**
    - 1495 x 3100 (prio 0, 1 pieces)
    - 1495 x 1550 (prio 1, 2 pieces)

If it is not possible to enter different priorities for the rush lites, please first perform the steps described under 2.5.2.

**Checking the database**

Check whether the associated database tables are filled, as soon as defects are received and processed:
`XOPT_FEHLSTELLEN_JUMBO`, `XOPT_FEHLSTELLEN_DETAIL` and both fields `DEFECTAREABEFORE` and `DEFECTAREAAFTER` in `XOPT_STATISTIK_JUMBO`.

A query statement of the statistics is in section 2.5.3.

### 2.5. Tips and tricks

#### 2.5.1. Checking whether a socket (PORT) is open
For example, you can use telnet or PowerShell to check whether a port is open. If it's not possible to establish a connection, then the network administrator must ensure that the port is released.

**Checking with telnet**

Open the `telnet` program and enter the following command:
`open IP-PORT`

**Example:**
```
Microsoft Telnet> o 10.202.46.41 25
Connecting To 10.202.46.41...
```

**Checking with PowerShell**

Open the program and enter the following command:
`(New-Object Net.Sockets.TcpClient IP, PORT).Connected`

**Example:**
```powershell
PS C:\Users\AWServices> (New-Object Net.Sockets.TcpClient 10.128.128.27, 10000).Connected
True
PS C:\Users\AWServices>
```

#### 2.5.2. Activating prioritization of rush lites
The prioritization of rush lites is configured in the file `alcimtools.ini` under `%appdata%\techsoft\common`. Under `[Rush lites]`, add:
`EnablelnputOfPrio=0,1;`

With this entry, it is possible to record rush lites in the Realtime Optimizer with priority 0 or 1. If the section does not exist, you must add it manually. If the file alcimtools.ini is not available under `%appdata%`, you can copy it from the Trans drive `P:\common`.

#### 2.5.3. Statistics query
The A+W Realtime Optimizer sends data to the SGG box. With the following SQL script, you can query data sent to the SGG box (adjust `tisch_id` and `xfj.schneidzeit` in advance):

```sql
SELECT xfj.jobid, xfj.opt_run, xfj.muster, xfj.jumboid, sum(xfd.reorgtime) reorgtime,
    sum(xfd.totaldefectsbefore) as totdefbefore,
    sum(xfd.totaldefectsafter) as totdefafter,
    sum(xfd.primarydefectsbefore) as primdefbefore,
    sum(xfd.primarydefectsafter) as primdefafter,
    sum(xfd.defectareabefore)/1000000 as areabefore,
    sum(xfd.defectareaafter)/1000000 as areaafter
FROM xopt_fehlstellen_jumbo as xfj, xopt_fehlstellen_detail as xfd
WHERE xfj.guid = xfd.xopt_fehlstellen_jumbo_guid and schneidstatus = 1 and
    xfj.schneidzeit > '2019-01-23 00:00:00' and tisch_id = 'TB1'
group by xfj.jobid, xfj.opt_run, xfj.muster, xfj.jumboid;
```

## 3. Licensing

### 3.1. Licensing of the A+W Defect Optimizer
The A+W Defect Optimizer is a new function within the A+W Realtime Optimizer:
**Options: defect display on XTV with optimization (8[p]).**

This function requires an individual license, therefore, a new license file must be created and imported. As soon as the option is activated, it is available for all licenses of the A+W Realtime Optimizer. Therefore, it is not necessary to exchange the license file if tables on-site are already equipped with the A+W Defect Optimizer and new tables should be equipped with it.

> **Caution:** Prerequisite for the successful reading in of the new license is that the LicenseServer and the client are Version 5.4 or higher. Even if the license monitor displays a correct installation of option 4, it is not otherwise guaranteed that the license could be imported correctly and transferred to the A+W Realtime Optimizer if the LicenseServer is too old!

### 3.3. Checking of the license update
The import of the new license can be checked with the logfiles. Under:
`%programdata%\A+W\Log\XOPTON.NET_YYYYYY-MM-DD.12345.0.awtrc`

you will find one of the following entries:
- `Configuration Defect Optimization: Available! [OK]`
- `Configuration Defect Optimization: Available only for displaying defects! [OK for simulation mode]`
- `Configuration Defect Optimization: Not available! No License found! [NOK]`

## 4. Configuration

### 4.1. DefectOpti environment
Within the A+W Realtime Optimizer environment, you must create a new folder with the name `Defect`. If this folder does not exist, it must be created manually. In this folder, each table that refers to this A+W Realtime Optimizer instance has a subfolder:

- Create the folder `%appdata%\Roaming\A+W\Techsoft\Xopton\Defect\Tablename`

The A+W Defect Optimizer runs in this subfolder. It is executed with a batch called `defectopti.bat`.

- Create the batch file `defectopti.bat` in the `Tablename` folder with at least the following content:
  ```batch
  copy xopt_defect.cfg xopt.cfg
  
  XoptReorg.exe %1
  ```

Within this batch file, it is possible to copy an `xopt.cfg` file in order to consider A+W Defect Optimizer-specific settings (see section 4.4). Together with the A+W Defect Optimizer, it is no longer possible to use `XoptMult.exe`! The changes made by `XoptMult` are executed by `XoptReorg`. The configuration for `XoptReorg` (within `xopt.cfg`) can be adjusted by the customer during the test phase.

- Deactivate `XoptMult.exe` (delete it) and make the changes in the `xopt_defect.cfg` in the newly-created folder.

The application `XoptReorg.exe` executes the reorganization of the lites on a pattern with defects. The extension `%1` means that the defect optimization will be executed for each cutting code. The `XoptReorg.exe` must be in the same folder in which `xopt.exe` and `xopts.exe` are located.

- Make sure that the file `XoptReorg.exe` is in the following folder:
  `C:\Program Files (x86)\A+W\Techsoft\Xopt`

Some customers may not use `C:\`, but rather `F:\` as drive name. If the file `XoptReorg.exe` does not exist, you can simply copy one of the other `xopt.exe`, `xopts.exe`, `xoptd.exe` and rename it. The decisive difference that enables the appropriate functionality is in the 5th letter of the file name: `_`, `s`, `d`, `r`.

- Make sure that `XT_OPT2SINGLE.exe` is in the folder `C:\Program Files (x86)\A+W\Techsoft\Planedit`: it must be the latest version. Caution: this file seldom appears in updates.

### 4.2. Cut driver
`Xoptreorg.exe` sets the value `optstat=2` within the file `opt2dat.dat`. This value means "Reoptimized, pattern may not be changed after the fact." However, older machine drivers interpret this value as an error and exit. Therefore,
- you need the latest machine driver.
- The exe file for the driver must be in the subdirectory `panorama\<Table>` : `%appdata%\A+W\Techsoft\PANORAMA\XoptOn\CuttingTableHEG\cutting`

In case of the Hegla cutting table, an XML cutting code is required. In order to configure the XML cutting code,
- set the parameter `UseXMLHeader=Y` under `[Options]` in `xt_rcutf32.cfg`.
- insert 1 in section 98, position 46 in `opt2txt.dat`.

Both under `%appdata%\A+W\Techsoft\PANORAMA\XoptOn\CutTableHEG\cutting`.

For the download, you can create a file `satz98.dl` and insert the following line in `cutting.bat`:
`dl opt2txt.dat < satz98.dl`

### 4.3. XOPTON.CFG
If there is also an update of the machine partner (e.g. Hegla update to the TCP/IP protocol), the section `[Cutting]` must be adjusted, while for the A+W Defect Optimizer itself, only the section `[DefectHandling]` must be configured.

**[Cutting]**
`StationID=1`
This value represents the table ID.

> **Attention:**
> There are 2 stationIDs in the xopton.cfg:
>
> **[Cutting]**
> `StationID=1` (=Tisch ID)
>
> **[DefectHandling]**
> `InitDefectStatistic=Type=SGG;Port=4001;StationID=1` (= Box ID)

**[DefectHandling]**
There is one section per associated cutting table. In case of several cutting tables, the sections will be numbered in the usual way:
`[DefectHandling]`
`[DefectHandling1]`
`[DefectHandling2]`

The `[DefectHandling]` section is under the `[Cutting]` section and must be added manually if necessary.

If the SGG box is present, the following parameters for communication with the box must be set correctly:
- `InitDefectCommunication=Type=SGG;IP=127.0.0.1;Port=3000` (this line is not necessary for Hegla TCP/IP)
- `InitDefectStatistic=Type=SGG;Port=4000;StationID=1`

`InitDefectCommunication` serves to receive the defect maps with the error coordinates; the entry `InitDefectStatistic` is for the reporting of the statistics to the SGG box.

The IP and port addresses - in this example 4000 - must be agreed upon with SGG. In case of a Terminal Server installation, each table requires its own port! If there are 4 cutting systems with the A+W Defect Optimizer, it is likely that the ports are 4001, 4002, 4003, 4004.

The `stationID` in the line `InitDefectStatistic` is the stationID of the SGG box. The ID is important for the query of the error statistics from SGG. If an incorrect `stationID` is entered here, all available defect statistics from the database are sent.

- **Mode** = integer [0,1, 2] default 0
  - `0` -> DefectOpti Aus (for deactivation, even with active license)
  - `1` -> Display defects in XTV, but do not reoptimize (simulation mode)
  - `2` -> DefectOpti On

- **Mirror** = integer [1,2,3,4] default 1. For standard glass lites, if is is necessary to mirror the defects.
  - `1` -> No mirroring.
  - `2` -> Mirror along the X-axis (that is, on the Y-axis).
  - `3` -> Mirror along the Y-axis (that is, on the X-axis).
  - `4` -> Mirror along the X and Y-axis.
  **Example:** Error on (400|800) on a stockplate (6000|3210). Then the error is at the following coordinates:
  - `1` -> (400|800)
  - `2` -> (5600|800)
  - `3` -> (400|2410)
  - `4` -> (5600|2410)

- **MirrorCoated** = integer [1,2,3,4] default 1: like mirror, but for coated glass lites

- **MirrorStructure** = integer [1,2,3,4] default 1: like mirror, but for structured glass lites

- **DefectLimit1=A-Z, Default for SGG: K**: This defect category is only checked within the visible area and not in the area that is covered by an IG spacer.
- **DefectLimit2=A-Z, Default for SGG: Z**: This defect category (and the more severe) are considered on the entire surface per lite.
- **AutomaticLoader=Y**: If an automatic portal is present, which requires a late exchange of the cutting instructions, this switch must be set.
- **InitDefectStatistic=Type=SGG;Port=4002;StationID=1**: Required for all tables for the calling up of the statistics. The port handles the communication and is provided by the SGG Emarking Team. The stationID is the ID of the box.
- **InitDefectCommunication=Type=SGG;IP=127.0.0.0.1;Port=3000**: For all tables except Hegla tables with TCP/IP protocol! IP and port is for the communication with the SGG box. The DefectMaps are made available via this communication path.

**Additional information about the parameter DefectLimit:**
There are 2 different defect limits, which are checked by the A+W Defect Optimizer. A limit (`DefectLimit2`) is checked on the entire surface of each lite; the other (`DefectLimit1`) only within the visible area, which is not covered by the IG frame. It is intended that these limits are specified starting from a customer order. The data transfer takes place with `opt2dat.dat` and `label.set`. As long as no data come from an order, the A+W Realtime Optimizer sets the appropriate parameters with the following two switches: `DefectLimit1` and `DefectLimit2`.

The severity of the defects is coded in a single letter (A-Z). In this case, Z refers to the most severe defects, while A to the least severe defects.

**Info:** the SGG box only sends relevant defects; these are all category U. A setting outside of the SGG standard listed above is not necessary. This SGG default setting causes defects to be considered up to a medium degree of severity within a pattern, while on the edge (edge deletion area), no defect is considered.

#### 4.3.1. All tables without TCP/IP
Since the A+W Defect Optimizer also uses the PanoramaBackup file, it is necessary to add the following entry (without spaces around the character '=') in the `[Panorama]` section:

**[Panorama]**
`DeletePanoramaBackupAtStart=N`

The switch prevents not just the deletion of the panorama backup file on start of the A+W Realtime Optimizer, but also the intermediate deletion every 6 hours.

**Limitations** for all tables without TCP/IP: `Defect-Mode=2` is only possible without automatic portal (`AutomaticLoader=N`). The combination `[Mode=2; AutomaticLoader=Y]` is thus not valid.

#### 4.3.2. Example for Hegla cutting table with TCP/IP
In order to be able to use the new Hegla interface, it is necessary to add the following entries under section `[Cutting]` in `xopton.cfg` for the Hegla tables:
`InitTable=TABLE=HEGLA;TYPE=TCP/IP;IP=10.128.128.27;VERSION=3.2.0.0;PORT=10000;ENDSTATUS=1`
The IP must be the address of the Hegla computer, the port can be configured by Hegla. Normally, port 10000 is used, except if several tables are controlled by the same A+W Realtime Optimizer.

**Complete Hegla example:**
```ini
; Normal table configuration for the TCP/IP protocol
[Cutting]
Table=HEG1
StationId=1
;**********************************************************
; section for HEGLA tables
;**********************************************************
inittable=TABLE=HEGLA;TYPE=TCP/IP;IP=10.128.128.27;VERSION=3.2.0.0;PORT=10000;ENDSTATUS=1
CuttingCodeName=0(P).EDI
CuttingCodeNameSource=0(P).EDI

; Additional A+W Defect Optimizer configuration
[DefectHandling]
Mode=2
Mirror=1
MirrorCoated=1
MirrorStructure=1
DefectLimit1=K
DefectLimit2=Z
InitDefectStatistic=Type=SGG;Port=4000;StationID=1
AutomaticLoader=Y
```

#### 4.3.3. Example for Bystronic cutting table with TCP/IP
In order to be able to use the new Bystronic interface, it is necessary to add the following entries under section `[Cutting]` in `xopton.cfg` for the Bystronic tables:
`InitTable=TABLE=BYSTRONIC;TYPE=TCP/IP;IP=127.0.0.1;PORT=60000;ENDSTATUS=1`

**Complete Bystronic example:**
```ini
; Normal table configuration for the TCP/IP protocol
[Cutting]
Table=BYS1
StationId=1
;**********************************************************
; section for Bystronic table
;**********************************************************
inittable=TABLE=BYSTRONIC;TYPE=TCP/IP;IP=127.0.0.1;PORT=60000;ENDSTATUS=1
CuttingCodeName=J00(O).(P)
CuttingCodeNameSource=J00(O).(P)

; Additional A+W Defect Optimizer configuration
[DefectHandling]
Mode=2
Mirror=1
MirrorCoated=1
MirrorStructure=1
DefectLimit1=K
DefectLimit2=Z
InitDefectCommunication=Type=SGG;IP=127.0.0.1;Port=3000
InitDefectStatistic=Type=SGG;Port=4000;StationID=1
AutomaticLoader=Y
```

### 4.4. XOPT.CFG
After the reoptimization, neither the machine driver nor `XOPTMULT` may change the pattern. Favored changes within a pattern are configured in the `xopt.cfg`. For the A+W Defect Optimizer, it is possible to create an individual `xopt.cfg` within the defect environment (see section 4.1).

A new binary file called `XoptReorg.exe` calls up the optimization kernel within the defect folder. As a result, the `xopt.cfg` is read into this folder and used. There are some parameters in the `xopt.cfg` that control special functions in connection with the A+W Defect Optimizer. These are as follows:

- **MinRestKeepRight=1200**: Residual plates that exceed this length may not be shifted since they can be stored in a residual stock. If there is a residual stock, it is absolutely necessary to set these parameters. In addition, the cutting table itself can have a restriction. All smaller residual plates can be shifted and thus placed in the middle of the pattern. The default value is 1200.
- **ReorgTimeLimit=5**: Time limit in seconds for the entire reoptimization.
- **ReorgRefineLimit=5**: Time limit in seconds for the refinement within the reoptimization. A value of 0 for the second parameter switches the refinement off!
- **PushTraverseUp=0**, **PushZPrimitivesRight=0**, **PushXPrimitivesRight=0**: Since `XOPTMULT` cannot be used within the A+W Defect Optimizer, there are a few features that replace corresponding `XOPTMULT` methods, which can be activated with `0:no` `1:yes`.
- **AddXWasteToStripe=1**, **AddYWasteToStripe=1**: After the reoptimization, there is probably waste within the pattern. To ease breakout or use with automated breakout, it can be necessary to add the waste to the next adjacent stripes.
- **SimulateReorg=1**: Shifts the reoptimization into simulation mode: `opt2out.dat` and the list of the elements affected after the reoptimization is not overwritten. Recommended for first tests to check the alignment of the defects on the actual pattern!
- **KeepSecondaryDefectsVisible=1**: Normally, secondary defects are hidden. If the defects should nevertheless be displayed, this switch must be set.

These switches must be placed under the normal section `[GenericXopt]` and not under another one! Otherwise they are ignored.

### 4.5. XTV

#### 4.5.1. Position of the defects
With the use of the A+W Defect Optimizer, the DefectMaps may have to be mirrored through configuration so that the defects displayed in the XTV clearly correspond to the correct positions on the physical sheet.

#### 4.5.2. Yellow or red cross
**Yellow cross -> default, here there is nothing to configure.**

All defective lites are pre-marked on the XTV with a yellow cross. The pre-marking has no influence on the booking. In order to book a lite broken, the operator must identify it as defective as usual. If additional information (breakage causes) is configured and required, it is queried as usual.

**Red cross -> registry configuration required.**
