---
description: "EN CONFIG A+W Production MachineControl"
---



# EN CONFIG A+W Production MachineControl

         Configuration


A+W Production Machine Control




                                                                      english




   A+W Software GmbH                                          - -INTERNAL-
                       EN-CONFIG-A+W Production MachineControl.docx   1
CHANGE HISTORY


           Date          Author:                 Remarks                                 Version
                                                 Cutting, GeorgianBars,
           2018-05-18 DLA                                                                1.0
                                                 ProcessingMachines, Bender Sealer
           2018-07-30 DLA                        Processing machines SN                  1.1
                                                 Add 3 SN processing parameters
           2018-08-01 T.H. Schmidt               (Driver settings, Standard driver, SN   1.2
                                                 Command)
                                                 Modify chapter “Labels with INTERMAC
           2018-10-08 DLA                                                             1.3
                                                 OTD”, Laser marking
           2018-10-11 DLA                        FORVET KEY                              1.4
           2019-11-26 EB                         Turomas                                 1.5




Content

1.   Cutting table                                                                              5
     1.1. Configure cutting table in A+W Production                                             5
          1.1.1. Integrate Cutting Table into JobRelease                                        6
     1.2. Configure cutting table in A+W Business Pro                                           7
     1.3. Configuration of cutting code driver                                                  9
     1.4. List of cutting code driver and their characteristics                                10
     1.5. Cutting Code with Label Print                                                        13
          1.5.1. LABEL.DAT                                                                     13
          1.5.2. PrintCuttingLabels.PDF                                                        14
          1.5.3. Configuration A+W Business Pro                                                15
          1.5.4. Configuration A+W Production                                                  15
          1.5.5. Labels with Turomas                                                           16
          1.5.6. Labels with BOTTERO                                                           19
          1.5.7. Labels with HEGLA                                                             20
          1.5.8. Labels with OPTIMA                                                            20
          1.5.9. Labels with INTERMAC OTD                                                      22
     1.6. Laser marking                                                                        24
          1.6.1. Variant without SN file                                                       24
          1.6.2. Variant with SN file                                                          24
     1.7. Troubleshooting                                                                      26
          1.7.1. Circle troubles on INTERMAC (XCAWCUT)                                         26
2.   Cutting Table via A+W Realtime Optimizer and CutTV                                        27
     2.1. BYSTRONIC                                                                            27
     2.2. LISEC                                                                                29
     2.3. HEGLA                                                                                30
     2.4. BOTTERO                                                                              31
     2.5. BILLCO                                                                               32
     2.6. TUROMAS                                                                              32
          2.6.1. Initial settings (AUW_Configuration_cutting.docx)                             32


A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                             2
         2.6.2. RTO label                                                     32
         2.6.3. Installation and settings for PDF24 application               33
         2.6.4. Configuration of “lblprinting.bas”                            36
         2.6.5. Configuration of cutting.bat                                  36
         2.6.6. Settings for “Turomas.config”: Field Digit job ID             37
         2.6.7. New Batch “PostCut.bat”                                       37
3.   Bender and Sealer                                                        39
     3.1. Configure bender and sealer in A+W Production                       39
          3.1.1. Integrate bender/sealer into Release                         40
          3.1.2. Configure bender texts                                       41
     3.2. Configure bender/sealer in A+W Business Pro                         42
     3.3. Configuration of bender and sealer driver                           44
          3.3.1. Process create machine code old driver                       44
          3.3.2. Process create machine code new driver                       45
          3.3.3. Converting spacer type and spacer colour in machinery code   45
          3.3.4. Converting gas type in machinery code                        45
          3.3.5. Specialties of individual drivers                            46
     3.4. Configure Sealer in A+W Production Terminal IG-IN                   48
     3.5. Configure Sealer/Bender in JobTV                                    49
     3.6. Troubleshooting                                                     50
4.   Georgian Bars                                                            52
     4.1. Report                                                              52
          4.1.1. Print direct with A+W CAD Designer (Bars)                    52
     4.2. AWD file generation                                                 53
          1.1.1. Configuration until version 5.5                              53
          1.1.2. Configuration since version 6.0                              54
     4.3. Machine control from A+W CAD Designer (Bars)                        54
     4.4. Machine control from XLCLASS                                        56
5.   Processing machines (XL)                                                 58
     5.1. Processing machine in A+W Production                                58
          5.1.1. Configure machine type 103                                   58
          5.1.2. Configure processing machine                                 59
          5.1.3. Configure XL_JOBRELEASE.CFG                                  60
          5.1.4. Processing master data                                       61
          5.1.5. Configure machinery allocation                               61
          5.1.6. Configure detailed scheduling                                62
          5.1.7. Configure JobRelease                                         64
     5.2. Machine control via A+W Production Terminal                         64
          5.2.1. Example                                                      65
     5.3. Troubleshooting                                                     67
6.   Processing machines (SN)                                                 69
     6.1. SN.INI                                                              69
          6.1.1. Example Section                                              69
     6.2. Configure A+W Production Terminal Processing                        70
     6.3. Available Drivers                                                   75
          6.3.1. Intermac                                                     75
          6.3.2. Forvet                                                       75
          6.3.3. Busetti                                                      76


A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx             3
         6.3.4. SkillGlass                                                  76
7.   Processing machines (XL – SN)                                          77
     7.1. FORVET KEY                                                        77
          7.1.1. Configuration A+W Production                               77
          7.1.2. Configure XL_JOBRELEASE.CFG                                77
          7.1.3. Configure SN driver                                        78




A+W Software GmbH            EN-CONFIG-A+W Production MachineControl.docx        4
1. Cutting table
This chapter describes how to implement a cutting code driver package in an A+W Production and
A+W Business Pro environment. Requirement is the base database from MarketSolutions. For
other databases, the document may differ.


1.1. Configure cutting table in A+W Production
Defining a new machine is made in the machinery allocation (MZO). Important is that the
Component-ID cannot be adjusted later. This ID creates a new data record to be found in [Master
Data / Machinery / Tables]. The new machine ID must not exist in the machinery allocation.




The configuration of the table parameters can be made via MZO. Below, you will find the
description via A+W Production Machine Dialog. You will find the component IDs to be used in the
following description.
In case of questions how to configure a machine in the machinery allocation, please read the
documentation regarding machinery allocation.
ID Table
[Master Data / Machinery / Tables]




The unique ID of each cutting table is named in the standard database consecutively TB1 ... TBn.
Overview ID MZO, Machine and Registration Point



A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                             5
     MZO ID          Machine ID        Registration Point    Release Dialog       Description
      110               TB1                   110               TABLE1           Cutting Table 1
      120               TB2                   120               TABLE2           Cutting Table 2
      150               TB3                   150               TABLE3         LAMI Cutting Table 1
      190               TB4                   190                  -             Manual Cutting


1.1.1. Integrate Cutting Table into JobRelease
[Configuration / ALCIM / Release Dialog / Tables]




For each cutting table, a TABLE action has to be defined. The actions are numbered consecutively
while they are added and have to be allocated afterwards to a respective button in the release
dialog.
The behaviour of the cutting plan printout is also defined here (more about that later).
The Most Important Switches
    •   Lot type
        Lot type of detailed scheduling: always 100
    •   Machine ID
        MZO ID of machine:
        110, 120,… = Table1, Table2,…
        150, 160,… = LAMITable1, LAMITable2,…
        190 = Manual Cutting
    •   Driver directory
        Directory of driver package, e.g. HEG. This directory has to exist under
        $ROOT$\RELEASE\TABLES\



A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                               6
    •   Parameter XOPTC_NETZ
        Path for machinery code. For output on disc (parameter XOPTC_DISK) a message appears
        to insert the disc. Per default the output is to network in $SERVERDIR$\PROD\
    •   Parameter XOPTC_OPTI_LOS
        0 = one cutting code per lot
        1 = one cutting code per batch (this is not possible for each driver)
Machine code output for all machines
It is possible to process all machines of a lot type with one configuration instead of using
configurations for each machine. Therefore the switch Machine ID has to set to 0. In the past a
special script $SERVERDIR$\SCRIPTS\JobRelease_AllForType.VB was need, but actual this will
work with the standard script $SERVERDIR$\SCRIPTS\JobRelease.VB.
Pro: In Dialog Release you need just one button for IG line and one for spacer bender.
Contra: The machine code of all IG lines or spacer benders will be saved to one directory. This can
be adjusted by changing the PostCreationScript for the machines via XL_JobRelease.CFG. This is
beyond the standard.
Print Cutting Plan
Cutting plans can be print via Release or displayed on screen. The printout has to be configured
for each cutting table.
Parameter XOPTB_ALL_LAST
Refers to printout, do you want to print all cutting plans or just the last one and with or without
summary.
Parameter XOPTB_PRINTER
Printer for cutting plan. The variable <DR1> uses the printer that can be selected for lists during
release.
Parameter XOPTB_DISPLAY_PRINTER
This switch controls whether to print or do display the cutting plan. Since the user want to decide
this during runtime, the variable <PrinterDisplay> will be entered per default and a combo box in
dialog Release controls this.
Parameter XOPTB_PARAMETERHere you can enter additional parameters that change the
behaviour of the cutting plan printout, e.g. to reflect the cutting plan at X or Y axis using /MPX
and /MPY.


1.2. Configure cutting table in A+W Business Pro
Cutting tables are configured at the machine in A+W Business Capacity planning [Capacity
planning  Master Data  Organisation  Machines]
In the dialog yon set the options for the cutting table which are import for optimization too. You
set an output directory, were cutting code will be stored and you select a machine code.




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                               7
Machine codes with a number smaller than 1000 are standard machines and can’t be changed. If
you generated a new machine, the new machine will be copied of the selected one and gets a
new free number greater than 999.




The Keyword setting is important. The minimum lengths are 5 digits. This will be the name of the
directory where the driver files are stored. The directory is generated automatically if a new
cutting driver is entered. The content of the directory are the files from the template directory of
the copied machine, BAT file renamed to the new directory.
SELECT * FROM [SYSADM].[PROD_MACHINECODE] WHERE [MACHINETYPE] = 1 ORDER BY
[MACHINECODE];
Output to floppy disk
A+W Business Pro doesn’t know is this an Output to a network drive or to a floppy disk or USB
stick. If you want have a message before the files are copy to the disk, enter the following
commands in the BAT file (e.g. HEG.BAT) bdirect behind the line “:OUTPUT”:
ECHO MsgBox "Please insert floppy for Optimization ID " + %2, 48, "Bys cutting
code driver" > TempMsgBox.vbs
wscript TempMsgBox.vbs




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                                8
1.3. Configuration of cutting code driver
Each cutting table has a directory containing the drivers and corresponding configuration. This
includes a script for controlling, a DL file to adopt the driver configuration, BLOCK.PTH, and
further driver-dependent programs.
The BATCH script for controlling has to be the same name as the directory of the driver package.
If not, it will not be found by the batch release. Please consider this, in case the directory is
renamed during customer installation.
The SETUP overwrites the template directories, which can be used if you configure a new cutting
table. If not exist SETUP copies the template directories to the production directory.
During machine code creation, the OPT2SAVE file will be unpacked and copied to the working
directory. Afterwards the script for controlling will be called in production directory. In the script
the driver configuration of the DL file will be written to the unpacked OPT2TXT.DAT. Then, the
driver will be called that generates a cutting code in the working directory. At the end this cutting
code will be copied to the target directory. The process will be controlled by a control script which
will be installed during SETUP. Don’t manipulate the control script; the files will be overwriting
during SETUP.
Now it is possible to generate a cutting code. Depending on the cutting table, sometimes it is
necessary to adapt the driver configuration (often in DL file). The DL file modifies the
configuration of the OPT2TXT.DAT. This configuration file contains at least one record for each
driver. A description of the OPT2TXT.DAT can be found here:
\\jupiter\DOKU_DocuWare\XOPT_XOPTS\XOPTFiles\User_Manuals\Opt2txt.pdf
List of directories
A+W Production and A+W Business Pro uses the same files, but in different directories. The
working directory is the same.
A+W Production                   %ProgramFiles(x86)%\A+W\Techsoft\Release\...
A+W Business Pro                 P:\Release\...
Template directory               …\Driver\AUW_Tables\
Driver directory                 …\Driver\
Production directory             …\Tables\
Control script (AWBPro)          …\Tables\CuttingDrivers.BAT
Control script (AWP)             …\Tables\CUTTING2.BAS
Working directory                %APPDATE%\A+W\Techsoft\Release\Tables\




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                             9
For each cutting code you have one sub directory in the TABLES folder. The directory name is the
ID. The directory includes a control script <ID>.BAT, BLOCK.PTH, DL files, cu_DL.BAT (e.g. sub
directory HEG includes control script HEG.BAT). The sub directories in the template folder will be
overwrite during SETUP, in production folder not.
The control scripts execute cutting code driver in driver directory (e.g. HEG.BAT executes
XOPTB.EXE and XCEDICUT.EXE). This driver directory will be overwriting during SETUP, too.
cu_DL.BAT
With this script it is possible to disable or activate DL files in each driver package. Each driver
could have different settings, so you have to manipulate this cu_DL.BAT and the DL files, but not
the control script. In each cutting code driver package you will find a cu_DL.BAT script and it is
execute in the cutting code driver control script.
Newer driver (Albwir.Xopt….exe) don’t use OPT2TXT for their settings, they have its own CONFIG
file and no cu_DL.BAT.


1.4. List of cutting code driver and their characteristics
Each driver package must contain a BLOCK.PTH. The BLOCK.ZIP is used for default. Depending on
the cutting table, it is necessary to adapt the DL files on site, e.g. the cutting table works in INCH.
For details refer to the OPT2TXT description. The default package contains the following cutting
code driver.
HEGLA
Directory:      HEG                               Script:          HEG.BAT
Driver:         XCEDICUT.EXE              Cutting Code: <Job>[<Lot>].EDI
DL File:        XCEDICUT_mm.DL, XCEDICUT_inch.DLL
XOPTC_OPTI_LOS:          0/1, both is possible, output per batch or lot
ADDON:          Albwir.Xopt.HeglaLabel.EXE, HeglaLabel.CONFIG
BYSTRONIC
Directory:      BYS                               Script:          BYS.BAT
Driver:         XCBYSXYZ.EXE              Cutting Code: J< JOB >< LOT >.<Stockplate No.>


A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                              10
DL File:      XCBYSXYZ_f84.DL, XCBYSXYZ_f89.DL, XCBYSXYZ_f92.DL, XCBYSXYZ_f97.DL,
118_area_del_off.DL, 118_area_del_on.dl
XOPTC_OPTI_LOS:        1, output only per lot possible
LISEC
Directory:     LIS                     Script:             LIS.BAT
Driver:        XCLICUT.EXE             Cutting Code: <JOB>\<LOT>\PL<Stockplate No.>.DAT
DL File:       XCLICUT.DL, 118_area_del_off.DL, 118_area_del_on.dl
XOPTC_OPTI_LOS:        1, output only per lot possible
BOTTERO
Directory:     BOT                               Script:             BOT.BAT
Driver:        XCBOTHPS.EXE            Cutting Code: <JOB><LOT>\COD.DAT
DL File:       XCBOTHPS.DL, 118_area_del_off.DL, 118_area_del_on.dl
XOPTC_OPTI_LOS:        1, output only per lot possible
AWCUT
Directory:     AWC                               Script:             AWC.BAT
Driver:        XCAWCUT.EXE             Cutting Code: AWC<JOB>[<LOT>].CUT
DL File:       XCAWCUT.DL
XOPTC_OPTI_LOS:        0/1, both is possible, output per batch or lot
MACOTEC (XCMACVSG)
This driver is running with our standard XCAWCUT driver.
Directory:     MAC                                         Script:         MAC.BAT
Driver:        XCAWCUT.EXE, XCMACVSG.EXE Cutting Code: MAC<Lauf>[<Los>].CUT
DL File:       XCAWCUT.DL, XCMACVSG.DL
XOPTC_OPTI_LOS:        0/1, both is possible, output per batch or lot
INTERMAC
Directory:     INT                                         Script:         INT.BAT
Driver:        XCAWCUT.EXE, XCIMCDEL.EXE Cutting Code: INT<JOB>[<LOT>].CUT
DL File:       XCAWCUT.DL, XCIMCDEL.DL
XOPTC_OPTI_LOS:        0/1, both is possible, output per batch or lot
XTV
Directory:     XTV                               Script:             XTV.BAT
Driver:        XTVSR.EXE                         Cutting Code: OPT<JOB>.SAV
PerfectCut
PerfectCut is a common software from company RO which can control different cutting tables,
like MACOTEC.



A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                       11
We have 2 driver, one a normal driver which generates a cutting code and one which generates a
list of units with their sequence and rack number. This list can be optimized by PerfectCut. For
both drivers we generate DXF files for each shape. The settings for the driver are configured in a
CONFIG file in the working directory. If the CONFIG file doesn’t exist, the driver generates one
with all possible parameter.
•   Script: ROP.BAT     Driver: Albwir.XOPT.RoPattern.exe (RoPattern.config)
    Output: *.IMP
    Generates a normal cutting code for each pattern in one file or one file for all pattern
•   Script: ROR.BAT     Driver Albwir.XOPT.RoRack.exe (RoRack.config)
    Output: *.IMP
    Generates a file with all sheets, their sequence and rack information
•   Additional Tool: Albwir.Xopt.ShapeToDXF.exe (ShapeToDxf.config)
    Output: *.DFX
    Generate a DXF file for each shape, the name of the files can configure in the CONFIG file. This
    definition has to be configure in the config files of the driver too.
Optima
Optima Software can controls different cutting code tables, e.g. MACOTEC. The interface format is
similar to AWCUT. Configuration will set in a CONFIG file in the working directory. If the file
doesn’t exist, the driver generates one with all possible parameter.
Script: OPTI.BAT        Driver: Albwir.Xoptc.Optima.exe (Optima.config)          Output: *.OPT
Turomas
Directory:      TUR                             Script:          TUR.BAT
Driver:         Albwir.Xoptc.Turomas.exe        Cutting Code: P<4digit JOB><3digit LOT >.R01
CONFIG:         Turomas.config
DL File:        118_area_del_off.DL, 118_area_del_on.dl
XOPTC_OPTI_LOS:         1, output only per lot possible
ADDON:          TuromasLabelProcess.exe (see chapter for Labelprint)
In the Turomas.config the parameter for the cutting code file name are configure in section
<Settings>, the cutting code file name must be max. 8 character long:
           <Settings>
               <OptiBaseName>P</OptiBaseName>
               <FillJob>_</FillJob>
               <DigitOptRun>3</DigitOptRun>
               <DigitJobId>4</DigitJobId>
               <SplitJobOpt></SplitJobOpt>
               <IsCod_dat>false</IsCod_dat>
               <OutputFormat>0</OutputFormat>
             </Settings>



A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                          12
INTERMAC OTD
Directory:       IOTD                            Script:          IOTD.BAT
Driver:          Albwir.Xoptc.IntermacOtd.exe Cutting Code: P<4digit JOB>_<3digit LOT >.OTD
CONFIG:          IntermacOtd.config
XOPTC_OPTI_LOS:          1, output only per lot possible
In IntermacOtd.config the parameter for the cutting code name could be found. You can change
the parameter, the script copy all OTD files with batch number in name into destination folder.
The following parameter control the name of the output files:
    •     DigitsJobId – Number of digits of the job or batch number
    •     DigitsRun - Number of digits of the lot number
    •     SplitJobOpt – Delimiter between job and lot number
    •     FileBaseName - String with which the name begins


1.5. Cutting Code with Label Print
Since version 6.4 there exist cutting tables which can directly control a label printer during cutting.
All printers need extra information for the labels, but the technology used is different. We have
built features which generate additional information using Crystal Reports in A+W Business Pro
and A+W Production. These reports generate PDF and/or Text files which are stored as additional
information besides the OPT2 files. Cutting code drivers use these files to generate label specific
output files for the cutting table.
This feature is chargeable and is not include the price of the normal A+W cutting table
connector. For a normal cutting table a customer needs an A+W connector B. To use
label printing a customer needs an A+W connector C. Ask sales for more information.
To make it work an OPT2BAR.DAT is needed, to allow the driver to find the correct label
corresponding to the barcode. So you need to generate a label for each barcode. There are 2
kinds of additional data: LABEL.DAT and PrintCuttingLabels.PDF.
Optimizations with ShapeOpt maybe not supported, because in the cutting code you often have
only one record set for the both sheets optimized together with shape opt.


1.5.1. LABEL.DAT
LABEL.DAT is a text file generated by Crystal Report LABELDAT.RPT. This report generates a
section of data for each barcode. Each section starts with the following line which is needed to
identify the section [CuttingDataProviderSection][{Number of
Machine}][{Barcode}]and it ends with [EOS].
Our drivers currently support the keyword CuttingDataProviderSection. New drivers or
other applications in the future will possibly support other keywords.
The section contains a list of individual parameters in the following format:
<{Name of Parameter}="{Parameter Value}">
This format could be different for individual drivers, currently we have only one driver which uses
this format.

A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                            13
Here is an example from A+W Business Pro:
        [CuttingDataProviderSection][1000][T200020630001000]
        <ORDERNO="20630"> <ITEMBNO="1"> <BOMID="0"> <JOB="1004">
        <OPTIMIZATION="8"> <QUANTITY="5"> <SHAPENO="0">
        <COMMISSION="Kommission A"> <CUSTOMERITEM="KDPos A">
        <DELIVERYDATE="30.06.2017"> <BARCODE="T200020630001000">
        <PRODUCTNO="104"> <PRODUCT="Float 4 mm A+W">
        <CUSTOMERNO="1070"> <CUSTOMERNAME="Becker Glasbau">
        <WIDTH_CUT="1.700,00"> <HEIGHT_CUT="1.800,00">
        …
        [EOS]
This file can be used for every cutting code driver, maybe in future also to send additional
information to the cutting code driver. Actual (v6) it is used only for the label print feature of the
BOTTERO cutting code driver.
In our standard report you find a formula “<LabelDatFormat”. In this formula the shared number
variable “LabelDatFormat” will be set. Actual values are 0 (default) and 1 (OPTIMA). If you set this
to 1 the output are fields which are for OPTIMA, because this driver recommend fields with fix
names. In future maybe more options will be available, but it still could be that the reports must
be adjusted during the project to solve the customer’s request.


1.5.2. PrintCuttingLabels.PDF
In the PrintCutting.PDF you provide real labels, one label per page and one label for each barcode
in the optimization.




Each page must have a hidden control field containing the barcode number:
        @@BARCODE={Barcode}@@
        For example: @@BARCODE=00010002@@
The cutting code driver splits the PDF into one page for each barcode and builds a new PDF for
each pattern in the correct sequence. This new PDF is sent to the cutting table along with the
cutting code.




A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                             14
1.5.3. Configuration A+W Business Pro
Configure parameter in for cutting machine settings with a comma separated list of cutting
machine IDs. One Parameter for the LABEL.DAT [PARAM23 / STRVALUE1] and one Parameter for
PrintCuttingLabels.PDF [PARAM23 / STRVALUE2].
LABEL.DAT will be generate with Report LABELDAT.RPT.
PrintCuttingLabels.PDF generate with Report PrintCuttingLabels.RPT. If you need different Reports
for different cutting table you can use the Report PrintCuttingLabels<MachineID>.RPT.
The reports must exist in the Reports directory of A+W Business. The output files will be generate
direct in directory %APPDATA%\A+W\Techsoft\Release\Tables\ and are copied in the TableID sub
directory.




1.5.4. Configuration A+W Production
This function are implemented in the scripts JobRelease.VB and Cutting2.BAS since version 13.4.0
(20.06.2017).
In the JobRelease configuration of the cutting table a new additional Parameter XOPTC_LABEL has
to be added. Set the parameter name and Value in the Field Parameter. If you have more
additional parameter, separate the parameter with a semicolon. The following values are
possible:
XOPTC_LABEL=1 – generate LABEL.DAT with Report LABELDAT.RPT
XOPTC_LABEL=2 – generate PrintCuttingLabels.PDF with Report PrintCuttingLabels.RPT, if you
need different Reports for different cutting table you can use the Report
PrintCuttingLabels<TableID>.RPT.
XOPTC_LABEL=3 – generate both
The Reports must exist in folder $SERVERDIR$\Reports\Lables\. The output files will be generate
direct in directory %APPDATA%\A+W\Techsoft\Release\Tables\<TableID>\.




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                          15
In The report for the LABEL.DAT use the Machine ID from XOPT_OPTIMIERUNG.OPTIPAR.


1.5.5. Labels with Turomas
After generate the cutting code driver with Albwir.Xoptc.Turomas.exe, execute the additional tool
TuromasLabelProcess.exe. This tool uses the same configuration file, Turomas.config, and is
working if OPT2BAR and PrintCuttingLabels.PDF exist beside the generated cutting code.
For each pattern in the cutting code a file <CuttingCodeName>_<PatternNo>.POS and
<CuttingCodeName>_<PatternNo>.PDF will be generated. The PDF file contains the labels from
PrintCuttingLabels.PDF.
After this the generated PDF files per pattern will be convert into a PRN file. A PRN file is the file
format which is generated direct by the printer driver. In this solution the printer driver generate
his output direct into a file. The generated PRN file will be renamed into
<CuttingCodeName>_<PatternNo>.PRN and is part of the package of cutting code and .POS files.
The PDF file isn’t need anymore and the files will be removed if the conversion was done fine.
The conversion into PRN file is not so easy, you need some tools and some configurations:
Windows printer driver
Turomas uses CAB Printer (https://www.cab.de), e.g. Model Hermes+ 4L/300. Download the right
printer driver and install it on the Server where you generate cutting code. Configure the printer
driver, generate a label format with the size of the used label and set this format as default,
maybe it is need to set this as default for each windows user.
The Crystal Report PrintCuttingLabels.RPT has also to be generated and stored with this printer
driver and the same label layouts you use on the server during cutting code generation. The same
technic we use if we generate normal labels with Crystal Reports.
The name of the printer has to be configured in Turomas.config parameter <Printer>.
<Printer>CAB Hermes+ 4L/300</Printer>
PDF Reader
We support ADOBE or FOXIT. One of the reader must be installed and which one is used has to be
configured in Turomas.config in parameter <ReaderType>: 1 = ADOBE, 2 = FOXIT. Our driver open


A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                             16
the PDF in the reader and print them on the configured printer. The driver also close the PDF
reader if the PRN file was generate. This can take a while so you have to configure some timeouts
in milliseconds if nothing happens in the parameter <WaitForPdfReader> and <WaitOpenFile>.
<ReaderType>1</ReaderType>
<WaitForPdfReader>10000</WaitForPdfReader>
<WaitOpenFile>2000</WaitOpenFile>
Multi File Port Monitor
The freeware tool Multi File Port Monitor is need (https://sourceforge.net/projects/mfilemon/).
The tool can be find in the AUW Turomas package in sub directory tools
(.\Release\Driver\AUW_Tables\TUR\Tools\), or download it.
Install the tool and configure a printer port for the Windows printer driver and set the output in
the driver fix to this port. If you do this, the driver doesn’t print on a physical printer, it print the
result into a file. We can’t use the Windows standard printer port FILE, because in this function
you have to enter an output filename every time you print and with the Multi File Port Monitor
you can configure the filename.
In Devices and Printers mark a printer and open in the Printer server properties the tab Ports and
Change Port Settings.




Add a new Port from type Multi File Port Monitor. We recommend as port name PRNFILES.




A+W Software GmbH            EN-CONFIG-A+W Production MachineControl.docx                               17
Configure the Output path and the Filename pattern for this port.




The path must be fixed, UNC path possible but variables (e.g. %APPDATA%) doesn’t work. The
user need reading and writing rights on this path.
For the Filename use the following pattern: PrintCuttingLabels.%u.%c.prn. This generate a file
with user name and computer name. So it is possible to generate this cutting code on one Server
from different users.
In the next step allocate the new port to the Turomas printer. Open the Printer Properties and in
tab Ports select the new port PRNFILES.




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                          18
For testing the configuration open a PDF document in your PDF reader and print the document on
this printer. After this the PRN file should be generated in the configured output directory.
You must configure the same output path and file pattern in the Turomas.config in parameter
<TempPrinterFile> as configured in Multi File Port Monitor. The placeholder %u and %c works in
both file pattern.
<TempPrinterFile>C:\Temp\PrintCuttingLabels.%u.%c.prn</TempPrinter
File>
Turomas.config
In the Turomas.config the parameter for the label print function are configure in section <Label>.
Here an Example:
  <Label>
      <WaitForPdfReader>10000</WaitForPdfReader>
      <WaitOpenFile>2000</WaitOpenFile>
      <ReaderType>1</ReaderType>
      <Printer>CAB Hermes+ 4L/300</Printer>

<TempPrinterFile>C:\Temp\PrintCuttingLabels.%u.%c.prn</TempPrinterFile>
  </Label>


1.5.6. Labels with BOTTERO
BOTTERO generates and print the Labels with his own applications, but they need several
information for the sheets in the cutting code to print them on the label. The information we
prepare in the LABEL.DAT
The driver BotLabelProcess.exe must be execute before XCBOTHPS.EXE and it search in
LABEL.DAT for packages with the following syntax:
[CuttingDataProviderSection][{Maschin ID}][{Barcode Number}]
<{Name of Parameter}="{Parameter Value}">
...



A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                           19
[EOS]
The Output is the file BotLabel.TXT. The cutting code driver XCBOTHPS.EXE uses this file if exist
and add the information into the cutting code. The complete text between the header line and
[EOS] will be used and convert into one line. Special character like line/page break will be
removed. You need XCBOTHPS.EXE version 1.81 or higher.


1.5.7. Labels with HEGLA
HEGLA need a PDF file for each label with the name <BarcodeNumber>.PDF. The tool
Albwir.Xopt.HeglaLabel.EXE will split PrintCuttingLabels.PDF into different PDF files for all barcode
numbers which are found in the optimization. This tool must be execute before “XOPTB –e” (min.
XOPTB version 6.87) and will be configured in HeglaLabel.config.
An OPT2BAR is necessary and the following OPT2TXT parameter must be set to make it work:
[45:26] = 1
[98:17-20] > 0000
The cutting code driver stores the label number of the sheets in Parameter ISheetId in T records.
Actual this function doesn’t work for sheets nested with ShapeOpt.
HeglaLabel.config
The PDF files will be stored in the Parameter PdfPath. The Parameter can be an environment
variable which can be set in the HEG.BAT with the SET command before
Albwir.Xopt.HeglaLabel.EXE will be execute.
With the Parameter MinSheetSerialMode you can set the quantity when a line item will count as
series. For a series only one PDF for the first sheet and one for the last sheet will be generate.
<?xml version="1.0" encoding="utf-8"?>
<HeglaSettings xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <PdfPath>%HeglaPDFPath%</PdfPath>
  <SplitPdf>true</SplitPdf>
  <EmptyLabelInfo>1</EmptyLabelInfo>
  <MinSheetSerialMode>9999</MinSheetSerialMode>
  <RectangleMode>2</RectangleMode>
</HeglaSettings>


1.5.8. Labels with OPTIMA
OPTIMA generates and print the Labels with his own applications, but they need several
information for the sheets in the cutting code to print them on the label. The information we
prepare in the LABEL.DAT
The driver Albwir.XOPTC.Optima.exe search for in LABEL.DAT and if exist it uses special Fields
which are allowed in the INFO section of the OPTIMA Cutting code driver. Not all allowed Fields
are supported by our cutting code driver. So if OPTIMA extend their interface it is need to extend
our cutting code driver and the LABELDAT.RPT report. The LABEL.DAT has the following format:
[CuttingDataProviderSection][{Maschin ID}][{Barcode Number}]


A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                             20
<{Name of Parameter}="{Parameter Value}">
...
[EOS]
The following fields of the interface will be ignored by the cutting code driver, if they exist in
LABEL.DAT. These fields will be filled direct by cutting code driver: Id, SheetWidth, SheetHeigth,
RackNo


Following a few example fields which are supported by cutting code driver:
        [CuttingDataProviderSection][TB1][00010000]
        <SecondGlassReference="1">
        <Customer="Customer0">
        <PosNo="1">
        <OrderNo="513654">
        <RackCode="201">
        <RealDimXPz="5200">
        <RealDimYPz="2528">
        <DescMatCompPz="Novellini">
        <DeliveryDatePz="17-10-2017">
        <PzNOTE="Job 0815">
        <PzNOTE1="OPTIMIZATION 9">
        <PzNOTE3="BARCODE 00010000">
        [EOS]
This looks like that in the cutting code:
        [Info]
        Id=1
        RackNo=288
        SheetWidth=1473.200
        SheetHeight=800.100
        SecondGlassReference=88
        Customer=Customer22
        PosNo=23
        OrderNo=513654
        RealDimXPz=4032
        RealDimYPz=7424
        DescMatCompPz=Novellini
        PzNote=Job 0815
        PzNote1=OPTIMIZATION 9
        PzNote3=BARCODE 00010087




A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                             21
List of supported Parameter. If they exist in LABEL.DAT they will transferred into the INFO field of
cutting code:
SecondGlassReference, Customer, PosNo, OrderNo, PieceStandardPz,
RealDimXPz, RealDimYPz, GrindingPz, GrindingPzX1, GrindingPzY1,
GrindingPzX2, GrindingPzY2, BendingPz, QuantityPz, PriorityPz, LabelsPz,
LabelsPzCounter, RotationAllowed, PreferencePz, DescMatCompPz,
DeliveryDatePz, PzNote, PzNote1, PzNote2, PzNote3, PzNote4, PzNote5,
PzNote6, PzNote7, PzNote8, PzNote9, PzNote10, PzNote11, PzNote12,
PzNote13, PzNote14, PzNote15, PzNote16, PzNote17, PzNote18, PzNote19,
PzNote20


1.5.9. Labels with INTERMAC OTD
The INTERMAC cutting code driver Albwir.Xoptc.IntermacOtd.exe automatic search for
PrintCuttingLabels.PDF. If file exist, the PDF will be renamed into the same name like the cutting
code OTD file. The renamed PDF and a XML file with same name will be copied into an existing
folder which is configured in IntermacOtd.config parameter <LabelPath>.
The label printing our special application IntermacPrintDaemon will handle. This tool will monitor
the cutting process of the INTERMAC cutting table and send the right label file to the label printer.
The interface of INTERMAC is described here:
\\jupiter\Doku_DocuWare\Technology_Partner\Intermac\Product_OTD_Specification\LabelPrint
erOnGeniusCT_Rev00.pdf
In a released folder the cutting table generate a file called ToPrint.TXT. IntermacPrintDaemon
monitor this folder and read this file. In this file information about actual cut sheet can be found
and the IntermacPrintDaemon search in the PDF and XML files for the right label. Temporary the
PDF file of the lot is split into a bitmap file for each label. The bitmap file will be send to the
printer and the ToPrint.TXT will be deleted.
The IntermacPrintDaemon requires Ghostscript driver to handle the PDF files. Download and
install GPL Ghostscript on the PC where IntermacPrintDaemon will be execute:
https://www.ghostscript.com/download/




Configure IntermacPrintDaemon with this configuration file PrintDaemon.config.
Attention: If you have a 64-Bit Operation System you need the 64-Bit Ghostscript driver. The 32-
Bit driver works, but doesn’t create an output.



A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                            22
PrintDaemon.config
The PrintDaemon.config has the same configuration parameter like IntermacOtd.config to identify
the file names of OTD, XML and PDF files. The parameter in both configuration files must be
equal.
    •   DigitsJobId – Number of digits of the job or batch number
    •   DigitsRun - Number of digits of the lot number
    •   FillJob – Fill character if job number is shorter
    •   SplitJobOpt – Delimiter between job and lot number
    •   FileBaseName - String with which the name begins
The parameter for the folder:
    •   OptiPath – Folder where XML and PDF files are stored; same path like parameter
        LabelPath in IntermacOtd.config
    •   ToPrintPath - Folder where IINTERMAC store ToPrint.txt
    •   PdfConverterPath – Folder where PDFConvert.exe is stored
    •   BitmapBase – local directory where IntermacPrintDaemon stores bitmap files
Parameter to adjust the bitmap on a label for printing:
PrinterName – Name of printer where labels should be print
OffsetLabelX - X coordinate of the bitmap on the label
OffsetLabelY - Y coordinate of the bitmap on the label
DpiX – Resoltion in X direction for converting PDF into bitmap
DpiY - Resoltion in Y direction for converting PDF into bitmap
UseCrop – Use section from PDF (actual set on true)
First a bitmap of total page with defined resolution is created.
The following section is defined in pixels of the intermediate image.
CropLeft - Left edge of the section
CropTop - Top edge of the section
CropRight – Right edge of the section
CropBottom – Bottom edge of the section

Printer
Information about the printer by INTERMAC:
    •   Printer is Toshiba B-EX4T2

    •   The printer is connected by network cable in Genius CT (in HUB or D-LINK ethernet port).
        It is placed in Intermac private network. Printer requires static IP address. Genius CT will
        be configurated for costumer network with static IP address too.




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                           23
    •   If labeling section was written in OTD files, Genius CT wait for print the label. It is not
        possible to cancel or avoid a single label. Anyway it is possible to avoid the labelling
        process by a button enable/disable placed in Genius CT interface


1.6. Laser marking
What is laser marking? During the cutting process a laser burns a logo on the sheet. The position
of the logo is defined in the cutting code.
In the BOM the logo is defined in a processing of standard A+W processing type 1255. In A+W
Production, the processing has to be attached at the cutting part and contains information about
position, rotation angle or logo id.


1.6.1. Variant without SN file
You activate this variant with OPT2TXT parameter [45:24]. This only applies for rectangles and is
supported by EDICUT cutting code interface. A record in the BLOCK file isn’t necessary.
A+W Realtime Optimizer is necessarily required. Before generating the cutting code the logo
information will be stored in the OPT2DAT (CHRHOST filed, LABEL.SET) if they are not filled
(detailed scheduling doesn’t fill the fields).
The processing with the laser marking information has to be allocated in machinery allocation to
the cutting table. If not, the A+W Realtime Optimizer doesn’t write the information into OPT2 file.
Configuration XOPTON.CFG:
[Laser]
Mode=1
AdditionalTextMode=0
Configuration OPT2TXT:
[45:24] =       1        for “XOPTB –e” to generate the info records
                2        for mirrored coordinates
Configuration LABEL.SET:
The following fields has to be defined in LABEL.SET for laser marking.
 Field                          Length    Description                                            Used
 CUTMIRROR                      1         FEIN_UNIT.CUTMIRROR                                    Yes
 AWTYPE_LOGO_LAYER              1         POOL_BEARBEIT.MASS1                                    Yes
 AWTYPE_LOGO_IDENT              8         POOL_BEARBEIT.MASS2 (Logo ID)                          Yes
 AWTYPE_LOGO_CORNER             1         POOL_BEARBEIT.MASS3                                    Yes
 AWTYPE_LOGO_XPOS               5         POOL_BEARBEIT.MASS4 (X - position of the mark)         Yes
 AWTYPE_LOGO_YPOS               5         POOL_BEARBEIT.MASS5 (Y - position of the mark)         Yes
 AWTYPE_LOGO_WIDTH              5         POOL_BEARBEIT.MASS6                                    No
 AWTYPE_LOGO_HEIGHT             5         POOL_BEARBEIT.MASS7                                    No
 AWTYPE_LOGO_REFPOINT           1         POOL_BEARBEIT.MASS10                                   No
 AWTYPE_LOGO_REFEDGE            2         POOL_BEARBEIT.MASS11                                   No
 AWTYPE_LOGO_ANGLE              3         POOL_BEARBEIT.MASS12 (rotation angle 0-360)            Yes
 AWTYPE_LOGO_DATA               24        ?                                                      Yes


1.6.2. Variant with SN file
This variant is activated via the OPT2TXT switch [45:25] and available since release version 5.4. It
also applies to shapes and is currently supported by the EDICUT cutting code.


A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                               24
Requirement:
    •   BLOCK Entry of the sheet (thus also an SN drawing is required) which is also used during
        optimization.
    •   A+W Realtime Optimizer for cutting code output (OPT2BAR is absolutely necessary to
        accurately identify individual sheets).
Configuration SN.INI:
In the machine section ([ALCIM2000], import in A + W Production), the switch
ExportSurfaceProcessing = 1 must be set to activate the LOGO export.


Configuration A+W Production:
To optimize the sheets (rectangles and standard models) with SN drawing, and use the BLOCK
entry during optimization, disable parameter [ALCIM_SHAPE / SNCUTASSTANDARDFRM].
If you use this variant you lose the possibility of other A+W Production features, which doesn’t
work with BLOCK entry for standard shapes and rectangle: Extended edge deletion, Shape
optimization
EDICUT Cutting Code:
The laser marking is transferred in the info fields of the EDICUT code, XOPTB -E must be called and
the EDICUT code must be set to read the EDICUT.TMP
    •   Call LaserMarkWriter.exe (currently without parameters, will be improved if the details of
        the machine are known). The program reads OPT2DAT and BLOCK and extracts the data
        from the laser marking. The program creates a file LaserMark.TXT. Previously, the old file
        should be deleted.
    •   XOPTB reads the file LaserMark.TXT (if the laser marking is activated) and fills the
        corresponding info data in the EDICUT.TMP.
    •   XCEDICUT reads the EDICUT.TMP and creates the code
Data record for laser marking:
The data set is accommodated in the T information of each sheet. The structure is as follows:
IMarkierungNNNXXXX.XXXYYYY.YYYLLLLLLLLWWWWTTTTTTTTTTTTTTTTTTTTTTTT
Example: IMarkierung0010030.0000373.00000000001000033.1F
    •   Identification ("Markierung")
    •   3 digits for Identification number (Datatyp: Integer)
    •   8 digits for the X-Position of the marking (e.g.: 1234.567 mm)
    •   8 digits fort he Y-Position of the marking (e.g.: 1234.567 mm)
    •   8 digits for the logoID (Datentyp: Integer)
    •   4 digits for the angle of rotation (0-360)
    •   24 digits User data (Zahlen 0…9, Buchstaben)




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                         25
1.7. Troubleshooting
In case of problems with generated machine code the generated code, the OPT2SAVE file of the
corresponding optimization, and the driver directory are necessary for investigation. Error
messages of the driver appear in a DOS Prompt during call.


1.7.1. Circle troubles on INTERMAC (XCAWCUT)
It could happen, that an INTERMAC cutting table with XCAWCUT cutting driver cuts a full circle
three times.
The reason is, INTERMAC has a problem with the 4 quarter circle. We transfer them as 4 quarter
circle in clockwise (CW) orientation, but INTERMAC produced them as counter clockwise (CCW)
orientation.
 If you set the OPT2TXT parameter [106:22] = 1, the problem will be solved. With this we transfer
the data with counter clockwise (CCW) orientation.




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                           26
2. Cutting Table via A+W Realtime
  Optimizer and CutTV
One of the first things to do for any technician going out on an A+W Realtime Optimizer install is
to prepare in advance for his upcoming visit. This starts for me by getting in touch with the
responsible sales person from our end to make sure all modules etc. have been included from the
A+W side. Furthermore it is also very important to get in touch with the customer to make sure
everything required for our software to communicate properly with cutting table is in place. In
case we are missing modules from the cutting table manufacturer’s end he will have to get in
touch with them.
Some of the key questions to be asked will depend on the type of cutting table of course – I will
try to address these in each of the upcoming chapters.
If uncertain about specific configurations, etc. I always like to go back to my previous installs of
the cutting table in question to review what has been done in the past.
Please also note that the setup for controlling cutting tables is pretty much identical for both A+W
Realtime Optimizer and CutTV (CUTTV.CFG vs. XOPTON.CFG).


2.1. BYSTRONIC
BYSTRONIC is probably one of the most common cutting tables out there. One of the key things to
look at prior to the install is the type of cutting table. From the 1980’s up until about 1992, 1993
Bystronic tables used to be controlled via a serial connection.
After that till now they use their MMC software which is running the DNC Net online protocol
that allows us a “pattern by pattern” control of the table.
BYSTRONIC 84/89/92
In order to control the table you need to create your own cable. There is a configuration for it on
the “Glasstree”. On the Bystronic side there are usually two “SERCOM” boards – which you can
access to the back of the Bystronic Control Panel. These SERCOM boards will have switches and
radio buttons to set Baudrate etc. which have to match the settings you have in your
XOPTOPN.CFG file (sample settings below). In regards to these settings there is no rule of thumb –
I had to adjust these for each table. Please also note that you have to be very careful when
putting them back into the panel since they a) break easily and b) have to be pushed hard back
into the slot.
These Sercom boards are also one of them main trouble makers – they tend to break every couple
of years and if you seem to not getting any connection established it is always worth switching
them.
Beside the XOPTON.CFG and Bystronic Sercom board settings also make sure you configure your
Serial port properly on your PC. You can actually test the connection through Hyper Terminal to
see if the communication works at all.
Please also note that these old tables need the “old” header record since in the cutting code – you
will find more info about that in the individual cutting code documentation.
; Section for cutting



A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                             27
[Cutting]
MzoTableId=1
Table=BYS1
inittable=TABLE=BYSTRONIC;TYPE=XYZ84;COMDRV=RS232_WIN32API;PORT=0;TIMEOUT
=30;BLOCKSIZE=256;IGNORECRLF=N;WAITFORREQUEST=100


; Device configuration for serial communication
[Transfer]
;Device_configuration=port.dat
BAUD=2400
LENGTH=7
PARITY=2
STOPBIT=0
INBUF_LENGTH=1024
OUTBUF_LENGTH=1024
XON/XOFF=0
BYSTRONIC 92-2012
Following a decade of serial controlled cutting tables Bystronic switched to new operating
software called MMC which included the DNC Net online control protocol.
As suppose to the old tables these machines run a Windows operating system (either Windows
NT or Window XP) that will allow you to control them over the network. Please note though that
Bystronic doesn’t like it if you change the Ip Address of their machine – they have their own little
network that relies on their current IP address.
That’s why you either add a second network card to your own XOPTON-CutTV PC or you add
another network card if possible to the Bystronic machine which with using Terminal Server these
days will be the better option.
The Bystronic software has one main configuration file called mmc.ini which is located under
c:\windows on the Bystronic PC. In there you want to turn on the DNC Net protocol (DNCNET=1)
and you also want to configure the working directory. There is no specific directory that needs to
be used – you can create a new one or simply share the existing one (C:\data) for example.
Now on the XOPT-ON side you will have to obviously have to create a map drive to the Bystronic
PC – then you have to configure the “Cutting” section in the XOPTON.CFG. Please note that the
ParamDir directory reflects the path on the Bystronic machine so don’t use the map drive!
This Param Directory contains the parameter files for each glass type (cutting pressure, speed
etc.). If not existing you can usually create copies of existing ones and then just rename them.
The file name is based on the ALCIM article code field entry – for example your article has
00000006 in there for 6mm Clear glass the program will for a 00000006.par file in the respective
folder on the Bystronic PC.
The main communication between XOPT-ON and the Bystronic PC is done via the status.net and
job.net files so you should make sure that you have read & write rights to these files.
; Section for cutting - Old Serial Connection table………………..
[Cutting]



A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                            28
MzoTableId=1
Table=Bys1
inittable=TABLE=BYSTRONIC;TYPE=XYZ84;COMDRV=RS232_WIN32API;PORT=0;TIMEOUT
=30;BLOCKSIZE=256;IGNORECRLF=N;WAITFORREQUEST=100
CuttingCodeName=J00(O).(P)


; Section for cutting – New DNC Net controlled table
[Cutting]
MzoTableId=2
Table=Bys2
inittable=TABLE=BYSTRONIC;TYPE=DNCnet;WORKDIR=M:\Transfer;NCProgDir=M:\Tr
ansfer\NC;ParamDir=C:\Transfer\Param;BysNCDir=C:\Transfer\NC;JOBFILE=job.
net;STATUSFILE=status.net;TIMEOUT=60;READINTERVAL=12;ENDSTATUS=3
CuttingCodeName=J00(O).(P)


2.2. LISEC
Similar to BYSTRONIC LISEC also started off with tables being controlled with a serial cable. As far
as I know there is no one left of those so I will focus on the new generation tables that are also
controlled via online protocol.
With Lisec it is very important to get in touch with the customer before the technician takes off
for his visit. In order for the “GPS-Hand”( Lisec table software) the customer has to make sure he
has the following Lisec Modules:
        a)      Lisec File converter
        b)      Remote read module
The Lisec file converter is a must – without that the software can’t read the A+W code.
The Remote read module is necessary for the pattern by pattern communication but is not
mandatory!
This should be setup by a Lisec technician – I know it is a locked option and also needs to be
enabled in GPS-Hand. A map drive to wherever they would like to receive their cutting codes will
also be necessary. The online protocol is actually one of the best out there since Lisec is feeding
back detailed error messages as to what is not correct. Further below I have added in a diagram
that explains the way the protocol works – the Transfer.* files will be created in the NCprogdir.
On the Lisec side the customer needs to setup “recipes” for the individual Glass Types – the recipe
# comes from our article code field. If nothing is in there it will use 0 as a default.
Please note for tables capable of running both regular glass and Lami glass the recipe number for
Laminated glass has to be >= 101.
; Section for cutting
[Cutting]
Table=LIS1
Inittable=TABLE=LISEC;TYPE=R4_11;NCProgDir=L:\;NCProgName=PL001.DAT;ReadI
nterval=3
CuttingCodeName=PL(P).DAT


A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                           29
Lisec Protocol Communications diagram




2.3. HEGLA
HEGLA is probably the most common cutting table in Europe but also has become a household
name in a lot of North American plants. The HEGLA table has always been controlled over the


A+W Software GmbH        EN-CONFIG-A+W Production MachineControl.docx                         30
network but it has just been since the late 1990`s that they are using the latest HEGLA program
OPTIMAX that allows online control (pattern by pattern control).
The setup is simple – XOPTON will simply create the cutting code into a shared directory (the one
that you agree with the HEGLA technician on).From there HEGLA will pick up the file and
communicate with XOPT-ON through the Dummy.edi log file located within the shared folder.
One of the biggest issues that will come with HEGLA table is the limitation of the HEGLA software
only excepting only 5 digit article numbers. That means that if your article number is greater than
that it will be cut off after five digits automatically from the cutting code driver. In case you have
several tables you can use the ALCIM-tables-Articles function to work around the issue or in case
you just have a HEGLA table you will have the article code field to translate article numbers into
shorter numbers.
HEGLA also has a Remaster module the documentation for that will be dealt with in a separate
document.
; Section for cutting
[Cutting]
MzoTableId=1
Table=HEG1
inittable=TABLE=HEGLA;DESTINATION=S:\AW\DATA.EDI;LOGFILE=DUMMY.EDI
CuttingCodeName=HEGLA(P).EDI


2.4. BOTTERO
BOTTERO is also one of the more common cutting tables globally and they have improved their
communication significantly with their latest generation table and their revised software.
Up until about 2006 there was no direct online control possible – the BOTTERO software was
running in a dos environment. Getting these machines into a network environment used to be
very tricky and time consuming. That’s why in a lot of cases the old floppy drive was the main
source of transferring the cutting codes. The BOTTERO also has the specialty that the cutting code
is written in a hexadecimal format. It also requires the shape information to be created into a
separate file so you will see two file for the run in question.
For the old tables that meant that you created your cutting codes then had the table read in the
file – in case there were recuts that went onto the last sheet or that required additional sheets
XOPTON will recreate the cutting code and the code will need to be read in by the BOTTERO
software again.
For the new generation tables since 2006 there is new BOTTERO table software which runs under
the new generation Windows operating systems that will allow a single pattern transfer
communication in between XOPTON and the cutting table. Similar to the HEGLA table the
XT_RCUTF32.EXE is used to create the individual files per sheet.
; Section for cutting
Cutting]
;UseMZO=Y
Table=BOT2
inittable=TABLE=BOTTERO;DESTINATION=O:\cutcodes\BOT2\CUTCODE.OPT;LOGFILE=
dummy.log


A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                             31
CuttingCodeName=cutcodes\bot(P).dat


2.5. BILLCO
BILLCO is an American cutting table manufacturer. The interface hasn’t really changed in a long
time – since there is no online connection to the table will be controlled simply by creating the
cutting code into the share folder of the BILLCO PC.
The cutting codes consist of two files Batch.* and scores.*.
; Section for cutting
Cutting]
MzoTableId=1
Table=Bil1
inittable=TABLE=DUMMY




2.6. TUROMAS
2.6.1. Initial settings (AUW_Configuration_cutting.docx)
After the RTO is installed, we have to install the following software following the description at
the point 6.5 of the document “AUW_Configuration_cutting.docx”:
    1. Windows printer driver
    2. PDF Reader (ADOBE)
    3. Multi File Port Monitor



2.6.2. RTO label
The RTO label has only 2 parameter fields: “schedule” and “los”.
The label has to contain the variable: @@BARCODE={Barcode}@@


Example: '@@BARCODE=' +CStr({fein_unit.etikettnr}) +'@@'  @@BARCODE=00010002@@


This variable has to be printed and hidden (using white color) for each label.




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                              32
2.6.3. Installation and settings for PDF24 application
We have to install the virtual printer “PDF24” and rename it to “TuromasPDF”.
To install this pinrter we use the “pdf24-creator-8.4.1.exe”




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx         33
We need to do the following settings at the PDF24 application




Wizard




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx   34
Virtual printer PDF24




Context of the Interfase menu




Online PDF Converter




A+W Software GmbH        EN-CONFIG-A+W Production MachineControl.docx   35
Features




2.6.4. Configuration of “lblprinting.bas”
At the “lblprinting.bas” we need to inform that “TuromasPDF” will be the printer in use. By doing
this setting, the printing will be performed always at the folder
%appdata%\A+W\Techsoft\Xopton\Cutting using as name “PrintCuttingLabels”.



2.6.5. Configuration of cutting.bat
At the “cutting.bat”, we have to do the following actions:
    1. Clean the existing files (PRN,POS,PDF) before starting the process
    2. Execute the cutting code geneartion
    3. Start a second Batch “Postcut.bat”




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                         36
2.6.6. Settings for “Turomas.config”: Field Digit job ID
At the “Turomas.config”, we have used 4 digits for the field “DigitJobId”:




2.6.7. New Batch “PostCut.bat”
We have to use the new “PostCut.Bat” that will be executed in the background during the
“cutting.bat”. The RTO will start printing the labels creating the PDF file at the “cutting” folder.




A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                               37
   1. At this Batch we initialize the “Labelfolder” variable, it will be here where the files needed
      for Turomas are saved: Cutting code (*.R01) and Printing labels (POS,PRN).
   2. This Batch will wait to finish the PDF printing of the RTO by 2 options:
          a. Based on the size of the PDF file

          b. Loop up to 50 seconds (we can modify this value based on the amount of labels to
              print or depending on the printing speed). If after 50 seconds, there is not PDF file,
              then it will be redirected to the section “ERROR2”.
   3. Once the PDF file has been created, the TuromasLabelProcess.exe will be executed to
      create 1 pdf file per pattern
   4. The turomas printing files “POS” and “PRN” will be generated with the calling to the
      HERMES virtual printer *** this has to be the default printer ***
   5. The last step it is to copy the files to path, but it is not necessary to remove the files.




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                           38
3. Bender and Sealer
This chapter describes how to implement a bender and sealer driver package in an A+W
Production and A+W Business Pro environment. Requirement is the base database from
MarketSolutions. For other databases, the document may differ.


3.1. Configure bender and sealer in A+W Production
Defining a new machine is made in the machinery allocation (MZO). Important is that the
Component-ID cannot be adjusted later. This ID creates a new data record to be found in [Master
Data / Machinery / IG Lines or Spacer Bender]. The new machine ID must not exist in the
machinery allocation.




The configuration can be made via MZO. Below, you will find the description via ALCIM Machine
Dialog. You will find the component IDs to be used in the following description.
In case of questions how to configure a machine in the machinery allocation, please read the
documentation regarding machinery allocation.
ID for IG line and bender
[Master Data / Machinery / IG Lines]
[Master Data / Machinery / Spacer Bender]




The unique ID has to be named consecutively LIN1 ... LINn for of each IG and BEN1 ... BENn for
each bender. LINM and BENM is reserved for the manual line and bender.
Allocate machine driver




A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                         39
Each sealer and bender is allocated to a machine driver format and a section. Please note, that a
section can only be selected once for each driver. If you use the identical driver for IG line and
spacer bender, the section must be unique, too.
E.g. If LISEC IG line section 0 exists, no LISEC spacer bender may use section 0.




The machine code and section selected here refer to the configuration file XL_JobRelease.CFG.
Overview ID MZO, machine and registration point
    MZO - ID        Machine ID       Registration point      Release Dialog            Description
     1610             LIN1                  1610            BENDER_SEALER2              IG Line 1
     1620             LIN2                  1620            BENDER_SEALER4              IG Line 2
     1690             LINM                  1690                   -                  Manual Line
     1710             BEN1                  1710            BENDER_SEALER1              Bender 1
     1720             BEN2                  1720            BENDER_SEALER3              Bender 2
     1790            BENM                   1790                   -                Manual Bender
       0                -                     -             BENDER_SEALER8              LISEC KSR
       0                -                     -             BENDER_SEALER9          LISEC LineServer


3.1.1. Integrate bender/sealer into Release
[Configuration / ALCIM / Release Dialog / Bender and sealer]




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                                40
A BENDER_SEALER action has to be defined for each machine that should create a machine code.
The actions are numbered consecutively while they are added and have to be allocated
afterwards to a respective button in the release dialog.

The Most Important Switches
    •     Lot type
          Lot type of detailed scheduling: 700 = ISO / 1200 = Spacer bender

    •     Machine ID
          MZO ID of machine:
          1610,1620,1630… = IG Line / 1690 = Manual Line
          1710,1720,1730… = Spacer Bender / 1790 = Manual Bender

    •     Output path
          Path to save the machine code. For output on disc a message appears to insert the disc.
          Per default the output is to network in $SERVERDIR$\PROD\


Machine code output for all machines
It is possible to process all machines of a lot type with one configuration instead of using
configurations for each machine. Therefore the switch Machine ID has to set to 0. In the past a
special script $SERVERDIR$\SCRIPTS\JobRelease_AllForType.VB was need, but actual this will
work with the standard script $SERVERDIR$\SCRIPTS\JobRelease.VB.
Pro:
In Dialog Release you need just one button for IG line and one for spacer bender.
Contra:
The machine code of all IG lines or spacer benders will be saved to one directory. This can be
adjusted by changing the PostCreationScript for the machines via XL_JobRelease.CFG. This is
beyond the standard.


3.1.2. Configure bender texts
Bender texts are managed per item in table POOL_TXT for the header part.
POOL_TXT.TEXT_TYP = 1000
     Bender text of order entry transferred to ALCIM
POOL_TXT.TEXT_TYP = 1001
     Bender text created at batch release via ALCIMJobRelease.DLL and LABELPRINT.DLL
The switch [ALCIM_JOB RELEASE / BENDER TEXT TYPE] (Parameter  ALCIM  General  Job
Release  Bender Text Type) controls which bender text shall be written to the machine code.

Configuration of bender text at batch release
If the bender text is not transferred from order entry, the release can create an individual bender
text for each item. Therefore, enable function Bender Text Initialization at release.



A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                            41
The layout of the bender text is defined in configuration file $SERVERDIR$\COMMON
\LABELPRINT.INI:
[BenderText]
Text0= <AufNr>/<PosNr> <Lauf> <Breite>*<Hoehe> <SZR1>/<SZR2> <ArtBez>
The text can consist of fixed text blocks and variables. The variables (e.g. <AufNr> for the order
number) are defined in the configuration file in section [BeginVar] … [EndVar].
The bender texts created at release are saved in database table POOL_TXT with TEXT_TYP 1001.

Configure various bender texts at batch release
ALCIM includes just one bender text layout for all IGs: [Master Date / Labels, Sketches, Bender
texts / Configuration Bender Texts]
If various bender texts are necessary, define here several layouts. It is possible to define a shape
file (e.g. Bendertext_Mueller.txt) in the configuration of the bender text layout. This file has to be
saved in the form directory and contains the definition of bender text (only the definition!) usually
to be found in LABELPRINT.INI under [BenderText]Text0.
The form directory is fixed in $SERVERDIR$\Formulars\. There is a switch not used any longer in
the LABELPRINT.INI to set the directory, this one should be disabled: [Options]FormularPath

Show production number in bender text
Often it is necessary to show the production number in bender texts. Therefore, the bender code
must be shown per unit and not per item (XL_JobRelease.CFG switch SplitItemToUnits=Y). The
following variable in bender text can be used in LABELPRINT.INI:
<ProdNr_Bieger>=FEIN_UNIT.SEQUENZTYP(T=8)
POOL_TXT shows in bender text the text „FEIN_UNIT.SEQUENZTYP“, it will be converted to the
corresponding value while creating the bender code.


3.2. Configure bender/sealer in A+W Business Pro
Bender and sealer are configured at the machine in A+W Business Capacity planning [Capacity
planning  Master Data  Organisation  Machines]
In the dialog you have a type for bender and one for sealer, both works similar. You set an output
directory, were machine code will be stored and you select a machine code kind.




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                              42
Machine codes with a number smaller than 1000 are standard machines and can’t be changed. If
you generated a new machine, the new machine will be copied of the selected one and gets a
new free number greater than 999.




The IG driver and IG section parameter is important. This is the direct link to the configuration file
XT_AWISO.CFG.
IGU:
SELECT * FROM [SYSADM].[PROD_MACHINECODE] WHERE [MACHINETYPE] = 2 ORDER BY
[MACHINECODE];
Bender:
SELECT * FROM [SYSADM].[PROD_MACHINECODE] WHERE [MACHINETYPE] = 3 ORDER BY
[MACHINECODE];




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                             43
3.3. Configuration of bender and sealer driver
The machine driver and section definition is listed in the configuration (CFG) file. The CFG contains
an area for each machine, structured as follows: [XL_ISO_<Treiber>_<Sektion>] e.g.
[XL_ISO_LISEC_0].
Various switches can be set for each machine. A detailed description of these switches can be
found in the following document:
\\jupiter\DOKU_DocuWare\ALCIM2000\Freigabe\Installation_Configuration\File_Description_XL
CLASS.CFG_E.pdf
The base configuration file AUW_XL_JOBRELEASE.CFG and AUW_XT_AWISO.CFG contains a
functional area for each driver of section 0. Specialties are shown in the CFG description. These
files are a reference for the used configuration files and will be overwrite during SETUP. The
belonging PostCreationScript POSTIGU2.BAS as well as directories of former drivers are also
included in the standard.
A+W Production           %ProgramFiles(x86)%\A+W\Techsoft\Release\...
A+W Business Pro                 P:\Release\...
Template directory               …\Driver\AUW_ISO\
Driver directory                 …\Driver\
Production directory             …\ISO\
Control script (AWBPro)  …\ISO\IGUDRIVERS.BAT
Control script (AWP)             …\ISO\POSTIGU2.BAS
CONFIG file (AWBPro)             P:\Release\ISO\XT_AWISO.CFG
CONFIG file (AWP)                P:\COMMON\XL_Jobrelease.CFG
Working directory                %APPDATE%\A+W\Techsoft\Release\Tables\
Template and Driver directory will be overwritten during SETUP.


3.3.1. Process create machine code old driver
Old drivers are drivers executed via individual driver program, e.g. Lisec (XOPTLBID), Bayer
    1. OPT2 files are created for the driver in WorkingDir.
    2. The script AppName is called. The driver program is started and creates the machine
       code. This is renamed by the script (batch number in file name) and moved to the
       subdirectory OUTPUT.
    3. Call of PostCreationScript to copy the machine code to the configured target directory.
Example:
        [XL_ISO_XOPTLBID_0]
        AppDir=$ROOT$\Release\ISO\xoptlbid
        AppName=liframe.BAT
        OutputFile=LISEC.DAT
        WorkingDir=$USER$\Release\ISO\xoptlbid
        PostCreationScript=$ROOT$\Release\ISO\PostIGU2.bas




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                             44
3.3.2. Process create machine code new driver
New drivers are drivers that do not use driver programs. In this case the machine is created
directly from the application: e.g. ALCIMJobRelease module in AWP for Lisec (Format 1.8x),
Lenhardt (Format 5.x),…
    1. The machine code is created in OutputDir
    2. Call of PostCreationScript to rename the machine code and to copy the machine code to
       the configured target directory. Additionally, in AWP a file SCRIPTRESULT.TXT is created
       containing path and file name of the output. This information is written back to table
       FEIN_JR_FILES.
Example:
        [XL_ISO_LISEC_0]
        OutputFile=LISEC.TRF
        OutputFilePattern=LISECxxxxy.TRF
        WorkingDir=$USER$\Release\ISO\lisec
        PostCreationScript=$ROOT$\Release\ISO\PostIGU2.bas


3.3.3. Converting spacer type and spacer colour in machinery code
Depending on the interface it is possible to transfer a spacer type and a spacer colour in the
machinery code for spacer bender. Different benders can request different values for identical
types. If nothing else is configured, the values are transferred directly from ALCIM to the driver.
Therefore, the database fields POOL_SZR.RAHMENTYP and POOL_SZR.RAHMENFARBE are used..
Most drivers can modify these values via conversion table in the XL_JobRelease.CFG. A machine
comprehensive standard does not exist. It is necessary to discuss and configure this for each
machine together with the customer.
For spacer type there is a conversion matrix Frame and for the color Colour. For former drivers
there is only Colour, Frame has been added with the interfaces that can handle two values. Please
see description of CFG.


3.3.4. Converting gas type in machinery code
The sections of the individual drivers offer the possibility to define a default value for IG with gas
fillings. Example: LISEC driver:
        DefaultGas=1
        DefaultNoGas=0
Additionally, a gas article conversion can be defined in the CFG. Therefore, it is necessary to
enable the switch GasArticleTranslation. Conversion will be made in a new section
[<Treiber>_ARTICLE_GAS] in format <Gasartikel>=<Ausgabewert>. The conversion can also be
made directly in the machine section, but, for a better overview an individual section should be
used.
Example:
        [XL_ISO_LENHARDT_0]
        GasArticleTranslation= Y
        [XL_ISO_LENHARDT_ARTICLE_GAS]
        1000=1
        1015=7


A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                             45
        2025=12


3.3.5. Specialties of individual drivers
Since the interfaces to the various manufacturers are quite different, the XL_JobRelease.CFG does
not contain a parameter record valid for all drivers.

Format 01 Lisec (XOPTLBID) - [XL_ISO_XOPTLBID_0]
This is the old LISEC format created with the driver XOPTLBID.EXE. The base contains the
XOPTLBID directory including all necessary files.
There are 2 scripts for parameter AppName: LIFRAME.BAT for bender or LISEAL.BAT for sealer.
The script calls the driver XOPTLBID.EXE including parameters. This includes – among others - the
version number. Maybe, the script has to be adapted.. Check with the customer which version the
machine can handle. When calling the XOPTLBID.EXE via parameter „-?“ a list appears including all
possible parameters.
        LIFRAME.BAT  XOPTLBID.EXE -2.14
        LISEAL.BAT        XOPTLBID.EXE -V3.3 -L

Format 06 Lenhardt (Format 5.x) -
[XL_ISO_LENHARDT_0]
The driver always transfers the spacer type from ALCIM (POOL_SZR.RAHMENTYP) increased by +1,
in case of Georgian Bars +4 and for cast resin +8.
This is important for Lenhardt IG line. If this format is used for a Lenhardt bender, you can turn-off
adding of +4 or +8 by OutputForBending. +1 is still added.
LECHECK
For sealer LECHECK must run to calculate the bottom edge. It will be written into field
MZO_ROUTE_MAP.AUFSTELLKANTE or MZO_EINSTELLEN.KANTE_IN. If LECHECK is installed it
must be activated in XL_JOBRELEASE.CFG.
        DoCheck=Y
        CheckLineRestrictions=1
The machinery manufacturer delivers a LECHECK version to the customer matching the machinery
(Bystronic/Lenhardt. This is not an A+W product. LECHECK must be installed to the directory
configured in the XL_JoRelease.CFG (LeCheckWorkingDir). If this is not the case, the CFG needs to
be adapted.

Format 09 Lisec (Format 1.8x) - [XL_ISO_LISEC_0]
        FormatVersion=2.40
If this switch is not set or the value is not supported, the first supported interface version (Version
1.80) is used. New machines cannot handle this version. You can find the possible values in the
CFG description.

Format 09 Lisec (Format 1.8x) – KSR and LineServer

A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                             46
It exist to special LISEC interface, LISEC KSR and LineServer
LISEC KSR is a machine for edge processing which can be inside the IGU line or a separate
machine. If it is inside the IGU line the controlling for the KSR will be inside the sealer machine
code and has to be configured in the XL_JOBRELEASE section.
If it is a separate machine you have to configure detailed scheduling lot type 1400 (KSR). During
JobRelease use action BENDER_SEALER8 which generate a KSR machine code for lot type 1400. It
uses the XL_JOPRELEASE section XL_ISO_LISEC_11. Standard Output directory is
$SERVERDIR$\PROD\KSR\.
Read chapter for processing machines for more information
Output for LISEC LineServer can generated independent from machinery allocation. Use action
BENDER_SEALER9 during the JobRelease. The configuration happens in XL_JOBRELEASE section
XL_ISO_LISEC_10. Standard Output directory is $SERVERDIR$ \PROD\LineServer\.

Free shapes for BENDER and IG Line
An interface exists for individual drivers for free shapes (shape 99). The following switches must
be set in the CFG file:
    •   FilterShape99=N
        Real shape 99 items are not transferred to the driver.
    •   UseShapeFile=Y
        Path of SN drawings are transferred to the driver.
    •   WriteShape99=Y
        The driver writes shape 99 for all line items where an SN drawing exist.
    •   DXFFilePath=
        For LISEC it is necessary to configure the path (LISEC can handle max. 40 characters) for
        the DXF file. Maybe, this path must not be a UNC path. It has to be reached on the PC of
        release and the LISEC - PC.
    •   DXFOutputFilePath=
        (Optional for LISEC) does the same like DXFFilePath and has to link to the same directory.
        It will use for the driver, UNC path is possible. In the machine code the value from
        DXFFilePath will be entered.
Presently [2011.02 #180978], this function exists for the LISEC and LENHARDT 5.x format. From SN
version 2009 5.8.29.8209 or 2011 5.9.7.836 on and from ALCIMJobRelease 2009 patch on.

Create bender code without bender text
To control a bender without bender text, the check of bender text must be turned-off. If not, a
warning appears and the machinery code will not be generated.
        ThrowExceptionOnUninitializedBenderTexts=N
        [Trace] XTH10383=N


How does old driver create bender code with edge
individual sealing depth?

A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                               47
If a spacer record with POOL_MODELL.BEARB_NR=-1 and POOL_MODELL.ISROOTSHAPE=10 exist,
you can use the following XL_JOBRELEASE.CFG parameter to write the real spacer geometry into
OPT2DAT. Activate the parameter in [GENERAL] section:
        UseExplicitSpacerGeometry=Y
In the driver Section you have to set the following parameter:
        UseExplicitSpacerGeometry =Y
For RJKAN driver use the following parameter to manipulate the sealing value:
        DefaultSealingValue=0
        UseSealingFromCharacterhost=N
        SpacerDisplacementMode=0
It could be that you have a parameter UseExpliciteSpacerGeometrie in the CFG file, this is a
wrong parameter. Use parameter UseExplicitSpacerGeometry.


3.4. Configure Sealer in A+W Production Terminal IG-
   IN
It is possible to generate machine code direct in A+W Production Terminal, so it isn’t need to
generate it during job release. This works since version 5.5 + hotfix. The following example was
done for LENHARDT sealer code.
If you activate this function, a machine code is generated during loading a lot. If you press
produce, some information will be send to the machine (e.g. the barcode), with this information
the IG line can identify the machine code record in the interface file.
The machine code will be generate with the module ALCIMJobrelease.DLL. The file has to be
generate in a directory which is known in A+W Production Terminal and A+W Production Terminal
copy this files into a target directory.
ALCIMJobRelease.DLL is execute on the server where PPSWebService is running. The windows
user is the user of PPSWebService.
It could be important to define an XL_JOBRELEASE.CFG for this windows user for the settings
which deviate. For LENHARDT it is the setting PostCreationScript, for A+W ProductionTermianl you
don’t need to execute a script and the standard script doesn’t work here because it is optimized
for machine code generation in job release.
ALCIMJobRelease.DLL has to generate the machine code in a directory where A+W Production
Terminal has access. It can’t be the $USER$ directory, because the User directory of
PPSWebService isn’t the same user of A+W Production Terminal who copy the files later.
Here an example how the XL_JOBREELASE.CFG for the PPSWebService user could look like:
        [XL_ISO_LENHARDT_0]
        WorkingDir=$USER$\Release\ISO\Lenhardt
        OutputDir=$SERVERDIR$\Prod\TTV_LEN\Temp
        PostCreationScript=
In the A+W Production Termianl configuration you have to configure the machinery allocation
machine ID, a source directory where ALCIMJobRelease.DLL generate the machine code (for
LENHARDT it is the same value of XL_JOBREELASE.CFG parameter OutputDir), a target directory
where the machine code files are copied and a file mask which describe the files which should be
copy (e.g. *.len).




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                             48
3.5. Configure Sealer/Bender in JobTV
In A+W Production Terminal JobTV you can generate machine code from the release dialog for an
individual lite.




The driver call must be activate and a lot type of the machine must be set.




In XL_JOBRELEASE.CFG in the section of used machine a Parameter ParameterString must be
configured to define the path where the machine code should be stored:
        ParameterString=059;OutputPathNet=\\MyServer\Trans\Prod\TTVBender\;
        SilentMode=1
059 is the ASCII value (;) of the delimiter of the parameter value. This parameter string will be
transfer into PostCreationScript which uses the value of OutputPathNet as output directory for
the machine code. SilentMode must be set, so our standard PostCreationScript (PostIGU2.BAS



A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                              49
version 6.4.1 or higher) make no output messages which doesn’t work because the script is
running in background in the PPS WebService.
In JobTV Select the lites you want produce and a machine code with our normal JobRelease
function will be generate in OutputPathNet with always the similar name based on
OutputFilePattern. So if you release the next lites, the old machine code file will be overwritten.




3.6. Troubleshooting
In case of problems with generated machinery code, the configuration file XL_JobRelease.CFG as
well as the AWISO LOG file is needed apart from the machinery code. The AWISO file is activated
in the XL_JobRelease.CFG in the machinery section by the switch WriteAwisoSavForCheck.
Additionally, the XL_JobRealease contains a [Trace] section to activated further LOG files. For old
drivers, the drivers, driver configuration, and the generated OPT2 files are needed.
PostCreationScript POSTIGU2.BAS cannot be called
A cryptic message appears. This happens in case of “old“ drivers that generates OPT2 files.
Machinery code is generated via script, but the script POSTIGU2.BAS cannot be called afterwards.
The switch OutputFile in the XL_JobRelease.CFG must be set, even for drivers that do not need
the switch. The value is transferred to the PostCreationScript.
Message „Bender text not initialized!“ although bender texts exist
In case of this message machinery code is not created. Either an item of a batch has no bender
text or ALCIM is set to a wrong bender text type (POOL_TXT.TEXT_TYP 1000 or 1001).
[ALCIM / General / Job Release / Bender Text Type]
Performance problem while executing LECHECK or another check program
If a machine has many logical machines a check program like LECHECK can cause performance
problems. This check program is executed for each logical machine, although it is requested only
once for the physical machine.
This has been corrected from patch 2011 on (AWDesk #247464). To enable the behaviour use the
following switch:


A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                           50
INSERT INTO parameter (lastmodstation, lastmodzeit, bereich, eintrag,
text, nummer, modul) VALUES ('__INIT', CURRENT, 'MZO_CHECKING_IG_LINE',
'ONCE', '1', 0, 'MZO');
Message: XMM10229: No valid Lisec shape found for FRM




For some A+W shapes no LISEC shape exist (e.g. A+W shape 92, 93). To, solve this use the DXF
interface for the driver, if possible.
Run old 16-Bit driver in 64-Bit OS
Some of the old driver (like LENLINIE.EXE) are old 16-bit driver which doesn’t work in 64-Bit OS.
Development can convert this old driver, but this is expansive and this driver die out. If it is known
a request to development can be made in advance of the project.
Alternatively you can use an emulator: AWDesk #217872/#127638
In some installations with LENLINIE.EXE we use the free emulator from http://www.dosbox.com.
If you do this, install the emulator and execute in our BAT script the driver with the emulator:
"c:\Program Files (x86)\DOSBox-0.74\DOSBox.exe" -exit -c "MOUNT C %~5" -c
"C:" –c "SET XOPTFRM=C:\Lenhardt" -c "C:\lenlinie.exe -e -ln -b -v" -c
"exit"
The “–c” Parameter send commands to the emulator. First mount actual working directory as
drive C and go to drive C. Next execute the driver and at the end exit the emulator.




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                            51
4. Georgian Bars
For Georgian Bar production we need paper with a Georgian Bar sketch, also some machines can
be controlled direct with a machine code.


4.1. Report
Paper can be printed direct with A+W CAD Designer (Bars). This technique is no longer
recommended because you do not have much influence on the design of the papers.
It is recommended to generate the papers via CrystalReport, for this we have a standard report:
AUW_Grill_list.RPT ($SERVERDIR$\Reports\)




About special CrystalReports functions, the AWD file will be execute direct in A+W CAD Designer
(Bars) and a sketch and additional information will be send into the Report.
This requires an AWD file for each Georgian Bar. The file can be generated during Import, if not
the report works but without the most information.
The print with crystal reports has a lot of advantages, but one disadvantage. If you have the same
Georgian bars in both spacer of a triple IGU, you get a page for each spacer. In the old solution it
was possible to print one page.


4.1.1. Print direct with A+W CAD Designer (Bars)
The old way to print a grill list still works but isn’t configured in the standard. There A+W Production controls
A+W CAD Designer (Bars). The printout happens before JobRelease or direct in JobRelease with the action
MUNTINS_PRINT.




A+W Software GmbH             EN-CONFIG-A+W Production MachineControl.docx                                    52
In JobRelease Dialog add a simple On/Off-Action control for action MUNTINS_PRINT.




4.2. AWD file generation
If no AWD file is send from order entry via ORDERXML, A+W Production has a function to
generate an AWD file automatically during import.

1.1.1. Configuration until version 5.5
The parameter [ITEMS45ALCIM / AWDESIGN] to activate the function could be set only with an
SQL Editor, it doesn’t exist in A+W Production configuration (AWDesk ticket for develop the
missing parameter in ALCIM: #252438).


SELECT bereich, eintrag, nummer, modul, text FROM parameter WHERE
bereich='ITEMS4ALCIM' AND eintrag='AWDESIGN';
If the record exists, in column text the path for the AWD directory is stored. This is the same path
like in AWD20.INI. Standard value: $SERVERDIR$\AWDesign\Pool\



A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                           53
If no record exists, a record has to be inserted. The filed NUMMER is important, standard is 75 but
this depends on the other parameter of bereich='ITEMS4ALCIM'.
Read the following documentation file for more information:
\\jupiter\DOKU_DocuWare\ALCIM2000\Import\DirekterDatenimport\Installation_Configuration\
AddCustomizingSteps.SQL

1.1.2. Configuration since version 6.0
The file path to the AWDesign files is used from the standard parameter [POOL_GEORGIANBARS /
DATAFILEPATH]. If the parameter is empty the standard value $SERVERDIR$\AWDesign\Pool\ is
used.
I4A
With parameter [ITEMS4ALCIM_SETTINGS / SEQUENCE_OF_EXECUTION] you configure the
sequence of task which can be started during import interface Items4Alcim (I4A). Enter the task
AWD in the list to activate the AWDesign file generation.




O4P
In import interface Orders4Production (O4P) a thread with name AWDesign has to be configured
for import orders and reservations.




4.3. Machine control from A+W CAD Designer (Bars)
If you want control a saw for grills, you can use the action MUNTINS_MACHINE_CONTROL in the
standard JobRelease dialog.




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                            54
This is a simple On/Off-Action control for action MUNTINS_MACHINE_CONTROL.
To make it work a driver is need. Configure the driver in grill setting of AWP configuration [Rough
Scheduling  Grill Settings]…




… and in the configuration of AWDesign (AWD20.INI):
[Exports]
MaschineNames=RWSPROSS
OptimizeLength=@DISABLE
OptimizePrintList=@DISABLE
OptimizeRestLengthFile=SoptRest.DAT
OptimizeBorder=0
OptimizeMaxBoxes=100
OptimizeMinRest=200
OptimizeMinItem=5
OptimizeMaxItem=20
OptimizeMinYield=0.90
OptimizeExpand=2
InvertSorting=1
MaxNumberOfLines=0

[RWSPROSS]


A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                          55
MenuEntryName=R+R Spossenmontage
DriverName=RWSPROSS.DRV
FileName=@RUNNUMBER
FileExtention=RWB
DriverCode=2240420
PostExeName=awd.bat
PreExeName=@NONE
PostExeWaitForTermination=@YES
PostExeParameter=@NONE
PreExeParameter=@NONE
PreExeWaitForTermination=@YES
This is an example for the R&R grill saw configuration.
The name of the machine can be maximum 8 characters long name, in this example RWSPROSS.
The name is set as driver in A+W Production configuration and in AWD20.INI in MaschineNames
and section name.
“[MaschineName]DriverCode“ is a ONEWAY code generated with the following parameter from
AWD20.INI:
[AWDesign]CompanyName + [Exports]MaschineNames + [MaschineName]DriverName


The driver will be execute direct from A+W CAD Designer (Bars), after this the batch configured in
PostExName is execute to copy and delete the machine code from user directory to an output
directory.
If the configuration was OK, your see the driver in A+W CAD Designer (Bars) in [File  Export].




4.4. Machine control from XLCLASS
New machine driver for Georgian Bars are configured like driver for bender and sealer with
XLCLASS (XL_JOBRELEASE.CFG) functions.
In machinery allocation you configure the Georgian bar machine with machine type 102. For this
machine type a machine in A+W Production, with the right format and a section linked to
XL_JOBRELEASE.CFG, has to be configured.
In detailed scheduling the lot configuration must be changed that a lot for Georgian bar
production (standard 1300) is generated.
In release dialog you configure a new sealer/bender action and use the script
JOBRELEASE_ALLFORTYPE.VB.




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                           56
In the XL_JOBRELEASE.CFG the PostCreationScript POSTIGU2.BAS must be enabled to copy the
machine code into the directory defined in ReleaseDialog configuration.
JOSEPH Grid Cutter
Format 23  XL_ISO_JOSEPH
\\jupiter\DOKU_DocuWare\Technology_Partner\Joseph\Product_Grid_Processor\Interface_Feat
ures\JOSEPH_MUNTIN_Interface Configuration.docx




A+W Software GmbH       EN-CONFIG-A+W Production MachineControl.docx                       57
5. Processing machines (XL)
This chapter describes machines whose machine code generated at job-release (XL Class) and the
interfaces corresponding to that of the sealer and bender.
LISEC KSR
LISEC KSR is a seaming machine which can be integrated in an IG line, but also available
individually.
If the KSR integrated into an IG line, it will be controlled with the machine code of the IG line,
no extra machine needs to define. But if the KSR is alone, it can be used for all sheets
independent of the final product. For this a machine code is only needed for sheets which are not
build in an IGU, sheets for IGU are still handled with the IG machine code. To solve this configure
2 machines, one for IG line without machine code and one for the rest with machine code.
\\jupiter\Doku_DocuWare\Technology_Partner\Lisec\Product_ISO_GPS.Bender\Interface_Featur
es\Lisec Standard Transferfile 2.40_de.pdf
FOREL Processing Machine
Entwickelt über #329103. Hier wird wie bei der LISEC KSR die ISO Schnittstelle verwendet um eine
Bearbeitungsmaschine anzusteuern. Es gibt die Möglichkeit die Maschine über das alte FOREL
Format anzusteuern (ID 3 [XL_ISO_FOREL]) oder über das neue Format (ID 18 [XL_ISO_FOREL_IG])
ab Version 5.5 oder als Hotfix in Version 2011.
\\jupiter\Doku_DocuWare\Technology_Partner\Forel\Product_ISO_Line\Interface_Features\FILE
_TRANSFER.pdf


5.1. Processing machine in A+W Production
Processing machines in job release is not a standard function. In our standard database, the
function is prepared, but it must be enabled.


5.1.1. Configure machine type 103
It must be ensured that the machine type 103 is defined in the database for machinery allocation.
This type is used to generate a corresponding machine code during job release (1 = cutting, 100 =
IG line, 101 = bender, 102 = Georgian bars, 103 = processing machine).
Normally, A+W Production automatically creates a corresponding record in table
MZO_MASCHINTYP, but not for type 103 (AWDesk ticket #283650 to resolve this situation).
Check if record already exist:
SELECT * FROM mzo_maschintyp WHERE id_typ = 103;
If the record is missing add record manually:
SQLServer: INSERT INTO mzo_maschintyp (SPERRSTATION, SPERRZEIT,
LASTMODSTATION, LASTMODZEIT, ID_TYP, [TEXT], PARAM_DB_TBL_NAME,
DRIVER_CALL_METHOD, EXKLUSIV_FLAG, PFLICHT_FLAG, IMPLIZIT_FLAG)
VALUES ('------', CURRENT_TIMESTAMP, '------', CURRENT_TIMESTAMP,
'103', 'PROCESSINGLINE',
'MZO_BEARBEITUNGSMASCHINE,KOMPONENTEN_ID,BESCHREIBUNG' ,'Methode


A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                          58
(Driver-Call)' ,'0' ,'1' ,'1');
Informix: INSERT INTO mzo_maschintyp (SPERRSTATION, SPERRZEIT,
LASTMODSTATION, LASTMODZEIT, ID_TYP, TEXT, PARAM_DB_TBL_NAME,
DRIVER_CALL_METHOD, EXKLUSIV_FLAG, PFLICHT_FLAG, IMPLIZIT_FLAG)
VALUES ('------', CURRENT, '------', CURRENT, '103',
'PROCESSINGLINE',
'MZO_BEARBEITUNGSMASCHINE,KOMPONENTEN_ID,BESCHREIBUNG' ,'Methode
(Driver-Call)' ,'0' ,'1' ,'1');


5.1.2. Configure processing machine
A processing machine is defined like a sealer or bender, only there is no dialogue for this (AWDesk
ticket #283650 to resolve this situation).
Without dialogue, the only option entries for a corresponding machine manually adjust the table
MZO_BEARBEITUNGSMASCHINE.
SELECT * FROM mzo_bearbeitungsmaschine;
Important are the following columns:
    •   KOMPONENTEN_ID
        A unique name that is selected in the machinery allocation
    •   MASCHINENTYP
        103 (currently there are no other types)
    •   FORMAT_ID
        Number of driver from ALCIMJOBRELEASE.DLL, the same number as for bender and sealer
        (999 = no machine code).
    •   AUFRUF_SEKTION
        Section oft he driver in XL_JOBRELEASE.CFG.
Machine LISEC KSR used in the Standard the format 9 and section 11: [XL_ISO_LISEC_11]
The following SQL statements insert a record for a LISEC KSR:
INSERT INTO mzo_bearbeitungsmaschine (LASTMODSTATION, LASTMODZEIT,
KOMPONENTEN_ID, BESCHREIBUNG, MASCHINENTYP, FORMAT_ID,
AUFRUF_SEKTION) VALUES ('INIT', CURRENT_TIMESTAMP, 'LISEC_KSR',
'KSR Lisec format 2.40', 103, 9, 11);
Machine FOREL KSR used in the Standard the format 18 and section 0: [XL_ISO_FOREL_IG_0]
The following SQL statements insert a record for a FOREL IGU:
INSERT INTO mzo_bearbeitungsmaschine (LASTMODSTATION, LASTMODZEIT,
KOMPONENTEN_ID, BESCHREIBUNG, MASCHINENTYP, FORMAT_ID,
AUFRUF_SEKTION) VALUES ('INIT', CURRENT_TIMESTAMP, 'FOREL_IG',
'FOREL Processing machine', 103, 18, 0);
The following SQL statements insert a record for manual machine:
INSERT INTO mzo_bearbeitungsmaschine (LASTMODSTATION, LASTMODZEIT,
KOMPONENTEN_ID, BESCHREIBUNG, MASCHINENTYP, FORMAT_ID, AUFRUF_SEKTION)
VALUES ('INIT', CURRENT_TIMESTAMP, 'HAND', 'Hand control (manuelle
Steuerung)', 103, 999, 0);




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                          59
5.1.3. Configure XL_JOBRELEASE.CFG
It must be ensured that the relevant section of the selected driver exists in the
XL_JOBRELEASE.CFG. For LISEC KSR in the standard that would be the section [XL_ISO_LISEC_11].

How to get the edge processing into AWISO
interface?
Enable the parameter UseProcessings=Y in XL_JOBRELEASE.CFG section [GENERAL], so processing
are now known. In the section of the driver also enable this parameter UseProcessings=Y, so
processing are used for this driver.
In the driver section you have the parameter ProcessingTypeMode, which configure which
information should be send into the machine code (e.g. as LISEC type):
    -   0 = pool_bearbeit.klasse (Standard)
    -   1 = pool_bearbeit.typ + pool_bearbeit.klasse (used e.g. for LISEC LineServer)


If you use ProcessingTypeMode=1 you can manipulate the value which is send in the machine
code with matrix parameter ProcessingType[n1]=n2,n3,n4
    -   n1=Extension for Keyword 'ProcessingType' Valid(0..99)
    -   n2=Value to set for Processing Type (value for machine, find in interface docu)
    -   n3=Value read from field 'POOL_BEARBEIT.TYP'         (-1 ignore typ)
    -   n4=Value read from field 'POOL_BEARBEIT.KLASSE' (-1 ignore klasse)


For FOREL we have ProcessingType and a second matrix for application name on the FOREL
machine ProcessingText[n1]=n2,n3
    -   n1=Extension for Keyword 'ProcessingText' Valid(0..99)
    -   n2= Value read from field 'POOL_BEARBEIT.TYP' OR '.AW_BEARBTYP' (not clear)
    -   n3=application name on FOREL machine
ProcessingText0=1000,SFIL3
ProcessingText1=1005,SFIL4
ProcessingText2=1010,SFIL5


Write DXF file for line items
A DXF interface exists to transfer free shapes (shape 99) into the machine code. This happens for
all line items where a SN drawing exists. The following switches must be set in the CFG file:
    •   FilterShape99=N
        Real shape 99 items are not transferred to the driver.

    •   UseShapeFile=Y
        Path of SN drawings are transferred to the driver.



A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                         60
    •   WriteShape99=Y
        The driver writes shape 99 for all line items where an SN drawing exist.

    •   DXFFilePath=
        For LISEC it is necessary to configure the path (LISEC can handle max. 40 characters) for
        the DXF file. Maybe, this path must not be a UNC path. It has to be reached on the PC of
        release and the LISEC - PC.

    •   DXFOutputFilePath=
        (Optional for LISEC) does the same like DXFFilePath and has to link to the same directory.
        It will use for the driver, UNC path is possible. In the machine code the value from
        DXFFilePath will be entered.

This feature isn’t implemented for KSR interface, but it should be done: #332650


5.1.4. Processing master data
All edge processing for machine code generation must be assigned to category 1 (Edge
Processing) in master data.




5.1.5. Configure machinery allocation
The machines involved must be associated with the type 103, this can be done in the MZO only when
creating a new machine.




A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                            61
Currently it is not possible to select the component ID from
MZO_BEARBEITUNGSMASCHINE.KOMPONENTEN_ID (AWDesk ticket #283650 to resolve this
situation).
If you want to assign the component ID or a machine afterwards the ID_TYP 103, this is only
possible through a SQL editor on the table MZO_REALMACHINE. PARAM_DB_TABLE_KEY is the
link to the record in table MZO_BERBEITUNGSMASCHIEN.KOMPONENTEN_ID: “LISEC_KSR”,
“FOREL_IG”.
SELECT * FROM mzo_realmaschine WHERE id_phys = ?;
UPDATE mzo_realmaschine SET id_typ = 103, param_db_table_key =
'<MZO_BERBEITUNGSMASCHIEN.KOMPONENTEN_ID>' WHERE id_phys = ?;
Attention: If the processing type can be assigned to other processing machines which are no KSR,
you have to set this machines to machine type 103 too. Set the component ID to the manual
processing machine HAND.
UPDATE mzo_realmaschine SET id_typ = 103, param_db_table_key =
'HAND' WHERE id_phys = ?;


5.1.6. Configure detailed scheduling
A detailed scheduling lot type is need, if you want generate machine code during JobRelease. If
machine code is generate only with A+W Production Terminal, you need no special Lot.
The detailed scheduling must be configured to read processing: [FEIN_TREATMENTS /
READPOOLBEARBEIT] = 1




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                            62
For processing machines the detailed scheduling lot type 1400 is reserved. This is defined in
[Master Data  Detailed Scheduling  Lot Types].




Processing assigned on the lot types make the difference whether a machine code can be
generated or not. If no lot type 1400 is found, no machine code will be generated even if the
correct machine is allocated.




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                          63
5.1.7. Configure JobRelease
In the standard release dialog there is the option KSR. This generates machine code for a LISEC
KSR that is configured in the standard.




The checkbox is linked to the Bender/Sealer action BENDER_SEALER8:




The machine ID should be 0, so that the machine code will be generated for the complete lot
1400. A solution for each machine isn’t implemented.


5.2. Machine control via A+W Production Terminal
A script must be configured in the A+W Production Terminal, which is given the order number,
item and part number. In the script, the processing lot 1400 is fed with the transferred items and
a machine output is started. If there is no processing lot available, the lot is set to 0 in the script
and a corresponding output is generated for the corresponding processing.
From the A+W Production Terminal Processing only one item is processed at a time, here the
quantity must also be transferred to the script. In the A+W Production Terminal Order with a list


A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                             64
of single units, the marked units are passed to the script, here no quantity is needed, each record
is used with quantity 1.
The following steps must be executed in the script:
    •   AlcimJobRelease.USERRELEASE1
        Create object
    •   STDMETHOD(BeginDefinitionUserLotEx)
        Loads the object
        [in] BSTR ConnectString     Connect-String of database
        [in] BSTR StationID         Station ID
        [in] int ShowProgress       Enable progress indicator=1 disable=0
        [in] int ShowErrorMessages  Enable error messages=1 disable=0
        [in] int ShowErrorList      Enable error list=1 disable=0
        [in] BSTR ListOfMachines    E.g.: '5, 6, 88' = ID of alternative phys. machines
        [in] long SizeOfList        3 (three alternatives in list)
        [in] long ProcessingNumber  Generally valid processing number (0|-999 for
        IG/spacer)
        [in] long LotType           Def. In FEIN_BEARBTYP, e.g. 700, 1200 or 1400; 0
        creates
                                   a lot if none exists
        [out]long                   Return value of function
    •   STDMETHOD(AddToUserLotEx)
        adds unit to object
        [in] long order                   Order number
        [in] long item                    Item number
        [in] long sub_item                Sub item
        [in] long partnumber              Part number
        [in] long processingnumber        Processing number (-999=use generally valid)
        [in] long amount                  Quantity to be produced
        [out]long Return value of function
    •   STDMETHOD(AddToUserLotExWithLabel)
        like AddToUserLotEx plus one additional parameter
        [in] BSTR labelnumber          Label number
    •   CreateOutputUserLotCompact()
        creates output in file


5.2.1. Example
In the Designer a new script must be configured, here the fields are defined, which are transferred
into the SKRIPT_SELEKTION. Required is the order number, item number, part number and
possibly the quantity.




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                          65
You can call the script via the menu or define a button for calling the script.




Option Explicit
Const Scriptname = "TTV_ProcessingMachineJobRelease.VBS"
Const Scriptversion = "1.0"
Const MZO_ID = 310 'set right MZO ID of processing machine with ID_TYP 103
Const ConnectString = "DSN=alcimdb;" ' INFORMIX: "DSN=;" SQLServer: "DSN=;UID=;PWD=;"
Function Main (ParamSperrstation)
  Dim oDB, sqlCommand, oUserRelease, lReturn, lOrder, lItem, lPart, lQuantity
  Set oDB = CreateObject("AlcimRun.AlcimDB")
  Set oUserRelease = CreateObject("AlcimJobRelease.USERRELEASE1")
  ' BeginDefinitionUserLotEx(ConnectString,StationID ShowProgress,ShowErrorMessages,
  '
ShowErrorList,ListOfMachines,SizeOfList,ProcessingNumber,LotType)
  lReturn = oUserRelease.BeginDefinitionUserLotEx(ConnectString,"NO",1,1,1,MZO_ID,1,-999,0)
  ' ToolTV muss die Tabelle SKRIPT_SELEKTION wie folgt beim Skriptaufruf füllen
  ' wert1 = Auftragsnummer
  ' wert2 = ALCIM Positionsnummer



A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                  66
  ' wert3 = Teilenummer
  ' wert4 = Menge (bei Einzelscheiben diesen Menbge im Skript fest auf 1 setzen)
  sqlCommand = "SELECT wert1, wert2, wert3, wert4 FROM skript_selektion " _
               & " WHERE sperrstation = '" & ParamSperrstation & "'"
  oDB.SelectExec(sqlCommand)
  While(oDB.SelectFetch())
    lOrder = CLng(oDB.GetString(1))
    lItem = CLng(oDB.GetString(2))
    lPart = CLng(oDB.GetString(3))
    lQuantity = CLng(oDB.GetString(4))
    ' MsgBox lOrder & " " & lItem & " " & lPart & " " & lQuantity
    ' AddToUserLotEx(Auftrag, Position, 0, teile_nr, processingnumber, menge)
    lReturn = oUserRelease.AddToUserLotEx(lOrder, lItem, 0, lPart, -999, lQuantity)


  Wend
  lReturn = oUserRelease.CreateOutputUserLotCompact()
  Set oUserRelease = Nothing
  oDB.SelectDone()
  oDB.Done()
  Set oDB = Nothing
  Main = 0
End Function

In the XL_JOBRELEASE.CFG a PostCreationScript is defined if you want to output the machine code
also in the batch release. You cannot use the standard POSTIGU2.BAS here, since it is only
intended for batch release. Here a copy is used which has configured the output path and file
name in the script.
If you want to generate an output only via the A+W Production Terminal, then simply deactivate
PostCreationScript in the XL_JOBRELEASE.CFG machine section and set WorkingDir to the final
directory. Set the name of the file fixed via OutputFilePattern (batch number is 0 and lot 1,
placeholders x and y should be used in OutputFilePattern).
Example:
[XL_ISO_FOREL_IG_0]
UseProcessings=Y
;WorkingDir=$USER$\Release\ISO\Forel_IG
WorkingDir=$SERVERDIR$\PROD\FOREL
;PostCreationScript=$ROOT$\Release\ISO\PostIGU2.bas
OutputFilePattern=FOREL.TFF


5.3. Troubleshooting
Message “Lot type not defined” during JobRelease




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                       67
If the reason in the message isn’t the problem, than it could happens if you use an old
P:\SCRIPTS\JOBRELEASE.VB. The script needs the following changes:




Input box opens during JobRelease
If you use the Standard POSTIGU2.BAS an InputBox open to enter the output path for the KSR
machine code. The path will not transferred to the script, this is a known problem and will be
solved with #283759. Until a solution, use a copy of the script and enter the output path fix in the
script.
Message: XMM10229: No valid Lisec shape found for FRM




For some A+W shapes no LISEC shape exist (e.g. A+W shape 92, 93). To, solve this use the DXF
interface for the driver, if possible.




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                           68
6. Processing machines (SN)
This chapter is for configuration of processing machines which are controlled with special driver
build for A+W CAD Designer (Shapes); e.g. CAMDXF driver.
In the normal process an A+W Production Terminal Processing called a machine driver configured
in A+W CAD Designer (Shapes). In most cases a SN file is needed.
A driver package contains a section in A+W CAD Designer (Shapes) configuration file SN.IN and
driver executable plus BATCH files for control.


6.1. SN.INI
In a common installation the global SN.INI is stored in $SERVERDIR$\SN\. In this configuration the
base setting for the ERP and PPS system are stored.
For a processing machine the standard deviating switches are stored in an additional SN.INI. For
the deviation the A+W Production Station-ID can be used or if processing machine is configured
on an independent PC a self-defined ID can be configured: $SERVERDIR$\SN\User\<Station-ID>\
Configuration of SN.INI will be done with the A+W CAS Designer (Shapes) Config Tool and can set
for each User.




In the SN.INI for each processing machine minimum one section must exist. In this section set of
switches has to be configured. To activate this processing machine, the name of this section must
add in the switch Machines in section [Customer].
Often 2 section for one machine exist. One section for control by A+W Production Terminal and a
second section for control manually direct with a SN drawing in A+W CAD Designer (Shapes).
The different in the section will be the parameter ExportName. If controlled by PT, the value must
be @EXTERN (value is set by PT), for manually use the value must be @NAME (Name of the
loaded SN file).
The SN view, which should use for the driver, must defended in the parameter VIEW. The driver
call happens with a BATCH file which is defined in the parameter WindowsPif.


6.1.1. Example Section
[Customer]
Machines = ALCIM2000 ALCIM2000I FORVET
...
[FORVET]
Title = Export Forvet ToolTV
ShowView = 0


A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                              69
Export = @BLOCKFILE
ExportName = @EXTERN
ExportExtension = DXF
View = DRILL2
Path = @WORKPATH
Orientation = @CCW
WindowsCommand = NIL
WindowsPIF = Albwir.MC.Launcher.exe Albwir.MC.CamDxf.Forvet.bat
ToolTVFilterCheck > Albwir.MC.CamDxf.log
WindowsStarterBatch = sn3temp.bat
AttributeDescriptionFile = CamDxf.Forvet.Atr
Is0PARTEMPAuthor = 0
Is0PARTEMPClient = 0
ExcludeAttributes =
MarkShortSegmentBelow = -100000.
MarkInsideAngleAbove = -100000.
MarkInsideRadiusBelow = -100000.
MarkOutsideAngleAbove = -100000.
Axes =
Suctioncups =
Cutsize =
MinNCCodeFileNameLength = 1
NCCodeFileReplacementCharacter = 0S
WritePSMCenterShapeAttributes = 0
NCCodeFileName = @EXTERN(1-10).DXF
IsUsedForIG = 0
SplitOnIntegratedAuxcut = @NEVER
ForceDOSConventionForNCCodeFileName = 0
MinNCCodeFileExtensionLength = 0
HasRectangle = 0
HideFromMenu = 1
NestingStyle = 0
UseEdgeProcessingMacroStrings = 0


6.2. Configure A+W Production Terminal Processing
First make a copy of the standard PT Processing Parameter-Set AUW_PROCESSING for your
processing machine.




Next generate a PT Station and allocate the generated PT Processing Parameter-Set as default to
this new station.




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                        70
A+W Software GmbH   EN-CONFIG-A+W Production MachineControl.docx   71
The SN parameter section offers some basic settings for all Shaping & Nesting drivers.




    •   Driver settings
        This allows to edit the list of installed drivers.
    •   Standard driver
        This is shown as default driver in PT. The setting must contain the "Display Name" of the
        desired SN driver.
    •   SN Command
        The "SN command" setting can contain functions that are executed after opening the SN
        drawing. Several function numbers can be passed, each separated by ','. The numbers
        correspond to menu entries in Shaping & Nesting (SNDoMenuItem is called internally,
        the header snmenu.h defines the corresponding constants, see also.
        \\jupiter\DocuWare\Shaping_Nesting\!General\Installation_Configuration\wwSNINI.doc).
        Sample function numbers: 1806 - show all dimensions, 1807 – show only dimensions from
        the current view, 1793 – show dimension in mm, 1794 – show dimensions in fractional
        inches, 1795 – show dimensions in decimal inches).




A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                        72
In the Parameter-Set you have to configure your driver. If it is needed to configure several drivers,
they can be selected directly in a combo box in PT.




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                           73
   •   Alternative driver [optional]
       If this driver is set to need SN files, you can configure here an alternative driver which is
       used if the loaded unit has no SN file.
   •   Display Name
       The name which is displayed in PT Combo Box for driver selection.
   •   Load driver automatically [optional]
       After each change of order number and line item a note will displayed and the driver is
       executed automatically. Default value is false.
   •   Permitted RPNOs [optional]
       List of registration points which are allowed for this machine driver.
   •   Generate NC Code
       NC code for this machine should be generate. Default value is false.
   •   Path to SN Batch Files [optional]
       Path of batch files for trigger driver. Is used for simplified SN control.
   •   SBName Special Mode [optional]




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx                                 74
        Output of several SBNameXX.TRX files with one final driver call. Attention: The driver will
        also mnot execute after change of order number or line item, it is called only when all
        SBNameXX.TRX are written. Default value is false.
    •   SN Driver View
        SN file is open with this SN view. Default value: DRILL.
    •   SNExportMachine
        Section of the machine in SN.INI which is called
    •   Use Link to SN Panorama [optional]
        Machine driver will be execute by Panorama.
    •   Driver needs SN file
        Set on true if driver needs a SN drawing. For units without SN drawing, driver will not
        available in PT. Default value is false.




6.3. Available Drivers
The available drivers will not be installed with our DISKSETs. You’ll find all available drivers in the
following directory:
\\jupiter\TECHSOFT_Glasbaum\SHAP_NES\DRIVER\
The driver and corresponding BATCH files must be stored in $SERVERDIR$\SN\User\Default\. At
start of A+W CAD Designer (Shapes) this files will be copied into folder
%appdata%\A+W\Techsoft\SN\, if the files doesn’t exist.
If a driver must updated with a newer version, it isn’t enough to replace the files in
$SERVERDIR$\SN\User\Default\; the files in %appdata%\A+W\Techsoft\SN\ must be deleted.


6.3.1. Intermac
.\CAM-DXF\Albwir.MC.CamDxf.Intermac\
    •   CamDxf.Intermac.zip
    •   Albwir.MC.Camdxf.Intermac.Update.7z


6.3.2. Forvet
.\CAM-DXF\Albwir.MC.CamDxf.Forvet\
    •   Albwir.CamDxf.Forvet.Install.zip
    •   Albwir.MC.Camdxf.Forvet.Update.7z




A+W Software GmbH           EN-CONFIG-A+W Production MachineControl.docx                              75
6.3.3. Busetti
.\CAM-DXF\Albwir.MC.CamDxf.Busetti\
    •   Albwir.MC.Camdxf.Busetti.zip
    •   Albwir.MC.CamDxf.Busetti.Update.7z
    •   Busetti.chm


6.3.4. SkillGlass
.\SkillGlass\DXF\
    •   Albwir.MC.Dxf.Skill.7z
    •   Albwir.MC.DXF.Skill.Update.7z
    •   SkillDxf.chm




A+W Software GmbH         EN-CONFIG-A+W Production MachineControl.docx   76
7. Processing machines (XL – SN)
This chapter describes machine code driver which are controlled by job release (XL Class), but
execute an SN driver to generate the machine code.


7.1. FORVET KEY
FORVET has a processing machine park with cutting table and edge work machines which are
controlled direct by FORVET software. A+W Production transfer during job release all needed data
to this machine (DXF file for each sheet), the FORVET software optimize the glass by itself and
control the machines. Via FILEMUX interface the machine park can send A+W Production the
status of the sheets, e.g. sheet is cut, sheet is seamed. This is possible, because we send our
barcode number into the interface.
On the edge work stations optional A+W Production Terminal can be installed which generate the
machine code via SN driver like we do this for each single machine.


7.1.1. Configuration A+W Production
In A+W Poduction a processing machine for machine type 103 and a detailed scheduling lot for
this processing must be configured like it is described in the corresponding chapter in this
document.
The machine configured in table MZO_BEARBEITUNSGMASCHINE (can set in machinery allocation
editor in further version) uses the format number 24 and must be section 11:




In our example we use the component ID “FORVET_KEY” which is linked to the machine in
machinery allocation: MZO_REALMASCHINE.PARAM_DB_TABLE_KEY


7.1.2. Configure XL_JOBRELEASE.CFG
It is need to set the following general parameter in the CFG:
        [GENERAL]
        SplitItemToUnitsDefault=Y
        WriteFeinJrTables=Y
For the driver a section [XL_ISO_FORVET_11] is used. Use the section from standard configuration
file (AUW_XL_JOBRELEASE.CFG) as base. The following parameter are special for this driver:
    •   NcExportMachine=FORVETJR
        Link to machine section configured in SN.INI
    •   NcWorkingDir=$USER$\SN\
        The folder where A+W CAD Designer (Shapes) executes the SN driver
    •   NcOutputFilePath=$SERVERDIR$\Prod\FORVET\
        Output folder where the driver direct store the machine code




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                          77
    •   UseBatchSubFolder=Y
        In NcOutputFilePath a sub directory for a batch is generated.
    •   RemoveAllFilesFirst=Y
        if files exist in the NcOutputFilePath and sub folder, they will be deleted before the driver
        generate new ones
    •   NCDriverMode=2
        Controls how the SN driver generate the machine code: 0=Default; 1=AlcimSNDraw-
        >LaunchNCCode; 2=AlcimSNDraw->LaunchNCCodeForPacLayer()


7.1.3. Configure SN driver
The newest FORVET CamDXF driver is need and must be configured like all SN driver. It must be
configurerd for the A+W Production station which is doing the JobRelease.
\\jupiter\TECHSOFT_Glasbaum\SHAP_NES\DRIVER\CAM-DXF\Albwir.MC.CamDxf.Forvet\
This driver package include a configuration package for this driver in job release. In this package
you find an Albwir.MC.CamDxf.ForvetDxf.config, a SN.INI (only with the specials for this
machine) and the script Albwir.MC.CamDxf.ForvetJR.bat to execute special for this driver.
The machine in SN.INI must be configured in the section which is defined in XL_JOBRELEASE.CFG,
in our example [FORVETJR]. In this section the Parameter ExportSurfaceProcessing=1 must be
set.
In this section the script is execute in the WindowsPIF parameter. In this execute command, don’t
use the script parameter ToolTVFilterCheck like it is need for execution in A+W Production
Terminal:
     WindowsPIF = Albwir.MC.Launcher.exe
Albwir.MC.CamDxf.ForvetJR.bat
One different in the script for job release and for A+W Production Terminal is, that the driver EXE
will be execute in the script with the parameter –BATCH, to suppress the user input for every
item:
        start /wait Albwir.MC.CamDxf.Forvet.exe –BATCH




A+W Software GmbH          EN-CONFIG-A+W Production MachineControl.docx                               78

