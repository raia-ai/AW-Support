---
description: "EN-INST-AW_Business_Production_Manager_3"
---


---
## 6.1.10 New AWB function: turning of standard models on the order entry screen (#377601)

Please, check the minimal Program requirements (October 2017):

1.  AWB version: 13.4.47
2.  Production Manager version: 13.4.629
3.  AWB DB Skript: 20170927a.sql

## 6.1.11 Different stock and plate bookings via XTV reporting

The Production Manager writes a PRODBDA into the FS_POOL_KOPF table and P and S records into the FS_POOL table to book the stockplates (used by optimization) in AWB. The extension of the PRODBDA tells the AWB the stock from the stockplate. The extension is a number like 002 or 013 and means stock with id 2 or 13. You have to set one thing in the stock masterdata of AWB and then AWB books correct.

Goto: MasterData > Stock > Stock Definition

_Figure 60: Stock ID for the booking of stockplates_

You have to enter the **Name** text field (orange marked). You can enter the Stock Ids (semicolon separated) in the Name text field: `1;2;3;4`. If the PRODBDA file name has one this extension, AWB books the plate from this stock.

You should write follow in the **Name** text field in the Production Manager environment:

`Stockld;Stock name`

For example:

`2;Hegla Stock`

This means for XOPTON that a stock is used. The Stock ID comes from the column Barcode-ID (green marked).

## 6.2 Known errors and workarounds

### 6.2.1 Problems installing Microsoft components

*   **Problem**
    Installation of the SQL Server Native Client and/or MS C++ Redistributable fails.

*   **Cause**
    Regular Windows updates have been run previously and require the system to be rebooted.

*   **Remedy**
    The system first has to be brought to a consolidated status. Any updates need to be performed as well as any required reboots.

### 6.2.2 xOptMult and xRecalc batches

If you have problems with the order of sheets after the optimization, it could be that the optimization does not call xOptMult and xReCalc.

**Issue**: We have to use the short path in the batches, but we used the long path.

Please, check this registry entry to check the Techsoft RootDirectory path:
`Computer\HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Albat+Wirsam\Techsoft`

_Figure 61: Registry Techsoft root directory_

| Name | Type | Data |
| --- | --- | --- |
| (Default) | REG_SZ | (value not set) |
| RootDirectory | REG_SZ | C:\Program Files (x86)\A+W\Techsoft\ |
| ServerDirectory | REG_SZ | \\MST-DEV15\Trans |
| ServerVolume | REG_SZ | P: |
| TerminalServerMode | REG_DWORD | 0x00000001 (1) |

Open the directory `ServerDir\Common` (mostly `P:\Common`):

_Figure 62: p:\Common directory_

1.  Open the `xOptMult.bat`

If the batch looks like this:

_Figure 63: xOptMult batch long path name_
```bat
@ECHO ON
REM Root Dir bestimmen
setlocal ENABLEEXTENSIONS
@for /f "tokens=3*" %%i in ('reg query "HKLM\Software\Albat+Wirsam\Techsoft" /v "Root Directory"') do @Set "RootDir=%%~j"
echo RootDir = %RootDir%
REM Remove trailing backslash
if %RootDir:~-1%==.\ set RootDir=%RootDir:~0,-1%
```

Change the marked place to:
`"RootDir=%%~sj"`

See here:

_Figure 64: xOptMult batch short path name_
```bat
@ECHO ON
REM Root Dir bestimmen
setlocal ENABLEEXTENSIONS
@for /f "tokens=3*" %%i in ('reg query "HKLM\Software\Albat+Wirsam\Techsoft" /v "Root Directory"') do @Set "RootDir=%%~sj"
echo RootDir = %RootDir%
REM Remove trailing backslash
if %RootDir:~-1%==.\ set RootDir=%RootDir:~0,-1%
```

You have to do the same at the `xReCalc.bat`.

### 6.2.3 XRecalc errors

We get sometimes errors at optimization from the XRecalc. Check the follow files:
Block.pth and Opt2txt.dat in SN Default user directory and SN user `%Appdata%\A+W\TECHSOFT\SN` (see 6.4)

Either the Block file path is wrong and/or the block entry has the wrong dimension. That means that you have Shape 99 in the optimization because:
- There is a Shape 99 in the Job
- The customer marks some processing on the cutting table (drill holes, cut-out or corner rounding).

## 6.3 New features in V6

The features 6.3.1 till 6.3.4 implemented in latest hotfix of V6 and V6.1 or higher.
Check chapter 2.4 because we do not patch V6 anymore.

### 6.3.1 New columns in Prod_OPTI_STATISTICS (#361422)

You need the SQL script with the number 20160405.

The new columns (all decimal(28,8)) could be used for reports:
1.  **RES_OUT_AREA**: residual area created
2.  **RES_IN_AREA**: Area of used residual plates (without trim)
3.  **RES_IN_AREATRIM**: Area of residuals used

### 6.3.2 Use the latest user input for new variant of optimization in Optimization Manager (#360709)

**The situation before:**
The user edits stockplate and optimization parameters and after the optimization the user input is away.

**Now**, the programs remember the user input for every glass article and show the latest user input for every glass article.

### 6.3.3 Send waste to AWB for cost calculation (#363566)

The A+W Production Manager sends the waste to the A+W Business after the user saves the quotation and the AWBusiness calculates the cost for the item in the position automatically because the Production Manager calls the A+W Business COM object to calculate the costs. This only works in the Production Manager quotation mode (Offer mode).

You need the script 20160509 to insert (BW_AUFTR_OPTI and BW_ANGEB_OPTI) and update database tables.

### 6.3.4 New driver scripts

We support new drivers (the script 20160502 update database tables):
- PerfectCut - Pattern
- PerfectCut - Racks
- Optima cutting driver

Other new drivers (the script 20160201 update database tables):
- PDS bender
- PDS IG line

### 6.3.5 Multi selection in lists

The user can select several entries in list with mouse and keyboard:
- `ctrl + left mouse` clicks to select entry (other selected entries are remain selected)
- `ctrl + space` to select entry (other selected entries are remaining selected)
- `ctrl + A` to selected all entries. If all entries selected, the entries will be deselected
- `shift + left mouse` clicks select all entries in row between the selected rows.

This function is not implemented in the TABs Optimization Manager and Output. Here only works the `ctrl + A` function.

### 6.3.6 Customized edge deletion

**1. Isolated glass unit**

We use the cutbacks (REUCKSCHNITT1...8) of the table SYSADM.BW_AUFTR_MODELL to create edge deletion. The user can enter the cutbacks in the AWB dialog (mouse click on spacer item [here orange]).

_Figure 65: Edit cutback in AWB_

The user can change the cutbacks in the green box. There is a default cutback on the position (BW_AUFTR_POS.REUCKSCHNITT) of the spacer (value yellow box).

The program uses the cutbacks of SYSADM.BW_AUFTR_MODELL. If the values are zero, we use the cutback of the BW_AUFTR_POS.REUCKSCHNITT table. We only write a -1 record to Opt2Fa, if the edge deletion/cutback is greater than the default cutback of the machine. You can set the default cutback of the machine in the aggregate dialog of AWB (see below).

**Next possible solution to set cutback:**
Otherwise, you could create a CU to add or change the cutback in the SYSADM.BW_AUFTR_MODELL table. E.g. If you use U-Profiles, you have to add a small value to the cutbacks.

Follow settings are needed to enable the feature:
You have to enable the feature on the aggregate dialog in AWB and check the orange marked check box:

_Figure 66: Enable edge deletion in AWB and set default cutback_

You should set the default cutback of the machine in the green marked text field.

**2. Single glass or laminated glass unit**

The user can use the AW Processing 1025 edge deletion for single glass or laminated glass. He has to add this processing on the single glass and the A+W Production Manager use these values as cutbacks.

You have followed restrictions:
- We only calculate the cutback from A+W catalog
- All segments of the shape have to be lines (no arcs). We do not calculate the cutback for shapes with arc segment.

You need the DB script: 20161014a.sql.
See case #376802.

### 6.3.7 New columns in table PROD_OPTI_STATISTICS

Here the new columns (all decimal (28,8), not null and default is 0):

- **OPTI_AREA**: Optimized area without residual plates and with trims
- **OPTI_COST**: Costs of OPTI_AREA
- **NET_AREA**: net area of the sheet (not of the circumscribing rectangle)
- **NET_AREA_COST**: Costs for NET_AREA
- **NET_QUANTITY**: Number of sheets
- **INVOICE_AREA**: Invoice area of the sheets from AWB (STL_QM_FAKT or PP_QM_FAKT columns in AWB tables)
- **INVOICE_AREA_COST**: Costs of INVOICE_AREA
- **REUSABLE_REST**: Area of residual plates
- **REUSABLE_REST_COST**: Costs of REUSABLE_REST_QM
- **WASTE_AREA**: waste area (includes sheet waste, trim area of jumbo, residuals not used)
- **WASTE_AREA_COST**: Costs of WASTE_AREA
- **BREAK_AREA**: area of the broken sheet (not of the circumscribing rectangle)
- **BREAK_AREA_COST**: Costs for BREAK_AREA
- **BREAK_QUANTITY**: Number of broken sheets

You need the DB script: 20161016a.sql.
See case #378569.

### 6.3.8 Save residual plates in AWB DB

If you click 'Book Stockplates' in the context menu of Optimization TAB, The Production Manager saves the residues plates in the AWB DB.

In AWB you can do the following:
- You could edit the residual plates in the AWB residual plates management (see next picture). You can only change values if the residual sheet is not used by an optimization (you will see this if the 'in optimization' field is 0).
- You can change the amount and other properties (See orange box).
- The field 'From Optimization' can be negative. Then we use a residual plate that was added manually by a user.

_Figure 67: residual plate management and edit amount of residual plate_

We only save the residual plates, if the plate is greater or equals a minimal width and a minimal height. You can edit the minimal residual plate width and height in the AWB master data of the glass article (See orange box):

_Figure 68: Edit residual plate width and height_

**For your information**
The default values for the minimal width and height are 9999 mm to have the old behaviour, where we do not save the residual plate.

The Production Manager writes the new residual plates in the DB, if the user Book the stockplates via context menu in the Optimization Manager TAB.

You will see the following residuals:

_Figure 69: Recognized residual plates_
The program recognized only residual plates which are ends on the border of the plate.

_Figure 70: Not recognized residual plates_
We will not detect any residual plates that are in the middle of the plate where sheets are on either side of the residual.

See new Parameter ID 22 to decrease the width and height of created residual plate.
You need the DB script: 20161005a.sql.
See case #378522.

### 6.3.9 Marking stepped drilled holes in cutting code

We mark stepped drill holes, too. The user can only add stepped drill holes and the drill holes for the sheets will be marked in the cutting code.
See 6.8 for implementation.

### 6.3.10 Print cutting labels via machine driver

1.  You have to add the machine IDs in the category 'Labels from cutting machines' in the Production Manager Config Tool (new parameter ID 23). Look at the orange rectangle in the next picture:
    _Figure 71: ConfigTool Settings for cutting labels via driver_
    In the `Cutting machine labels` section, you can specify machine IDs for `Print label.dat for cutting machine driver` and `Print PrintCuttingLabels.pdf for cutting machine driver`.

2.  You have to add 2 reports to the AWB report directory. The reports are known as:
    - **LabelDat.rpt** (Bottero, Macotec need only this report)
    - **PrintCuttingLabels.rpt** (not every machine needs this report. E.g. Turomas, Hegla need this report.)

    **Note:** Every machine could have a own PrintCuttingLabel.rpt named `PrintCuttingLabels[AggregateId].rpt`. E.g. if the machine ID is 1000, the name of the report file has to be `PrintCuttingLabels1000.rpt`.

    If we support a new machine and there is no information about this machine in this document, you can look for this in the Market Solutions document:
    `\\jupiter\Doku DocuWare\MarketSolutions\AUW_Configuration cutting.docx`

    It could be that you need the new Cutting Driver Batch. IF you need a new one, you have to ask DLA for this batch.

You get the AWB Report directory in the master data. Look at this picture and check the green box:

_Figure 72: Master data report location_
The path is configured under `Master Data` > `Firma` > `Firmendaten`, in the `Primary form-/report-search Path` field.
Example: `C:\Program Files (x86)\A+WALFAK 2012\Report\`

Now, we write some data for the cutting label printing via machine driver. We write 2 new files in the cutting driver path:
- `Label.dat`
- `PrintCuttingLabels.pdf`

We write an Opt2Bar file to the optimization save file. The machine driver needs the Opt2Bar file for cutting label printing (barcode and optimization order of sheets).

If the user adds some sheet via PlanEdit, we write follow for the sheets to the Opt2Bar file:
- Order number = -2
- Item number = -1
- Barcode is an empty string

The Turomas cutting table requires both reports and generates from the `PrintCuttingLabels.pdf` report a `.prn` file (that's the binary file format of the Hermes printer).

The Hegla cutting table also requires both reports. But Hegla needs only the real pdf output and not a prn file like Turomas.

For the Turomas cutting table, you need the following tools (see next chapter 7.3.10.1)
- The CAB Driver for Hermes printer
- Multi File Port Monitor (mFileMon)
- PDF Reader/Viewer Adobe or Foxit Reader

#### 6.3.10.1 Reports

##### 6.3.10.1.1 LabelDat.pdf

`LABEL.DAT` is a text file generated by Crystal Report `LABELDAT.RPT`. This report generates a section of data for each barcode. Each section starts with the following line which is needed to identify the section `[CuttingDataProviderSection][{Number of Machine}][{Barcode}]` and it ends with `[EOS]`.

Our drivers currently support the keyword `CuttingDataProviderSection`. New drivers or other applications in the future will possibly support other keywords.

The section contains a list of individual parameters in the following format:
`< {Name of parameter}="{Parameter Value}">`
This format could be different for individual drivers, currently we have only one driver which uses this format.

Here is an example from A+W Business Pro:
```
[CuttingDataProviderSection][1000][T200020630001000]
<ORDERNO="20630"> <ITEMBNO="1"> <BOMID="0"> <JOB="1004">
<OPTIMIZATION="8"> <QUANTITY="5"> <SHAPENO="0">
<COMMISSION="Kommission A"> <CUSTOMERITEM="KDPOS A">
<DELIVERYDATE="30.06.2017"> <BARCODE="T200020630001000">
<PRODUCTNO="104"> <PRODUCT="Float 4 mm A+W">
<CUSTOMERNO="1070"> <CUSTOMERNAME="Becker Glasbau">
<WIDTH_CUT="1.700,00"> <HEIGHT_CUT="1.800,00">
...
[EOS]
```
This file can be used for every cutting code driver, maybe in future also to send additional information to the cutting code driver. Actual (v6.3 and v6.4) it is used only for the label print feature of the BOTTERO or Macotec cutting code driver.

##### 6.3.10.1.2 PrintCuttingLabels.PDF

In the `PrintCutting.PDF` you provide real labels, one label per page and one label for each barcode in the optimization.

_Figure 73: LabelDat.pdf report_

Each page must have a hidden control field containing the barcode number:
`@@BARCODE={Barcode}@@`

The cutting code driver splits the PDF into one page for each barcode and builds a new PDF for each path.

#### 6.3.10.2 Configuration of Turomas cutting tables

After generate the cutting code driver with `Albwir.Xoptc.Turomas.exe`, execute the additional tool `TuromasLabelProcess.exe`. This tool uses the same configuration file, `Turomas.config`, and is working if `OPT2BAR` and `PrintCuttingLabels.PDF` exist beside the generated cutting code.

For each pattern in the cutting code a file `<CuttingCodeName>_<PatternNo>.POS` and `<CuttingCodeName>_<PatternNo>.PDF` will be generated. The PDF file contains the labels from `PrintCuttingLabels.PDF`.

After this the generated PDF files per pattern will be convert into a PRN file. A PRN file is the file format which is generated direct by the printer driver. In this solution the printer driver generates his output direct into a file. The generated PRN file will be renamed into `<CuttingCodeName>_<PatternNo>.PRN` and is part of the package of cutting code and .POS files. The PDF file isn't need anymore and the files will be removed if the conversion was done fine.

The conversion into PRN file is not so easy, you need some tools and some configurations:

*   **Hermes CAB Windows printer driver**
    Turomas uses CAB Printer, e.g. Model Hermes+ 4L/300. Download the right printer driver and install it on the Server where you generate cutting code. Configure the printer driver, generate a label format with the size of the used label and set this format as default, maybe it is need to set this as default for each windows user. The Crystal Report `PrintCuttingLabels.RPT` has also to be generated and stored with this printer driver and the same label layouts you use on the server during cutting code generation. The same technic we use if we generate normal labels with Crystal Reports. The name of the printer has to be configured in `Turomas.config` parameter `<Printer>`.
    ```xml
    <PRINTER>CAB Hermes+ 4L/300</PRINTER>
    ```

*   **PDF Reader**
    We support ADOBE or FOXIT. One of the readers has to be installed and which is used has to be configured in `Turomas.config` in the parameter `<ReaderType>` :1 = ADOBE, 2 = FOXIT. Our driver opens the PDF in the reader and print them on the configured printer. The driver also closes the PDF reader if the PRN file was generated. This can take a while so you have to configure some timeouts in milliseconds if nothing happens in the parameter `<WaitForPdfReader>` and `<WaitOpenFile>`.
    ```xml
    <ReaderType>1</ReaderType>
    <WaitForPdfReader>10000</WaitForPdfReader>
    <WaitOpenFile>2000</WaitOpenFile>
    ```

*   **Multi File Port Monitor**
    The freeware tool Multi File Port Monitor is needed (https://sourceforge.net/projects/mfilemon/). The tool is in the AUW Turomas package in the Tools subdirectory or it can be downloaded.

Install the tool and configure a printer port for the Windows printer driver and set the output in the driver fix to this port. If you do this, the driver doesn't print on a physical printer, it prints the result into a file. We can't use the Windows standard printer port FILE, because in this function you have to enter an output filename every time you print and with the Multi File Port Monitor you can configure the filename.

1.  In **Devices and Printers** mark a printer and open in the **Printer server properties** the tab **Ports** and **Change Port Settings**.
    _Figure 74: Configure CAD Hermes printer for Turomas cutting table_

2.  Add a new Port from type **Multi File Port Monitor**. We recommend as port name `PRNFILES`.
    _Figure 75 & 76: Configure mFileMon Port for Turomas cutting table_

3.  Configure the **Output path** and the **Filename pattern** for this port.
    _Figure 77: Settings for mFileMon_
    *   **Output path:** `C:\TEMP` (The path must be fixed, UNC path possible but variables e.g. `%APPDATA%` doesn't work. The user needs read and write rights.)
    *   **Filename pattern:** `PrintCuttingLabels.%u.%c.prn` (This generates a file with user name and computer name, making it possible to generate cutting code on one Server from different users.)

4.  In the next step allocate the new port to the Turomas printer. Open the **Printer Properties** and in tab **Ports** select the new port `PRNFILES`.
    _Figure 78 & 79: Open Printer properties and set PRN Port_

For testing the configuration open a PDF document in your PDF reader and print the document on this printer. After this the PRN file should be generated in the configured output directory.

You must configure the same output path and file pattern in the `Turomas.config` in parameter `<TempPrinterFile>` as configured in Multi File Port Monitor. The placeholder `%u` and `%c` works in both file pattern.
```xml
<TempPrinterFile>C:\Temp\PrintCuttingLabels.%u.%c.prn</TempPrinterFile>
```

##### 6.3.10.2.1 Turomas.config

In the `Turomas.config` the parameter for the label print function are configure in section `<Label>`. Here an Example:
```xml
<Label>
    <WaitForPdfReader>10000</WaitForPdfReader>
    <WaitOpenFile>2000</WaitOpenFile>
    <ReaderType>1</ReaderType>
    <Printer>CAB Hermes+ 4L/300</Printer>
    <TempPrinterFile>C:\Temp\PrintCuttingLabels.%u.%c.prn</TempPrinterFile>
</Label>
```

#### 6.3.10.3 Configure the Bottero cutting driver

BOTTERO generates and print the Labels with his own applications, but they need several information for the sheets in the cutting code to print them on the label. The information we prepare in the `LABEL.DAT`.

The driver `BotLabelProcess.exe` must be execute before `XCBOTHPS.EXE` and it search in `LABEL.DAT` for packages with the following syntax:
```
[CuttingDataProviderSection][{Maschin ID}][{Barcode Number}]
<{Name of Parameter}="{Parameter Value}">
...
[EOS]
```
The Output is the file `BotLabel.TXT`. The cutting code driver `XCBOTHPS.EXE` uses this file if it exists and inserts the information into the cutting code. The complete text between the header line and `[EOS]` will be used and convert into one line. Special character like line/page break will be removed.

### 6.3.11 Crystal report Runtime 13 (#399962)

We could use the Crystal Report (CR) Runtime 13 since Version 6.4. The old (CR) Runtime version 12 works, too. The old CR Runtime version will be used, if the new CR Runtime version not installed. That's the fallback. Check AWD case #399962.

### 6.3.12 Notes about shape 770, 771, 772

There are no FRM files for these shapes. You have to create SN files for the shape. The shapes will be handled as shape 99 in the Production Manager program.

### 6.3.13 Refinements in Hotfix 898, 915, 952, 980

- Faster breakage loading, if you open the breakage dialog
- Faster job item search in wizard/standard mode (= faster job creation and less memory needed) (since version 915)
- Save the same job items in wizard mode like in standard mode. The wizard mode saves only scheduling item at previous version.
- Marking rounding corners (see Parameter 18)
- If the user optimizes jobs in the Optimization Manager, the program checks the items which will be written to PROD_JOBITEMTEMP table. If there are no items to write, the program cancels the optimization.
- If the user saves optimizations in the Optimization Manager, the program checks if their item in the PROD_JOBITEMTEMP table. If no item in the table, the program does not save the optimizations.
- New DB Script: 20171201a. This script contains an update for table PROD_SHAPETRIM. Follow shapes will be added: 200, 201, 770, 771, 772, 773, 801, 802, 803, 804, 807, 808
- Faster loading of optimizations in Optimization Summary Tab (since version 950)
- For some database queries, capitalization is not heeded (since Version 952).
- We fixed a memory leak. The List Controls do not remove the added function pointers. That is solved and the List Control needs less memory because there is no memory leak (since version 980)

### 6.3.14 Feedback from Realtime Optimizer (RTO) to AWB to discount stockplates in AWB (#407260)

You have a cutting table with a Remaster. Then the RTO has to write PRODBAZ files and the AWB read the PRODBAZ files to discount the stockplates, set status from AWB orders.

#### 6.3.14.1 AWB Configuration

You need to install the latest AWB and AWB SQL script: 20180126a.

You have to set the follow check box in AWB:
In the aggregate settings (`Capacity planning` > `Aggregate`), check the `ReMaster / RPS` box.

_Figure 80: Set the Remaster for RTO/Cutting table_

The AWB interface service have to handle the ProdBaz file from the RTO (see the Installation Docu from the AWB Interface Service 1.12). You have to activate the XTV Workflow and enable AWB to read ProdBaz files (see AWB Config Docu for further details 7.4).

You have to add the ProdBaz directory in this dialog (Red marked. You find this dialog in Production settings under `Master Data` > `Company` > `Data Tab 13. Production`). Press 'Settings' to open the dialog.

_Figure 81 & 82: Set ProdBaz file path for RTO_
In the `Import XTV reports` section, set the file path, e.g., `C:\Trans\Prod\TB1\` for `(PRODBDA*.*)`.

#### 6.3.14.2 RTO, AWB Pro Configuration

You have to set follow in the RTO config file (`xopton.cfg`):

1.  RTO writes no feedback file for residual plates at the moment. No sheet information (Order/Pos) will be passed to AWB for residual plates. A new flag “ResidualPlates” will be added to the section `[FeedBackFile]`. For `“ResidualPlates=Y"` a feedback file will also be written for residual plates. AWB will not find the stockplate size and has to ignore it. AWB will only use the “Order/Itm” information of the sheet records.
2.  You have to set the `WriteSheetRecord=Y` in section/partition `[FeedBackFile]` to write the sheets into the feedback file. Then we can set the state of the order in AWB.
3.  AWB Pro needs the status information ("Cutting started" and "Cutting finished") for each imported save file (ZWB optinumber). A new section `[BusinessProFeedback]` will be added to the `XOPTON.CFG`. With the entry “FeedbackFilePath” a path can be configured which is reachable for the RTO and AWB Pro. The “FeedbackFilePath" has to be the same like the aggregate Output Directory in AWB settings `Capacity Planning > Aggregate > General`.
    _Figure 83: Set the Remaster for RTO/Cutting table_

When the RTO starts cutting an AWB Pro optimization or the AWB Pro optimization is reoptimized in a tableoptimization the RTO writes an empty file (Name=AWB Optinumber Extension=state). Example: For optinumber=1956 the filename will be "1956.300” (1956=AWB Pro optinumber / 300=Production started). If the optimization has been completely cut the RTO will write a file "1956.700" (1956=AWB Pro optinumber / 700=Produced). Then the A+W Production Manager sets to the optimization status to 700 (=released) and releases the reserved stockplates of AWB Pro. The 'Book Stockplates' context menu is deactivated on the Optimization Summary tab in the Production Manager.

**AWB configuration:**
You need the call of the function `udf_ReadFeedbackFiles()` so that the exchange service knows where it can read the feedback files and import them into the database under `A+W Business > Master Data > Import Customizing`.
And you need the call of `udf_ProcessXTV()` to process the data imported.

The A+W Production Manager reads the `*.700` file and sets the status of the stockplates, optimizations, and optimization statistics to booked.

You can send the status finished cutting to A+W Business automatically with the A+W Production Manager. Please, check the ParameterID `27` at config tool.

#### 6.3.14.3 Optimization statistics

The `PROD_OPTI_STATISTICS` is not correct for changed optimization by RTO. The table contains the old optimization data from the Production Manager. The Production Manager do not update the entries. You have to use the AWP tables `xopt_optimierung` and so on in this environment.

#### 6.3.14.4 A+W Production Manager

The user could not book stockplates in the Optimization summary tab, if the Remaster setting active on the producing machine. The entry on the content menu (Book stockplates) is deactivated. The Context menu entry is enabled if one or more optimizations were produced on a machine without Remaster. The Production Manager only books only the stockplates for optimization produced on a machine without remaster.

The optimization state in `PROD_OPTIMIZATION` and `PROD_OPTI_STATISTICS` are only set to Booked, if the optimization produced on a machine without remaster.

The A+W Production Manager reads the `*.700` files and books the plates and sets the status to booked with a background process. The user doesn't have to do anything. There is nothing to configure on the Production Manager.

We implemented a new context menu entry in the Optimization Summary TAB. The entry bears the name 'Update.' If the menu entry enabled, the Production Manager read one or more `*.700` files and make some database updates. If the menu entry disabled, there is no new data. The menu entry is only shown, if there are a XOpton with a remaster.

The Production Manager shows a message in the Status Bar (where the Program and Database Info is shown), if there are new data.

### 6.3.15 Fix some issues 417027, 416756, 417132, 416887

#### 6.3.15.1 #417027: Booking stockplate error. Sheet is not placed in the cutting state

If in the optimization there are sheets with different PO numbers, not all sheets will be booked in the cutting status. Now we will book all sheets correctly.

#### 6.3.15.2 #416756: Hardware products/articles in the order selection

If you are seeking sheets in the order selection, the tab also displays hardware products/products. Now we do not show this item.

#### 6.3.15.3 #417132: Bavelloni cutting machines (MTS, MTL) supports optimization numbers larger than 3 digits.

That was fixed at the machine driver `xcbavshp.exe`. The driver will be deployed by the A+W Production Shared Folder Setup. The new driver has the version 13.0.178.1 from 23.02.18.

#### 6.3.15.4 #416887: faster GetFRM

The GetFRM assembly is faster now. It should be 2-3 times faster. The creation of batches is faster since the creation of batches uses the edge correction and shape detection. The GetFRM assembly will be deployed by the A+W Production Runtime Setup.

### 6.3.16 Archive reports as pdf

If the batch has been optimized, we were able to save all order and optimization reports and labels on the hard disk. The base archive folder is the AWB file attachment path from the AWB master data (red marked in the next picture). That is the default path:

_Figure 84: File attachment path at AWB master data_
`Master Data` > `Company Data` > Tab `8. Archives`. The path is set in the `File attachments` section. Example: `\\localhost\Trans\ERP-attachment\AWB\`

You can change the base archive Folder path at the Config Tool. See parameter 25.

Then we add the relative path `\ProdMan\Archive\` to the master data path. That's the base path for every batch. We add the year and month (double digit, leading zero, if necessary) to the path. The path for one batch is:
`'File attachments path' + '\ProdMan\Archive\' + 'Year\Month\' + ‘JobNumber'`

For example:
`'File attachments path' + '\ProdMan\Archive\2018\08\1234'`

_Figure 85: Archive reports at Production Manager_

The orange marked button (`Speichere Reports`) and context menu saves the reports to disk. You have to selected least one batch with status optimized or higher.

The green marked context menu (`Öffne Reportarchiv`) opens the archive folder. We opened the base folder if the user selected more than one job or the user select no job.

If the user selects one batch with status optimized or higher, we check if there a directory with the job number and open the directory with the job number, if it exists. Otherwise we open the base folder.

**For your information:**
- If the reports exist on disk, we override them.
- Please, use the crystal reports for the optimization result and optimization pattern report because if you not use these reports, we use the PlanEdit print export and this export needs a user input for saving.
- Each batch report or each label has the batch number as prefix (e.g. `2062_795_LGUProductionList.pdf`).
- Every optimization report or label has the job number + '_' + optimization number as prefix (e. g. `2062_795_ListOfStockplate.pdf`)

### 6.3.17 New Job Status at Job Status dialog

We can set a new job status 'Produced' at Job Status dialog.

_Figure 86: Setting Job Status_

You change the job status at the orange marked combo box (`Neuer Laufstatus`). If you set this status, you can mark the job as produced but the job will not be archived. The next status is ‘Released' and then the AWB archiving workflow works.

### 6.3.18 Residual plates size not correct (420104)

We calculate the residual plate size not correctly. That issue is solved with April 2018 setup/release.

### 6.3.19 Add supplier info

We have to execute the SQL script 20180614a to switch on the feature.

You can open a new dialog under optimization summary TAB via the context menu:

_Figure 87: Open supplier info dialog_

The dialog shows like this:

_Figure 88: supplier info dialog_

You select some rows and add a text into the green marked box (`Supplier Info`). Press the red button (`Apply Supplier Info`) and the program adds the text to the last column.
- **Ok** save the data to database.
- **Cancel** do not save the data.

### 6.3.20 New filter criteria at optimization summary TAB

You can show only optimizations with job, which status is smaller than produced and released.

You have to uncheck the green marked check button (`Show Produced or higher status`) (checked is the previous behavior):

_Figure 89: Status criteria at optimization summary tab_

### 6.3.21 Default PDF printer to show Optimization Result and Pattern report on screen from PlanEdit

We have changed the behavior:

1.  We try to find the `maxx PDFMailer` printer. If we find this PDF printer, we use this PDF Printer for PlanEdit reports to show on screen. We search after the printer name “maxx PDFMailer".
2.  If we do not find this PDF Printer, we use another PDF printer. We use the first printer, which contains "PDF" in his name. That's was the old behavior.

You should always install the maxx PDFMailer printer. Then you get no FileSave Dialog to save the PlanEdit reports.

### 6.3.22 Mark macro processings

We can mark macro processing. You have to set the mark drill hole and cut-out parameter (6.8 and ParameterID 18) because the program does not know the content of the macro. The macro could contain drill holes and/or cut-outs.

### 6.3.23 Some hints for specials shapes 901 and 902

Let's take a look at the 2 shapes:
_Figure 90: Shape 901 and Shape 902_

> **Do not use** the shapes in the AWB entry. This cannot work since the shapes have more than 8 edges.

Some hints for AWP and **not** AWB Pro:

The shapes 901 and 902 only work with a product of the insulated glass unit (IGU). You cannot add some steps, edge processings or other inner cut-outs, border cut-outs, corner cut-out and corner processing. Heed the restriction of the A+W Production system (AWProduction):

- We have no shape recognition since we cannot detect the inner cut-out and would detect shape 0.
- We ignore steps and edge processings.
- No marking of drilled holes, inner cut-outs or corner processings on the cutting table
- This makes sense if the customer has a Bystronic cutting table and a Lenhardt IG line.

The A+W Bystronic cutting table driver can cut and delete the edges of these special forms (also inner cut-outs). The Lenhardt line can produce the frames. It is model 91 in the Lenhardt shape catalog.

You have to change the spacer report. We do not calculate the spacer segment length from the inner cut-out since the shape detection detects the shape 0. We calculate the spacer only from the rectangle/shape 0 (outer contour).

You can enter this `XL_JobRelease.cfg` entry:
```ini
[XL_SHAPE_CATALOG]
;#253779 implementation shape 901
ConvertSpecialShapes=Y
```
Then the shapes 901 and 902 will be produced as shape 0 (rectangle); otherwise as shape 98 (Lisec free shape).

### 6.3.24 February Release 2019

1.  Edge correction at aggregate assignment was not correct. We have corrected this.
2.  Use Crystal Reports for cutting results and cutting pattern in PO mode and do not print with PlanEdit or a PDF printer.
    - You need the `Prodman_OptimisationResult.rpt` and `Prodman_OptimisationCuttingplan.rpt` report.
    - You have to add the reports at the AWB masterdata. The `OptimizationResult` has the ID 826 and the `CuttingPlan` has the ID 830.
3.  Print archive reports at background in Job summary control. User could work further with the program but he cannot enter the job or optimization output control and cannot enter the wizard mode.
4.  Background printing is used in the output tab with the same restriction at 3).

### 6.3.25 March release 2019

1.  **Filter and search short keys**
    The user can press `enter` (instead of pressing the search button) to search data in job summary, order search, optimization summary and job information TAB. The filter button has the short key `Ctrl+Alt+A` or `Ctrl+F`. `Ctrl+A` is used by the list controls to select all entries.

2.  **Obsolete script in v12.5**
    Do not install script with name: `20180614a` at v12.5. The new column `SUPPLIER_INFO` only works in v6. We made a new script for v12.5 to solve the issue: `20190307a`.

3.  **ConfigTool warning**
    Config Tool is warned if the batch number range overlaps the breakage or quotation number ranges. The config tool shows a warning if:
    - Job number and breakage job number overlap. You can reduce the job number range to 8999. Check whether some batch numbers are in the range of the breakage batch number.
    - Batch quotation and batch number overlap. You can adjust the number range of the quotation. Check whether some batch numbers are in the quotation job number range.

4.  **Delete block file entries**
    There is a new Ribbon to make some internal and environment work.
    _Figure 91: New ribbon TAB_
    The first and only entry is 'Remove Entries' from block file. If you press the button, you see this dialog:
    _Figure 92: Delete block file entries dialog_
    You can set a time in days (`Einträge älter als löschen [Tage]`). If the block file entry older, the entry will be removed. The program reminds the last setting of the days.
    It will be only delete entries with follow naming:
    - Starts with prefix ';-)Shape99_' (=nested shape from ShapeOpt)
    - The name matches `OrderNumber_PositionNumber_Bomld` (= Blockexport from ProductionManager)
    - The name matches `OrderNumber_PositionNumber_Bomld_AggregateID` (= block export from AWB Production Terminal)

### 6.3.26 Write Muntin section in AWISO.dat for TFB Bender driver to make drilled holes for muntins in the spacer

**Restriction:** The muntins have to be below the spacer item at AWB order entry.

_Figure 93: Place of muntins at AWB order entry_

You have to add the muntin to a spacer in muntin/georgian bar entry. We have to use the red marked combo box for spacer selection. The green marked button adds the muntin/georgian bar to the other spacers and all spacers contain the same muntin/georgian bar.

_Figure 94: AWB muntin entry_

- We only support the TFB bender driver (driver number 13) at the moment.
  - `13 = TFB`
  - `= XL_ISO_TFB_0`
- You have to set the `FormatVersion` in the driver section at `XT_AWISO.cfg` file to `2.00` e. g.
  ```ini
  [XL_ISO_TFB_0]
  FormatVersion=2.00
  ```

### 6.3.27 Partial deliveries in AWB (#444661)

You need the database script `20190603a` to use the function.

If a customer makes partial deliveries in AWB, the AWB deletes the entries in some database tables (BW_AUFTR_*). The AWB sends us the job number and we marked the job as Partial delivered (new column in `PROD_JOB` table `PARTIALDELIVERED`, Not null, int, default is 0). The column `PARTIALDELIVERED` is 0, if not partial delivered; 1 = PARTIALDELIVERED.

If the job is partial delivered, the user cannot do:
- any output (job and optimization)
- Resolve batch
- Resolve the optimization
- Edit the optimization
- Archive batch
- Aggregate assignment
- Show detailed job view

**Restrictions at Production Manager:**
- The user has to print the job and cutting reports and labels reports and create all bender and cutting code before one order is partial delivered.
- If the user needs labels for the partial delivery order, he has to make a job with the partial delivered order. Then the user can print labels. The user has to release the job because of the achieving.

### 6.3.28 Selected plate as first plate in optimization (#449810)

The user can use the priority value for special selecting. If the user enters a negative value, the plate will be used as first plate at the optimization. The user can only enter one negative priority value in the stockplate dialog. That means only one plate could be used. The plates get a green ball (blue ball means stockplate; yellow ball means residual plate) at second column.

### 6.3.29 Support of bended IGU and LGU (#450801)

We cut the correct cutting size at cutting table, if the glasses will bended.

Follow restrictions:
- It works only with shape 0
- You cannot edit the shape number and parameters with the cutting edit dialog

### 6.3.30 XTV Mode (#451823)

You can start the Production Manager in an XTV mode. The program starts only with the last 2 tabs (Optimization summary and Output).

_Figure 95: XTV Mode_

The user cannot resolve, edit, save optimizations with the context menu at optimization summary tab. The output tab is not changed.

_Figure 96: XTV mode optimization summary context menu_

If the user presses 'Detailed view' at context menu, it opens a new window with the pattern list and pattern picture of optimization. This dialog is modal and opens in full size. The user can select the next the pattern with the controls `Space`, `Arrow down`, `F12`. If the user wants to select the previous pattern, he has to press `Shift+Space`, `Shift+Arrow up` or `Shift+F12`. The window closes, if the user presses escape (ESC) button.

_Figure 97: XTV detail view windows_

The Production Manager starts in XTV mode, if the user belongs to the ‘XTV' (case sensitive) group. You can edit the setting in the AWB. See the following figure:

_Figure 98: Set group for AWB user_
In `Master Data` > `Employees` > `Specification`, set the `Group` to `XTV`.

### 6.3.31 Changes in September 2019 release

#### 6.3.31.1 New assemblies in Setup

The Production Manager deploy all assemblies, which are needed to run. There are new assemblies in the setup:
- Get99.dll
- GetFRM32.dll
- The native logging dlls: Log4cxx.dll and AWSOA.Core.Native.dll

#### 6.3.31.2 Faster batch creation and detailed scheduling

We load the data (glass article, capa properties, edge processing data, etc.) only one time from the database and not every time and sometimes in for-loops. This makes batch creation and the detailed scheduling faster.

#### 6.3.31.3 Minimized ribbon bar

_Figure 99: Minimized ribbon bar_

The user can minimize or maximized the ribbon bar with the red marked button.

#### 6.3.31.4 Rack numbers with more than 4 digits and ACLIM_BOCK_FACH in label.set

The opt2dat contains the ACLIM_BOCK_FACH at character host field. The default is 2 and means that the last 2 digits from the rack number is the slot number at harp rack.
E. g. the ACLIM_BOCK_FACH is 2 and we use a harp rack:
Rack number 30056 means slot 56 at harp rack 30000.

#### 6.3.31.5 Tool tip with information about batch, breakage, optimization number range, etc.

If the user moves the mouse pointer over the batch or the optimization labels/text, a tool tip can be displayed. The text of the tooltip always follows the format: `1000 - 8999 (4711)`.
- **1st number (1000):** minimum job, breakage, optimization number
- **2nd number (8999):** maximal job, breakage, optimization number
- **3rd number (4711):** current job, breakage, optimization number

_Figure 100: Tooltip about number range_

### 6.3.32 Changes in November 2019 release

- **ParameterID 28:** Keep float glasses together at same rack if the shape is a shape 99 and an IGU/LAMI.
- The Production managers calculates the correct cutting rectangles of shape 99 and show the right cutting rectangles at order summary tab.
- **#453238 New formula variables 6.6**
  - Machine1AfterCutting
  - Machine2AfterCutting
  - Machine3AfterCutting
  - Machine4AfterCutting
  - Machine5AfterCutting

**What the difference to Machine1, Machine2, ..., Machine5 variable:**
The Production Manager has the variables Machine1, Machine2, Machine3, Machine4 and Machine5. These variables contain the machine number of the First, Second, Third, Fourth and Fifth processing machine after cutting. The problem is that the same machine can participate in several processings and our goal is to identify individual and unique machines after the cutting, and we have to ignore doubled machines for the processing sequence.

### 6.3.33 Barcoding - unique label identification per glass (#439200)

Now you can create barcoding for the individual identification of glass.
With the current process of glass manufacturing, a single barcode is used for all BOM items.

In order to work with this setting, please insert the value of the last barcode in the Production Management Config Tool:

_Figure 101: Barcode number setting_

The pre-set minimum value is 1000 and the value increases with each newly created barcode. The maximum value for the barcode is 9223372036854775807. It is expected that a barcode with 19 digits is the typical maximum. Barcodes with 20 digits up to the maximum value are also possible, however.

Information about the parameter in the configuration is also under the settings of `PROD_PARAMETER` chapter 5.9 in the new field number 29.

**How is the unique label ID per glass generated?**
As soon as a new job is created, the associated orders receive the START_BARCODE for the products of the type single glass, LAMI glass, and IG, as well as the entire BOM for these products. All of this happens in the background.

After the order goes into production, the labels are printed with the new single glass barcodes. Important is that the labels are printed with one label per product.

The labels affected by this change are the following:
- Labels for the optimization
- Labels for the batch

_Figure 102: Affected labels during the label detection_

After this change, each label that is a single label per product, has the unique barcode per glass.

### 6.3.34 Production racks [AW-59393]

You need the database script `20210114a` to use the function.

The "AWB Barcoding" now has information about the physical rack (production rack) on which the glass is located after booking of the label. Thus it is possible, if someone is seeking a particular glass in production, to locate information about on which physical rack it is located.

The management of the production racks is developed as part of the "AWB Advance Barcode" module. At the moment, "AWB Advance Barcode" consists of the unique barcode label per glass. (T1 + "Glass Barcode")

To define the production rack, we use the existing rack management in A+W Business. The production racks use the same barcode pattern as the dispatch racks: `GE + "rack number"`

#### 6.3.34.1 Set-up of the racks in A+W Business (rack management)

The rack management in production now allows the selection of the rack type; you can choose between dispatch, production, and mixed racks. A mixed rack is a rack that is available both for dispatch and production.

#### 6.3.34.2 Completion report (Business Scanner)

After the production racks are set in rack management, you can book a glass on the scanner with a selected rack on which first the production rack is set on the completion report dialog with the `GE + "rack number"` barcode and then the glass label scanned.

#### 6.3.34.3 Options on the rack menu (Business Scanner)

On the "Racks" menu of the scanner program, the following new options have been added to manage production racks:

*   **Unload Rack**: This option is already available for dispatch racks and is also used for production racks.
*   **Display Rack**: This option is already available for dispatch racks. In case of production racks, however, the information is expanded to: sequence + order + article + customer number + width + height.
*   **Search for order**: The idea is that the user can enter the order, the element, and the BOM_ID and the scanner returns the physical rack that matches the search criteria.
*   **Reallocate Rack**: This option is already available for dispatch racks. Sometimes, the entire content of a rack is shifted to another rack. With this option, two bookings must be made: on the source rack and on the target rack in order to update the value for the rack in the table "BA_GESTELLE_AUFTR".
*   **Reallocate unit**: Frequently after a mistaken booking, a single glass is shifted from one rack to another rack. With this option, the barcode of the individual glass, the source rack, and the target rack are used in order to update the rack booking in the table "BA_GESTELLE_AUFTR".

#### 6.3.34.4 Booking history

In the booking history, a new field called "Rack" is displayed, with a search field.

