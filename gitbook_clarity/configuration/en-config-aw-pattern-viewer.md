---
description: "EN CONFIG A+W Pattern Viewer"
---



# EN CONFIG A+W Pattern Viewer

         Configuration


A+W Clarity Pattern Viewer
Multistep Automated Production System




                                                           english




   A+W Software GmbH   EN-CONFIG-A+W Pattern Viewer.docx   1

                - INTERN -
Change history


        Date        Author            Notes                                       Version
                    Todd Leiseman     Draft                                       1.0
                    Todd Leiseman     Workflow Studio Customizing                 1.1
                    Todd Leiseman     Workflow Studio Clean Up Scripts            1.2
                    Jens Schmidt      RegisterForCurrentUser                      1.3
                    Jens Schmidt      Workflow activities: describing pictures and 1.4
                                      other activities
                    Jens Schmidt      Logos, stamps, reference marks              2.0




A+W Software GmbH            EN-CONFIG-A+W Pattern Viewer.docx                              2
Content

1.   A+W Clarity Pattern Viewer installation and customizing           4
     1.1. Installed diskset requirements                               4
     1.2. Extra component installation                                 4
     1.3. Pattern Viewer configuration                                 5
          1.3.1. Registration in the Pattern Viewer                    5
          1.3.2. PreparePatternViewer Tool                             7
          1.3.3. Differences between the two procedures                7
     1.4. IceGrid review and testing                                   9
     1.5. A+W Pattern Viewer tester                                   10
     1.6. Known issue messages                                        11
2.   A+W Realtime Optimizer configuration                             14
     2.1. RegisterForCurrentUser                                      14
     2.2. A+W Infrastructure 6 workflow studio configuration          15
     2.3. Known issue message                                         16
     2.4. Server with workstation A+W Pattern Viewer configurations   17
     2.5. A+W Realtime Optimizer usage                                18
3.   A+W Pattern Viewer workflow studio customizing                   22
          3.1.1. Setting starting point of the pattern                22
          3.1.2. AddCustomText                                        24
          3.1.3. AddCustomType                                        27
          3.1.4. ReferenceMark                                        30
          3.1.5. MirrorStripe                                         34
          3.1.6. MoveWaste                                            34
          3.1.7. RemoveAdditionalText                                 36
          3.1.8. Format Rack                                          36
          3.1.9. Prefix2ndGlassType                                   36
          3.1.10. Add2ndGlassTypeToAdditional                         38
          3.1.11. Change Sequence                                     39
          3.1.12. Processing marker                                   39
          3.1.13. Remove depiction of the support edge                40
     3.2. Table-dependent workflows                                   41
     3.3. Workflow clean up scripts                                   42
     3.4. Breakage reason                                             42
4.   Configuration                                                    44
     4.1. Rotating subplates automatically                            44
5.   A+W Push Button Tool                                             45
6.   Ice know how                                                     48
          6.1.1. Pattern tray and IceNode                             48
          6.1.2. Callback                                             48
7.   Research options                                                 49




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx          3
1. A+W Clarity Pattern Viewer installation
  and customizing
The documentation below shows the steps to complete an installation of A+W Pattern Viewer
when being configured with one cutting table (TB1).
Plus, how to customize the A+W Clarity Pattern Viewer Workflow to change how the screen can
be presented to the operator.
Please ensure the latest installation of A+W Clarity is downloaded with all current hotfixes and the
system is installed with the latest Windows Updates for the system in question.


1.1. Installed diskset requirements
    •   A+W Infrastructure Process Server Diskset with an AWSOA Database and valid ICEGrid
        connection


1.2. Extra component installation
    •   Component Selection > A+W Clarity > A+W Clarity Pattern Viewer
    •   Component Selection > A+W Common > A+W Planning 6 Optimization Services
    •   Component Selection > A+W Production > A+W Production 6 Realtime Optimizer




A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                                4
1.3. Pattern Viewer configuration
Here is the proven process that you undertake the registration in the A+W Pattern Viewer only for
the first installation and otherwise use the PreparePatternViewer tool.



1.3.1. Registration in the Pattern Viewer
Open the A+W Pattern Viewer under the Blue A+W Desktop Shortcut
On the A+W Pattern Viewer screen select the A+W Logo at the top of the screen




Click the Register Application entry on the left side of the screen
On the Register Application screen under Information click
    •   ICE Node Registered > click Register Application
    •   Tray-Application Installed > click Install
    •   Tray-Application Running > click Start (if needed)
Under Registration click the following
    •   Click [+] add new Service
    •   Change the Site ID as needed
            o   If no Site ID is present, please configure the Sites/Clients in A+W Infrastructure
    •   Update or Confirm the Table ID and Label ID as required
    •   Click the Register Application button




A+W Software GmbH                   EN-CONFIG-A+W Pattern Viewer.docx                                5
Ensure the Registration name is similar to 001#TB1#001 <SERVERNAME> with an active (Green)
status




Finally close the A+W Pattern Viewer screen.




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                            6
1.3.2. PreparePatternViewer Tool
The PreparePatternViewer.exe tool is installed in the folder C:\Program Files
(x86)\A+W\Clarity\A+W Clarity PatternViewer\PreparePatternViewer.
It's best to navigate with the Windows Explorer to the directory and then enter cmd on the
navigation line (there where the path is displayed) and press Enter.
In the Dos box, type PreparePatternViewer followed by the registration name (e.g., 1#TB1#001).




This causes the PatternViewer instance to be generated, or if it was already generated, it is moved
from another user to the user currently logged in.




1.3.3. Differences between the two procedures
First an application is created in the ICE registry and then you can create several instanced of this
application.
The Register application in the PatternViewer generates an XML file with such an ICE application
and the instances that are generated for this user.
ThisXML file is then loaded into the ICE registration; here, all instances of the participating
application are interrupted and re-registered.
If you do this for different users, then you generate several PatternViewer applications with 1-n
instances of this.


The PreparePatternViewer tool makes do without an XML file, it uses the API of the registry
directly and searches for the ICE-PatternViewer application (<COMPUTERNAME>-PatternViewer)
and moves the instance (PatternViewer-1-TB1-001) to another user; in case of a new registration,
any ICE-PatternViewer application, and generates a new instance
All other applications and instances are not affected like this and continue to run. If you would
like to make a change to the PatternViewer configuration in ongoing operation, you should
therefore always user the PreparePatternViewer tool.


You can get an overview of the ICE applications with Tools->Application->Show



A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                                     7
A+W Software GmbH   EN-CONFIG-A+W Pattern Viewer.docx   8
1.4. IceGrid review and testing
Open the Config Tools > Service Locator Administration under the Blue A+W Desktop Shortcut.
A new entry should exist for the A+W Pattern Viewer as seen below.




Right click on the PatternViewer-1-TB1-001 entry and choose Start, this should open the A+W
Pattern Viewer application and show a Green Play button.




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                             9
1.5. A+W Pattern Viewer tester
Open the Tools > A+W Clarity PatternViewer Tester under the Blue A+W Desktop Shortcut.
Note - If this does not open or there is an error message then the configuration is missing a
previous step from being completed
Under the AW.Clarity.PatternViewer.Tester screen change the first entry to read 1#TB1#001 then
click Start/View.
Note - Make a note of the 1#TB1#001 entry as we will need this in the future




A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                              10
This should also open an A+W Pattern Viewer screen with (1#TB1#001) in the top menu as show
below.




1.6. Known issue messages
Issue - Error while startup. Message: Spring.Objects.Factory.ObjectCreationException



A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                         11
Cause
The user receives the following screen when trying to open Tools > A+W Clarity PatternViewer
Tester under the Blue A+W Desktop Shortcut.
Solution
   •    Ensure the Component Selection > A+W Common > A+W Planning 6 Optimization Services
        has been installed from the A+W Installation Diskset and try the step again.
   •    If the A+W Planning 6 Optimization Services has been installed, then have a look in the
        logfile.
        If you find a string like:
        Message: Cannot instantiate Type [OptimizationMixed.OptimizationMixedCore] using ctor
        [Void .ctor()] : 'OptimizationMixedCore::checkEnviromentVariablesForOptiKernel:
        environment variables XOPTFRM or XOPTPLT or both are empty or the path does not
        exist; set variables to the existing path and restart the service'
        The environment variables are missing, you can either create the variable ones by hand,




A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                                12
      or simply install A+W CAD Designer (Bars).
      After that please restart the A+W Planning 6 Service from the Windows Service Manager
      (services.msc).




A+W Software GmbH             EN-CONFIG-A+W Pattern Viewer.docx                           13
2. A+W Realtime Optimizer configuration
Important - Make a backup of the current entries so they can be restored if needed - either by
making a duplicate copy of the XOPTON.CFG (Example - $XOPTON.CFG) file or saving the original
entry in the XOPTON.CFG.
Open the XOPTON.CFG file under Notepad/Notepad++ from the following folder location -
C:\Program Files (x86)\A+W\Techsoft\XoptOn
Find the section [XTV] as shown below and make the following changes.
Change ServerName=127.0.0.1 to ServerName=1#TB1#001
Change Path=$USER$\XTV to Path=ICE




Also check the XOPTON.CFG file in the following path - %APPDATA%\A+W\Techsoft\XOPTON and
make the same changes as listed above (if required).
Save the XOPTON.CFG file(s) changes and then close all open screens.


2.1. RegisterForCurrentUser
With RegisterForCurrentUser you can automatically move the A+W Pattern Viewer with the
MachineLabel configured under ServerName in the ICEGrid at RTO startup so that the A+W
Pattern Viewer starts under the current user.
The A+W Pattern Viewer tray and all necessary configuration files are automatically adjusted or
created.
If a new MachineLabel is entered, an additional Pattern Viewer is created in ICEGrid.
In order for the switch to work, the A+W Pattern Viewer must be known in ICEGrid, i.e. the above
described A+W Pattern Viewer configuration must be run at least once per ServiceLocator (i.e.
usually once at the customer's site).




A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                                14
2.2. A+W Infrastructure                              6        workflow               studio
   configuration
Open the Config Tools > A+W Infrastructure 6 Workflow Studio under the Blue A+W Desktop
Shortcut
From the top menu select Configuration > Settings > Reference Paths




Next to Folder click on the button with the … and then select the A+W Realtime Optimizer Path =
C:\Program Files (x86)\A+W\Techsoft\XoptOn folder then click Add




Under the A+W Infrastructure 6 Workflow Studio select from the top menu File > Load then
choose Pattern Viewer Default Workflow from the OpenWorflowDialog screen then click Open as
seen below.




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                             15
Some Activities are missing in the Toolbox
Choose File -> Add References… and point to the AW.Clarity.CIM.Cutting.Facade.dll in the XOPTON
Directory.
After that all Activities are shown in the Toolbox.


2.3. Known issue message
Issue - 'The type ‘InArgument(acccm:Pattern)’ of property ‘PatternIn’ could not be resolved.' Line
number '3' and line position '34'.




Cause - The user receives the following screen when opening the A+W Pattern Viewer Default
Workflow



A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                             16
Solution - Ensure the Reference Paths has an entry for the A+W Realtime Optimizer Path =
C:\Program Files (x86)\A+W\Techsoft\XoptOn is listed then try the step again.


2.4. Server with workstation A+W Pattern Viewer
   configurations
The following section is dedicated to the purpose of detailing the setup of A+W Pattern Viewer on
a Workstation while the A+W Pattern Viewer Workflow Studio customizing is run off an A+W
Process Server.
Note - It is not possible to have two systems setup with the same A+W Pattern Viewer registration
(Example - 001#RTO1#001) on different computers, as this stops the registration working on the
second registered system. This string is unique in the network and it is also possible to start the
A+W Pattern Viewer remotely on another server.


First Registration - Server with A+W Pattern Viewer Configuration
    •   001#RTO2#001
    •   001#RTO3#001




Second Registration - Workstation with A+W Pattern Viewer Configuration
    •   001#RTO1#001




A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                              17
Correct - ICEGrid Configuration (Config Tools > Service Locator Administration Shortcut)
    •   001#RTO2#001 - AWPROC2019 (Server)
    •   001#RTO3#001 - AWPROC2019 (Server)
    •   001RTO1#001 - ClientRTO (Workstation)




2.5. A+W Realtime Optimizer usage
Transfer an order from A+W Business to A+W Production or use a previously released batch.
Open A+W Realtime Optimizer from under the Blue A+W Desktop Shortcut.
This will open A+W Realtime Optimizer and the A+W Pattern Viewer screens.



A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                          18
Under A+W Realtime Optimizer click on Cutting from the top menu.




Choose the previous A+W Production Batch that has been released then click on the Cut button.




This will open the Cutting Overview screen as seen below, click on the Start Button in the top
menu.




A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                               19
Finally, under the A+W Pattern Viewer program we will see the Stockplate Cutting Pattern
displayed on the screen.




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                          20
A+W Software GmbH   EN-CONFIG-A+W Pattern Viewer.docx   21
3. A+W Pattern Viewer workflow studio
  customizing
3.1.1. Setting starting point of the pattern
In some instances, it maybe required that the breakpoint (start point) of the stockplates needs to
be changed to a different corner than the default at the bottom left.
This is possible by changing the StartPoint found under the ChangeStartOfBreakage entry under
A+W Pattern Viewer Default Workflow under the A+W Infrastructure 6 Workflow Studio.




BottomLeft:




TopLeft:




A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                              22
TopRight:




BottomRight:




A+W Software GmbH   EN-CONFIG-A+W Pattern Viewer.docx   23
3.1.2. AddCustomText
AddCustomText - Add Customer Name To Order Item
The A+W Pattern Viewer Workflow also provides the ability to add a custom field to the glass
based on a SQL Statement.
Open A+W Infrastructure 6 Workflow Studio > Pattern Viewer Default Workflow >
AddCustomText


Use one of the following SQL options
Version 1 - select distinct pool_auftrag.kunde_name1 from pool_auftrag inner join
awbar_bearbeit on pool_auftrag.auftnr=awbar_bearbeit.auftnr where
awbar_bearbeit.etikettnr = #barcode#
Version 2 - select distinct pool_auftrag.kunde_name1 as Customer from pool_auftrag
inner join awbar_bearbeit on pool_auftrag.auftnr=awbar_bearbeit.auftnr where
awbar_bearbeit.etikettnr = #barcode#




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                              24
If we then move the mouse cursor over a cut, we can see in the Lite information popup box the
kunde_name1 field from the Select SQL statement.




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                               25
Version 1 Result




In the Version 2 script we have setup an alias for the kunde_name1 field as Customer and when
we use this, we can see the result below.
Version 2 Result




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                               26
3.1.3. AddCustomType
AddCustomType - Highlight Order Items In A Custom Color That Have A Matching Processing
The A+W Pattern Viewer Workflow also provides the ability to color glass based on a SQL
Statement.
Open A+W Infrastructure 6 Workflow Studio > Pattern Viewer Default Workflow >
AddCustomType


Color selection




First, we are going to set the Color to Value 1 = Orange.
On the right hand side click on the drop down box next to the entry CheckForCustomType and
then choose the CustomeType color wanted from the list above.




Now we are going to identify which processing we want to highlight.
In this example we will select the Edger Seaming Machine.
Order 21282 - Seaming A+W is due on the Edger Seaming Machine - 310


A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                           27
Order 21283 - No Seaming Due




This will cause the colored to match on the Order 21282 Item only
The Seaming Processing is attached to the Processing Article = 900. The reason why we selected
the Processing Article is because if we use a specific machine it may not match to the item.




Use the following SQL
select etikettnr from awbar_bearbeit where etikettnr=#barcode# and art_nr = '900'




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                            28
A+W Software GmbH   EN-CONFIG-A+W Pattern Viewer.docx   29
3.1.4. ReferenceMark
ReferenceMark – Show an Icon for Stamps, Logos or Reference Marks
The A+W Pattern Viewer Workflow also provides the ability to show a picture on the location of a
stamp or a logo.
So that the exact item and the position can be determined, the AWSOA.CAD.SheetsService and
the AWSOA.CIM.Barcoding Service are required.
Please install these first. So that the Sheets Service is filled with the CAD Designer (Shapes) items,
the following entry must be made in the SN.ini:
        [User]
        RegisterModelInSheetsService = 1

So that the logos and stamps are also active in cutting, it must be ensured that they are not in the
switch UNICUTRemoveProcessing:

        [View]
        ;remove LOGO from the Remove List ->show LOGO (and export LOGO) in UNICUT
        UNICUTRemoveProcessing = ......

Adjusting the workflow
Next, the workflow must be adjusted. For this, the lites and the barcoding service must be created
in the arguments.
To do this, first add the references to AW.Clarity.CIM.Cutting.Facade.dll and
AWSOA.CIM.Barcoding.ServiceContracts.dll. Do this on the File->Add Reference menu and add
the two files one after the other from the Techsoft\XOPTON directory. Alternatively, the directory
from the Pattern Viewer Tester also works if the A+W Realtime Optimizer is not installed locally.

Then, under Arguments, click Create Argument and create the SheetsService and the
BarcodingService.




A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                                 30
Under Argument Type, select the IBarcodingService and the ISheetService.




Under Argument Type, select the IBarcodingService and the ISheetService.




A+W Software GmbH              EN-CONFIG-A+W Pattern Viewer.docx           31
The arguments list should look like this:




Now we can attach the ReferenceMark Activity and set the properties.



A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx    32
Finally, the AfterWorks step in the A+W Production scheduling must be activated.
For this, add the entry AfterWorks; 1 in the sequence for order import.




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                  33
If you want to change the logos, you can use the tool under
\\jupiter\SW_Install\Tools\LogoActivityHelper. With it, you can transform your own pictures to a
Base64 string and enter it under Logo1Base64 and Logo2Base64.



3.1.5. MirrorStripe
Reverses all stripes in a travere.


3.1.6. MoveWaste
Shifts the rest to the other side of the selected stripe.
The TrimSize specifies starting with which size the "rest" is considered so that no trim is shifted.




Original:



A+W Software GmbH                    EN-CONFIG-A+W Pattern Viewer.docx                                 34
Move waste:




A+W Software GmbH   EN-CONFIG-A+W Pattern Viewer.docx   35
3.1.7. RemoveAdditionalText
Removes undesired default texts, it is not possible to remove the barcode since this is the key for
further activities.




3.1.8. Format Rack
With this activity, the slot in the rack number can be marked.




3.1.9. Prefix2ndGlassType
With this activity, a prefix for the text of the 2nd glass type can be specified in order to avoid
mistaken interpretations, e.g. if the rack number is single-digit.




A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                                  36
A+W Software GmbH   EN-CONFIG-A+W Pattern Viewer.docx   37
3.1.10.         Add2ndGlassTypeToAdditional
With this activity, the "ReferenceText" (8725 in the figure) can also be displayed in the additional
information area. Then you can switch off the reference text in the PatternViewer and for marrow
lites, achieve larger texts. With the title, you can place the text in the left column in the ToolTip.




A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                                38
3.1.11.         Change Sequence
With this activity, the "breakout sequence" can be set to a new sequence that has nothing to do
with the original breakout sequence.
The activity has the following configuration parameters:
1) StartAtCorner : Possible values are "BottomLeft", "BottomRight", "TopRight" and "TopLeft".
2) SequenceDirection : Possible values are "Row" and "Column".
3) Tolerance: Maximum distance in mm from the first lite found
4) RestartAtOne : Possible values are true and false. If true, the sequencing begins with 1;
otherwise with the smallest sequence number found in the pattern.
5) StopRenumberingAtSheetAtSensor : Possible values are true and false; if set to true, a new first
lite is searched for if the current first lite receives a sequence number.
The first two parameters determine the flow of the sequence; e.g., BottomRight and Column
mean that the lites on the right side receive the first sequence numbers beginning from the
bottom, then the same things is done on the left side, from bottom to top.


The lites are sorted according to the smallest distance to the transport edge, e.g., with
BottomRight and Column, this is the right edge.
Then all lites that are within the start of the first lite and the tolerance parameter added to the
first lite are sorted according to the SequenceDirection, e.g., for BottomRight and Column, this is
the distance from the lower edge. The lites receive the new sequence number in this sequence. If
the fifth parameter is set to true, only the lites up to the first lite receive a sequence number.
Now this document will repeat for lites without new sequence number until all lites have received
a new sequence number.
If RestartAtOne is set to true, the sequencing begins with 1; otherwise with the lowest sequence
number that was found on the pattern before the renumbering.



3.1.12.         Processing marker
In expansion of the activity "ReferenceMarker", it is now possible to display a symbol for any
processing. For this, the activity of the processing type must be stored in the parameters for the
activity under "ProcessingType".

The information about the turning behavior (Flipstatement) is now determined another SQL
command:

select etikettnr,cutmirror from fein_unit where job = lauf and etikettnr in (#barcode#) and typ =
100

For performance reasons, the information is read here for several labels at the same time;
therefore, here in the unlikely case that you would like to change this SQL, you must absolutely
pay attention to this logic.



A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                                 39
3.1.13.         Remove depiction of the support edge

If this activity is added to the workflow, then the markings for the support edge (triangle) are
removed for all lites.




A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                                40
3.2. Table-dependent workflows
So that different workflows can be executed per table or per MachineLabel, a so-called extension
point has to be created in the workflow service.
At the moment, unfortunately this only works with the following SQL statement (example for
table: 001#TB1#001:
SQL Server
insert into Core_WFActivityAssignments
(Guid,VersionId,ExtensionPoint,WorkflowType,Token)
values(NEWID(),1,300,300,'100#TB1#001')
Informix under Windows
insert into Core_WFActivityAssignments (Guid,VersionId,ExtensionPoint,
WorkflowType,Token) values(makeguid(),1,300,300,"1#TB2#001")
Informix under Linux
insert into Core_WFActivityAssignments (Guid,VersionId,ExtensionPoint,
WorkflowType,Token) values(makeguid()::char(36),1,300,300,"1#TB2#001")


After that, you can assign a workflow to the table with the MachineLabel via the workflow
management.




If the table is not listed there, then the default 0300 – PatternViewer is used.




A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                           41
3.3. Workflow clean up scripts
During the history of the programs usage archive entries may appear under the Workflow Studio
> OpenWorkflowDialog box where an unwanted A+W Pattern Viewer name is listed.
These unwanted entries need to be manually deleted from the database with 2 SQL commands
shown below.
Example - Workflow Cleanup Entry




Use the following SQL Templates
delete from Core_WFActivityArchives where wfactivityguid in (select distinct guid
from core_wfactivities where description = 'NAME')
delete from core_wfactivities where description = 'NAME'
Example - Workflow Cleanup Script
delete from Core_WFActivityArchives where wfactivityguid in (select distinct guid
from core_wfactivities where description = 'Workflow Cleanup')
delete from core_wfactivities where description = 'Workflow Cleanup'
Example - Workflow Cleanup Result




3.4. Breakage reason
On the A+W Pattern Viewer screen select the A+W Logo at the top of the screen and select
Breakage Reasons.




A+W Software GmbH              EN-CONFIG-A+W Pattern Viewer.docx                            42
On this dialog, you can select whether you want to use breakage reasons (option Use Breakage
Reasons) and specify the new reasons. Here you can enter any breakage reasons; however, the
values should match the values from the table AWBAR_STATE since the RTO writes the breakage
reasons to the database.
In the Combobox you can choose Standard to configure all Tables (A+W Pattern Viewer
registrations), or you can choose the registration (1#RTO3#001) to configure special breakage
reasons for a specific table.
In the current version of the A+W Pattern Viewer, you have to enter the breakage reasons
manually. In the future, the file takeover is planned.




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                               43
4. Configuration
4.1. Rotating subplates automatically
It is possible to rotate the subplates automatically if the size ratio of the rotated subplates fits
better on the screen.
This can be switched on with a switch on the ribbon bar:




The result then looks like this:
Original:




Rotated:




A+W Software GmbH                  EN-CONFIG-A+W Pattern Viewer.docx                                   44
5. A+W Push Button Tool
A+W Push button is a small application that takes over control of the keyboard
(serial/USB/wireless).
The tool monitors the input devices (serial or keyboard) and if necessary, sends the control
commands remotely via the network to the A+W Pattern Viewer.
Depending on the operating mode of the pattern viewer, the remote control can be zoomed and
forwarded (RTO) mode, or forwarded and breaks generated (DynOpt mode).


Ice Settings
In A+W Push Button, you configure it like this:




Important is the ICE Host and the ICE Port; you must enter the ICE Service Locator (ICE Registry)
there. The Machine Label is also important; with that, it is clear to which table the signals should
be sent.


Serial button




The serial button is connected via a serial interface (serial port: COM x). The Ice settings must be
configured.
On the status bar, you will see the result when someone presses a button; then you will see there
which signals were received via the serial line.
With Reverse Holding, you can set whether the action is executed when pressed (setting on) or
when released (setting off, default setting); with Switch Serial Buttons, you can logically exchange
both buttons of the serial buttons.
Keyboard Settings

A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                                45
In contrast to the serial COM interface, direct access to the USB pins is not possible; special
Windows licenses are required for this, which only certified hardware manufacturers can obtain.
Therefore, all USB-based devices (switches, buttons, keyboard, mouse, etc.) use the HID - human
interface device, which forwards keypresses to the operating system. A+W Push Button can record
these keypresses and then send actions to the Pattern Viewer.




To record the keypresses, Use Keyboard must be activated.
The standard actions Accept / Zoom and Breakage / Next correspond to the green and red buttons
on the serial buttons. There a button can, if this key is sent on the keyboard or on another USB
device, trigger the action in the Pattern Viewer.
If breakage reasons are activated in the Pattern Viewer, then the breakage reasons resurface in the
interface and can also be assigned a keypress. If the breakage reasons are changed in the Pattern
Viewer, then A+W Push Button must be restarted so that the changes are active there.

Test mode




If you have set ICE Host, ICE Port and Machine Label and a connection could be established to the
A+W Pattern Viewer, then the status bar turns green.
In this state, you can click the mouse somewhere in the window in A+W Push Button and thus
trigger Accept/Zoom with a left-click or Breakage/Next with a right-click. Please note that here you
do not click on the control lamp to the right next to Accept/Zoom or Breakage/Next; for technical
reasons, no signal can be sent then. You must click the mouse on an empty white area. Best suited
for this is the free area next to the lamp, marked on the screen with a blue rectangle.




A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                               46
Radio mushroom button
The radio mushroom button connects wirelessly with a USB dongle and simulates a configurable
keypress.
For this, you start the "Key Configurator" tool; there, you can see the connected mushroom
buttons and set the keypress to be set:




These settings must match the configured action in A+W Push Button.




A+W Software GmbH               EN-CONFIG-A+W Pattern Viewer.docx                            47
6. Ice know how
6.1.1. Pattern tray and IceNode
When two processes need to communicate with each other (RTO and PV), there is a client and a
server.
The client is always the active one that drives the process, the server is the service provider that
only becomes active when it is asked.
For a service to be queried, the service must either be running or started.
Under ICE the role of the service starter is taken over by ICENode.exe (C++ services) or
ICENodeNet.exe (C# services).
Normally our ICE services are all without user interface and run under a service account. In this
case the IceNode(Net) are started by a Windows service.
This is not possible in the case of A+W Pattern Viewer, because under Windows a service account
cannot get access to the desktop.
So the node must be started by a process running under the current user. This process is called
AW.Clarity.PAtternViewer.Tray.exe, it can be seen in the task bar as A+W NodeOrganizer.
If this Tray Application is not running, no A+W Pattern Viewer can be started!
The node can be started and stopped in the context menu of the tray. The result can be followed
in the ICEGrid: The node from A+W Pattern Viewer is started and stopped.
The IceNodeNet.exe which is started from the tray is configured via a file. This file is located at
C:\ProgramData\A+W\Sandpiper1\PatternViewer\Nodes and has the name
"config.%USERNAME%.node".
The RTO switch "RegisterForCurrentUser" takes over the complete configuration.


6.1.2. Callback
Normally the RTO starts the A+W Pattern Viewer and creates the communication between RTO
and A+W Pattern Viewer.
But in order for the A+W Pattern Viewer to report broken lites and to confirm pattern or lites, the
A+W Pattern Viewer needs a back channel to the RTO.
The back channel is called an ICE callback and is created at the A+W Pattern Viewer start. If the
A+W Pattern Viewer is closed by mistake, the next call from the RTO will automatically restart the
A+W Pattern Viewer. There is a logic implemented in the A+W Pattern Viewer, which checks for
the back channel and tries to reactivate it if needed.
During error analysis always remember that there are two independent connections, if one
direction has a problem, the other one can still work. If the communication is broken for some
reasons and couldn’t repair automatically, a RTO restart should help.




A+W Software GmbH                 EN-CONFIG-A+W Pattern Viewer.docx                                   48
7. Research options
   •   Processing not found (e.g. reference mark/logo/etc.)The SQL from the workflow activity
       should return a line for the questionable barcode
   •   Use of the SheetsService
       If the Sheets Service is used, then in the trace (XOPTON_NET.awtrc) you will find the
       query to the Sheets Service and also the result.
       Under \\jupiter\SW_Install\Tools\CAD Sheets Admin Tool you will find a tool with which
       you can query the SheetsService; in addition the tool provides SQL statements with which
       you can research yourself on the SOA database.
       Here too, the query must be successful; if it is not, then you must look in the import why
       the lites have not been exported to the SheetsService. If there are problems there, then
       you should look in the trace of the Sheetsservice and if necessary, increase the trace level.
   •   Use of the Barcoding Service
       The Barcoding Service is used to determine the order number and item number of the
       lite; the Pattern Viewer initially knows only the barcode. If there are problems there, then
       you should look in the trace of the BarcodingService and if necessary, increase the trace
       level.
   •   Use the PatternTester
       With the PatternTester, you can open SaveFiles quickly and easily and let the workflow
       run.
       In this case it is not the XOPEON_NET trace but rather the trace of the PatternTester
       where you can go to look for errors.
   •   Trace PatternViewer
       The PatternViewer itself hardly has logic; it only displays the pattern. Generally the
       pattern is generated incorrectly, the logic for this takes place in the RTO, in the Cutting
       Service, in the Furnace Client, PatternTester, etc. An analysis of PatternViewer trace is
       seldom required or useful.
   •   Ticket to development
       Generally the development needs the SaveFile and if necessary the Block.ZIP file. If
       processings or other customizings are affected in the workflow, it can be that the
       database is also required. Generally it is not sufficient to send a screenshot.




A+W Software GmbH                EN-CONFIG-A+W Pattern Viewer.docx                                   49

