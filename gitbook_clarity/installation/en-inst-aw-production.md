---
description: "EN INST A+W Production"
---



# EN INST A+W Production

 Installation Instructions

 A+W Production 6
   Change history:
     Date            Edited by               Comments                                  Version
     08/2012         Jens Schmidt            Release                                   1.0
     2014-07-07      D.Langsdorf             Revision for SP5.4                        1.1
     2016-12-27      M. Schmidt              Revision for v6.2 + PT Licensing          1.2




     The installation instructions guide the consultant through the installation and
     the configuration process of the cited software. Please proceed in the
     following order:


     1.      Check the installation requirements.

     2.      Collect the necessary data, additional programs, drivers, etc.

     3.      Consider or calculate the time required.




08.05.2018                              EN-INST-A+W Production.docx                     1
Content

   Installation Instructions ................................................................... 1

   A+W Production 6 ............................................................................ 1

   1         Overview and Basics............................................................. 4
   1.1       Prerequisites .............................................................................................4
   1.1.1     Hardware ...................................................................................................4
   1.1.2     Network .....................................................................................................4
   1.1.3     Software ....................................................................................................4
   1.1.4     Database ...................................................................................................4
   1.1.5     Exchange directory ....................................................................................4
   1.1.6     Documentation and manuals .....................................................................5

   2         Installation ............................................................................. 6
   2.1       Procedure ..................................................................................................6
   2.2       Installation of A+W SetupLauncher ...........................................................6
   2.3       Component selection ...............................................................................13
   2.4       Module-based dialogs .............................................................................14
   2.4.1     Exchange directory ..................................................................................14
   2.4.2     Database connection parameters ............................................................15
   2.4.3     Enter the service users ............................................................................17
   2.4.4     Infrastructure Collector Service ...............................................................18
   2.5       Configuration ...........................................................................................19
   2.5.1     A+W ProductionComServer ....................................................................19
   2.5.2     Exchange directory ..................................................................................20
   2.5.3     Protocolling configuration ........................................................................21
   2.5.4     Database connection parameters ............................................................22
   2.5.5     Parameter from the production database ................................................23
   2.5.6     Plan Editor settings..................................................................................27

   3         Licensing ............................................................................. 29
   3.1       Production Terminal ................................................................................29
   3.1.1     Problem handling.....................................................................................31

   4         Tips and tricks ..................................................................... 40
   4.1       Uninstalling the Informix driver ................................................................40


08.05.2018                                  EN-INST-A+W Production.docx                                                  2
08.05.2018   EN-INST-A+W Production.docx   3
1 Overview and Basics
1.1     Prerequisites
1.1.1 Hardware
No special requirements.
1.1.2 Network
A+W Production 6 requires at least a 10 Mbit Ethernet (10Base2 / IEEE 802.3a,
10Base-T / IEEE 802.3i ) network, better Fast Ethernet or Gigabit Ethernet. Please
make sure that the client terminals can access the database.
1.1.3 Software
For A+W Production 6, Microsoft Windows 7 is the minimum requirement. For the
process server and terminal server, Windows Server 2008 R2 is required.

Please also remember to install all other available service packs for the framework
and the operating system. We recommend to always keep the server up to date with
the Microsoft Update Service.
The .NET Framework 3.5 SP1 is installed by A+W SetupLauncher. This installation
takes about 30 minutes! If possible, please install .NET Framework in advance (or
have it installed).
1.1.4 Database
Informix or Microsoft SQL Server 2008 is required as the database system.


1.1.5 Exchange directory
A+W Production 6 requires an exchange directory (also known as Trans or drive
P:). This directory must be set up prior to installation. Please make sure that the
necessary rights are available for this directory. All A+W Production users have to
have full access to this directory. These rights must be granted regarding safety
and regarding the release.




08.05.2018                      EN-INST-A+W Production.docx                           4
1.1.6 Documentation and manuals
The setup also includes the existing manuals in German and in English. They are located in
the exchange directory in sub-folder User_Manuals.




08.05.2018                        EN-INST-A+W Production.docx                            5
2 Installation
The setup for A+W Production 6 is available from \\jupiter\SW_Install\v6.

2.1     Procedure
        1. Please check the requirements
        2. Please make sure that you belong to the local group of administrators.
        3. Start Setup.exe.



2.2 Installation of A+W SetupLauncher
A+W SetupLauncher is the central installation and update tool of A+W Software GmbH.
After starting "SetupStartes.exe", the following warning may be issued which has to be
acknowledged by using the button "Install".




                       Fig.: 1        Installation of the Setup Launcher

While the A+W SetupLauncher is installed, .NET Framework 3.5 and Microsoft Windows
Installer 3.1 may be installed as well if necessary. When this installation is finished, the
program opens and the actual software to be installed can be selected.




08.05.2018                          EN-INST-A+W Production.docx                                6
    •   A splash screen appears.      Press [Next] to proceed.
    •   Dialog Diskset Selection opens.




        Fig.: 2        SetupLauncher – Diskset dialog




        Select the version to be installed. This version is just a preselection of set-up
        components which can be changed during the installation process.
        The shown sequence of packages should match the installation sequence. This
        means, if several packages are necessary on one server, the individual packages
        should be installed in the sequence displayed in the A+W Setup Launcher.
        These components are listed in section "Component selection".




08.05.2018                           EN-INST-A+W Production.docx                            7
        A dialog opens in which the directories have to be entered:




        Fig.: 3          SetupLauncher – Select the installation directory


                  Enter the path for the A+W Diskset in Diskset Folder.
                  (e.g. \\jupiter\SW_Install\v6\Diskset)
                  Enter a hard disk under Installation drive and the additional directory structure
                  is provided by the installation.

                  The A+W Setup Launcher features „Auto Update“ and „FTP Download“ are
                  described in detail in A+W Setup Launcher Dokumentation.

    •           Press [Next] to proceed.
    •   The following dialog shows the already installed A+W components. Press [Next] to
        proceed.




08.05.2018                             EN-INST-A+W Production.docx                                8
    •   A dialog opens to select the installed components.




        Fig.: 4       Setup-Launcher – Component selection


        Press [Next] to proceed.

    •   Maybe, further configuration dialogs appear.

    •   The, a dialog appears with the respective languages for A+W Production, which will
        be updated in the Text-Table of the Production database.




08.05.2018                         EN-INST-A+W Production.docx                               9
        Fig.: 5 SetupLauncher – Language update

    •   After this step further configuration dialogs follow.

    •   The following dialog allows to select the required action:




08.05.2018                           EN-INST-A+W Production.docx     10
        Fig.: 6         SetupLauncher – Starting the installation


             Install Software: Installs the selected packages without saving the parameters
             entered.

             Install Software and save setup configuration to a xml file: Installs the selected
             packages and saves the defined parameters in a .diskset file for further
             installations. This diskset can be selected from the Diskset Selection Control
             dialog afterwards.

             Only save setup configuration to an Xml file: This means that just a diskset file
             will be created. No software will be installed. This option serves for preparation
             purposes only.

             Manage Hotfixes: This means that the hotfix management is started.

        Select "Install Software and save setup configuration to a xml file" and press [Next].




08.05.2018                            EN-INST-A+W Production.docx                                 11
    •    The following dialog lists the individual components to be installed and configured.
         Installation of the individual components will start automatically.




        Fig.: 7        SetupLauncher - Progress display




08.05.2018                           EN-INST-A+W Production.docx                                12
2.3 Component selection

2 default disksets in SetupLauncher are available for A+W Production; they define which
components are to be installed.
Note: Please make sure that the A+W Infrastructure Services (for Logging, Tracing, etc.)
especially A+W Infrastructure Service Locater is installed.
Make sure that only one instance of the Service Locator exists in the customer network.


A+W Production Process Server – Installation of process server
A+W Production Terminal Server – Installation of terminal server or workstation




08.05.2018                        EN-INST-A+W Production.docx                              13
2.4 Module-based dialogs


2.4.1 Exchange directory




Fig.: 7 SetupLauncher - Exchange directory

Server Directory: Path where A+W Production finds the exchange directory. Please
enter the UNC path for the directory you have set up in step 1.5.
Server Volume: The preset P: should not be changed because it cannot be
guaranteed that all scripts read the value from the registry.




08.05.2018                        EN-INST-A+W Production.docx                      14
2.4.2 Database connection parameters




Fig.: 8 SetupLauncher - Connection parameters SQL Server

Please choose the database system and enter the connection parameters.
Alternative: Informix-Database system




08.05.2018                       EN-INST-A+W Production.docx             15
Fig.: 9 SetupLauncher - Connection parameters Informix




08.05.2018                        EN-INST-A+W Production.docx   16
2.4.3 Enter the service users




Fig.: 10 SetupLauncher - Service users

This dialog can be used to select a user for whom the services are executed.
SetupLauncher may want to know whether the user shall have the right to log in as a
service. Please enter Yes to confirm this




08.05.2018                         EN-INST-A+W Production.docx                        17
2.4.4 Infrastructure Collector Service




Fig.: 11 SetupLauncher – Collector Service

This inquiry is only shown when no infrastructure services have been installed on this
computer yet. As a host, enter the computer on which the infrastructure services and thus
the service locator have been installed. Enter 12000 as the port. It should only be changed if
it is already occupied in the system. This change must then be executed company-wide.




08.05.2018                         EN-INST-A+W Production.docx                              18
2.5 Configuration
2.5.1 A+W ProductionComServer
Define the user account that is in control of the A+W ProductionComServer execution.
Start the program 'Component Services' for this purpose (Control Panel/Administration).
Select the entry A+W ProductionComServer under DCOM configuration.




Select the function "Properties" in the context menu. Select the "Identity" tab in the dialog.

Enter a user with rights in the network, i.e. belongs to a domain.
The user must have the right to change Block.ind or Block.zip.

Ensure that for the user account that is used by A+W ProductionComServer

                                        •    the Brieve-32 bit driver has been installed
                                                (only applies if Block.ind is used).
                                        •    the right has been granted to change the file
                                        block.ind
                                             or block.zip.
                                        The path to the block database is defined in the
                                        file block.pth. If the path includes a drive letter,
                                        the drive letter must be connected with the
                                        network directory.




08.05.2018                          EN-INST-A+W Production.docx                                  19
2.5.2 Exchange directory




Server Directory: Path where A+W Production finds the exchange directory. Please
enter the UNC path for the directory you have set up in step 1.5.
Server Volume: The preset P: should not be changed because it cannot be
guaranteed that all scripts read the value from the registry.
User Directory Template: Location to save user settings and temporary files
Override User Directory: Activates the deviating user directory
Terminal server mode: Set to terminal server; cannot be changed and must be
activated on workstation. It activates Windows-compliant work by writing into the
Program Files directory.
Log File Mode: This settings determines whether the tracing for calculating geometries is
active only in case of errors (0: default) or always (1: default). The logging is always the same,
this settings only determines the trigger. This function is required for tracing so called
“Incorrect Cutting Sizes” in order to understand how the calculation was made.
Don’t map Server Directory: Drive P is not mapped




08.05.2018                           EN-INST-A+W Production.docx                               20
2.5.3 Protocolling configuration




Tracing and logging behavior for the application and all its integrated components
can be set. This is possible globally or per user.




08.05.2018                      EN-INST-A+W Production.docx                          21
2.5.4 Database connection parameters




This dialog serves to configure the database connection of A+W Production to its
production database.

Please choose the database system and enter the connection parameters. The
connection can be checked by means of the Test Connection button.




08.05.2018                     EN-INST-A+W Production.docx                         22
2.5.5 Parameter from the production database
Settings from the production database that must be reset when a system is
transferred can be changed now.




A+W Production Service User: User for whom the services run.
Shape Catalog: Shape catalog for the system.
A+W PPS Webservice: The URL where the PPS web service can be reached.




08.05.2018                    EN-INST-A+W Production.docx                   23
A+W ERP WebService: Parameter to address the ERP web services.




08.05.2018                  EN-INST-A+W Production.docx          24
Settings for the Block.ind access




08.05.2018                      EN-INST-A+W Production.docx   25
Setting for the licenses to be queried for certain modes of A+W Production.
Unless a different setting per station has been selected, the default configuration
applies globally for all stations. The corresponding license is subsequently
allocated on the license server.




08.05.2018                       EN-INST-A+W Production.docx                          26
2.5.6 Plan Editor settings
Subsequently, set the settings of the Plan Editor.




Here, the language of the Plan Editor is defined




Path to Block.ind with shape 99 parameters




08.05.2018                      EN-INST-A+W Production.docx   27
Selection of Shape catalog for Plan Editor




08.05.2018                      EN-INST-A+W Production.docx   28
3 Licensing
3.1 Production Terminal
Licensing of A+W Production Terminal is made in several steps and starts while
opening the respective version. The following components are part of the licensing:
    •   A+W Production Terminal
    •   A+W PPS Webservice
    •   A+W AWSOA Infrastructure License (AWSOA-Service)
    •   A+W LicenseClient


If a Production Terminal is started, then after selection of the mode to be started
and the user, a license query is started via the PPS Webservice. If after an update
it is executed for the first time or if initially a license is queried, the PPS Webservice
calls an internal component that asks the AWSOA service for the license in
question. The AWSOA service logs and initiates the query to the A+W
LicenseClient, which grants or refuses the license.
If the AWSOA service cannot be reached later (error, etc.), then an internal cache
mechanism in the component of the PPS Webservice ensures that the Production
Terminal will still temporarily have access to a valid license. This prevents
production shutdowns. The temporary use is indicated to the user for the fastest
possible elimination.


Summarized again in brief below:
    1. Start of the Production Terminal
    2. Query of the license via the PPS Webservice
    3. Forwarding of the query to the AWSOA service
    4. Granting/refusal of the license by A+W LicenseClient


While the Production Terminal is running, the license will be confirmed every 5
minutes with a "hold." This serves only the purpose of logging (for query of the
license usage duration). On exiting, the license is also "released" again with a
corresponding method. However, the current Production Terminal license it not a




08.05.2018                         EN-INST-A+W Production.docx                               29
limited volume license, so that both of these last steps currently serve only the
purpose of evaluation.
With respect to the evaluation, it must be mentioned that within the AWSOA
service, a Web interface can be called up, which displays the license queries of all
A+W programs in "compressed" form. Warning: this is not a real-time display!




View of the license data
This display shows the license data (duration, module, version, etc.) and the
respective duration of usage. You must note that current license queries are only
displayed after "compression" (once a day) and thus there is a brief offset.
Furthermore, "parallel use" is also visible, which displays the respective parallel
use of individual modules.




08.05.2018                       EN-INST-A+W Production.docx                           30
Parallel use
These displays should serve sales and planning to get an overview of the
customer's licenses and modules. Thus it is possible to point out bottlenecks to the
customer and to enable him to adjust his licensing in timely fashion.


3.1.1 Problem handling
The following section will explain important steps to take if the Production Terminal
does not start because it cannot get a license.
    1. Are all participating components installed and available?
             a. In particular: can the PPS service be reached and can the A+W
                LicenseClient reach the appropriate license server?
    2. Is the appropriate AWSOA service running?
    3. Is the appropriate Production Terminal license installed on the license server
       and can it be reached?


    Usually checking into these questions helps clarify licensing problems.




08.05.2018                       EN-INST-A+W Production.docx                            31
       Point 1 is each to check with the set PPS Webservice URL and the A+W
       LicenseClient Config Tool.
       Point 2 can best be checked with the "Service Locator Administration" tool. This
       can be found in the A+W Start menu folder under "Config tools."




       Initial view of the opened tool
       First you must connect to the respective "IceGrid registry," under which all A+W
       AWSOA services run and can be reached.
       The following steps describe how to add the connection:
1. Click the "Log into an IceGrid Registry" button in the top left. The following window
   opens:




2. Here, first the connection must be created once with "New Connection."


   08.05.2018                        EN-INST-A+W Production.docx                           32
    2.1. Direct Connection




    2.2. Master Registry




    2.3. Manuel Endpoint




    2.4. Hostname and port number




08.05.2018                    EN-INST-A+W Production.docx   33
    2.5. Localhost, 12000 and TCP




    2.6. Username und password (both are arbitrary, but not empty)




    2.7. Finish


After these steps, you should see the following view:




08.05.2018                      EN-INST-A+W Production.docx          34
Connection to AWRegistry
Links are now listed for all installed AWSOA services. For successful licensing, the
following service should be installed and started:




Infrastructure-License-001


08.05.2018                       EN-INST-A+W Production.docx                           35
3.1.1.1 Execution of the AWSOA service
If the AWSOA service "{Computername}-Infrastructure-License-{ClientId}" is not
started (you can see if something is started if there is an icon with a green arrow),
then it can be started with a right-click on "Start" on the context menu.
Here you can see that the start of the service also starts all dependent components
and services.
Usually, there are errors here: The service cannot be started. Here, a view of the
error output of the service to be started can help:




Now a window opens on which the start process is logged and errors are displayed
accordingly:




08.05.2018                       EN-INST-A+W Production.docx                            36
If the display does not show the complete list of errors, you can use "Edit >
Preferences" to increase the internal display of the characters and lines:




If you make adjustments here, then close the output and open it again (only then
are the settings applied).
The error messages logged can indicate missing components (usually after a
flawed update) or occupied or locked ports.


3.1.1.2 Logging and tracing of the AWSOA services
If the license service runs successfully, however, then the next thing you should do
is increase the tracing to find a possible cause.




08.05.2018                       EN-INST-A+W Production.docx                           37
For this, you should first start the "A+W Protocolling Config Tool" in which all
AWSOA services can be configured appropriately:




Here, select "Infrastructure License" in the combo box and click "Protocol."
On the dialog that appears, select the category "InfrastructureLicense" under
"AWSOA Infrastructure" and set the trace level for error tracing to "Debug."
Then you stop and start the license service in the Service Locator Administration
and try again to query a license by starting the Production Terminal. Now there
should be at least one entry with the appropriate category in the trace file for the
service; it describes possible causes.


If you cannot find any error here, you can also check whether the correct Production
Terminal license was installed – via A+W License Monitor – and whether the
license server can also be reached. There is an appropriate connection test in the
config tool of the license server. This test checks the connection to the license
server if it is on another computer on the network. If the license server is running
on the local computer, you can check with the display of the local services (e.g. in


08.05.2018                      EN-INST-A+W Production.docx                            38
the Task Manager) whether the license server has been started. With the "SafeNet
Aladdin Control Center (HASP Tool)" from the Config Tools folder, you can check
whether the dongle is connected correctly to the computer (for more information
about this, see the installation instructions for the license server, section 1.8).




08.05.2018                      EN-INST-A+W Production.docx                           39
4 Tips and tricks


4.1 Uninstalling the Informix driver
        During the installation of the Infomix driver an assembly redirect is entered
        into the machine.config.
        For this purpose, the key is



        replaced with




        Machine.config is located at two locations:
    •   C:\Windows\Microsoft.NET\Framework\v2.0.50727\CONFIG
    •   C:\Windows\Microsoft.NET\Framework\v4.0.30319\Config


        When you uninstall the Informix driver, you must reset these entries
        manually! This is not necessary when an update is executed!




08.05.2018                        EN-INST-A+W Production.docx                           40

