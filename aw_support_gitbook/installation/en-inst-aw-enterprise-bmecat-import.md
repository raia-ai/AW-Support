---
description: "EN INST A+W Enterprise BMECat Import"
---



# EN INST A+W Enterprise BMECat Import

        Installation Instructions

        A+W Enterprise 6 BMECat Import
   Change history:
    Date          Edited by                Remarks                                     Version
    16.04.22      MP                       New creation                                1.0
    16.12.13      MP                       AutoUpdate                                  1.1




     The installation instructions will assist the planner with the installation and
     configuration process for the software named. Please proceed in the following
     sequence:


     1. Check the installation requirements.

     2. Compile the required data, additional programs, drivers, etc.

     3. Note or determine the time required.




23.01.2023                      EN-INST-A+W Enterprise BMECat Import.docx                1
Content

   1         Installation des A+W Enterprise 6 BMECat Import............... 3
   1.1       Übersicht und Grundsätzliches ................................................................... 3
   1.2       Zeitbedarf ................................................................................................... 3
   1.2.1     Installationszeit für die Software ................................................................. 3
   1.3       Voraussetzungen........................................................................................ 4
   1.3.1     Windows Server-Version ............................................................................ 4
   1.3.2     Netzwerk .................................................................................................... 4
   1.3.3     Software ..................................................................................................... 4
   1.4       Vorgehensweise ......................................................................................... 4
   1.5       Inkompatibilitäten ....................................................................................... 9
   1.6       Verzeichnisstruktur ..................................................................................... 9
   1.7       Ergebnis der Installation ............................................................................. 9
   1.8       Konfiguration .............................................................................................. 9
   1.9       Tipps und Tricks ......................................................................................... 9
   1.9.1     Bekannte Fehler und Workarounds ............................................................ 9
   1.10      Deinstallation .............................................................................................. 9




23.01.2023                           EN-INST-A+W Enterprise BMECat Import.docx                                             2
1 Installation of the A+W Enterprise 6 BMECat Import
The following installation instructions assume that there is no previous version
installed.
An update of an earlier release version of the A+W Enterprise 6 BMECat Import is
executed precisely like a new installation.
An update of an earlier version of the BMECat Import, e.g. from ALCIB 2011
BMECat Import to A+W Enterprise 6 BMECat Import is not possible. Only one
version of the BMECat Import should be installed.
This document describes only the installation and configuration of the A+W
Enterprise 6 BMECat Import. In case of questions about the installation or
configuration of dependent set-ups/disk sets, please see the installation instructions
for these products.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during
installation:
    -   Installation and configuration of the Informix driver via setnet32.exe
    -   Creation of the necessary set-ups/disk sets
            o A+W Enterprise 6 BMECat Import
            o A+W Infrastructure 6 Collector Services
            o A+W Infrastructure 6 Middleware
            o Java 7 Update 51
            o A+W Setup Launcher
    -   Installation of the BMECat Import and the dependent disk sets with the Setup Launcher
    -   Configuration of the BMECat Import with the ConfigTool

1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data:
1.2.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times
will vary for different computers. The installation time specified was determined
using a reference device with the following characteristics:
    -   Processor: 3000 Mhz
    -   RAM: 4 GB
    -   Other: /
For an initial or new installation, an installation time of 5 minutes must be anticipated
for the reference device. For higher or lower-power hardware, shorter or longer
installation times must be anticipated.


23.01.2023                     EN-INST-A+W Enterprise BMECat Import.docx                        3
1.3 Requirements
1.3.1 Windows Server Version
Supported operating systems:

    •   Windows 7, 8, 8.1 32/64bit
    •   Windows 2008 Server R2 32/64bit
    •   Windows 2012 Server R2 32/64bit


1.3.2 Network
For the installation itself, no network access is necessary.
For the operation of the service, there must be a connection to the A+W Enterprise
DB Server and the company network.
1.3.3 Software
It is assumed that the following disk sets were already installed and configured BEFORE the
installation of the A+W Enterprise 6 BMECat Import disk set.

    •   Informix Client SDK 3.5 TC9 (or newer)
    •   Microsoft .NET Framework 4.5.1 SDK



1.4 Procedure
For the installation, please proceed in the following sequence:
1. Use setnet32.exe to configure the database server and hosts. This assumes that an IBM Informix
   Client SDK was installed (see software requirements).

2. Installation of the A+W Enterprise 6 BMECat Import with the Setup Launcher

    On the Component Selection dialog on the A+W Enterprise node, select the "A+W Enterprise 6
    BMECat Import" module. This automatically selects all dependent set-ups.




23.01.2023                     EN-INST-A+W Enterprise BMECat Import.docx                         4
3. After the successful installation, the BMECat Import is configured with the Config Tool.

    3.1. Database settings




23.01.2023                      EN-INST-A+W Enterprise BMECat Import.docx                     5
             o   The database server is entered in the Server Name field. Via the combo box, all DB
                 servers entered in the setnet32 can be selected.
             o   A user name that has access to the database must be entered in User Name.
             o   If the fields Server Name, User Name, and Password are filled with valid values, the
                 Database Name combo box already contains all available database names of the
                 database server.
             o   The appropriate locale settings are entered in the Client Locale and DB Locale fields.
                 The combo boxes already contain most values used. If it is necessary to enter
                 deviating values, this is also possible manually.
             o   With the Start Setnet32 button, it is possible to start the setnet32.exe program
                 directly; with it, database server/hosts can be set up.

             o   The Test Connection button allows you to check the current values of the database
                 configuration. If a database connection can be established with this values, you will
                 see the following message box; otherwise an error message.




23.01.2023                       EN-INST-A+W Enterprise BMECat Import.docx                            6
        3.1.1.   Protocol-Button

        With the Protocol button, you can reach the Protocol Configuration dialog. This automatically
            selects all dependent set-ups. On the first tab, the trace categories for the frontend are
            configured; on the following tabs, the tracing of dependent modules and programs can be
            activated if necessary.




23.01.2023                         EN-INST-A+W Enterprise BMECat Import.docx                         7
             The following trace levels are distinguished:
             o Fatal
             o Error".
             o Warning
             o Info
             o Debug

             With the Protocol button, you can reach the Protocol Configuration dialog. If, for example,
             the Info level is active, trace messages of the type Error and Warning will also be written
             into the tracing file.

             The tracing file is always in the directory %ProgramData%\A+W\Log. The file name
             consits of the service name, the current date and the process number and ends with
             .awtrc.

             The A+W Enterprise BMECat Import currently uses no log protocol.

4. Setting of A+W Enterprise environment variables




23.01.2023                       EN-INST-A+W Enterprise BMECat Import.docx                             8
1.5 IncompatibilitiesIncompatibilities
        No incompatibilities are known.

1.6 Directory structure


1.7 Result of the installationResult of the installation
If the service could be started, the installation was successful. Otherwise, the trace
log is available for determining possible problems.

1.8 Configuration
For additional configurations, please see the BMECat Import documentation.

1.9 Tips and tricks
1.9.1 AutoUpdate
        In order to be able to install the program via AutoUpdate, the setup must
        have been installed successfully at least once with the Setup Launcher and
        configured with the ConfigTool.
1.9.2 Known errors and workarounds

1.10 Uninstalling
You can uninstall the program as usual via Control Panel -> Programs and
Functions.




Note: The config file is not deleted automatically. For a final uninstallation, the
program directory of the A+W Enterprise 6 BMECat Import must be deleted
manually.




23.01.2023                  EN-INST-A+W Enterprise BMECat Import.docx                    9

