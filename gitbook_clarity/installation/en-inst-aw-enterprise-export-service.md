---
description: "EN INST A+W Enterprise Export Service"
---



# EN INST A+W Enterprise Export Service

        Installation Instructions

        A+W Enterprise 6 Export Service
   Change history:
    Date          Edited by                 Remarks                                    Version
    16.04.22      MP                        New creation                               1.0
    16.10.04      SVH                       Addition                                   1.1
    16.12.13      MP                        AutoUpdate                                 1.2
    17.12.14      MP                        Multi DB configuration                     1.3




     The installation instructions will assist the planner with the installation and
     configuration process for the software named. Please proceed in the following
     sequence:


     1. Check the installation requirements.

     2. Compile the required data, additional programs, drivers, etc.

     3. Note or determine the time required.




19.04.2018                       EN-INST-A+W Enterprise Export Service.docx              1
Content

   1         Installation of the A+W Enterprise 6 Export Service............ 3
   1.1       Overview and the basics ............................................................................ 3
   1.2       Time requirement ....................................................................................... 3
   1.2.1     Installation time for the software ................................................................. 3
   1.3       Requirements ............................................................................................. 4
   1.3.1     Windows Server Version ............................................................................ 4
   1.3.2     Network ...................................................................................................... 4
   1.3.3     Software ..................................................................................................... 4
   1.4       Procedure ................................................................................................... 4
   1.5       Incompatibilities ........................................................................................ 11
   1.6       Directory structure .................................................................................... 12
   1.7       Result of the installation ........................................................................... 12
   1.8       Configuration ............................................................................................ 12
   1.9       Tips and tricks .......................................................................................... 12
   1.9.1     AutoUpdate .............................................................................................. 12
   1.9.2     Known errors and workarounds ................................................................ 12
   1.10      Uninstalling ............................................................................................... 12




19.04.2018                           EN-INST-A+W Enterprise Export Service.docx                                            2
1 Installation of the A+W Enterprise 6 Export Service
The following installation instructions assume that there is no previous version
installed.
An update of an earlier release version of the A+W Enterprise 6 Export Service is
executed precisely like a new installation.
An update of an earlier version of the Export Service, e.g. from ALCIB 2011 Export
Service to A+W Enterprise 6 Export Service is not possible. Only one version of the
Export Service should be installed.
This document describes only the installation and configuration of the A+W
Enterprise 6 Export Service. In case of questions about the installation or
configuration of dependent set-ups/disk sets, please see the installation instructions
for these products.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during
installation:
    -   Installation and configuration of the Informix driver via setnet32.exe
    -   Creation of the necessary set-ups/disk sets
            o A+W Enterprise 6 Export Service
            o A+W Infrastructure 6 Collector Services
            o A+W Infrastructure 6 Middleware
            o Java 7 Update 51
            o A+W Setup Launcher
    -   Installation of the Export Service and the dependent disk sets with the Setup Launcher
    -   Configuration of the Export Service with the ConfigTool

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


19.04.2018                      EN-INST-A+W Enterprise Export Service.docx                       3
1.3 Requirements
1.3.1 Windows Server Version
Supported operating systems:

    •   Windows 2008 Server R2 32/64bit.
    •   Windows 2012 Server R2 32/64bit.


1.3.2 Network
For the installation itself, no network access is necessary.
For the operation of the service, there must be a connection to the A+W Enterprise
DB Server and the company network.
1.3.3 Software
It is assumed that the following disk sets were already installed and configured BEFORE the
installation of the A+W Enterprise 6 Export Service disk set.

    •   Informix Client SDK 3.5 TC9 (or newer)
    •   Microsoft .NET Framework 4.5.1 SDK



1.4 Procedure
For the installation, please proceed in the following sequence:
1. Use setnet32.exe to configure the database server and hosts. This assumes that an IBM Informix
   Client SDK was installed (see software requirements).

2. Installation of the A+W Enterprise 6 Export Service with the Setup Launcher

    On the Component Selection dialog on the A+W Enterprise node, select the "A+W Enterprise 6
    Export Service" module. This automatically selects all dependent set-ups.




19.04.2018                      EN-INST-A+W Enterprise Export Service.docx                       4
3. After the successful installation, the Export Service is configured with the Config Tool.

    3.1. Common Settings




19.04.2018                       EN-INST-A+W Enterprise Export Service.docx                    5
        3.1.1.   Polling Interval

                 In the Polling Interval (Seconds) field, the number of seconds is set that the service
                 waits until it checks the printtransfer transfer table again for new data records. The
                 default value is 18 seconds.

        3.1.2.   Maximum Number of Attempts

                 In the Maximum Number of Attempts field, the number of attempts is specified that
                 the Export Service makes to start processing again in case of an error (e.g. PPS
                 Webservice not available). The default value is 10.

        3.1.3.   Protocol-Button

                 With the Protocol button, you can reach the Protocol Configuration dialog. This
                 automatically selects all dependent set-ups. On the first tab, the trace categories for
                 the frontend are configured; on the following tabs, the tracing of dependent modules
                 and programs can be activated if necessary.




19.04.2018                          EN-INST-A+W Enterprise Export Service.docx                         6
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
             consists of the service name, the current date and the process number and ends with
             .awtrc.

         The A+W Enterprise Export Service currently uses no log protocol.




19.04.2018                        EN-INST-A+W Enterprise Export Service.docx                               7
    3.2. Database settings

        On this dialog, all database-precise settings are configured, starting with the database itself.




             o   With the New button, you can edit an existing configuration.
             o   With the Edit button, you can delete an existing configuration.
             o   With the Delete button, you can delete an existing configuration.
             o   With the Copy button, you can copy an existing configuration. So that there are no
                 problems with identical configurations, the configuration created this way is initially
                 deactivated and the value ENTER_NEW_DATABASE_NAME is entered in the
                 Database Name field. Otherwise, all settings are taken over 1:1.
             o   With the De/Activate button, individual database configurations can be deactivated or
                 activated again. Thus, for example, the processing of ottransfer records on a
                 database server can be interrupted without having to delete the entire configuration.




19.04.2018                       EN-INST-A+W Enterprise Export Service.docx                                8
        3.2.1.   Site Properties

                 With the New or Edit buttons or with a double-click on a row in the table, you reach
                 the Site Properties dialog. Here, all database-dependent settings can be made.




        3.2.2.   Site Settings
            o    The Config No field contains a sequential number. The field is filled automatically.
            o    With the Active Connection checkbox, the database configuration can be activated or
                 deactivated. Only active configurations are considered by the Export Service for the
                 processing of print jobs.
             o   In the AWE Site field, a site number can be entered. If this field is empty or 0, the
                 export service will process all documents for this configuration, as previously.
                 If an actual client number was defined, only data records of exportinfo are processed
                 where exportinfo.hausnr matches this value.

        3.2.3.   Database settings
            o    The database server is entered in the Server Name field. Via the combo box, all DB
                 servers entered in the setnet32 can be selected.
             o   A user name that has access to the database must be entered in User Name.


19.04.2018                         EN-INST-A+W Enterprise Export Service.docx                            9
             o   If the fields Server Name, User Name, and Password are filled with valid values, the
                 Database Name combo box already contains all available database names of the
                 database server.
             o   The appropriate locale settings are entered in the Client Locale and DB Locale fields.
                 The combo boxes already contain most values used. If it is necessary to enter
                 deviating values, this is also possible manually.

        3.2.4.   DB Functions
            o    With the Start Setnet32 button, it is possible to start the setnet32.exe program
                 directly; with it, database server/hosts can be set up.
             o   With Check Alenv you can check the A+W Enterprise environment variables for this
                 service and view the current database configuration. Since this dialog is only for
                 checking purposes, it will not be described in any more detail. The settings of the
                 Alenv variables are made in A+W Enterprise.
             o   The Test Connection button allows you to check the current values of the database
                 configuration. If a database connection can be established with this values, you will
                 see the following message box; otherwise an error message.




19.04.2018                       EN-INST-A+W Enterprise Export Service.docx                              10
    3.3. Windows Service configuration




        The service users are stored on the Windows Service Configuration dialog. These are
        Windows users who are used to access external objects such as network paths, etc. This
        user must have the appropriate rights.

        With the Pick user... button it is possible to select a domain user.

        If no network domain is available, e.g. because the service was installed on a PC, the value
        "." can be entered in field Domain.

        If no user is available, the service can also run under "LocalSystem" in case of emergency.
        This is the default services user in a Windows system.

4. Now the A+W Enterprise 6 Export Service is ready and it writes a log into the directory named
   above.

5. Setting of A+W Enterprise environment variables



1.5 Incompatibilities
        No incompatibilities are known.


19.04.2018                       EN-INST-A+W Enterprise Export Service.docx                       11
1.6 Directory structure


1.7 Result of the installation
        If the service could be started, the installation was successful. Otherwise,
        the trace log is available for determining possible problems.

1.8 Configuration
        For additional     configurations,        please       see        the   Export   Service
        documentation.

1.9 Tips and tricks
1.9.1 AutoUpdate
        In order to be able to install the service via AutoUpdate, the setup must
        have been installed successfully at least once with the Setup Launcher and
        configured with the ConfigTool.
1.9.2 Known errors and workarounds

1.10 Uninstalling
You can uninstall the program as usual via Control Panel -> Programs and
Functions.




Note: The config file is not deleted automatically. For a final uninstallation, the
program directory of the A+W Enterprise 6 Export Service must be deleted
manually.




19.04.2018                   EN-INST-A+W Enterprise Export Service.docx                            12

