---
description: "EN INST A+W Planning Stock"
---



# EN INST A+W Planning Stock

          Installation Instructions

          A+W Planning Stock
   Change history:
     Date            Edited by              Remarks                                    Version
     2018.11.21      AKU                    Original version                           1.0




     The installation instructions will assist the planner with the installation and
     configuration of the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




29.01.2019                            EN-INST-A+W Planning Stock.docx                   1
Content

   Installation Instructions ................................................................... 1

   A+W Planning Stock ........................................................................ 1

   1         New Installation ..................................................................... 3
   1.1       Overview and the basics ...........................................................................3
   1.2       Time requirement ......................................................................................3
   1.2.1     Installation time for the software ................................................................3
   1.3       Requirements ............................................................................................3
   1.3.1     Network .....................................................................................................3
   1.3.2     Software ....................................................................................................3
   1.4       Procedure ..................................................................................................3
   1.5       Settings .....................................................................................................4
   1.6       Result of the installation ............................................................................4
   1.7       Uninstalling ................................................................................................5
   1.7.1     Checking the uninstallation........................................................................6

   2         Updates .................................................................................. 8
   2.1       Time requirement ......................................................................................8
   2.2       Procedure ..................................................................................................8
   2.2.1     The job service does not start ...................................................................8




29.01.2019                                 EN-INST-A+W Planning Stock.docx                                                2
1 New Installation
The following installation instructions assume that there is no previous version
installed. The set-up and additional configuration possibilities are described in the
start-up documentation.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during
installation:
    -   Installation of the Planning Stock Service
    -   Installation of the Job Service (dependency)
    -   Installation of the Planning Web

1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data: 30 minutes.
1.2.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times
will vary for different computers. The installation time specified was determined using
a reference device with the following characteristics:
    -   Processor: Intel Core i7 870
    -   RAM: 16 GB
    -   Other: Windows 8
For an initial or new installation, an installation time of 10 minutes must be anticipated
for the reference device. For higher or lower-power hardware, shorter or longer
installation times must be anticipated.

1.3 Requirements
Prerequisite is an A+W Infrastructure ProcessServer in the customer environment.
1.3.1 Network
The URL for the Stock function is:
http://servername/Planning.web/Stock
http://servername/CIM.web/SmartTerminalBooking
1.3.2 Software
An IIS (at least Version 8) must be installed and activated on the server.

1.4 Procedure
In the A+W SetupLauncher, the following points must be installed including their
dependencies:



29.01.2019                             EN-INST-A+W Planning Stock.docx                   3
    -   A+W Planning Stock Services
    -   A+W Planning Web
    -   A+W Planning Job Services


After the installation has been completed, the page must be called up in the browser
again so that the database tables are created.
To do this, go to the link: http://<servername>/Planning.web/
The initial execution can take a moment.

1.5 Settings
Since Version 6, the A+W Planning Job Service and the A+W Planning Stock
Service use switches to find the A+W Production database. These must be set in
the A+W Infrastructure. If the configuration is not correct, the services cannot be
started in the IceGrid.




1.6 Result of the installation
The services are addressed via browser (e.g. IE) in domain PLANNING.WEB. If
the page is not displayed in the browser, then you must check in the Service
Locator Administration (IceGrid Admin) whether the ICE services are registered
and can be started.
The log files for the service are here: %ProgramData%\A+W\Log\




29.01.2019                        EN-INST-A+W Planning Stock.docx                     4
Functions Residual Stock Management




1.7 Uninstalling
To uninstall the A+W Planning Stock Service, the installed programs must be
uninstalled using the standard Windows function "Programs and Features."




It is recommended that of the dependencies, you first uninstall A+W Planning Web,
then A+W Planning Stock, and then the A+W Planning Job Service.


29.01.2019                    EN-INST-A+W Planning Stock.docx                       5
1.7.1 Checking the uninstallation
Open "Services" and check whether the following Windows services were
removed:




    -   A+W Planning Stock Services
    -   A+W Planning Job Service

If the services are still present, you can remove them using the command line.
        1. Open the command line as administrator
        2. Open the Properties of the service that was not uninstalled.




29.01.2019                        EN-INST-A+W Planning Stock.docx                6
        3. Copy the "Service name" to the clipboard
        4. Close the Property window
        5. Enter the following on the command line: sc delete <service name>
Check whether the services were removed from the "Service Locator
Administration."




29.01.2019                     EN-INST-A+W Planning Stock.docx                 7
2 Updates
The following installation description only describes the points that differ from the
full installation described above and that must be heeded for an update.
An automatic update of the services is not possible since the procedures, precisely
those for installation, have changed between the versions. A manual uninstallation
of the services may be unavoidable under some circumstances.

2.1 Time requirement
15-30 minutes.

2.2 Procedure
If the Stock interface is not displayed or if it is not possible to enter a residue, then
you must check in the Service Locator Administration (IceGrid Admin) whether the
services are registered and started (see Result of the installation).
Required services:
    -   A+W Planning Stock Service
    -   A+W Planning Job Service
2.2.1 The job service does not start
For the Job Service, the A+W Production database connection must be stored in
the infrastructure. Otherwise, the service will not start (see Settings).




29.01.2019                           EN-INST-A+W Planning Stock.docx                        8

