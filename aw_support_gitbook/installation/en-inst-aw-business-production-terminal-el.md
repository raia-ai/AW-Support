---
title: "EN INST A+W Business Production Terminal (EL)"
category: "installation"
product: "A+W Business Production Terminal (EL)"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Business Production Terminal (EL)"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation and Configuration Documentation A+W Business Production Terminal (EL)    Change history:      Date             Edited by          Remarks                                                  Version     2017-11-16       MST                Original version                                         0.1     2017-12-01       PK                 Corrections                                              0.2     2018-06-25       MST                Driver version Chapter Set-up 4.1.2 and function 5"
source_file: "EN-INST-A+W Business Production Terminal (EL).pdf"
---


# EN INST A+W Business Production Terminal (EL)

Installation and Configuration Documentation
A+W Business Production Terminal (EL)
   Change history:

    Date             Edited by          Remarks                                                  Version
    2017-11-16       MST                Original version                                         0.1
    2017-12-01       PK                 Corrections                                              0.2
    2018-06-25       MST                Driver version Chapter Set-up 4.1.2 and function 5.2.3   0.3
    2018-08-31       MST                Release August 2018 6.1:                                 0.4
                                        Barcode and checksum 6.1.1
                                        BOM tree with additional capacity planning parts 6.1.2
                                        Read barcode 6.1.3
    2019-03-12       MST                Release March 2019 6.2                                   0.5
                                        Short keys, Parameter settings
                                        Delete block file entries
    2019-09-12       MST                September Release 2019 Fehler! Verweisquelle konnte      0.6
                                        nicht gefunden werden.
                                        Setup provides all dependencies
    2020-04-22       DNI                Barcoding - unique label identification per glass 6.4    0.7




    The installation instructions will assist the planner with the installation and configuration of the
    software named. Please proceed in the following sequence:


    1.       Check the installation requirements.

    2.       Compile the required data, additional programs, drivers, etc.

    3.       Note or determine the time required.




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                        1/41
Content

   1         Overview ......................................................................................... 5

   2         Requirements .................................................................................. 6
   2.1       Other program documents .................................................................................... 6
   2.1.1     Installation instructions A+W Business Pro ........................................................................ 6

   2.1.2     Configuration instructions A+W Business ........................................................................... 6

   2.1.3     Configuration instruction License Server ............................................................................ 6

   2.1.4     Configuration instruction License Client ............................................................................. 6

   2.1.5     Configuration instruction A+W CAD Designer (Shape) ....................................................... 6

   2.1.6     Configuration instructions machines, bender output ........................................................ 6

   2.2       System environment ............................................................................................. 6
   2.3       Database Server .................................................................................................... 7
   2.4       .Net Framework 4.5 ............................................................................................... 7
   2.5       License Server........................................................................................................ 7

   3         Installation ...................................................................................... 8
   3.1       Minimal program versions..................................................................................... 8
   3.1.1     A+W CAD Designer (Shapes) ............................................................................................... 8

   3.1.2     A+W Business database scripts ........................................................................................... 8

   3.1.3     A+W Production Manager .................................................................................................. 8

   3.1.4     A+W Business Module ........................................................................................................ 8

   3.2       Setup Starter ......................................................................................................... 8
   3.3       Installation with the Setup Launcher ..................................................................... 8
   3.3.1     Welcome Screen ................................................................................................................. 8

   3.3.2     Select disk set...................................................................................................................... 9

   3.3.3     Setup directory ................................................................................................................. 10

   3.3.4     Previously installed components ...................................................................................... 11




10.12.2021                                 EN-INST-A+W Business Production Terminal (EL).docx                                                          2/41
   3.3.5      Selection of the components ............................................................................................ 11

   3.3.6      Interface Service Configuration ........................................................................................ 13

   3.3.7      AWSOA Service User ......................................................................................................... 14

   3.4        Configuration after the Setup Launcher .............................................................. 15
   3.5        Execute restart .................................................................................................... 16

   4          Configuration................................................................................. 18
   4.1.1      Machine tab ...................................................................................................................... 18

   4.1.2      CAD tab ............................................................................................................................. 18

   4.1.3      Booking and scanner settings ........................................................................................... 19

   4.1.4      List settings ....................................................................................................................... 19

   4.1.5      Auto update settings......................................................................................................... 20

   4.1.6      Global Production Terminal settings ................................................................................ 20

   4.1.7      Saving, discarding settings ................................................................................................ 21

   4.1.8      New database tables ......................................................................................................... 21

   1.1.1.1. PROD_PT_AGGREGATE........................................................................................ 21
   1.1.1.2. PROD_PT_PARMETER .......................................................................................... 22

   5          Operation ...................................................................................... 23
   5.1        User login ............................................................................................................ 23
   5.2        Navigation control (control on the left side) ....................................................... 23
   5.2.1      Finding and booking the part ............................................................................................ 23

   5.2.2      Booking the part completed or broken ............................................................................ 25

   5.2.3      Machine code output........................................................................................................ 26

   5.2.4      Description of main window ............................................................................................. 28

   5.3        Auto update......................................................................................................... 30
   5.4        Logging and tracing ............................................................................................. 30

   6          Release .......................................................................................... 33
   6.1        August 2018......................................................................................................... 33



10.12.2021                                  EN-INST-A+W Business Production Terminal (EL).docx                                                           3/41
   6.1.1     Barcode and checksum ..................................................................................................... 33

   6.1.2     BOM tree with additional capacity planning parts ........................................................... 33

   6.1.3     Barcode improvements..................................................................................................... 33

   6.2       Short keys and parameter settings ...................................................................... 33
   6.3       September Release 2019 ..................................................................................... 34
   6.4       Barcoding - unique label identification per glass ................................................. 36

   7         Uninstalling ................................................................................... 38

   8         Updates from earlier versions ........................................................ 39

   9         Table of Figures ............................................................................. 40




10.12.2021                               EN-INST-A+W Business Production Terminal (EL).docx                                                  4/41
1 Overview
The following description assumes that no version was previously installed and therefore that this is a new
installation.
    -   Follow this description exactly
    -   Use the setups and configuration programs offered
    -   Do not use programs such as XCOPY or REGEDIT. Please only use programs that the setup offers.
The following list offers an overview of which steps must be run through during and after the installation:
    -   RequirementsChapter 2
    -   Installation: Chapter 3
    -   Configuration: Chapter 4




10.12.2021                         EN-INST-A+W Business Production Terminal (EL).docx                         5/41
2 Requirements
The following prerequisites must be implemented before installation.

2.1 Other program documents
The following documents offer a detailed description of steps that must be performed beforehand. You can find
these documents on the Intranet > Online service Area > Documentation > Internal Documentation.
2.1.1 Installation instructions A+W Business Pro
The installation instructions for A+W Business Pro are here:

\\Jupiter\SW_Install\v6\InstallationDocumentation\EN-INST-A+W Business Pro.pdf
2.1.2 Configuration instructions A+W Business
The old instructions are here:

\\jupiter\doku_docuware\ALFAK2000\!General\Installation_Configuration\DE-Installationshinweise.pdf
The current instructions are found here:

\\Jupiter\SW_Install\v6\ConfigurationDocumentation\DE-CONFIG-A+W Business.pdf
2.1.3 Configuration instruction License Server
The current instructions are found here:

\\Jupiter\SW_Install\2012\InstallationDocumentation\EN-INST-A+W License Server.pdf
2.1.4 Configuration instruction License Client
The current instructions are found here:

\\Jupiter\SW_Install\2012\InstallationDocumentation\EN-INST-A+W License Client.pdf
2.1.5 Configuration instruction A+W CAD Designer (Shape)


The current instructions are found here:
\\Jupiter\SW_Install\V6\InstallationDocumentation\EN-INST-A+W CAD Designer Shapes.pdf


2.1.6 Configuration instructions machines, bender output
The current instructions are found here:
\\Jupiter\SW_Install\v6\ConfigurationDocumentation\EN-CONFIG-A+W Production MachineControl.pdf

2.2 System environment
The operating system should support at least .Net 4.5.2 (Windows 7 SP1, Windows 8, Windows 8.1, Windows
Server 2008 SP2, Windows Server 2008 R2 SP1, Windows Server 2012 and Windows Server 2012 R2 and higher).




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                        6/41
The latest Windows updates should be imported. If the system has to be updated before installation, it must be
restarted before installation.

2.3 Database Server
A+W Business Production Terminal uses the existing A+W Business Pro database. Among other things, this means
that only the SQL Server database system is supported. For more information, please read the A+W Business Pro
installation instructions (chapter Fehler! Verweisquelle konnte nicht gefunden werden.).

2.4 .Net Framework 4.5
The .Net Framework 4.5 is required and will be installed by the Setup Launcher. Before installation, please check
the required rights for the installation.

2.5 License Server
The license server must be installed. Please read the appropriate instructions (chapter 3.1.2).




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                           7/41
3 Installation
You need administrator rights for the installation and configuration.

3.1 Minimal program versions
3.1.1 A+W CAD Designer (Shapes)
The following program and build versions are required:

AWSNLive.ocx: 13.4.389

SN.exe: 13.4.322

3.1.2 A+W Business database scripts
You need at least the following database scripts:

20171124a

20171026a

20170922a


It is recommended that you bring the A+W Business Pro database up to date

3.1.3 A+W Production Manager
You need at least version 13.4.885.0

3.1.4 A+W Business Module
The A+W Business Time Management is absolutely necessary

3.2 Setup Starter
Start the Setup Starter from your installation disk set. First the required .Net framework is installed if it is not yet
on the PC.

3.3 Installation with the Setup Launcher
3.3.1 Welcome Screen
First you see the welcome screen of the Setup Launcher




10.12.2021                         EN-INST-A+W Business Production Terminal (EL).docx                                8/41
Figure 1: Setup Launcher Welcome Screen
Click [Next]

3.3.2 Select disk set
A dialog appears on which you can select or generate a diskset. A diskset contains all components and settings
that you have selected during a previous installation process in order to repeat this installation.




10.12.2021                      EN-INST-A+W Business Production Terminal (EL).docx                           9/41
Figure 2: Dialog for selecting or generating a diskset.
Select [Create new Diskset] or a generated diskset

Click [Next}

3.3.3 Setup directory
A dialog appears on which you specify the source and target directory for the installation. If you are already using
an existing diskset, the directories are specified by the diskset.

Generally, the dialog looks like this:




10.12.2021                         EN-INST-A+W Business Production Terminal (EL).docx                          10/41
Figure 3: Directory selection
Enter the source directory of the installation (must point to the directory in which the setup of the A+W
Production Terminal (EL) lies.

Enter the target directory of the installation (is generally "C:\")

Click [Next]

3.3.4 Previously installed components
A dialog appears with the previously installed modules and components.

Click [Next]

3.3.5 Selection of the components
On the next dialog, select the program "A+W Business Production Terminal (EL)". All associated components are
automatically also selected by the Setup Launcher.




10.12.2021                         EN-INST-A+W Business Production Terminal (EL).docx                       11/41
Figure 4: Select setup
No other settings are required.

Click [Next]




10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx   12/41
3.3.6 Interface Service Configuration




Figure 5: Interface Service Configuration
Enter <Domain>\AWSERVICES as user

Enter the use password

Click [Next]

If the user entered has no rights to log into the service, you are asked whether the user should receive these
rights. In this case, the following notification appears:




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                              13/41
Figure 6: Granting service user rights
Click [Yes]

3.3.7 AWSOA Service User




Figure 7: AWSOA service user dialog
You can determine under which user the service runs. To do this, click the "Browse" button and the service user
dialog appears in order to find or enter the user more quickly.




Figure 8: Service user dialog
The user should be the same as the A+W Business COM user.




10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx                        14/41
When you have selected the user, click [Ok].

Click [Next] and you can now save the diskset and/or just install it

3.4 Configuration after the Setup Launcher
You can make the following settings:

SQL Server authentication

Entry of the database connection

Use the Protocol button to change the trace settings.

If the customer has no Windows domain, you can set this on the first dialog of the Config Tools:




Figure 9: Setting SQL Server authentications in the ConfigTool
Select "Use SQL Server Authentication" and insert the user and password for the SQL authentication.

Click [Next]




10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx                  15/41
Figure 10: Setting for database connection in ConfigTool
Enter the database server

Enter the database

Enter the user name

Enter the password

Click [Next]

Click [Finish]

3.5 Execute restart
Some services can demand a restart of the system. The Setup Launcher recognizes this and this dialog appears:




10.12.2021                      EN-INST-A+W Business Production Terminal (EL).docx                        16/41
Figure 11: Reboot is required dialog
Click [Yes]




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx   17/41
4 Configuration
Now you can start A+W Production Terminal. Under Program > Settings you can make settings there.




Figure 12: Finding program settings
4.1.1 Machine tab
On the 1st tab "Machine," you can select the machine or work process for the A+W Production Terminal.




Figure 13: Machine settings
The A+W Production Terminal (EL) starts with the machine set here. In addition, the color of the machine or the
work process is indicated. The color serves to make the next production step easier to see. It is recommended
that you do not give each machine its own color; otherwise it is easy to lose sight of the overview. It's better to
assign colors for machine groups. Thus, for example, you could give all cutting machines one color, the edge
processings another, etc. The various colors are set on the "Terminal Settings" tab (see Fehler! Verweisquelle
konnte nicht gefunden werden.).
4.1.2 CAD tab
The 2nd tab enables the making of CAD settings. The SNLive view of the Production Terminal is displayed in the
1st row here. The 'Drivers' grouping indicates the setting for the SN drivers. The user can select the SN machine
name in the 'Machine name' column using the combo box. These are the names of the machine partitions in the
SN.INI, for example, ALCIM2000, XOPT, FORVET, BENTELER.

The 3rd row displays the view of the SN machine driver. The display cannot be changed and serves only to check
whether the SNLive view matches that of the machine driver. If this is not the case, the user can change the
SNLive view on the 'Terminal settings' tab (see Fehler! Verweisquelle konnte nicht gefunden werden.).




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                             18/41
Figure 14: CAD settings
These are local settings per machine.

4.1.3 Booking and scanner settings
On the 3rd tab, default values for the quantities to be booked can be set and special settings for the connected
bar code scanner adjusted.




Figure 15: Booking and scanner settings
You can make booking settings in the upper grouping rectangle. Either the maximum possible quantity for the
booking is specified or you can store a fixed value here (e.g. 0 or 1). This is a local setting per machine.

In the lower grouping rectangle, you can make settings for the connected bar code scanner. The position and
prefix of the scanner and the time that that scanner read logic should wait for a scanner input. These are global
settings that apply for every Production Terminal. Only keyboard scanners are supported. Please 6.1.1 note and
do not activate the checksum sign for the scanners.

4.1.4 List settings
On the 4th tab, the list can be set that is on the main window.




Figure 16: List settings



10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                           19/41
The font size for the column header and for the columns can be set. The settings are local.

4.1.5 Auto update settings




Figure 17: Auto update settings
You can make settings for an auto update on this tab. Thus, a OneClick setup is simulated. If the A+W Production
Terminal (EL) is started as administrator, the program tries to find a new version and install it. For this, you must
store the new program version in a particular directory. You can configure this on this dialog.

First you determine a server directory. To do this, in the first grouping rectangle, you set the server directory
name and the path of the directory. In the last text box, the directory in which the setup and other files are
located is selected. The path from the first grouping rectangle is used as root directory. These are global settings.

3 files are provided for the automatic setup:

The setup (a msi file and is absolutely necessary)

The Package.xml (contains the setup version and is absolutely necessary)

The ReleaseNotes.html (optional)


These first 2 files must be in the specified directory (see above).

If the program finds a new version, it is installed and the program exits automatically. If the program does not
exit, the user must close the program. This is no problem. The current Release Notes can also be opened in the
About box - via Http link.

4.1.6 Global Production Terminal settings
On the last tab, you can define colors for individual machines (see 4.1.1):




Figure 18: Global PT settings



10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx                             20/41
It is recommended that you do not give each machine its own color; otherwise it is easy to lose sight of the
overview. It's better to assign colors for machine groups. Thus, for example, you could give all cuts a color, the
edge processings another, etc. In addition, the SNLive view can be set individually for each machine. Thus the
view for processing machines can be adjusted so that the view fits the view in the SN machine partition. SN
machine partitions are the names of the machine partitions in the SN.INI, for example, ALCIM2000, XOPT,
FORVET, BENTELER.

4.1.7 Saving, discarding settings




Figure19: Saving settings
You can save the settings [Save] or discard them [Cancel]. You can find the local config file by clicking the [Local
Configuration] button. The file name has the following structure:

        PTConfig_[AggregateID].xml
If you use the machine with the ID 3000, for example, the file name is "PTConfig_3000.xml".



4.1.8 New database tables


There are 2 new database tables in the A+W Business Pro environment:



1.1.1.1. PROD_PT_AGGREGATE


Machine-related data is saved here. There is a column for each machine.



 Column name                             Type                                   Description

 AGG_ID                                  int                                    AggregateID primary key

 MACHINECOLOR                            String 12 characters                   Machine color in the following
                                                                                format '#RGB' written under the
                                                                                column MACHINECOLOR. R, G, and




10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx                             21/41
                                                                                 B are each expressed in
                                                                                 hexadecimal. Pure blue would be
                                                                                 #0000FF.

 SNDRAWINGVIEW                           String 80 characters                    The SN Live view for the machine




1.1.1.2. PROD_PT_PARMETER


Here, global settings that apply for all terminals are saved. Therefore, there is only one entry in this table.



 Column name                             Type                                    Description

 SCANNERPREFIX                           String 10 characters                    Prefix for the scanner

 SCANNERPOSTFIX                          String 10 characters                    Postfix for the scanner

 SCANNERTIMEBETWEENKEYSTROKE int                                                 The parser desd for the scanner
                                                                                 input waits this specified duration
                                                                                 in ms for the next character. If the
                                                                                 wait time is greater than the
                                                                                 specified time, it is assumed that it
                                                                                 is a manual keyboard input.

 SERVERVOLUMENAME                        String 5 characters                     The drive letter for the update
                                                                                 network drive

 SERVERVOLUMEPATH                        String 254 characters                   The path for the network drive

 SERVERUPDATEPATH                        String 254 characters                   The path to files for the update.




10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx                               22/41
5 Operation
5.1 User login
After the start of the A+W Production Terminal (EL), first you must log in. The program opens after you have
successfully logged in.




Figure 20: : Login dialog



5.2 Navigation control (control on the left side)
On the left side, there is a navigation control with which the user can load sheets and processings and report
these completed or broken. For this, the navigation control has 2 tabs; one for loading the part and one for
booking the part.
5.2.1 Finding and booking the part
The program allows you to load sheets or processings on sheets that should be done on the set machine via
scanner or manual input (after pressing F2) for the order, item number, and part ID (processing ID). The scanner
loads the sheet and fills the fields order, item, and part automatically. During manual entry, the fields must be
filled and after that F2 or the Search button (marked in green) pressed to load the sheet. The machine can be
changed for the search. For this there is a combo box (marked in orange) with which the user selects the machine.
The default machine is specified in the settings (see chapter 4.1.1). In order to see the "Search" tab, the search
(the telescope, marked in blue) must be selected.




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                              23/41
Figure 21: Search dialog
On the very first loading of the SN file, surcharges for the edge processings are calculated and the SN file is saved.
The original file is not overwritten; instead, a new folder is created in the SN file directory with the name PT and
the SN file is copied to this folder and then edited with SN. If the SN file already exists in the PT folder, the
surcharges are not calculated again. If the surcharge values for production are changed, the SN files must be
deleted from the PT folder.

If no part was found, there is additional information in the log about why this is the case. Some cases might be as
follows:

The batch status must be greater than or equal to Optimized (400) and less than FullProduced (700).

We need a parent part that it a glass.



10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx                             24/41
We need an AWB Capa part (ZW_AUFTR_ZEIT)

We need an order part (BW_AUFTR_STKL)

We need a batch part (PROD_JOBITEM)

5.2.2 Booking the part completed or broken
On the 2nd dialog tab, a message with respect to the sheet or processing can be sent to the ERP system. The user
can report this loaded sheet or processing complete (Product button, F5, marked in green) or broken (Reject
button, F7, marked in red). In this control, the large SNLive display can also be opened (Zoom button, F12, marked
in yellow). It is also possible to empty the list (Empty list button, F10, marked in orange), which causes the entire
display to be emptied; the loaded part is no longer visible and therefore no further bookings are possible.




Figure 22: Parts dialog
In the Book field, the number of parts can be specified that should be removed for production or reported
broken. If too many parts are specified, the maximum possible quantity is used for booking. This means:




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                            25/41
If on machine 3 parts are reported completed, but 4 or more were reported broken, the breakage dialog appears
with the quantity 3. The quantity on the breakage dialog can be changed, but it is not possible to enter a larger
number than the maximum quantity.

For the completed message, the number of not yet completed parts is reported.

Some buttons may be grayed out:

The Produce button is grayed out if everything on the part has been produced. You see this using the line
Open/Done line (highlighted in Figure 22) and Done has the quantity 0.

The Breakage button is grayed out if no part has been produced yet. You see this using the line Open/Done line
(highlighted in Figure 22) and Done has the quantity 0.

If the number of parts is less than the maximum possible number, only precisely is booked.

If all parts are reported completed, the Produce button is deactivated and it can no longer be triggered. A
breakage report is still possible. As soon as a part has been reported broken, the Produce button is active again.
That is, there must be at least one part to produce so that the Produce button is active. The same applies for the
Reject button. If no part has been reported completed, the button is deactivated. At least one part must be
completed.

Under some circumstances it can happen that only a loading of the sheets is possible, but no completion or
breakage report can be made. Both buttons for completed or breakage reporting are then deactivated. There are
2 reasons for this, which are in the log, and the user is informed with a message:

No AIS user created in A+W Business

No A+W Business time management active




Figure 23: Grayed out booking buttons
5.2.3 Machine code output
The necessary settings for machine code are described in Chapter 4.1.2. The code is generated with F8 or the
ribbon by using the button code (marked in green). You need a SN file to generate the machine code. If there is no
SN, the Code button is grayed out and it cannot be pressed.




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                           26/41
Figure 24: Generating machine code


No ToolTVFilterCheck file is required since the block file output is done per sheet. The block entry has the name
Auftragsnummer_Positionsnummer_Teilenummer/BOMID_AggregateID. After pressing the code button, a block
entry is generated and an additional XML file is written to the directory
%Appdata%\A+W\BusinessProPT\MachineDriverInput. This XML has the name: MachineInformationData.xml.
The MachineInformationData.xml file can be copied by the driver batch to the driver directory and must be
deleted in the driver directory after the driver call. The copying and deletion must be done by the calling driver
batch. The MachineInformationData.xml file contains e.g.

    -   the batch number (XMLTag Jobnumber)

    -   the barcode of the sheet (XML tag Barcode)

    -   the batch number (=batch number) (XML tag Batchnumber)

    -   the article number or article code (XML tag ArticleCode)

    -   the article description (XML tag ArticleShortDescription)

    -   Number of produced sheets (XML tag NumberOfSheetsToProduce, is always 1)

    -   it is a TG or it will be one (XML tag IsTemperedSheet)

    -   the article height (XML tag Height)

    -   the article width (XML tag Width)

    -   the article thickness (XML tag Thickness)

    -   the order number (XML tag OrderNumber)

    -   the customer name (XML tag CustomerName)

Some drivers use these values for the output and in the driver the tags must be defined, so that the driver can
map the information. However, this does not apply to all drivers. The data of the MachineInformationData.xml
file can be extended. The MachineInformationData.xml file in the
%Appdata%\A+W\BusinessProPT\MachineDriverInput directory is deleted by the program automatically. After
that, the machine code is generated.

The code button is grayed out if:

    -   the physical machine is not a processing machine (type 20). The physical machine must be set up as
        described under 4.1.1.

    -   there is no SN file

    -   no SN machine was selected. The SN machine must be set up as described under 4.1.2.

We no longer need a ToolTVFilterCheck file. You should comment out or delete this line in the batch file (e.g.
Albwir.MC.Dxf.Skill.bat):




10.12.2021                          EN-INST-A+W Business Production Terminal (EL).docx                           27/41
….
for /f %%i in ("%SB1%") do set FilterName=%%i
if %3.==ToolTVFilterCheck. (
     echo generating ToolTV filter name from from SBNAME.TRX, line [1] = "%SB1%"
     echo ToolTV filter name is "%FilterName%"
     if not exist ..\ToolTV\Script\nul (
       echo ..\ToolTV\Script does not exist, apparently this batch was not called from ToolTV
       goto errorFLT
             )     )
  if not exist ..\ToolTV\Script\%FilterName% echo ..\ToolTV\Script\%FilterName% does not exist, this Shaping ^&
Nesting BOM part is not to be processed, exit
     if not exist ..\ToolTV\Script\%FilterName% exit
     echo ..\ToolTV\Script\%FilterName% exists, so this is the right BOM part, proceed ...
     echo.
))
….….
The program writes the correct glass to the block file and the driver reads the block name (marked in red) from
the 1st line of the sbName.trx file:
 20787_2_0_2000
0001466.DXF
4
TG / Tempered glass
10


0001466_0.SN
\\awbawp60\Trans\SN\201711\PT
FORVETU
Export Forvet
….


5.2.4 Description of main window
Additional information about the sheet is displayed. For this, there are the following controls:




10.12.2021                            EN-INST-A+W Business Production Terminal (EL).docx                    28/41
SNLive display (marked in green), displays a sketch of the sheet (if necessary with side view). The SNLive control
enables a zooming in on the drawing.

BOM of the item (marked in orange) in which the processing or sheet loaded is located. The sheet is displayed in
blue and the processing in red. If only one processing is displayed that is directly in connection with the glass
(cutting, hardening of the sheet or shipping), only the sheet is marked in blue.

A list control (marked in blue), which displays information about the sheet (height, width, cut size, next
processing, route, etc.). The display and sequence of the columns of the list can be set individually for each
station and user.

A large SNLive display for an external monitor with the same content as the SN Live display mentioned above
(F12).




Figure 25: Main screen


During the BOM control, the texts for the glass item can be marked in blue and the processings in red. These are
notes about on which glass the processing lies that is being searched for. It can happen that there is no red text
because you are searching for the cut, it's on another glass item and only the glass items are displayed in blue
(see Figure 24). It can happen that several processings or other parts are marked in red because they are all
produced on this machine.

Here the drillings are searched for on the first TGH.




10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx                             29/41
Figure 26: BOM window and marked texts

5.3 Auto update
The user must start the program with administrator rights in order to update the program. A dialog appears if a
new version is found. Here, the user can decide whether or not he would like to update. If he would like to update
(OK button pressed), the program closes automatically and the update is done. If he presses the Close button, the
program continues normally without executing an update. The setup of the auto update is described in
chapter 4.1.5. The current Release Notes can also be opened in the About box - via Http link.
3 files are provided for the automatic setup:

The setup (a msi file and is absolutely necessary)

The Package.xml (contains the setup version and is absolutely necessary)

The ReleaseNotes.html (optional)

5.4 Logging and tracing
The log and trace files of the programs are under C:\ProgramData\A+W\Log. To adapt the tracing and logging
settings for all users, start the ConfigTool with administrator rights. The log level for the programs and modules is
set using ConfigTool on the 1nd control.




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                             30/41
Figure 27: ConfigTool log settings
It is recommended that in case of error, you log in with the trace level "info".

If the ConfigTool was started without administrator rights, the following dialog appears to change the logging and
tracing settings for the current user or to start the ConfigTool as administrator.




10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx                         31/41
Figure 28: ConfigTool started as non administrator




10.12.2021                      EN-INST-A+W Business Production Terminal (EL).docx   32/41
6 Release
6.1 August 2018
6.1.1 Barcode and checksum
Please do not actdivate the checksum sign for barcode reading in the scanner settings. The program ignores this
checksum sign and therefore, errors can arise.
6.1.2 BOM tree with additional capacity planning parts
In the BOM tree, now processings are also displayed that arise due to the capacity planning. These are, e.g.
packing, delivery, tempering, TG furnace or laminated glass or IG line. We display these processings since the
processings can also be charged.




Figure 29: BOM window with capacity planning parts
6.1.3 Barcode improvements
Individual barcodes are now also read in. There were smaller problems with this.

6.2 Short keys and parameter settings
    1) Short keys and parameter settings
Part of the AWBusiness keyboard programming was implemented. That is, it is possible to navigate through
dialogs with the plus key and Ctrl+Plus. It is now possible to search for lites with the Enter key. On the Parameters
dialog, the values of the combo boxes were fixed and the user cannot enter any other values. The Parameter
dialog can be saved with Ctrl+S. Navigation with Ctrl+Plus and Plus has been implemented.



10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                              33/41
Delete block file entries

There is a new button on the program ribbon bar.




Figure 30: Delete block file Entry button


If the user presses this button, this dialog appears:




Figure 31: Delete block file Entry dialog


The user can specify the time in days when all block file entries will be deleted that are older than the specified
number of days. The program notes this entry.
All block entries with the following name were deleted:

    -   The name starts with ‘ ;-)Shape99_’ (=nested shape from ShapeOpt)

    -   The name matches OrderNumber_PositionNumber_BomId (= Block export from the ProductionManager)

    -   The name matches OrderNumber_PositionNumber_BomId_AggregateID (= Block export from AWB
        Production Terminal)



6.3 September Release 2019
    -   Setup provides all dependencies. The following assemblies are now part of the setup:

                             •   Log4cxx.dll

                             •   Get99.dll



10.12.2021                        EN-INST-A+W Business Production Terminal (EL).docx                            34/41
             •   AWSOA.Core.Native.dll




10.12.2021       EN-INST-A+W Business Production Terminal (EL).docx   35/41
6.4 Barcoding - unique label identification per glass
After scanning one of the unique individual lite barcodes, the glass side is displayed, but you can only produce 1
product and you cannot change the quantity. This ensures that only one product is produced.




Figure 32: Just one individual lite barcode can be produced
You can now produce the product. After you have produced the product, the Produce button is locked. Since you
are only working with single glass, you cannot produce more than 1 product with this mode.




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx                            36/41
Figure 33: After an individual lite barcode production, the ribbon is locked
To produce the next product, you have to scan in a new unique barcode or mass product barcode.




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx              37/41
7 Uninstalling
Use the operating system's control panel to uninstall the software.




10.12.2021                       EN-INST-A+W Business Production Terminal (EL).docx   38/41
8 Updates from earlier versions
You must update the following products:

A+W Business Production Terminal (EL)

A+W CAD Designer (Shapes)

Furthermore, the A+W Business database must be brought up-to-date with the A+W Business 6 Database Update-
Tool.



See chapter 3.1 for the required, minimal program versions.




10.12.2021                     EN-INST-A+W Business Production Terminal (EL).docx                    39/41
9 Table of Figures
Figure 1: Setup Launcher Welcome Screen .................................................................................................................. 9

Figure 2: Dialog for selecting or generating a diskset. ............................................................................................... 10

Figure 3: Directory selection ...................................................................................................................................... 11

Figure 4: Select setup ................................................................................................................................................. 12

Figure 5: Interface Service Configuration ................................................................................................................... 13

Figure 6: Granting service user rights ......................................................................................................................... 14

Figure 7: AWSOA service user dialog.......................................................................................................................... 14

Figure 8: Service user dialog ....................................................................................................................................... 14

Figure 9: Setting SQL Server authentications in the ConfigTool ................................................................................ 15

Figure 10: Setting for database connection in ConfigTool ......................................................................................... 16

Figure 11: Reboot is required dialog .......................................................................................................................... 17

Figure 12: Finding program settings ........................................................................................................................... 18

Figure 13: Machine settings ....................................................................................................................................... 18

Figure 14: CAD settings............................................................................................................................................... 19

Figure 15: Booking and scanner settings .................................................................................................................... 19

Figure 16: List settings ................................................................................................................................................ 19

Figure 17: Auto update settings ................................................................................................................................. 20

Figure 18: Global PT settings ...................................................................................................................................... 20

Figure19: Saving settings ............................................................................................................................................ 21

Figure 20: : Login dialog .............................................................................................................................................. 23

Figure 21: Search dialog ............................................................................................................................................. 24

Figure 22: Parts dialog ................................................................................................................................................ 25

Figure 23: Grayed out booking buttons ..................................................................................................................... 26

Figure 24: Generating machine code ......................................................................................................................... 27

Figure 25: Main screen ............................................................................................................................................... 29

Figure 26: BOM window and marked texts ................................................................................................................ 30

Figure 27: ConfigTool log settings .............................................................................................................................. 31

Figure 28: ConfigTool started as non administrator .................................................................................................. 32



10.12.2021                                       EN-INST-A+W Business Production Terminal (EL).docx                                                                 40/41
Figure 29: BOM window with capacity planning parts............................................................................................... 33

Figure 30: Delete block file Entry button ................................................................................................................... 34

Figure 31: Delete block file Entry dialog ..................................................................................................................... 34

Figure 32: Just one individual lite barcode can be produced ..................................................................................... 36

Figure 33: After an individual lite barcode production, the ribbon is locked ............................................................ 37




10.12.2021                                    EN-INST-A+W Business Production Terminal (EL).docx                                                          41/41

