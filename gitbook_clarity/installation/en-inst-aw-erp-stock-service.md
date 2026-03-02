---
description: "EN INST A+W ERP Stock Service"
---



# EN INST A+W ERP Stock Service

          Installation Instructions

          A+W ERP Stock Service 6
   Change history:
    Date           Edited by                Remarks                                       Version
    13.07.17       SVH                      Original version                              0.9
    15.09.21       SVH                      AWDesk #338820                                1.1
    16.12.13       MP                       AutoUpdate                                    1.2
    2018-04-13     SVH                      AWDesk #391319
    2020-11-06     SVH                      AWDesk #461784 – Ignore Thickness
    2022-04-05     SVH                      [AW-76610] - purchase logic (only with AWE)




     The installation instructions will assist the planner with the installation and
     configuration of the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




09.05.2022                           EN-INST-A+W ERP Stock Service.docx                     1
Content

   Installation Instructions ..................................................................... 1

   A+W ERP Stock Service 6 ................................................................. 1

   1         New Installation of Version [No.] ........................................... 5
   1.1       Overview and the basics ............................................................................ 5
   1.2       Time requirement ....................................................................................... 5
   1.2.1     Installation time for the software ................................................................. 5
   1.2.2     Conversion Time for Data Set .................................................................... 5
   1.3       Requirements ............................................................................................. 5
   1.3.1     Hardware .................................................................................................... 5
   1.3.2     Network ...................................................................................................... 5
   1.3.3     Software ..................................................................................................... 6
   1.4       Procedure ................................................................................................... 7
   1.4.1     Trace settings ............................................................................................. 7
   1.4.2     Database settings ....................................................................................... 8
   1.4.3     Hegla Communication Settings ................................................................ 11
   1.4.4     Lisec Communication Settings ................................................................. 14
   1.4.5     Bystronic communication settings ............................................................ 17
   1.4.6     E-Mail Settings ......................................................................................... 19
   1.4.7     Service configuration ................................................................................ 20
   1.5       Incompatibilities ........................................................................................ 21
   1.6       Directory structure .................................................................................... 21
   1.7       Settings .................................................................................................... 21
   1.7.1     Parameters ............................................................................................... 21
   1.7.2     Customer-Specific Configuration .............................................................. 21
   1.7.3     Registry .................................................................................................... 21
   1.8       Result of the installation ........................................................................... 22
   1.9       Configuration ............................................................................................ 22
   1.9.1     ERP systems ............................................................................................ 22
   1.10      Alternative Installations............................................................................. 22
   1.11      Patches .................................................................................................... 22
   1.12      Tips and tricks .......................................................................................... 22
   1.12.1    AutoUpdate .............................................................................................. 22
   1.12.2    FAQs ........................................................................................................ 22
   1.12.3    Known errors and workarounds ................................................................ 22


09.05.2022                               EN-INST-A+W ERP Stock Service.docx                                                2
   1.13      Uninstalling ............................................................................................... 23

   2         Update Version [NO.-1] ......................................................... 24
   2.1       Overview .................................................................................................. 24
   2.2       Time requirement ..................................................................................... 24
   2.2.1     Installation time for the software ............................................................... 24
   2.2.2     Conversion Time for Data Set .................................................................. 24
   2.3       Requirements ........................................................................................... 24
   2.4       Procedure ................................................................................................. 24
   2.5       Incompatibilities ........................................................................................ 24
   2.6       Directory structure .................................................................................... 24
   2.7       Settings .................................................................................................... 25
   2.7.1     Parameters ............................................................................................... 25
   2.7.2     Customer-Specific Configuration .............................................................. 25
   2.7.3     Registry .................................................................................................... 25
   2.8       Result of the installation ........................................................................... 25
   2.9       Configuration ............................................................................................ 25
   2.10      Alternative Installations............................................................................. 25
   2.11      Patches .................................................................................................... 25
   2.12      Tips and tricks .......................................................................................... 25
   2.13      Uninstalling ............................................................................................... 25

   3         Update Version [No.-?].......................................................... 26
   3.1       Overview .................................................................................................. 26
   3.2       Time requirement ..................................................................................... 26
   3.2.1     Installation time for the software ............................................................... 26
   3.2.2     Conversion Time for Data Set .................................................................. 26
   3.3       Requirements ........................................................................................... 26
   3.3.1     Hardware .................................................................................................. 26
   3.3.2     Network .................................................................................................... 26
   3.3.3     Software ................................................................................................... 26
   3.4       Procedure ................................................................................................. 26
   3.5       Incompatibilities ........................................................................................ 26
   3.6       Directory structure .................................................................................... 26
   3.7       Settings .................................................................................................... 26
   3.7.1     Parameters ............................................................................................... 26
   3.7.2     Customer-Specific Configuration .............................................................. 26
   3.7.3     Registry .................................................................................................... 26



09.05.2022                               EN-INST-A+W ERP Stock Service.docx                                                3
   3.8       Result of the installation ........................................................................... 26
   3.9       Configuration ............................................................................................ 26
   3.10      Alternative Installations............................................................................. 26
   3.11      Patches .................................................................................................... 26
   3.12      Tips and tricks .......................................................................................... 26
   3.13      Uninstalling ............................................................................................... 26

   4         Appendix ................................................................................ 27
   4.1       Checklist [Name] ...................................................................................... 27
   4.2       Parameter list ........................................................................................... 27
   4.3       INI file(s) ................................................................................................... 27




09.05.2022                                EN-INST-A+W ERP Stock Service.docx                                                 4
1 New Installation of Version [No.]
The following installation instructions assume that there is no previous version
installed. The set-up and other configuration possibilities are described in the start-
up documentation.

1.1 Overview and the basics
The following list provides an overview of the work that must be done during
installation:
    -   Install LicenseClient
    -   Install Stock Service



1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data:
1.2.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times
will vary for different computers. The installation time specified was determined
using a reference device with the following characteristics:
    -   Processor:
    -   RAM:
    -   Miscellaneous
For an initial or new installation, an installation time of y minutes must be anticipated
for the reference device. For higher or lower-power hardware, shorter or longer
installation times must be anticipated.
1.2.2 Conversion Time for Data Set
Time for the conversion of existing data must be expected.
Name the duration and basis

1.3 Requirements
What is required or assumed, what must be on hand? What are the requirements for
the integration of particular components in other products (e.g. TAB, SN_ALCIM,
etc.)
1.3.1 Hardware
Dongle, scanner, printer, digi-table, machine
1.3.2 Network
IP addresses, access data


09.05.2022                      EN-INST-A+W ERP Stock Service.docx                          5
1.3.3 Software
The Stock Service 6 can be operated with the ERP systems ALCIB 2011 and A+W
Enterprise 6.
Starting with Version 5, SP 3, the Stock Service can also be made available for A+W
Business.


1.3.3.1 ALCIB 2011 and A+W Enterprise 5 and 5.1
        1. Bring the database up to the correct status. To do this, execute the
           SQL script from the installation directory of A+W Enterprise 5.2
           "xsql\12\1\2\120102012_wlportalsync.sql".


1.3.3.2 ALCIB 2011
        1. Install a current alcib binfile (buildnr >= 4082).
        2. Install a current wlager binfile (buildnr >= 2035).
        3. Bring the database up to the correct status. To do this, execute the
           SQL script from the installation directory of A+W Enterprise 5
           "xsql/12/1/0/120100008_wlraum_sql" or execute the following update
           statement:
           "ALTER TABLE wlraum ADD (welnr INTEGER DEFAULT 0);"
        4. Add files to the stock area. The files must be retrieved from the
           appropriate language version ALCIB 2011. The following files must be
           installed:
               a. $PRG/lager/mfo/wlraump.mfo
               b. $PRG/lager/pan/wlraump.pan (language-dependent)
               c. $PRG/lager/sel/wlraum_welnr.sel (language-dependent)
               d. fx_texte/messages (language-dependent, date > 12.10.2011)
        5. Create the A+W Enterprise environment variable WL_PORTALLAGER
           and activate it with "ON".


1.3.3.3 A+W Enterprise 5 and 5.1
        1. Install a current alcib binfile (buildnr >= 427)
        2. Install a current wlager binfile (buildnr >= 155)




09.05.2022                       EN-INST-A+W ERP Stock Service.docx                   6
1.4 Procedure
For the installation, please proceed in the following sequence:
        1. Call up the SetupLauncher

        2. Select the A+W ERP Stock Service for installation

        3. Start the installation

        4. After the installation, the config tool of the Stock Service is started automatically:


1.4.1 Trace settings




        The "debug" level should only be activated for research purposes.




09.05.2022                           EN-INST-A+W ERP Stock Service.docx                             7
1.4.2 Database settings




The dialog provides an overview of all configured database connections.
New connections can be added ([New] button) and existing connections edited
([Edit] button) or deleted ([Delete] button).




09.05.2022                   EN-INST-A+W ERP Stock Service.docx               8
1.4.2.1 Data Source Properties




        If you create a new database connection or edit an existing one, you reach
        this dialog.



09.05.2022                    EN-INST-A+W ERP Stock Service.docx                     9
        Database settings
        1. Data source name:       can be selected freely but must be unique
        2. ERP type:               AWE or AWB
        3. ERP site:               Site number
        4. Database type:          Informix, SQLBase, SQLServer
        5. Database server:        Database server name
        6. Database name:Database name
        7. Database user:          Database user
        8. Database password:      User's password
        9. Confirm password:        Confirmation of the password
        10. Client Locale:         ClientLocale setting
        11. Database Locale:       DBLocale setting
        12. Background Process Host: Only important for AWE, name of the
            server on which the stock booker runs
        13. Button “Check Alenv”: Shows important alenv variables, only AWE


        AWSOA settings ([AW-76610] - purchase logic, only AWE)
        1. Checkbox „Use AWSOA“
           Using the AWE purchaseservice
        2. AWSOA Login Name
           User for the use of the AWE purchaseservice, the stored name must
           exist in the AWE employee master as login name (mitarb.loginname)
        3. AWSOA Multisite ID
           Client number of the purchaseservice in case of a multisite installation,
           the client numbers available for selection are displayed in the drop-
           down menu of the field.
        4. Date Range Into Past (days)
           The number of days to search for open purchase orders in the past,
           starting from the current date, is entered.
        5. Date Range Into Future (days)
           The number of days to search for open purchase orders in the future,
           starting from the current date, is entered.


09.05.2022                     EN-INST-A+W ERP Stock Service.docx                      10
1.4.3 Hegla Communication Settings




The dialog provides an overview of all configured Hegla stock connections.
    1. Checkbox: Hegla communication active:           Activation of the Hegla
       connection. Only if there is a check in the checkbox is the appropriate license
       queried when the Stock Service is started and the configured connections are
       considered.
    2. Store Balance Time:        Start time for the nightly stock reconciliation,
       Format: hh:mm, the start time applies for all configured connections




09.05.2022                     EN-INST-A+W ERP Stock Service.docx                    11
1.4.3.1 Hegla communication properties




09.05.2022                  EN-INST-A+W ERP Stock Service.docx   12
        If you create a new Hegla stock connection or edit an existing one, you
        reach this dialog.
        A) Checkbox: Communication Active: Individual                 connections     can   be
           switched active separately from one another
        B) Stock settings
              1. Stock ID:          Number of the connected ERP stock
              2. Cover Sheet Stock ID: Number of connected ERP cover sheet
                 stock
              3. Stock MP:          Number of the ERP stock market partner
        C) Hegla Communication Settings
              1. Host:       Hegla Server Name
              2. Port:       Hegla Server Port, generally 10010
              3. Client ID: Generally 1, if several connections go on the same
                 server, the ID must be incremented
              4. Measurement: Measurement                 unit       during     communication,
                 presently just in "mm".
              5. Checkbox „Allow Inward Stock Booking”:
              6. Checkbox:      "Ignore broken lites":                  (default
                 setting/recommended setting: disabled)
              7. Checkbox „Ignore Thickness“:      Ignore                     glass   thickness
                 during article mapping (AWDesk #461784)


        D) Database settings
              1. Datasource Name:       Selection of the connected ERP
                 datasource, all following fields are only display fields for the
                 selected data source.




09.05.2022                      EN-INST-A+W ERP Stock Service.docx                                13
1.4.4 Lisec Communication Settings




The dialog provides an overview of all configured Lisec stock connections.
    1. Checkbox: Lisec communication active:           Activation of the Lisec
       connection. Only if there is a check in the checkbox is the appropriate license
       queried when the Stock Service is started and the configured connections are
       considered.
    2. Store Balance Time:        Start time for the nightly stock reconciliation,
       Format: hh:mm, the start time applies for all configured connections




09.05.2022                     EN-INST-A+W ERP Stock Service.docx                    14
1.4.4.1 Lisec communication properties




09.05.2022                  EN-INST-A+W ERP Stock Service.docx   15
        If you create a new Lisec stock connection or edit an existing one, you
        reach this dialog.
        E) Checkbox: Communication Active: Individual                 connections   can   be
           switched active separately from one another
        F) Stock settings
              1. Stock ID:          Number of the connected ERP stock
              2. Cover Sheet Stock ID: Number of connected ERP cover sheet
                 stock
              3. Stock MP:          Number of the ERP stock market partner
        G) Lisec Communication Settings
              1. Host:       Lisec Server Name
              2. Port:       Lisec Server Port
              3. Client ID: Generally 1, if several connections go on the same
                 server, the ID must be incremented
              4. Measurement: Measurement                 unit       during   communication,
                 presently just in "mm".
              5. Server name: please ask Lisec.
              6. Client name: please ask Lisec.
              7. Lisec client name: please ask Lisec.
        H) Database settings
              1. Datasource Name:       Selection of the connected ERP
                 datasource, all following fields are only display fields for the
                 selected data source.




09.05.2022                      EN-INST-A+W ERP Stock Service.docx                             16
1.4.5 Bystronic communication settings




The dialog provides an overview of all configured Bystronic stock connections.
    1. Checkbox: Bystronic communication active: Activation of the Bystronic
       connection. Only if there is a check in the checkbox is the appropriate license
       queried when the Stock Service is started and the configured connections are
       considered.
    2. Store Balance Time:        Start time for the nightly stock reconciliation,
       Format: hh:mm, the start time applies for all configured connections




09.05.2022                     EN-INST-A+W ERP Stock Service.docx                    17
1.4.5.1 Bystronic communication properties




        If you create a new Bystronic stock connection or edit an existing one, you
        reach this dialog.
        A) Checkbox: Communication Active: Individual               connections   can   be
           switched active separately from one another
        B) Stock settings




09.05.2022                     EN-INST-A+W ERP Stock Service.docx                            18
              a. Stocks:        Numbers of the connected ERP stocks, for
                 Bystronic (in contrast to Hegla), several stocks can be
                 connected.
              b. Stock MP:         Number of the ERP stock market partner
        C) Bystronic communication settings
              a. Host:    Bystronic Server Name
              b. Port:    Bystronic Server Port
              c. Checkbox:         Permit incoming goods
        D) Database settings
              a. Datasource Name:       Selection of the connected ERP
                 datasource, all following fields are only display fields for the
                 selected data source.




1.4.6 E-Mail Settings




09.05.2022                     EN-INST-A+W ERP Stock Service.docx                   19
On the dialog, the e-mail settings are made so that the Stock Service can send
information via e-mail if necessary.
    1. SMTP Server:        SMTP Server Name
    2. Port:               SMTP Server Port
    3. From:               E-mail address of the sender
    4. To:               E-mail address of the recipient, several recipients
       separated by a semicolon
    5. CC:               E-mail address of the CC recipient, several CC recipients
       separated by a semicolon
    6. Checkbox: Authentication:        Activate authentication, only if the
       checkmark is placed is the specified account considered.
    7. Account:            E-mail account for the authentication
    8. Password:           Password for the account
    9. Confirm password: Confirmation of the password
    10. Checkbox: Enable SSL:      Activate SSL encryption


1.4.7 Service configuration




09.05.2022                     EN-INST-A+W ERP Stock Service.docx                20
The configuration of the service user is done on this dialog. The configuration is
optional.
    A) Service configuration
             1. Domain:                 Domain of the service user
             2. User:                   Name of the service user
             3. Password:               Password of the service user
             4. Confirm password: Confirmation of the password
    B) Parallel Services
       Currently only a single service can be configured, that is, there are no parallel
       services.



1.5 Incompatibilities
Software does not run with ...

1.6 Directory structure
    -   What must be created
    -   What must be stored where
    -   What the program expects
    -   What the program creates
    -   Where what is saved



1.7 Settings
Which settings must be checked or set?
    -   What effects do different settings have?
    -   Which parameters are there and what is their meaning? (complete list)
1.7.1 Parameters
Which environment switches can be set – for what?
1.7.2 Customer-Specific Configuration
What can/must be set customer-specifically?
1.7.3 Registry
What in the registry must be checked, heeded, added?




09.05.2022                          EN-INST-A+W ERP Stock Service.docx                 21
1.8 Result of the installation
How can you check whether the installation was executed correctly?

1.9 Configuration
1.9.1 ERP systems
The instructions for the configuration of connected ERP systems are in the
documentation \\jupiter\Doku_DocuWare\ALCIB-
PMS\LAGER\User_Manuals\StockService.docx


1.10 Alternative Installations
Network protocols (FTP, mounting), depending on the machine

1.11 Patches
Designation           Description                          Prerequisite




1.12 Tips and tricks
1.12.1 AutoUpdate
        In order to be able to install the service via AutoUpdate, the setup must
        have been installed successfully at least once with the Setup Launcher and
        configured with the ConfigTool.
1.12.2 FAQs
1.12.3 Known errors and workarounds
1.12.3.1      Dependencies of the Stock Service
        If after reboot of the server on which the Stock Service is running, the
        following e-mail is sent:
        "
        ATTENTION: No valid license found for Hegla Stock Service. <[LS0109]
        Internal error during establishment of the connection to the license server.>
        Please contact your project manager.
        "


09.05.2022                     EN-INST-A+W ERP Stock Service.docx                       22
        Then dependencies must be entered manually in the service properties for
        the Stock Service. The dependencies are:
             o   AWCLCService
             o   AWLicenseProxyWatcher




1.13 Uninstalling
To uninstall the software...
When, why, how must uninstallation occur?




09.05.2022                       EN-INST-A+W ERP Stock Service.docx                23
2 Update Version [NO.-1]
The following installation description only describes the points that differ from the full
installation described above and that must be heeded for an update.

2.1 Overview

2.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data:
2.2.1 Installation time for the software
Based on the version [n-1], the program can be installed on the reference device in
approx. x minutes.
2.2.2 Conversion Time for Data Set
The installation time for the different computers depends on the computer type,
storage space, and configuration. The conversion time specified was determined
using a reference device with the following characteristics:
    -   Processor:
    -   RAM:
    -   Miscellaneous
For the required data conversion, a time of approx. 30 minutes plus 1-2 minutes per
GB must be calculated (depending on computer performance).

2.3 Requirements
New installation

2.4 Procedure
        1.

        2.

2.5 Incompatibilities
None/as for new installation

2.6 Directory structure
New installation




09.05.2022                      EN-INST-A+W ERP Stock Service.docx                        24
2.7 Settings
The existing settings are taken over unchanged. You may only have to adapt the
new switches.
2.7.1 Parameters
The following, new environment switches have to be checked/set:
2.7.2 Customer-Specific Configuration
What can/must be set customer-specifically?
2.7.3 Registry

2.8 Result of the installation
See new installation.

2.9 Configuration
See new installation.

2.10 Alternative Installations
none

2.11 Patches

2.12 Tips and tricks
See new installation.

2.13 Uninstalling




09.05.2022                   EN-INST-A+W ERP Stock Service.docx                  25
3 Update Version [No.-?]
The following installation description only describes the points that differ from the full
installation described above and that must be heeded for an update.

3.1 Overview

3.2 Time requirement
3.2.1 Installation time for the software
3.2.2 Conversion Time for Data Set

3.3 Requirements
3.3.1 Hardware
3.3.2 Network
3.3.3 Software

3.4 Procedure

3.5 Incompatibilities

3.6 Directory structure

3.7 Settings
3.7.1 Parameters
3.7.2 Customer-Specific Configuration
3.7.3 Registry

3.8 Result of the installation

3.9 Configuration

3.10 Alternative Installations


3.11 Patches

3.12 Tips and tricks

3.13 Uninstalling



09.05.2022                      EN-INST-A+W ERP Stock Service.docx                       26
4 Appendix


4.1 Checklist [Name]


4.2 Parameter list


4.3 INI file(s)




09.05.2022             EN-INST-A+W ERP Stock Service.docx   27

