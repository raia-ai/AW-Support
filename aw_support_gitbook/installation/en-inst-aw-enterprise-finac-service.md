---
title: "EN INST A+W Enterprise FinAc Service"
category: "installation"
product: "A+W Enterprise FinAc Service"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Enterprise FinAc Service"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions          A+W Enterprise 6 FinAc Service    Change history:     Date          Edited by                Remarks                                     Version     16.04.22      MP                       New creation                                1.0     16.10.04      SVH                      Addition                                    1.1     16.12.13      MP                       AutoUpdate                                  1.2     17.03.21      SVH"
source_file: "EN-INST-A+W Enterprise FinAc Service.pdf"
---


# EN INST A+W Enterprise FinAc Service

        Installation Instructions

        A+W Enterprise 6 FinAc Service
   Change history:
    Date          Edited by                Remarks                                     Version
    16.04.22      MP                       New creation                                1.0
    16.10.04      SVH                      Addition                                    1.1
    16.12.13      MP                       AutoUpdate                                  1.2
    17.03.21      SVH                      Additions/changes AWDesk #379226
    18.11.23      SVH                      Additions AWDesk #425206
    2021-12-16    SVH                      Addition [AW-84955], modifications
    2022-06-13    SVH                      Additions to Intrastat




     The installation instructions will assist the planner with the installation and
     configuration process for the software named. Please proceed in the following
     sequence:


     1. Check the installation requirements.

     2. Compile the required data, additional programs, drivers, etc.

     3. Note or determine the time required.




07.07.2022                       EN-INST-A+W Enterprise FinAc Service.docx               1
Content

   1         Installation of the A+W Enterprise 6 FinAc Service ............. 3
   1.1       Overview and the basics ............................................................................ 3
   1.2       Time requirement ....................................................................................... 3
   1.2.1     Installation time for the software ................................................................. 3
   1.3       Requirements ............................................................................................. 4
   1.3.1     Windows Server Version ............................................................................ 4
   1.3.2     Network ...................................................................................................... 4
   1.3.3     Software ..................................................................................................... 4
   1.4       Procedure ................................................................................................... 4
   1.5       Customer-specific configurations ............................................................. 22
   1.5.1     Open Amounts Import Settings ................................................................ 22
   1.5.2     Ongoing Orders Export Settings ............................................................... 23
   1.5.3     Customer-specific settings (account information) ..................................... 24
   1.5.4     Stock Movements Export Settings ............................................................ 25
   1.6       Incompatibilities ........................................................................................ 26
   1.7       Directory structure .................................................................................... 26
   1.8       Result of the installation ........................................................................... 26
   1.9       Configuration ............................................................................................ 26
   1.10      Tips and tricks .......................................................................................... 27
   1.10.1    AutoUpdate .............................................................................................. 27
   1.10.2    Known errors and workarounds ................................................................ 27
   1.11      Uninstalling ............................................................................................... 27




07.07.2022                            EN-INST-A+W Enterprise FinAc Service.docx                                            2
1 Installation of the A+W Enterprise 6 FinAc Service
The following installation instructions assume that there is no previous version
installed.
The update of an earlier release version of the A+W Enterprise 6 FinAc Service is
performed exactly as a new installation.
The update of an earlier version of the FinAc Service, e.g. A+W Enterprise FinAc
Service to A+W Enterprise 6 FinAc Service is not possible. There should always
only be one version of the FinAc Service installed.
This document describes only the installation and configuration of A+W Enterprise 6
FinAc Services. In case of questions about the installation or configuration of
dependent set-ups/disk sets, please see the installation instructions for these
products.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during
installation:
    -   Installation and configuration of the Informix driver via setnet32.exe
    -   Creation of the necessary set-ups/disk sets
            o A+W Enterprise 6 FinAc Service
            o A+W Infrastructure 6 Collector Services
            o A+W Infrastructure 6 Middleware
            o Java 7 Update 51
            o A+W Setup Launcher
    -   Installation of the FinAc Service and dependent disksets with the Setup Launcher.
    -   Configuration of the FinAc Service with the Config Tool.

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


07.07.2022                      EN-INST-A+W Enterprise FinAc Service.docx                   3
1.3 Requirements
1.3.1 Windows Server Version
Supported operating systems:

    •   Windows 2008 Server R2 32/64bit.
    •   Windows 2012 Server R2 32/64bit.


1.3.2 Network
For the installation itself, no network access is necessary.
For the operation of the service, there must be a connection to the A+W Enterprise
DB Server and the company network.
The service user used must have sufficient access rights also to network resources
used.
1.3.3 Software
It is assumed that the following disk sets were already installed and configured BEFORE the
installation of the A+W Enterprise 6 FinAc Service disk set.

    •   Informix Client SDK 3.5 TC9 (or newer)
    •   Microsoft .NET Framework 4.5.1 SDK



1.4 Procedure
For the installation, please proceed in the following sequence:
1. Use setnet32.exe to configure the database server and hosts. This assumes that an IBM Informix
   Client SDK was installed (see software requirements).

2. Installation of the A+W Enterprise 6 FinAc Service with the Setup Launcher

    On the Component Selection dialog on the A+W Enterprise node, select the "A+W Enterprise 6
    FinAc Service" module. This automatically selects all dependent set-ups.




07.07.2022                      EN-INST-A+W Enterprise FinAc Service.docx                       4
07.07.2022   EN-INST-A+W Enterprise FinAc Service.docx   5
3. After the successful installation, the FinAc Service is configured with the Config Tool.

    3.1. Common Settings




        3.1.1.   General Settings - Polling Interval

                 Time interval in minutes in which the FinAcService checks the transfer table
                 fibutransfer.

                 "Rush" transfer records, that is, records with status -1, will be processed at the next
                 polling time. "Normal" records (with status 0) will be processed only at the "Start
                 time".

                 "Urgent" records can only be generated by calling a corresponding script in the
                 individual programs. The update urgent scripts are made available by A+W. For
                 additional information, see the configuration instructions for the FinAc service.

                 Default value: 15 minutes. Maximum: 1440 minutes (= once a day).

        3.1.2.   FinAc Settings - FinAc Interface

                 Various FinAc Interface types are available. The correct setting is determined
                 customer individually after consultation with Development.




07.07.2022                        EN-INST-A+W Enterprise FinAc Service.docx                            6
        3.1.3.   FinAc Settings - Transfer Type

                        o   No Transfer

                         No data transfer. The XML files generated remain in the directory      that   was
                 specified in the XML Export Path field.

                            The files are also not deleted if the Delete XML option   Delete files from was
                 set.

                        o   Copy to network path

                         With this setting, the transfer of the XML files within a company network is
                 activated. Additional settings are necessary. See File Transfer Settings.

                        o   FTP upload

                 This setting activates the transfer of XML files on an FTP server. Additional settings
                 are necessary. See FTP Settings.

                 Default value: No Transfer.

        3.1.4.   Intrastat Settings - Intrastat Interface

                 Various Intrastat Interface types are available. The correct setting is determined
                 customer-specifically after consultation with Development.

        3.1.5.   Intrastat Settings – Lock Limit (records)

                 A record limit can be specified, starting from which the table intrastat is locked
                 exclusively for the Intrastat processing. The limit only applies if the "Exclusive Table
                 Lock" checkbox in the "Site Properties" is activated.




07.07.2022                           EN-INST-A+W Enterprise FinAc Service.docx                            7
        3.1.6.   Protocol-Button




        With the Protocol button, you can reach the Protocol Configuration dialog. This automatically
        selects all dependent set-ups. On the first tab, the trace categories for the frontend are
        configured; on the following tabs, the tracing of dependent modules and programs can be
        activated if necessary.

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

        The A+W Enterprise FinAc Service currently uses no log protocol.




07.07.2022                         EN-INST-A+W Enterprise FinAc Service.docx                           8
    3.2. Document Export Settings




        On this dialog, the settings for the FinAc document export are made.

        3.2.1.   Export Documents

                 Check box that activates the document export.

        3.2.2.   Use Site Folders

                 Check box that activates company-specific subdirectories.

        3.2.3.   Start Time (hh:mm)

                 Start time of the regular FINAC transfer. At this time, all data records of the table
                 fibutransfer are processed, which are in the table with status 0 (or -1).


                 The specification of the time is done in 24-hour format.

        3.2.4.   Rerun Interval (h)

                 Rerun                                      Interval                             (h)
                 Specification of the repetition interval in hours and how many times run should be
                 repeated.

        3.2.5.   Export Root Path



07.07.2022                          EN-INST-A+W Enterprise FinAc Service.docx                        9
                 File path in which all XML files generated are stored before they are transferred by
                 the transfer logic. If "Use Site Folders" is active, the files are stored in company-
                 specific subdirectories.




    3.3. Intrastat export settings




        On this dialog, the settings for the Intrastat document export are made.

        3.1.1.   Intrastat export

                 Checkbox that activates the Intrastat export.

        3.1.2.   Use Site Folders

                 Check box that activates company-specific subdirectories.

        3.1.3.   Export Root Path




07.07.2022                           EN-INST-A+W Enterprise FinAc Service.docx                      10
                 File path in which all XML files generated are stored before they are transferred by
                 the transfer logic. If "Use Site Folders" is active, the files are stored in company-
                 specific subdirectories.

        3.1.4.   Clean Up Time (days):

                 All back-up records for the table intrastatok are removed from the table as soon as
                 they are older than the time period specified here in days.



        3.1.5.   Daily Export

                 Checkbox that activates the daily export.

        3.1.6.   Daily Issue Check

                 Checkbox that activates the daily checking of Intrastat data available for export.



        3.1.7.   Daily - Start Time (hh:mm)

                 Start time of the daily Intrastat-xml file generation. At this time, all data records of the
                 table intrastat are processed, which are in the table with status 0 (or -1).


                 The specification of the time is done in 24-hour format.

        3.1.8.   Daily - Rerun Interval (h)

                 Rerun                                      Interval                             (h)
                 Specification of the repetition interval in hours and how many times run should be
                 repeated.

        3.1.9.   Monthly Export

                 Checkbox that activates the monthly export.

        3.1.10. Monthly - Start Day

                 Day of the month on which the monthly Intrastat-xml file generation should start.

        3.1.11. Monthly - Start Time (hh:mm)

                 Start time of the monthly Intrastat-xml file generation. At this time, all data records of
                 the table intrastat are processed, which are in the table with status 0 (or -1).


                 The specification of the time is done in 24-hour format.




07.07.2022                         EN-INST-A+W Enterprise FinAc Service.docx                               11
    3.2. Database settings

        On this dialog, all database-precise settings are configured, starting with the database itself.




             o   With the New button, you can edit an existing configuration.
             o   With the Edit button, you can delete an existing configuration.
             o   With the Delete button, you can delete an existing configuration.




07.07.2022                        EN-INST-A+W Enterprise FinAc Service.docx                                12
        3.2.1.   Site Properties

                 With the New or Edit buttons or with a double-click on a row in the table, you reach
                 the Site Properties dialog. Here, all database-dependent settings can be made.




07.07.2022                         EN-INST-A+W Enterprise FinAc Service.docx                       13
07.07.2022   EN-INST-A+W Enterprise FinAc Service.docx   14
        3.2.2.   Site Settings

             o   Active Connection
                 Activates the DB connection

             o   AWE Site
                 The site number of the AWE site. See xhaus.hnr.

        3.2.3. FinAc Interface Settings
            o FinAc Site
               The FinAc site number assigned to this site.

             o   FinAc Interface
                 The designation of the FinAc interface.

             o   FinAc Interface Version
                 The client-specific version of the FinAc interface.



        3.2.4.   Intrastat Interface Settings

             o   Intrastat export
                 Activation of the Intrastat export
             o   Test
                 Intrastat export in test mode
             o   Exclusive Table Lock
                 Activates the exclusive locking of the table intrastat during processing, applies only
                 starting with -> Lock Limit

             o   Lock Limit (records)
                 Specifies the lower limit. Starting with this number of records, the table intrastat is
                 locked exclusively during processing. The value is taken over from the common
                 settings ("Common Settings"), but it can be adjusted DB-specifically here.

             o   Intrastat Interface Version
                 The client-specific version of the Intrastat interface.



        3.2.5.   Database settings
            o    The database server is entered in the Server Name field. Via the combo box, all DB
                 servers entered in the setnet32 can be selected.
             o   A user name that has access to the database must be entered in User Name.
             o   If the fields Server Name, User Name, and Password are filled with valid values, the
                 Database Name combo box already contains all available database names of the
                 database server.
             o   The appropriate locale settings are entered in the Client Locale and DB Locale fields.
                 The combo boxes already contain most values used. If it is necessary to enter
                 deviating values, this is also possible manually.




07.07.2022                         EN-INST-A+W Enterprise FinAc Service.docx                               15
             o   SQL Explain
                 Activates the database log.


        3.2.6.   DB Functions
            o    With the Start Setnet32 button, it is possible to start the setnet32.exe program
                 directly; with it, database server/hosts can be set up.
             o   With Check Alenv you can check the A+W Enterprise environment variables for this
                 service and view the current database configuration. Since this dialog is only for
                 checking purposes, it will not be described in any more detail. The settings of the
                 Alenv variables are made in A+W Enterprise.
             o   The Test Connection button allows you to check the current values of the database
                 configuration. If a database connection can be established with this values, you will
                 see the following message box; otherwise an error message.




07.07.2022                        EN-INST-A+W Enterprise FinAc Service.docx                              16
    3.3. Subsite Settings

        On this dialog, all subsites of a multisite system can be entered. The subsides can optionally
        be entered in the "Database Settings." The difference is that in the "Database Settings" for
        each subsite, the DB connection must be entered. In the "Subsite Settings," the DB
        connection is referenced via the entry in "AWE Main Site." Therefore, there must only be an
        entry in "Database Settings" for the main site.

        3.3.1.   Active Site

                 This checkbox marks whether or not the specified subside is active. Active subsites
                 are processed by the FinAc service, inactive ones not.

        3.3.2.   AWE Main Site

                 Number of the main site via which the DB connection is referenced.

        3.3.3.   AWE Subsite

                 Number of the subsite

        3.3.4.   FinAc Site

                 Number of the FINAC sites assigned to the subsites




07.07.2022                       EN-INST-A+W Enterprise FinAc Service.docx                          17
    3.4. See File        Transfer Settings.

        If in the switch Transfer Type the point Copy to network path was selected, the File Transfer
        Settings dialog appears. Here there is only a field for the base path.

        3.4.1.   Base Path

                 The defined directories are created below the base path; the XML file are copied to
        these.

                 The path must be reachable from the server on which the FinAc Service is installed.
                 Write permissions have to be set up for the Service user.




    3.5. FTP Settings

        If on the tab Transfer Type the point FTP upload has been selected, the dialog FTP Settings
        appears. There are fields here to establish a connection to an existing FTP server.

        3.5.1.   FTP Server

                 The address of the FTP server without the specification "ftp://"

        3.5.2.   FTP User



07.07.2022                        EN-INST-A+W Enterprise FinAc Service.docx                        18
                 The login name of the FTP user.

        3.5.3.   FTP Password + Confirm Password

                 The password of the FTP user.

        3.5.4.   FTP Base Path

                 The defined directories are created below the base path; the XML file are copied to
        these.

                 Write permissions have to be set up for the FTP user.

        3.5.5.   Max. Attempts

               The maximum number of attempts to upload a file to the FTP server before the
        process is terminated. Default value: 1. Maximum: 100.




    3.6. Maintenance Settings




07.07.2022                        EN-INST-A+W Enterprise FinAc Service.docx                       19
        The maintenance functions of the FinAc Service are configured in the Maintenance Settings
        dialog.

        3.6.1.   Archive Transfer Data:

                 It can be set as to whether processed records of the table fibutransfer should be
                 deleted or whether they should remain in the table for research purposes.

                 Default value: Move transfer data to ok*-table.

        3.6.2.   Clean Up Time (days):

                 All successfully processed records of the fibutransfer table are removed from the
                 table as soon as they are older than the time interval set here.

                 Default value: 90 days. Maximum: 360 days.

        3.6.3.   Delete XML Files:

                 You can also select for generated XML files whether they are deleted after
                 successful transfer or whether they should remain.

                 If as transfer type "No transfer" was selected, the XML files are not deleted
                 automatically.

                 Default value: Delete XML files after successful transfer.



07.07.2022                        EN-INST-A+W Enterprise FinAc Service.docx                      20
    3.7. Service configuration




        The service users are stored on the Windows Service Configuration dialog. These are
        Windows users who are used to access external objects such as network paths, etc. This
        user must have the appropriate rights.

        With the Pick user... button it is possible to select a domain user.

        If no network domain is available, e.g. because the service was installed on a PC, the value
        "."

        If no user is available, the service can also run under "LocalSystem" in case of emergency.
        This is the default services user in a Windows system.

        Last but not least, you can set up the quantity of additional parallel services here in order to
        increase the processing speed. For this function, the computer on which the FinAc Service is
        running must have appropriate hardware (e.g. multi-core processor).

        With a click on Next, the component registration for SN is executed. Here the Windows
        component manager is opened and then closed again. For this reason, it is recommended
        that you always let the ConfigTool run through to the end.

4. Now the A+W Enterprise 6 FinAc Service is ready and it writes a log into the directory named
   above.

5. Setting of A+W Enterprise environment variables



07.07.2022                        EN-INST-A+W Enterprise FinAc Service.docx                           21
1.5 Customer-specific configurations
        The information whether the respective functionality is available for the
        customer FinAc interface can be found in the customer-specific interface
        description.


1.5.1 Open Amounts Import Settings
             a. Import Open Amounts
                check box, which activates the import of the open items.
             b. Start Time (hh:mm)
                First daily start time of the import.
                The specification of the time is done in 24-hour format.
             c. Rerun Interval (h)
                Specification of the repetition interval in hours and how many times
                run should be repeated.
             d. Import Root Path
                File path in which the import files should be searched for.




07.07.2022                    EN-INST-A+W Enterprise FinAc Service.docx                22
1.5.2 Ongoing Orders Export Settings
             a. Export Ongoing Orders
                Check box that activates the export of the open orders.
             b. Start Time (hh:mm)
                First daily start time of the export.
                The specification of the time is done in 24-hour format.
             c. Rerun Interval (h)
                Specification of the repetition interval in hours and how many times
                run should be repeated.
             d. Export Root Path
                File path in which all export files generated are stored. The files are
                stored in company-specific subdirectories




07.07.2022                     EN-INST-A+W Enterprise FinAc Service.docx                  23
1.5.3 Customer-specific settings (account information)
             a. Basis Account

             b. Department Account




07.07.2022                      EN-INST-A+W Enterprise FinAc Service.docx   24
1.5.4 Stock Movements Export Settings
             a. Export Stock Movem.
                Checkbox that activates the export of the incoming and outgoing
                stock transactions.
             b. Start Time (hh:mm)
                First daily start time of the export.
                The specification of the time is done in 24-hour format.
             c. Rerun Interval (h)
                Specification of the repetition interval in hours and how many times
                run should be repeated.
             d. Export Root Path
                File path in which all export files generated are stored.




07.07.2022                     EN-INST-A+W Enterprise FinAc Service.docx               25
1.6 Incompatibilities
        No incompatibilities are known.

1.7 Directory structure

1.8 Result of the installation
If the service could be started, the installation was successful. Otherwise, the trace
log is available for determining possible problems.

1.9 Configuration
For additional configurations, please see the FinAc Service documentation.




07.07.2022                  EN-INST-A+W Enterprise FinAc Service.docx                    26
1.10 Tips and tricks
1.10.1 AutoUpdate
        In order to be able to install the service via AutoUpdate, the setup must
        have been installed successfully at least once with the Setup Launcher and
        configured with the ConfigTool.
1.10.2 Known errors and workarounds

1.11 Uninstalling
You can uninstall the program as usual via Control Panel -> Programs and
Functions.




Note: The config file is not deleted automatically. For a final uninstallation, the
program directory of the A+W Enterprise 6 FinAc Service must be deleted manually.




07.07.2022                  EN-INST-A+W Enterprise FinAc Service.docx                27

