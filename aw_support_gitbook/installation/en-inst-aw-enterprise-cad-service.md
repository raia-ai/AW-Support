---
description: "EN INST A+W Enterprise CAD Service"
---



# EN INST A+W Enterprise CAD Service

        Installation Instructions

        A+W Enterprise 6 CAD Service
   Change history:

    Date             Edited by            Remarks                                      Version
    16.04.22         MP                   New creation                                 1.0
    16.12.13         MP                   AutoUpdate                                   1.2




     The installation instructions will assist the planner with the installation and
     configuration process for the software named. Please proceed in the following
     sequence:


     1. Check the installation requirements.

     2. Compile the required data, additional programs, drivers, etc.

     3. Note or determine the time required.




09.08.2021                       EN-INST-A+W Enterprise CAD Service.docx                 1
Content

   1         Installation of the A+W Enterprise 6 CAD Service ............................ 3
   1.1       Overview and the basics ........................................................................................ 3
   1.2       Time requirement .................................................................................................. 3
   1.2.1     Installation time for the software .......................................................................... 3
   1.3       Requirements ........................................................................................................ 4
   1.3.1     Windows Server Version........................................................................................ 4
   1.3.2     Network ................................................................................................................. 4
   1.3.3     Software ................................................................................................................ 4
   1.4       Procedure .............................................................................................................. 4
   1.5       IncompatibilitiesIncompatibilities........................................................................ 16
   1.6       Directory structure .............................................................................................. 16
   1.6.1     DATEI_REF_PFAD ................................................................................................. 16
   1.6.2     SNFILES_DIR ......................................................................................................... 16
   1.7       Result of the installationResult of the installation ............................................... 16
   1.8       Configuration ....................................................................................................... 16
   1.9       Tips and tricks ...................................................................................................... 16
   1.9.1     AutoUpdate ......................................................................................................... 16
   1.9.2     Known errors and workarounds .......................................................................... 17
   1.10      Uninstalling .......................................................................................................... 17




09.08.2021                               EN-INST-A+W Enterprise CAD Service.docx                                                      2
1 Installation of the A+W Enterprise 6 CAD Service
The following installation instructions assume that there is no previous version installed.
An update of an earlier release version of the A+W Enterprise 6 CAD Service is executed precisely
like a new installation.
An update of an earlier version of the CAD Service, e.g. from A+W Enterprise 5 CAD Service to A+W
Enterprise 6 CAD Service is not possible. Only one version of the CAD Service should be installed.
This document describes only the installation and configuration of the A+W Enterprise 6 CAD
Service. In case of questions about the installation or configuration of dependent set-ups/disk sets,
please see the installation instructions for these products.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during installation:
    -   Installation and configuration of the Informix driver via setnet32.exe
    -   Creation of the necessary set-ups/disk sets
            o A+W CAD Designer (Shapes)
            o A+W Enterprise 6 CAD Service
            o A+W Infrastructure 6 Collector Services
            o A+W Infrastructure 6 Middleware
            o Java 7 Update 51
            o A+W Setup Launcher
    -   Installation of the CAD Service and the dependent disk sets with the Setup Launcher
    -   Configuration of the CAD Service with the ConfigTool

1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the installation and
the conversion of the existing data:

1.2.1   Installation time for the software
Depending on the computer, storage space, and configuration, the installation times will vary for
different computers. The installation time specified was determined using a reference device with
the following characteristics:
    -   Processor: 3000 Mhz
    -   RAM: 4 GB
    -   Other: /
For an initial or new installation, an installation time of 5 minutes must be anticipated for the
reference device. For higher or lower-power hardware, shorter or longer installation times must be
anticipated.




09.08.2021                        EN-INST-A+W Enterprise CAD Service.docx                              3
1.3 Requirements
1.3.1 Windows Server Version
Supported operating systems:

    •   Windows 2008 Server R2 32/64bit.
    •   Windows 2012 Server R2 32/64bit.


1.3.2   Network
For the installation itself, no network access is necessary.
For the operation of the service, there must be a connection to the A+W Enterprise DB Server and
the company network.

1.3.3 Software
It is assumed that the following disk sets were already installed and configured BEFORE the
installation of the A+W Enterprise 6 CAD Service disk set.

    •   Informix Client SDK 3.5 TC9 (or newer)
    •   Microsoft .NET Framework 4.5.1 SDK


1.4 Procedure
For the installation, please proceed in the following sequence:

1. Use setnet32.exe to configure the database server and hosts. This assumes that an IBM Informix
   Client SDK was installed (see software requirements).

2. Installation of the A+W Enterprise 6 CAD Service with the Setup Launcher

    On the Component Selection dialog on the A+W Enterprise node, select the "A+W Enterprise 6
    CAD Service" module. This automatically selects all dependent set-ups.




09.08.2021                         EN-INST-A+W Enterprise CAD Service.docx                          4
09.08.2021   EN-INST-A+W Enterprise CAD Service.docx   5
3. After the successful installation, the CAD Service is configured with the Config Tool.

    3.1. Common Settings




        3.1.1.   Polling Interval

                 In the Polling Interval (Seconds) field, the number of seconds is set that the service
                 waits until it checks the sntransfer transfer table again for new data records. The
                 default value is 20 seconds.

        3.1.2.   CAD Export Types

                     o   Type A: Generation of SN files and machine export for product sets based
                         on templates.

                     o   Type B: Generation of SN files for order items based on templates.

                 The CAD Service currently recognizes two processing types. The correct
                 configuration can only be made in consultation with Development since both types
                 were developed based on special customer requirements.



        3.1.3.   Background iTOE



09.08.2021                          EN-INST-A+W Enterprise CAD Service.docx                           6
                 o   SN file synchronization: generation of SN files based on templates with
                     simultaneous synchronization of the AWE BOM with the template file.

                 At the moment, iTOE can only be activated with the export type B. There is a
                 detailed description of this in the configuration document for the A+W Enterprise
                 CAD Service.



        3.1.4.   Protocol-Button

                 With the Protocol button, you can reach the Protocol Configuration dialog. This
                 automatically selects all dependent set-ups. On the first tab, the trace categories for
                 the frontend are configured; on the following tabs, the tracing of dependent
                 modules and programs can be activated if necessary.




             The following trace levels are distinguished:
             o Fatal



09.08.2021                         EN-INST-A+W Enterprise CAD Service.docx                             7
             o   Error".
             o   Warning
             o   Info
             o   Debug

             With the Protocol button, you can reach the Protocol Configuration dialog. If, for
             example, the Info level is active, trace messages of the type Error and Warning will also
             be written into the tracing file.

             The tracing file is always in the directory %ProgramData%\A+W\Log. The file name
             consits of the service name, the current date and the process number and ends with
             .awtrc.

             The A+W Enterprise CAD Service currently uses no log protocol.




09.08.2021                        EN-INST-A+W Enterprise CAD Service.docx                            8
    3.2. Database settings

        On this dialog, all database-precise settings are configured, starting with the database itself.




             o   With the New button, you can edit an existing configuration.
             o   With the Edit button, you can delete an existing configuration.
             o   With the Delete button, you can delete an existing configuration.




09.08.2021                        EN-INST-A+W Enterprise CAD Service.docx                                  9
        3.2.1.   Data Source Properties

                 With the New or Edit buttons or with a double-click on a row in the table, you reach
                 the Site Properties dialog. Here, all database-dependent settings can be made.




        3.2.2.   Database settings
            o    In the Data Source Name field, a name is entered for the data source. The name can
                 be selected at will and has no further meaning than making the data source
                 identifiable for the user. The name stored here plays no role in the establishing of
                 the database connection.


09.08.2021                        EN-INST-A+W Enterprise CAD Service.docx                           10
             o   The ERP Type field cannot currently be changed. It defines the connected ERP
                 system. At the moment, only a connection to A+W Enterprise is possible.
             o   In the ERP Site field, the main site number of the connected ERP system is stored.
             o   The Database Type field cannot currently be changed. It defines the database type.
                 Thanks to the exclusive connection to A+W Enterprise, the database type is
                 specified as Informix.
             o   The database server is entered in the Server Name field. Via the combo box, all DB
                 servers entered in the setnet32 can be selected.
             o   A user name that has access to the database must be entered in User Name.
             o   If the fields Server Name, User Name, and Password are filled with valid values, the
                 Database Name combo box already contains all available database names of the
                 database server.
             o   The appropriate locale settings are entered in the Client Locale and DB Locale fields.
                 The combo boxes already contain most values used. If it is necessary to enter
                 deviating values, this is also possible manually.
             o   In the Background Process Host field, the server is entered on which the background
                 processes of the connected A+W Enterprise are working.


        3.2.3.   DB Functions
            o    With the Start Setnet32 button, it is possible to start the setnet32.exe program
                 directly; with it, database server/hosts can be set up.
             o   With Check Alenv you can check the A+W Enterprise environment variables for this
                 service and view the current database configuration. Since this dialog is only for
                 checking purposes, it will not be described in any more detail. The settings of the
                 Alenv variables are made in A+W Enterprise.
             o   The Test Connection button allows you to check the current values of the database
                 configuration. If a database connection can be established with this values, you will
                 see the following message box; otherwise an error message.




    3.3. Template Settings

        This dialog is only relevant if in Common Settings the export type A was selected.




09.08.2021                        EN-INST-A+W Enterprise CAD Service.docx                                11
        The machine assignment for each template that is used in the CAD export is entered here
        and it is decided whether in particular views in the SN the drill holes should be removed.




        3.3.1.   Template Properties

             o   In the Template Name field, the name of the template without extension (.sn) is
                 stored.




09.08.2021                       EN-INST-A+W Enterprise CAD Service.docx                         12
             o   The assigned machines are stored in the Machines field. The machines are required
                 to generate the machine driver.

             o   With the Delete Drill Hole checkbox, it is specified whether in particular views of the
                 SN the drill holes should be removed.



    3.4. E-Mail Settings

        On this dialog, the sending of e-mails from the CAD Service is configured.




             o   In the SMTP Server field, the SMTP server is specified.
             o   In the Port field, the SMTP port is specified.
             o   In the From Server field, the sender's address is stored.
             o   In the To field, the recipient's address is stored. Several recipients can be specified
                 separated by semicolons.
             o   In the CC field, the address of the CC recipient is stored. Several CC recipients can be
                 specified separated by semicolons.
             o   With the Authentication checkbox, the authentication of the E-mail recipient can be
                 forced. Account and Password are only relevant if Authentication was selected.


09.08.2021                         EN-INST-A+W Enterprise CAD Service.docx                             13
                       In the Account field, the authentication user is stored for Authentication.
                       In the Password field, the user's password is stored for Authentication.
                       In the Confirm Password field, the password for Authentication is
                        confirmed.
             o   With the Enable SSL checkbox, it is possible to activate SSL encryption.




    3.5. Maintenance Settings

        Use this dialog to configure the clean up-time for processed records in table sntransfer.




             o   In field Clean Up Time Success the clean up time in days is specified for successfully
                 processed records.
             o   In field Clean up Time Error the clean up time in days is specified for processed
                 records in sntransfer, that encountered an error.




09.08.2021                        EN-INST-A+W Enterprise CAD Service.docx                            14
    3.6. Windows Service configuration




        The service users are stored on the Windows Service Configuration dialog. These are
        Windows users who are used to access external objects such as network paths, etc. This
        user must have the appropriate rights.

        With the Pick user... button it is possible to select a domain user.

        If no network domain is available, e.g. because the service was installed on a PC, the value
        "." can be entered in the Domain field.

        If no user is available, the service can also run under "LocalSystem" in case of emergency.
        This is the default services user in a Windows system.

        Currently no parallel services can be installed. If necessary, please contact Development.

4. Now the A+W Enterprise 6 CAD Service is ready and it writes a log into the directory named
   above.

5. Setting of A+W Enterprise environment variables




09.08.2021                        EN-INST-A+W Enterprise CAD Service.docx                            15
1.5 IncompatibilitiesIncompatibilities
        No incompatibilities are known.

1.6 Directory structure
1.6.1 DATEI_REF_PFAD
        The env variable DATEI_REF_PFAD is defined in AWE. The file path stored here (or
        a superior path) must be connected as network drive on the Windows server.
        Both the CAD service as well as the access rights required by SN to the path
        stored in DATEI_REF_PFAD as well as all subdirectories.


1.6.2 SNFILES_DIR
        The env variable SNFILES_DIR is defined in AWE. The file path stored here (or a
        superior path) must be connected as network drive on the Windows server.
        Both the CAD service as well as the access rights required by SN to the path
        stored in SNFILES_DIR as well as all subdirectories.
        This is the directory in which the SN file generated by the CAD Service is saved.
        (General remark: If an existing SN file should be opened (specification in
        kposp.brokefile), it is opened by SN from this directory.)
        WARNING: The path specification must end with a backslash! (In contrast to the
        path specification in DATEI_REF_PFAD)!


1.7 Result of the installationResult of the installation
If the service could be started, the installation was successful. Otherwise, the trace log is available
for determining possible problems.

1.8 Configuration
For additional configurations, please see the CAD Service documentation.

1.9 Tips and tricks
1.9.1   AutoUpdate
        In order to be able to install the service via AutoUpdate, the setup must have
        been installed successfully at least once with the Setup Launcher and configured
        with the ConfigTool.



09.08.2021                         EN-INST-A+W Enterprise CAD Service.docx                                16
1.9.2   Known errors and workarounds

1.10 Uninstalling
You can uninstall the program as usual via Control Panel -> Programs and Functions.




Note: The config file is not deleted automatically. For a final uninstallation, the program directory of
the A+W Enterprise 6 CAD Service must be deleted manually.




09.08.2021                        EN-INST-A+W Enterprise CAD Service.docx                              17

