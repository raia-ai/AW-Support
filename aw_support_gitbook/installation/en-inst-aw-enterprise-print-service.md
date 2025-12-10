---
title: "EN INST A+W Enterprise Print Service"
category: "installation"
product: "A+W Enterprise Print Service"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Enterprise Print Service"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions          A+W Enterprise 6 Print Service    Change history:     Date          Edited by                 Remarks                                     Version     16.04.12      MP                        New creation                                1.0     16.08.26      MP                        Std. report environment                     1.1     16.12.13      MP                        AutoUpdate                                  1.2     17.06.12      MP"
source_file: "EN-INST-A+W Enterprise Print Service.pdf"
---


# EN INST A+W Enterprise Print Service

        Installation Instructions

        A+W Enterprise 6 Print Service
   Change history:
    Date          Edited by                 Remarks                                     Version
    16.04.12      MP                        New creation                                1.0
    16.08.26      MP                        Std. report environment                     1.1
    16.12.13      MP                        AutoUpdate                                  1.2
    17.06.12      MP                        Mail configuration                          1.3
    17.09.04      MP                        Default value SNLIVE                        1.4
    18.02.12      MP                        Switch CR-Runtime                           1.5
    18.11.27      MP                        Internal working directory + PDF printer    1.6
    24.02.29      ALW                       Termination of Crystal Report Engine 2008   1.7




     The installation instructions will assist the planner with the installation and
     configuration process for the software named. Please proceed in the following
     sequence:


     1. Check the installation requirements.

     2. Compile the required data, additional programs, drivers, etc.

     3. Note or determine the time required.




18.03.2024                        EN-INST-A+W Enterprise Print Service.docx               1
Content

   1         Installation of the A+W Enterprise 6 Print Service ............... 3
   1.1       Overview and the basics ............................................................................ 3
   1.2       Time requirement ....................................................................................... 3
   1.2.1     Installation time for the software ................................................................. 3
   1.3       Requirements ............................................................................................. 4
   1.3.1     Windows Server Version ............................................................................ 4
   1.3.2     Network ...................................................................................................... 4
   1.3.3     Software ..................................................................................................... 4
   1.4       Procedure ................................................................................................... 4
   1.5       Incompatibilities ........................................................................................ 21
   1.5.1     Crystal Reports Runtime 2013 ................................................................. 21
   1.5.2     Crystal Report Runtime 13.0.31 (SP 31) .................................................. 21
   1.5.3     Crystal Report Runtime A+W ReportRuntime 2008 (SP4) ....................... 21
   1.6       Directory structure .................................................................................... 21
   1.7       Result of the installation ........................................................................... 22
   1.8       Configuration ............................................................................................ 22
   1.9       Tips and Tricks ......................................................................................... 22
   1.9.1     AutoUpdate .............................................................................................. 22
   1.9.2     Known errors and workarounds ................................................................ 22
   1.10      Uninstalling ............................................................................................... 23




18.03.2024                            EN-INST-A+W Enterprise Print Service.docx                                            2
1 Installation of the A+W Enterprise 6 Print Service
The following installation instructions assume that there is no previous version
installed.
An update of an earlier release version of the A+W Enterprise 6 Print Service is
executed precisely like a new installation.
An update of an earlier version of the Print Service, e.g. from ALCIB 2011 Print
Service to A+W Enterprise 6 Print Service is not possible. Only one version of the
Print Service should be installed.
This document describes only the installation and configuration of the A+W
Enterprise 6 Print Service. In case of questions about the installation or configuration
of dependent set-ups/disk sets, please see the installation instructions for these
products.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during
installation:
    -   Installation and configuration of the Informix driver via setnet32.exe
    -   Creation of the necessary set-ups/disk sets
            o A+W CAD Designer (Bars)
            o A+W CAD Designer (Shapes)
            o SAP Crystal Reports runtime engine starting with 13.0.19
            o A+W Enterprise 6 Print Service
            o A+W Infrastructure 6 Collector Services
            o A+W Infrastructure 6 Middleware
            o Java 7 Update 51
            o A+W Setup Launcher
    -   Installation of the Print Service and the dependent disk sets with the Setup Launcher
    -   Configuration of the Print Service with the ConfigTool
    -   Set-up of the reports
    -   Setting of A+W Enterprise environment variables
    -   Further set-up of the file system

1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data:
1.2.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times
will vary for different computers. The installation time specified was determined
using a reference device with the following characteristics:
    -   Processor: 3000 Mhz


18.03.2024                       EN-INST-A+W Enterprise Print Service.docx                      3
    -   RAM: 4 GB
    -   Other: /
For an initial or new installation, an installation time of 15 minutes must be
anticipated for the reference device. For higher or lower-power hardware, shorter or
longer installation times must be anticipated.

1.3 Requirements
1.3.1 Windows Server Version
Supported operating systems:

    •   Windows 2008 Server R2 32/64bit.
    •   Windows 2012 Server R2 32/64bit.


1.3.2 Network
For the installation, network access is not absolutely necessary. However, without
contact to network or database, some functions of the ConfigTool will not work.
For the operation of the service, there must be a connection to the A+W Enterprise
DB Server and the company network. The printer on the company network must be
accessible.
1.3.3 Software
It is assumed that the following disk sets were already installed and configured BEFORE the
installation of the A+W Enterprise 6 Print Service disk set.

    •   Informix Client SDK 3.5 TC9 (or newer)
    •   Microsoft .NET Framework 4.5.1 SDK



1.4 Procedure
For the installation, please proceed in the following sequence:
1. Use setnet32.exe to configure the database server and hosts. This assumes that an IBM Informix
   Client SDK was installed (see software requirements).

2. Installation of the A+W Enterprise 6 Print Service with the Setup Launcher

    On the Component Selection dialog on the A+W Enterprise node, select the "A+W Enterprise 6
    Print Service" module. This automatically selects all dependent set-ups.




18.03.2024                       EN-INST-A+W Enterprise Print Service.docx                       4
3. After the successful installation, the Print Service is configured with the Config Tool.

    3.1. Common Settings




18.03.2024                        EN-INST-A+W Enterprise Print Service.docx                   5
        3.1.1.   Polling Interval

                 In the Polling Interval (Seconds) field, the number of seconds is set that the service
                 waits until it checks the printtransfer transfer table again for new data records. The
                 default value is 18 seconds.

        3.1.2.   Working Directory

                 Here you can specify a local directory in which the subdirectories Archive, Bitmaps,
                 Email, PDF, Reports are created; these can then be used as (intermediate) result
                 storage areas.

                 The latest versions of the A+W standard forms are installed in the Reports directory
                 in case of a new installation or an update.

        3.1.3.   Shared Folder

                 The ConfigTool generates permission for Everyone (that is, for all network users) for
                 the working directory. The permission name is always <Servername>\AIPrintService.

                 Info: the authorizations for the permission can be changed manually. These changes
                 are retained in case of a reconfiguration with the ConfigTool.

        3.1.4.   Protocol-Button



18.03.2024                          EN-INST-A+W Enterprise Print Service.docx                         6
                 With the Protocol button, you can reach the Protocol Configuration dialog. This
                 automatically selects all dependent set-ups. On the first tab, the trace categories for
                 the frontend are configured; on the following tabs, the tracing of dependent modules
                 and programs can be activated if necessary.




             The following trace levels are distinguished:
             o Fatal
             o Error"
             o Warning
             o Info
             o Debug

             With the Protocol button, you can reach the Protocol Configuration dialog. If, for example,
             the Info level is active, trace messages of the type Error and Warning will also be written
             into the tracing file.

             The tracing file is always in the directory %ProgramData%\A+W\Log. The file name
             consists of the service name, the current date and the process number and ends with
             .awtrc.




18.03.2024                         EN-INST-A+W Enterprise Print Service.docx                           7
             The A+W Enterprise Print Service currently uses no log protocol.

    3.2. Crystal Reports Runtime Version

             The Crystal Reports Runtime 2008 was terminated with Quality Release [2403].

             It is anticipated that a Crystal Report Runtime 2013 starting with Version 13.0.19 is
             installed on the server. The print service pulls the installed engine automatically. Nothing
             else needs to be configured.

    3.3. Database settings

        On this dialog, all database-precise settings are configured, starting with the database itself.




             o   With the New button, you can edit an existing configuration.
             o   With the Edit button, you can delete an existing configuration.
             o   With the Delete button, you can delete an existing configuration.
             o   With the Copy button, you can copy an existing configuration. So that there are no
                 problems with identical configurations, the configuration created this way is initially
                 deactivated and the value ENTER_NEW_DATABASE_NAME is entered in the
                 Database Name field. Otherwise, all settings are taken over 1:1.
             o   With the De/Activate button, individual database configurations can be deactivated or
                 activated again. Thus, for example, the processing of print jobs on a database server
                 can be interrupted without having to delete the entire configuration.



18.03.2024                         EN-INST-A+W Enterprise Print Service.docx                               8
18.03.2024   EN-INST-A+W Enterprise Print Service.docx   9
        3.3.1.   Site Properties

                 With the New or Edit buttons or with a double-click on a row in the table, you reach
                 the Site Properties dialog. Here, all database-dependent settings can be made.




        3.3.2.   Site Settings
            o    The Config No field contains a sequential number. The field is filled automatically.
            o    With the Active Connection checkbox, the database configuration can be activated or
                 deactivated. Only active configurations are considered by the Print Service for the
                 processing of print jobs.




18.03.2024                         EN-INST-A+W Enterprise Print Service.docx                       10
             o   In the AWE Site field, a site number can be entered. If a value not equal to 0 is
                 entered here, for the query to the printtransfer table, the hausnr field is linked to this
                 value. Thus it is possible to store site-specific database configurations.
        3.3.3.   Database settings
            o    The database server is entered in the Server Name field. Via the combo box, all DB
                 servers entered in the setnet32 can be selected.
             o   A user name that has access to the database must be entered in User Name. This
                 user is also used for the processing of the Crystal Reports.
             o   If the fields Server Name, User Name, and Password are filled with valid values, the
                 Database Name combo box already contains all available database names of the
                 database server.
             o   The appropriate locale settings are entered in the Client Locale and DB Locale fields.
                 The combo boxes already contain most values used. If it is necessary to enter
                 deviating values, this is also possible manually.
             o   In the Report DSN (ODBC) field, it is possible to select an existing ODBC
                 configuration via the combo box. This DSN (=Data Source name) is used in Crystal
                 Report to establish the connection to the database. That is, the ODBC connection
                 should fit the configured database.
                 A not-yet-extant ODBC name can also be entered in this field. If when saving the
                 database configuration it is determined that the ODBC name does not exist yet, there
                 is a query as to whether an ODBC connection should be created with the current
                 values of the database configuration. If this is confirmed, precisely this is done.
                 To be noted here is that ODBC connections must always be created in the area
                 System-DSN, since only these are available for all Windows users.
                 ODBC connections must always be set up with insulation level "1 - Read
                 Uncommitted" so that there cannot be DB blocks during output of Crystal Reports.

        3.3.4.   DB Functions
            o    With the Start Setnet32 button, it is possible to start the setnet32.exe program
                 directly; with it, database server/hosts can be set up.
             o   The 32-bit program for creating ODBC configurations is started with the Start ODBC
                 (32-bit) button. Since on 64-bit operating systems there are two different versions
                 and this always created problems in the past, here it is ensured that you start the
                 correct program version.
             o   With Check Alenv you can check the A+W Enterprise environment variables for this
                 service and view the current database configuration. Since this dialog is only for
                 checking purposes, it will not be described in any more detail. The settings of the
                 Alenv variables are made in A+W Enterprise.
             o   The Test Connection button allows you to check the current values of the database
                 configuration. If a database connection can be established with this values, you will
                 see the following message box; otherwise an error message.




18.03.2024                         EN-INST-A+W Enterprise Print Service.docx                             11
        3.3.5.   Print Service Settings




             3.3.5.1. Common Settings
             o Default Printer: The permitted name of an installed printer that is used if the printer
                 found in printtransfer does not exist. If no value is entered here, the Windows default
                 printer will be used. Default: Empty.
             o Text Encoding:
                 Default: Default.




18.03.2024                        EN-INST-A+W Enterprise Print Service.docx                            12
             o   Temp. Status List: Here stati can be entered, which under some circumstances no
                 longer occur at a later point in time and it is therefore worthwhile for the print job to
                 be processed again. Only the stati are considered that are described in the print
                 service document - Referenzen.docx. Default: Empty.
                 The comma is expected as separator.
             o   Maximum Attempts: Maximum number of attempts the Print Service will make to
                 process a print job that encounters an error that was specified in the Temp Status
                 list. Default: 1.
                 The value of this field will be compared to printtransfer.attempts.
             o   Wait On Error: Time in seconds that should be waited after a temporary error.
             o   Max. Attachments: The maximum number of attachments that may accompany an e-
                 mail. Default: 25.

             3.3.5.2. Export Path Settings
             o Default Export Path: The directory specified here is used if no directory was specified
                 during file export. Default: <Shared Folder>\PDF.
             o Archive Path: This directory is used for the export of PDF files if ArchiveNSG
                 (outputflag=10) was specified as output type for the print job. Default: <Shared
                 Folder>\Archive.

             3.3.5.3. Image Settings
             o A+W CAD Designer (Bars): De-/activates the generation of bar sketches.
             o A+W CAD Designer (Shapes): De-/activates the generation of shape and processing
                 sketches.
             o AWBom: De-/activates the generation of glass structure images.




18.03.2024                         EN-INST-A+W Enterprise Print Service.docx                             13
             3.3.5.4. Additional Data Source
                      On this dialog, you can save a second database connection in order to realize a
                      multi-DB report. The settings on this dialog are used if sub-reports begin with the
                      text "AWPSUB."
                      The content of the fields depends on the logic described above. The most
                      important element here is the ODBC connection to the A+W Production
                      database.




             3.3.5.5. Initialize Report Environment
                      On this dialog, it is possible to initialize all or individual components of the print
                      environment. The functions are attuned to initializing the print environment for the
                      A+W standard reports.
                       CR PDF Export Printer
                           If in the table drucker there is no printer "crpdfexport", an appropriate data
                           record is created in the database. The printer „crmailmitarb“ is also created.
                       A+W Standard Reports
                           Entries in the table rep are generated so that the forms can be selected in
                           A+W Enterprise.
                       Default Alenv Values
                           Default values are set for a series of environment variables.




18.03.2024                         EN-INST-A+W Enterprise Print Service.docx                              14
    Important:
    -  Only one action is triggered when the "Initialize..." action was selected. This option is pre-
       populated automatically if it was determined in the respective area that an initialization is
       required.
    -  For each of the three areas, a module block is requested by the to-server via alprc service.
       That is, the alrpc service must be available and it must be possible to establish a database
       connection. Otherwise no initialization is possible and there is an appropriate error message.
    -  Via the dialog no data is deleted, but under some circumstances, it is overwritten with default
       values. Missing data records will be inserted into the database.

The following ALENV variables are initialized


ALENV Name                                              Default value

CR_IMAGE_FORMAT_AWBOM                                   BMP

CR_IMAGE_FORMAT_AWDESIGN                                EMF

CR_IMAGE_FORMAT_SNLIVE                                  BMP

CR_IMAGE_PATH                                           <SHARED FOLDER>\Bitmaps

CR_IMAGE_SIZE_AWBOM                                     300,300



18.03.2024                       EN-INST-A+W Enterprise Print Service.docx                           15
ALENV Name                                           Default value

CR_IMAGE_SIZE_AWDESIGN                               300,300

CR_IMAGE_SIZE_SNLIVE                                 600,600

CR_STD_EXPORT_PATH                                   <SHARED FOLDER>\PDF

MODUL_PRINTSERVICE                                   2

REPCLEAN_TIME                                        30


The following reports are inserted

File name                            Meaning                              Form type

cr_aw_lian                           Inquiry                              901

cr_aw_best                           Purchase order                       902

cr_aw_angbk                          Quotation                            904

cr_aw_ab                             OC                                   905

cr_aw_lief                           Delivery note                        906

cr_aw_rech                           Invoice                              907

cr_aw_gut                            Credit note                          909

cr_aw_samr                           Collective invoice                   912

cr_aw_vls                            VLS sale                             923

cr_aw_ba                             Works order                          927

cr_aw_vlslap                         VLS dispatch                         928




18.03.2024                    EN-INST-A+W Enterprise Print Service.docx               16
    3.4. Maintenance Settings




        The maintenance functions of the Print Service are configured on the Maintenance Settings
        dialog.

        3.4.1.   With the Archive Transfer Data setting, it is determined how to work with
                 successfully-processed transfer data. There are three options:
             o   Do nothing.
             o   Delete the transfer data after successful processing.
             o   Move the transfer data into the respective *ok tables in order to be able to access it
                 later on.

        3.4.2.   With the Delete Image Files setting, it is determined how the graphic files should be
                 handled that the Print Service creates temporarily.
             o   Yes (Default) – the files are deleted directly after use.
             o   No – the files are retained. This can be useful for service purposes.

        3.4.3.   With the Delete Internal Working Folder setting, it is determined whether or not the
                 temporary working directory should be deleted in case of success.

        3.4.4.   With the Activate Maintenance switch, you can activate the self-maintenance of the
                 Print Service. This includes all clean-up activities such as the deletion of old files in
                 the *ok tables, the transfer tables, and temporary files. The clean-up function is



18.03.2024                        EN-INST-A+W Enterprise Print Service.docx                             17
                started once a day; at the earliest at the time configured in the Maintenance Time
                field.

    3.5. External Tools Settings




        An external program must be configured for the output of combined PDF files with a PDF
        printer.

        In the PDF Printer Tool field, a program (*.exe) or a Windows script (*.cmd) can be stored,
        which is in a position to send a PDF to a printer in the background via the command line.

        In the Arguments field, the argument list for the program is stored. Here, the parameters
        %PRINTER% and %PDFFILE% serve as placeholders for the actual values from the current
        print job.




    3.6. E-Mail Settings



18.03.2024                         EN-INST-A+W Enterprise Print Service.docx                     18
        Use dialog E-Mail Settings to configure whether and to which recipients the error messages
        can be sent via email.
            o SMTP Server: The name of the SMTP server
            o Port:            (optional) deviating SMTP port
            o From:            Email address of the sender
            o To:              Email address of the recipient. Several recipient addresses
                               can be specified separated by semicolons.
            o CC:              Email address of the CC recipient. Several recipient addresses
                               can be specified separated by semicolons.
            o Encoding:        Coding of E-mail. Default: utf-8.
            o Enable SSL: Activate SSL encryption (Y/N)

             o   Authentication: Activate authentication (Y/N)
                      Account:                  Domain account for the authentication
                      Password:                 Password
                      Confirm password:         Confirmation of the password




18.03.2024                        EN-INST-A+W Enterprise Print Service.docx                     19
    3.7. Service configuration




        The service users are stored on the Windows Service Configuration dialog. These are
        Windows users who are used to access external objects such as network paths, etc. This
        user must have the appropriate rights.

        With the Pick user... button it is possible to select a domain user.

        If no network domain is available, e.g. because the service was installed on a PC, the value
        "." can be entered in field Domain.

        If no user is available, the service can also run under "LocalSystem" in case of emergency.
        This is the default services user in a Windows system.

        Last but not least, you can set up the quantity of additional parallel services here in order to
        increase the processing speed. For this function, the computer on which the Print Service is
        running must have appropriate hardware (e.g. multi-core processor).

        With a click on Next, the component registration for SN is executed. Here the Windows
        component manager is opened and then closed again. For this reason, it is recommended
        that you always let the ConfigTool run through to the end.

4. Now the A+W Enterprise 6 Print Service is ready and it writes a log into the directory named
   above.

5. Set-up of the reports.



18.03.2024                        EN-INST-A+W Enterprise Print Service.docx                           20
    5.1. As described in the Print Service documentation, reports must be set up in A+W Enterprise.

    5.2. The Crystal Report files will be copied to the directory specified in A+W Enterprise. If a
         network path was specified, it must be ensured that the services user has appropriate access
         rights to the directory.

6. Setting of A+W Enterprise environment variables.

7. Set-up of the file system.

    7.1. For the sake of simplicity, all required directories are set up on the same computer. Sensibly
         on the computer on which the Print Service was installed. See details in Chapter 1.6.



1.5 Incompatibilities
        No incompatibilities are known.
1.5.1 Crystal Reports Runtime 2013
        No incompatibilities regarding Crystal Reports Runtime 2008 are known.
1.5.2 Crystal Report Runtime 13.0.31 (SP 31)
        Development was implemented with DevOps Feature 69004.
        It is now possible to use the Crystal Report Runtime 13.0.31 for the A+W
        Enterprise Print Service. Before the new runtime is installed, the old
        runtime must always be de-installed; otherwise there can be problems with
        printing.
1.5.3 Crystal Report Runtime A+W ReportRuntime 2008 (SP4)
        Development was implemented with DevOps Feature 99812
        The Crystal Report Runtime 2008 was terminated with Quality Release
        [2403] will no longer be supported. SAP has not supported this runtime for
        a long time already, and after a company-wide restructuring of the A+W
        Print Service, the connection to the old runtime was removed.

1.6 Directory structure
        It is recommended that you create the following directory structure on the
        server. For the topmost directory, a network permission must be created
        for all users who should have access to it.




18.03.2024                       EN-INST-A+W Enterprise Print Service.docx                            21
        With the new version, these directories and the permissions are created
        automatically.
        For internal use, an internal directory structure is created in order to ensure
        that the print service can perform its work locally on the server. Then, if
        necessary, a copy action is executed. For each print job, there is an
        internal working directory under %PROGRAMDATA%\A+W\A+W
        Enterprise 6 Print Service\<pid>.
        If the working directory cannot be created, the previous output directories
        are used.

1.7 Result of the installation
If the service could be started, the installation was successful. Otherwise, the trace
log is available for determining possible problems.

1.8 Configuration
For additional configurations, please see the Print Service documentation.

1.9 Tips and Tricks
1.9.1 AutoUpdate
        In order to be able to install the service via AutoUpdate, the setup must
        have been installed successfully at least once with the Setup Launcher and
        configured with the ConfigTool.
1.9.2 Known errors and workarounds
1.9.2.1 Error when sending mail
        If the Print Service cannot send any mail, this can have various causes.
        For troubleshooting, examine the Print Service log.
        The following errors have already occurred and could be solved as
        described.



18.03.2024                    EN-INST-A+W Enterprise Print Service.docx                   22
        a) Error Message:
             Service not available. Transmission channel is closed. The server
             response was: 4.3.2 Service not available, closing transmission
             channel
             Solution:
             This message only exists in connection with MS Exchange servers. For
             the Print Service, a SMTP relay must be set up so that the SMTP
             server can receive the mails from the Print Service. (#285402)

1.10 Uninstalling
You can uninstall the program as usual via Control Panel -> Programs and
Functions.




Note: The config file is not deleted automatically. For a final uninstallation, the
program directory of the A+W Enterprise 6 Print Service must be deleted manually.




18.03.2024                   EN-INST-A+W Enterprise Print Service.docx                23

