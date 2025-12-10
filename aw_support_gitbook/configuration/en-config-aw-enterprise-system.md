---
title: "EN CONFIG A+W Enterprise System"
category: "configuration"
product: "A+W Enterprise System"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W Enterprise System"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration Instructions   A+W Enterprise System                                          english                                  - INTERNAL - Change history  Date             Author           Remarks                                Version 2021-01-28       Ina Seifert      Original version                       1.0                                   5.11     A+W Commercial 6 2021-04-23       Alexander Weil   Converter Service                      1.1                                   5.12"
source_file: "EN-CONFIG-A+W Enterprise System.pdf"
---


# EN CONFIG A+W Enterprise System

    Configuration Instructions


A+W Enterprise System




                                     english




                             - INTERNAL -
Change history

Date             Author           Remarks                                Version
2021-01-28       Ina Seifert      Original version                       1.0
                                  5.11     A+W Commercial 6
2021-04-23       Alexander Weil   Converter Service                      1.1
                                  5.12     A+W iQuote 6
                                  Services/Web
2022-03-11       Jürgen Giesa     7.4 Housekeeping added                 1.2

2022-05-13       Alexander Weil   2.3. Unix  adjustment of              1.3
                                  iceconfig scripts
2022-07-28       Alexander Weil   ICE environment troubleshooting        1.4
                                  entry
2022-09-22       Alexander Weil   Front end chapter added                1.5

2023-05-26       Alexander Weil   ICE environment: Service control       1.6
                                  update
                                  Log added
2023-09-20       Ina Seifert                                             1.7
                                  Platform change AIX Linux introduced
2023-12-11       Ina Seifert      Archiving of documents
2024-05-17       SVH              Table aweprogversion
2024-06-18       SVH              Sketch "Product structure"
Content

1.   Logs                                                                               8
     1.1. Ftest - <Modul>_<PID>-<lfd>.test                                              8
     1.2. alrpc<MMDD>                                                                   9
     1.3. awsoa_documentservice_<pid>_<MMDD>                                            9
     1.4. CEIP<MMDD>                                                                   10
     1.5. CESGG<MMDD>                                                                  10
     1.6. buch.prot - Invoice posting                                                  10
     1.7. bgctrl                                                                       11
     1.8. c<Computername><DDMM> – ctrl_server                                          11
     1.9. connect.prot – socket communication                                          11
     1.10. docexport<MMDD> -Document export                                            12
     1.11. frei<MMDD> - invoice and delivery note                                      12
     1.12. FREI<MMDD> - order release                                                  12
     1.13. gewicht<MMDD>                                                               12
     1.14. gewichtKauf<MMDD>                                                           12
     1.15. iauf<n>.<MMDD>                                                              12
     1.16. Kauf<MMDD>                                                                  12
     1.17. Kuplus<MMDD>                                                                12
     1.18. Lief<MMDD> - delivery note generation                                       13
     1.19. print<MMDD> – start printout                                                13
     1.20. PRODAEND<MMDD>                                                              13
     1.21. rab2005<MMDD>                                                               13
     1.22. Rech<MMDD> - invoice generation                                             13
     1.23. Route<MMDD> - postponement of delivery date                                 13
     1.24. Still<MMDD>                                                                 14
     1.25. Stuf<MMDD>                                                                  14
     1.26. toeneu<MMDD>                                                                14
     1.27. VSGERB<MMDD>                                                                14
     1.28. Waein<MMDD>                                                                 14
     1.29. WaeinTrans<MMDD>                                                            14
     1.30. Environment variables                                                       15
2.   AWE/AWP system diagram                                                            17
3.   ICE environment                                                                     18
     3.1. Prerequisite                                                                   18
     3.2. Prerequisite and installation of the ICE environment                           18
     3.3. Ice 3.7.4                                                                      19
     3.4. Unix                                                                           19
          3.4.1. Environment variables                                                   19
          3.4.2. Configuration                                                           20
          3.4.3. Service control                                                         21
          3.4.4. Autostart IceGridNode                                                   22
     3.5. Windows                                                                        22
     3.6. Troubleshooting                                                                23
          3.6.1. ICE services do not start after conversion of the system names          23
          3.6.2. Change of the IP address of the Windows computer (Unix connection problem)
                  24



A+W Software GmbH            EN-CONFIG-A+W Enterprise System.docx                             3
          3.6.3. Connection problems of Unix IceNode to the Windows IceGridAdmin (Service
          Locator Administrator)                                                        24
          3.6.4. Problem with the communication with the license process                25
          3.6.5. Problems with ICE services and Unix licenceservice or .rc file         25
          3.6.6. Crash of the ICE binaries due to incorrect ICE version                 25
          3.6.7. BasicData/database service transaction problem on start                26
     3.7. Logging                                                                       27
     3.8. Services and Ports                                                            28
          3.8.1. iQuote                                                                 29
          3.8.2. Smart Companion                                                        30
          3.8.3. A+W Logistic Optimizer                                                 30
          3.8.4. CX Dispatch/CX Stock                                                   30
4.   System messages                                                                   31
     4.1. Send manually                                                                32
           4.1.1. Messages of a background process                                     32
           4.1.2. General message                                                      32
     4.2. Overview                                                                     33
     4.3. System message 1                                                             35
     4.4. System message 2                                                             36
     4.5. System message 4                                                             36
     4.6. System message 5                                                             36
     4.7. System message 6                                                             37
     4.8. System message 7                                                             37
     4.9. System message 22                                                            37
     4.10. System message 28                                                           38
     4.11. System message 32                                                           39
     4.12. System message 33                                                           39
     4.13. System message 41                                                           39
     4.14. System message 43                                                           40
     4.15. System message 45                                                           40
     4.16. System message 70                                                           41
     4.17. System message 72                                                           41
     4.18. System message 73                                                           42
     4.19. System message 74                                                           43
     4.20. System message 76                                                           43
     4.21. System message 80                                                           43
     4.22. System message 84                                                           44
     4.23. System message 90                                                           44
     4.24. System message 91                                                           44
     4.25. System message 92                                                           45
     4.26. System message 93                                                           45
     4.27. System message 94                                                           46
5.   Control server (ctrl_server)                                                      47
     5.1. Control (ctrl_serv.par)                                                      47
          5.1.1. Monitoring                                                            48
          5.1.2. System messages from the ctrl_serv.par                                49
          5.1.3. Starting the ctrl_server                                              49
     5.2. Error research                                                               50
          5.2.1. A background process is not started                                   50


A+W Software GmbH             EN-CONFIG-A+W Enterprise System.docx                           4
          5.2.2. Background processes run in an endless loop                            50
          5.2.3. What does the error 111 in the bgctrl log mean                         50
          5.2.4. ctrl_server cannot be stopped with exit_servers                        51
     5.3. Environment variables                                                         51
6.   watchdog                                                                           52
7.   Number server                                                                      53
     7.1. What do the IDs in the NR server log mean?                                    53
     7.2. Pre-population of the next number to be assigned in a number range            54
     7.3. Adjustment of the limit values of a number range                              54
     7.4. Releasing a locked number                                                     54
8.   ZU_SERVER                                                                          55
     8.1. Log $PROTOPFAD/zu_servMMDD                                                    55
9.   Process guard                                                                      56
     9.1. Number server                                                                 57
     9.2. Access server                                                                 57
     9.3. Transfer server                                                               58
     9.4. Control server                                                                58
     9.5. EDI starter                                                                   58
     9.6. Background process handling                                                   58
     9.7. PMS                                                                           59
     9.8. TRM CTRL                                                                      59
     9.9. Report server                                                                 59
     9.10. Environment variables                                                        59
10. Background process "intauf"                                                         61
    10.1. Order transfer to A+W Production                                              61
          10.1.1. Default with cost calculation and stock forecast                      61
          10.1.2. No cost and stock forecast if not released (AWC_POOL_NO_KOSTENKALK)   61
          10.1.3. Setting the time for cost calculation and stock forecast              62
          10.1.4. Margin check including production costs (AWC_CHECK_MARGIN)            62
          10.1.5. Environment variables                                                 65
11. Shared Memory /Master Data Cache                                                    67
    11.1. Speeding up of access to third-party article names                            69
    11.2. Configuration                                                                 69
12. Table aweprogversion                                                                70
    12.1. Apparently incorrect IP address in aweprogversion                             70
          12.1.1. Computer with several IP addresses                                    70
          12.1.2. Computer with dynamic IP address                                      71
          12.1.3. Computer with additional mobile phone network                         71
13. Update                                                                              72
    13.1. Language-dependent descriptions                                               72
    13.2. Bit2Byte – conversion                                                         72
    13.3. Places after the decimal point in SA and PU (DFUE)                            72
    13.4. Market partner-specific configuration (aldfuetyp and aldfuectrl)              73
14. Quality release                                                                     74
    14.1. Installation with environment                                                 74


A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                          5
          14.1.1. Requirements                                        74
          14.1.2. Procedure                                           75
    14.2. AWE (Backend) updates as of Version 6.4                     80
    14.3. New QR - compatibility AWE/AWP/SN                           82
15. SetupLauncher                                                     85
    15.1. Properties                                                  85
    15.2. Research on the setup process in general                    85
    15.3. Research on the setup process for individual programs       86
    15.4. Installation of the A+W Enterprise Frontend                 86
16. Installation/update of Windows components                         87
    16.1. ERP Webservice                                              87
    16.2. A+W Infrastructure & A+W iQuote                             87
    16.3. A+W CAD Services                                            88
17. A+W licensees in AWE Windows programs/services                    90
18. AWE Windows Services - AWE trace settings for research            91
    18.1. ERP Webservice                                              91
          18.1.1. Research in case of incorrect POs                   92
    18.2. OrderXML Service                                            92
    18.3. B2B Service                                                 93
          18.3.1. Research the eInvoicing export                      94
          18.3.2. Research about the EDI export                       95
    18.4. Export Service                                              96
    18.5. AWE CAD Service                                             97
    18.6. Print Service                                               98
    18.7. AWE front end                                               99
          18.7.1. Research about the FinAc export                     99
    18.8. ERP Stock Service                                          101
    18.9. FinAc Service                                              103
    18.10.      BMECat Import                                        104
    18.11.      A+W Commercial 6 Converter Service                   105
    18.12.      A+W iQuote 6 Services/Web                            107
    18.13.      SN connection                                        109
          18.13.1. Trace AWE Frontend                                109
          18.13.2. Trace AWE Frontend – long-term setting            110
          18.13.3. Trace SN                                          111
          18.13.4. Research for the SNLive image file                111
          18.13.5. Research with involved SN file                    111
          18.13.6. Special things to note in the iTOE research       112
19. AWE Windows services - notes                                     113
    19.1. Error messages from the AlbwirBasis                        113
    19.2. E-mail configuration                                       113
          19.2.1. E-mails are not sent                               114
20. Sketch "Product structure"                                       115
    20.1. General Information                                        115
    20.2. Search                                                     115
21. Package release dialog                                           118


A+W Software GmbH             EN-CONFIG-A+W Enterprise System.docx         6
     21.1. Binary activation                                                              118
     21.2. Package release                                                                118
           21.2.1. Configuration of autoupdate                                            119
           21.2.2. Logs                                                                   119
           21.2.3. Troubleshooting                                                        120
     21.3. Requirements                                                                   120
     21.4. Housekeeping                                                                   121
22. Informix error messages                                                               122
    22.1. Informix errors in Windows services                                             122
          22.1.1. SQL0035N The file 'en_us\IBM.Data.Informix.xml' cannot be opened        122
          22.1.2. Not enough space for parser stacks                                      122
23. New installation Informix client SDK (32-bit version)                                 123
24. Possibility for reaction in case nothing happens                                      124
25. Cancel in case of lack of activity                                                    126
26. Front end                                                                             127
    26.1. Problem with SSH proxy connection                                               127
    26.2. Communication with SN/SNLive sketch generation                                  129
          26.2.1. No SN sketches are displayed/the iTOE cannot be started                 129
    26.3. Error message when starting the front end: Missing font: "Bitstream Vera Sans
    Mono"                                                                                 129
27. Subscriber                                                                            130
28. Connecting a Linux server for AWE with an Active Directory domain                     131
29. Keyboard                                                                              132
30. Archiving of documents                                                                134
    30.1. Intention                                                                       134
    30.2. Process                                                                         134
    30.3. Configuration                                                                   135
          30.3.1. Environment variables                                                   135
          30.3.2. Tables                                                                  135
          30.3.3. Files                                                                   136
          30.3.4. Unreferenced deletion                                                   136
    30.4. Logs                                                                            136
    30.5. Known Problems                                                                  136
31. Platform change AIX – Linux                                                           138
    31.1. Scripts $0                                                                      138
    31.2. Environment variables                                                           138
32. Set-up of the CORE dump generation                                                    139
33. Message boxes and their meaning                                                       140
    33.1. Message 15048 in the order entry                                                140




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                            7
1. Logs
Here, "all" known and frequently required for error research logs are listed that are written by the
backend. For frontend and Windows components, see section "AWE trace settings for research"
Not all logs are written permanently; instead, they must be switched on via environment variable
and if necessary configured in their degree of detail.
Some logs can get very large over the course of time. If they should be forwarded to development
for research, they should be shortened to the necessary size.
Furthermore, the logs are not listed here that are written in the course of internal and external
EDI. These are documented in "EN-CONFIG-A+W Enterprise EDI".


1.1. Ftest - <Modul>_<PID>-<lfd>.test
        Source/content        The log can be written by the entire A+W Enterprise backend.
                              Usually this log includes program flows, function calls, keypresses,
                              and such.
        Activation            This log can be activated in the frontend via the system menu
                              Ctrl+F4 - Shift+F12. After pressing the key combination, there is a
                              query about the level. In case of doubt, this should always be 9.
                              Then comes the query whether the output should appear on the
                              screen. Here, the answer should always be "no".
                              It can happen that after switching on the Ftest messages, not more
                              than one window appears on the screen, but rather as Flash
                              message at the lower edge of the screen. If this is the case, the
                              environment variable GLOB_FTEST_LEVEL must be activated.
                              In addition, the Ftest can also be written by background programs.
                              Frequently, environment variables must be activated for this. See
                              section "Environment variables"
        Storage location      The log is written by default to $FTESTPFAD (default:
                              "$DBPATHEXT/ftest").
        Notes                 ATTENTION: Ftest logs can get very large. Be sure to monitor the
                              available disk space.
                              The name of the Ftest log includes the name of the program calling
                              it and the process ID.
                              FTest files break off after a fixed defined number of lines (currently
                              1,000,000 lines). If this happens, a new file with a sequential
                              number is generated (the first new file gets the number 2; the 1st
                              file receives no addition).
                              If a FTest file is written by intauf, before processing, its number, the
                              document, and the still flag are output. During output of a
                              document, the maximum number of lines is ignored in order to
                              prevent a splitting of the output. If the document is completely
                              processed, an end identifier is written.


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                     8
                         With the shell script alprotogrep <auftrnr> <vorgang>
                         <dateimuster> , all blocks that include the specified document
                         number and the document can be copied into a separate document.




1.2. alrpc<MMDD>
      Source/content     This log is written by the background process "alrpc". It provides an
                         overview of the back-end activities of the ERP Webservice.
      Activation         The log is written generally. The log can be set via the ALCIB env
                         variable ALRPC_PROTO (value 0-1).
                         Even with switched-off logging, the calls and important messages
                         are logged! The complete logging can be set with the value 1.
      Storage location   The log is in the $PROTOPFAD. With internal client separation, this
                         variable is evaluated client-specifically. Normally there is a
                         subdirectory with the appropriate client number.
      Notes              In addition to this log, a ftest with the ALCIB env variable
                         ALRPC_FTEST (value has to be entered in the FTEST level, e.g. "9") is
                         switched on.
                         All calls from the ERP Webservice make entries, with the functions
                         called and the values transferred by the ERP Webservice.




1.3. awsoa_documentservice_<pid>_<MMDD>
      Source/content     This log is written by the documentservice. It provides an overview
                         of the back-end activities of A+W iQuote.
      Activation         The log is written generally. The log can be set via the ALCIB env
                         variable AWSOA_LOGLEVEL_DOCUMENTSERVICE (value 1-4).
                             •   LOG_ERROR               1       (default)
                             •   LOG_WARNING             2
                             •   LOG_INFO                3
                             •   LOG_DEBUG               4

      Storage location   The log is in the $PROTOPFAD. With internal client separation, this
                         variable is evaluated client-specifically. Normally there is a
                         subdirectory with the appropriate client number.
      Notes              In addition to this log, a ftest with the ALCIB env variable
                         AWSOAFTEST (value has to be entered in the FTEST level, e.g. "1") is
                         switched on.




A+W Software GmbH          EN-CONFIG-A+W Enterprise System.docx                                  9
1.4. CEIP<MMDD>
      Source/content     This log is written by alcib (document entry 'intauf', invoice
                         generation). It includes function calls and data during the
                         calculation of the technical values.
      Activation         The log is written generally. It can be switched off with the UNIX
                         environment variables "NO_PROTO".
                         Attention: NO_PROTO switches off more logs.
      Storage location   The log is in the $PROTOPFAD. With internal client separation, this
                         variable is evaluated client-specifically. Normally there is a
                         subdirectory with the appropriate client number.
      Notes




1.5. CESGG<MMDD>

      Source/content     This log is written by alcib (document entry 'intauf', invoice
                         generation). It includes function calls and data during the
                         calculation of the CE values.
      Activation         The log is written generally if the CE code is configured
                         appropriately. It can be switched off with the UNIX
                         environment variables "NO_PROTO".
                         Attention: NO_PROTO switches off more logs.
      Storage location   The log is in the $PROTOPFAD. With internal client separation, this
                         variable is evaluated client-specifically. Normally there is a
                         subdirectory with the appropriate client number.
      Notes              Calculation of the technical values for CE codes if this is
                         configured. This is the complex method of SGG based on
                         kposprvfld and cu tables.


1.6. buch.prot - Invoice posting
                         This log is written by alcib.
      Source/content     It logs the various posting processes within invoice posting.
      Activation         No activation is required. The log is written by default.
      Storage location   The log is in the $PROTOPFAD.
      Notes




A+W Software GmbH          EN-CONFIG-A+W Enterprise System.docx                                10
1.7. bgctrl
      Source/content     This log is written by the CTRL server and all processes participating
                         in CTRL server communication (alcib, wlager, pms, etc.). It includes
                         error messages that can occur during this communication.
      Activation         The log is written generally.
      Storage location   The log is in the $PROTOPFAD. With internal client separation, this
                         variable is evaluated client-specifically. Normally there is a
                         subdirectory with the appropriate client number.
      Notes




1.8. c<Computername><DDMM> – ctrl_server
      Source/content     This log is written by the CTRL server. It provides an overview of all
                         requests and activities of the CTRL server.
      Activation         The log is written generally. Via the ALCIB env variable
                         BGCTRL_PROTO (value ON), it is possible to activate an expanded
                         log.
      Storage location   The log is in the $PROTOPFAD. With internal client separation, this
                         variable is evaluated client-specifically. Normally there is a
                         subdirectory with the appropriate client number.
      Notes



1.9. connect.prot – socket communication
      Source/content     This log is written by all processes (ctrl-server, nr_server, zu_server,
                         ue_server, alcib, pms, etc.) that use a socket communication. It
                         includes errors that have occurred during this communication.
      Activation         The log is written generally. Via the ALCIB env variable
                         SOCKET_CONNECT (value ON), it is possible to activate an expanded
                         log. Caution: large quantities of data can be created this way.
      Storage location   The log is in the $IPCDIR. With internal client separation, this
                         variable is evaluated client-specifically. Normally there is a
                         subdirectory with the appropriate client number.
      Notes              Error messages in this file do not necessarily indicate an incorrect
                         system state. The CTRL server tries, e.g. when starting to contact all
                         dependent processes. If this does not work because the
                         corresponding process is not running, this also causes error
                         messages in this file.




A+W Software GmbH         EN-CONFIG-A+W Enterprise System.docx                                    11
1.10.           docexport<MMDD> -Document export
                              This log is written by alcib.
        Source/content        It logs the test whether a document export is made via the table
                              ottransfer.
        Activation            No activation is required. The log is written by default.
        Storage location      The log is in the $PROTOPFAD. With internal client separation, this
                              variable is evaluated client-specifically. Normally there is a
                              subdirectory with the appropriate client number.
        Notes                 The log arose with PF [AW-156062].




1.11.           frei<MMDD> - invoice and delivery note
Creation of invoices and delivery notes


1.12.           FREI<MMDD> - order release
This log is always written regardless of a configuration. It is in $PROTOPFAD.
This log logs whether the question about the order release was posed and how it was answered.
Similiarly, it is logged whether the question about a transfer to dispatch was posed despite
existing dispatch planning and how it was answered.


1.13.           gewicht<MMDD>

1.14.           gewichtKauf<MMDD>

1.15.           iauf<n>.<MMDD>
Mostly not for invoice and credit note generation unless the environment variable
"RECH_MIT_KONFIGTXT" is active.


1.16.           Kauf<MMDD>

1.17.           Kuplus<MMDD>
    •   located in $PROTOPFAD
    •   This log logs the booking of the table "kuplus".

A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                12
    •   written without environment variable


In addition, starting with QR 2403, there is a log table "kuplushistorie". See also "EN-CONFIG-A+W
Enterprise" section "Limit check"




1.18.           Lief<MMDD> - delivery note generation

1.19.           print<MMDD> – start printout
        Source/content       This log is written by alcib or the BinFiles, where print jobs are
                             executed. There is an overview of some central activities for
                             preparation of the data for the print service.
        Activation           The log is activated via the ALCIB env variable PRINT_PROTO (value
                             ON).
        Storage location     The log is in the $PROTOPFAD. With internal client separation, this
                             variable is evaluated client-specifically. Normally there is a
                             subdirectory with the appropriate client number.
        Notes                In addition to this log, an ftest for reworking of print problems
                             before the print service is helpful.




1.20.           PRODAEND<MMDD>

1.21.           rab2005<MMDD>

1.22.           Rech<MMDD> - invoice generation

1.23.   Route<MMDD> - postponement of delivery
   date
        Source/content       In the log, is written by alcib and alrpc.
                             Delivery date calculation logs
        Activation           Activation is done with the environment variable
                             ROUTE_PROTOKOLL
        Storage location     The log is in the $PROTOPFAD. With internal client separation, this
                             variable is evaluated client-specifically. Normally there is a
                             subdirectory with the appropriate client number.



A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                                13
      Notes



1.24.         Still<MMDD>

1.25.         Stuf<MMDD>

1.26.         toeneu<MMDD>

1.27.         VSGERB<MMDD>

1.28.         Waein<MMDD>
      Source/content     In the log, is written by alcib and rserv.
                         The generation and cancellation of goods receipts is logged. The log
                         is written depending on the language.
      Activation         No activation is required. The log is written by default
      Storage location   The log is in the $PROTOPFAD. With internal client separation, this
                         variable is evaluated client-specifically. Normally there is a
                         subdirectory with the appropriate client number.
      Notes




1.29.         WaeinTrans<MMDD>
      Source/content     In the log, is written by alcib and rserv.
                         The transfer (insert in the appropriate transfer tables exportinfo and
                         fibutransfer) of goods receipts to the AWE Windows Services Export
                         Service and FinAc service is logged.
                         The log messages are always in English. The abbreviation "GR"
                         stands for "Goods Received."
      Activation         No activation is required. The log is written by default
      Storage location   The log is in the $PROTOPFAD. With internal client separation, this
                         variable is evaluated client-specifically. Normally there is a
                         subdirectory with the appropriate client number.
      Notes




A+W Software GmbH          EN-CONFIG-A+W Enterprise System.docx                                14
1.30.            Environment variables
ALCIB_FTEST_LEVEL (client reference: no) (employee-dependent: yes)
This variable causes the Ftest log to be generated automatically when the program is started. The
level of the FTest log to be written must be stored as the value.


ALRPC_FTEST (client reference: no)
This variable activates the ftest for the alrpc service. The name of the test file consists of
alrpc_<pid of the alrpc process> and ".test". The content of the variables is the ftest level.
All calls from the ERP Webservice make entries, with the functions called and the values
transferred by the ERP Webservice.


ALRPC_PROTO (client reference: no)
Activates the alrpc log (ON/OFF). The log file is in $PROTOPFAD


AWSOAFTEST (client reference: no)
The FTEST for the AWSOA services is activated with this switch. To be entered is the FTEST level
1-9


AWSOA_LOGLEVEL_DOCUMENTSERVICE (client reference: no)
Log level for the documentservice (A+W iQuote)
0-Fatal 1-Error 2-Warning 3-Info 4-Debug
File: $PROTOPFAD\awsoa_documentservice_<pid>_<MMDD>


FTESTPFAD (client reference: no)
ATTENTION: Unix variable path for ftest files


DFUE_RESEARCH (client reference: no)
With these variables, various research modes of the trm_ctrl and replication can be switched on.
Up to 10 areas are separated by | (pipe).
Currently available: ibout, ibin, mp_replicate, trm_ctrl, art_replicate, rueck, mp, rechrueck, fibu,
ibi_unl - legt unload files of the _i-Tables to $DFUEDIR/proto
ibout_unl: moves unload files of the _-tables to $DFUEDIR/proto
ON: extended logging for all EDI areas (see above)
If this variable is set, the log for this area will be unbuffered
(see also DFUE_PROTO_NOBUFF, REPLICATE_PROTO) and an appropriate FTest will be written.
This is especially interesting for the replication (*_replicate) and the status reporting (rueck).



A+W Software GmbH                 EN-CONFIG-A+W Enterprise System.docx                                 15
GLOB_FTEST_LEVEL (client reference: no)
Global switch for FTEST: messages remain win messages


HINTERGRUNDERZEUGUNG_FTEST (client reference: no)
This variable activates the writing of the FTEST log for the background document generation
(#186075).


INTAUF_TEST (client reference: no)
This variable activates a test log (Ftest) for the background order processing (intauf). The variable
content specifies the desired Helplevel (1-9, default=6). This serves A+W to detect possible errors
in the intauf process.


MPST_FTEST (client reference: no)
If this variable is active, it automatically starts an FTEST when entering the market partner master
and terminates it when leaving the market partner master.


NACHBUCHER_FTEST (client reference: no)
  The variable activates the ftest for the post-booker. The test level is stored as the value.
  (Cf.: 252240)


NO_PROTO (client reference: no)
Switches the extensive logging off. see "EN-CONFIG-A+W Enterprise System"
ATTENTION: This is a UNIX variable


POSZU_TEST (client reference: no)
This environment variable activates the ftest output for content of the table 'poszu' within the
background process "intauf".


PROCGUARDFTEST (client reference: no)
AWDesk #219445: With these variables the FTEST can be activated for the process processguard
and the log depth can be set.


RSERV_FTEST (client reference: no)
Switch on test level for RSERVER




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                16
2. AWE/AWP system diagram




Additional system/process diagrams can be found in
\\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity




A+W Software GmbH           EN-CONFIG-A+W Enterprise System.docx   17
3. ICE environment
ATTENTION: the iQuote-specific settings should be listed in the separate document (EN-CONFIG-
A+W Enterprise iQuote).


3.1. Prerequisite
   •   Under Linux, the version Redhat ES 7 is required. (File: /etc/redhat-release)
   •   For AIX, the Version 7.2 is required.


3.2. Prerequisite                    and         installation             of      the        ICE
   environment
   •   The ICE repositories must be installed:
         1. Check whether repository for ICE is present on the system (as root)
           yum provides ice-all-runtime


           In the version, the packages ice-all-runtime-3.7.4-1.el7.i686 and ice-all-runtime-3.7.4-
           1.el7.x86_64 should be present. If the packages are not present, they must be
           downloaded with the commands from 2.
         2. Supply if the packages are not present (log in again as root)
   cd /etc/yum.repos.d
   wget https://zeroc.com/download/Ice/3.7/el7/zeroc-ice3.7.repo
         3. ICE installation (as root)
               a. Installation of the ICE binaries and the 64-bit libraries:
                      yum install ice-all-runtime-3.7.4-1.el7
               b. Manual reinstallation of the ICE 32-bit libraries:
                      yum install libice3.7-c++-3.7.4-1.el7.i686
         4. If the installation reports problems, the missing packages must be installed after the
            fact.
             On systems without Redhat subscription, these can be obtained after the change in
             the directory /tmp with:
             wget http://mirror.centos.org/centos/7/os/x86_64/Packages/packagename
             and installed there with:
             yum update *.rpm
             installiert werden.
   •   For Linux 8:


A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                             18
            o   Supply of the repository:
                cd /etc/yum.repos.d
                rpm -i https://zeroc.com/download/ice/3.7/el7/ice-repo-3.7.el7.noarch.rpm
            o   The packages then have to be installed individually:
                yum install icegrid-3.7.4-1.el7.x86_64 – if this doesn't work, please try "yum
                install ice-all-runtime-3.7.4-1.el7"
                yum install libice3.7-c++-3.7.4-1.el7.i686
    •   For AIX 7.2:
            o   Supply of the repository:
                yum install https://zeroc.com/download/ice/3.7/aix7.2/ice-repo-
                3.7.aix7.2.noarch.rpm
            o   Installation of the ICE binaries:
            o    yum install ice-all-runtime



3.3. Ice 3.7.4
Since 05/27/2020, the Version 3.7.4 is also present in the repository. During the installation, there
are the following changes:
The command in step 3b now has to be
yum install ice-all-runtime-3.7.4-1.el7.i686
since with yum install ice-all-runtime the 3.7.4 version is installed. If you don't want this, you
have to specify the Version 3.7.3 during the installation of the 64-bit libraries.


3.4. Unix
A+W programs with ICE communication include client applications that have to connect to the
A+W Service Locator (Ice Grid Admin). The client application draws the connection data from the
A+W Service Locator in order to connect to other ICE servers and the A+W Service Locator starts
the required server if necessary.
The A+W Service Locator is the name of the computer on which the (Windows) service "A+W
Infrastructure 6 Service Locator" is running.


3.4.1. Environment variables
A+W Enterprise components that run under Unix require the alenv environment variables in order
to reach the A+W services in Windows. These include, e.g. the dispatch control, the A+W
LogisticBackEndService or the A+W Documentservice.
Environment variable           Value (default/example)           Description
AWSOA_ICEHOST                  -                                 Name of the host on which the



A+W Software GmbH                  EN-CONFIG-A+W Enterprise System.docx                              19
                                                               A+W Service Locator is running
AWSOA_ICEPORT                  12000 (default)                 Port on which the A+W Service
                                                               Locator can be reached
AWSOAFTEST                                                     Activation of FTests for A+W
                                                               SOA services



3.4.2. Configuration
To enter the applications in the A+W Service Locator, two scripts must be called. First, the script
iceconfig_setup must be started; it prepares the configuration of the desired services and writes
into a /tmp/aw_services file. The last /tmp/aw_services file created is backed up when it is
executed again and stored as aw_services.bak.
The content of /tmp/aw_services should be transferred to the file /etc/services in order to ensure
that the communication between Unix and Windows functions perfectly.
Under /etc/hosts, the IP address of the host computer where the Windows components are
installed must be entered. Similarly, the above-mentioned environment variables
AWSOA_ICEHOST and AWSOA_ICEPORT are required.
Now the script iceconfig_execute must be executed. For this, the package iceconfig-2.0.gz must
exist in the scripts directory ($ALCIBPRG/install/config/). The script generates under the
$ALDATPFAD/iceconfig a folder with the Unix computer names and under this, the Service Config
files are accommodated, the ones that are required for communication with the target computer
and the IceGridAdmin (Service Locator).
The iceconfig script mentioned checks the existing settings (AWOSA_ICEHOST, AWSOA_ICEPORT),
reads the /tmp/aw_services file out, generates the required config files under
$ALDATPFAD/iceconfig, which are used to enter them via applications in the A+W Service Locator
of the host computer on Windows.
Important for communication between the registry under Windows and the clients and server
under Unix is that the firewall does not hinder the communication.
Test wise, the firewall can be deactivated with "systemctl stop firewalld" and systemctl disable
firewalld" as root under Linux.
Starting the registry node for the Unix services is enabled via the script "icenodestart" (cdcmd). A
stop of the node can be forced with the script "icenodestop."



On Windows, the registry node can be checked in the Service Locator Administration Tool. A
running registry node is marked in green instead of red.


Figure 1: Unix icegridnode

On Unix, you can search for the running process with "psgrep icegridnode".




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                   20
3.4.3. Service control
Via the script icecmd, the ICE services relevant for A+W Enterprise can be stopped, started, and
the status monitored.
The script is under ALCIBPRG/cmd (cdcmd) and is started with parameters:
state   à      Status query
Example:
awedev-rhel7 130:/develop/alcib/13/0/de/cmd: icecmd state
AWEDEV-RHEL7-Commercial-130-Dispatch-130             inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Document-130-001             inactive (enabled)
AWEDEV-RHEL7-Commercial-130-LogisticBackEnd-130 inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Purchase-130             inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Sales-130              inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Stock-130              inactive (enabled)


start   à      Starts a particular ICE service
Example:
awedev-rhel7 130:/develop/alcib/13/0/de/cmd: icecmd start
start service AWEDEV-RHEL7-Commercial-130-Dispatch-130 (inactive (enabled))? (y|Y) y
AWEDEV-RHEL7-Commercial-130-Dispatch-130             active (pid = 9198, enabled)
start service AWEDEV-RHEL7-Commercial-130-Document-130-001 (inactive (enabled))? (y|Y) y
AWEDEV-RHEL7-Commercial-130-Document-130-001             active (pid = 9266, enabled)
start service AWEDEV-RHEL7-Commercial-130-LogisticBackEnd-130 (inactive (enabled))? (y|Y)
AWEDEV-RHEL7-Commercial-130-LogisticBackEnd-130 inactive (enabled)
…
All inactive services are queried and you confirm with y which ones should be started.


stop    à      Stops a particular ICE service
Example:
awedev-rhel7 130:/develop/alcib/13/0/de/cmd: icecmd stop
stop service AWEDEV-RHEL7-Commercial-130-Dispatch-130 (active (pid = 9198, enabled))? (y|Y) y
AWEDEV-RHEL7-Commercial-130-Dispatch-130             inactive (enabled)
stop service AWEDEV-RHEL7-Commercial-130-Document-130-001 (active (pid = 9266, enabled))?
(y|Y)
AWEDEV-RHEL7-Commercial-130-Document-130-001             active (pid = 9266, enabled)
AWEDEV-RHEL7-Commercial-130-LogisticBackEnd-130 inactive (enabled)


A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                                21
AWEDEV-RHEL7-Commercial-130-Purchase-130               inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Sales-130               inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Stock-130               inactive (enabled)
All active services are queried and you confirm with y which ones should be stopped.


stopall à       Stops all ICE services
Example:
awedev-rhel7 130:/develop/alcib/13/0/de/cmd: icecmd stopall
AWEDEV-RHEL7-Commercial-130-Dispatch-130              inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Document-130-001              active (pid = 9266, enabled) ->
AWEDEV-RHEL7-Commercial-130-Document-130-001              inactive (enabled)
AWEDEV-RHEL7-Commercial-130-LogisticBackEnd-130 inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Purchase-130               inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Sales-130               inactive (enabled)
AWEDEV-RHEL7-Commercial-130-Stock-130               inactive (enabled)
Stopping node AWEDEV-RHEL7-Commercial-130
node is down
All services are switched off and the IceGridNode is disabled.


For separate starting or stopping of the IceGridNode, you can use the following scripts:
icenodestart à Starts the IceGridNode
icenodestop à Stops the IceGridNode
The scripts are under ALCIBPRG/cmd (cdcmd).


3.4.4. Autostart IceGridNode
So that the IceGridNode under Unix starts automatically after a system boot, an adjustment must
be made in the startpar of the Unix server. The startpar is under ALCIBPRG/spec/rc/Rechnername
or cdrc. For multi-site systems, the startpar files have the site number, e.g. "startpar.20." In this
file, the script call icenodestart/2 must be added. Now the IceGridNode starts automatically after
a reboot.


3.5. Windows
The A+W services, such as the A+W Logistics Optimizer and A+W iQuote, run under Microsoft
Windows and draw the connection dat from the Microsoft registry. With these settings, the
connection to the A+W Service Locator is established. These settings are made through the
installation via the Setup Launcher.
This setting data is entered in the course of A+W setup and can be checked in the registry:


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                22
HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\Albat+Wirsam\Communication
    -   ICEHOST                  Name of the host on which the A+W Service Locator is running

    -   ICEPORT                  Port on which the A+W Service Locator can be reached (default:
        12000)
With the Service Locator Administration Tool, the individual services that communicate via the
Service Locator can be checked. To be found in the ..\A+W\Config Tools folder.


3.6. Troubleshooting
3.6.1. ICE services do not start after conversion of the system
    names
After you have converted the system name of the Windows computer, the ICE services in the
IceGrid Admin will not connect anymore and they will not restart.
The reason is that the services depend on the naming and the Windows services that stand
behind them are now searching for incorrect starting points for the start.
This problem can only be resolved if you deinstall and reinstall all ICE services. Then the services
will be configured with the new system name and start as usual.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                   23
Figure 2: ICE Services do not start – IceGrid Admin


3.6.2. Change of the IP address of the Windows computer (Unix
    connection problem)
If the IP address of the Windows computer on which an ICE service is installed changes, then the
ICE services that run under UNIX (e.g. document service for A+W iQuote) will no longer be able to
establish a connection to the IceGrid Admin on the Windows computer.
To eliminate this problem, you must delete under the $ALDATPFAD/iceconfig the existing folder
(name of the folder is the Unix computer name) or rename it. After that, perform the steps under
2.4. Unix again. Mainly the part with the iceconfig script.


3.6.3. Connection problems of Unix IceNode to the Windows
    IceGridAdmin (Service Locator Administrator)
    a. If the connection of the IceNode from the Unix machine to the Terminal Server cannot be
       established, the /etc/hosts entries in Windows and Unix should be checked. It must
       always be ensured that the computers know each other via IP address.
    b. On our test systems, we had the problem that the following error was written to the Ice
       logs:


A+W Software GmbH                     EN-CONFIG-A+W Enterprise System.docx                       24
         05/06/22 16:32:19.151 TROUBAIX-Commercial-140-Dispatch-140: error:
         src/Ice/Network.cpp:2411: ::Ice::SocketException: socket exception: Can't assign
         requested address
         As it turned out, the localhost was overwritten via DNS entry.
         troubaix 140:/etc: nslookup localhost
         Server:         194.39.66.43
         Address:        194.39.66.43#53
         Name: localhost.a-w.intra
         Address: 194.39.67.59
         This problem only occurred under AIX and was eliminated when the DNS entry was
         deleted.


3.6.4. Problem with the communication with the license process
When starting A+W Enterprise, the following message appears:
"Main menu: FX100: communication with licence process failed(send)"
Solution: In the back end (UNIX computer), there is a file /tmp/liserver.log. Please delete this file.


3.6.5. Problems with ICE services and Unix licenceservice or .rc file
This problem should be eliminated if it should occur again, please report directly to
Development!
In rare cases, the following error messages occur:
liserver: .log cannot be created (process running?)
License process "PID" does not seem to be running
License process is started ...
License process "PID" does not seem to be running
Cancel due to failed licensing
These error messages can occur due to problems with the fxinit() or the initialization of A+W
Enterprise in the ICE service. This problem has to be checked by developers.
Similarly, the following problem pattern may occur:
File /develop/alcib/13/0/de/awsoa.rc cannot be read (errno 116)
Initialization failed.
This problem, like the one above, must be checked.


3.6.6. Crash of the ICE binaries due to incorrect ICE version
In the ticket [AW-92613] we had the case that the documentservice crashed on the first function
call after the actual start. (affects all ICE binaries)
Example of documentservice:

A+W Software GmbH                  EN-CONFIG-A+W Enterprise System.docx                                  25
In the gp/awsoa+documentservice_* log, the following lines are the last lines before the crash:
14:53:19: D documentservice::run get service properties
14:53:19: D documentservice::run create adapter
14:53:19: D documentservice::run create service
14:53:19: D documentservice::run adding adapter
14:53:19: D documentservice::run activating adapter
14:53:19: D documentservice::run waiting for shutdown...
The problem was the incorrect ICE runtime version. The version 3.7.6 was installed and currently
(as of 10/25/2021) only version 3.7.4 may be installed on the back end system. In the new ICE
version, there will probably be errors in handling the DTO objects.
So that this behavior does not occur again, under <10.1 Voraussetzung und Installation der ICE
Umgebung> we have adjusted the installation calls (yum install …). The previous call always
installed the latest version. With the new call, 3.7.4 is installed explicitly.


3.6.7. BasicData/database service transaction problem on start
The required services BasicData and database for the A+W Infrastructure can produce the
following errors:
o




Program behavior:
    -   The database service starts, but the above-mentioned error message appears multiple
        times in the log
    -   The BasicData service does not start
The problem is that the database transaction logic that is provided in our software is not
supported. This behavior can be eliminated by switching on Database Logging. Please contact the
database admin in this regard and test again.




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                                26
3.7. Logging
Information about the flow of services is logged. The logging is written to files that are in the
'PROTOPFAD' directory under Unix. The file name has the prefix 'awsoa_' followed by the name of
the application or library and ends with month and day, e.g.:
    •   $PROTOPFAD\awsoa_documentservice_pid_MMDD

The logging can be set on 5 levels. The value of the environment variables is assigned the
appropriate number.
    •   LOG_FATAL               0

    •   LOG_ERROR               1       (default)

    •   LOG_WARNING             2

    •   LOG_INFO                3

    •   LOG_DEBUG               4

The logging of applications that run under Unix is controlled by environment variables. Each
application has its own environment variable:
Environment variable                        Value                  Description
                                            (default/example)
AWSOA_LOGLEVEL_DOCUMENTSERVICE              1/4                    Determines the loglevel for
                                                                   the logging of the A+W
                                                                   Documentservice
AWSOA_LOGLEVEL_STOCKSERVICE                         1/4             Determines the loglevel for
                                                                    the logging of the A+W
                                                                    Stockservice
AWSOA_LOGLEVEL_PURCHASESERVICE                      1/4             Determines the loglevel for
                                                                    the logging of the A+W
                                                                    Purchaseservice
AWSOA_LOGLEVEL_DISPATCHSERVICE                      1/4             Determines the loglevel for
                                                                    the logging of the A+W
                                                                    Dispatchservice
AWSOA_LOGLEVEL_SALESSERVICE                         1/4             Determines the loglevel for
                                                                    the logging of the A+W
                                                                    Salesservice
AWSOA_LOGLEVEL_DATAPROVIDERSERVICE                  1/4             Determines the loglevel for
                                                                    the logging of the A+W
                                                                    DataProviderservice
AWSOA_LOGLEVEL_LOGISTICBACKENDSERVICE 1 / 4                         Determines the loglevel for
                                                                    the logging of the A+W
                                                                    Logisticbackendservice
AWSOA_LOGLEVEL_LOGISTICCLIENT                       1/4             Determines the loglevel for
                                                                    the logging of the A+W
                                                                    Logisticclient (from lapool-

A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                                27
                                                                       otr)


With the AWSOAFTEST variable, the FTEST can be switched on with level 1 to 9 (FTEST level). The
FTEST is used in the area of price calculation and offers a more precise logging for this area. This
FTEST is written, like every other FTEST, and saved in the configured storage location.
AWSOAFTEST                                   -/1                      Switch for activating the
                                                                      FTEST via FTEST level 1 to 9.
AWSOA_EXPLAIN                                -/1                      Switch to enable all services
                                                                      of DB Explain.




3.8. Services and Ports
Essentially, all clients need a connection to the Service Locator (Windows process server, default
port 12000 for TCP or 120003 for WebSocket).
Furthermore, each client must establish a connection (two-way) to the services that it uses:
Client                               Services under Linux         Services under Windows
iQuote                               documentservice              Infrastructure config
                                                                  Web Configurator
                                                                  Converter Service
                                                                  …
Smart Companion                      purchaseservice,             Infrastructure config
                                     stockservice
                                                                  Production?
ERP Stock Service                    purchaseservice              Infrastructure config
CX Dispatch                          dispatchservice              Infrastructure config
CX Stock                             stockservice                 Infrastructure config
Dispatch control (lapool_otr)        logisticbackendservice       Infrastructure config
                                                                  Logistic Service
Each service under Linux needs 2 ports so that it can be called by any type of client (TCP or
WebSocket)!




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                   28
3.8.1. iQuote




A+W Software GmbH   EN-CONFIG-A+W Enterprise System.docx   29
3.8.2. Smart Companion




3.8.3. A+W Logistic Optimizer
Transfer A+W Logistics Optimizer




Return from A+W Logistic Optimizer to AWE




3.8.4. CX Dispatch/CX Stock
Follows...


A+W Software GmbH             EN-CONFIG-A+W Enterprise System.docx   30
4. System messages
A+W Enterprise sends a variety of so-called system messages. These are either activated through
environment variables or via the system menu (sysab table).
Ctrl+F4 – Mail System - System messages
Messages that are sent in the course of internal or external EDI or the master data replication are
documented in the "Messages" section in the separate configuration documentation "EN-CONFIG
A+W Enterprise EDI".
The recipient can be assigned individual messages or the whole message group.
If an employee who should receive messages is not assigned an e-mail address in the employee
master data (master data - employees), then he receives the messages in A+W Enterprise's own
message system (tables almail, almailtxt) and he can call these up there (system menu (Ctrl+F4) -
Mail system - Receive mail).




The messages go to the initiator and the distribution list stored here if "Additionally send to
initiator" has been activated. Here, the initiator refers to the default recipient defined by the
system for the message in question. This person is frequently determined by an environment
variable. That is, if the message should ONLY go to the distributor and NOT to the default
recipient, the field "Additionally send to initiator" may NOT be activated.
If this message should be suppressed completely, this can be done with the "Disable sending"
checkbox.
With the "Additionally send to group distributor" checkbox, you can also send mails to the
distribution list stored here:




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                31
4.1. Send manually
4.1.1. Messages of a background process
alcib -meldnum <loginname or manr of the addressee> <errno for the body>

The messageid 31 with the subject 31218: "background processes" is sent.

Example:

Text: 38533 : "No route is stored for this dispatch type."

Call "alcib -meldnum iseifert 38533"

Result:




4.1.2. General message
alcib –meldnum_ext <alsysab.meldid> <mitarb.manr> <errno-Betreff> <errno-Body> <String-
Zusatz>

A message is sent.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                      32
alsysab.meldid: A messageID from the system message definition. An invalid messageID means
that no message will be sent.

mitarb.manr: This employee counts as the initiator.

errno-Betreff: A text number from the A+W Enterprise system texts (fx_texte) is expected here.
This text is then used as subject of the e-mail.

errno-Body: A text number from the A+W Enterprise system texts (fx_texte) is expected here. This
text is then used as subject of the e-mail.

String-Zusatz: must absolutely be specified! If <errno-Body> expects a %s parameter, this
transferred text is inserted. If < errno-Body> does not expect a parameter, the parameter must be
transferred nevertheless. If a numeric parameter is expected the output is false because a char is
expected.

Example:

Currently, this call is used for the binfile activation with messageID 84.

alcib -meldnum_ext 84 99990 37338 37339 <progname.build>




4.2. Overview
There are 7 groups with the following subject texts:
Group:
    1.  Sales/Purchasing
    2.  Stock
    3.  PMS
    4.  EDI Messages that are sent in the course of internal or external EDI or the master data
        replication are documented in the "Messages" section in the separate configuration
        documentation "EN-CONFIG A+W Enterprise EDI".
    5. System
    6. Shipping
    7. Barcode
    8. Racks
    9. AWCapacity
    10. Print


Meldid     Group Reference Reference text
                  number
   1          1       30894      Stock withdrawal box



A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                             33
  2       1     30895   Defective order
  3       1     30896   Project bookings (NIU)
  4       1     30897   Booking through return server
  5       1     30899   Resubmission
  6       1     30906   Glazing order
  7       1     30907   Delivery note cancellation
  8       1     30908   Wrong supplier number (NIU)
  10      4     30964   Order entry (EN-CONFIG-A+W Enterprise EDI.pdf)
  15      4     31016   Order exit (EN-CONFIG-A+W Enterprise EDI.pdf)
  18      4     31017   Order transfer, announcement (EN-CONFIG-A+W Enterprise
                        EDI.pdf)
  19      4     31018   Order transfer, send request (EN-CONFIG-A+W Enterprise
                        EDI.pdf)
  20      4     31019   Purchase order completed (EN-CONFIG-A+W Enterprise
                        EDI.pdf)
  21      4     31020   Quotation received and booked (EN-CONFIG-A+W Enterprise
                        EDI.pdf)
  22      4     31021   Article transfer failed
  23      4     31277   Transferred article
  24      2     31082   Modification of delivery date
  25      2     31084   Incorrect booking of withdrawal of goods
  26      2     31085   Booking error
  27      2     31087   Incorrect booking of receipt of goods
  28      2     31088   Negative stock on hand
  29      2     31089   System message of stock booker
  30      1     31125   Order created according to quotation (NIU)
  31      5     31218   Background processes (EN-CONFIG-A+W Enterprise EDI.pdf)
  32      1     31257   Correction not to production
  33      3     31309   Change PO date
  34      3     31310   Postponement of delivery date
  35      3     31311   Work planning
  38      3     31312   Capacity planning
  41      1     31553   Change PO date in the delivery notice or PO management
  43      3     31777   A product reported broken includes purchased parts



A+W Software GmbH       EN-CONFIG-A+W Enterprise System.docx                      34
   45        3       32103       Data transfer OrderXML to production
   70        6       31311       Postponement
   72        6       34578       Delivery note was not generated
   73        9       34774    Scheduling or rescheduling failed
   76        9       35513       A+W Production: Scheduling failed
   80        1       36520       Production information without scheduling
   84        5       37338       Binary activation
   85        4       37713       Article transfer successful
   86        4       37714       Market partner transfer successful
   87        4       37715       Key transfer successful
   91        4       37977       Invoice control failed
   92        4       37978       Invoice control successful
   93        2       38060       Stock shortfall overview (AWP import)
   94        1       38101       Change of the part number despite order
   95        4       38299       Internal EDI: goods receipt postponement




4.3. System message 1
Action:
Changes for "stock withdrawal (order-related)"
Thus, intaufart 16 "BOX UPDATE" is executed
The message is only sent if the environment variables KISTENAEND_MELDMANR and
NEUE_KISTENLOGIK are active.
Subject: Textnr 30894– "Stock withdrawal box"
Message text: 30535 : "<date> <time> Order: <order> Item: <item> stock withdrawal."
Depending on the case, the following information is also provided
30533 : "Box supplier changed"
30531 : "Box quantity changed"
30532 : "Number of sheets changed"
30534 : "Packaging type changed"


Initiator: environment variable KISTENAEND_MELDMANR
Recipient: Configuration via Ctrl+F4 – Mail system - System messages



A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                 35
4.4. System message 2
This message is sent by various actions. In particular if the background process "intauf"
determines problems with the order processing.
Action 1:
Discount recalculation (see also "DE-CONFIG-A+W Enterprise" section "Recalculating discounts")
For the three Intauf types (-26,-28,-37), a check for data consistency is built in, which checks the
following aspects:
        kauf.gesnetto - <total kaufrab.betrag> = kauf.nettototal
        kauf.nettototal + kauf.mwstbetrag = kauf.gesbrutto
        kaufrab.grundwert * kaufrab.wert = +/- kaufrab.betrag (/100 for KLEINE_RABATTWERTE)
If this check fails, the A+W Enterprise - system report id= 2 will be dispatched; the case will be
locked
Subject: Text no. 29149 – "Check error - incorrect order total"
Message text: Fix
Updating surcharges of case <kauf.auftrnr>-<kauf.vorgang>-<kauf.subnr> failed. Data is
inconsistent. Case is locked. Please call A+W support."
Initiator: Document user – kauf.eusr
Recipient: Configuration via Ctrl+F4 – Mail system - System messages




4.5. System message 4
Action: Saving of an order with a project assignment
Only if a glazing employee is defined in the project (master data - market partners - "Order" tab)
Subject: Text no. 30897 : "Booking through return server"
Message text: Text no. 29498 : "Failed booking attempt Rserver, booking type: <booking>, Order
no: <order>"
Initiator: environment variable RSERV_MELD_EMPF
Recipient: Configuration via Ctrl+F4 – Mail system - System messages


4.6. System message 5
Action: start A+W Enterprise if a transaction was entered in the resubmission
Subject: 30899 : "Resubmission"
Message text: 22134 : "Resubmission:“ + <transaction> <orderno>-<subno> + 22135 : "Stored by"
<employee> + <Text1> + <Text2>
Initiator: employee who was entered in the resubmission



A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                   36
Recipient: Configuration via Ctrl+F4 – Mail system - System messages


4.7. System message 6
Action: Saving of an order with a project assignment
Only if a glazing employee is defined in the project (master data - market partners - "Order" tab)
Subject: Text no. 30906 : "Glazing order"
Message text: Text no. 20014 : "The glazing order <order> was entered or changed."
Initiator: Glazing employee from the project master data (master data – market partner – "Order"
tab)
Recipient: Configuration via Ctrl+F4 – Mail system - System messages




4.8. System message 7
Action(1): Cancellation of a delivery note if the environment variable LAGER_STORNOMELD is
active
Subject: Text no. 30907 : "Delivery note cancellation"
Initiator: Employee from the variable LAGER_STORNOMELD
Recipient: Configuration via Ctrl+F4 – Mail system - System messages
Message text: 22056 : "The following delivery note was cancelled: <Deliverynote> - <Part>"


Action (2): If the delivery note in the background is cancelled (AUTO_LS)
Subject: Text no. 30907 : "Delivery note cancellation"
Initiator: None
Recipient: Configuration via Ctrl+F4 – Mail system - System messages
Message text: 34842 : "<Order>->part>: All other delivery notes for this delivery are already
invoiced. Delivery surcharge <Text> is lost."




4.9. System message 22
This message is sent by various actions.
Action(1): This system message is sent in case of errors in article replication.
Subject: Text no. 31021 – "Article transfer failed"
Initiator: None
Recipient: Configuration via Ctrl+F4 – Mail system - System messages
Message text:


A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                37
Text no. 30494 - "Caution, the transfer of the article master data to client <Site> failed! (SC=<SQL-
error code>)"
Or
Text no. 33417 – "Processing types from the 'article dimensioning' were not replicated."
Or
Text no. 33416 – "Article types from the 'article dimensioning' were not replicated."
Or
Text no. 33415 – "Article types from the 'mandatory dimensions' were not replicated."
Or
Text no. 33412 : "The following articles were not replicated: <List of article numbers>"
The individual texts can be changed and added to in the course of function expansion in order to
provide the recipient with a more precise indication of the problems with article replication.


Action(2): Data consistency check in the client during the article or market partner replication
Subject: Text no. 27005 : "Local article master data"
Initiator: None
Recipient: Configuration via Ctrl+F4 – Mail system - System messages
Message text: The individual texts will be changed and added to in the course of function
expansion in order to provide the recipient with a more precise indication of the problems with
article replication.


4.10.             System message 28
Action: The message is sent if the stock booker determines a negative stock.
Subject: Text no. 31088: " Negative stock on hand"
Initiator: None
Recipient: Configuration via Ctrl+F4 – Mail system – System messages and environment variable
WL_MELD_EMPF. If the variable is not set, then the message goes to the user of the stock booking
that triggers the negative stock on hand.
Message text:
21790 : "Attention negative stock <Bestand> (article <Artikelnummer> stock <Lagernummer>
variant <Variantenbezeichnung> color <Farbbezeichnung>)"




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                38
4.11.           System message 32
The message is not sent if the environment variable "MODUL_PROD_SPAETE_AENDERUNGEN" is
active.
Action: saving of an order/processing of a released order by intauf
Subject: Text no. 31257 : "Correction not to production"
Initiator: user (kauf.eusr)
Recipient: Configuration via Ctrl+F4 – Mail system - System messages
Message text:
31256 : "A PO was just generated for the order <Order>. The changes could not be forwarded to
production."


4.12.           System message 33
This message is send via the alrpc service from the ERPWebservice (no call in the AWE back end).
This message is sent by various actions.
Action(1): Changed PO date in case of rescheduling
Subject: Text no. 31309 : "Change PO date"
Initiator: user of the order (kauf.eusr)
Recipient: Configuration via Ctrl+F4 – Mail system - System messages
Message text:
Text no. 36440 : "Rescheduled PO date for order <kauf.auftrnr>, item <kpos.lfdpo>, part <Artikel>
can no longer be taken over (old date <Date>, new date <Date>).


Action(2): Invalid PO date
Subject: Text no. 31309 : "Change PO date"
Initiator: user (kauf.eusr)
Recipient: Configuration via Ctrl+F4 – Mail system - System messages
Message text:
"For order <kauf.auftrnr> item <kpos.lfdpos> and part <article>, the PO date <newDate> was
determined due to supplier handling times our route days. This date is not a valid PO date."




4.13.           System message 41
This message is sent if the delivery date of the order was moved so far back that the delivery date
of the corresponding order also had to be moved.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                              39
Action: change of the planned goods receipt date in the dispatch notice (purchasing - dispatch
notice) or the PO management (purchasing - PO management)
Subject: Text no. 31553 : "Change of delivery date in the dispatch notice"
Initiator: environment variable AVISE_MAIL
Recipient: Configuration via Ctrl+F4 – Mail system
Message text:
Text no. "31554: "The delivery date of the order <ordernr> must be changed!"
Starting with QR 23/10:
Text no. 38324: "The goods receipt date of the PO <PO number> has been postponed, therefore
the delivery date of the order <Ordernumber> must be postponed!"


Both the sending as well as the message text can be overridden by the stored procedure
"cumailsp41()". See also "EN-CONFIG-A+W Enterprise" section "Dispatch notification".




4.14.           System message 43
This message is send via the alrpc service from the ERPWebservice (no call in the AWE back end)
Action: A purchased part was defined as needing reorder by the breakage handling
Subject: Text no. 31777 : "A product reported broken includes purchased parts"
Initiator: environment variable AWC_NACHBEST_MANR
Recipient: Configuration via Ctrl+F4 – Mail system
Message text:
Text no. 36134 : "The following parts have to be reordered (order, item, article: pieces): <Order,
item, article, pieces)"


4.15.           System message 45
To dispatch an email telling the user that the OrderXML file could not be created, please enable
the following switches in ALCIB:
ORDERXML_MESSAGEMANR: Define a user number to be treated as the initiator of the message.
The message will be sent to this user or to several users defined in the email system for report
number 45 (group PMS).
AWC_ALCIB_SERVER_NAME: The ALRPC background process in ALCIB is ordered to dispatch the
message. To address it, enter the name of the server on which the ALRPC process is run.
AWC_PORT_CONTROL_SERVER: The ALRPC background process in ALCIB is ordered to dispatch
the message. If the process does not work, the CTRL_SERVER must start it. This is why this switch
needs the socket port number of CTRL_SERVER. It can be found in the "services" file of the ALCIB
server.



A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                 40
AWC_PORT_RPC_DIENST: The ALRPC background process in ALCIB is ordered to dispatch this
message. To address it, this switch needs the socket port number of ALRPC. It can be found in the
"services" file of the ALCIB server.
Action: Error when creating the OrderXML file
Subject: 32103 : "File transfer OrderXML to production"
Initiator: environment variable ORDERXML_MESSAGEMANR
Recipient: Configuration via Ctrl+F4 – Mail system
Message text:
[Order|Quotation] <Documentnumber>: The transfer to an external program
failed! (OrderXML Error <Errornumber>)



4.16.           System message 70
If the environment variable SYSMELD70_NO_VK_LAPOOL is active, then the system message 70
will only be issued in case of delivery date shifts from production and PU records in dispatch. In
case of shifts of SA records in dispatch, there is no more message; instead, the logic from #459447
is used.
Action: In case of shift in dispatch
Subject: 33911: "Postponement" (e-mail subject line)
QR2406: With the environment variables EMAIL_DELIVDATE_SHIFT_SUBJECT_PLUS = ON, it is
possible to achieve that subject already receives an order number and customer name.
Initiator: A + W / System Service
Recipient: Person or dispatch employee who causes the shift.
Message text:
(Example) Dispatch: Order 5001926 from Customer 1 will be postponed from 11/30/2020 to
12/01/2020.
Dispatch info Moving a route: Backlog




4.17.           System message 72
Action: Delivery note was generated automatically (AUTOLS) (not manually via dialogs in dispatch
or sales). (see „EN-CONFIG-A+W Enterprise“ – section „Automatic delivery note generation”)
If this environment variable AUTOLS_MANR is not active and is not equal to 0, the message will
not be sent.
Subject: Text no. 34578 : "Delivery note was not generated"
Initiator: environment variable AUTOLS_MANR.
Recipient: Configuration via Ctrl+F4 – Mail system
Message text:

A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                             41
Text no. 30960 : "The order <Order number> was not found in the database."
Or
Text no. 34580 : "Order <Order number> already has a delivery note"
Or
Text no. 35870 : "For order <Order number> no DN could be generated since the arrival date is
before the date of the last period end."
Or
Text no. 34581 : "Order <Order number> is not yet packed."
Or
Text no. 34582 : "Order <Order number> is still locked by the background process intauf or rserv"
Or
Text no. 34583 : "Order <Order number> is not complete and cannot be booked to transport"
Or
Text no. 34585 : "Order <Order number>: No data found"
or
Text no. 34584 : "Order <Order number> is only on transport. Additional booking was not
possible."
Or
Text no. 22817 : "Delivery note <Order number> cannot be generated"
The individual texts are changed and added to in the course of function expansion in order to
provide the recipient with a more precise indication of the problems with delivery note creation.




4.18.           System message 73
This message is send via the alrpc service from the ERPWebservice (no call in the AWE back end)
Action: An order/an item with a purchased part should be scheduled anew or rescheduled. Here,
there are conflicts for the order generation
Subject: Text no. 34774: "Scheduling or rescheduling failed"
Initiator: user of the order (kauf.eusr)
Recipient: Configuration via Ctrl+F4 – Mail system
Message text:
Text no. 34776 : "Automatically generated PO <PO number> was released and has to be canceled
before new scheduling of the order <Order> - item <kpos.lfdpos>."
or
Text no. 34777 : "A PO item was already generated from the PO proposal for order <Order>, item
<kpos.posnr>, tuple <aufstrukt.tnr>. It has to be canceled before new scheduling."



A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                               42
4.19.             System message 74
Action:
Subject: Text no.
Initiator:
Recipient: Configuration via Ctrl+F4 – Mail system
Message text:
Environment variable
Released with Quality Release (2024/06))
EMAIL_DELIVDATE_SHIFT_SUBJECT_PLUS = ON (client reference: no)
If this environment variable is active, the order number and customer name are written in the
subject of the mail about delivery date postponement (ID 34,70, and 74).


4.20.             System message 76
Action: Order was scheduled incorrectly. The status 550 is booked. If the order was only
transferred to AWP for cost calculation, this message does not appear.
Subject: Text no. 35513 : "A+W Production: Scheduling failed"
Initiator: user of the order (kauf.eusr) / employee who made the last change (kaufedit.manr)
             (see environment variable AWC_NEU_LTPLAN_LASTMANR_MAIL)
Recipient: Configuration via Ctrl+F4 – Mail system
Message text:
If the scheduling affects a specific item
Text no. 36274 : "The item <kpos.lfdpos> of the order <kauf.auftrnr> could not be scheduled in
the production system. Error message from the production system: <Text from AWP>"
If it affects the whole order
35515 : "The order <kauf.auftrnr> could not be scheduled in the production system. Error
message from the production system: <Text from AWP>"
Environment variable
alcib - 13.04.12006 ((Released with Quality Release (2022/02))
AWC_NEU_LTPLAN_LASTMANR_MAIL
If this environment variable is active, then message are sent as initiator to the employee who last
changed the order and not to the user.


4.21.             System message 80
“EN-CONFIG-A+W Enterprise” section “Late change”
Action: Change and enabling of an order with production-relevant changes


A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                             43
Subject: Text no. 36520 : "Production information without scheduling"
Initiator: The employee who makes the order change (akt.manr)
Recipient: Configuration via Ctrl+F4 – Mail system
Message text:
Textnr: 36521 : "In the order <Order number> production-relevant information was changed.
Production documents should be checked."
Or
Text no. 36522 : "In individual items in the order <Order number>, production-relevant
information was changed. Production documents should be checked."
Dependent environment variable: MODUL_SPAETE_AENDERUNGEN


4.22.             System message 84
Action: Activation of a binary via menu item System > Activation / Release > Binary Activation
The message is sent from the activate_binary script.
Subject: Text no. 37338 : "Binary activation"
Initiator: Employee who triggered the bin activation in the tool.
Recipient: Will be assigned on the system menu
Message text:
Text no: 37339 : "The activation for binary <binaryname> was successful."
Or
Text no. 37340: "The activation for binary <binaryname> was not successful."


4.23.             System message 90
Action: Delivery note creation (Dispatch?) (main AWD: #459447)
Subject: Text no.
Initiator: none
Recipient:
Message text:
Expansion of the system message 90 with the AzureDev #31167:
Shift note (lapproto.aend_txt)
First and last name of the employee who made the shift.
SP:     laMGetMovedOrders.sql (/develop/globusr/rschepp)


4.24.             System message 91
Action: The import of the invoice transfer file failed

A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                            44
Subject: Text no. 37977 : "Invoice control failed"
Initiator: none
Recipient: Configuration via Ctrl+F4 – Mail system
Message text: the status information will be displayed depending on the flow of the process


4.25.             System message 92
Action: The import of the invoice transfer file was ended successfully and the transactions were
transferred to the booking process
Subject: Text no. 37978 : "Invoice control successful"
Initiator: none
Recipient: Configuration via Ctrl+F4 – Mail system
Message text: the status information will be displayed depending on the flow of the process


4.26.             System message 93
Ticket: [AW-72192] QR11 / 2021 – ERP-Webservice – “DE-CONFIG-A+W
EnterpriseProductionInterface” section “Stock forecast”
Action: scheduling of an order released for production in A+W Production
Subject: Text no. 38059: "Stock goods for order <Auftrag> not available – scheduling failed"
Initiator: none
Recipient: Configuration via Ctrl+F4 – Mail system
Message text: tabular listing of the articles that were determined for a stock shortfall
Product Variant      Color/size       Stock   Date       Predicted        Required    Quantity unit
                                                         quantity         quantity


    •   Article: article number - name
    •   Variant: Variant number – name
    •   Color/size: Color/size variant number -- name
    •   Stock: Stock number – name (standard stock)
    •   Date: Production start date
    •   Predicted quantity: Predicted stock on the specified date
    •   Required quantity: total quantity of the article required for this order (necessary
        quantity on this day if the article is required for the final product on different days). See
        "EN-CONFIG-A+W EnterpriseProductionInterface" section "Stock forecast"
    •   Quantity unit: Quantity unit for the article


    Dependent environment variable: AWC_CHECK_STOCK

A+W Software GmbH                 EN-CONFIG-A+W Enterprise System.docx                                  45
4.27.           System message 94
[AW-73052] e-mail notification in case of tuple change for glass ordered (Azure 60706)
alcib - 13.04.12470
Action: Change in the BOM for masking (configured module) despite warning.
Subject: Text no. 38101: "Change in the part number despite order"
Initiator: System service
Recipient: Person who made the change or CHECK_UTEIL_BEST_MELDMANR
Message text:
38102: "In the order %ld (Pos.%d), the numbering of the BOM was changed. Reference to existing
POs of production no longer applies"
38103: "In order %ld (Stückliste %d), the numbering of the BOM parts was changed. Reference to
existing POs of production no longer applies"
 If the appropriate modification check was activated, then when leaving the BOM there is a check
of element-ordered items whether due to the BOM change, the numbering of the BOM elements
has changed. Such a change ensures that through the later reporting from A+W Production, the
relationship between order and PO can no longer be determined. The consequences of the
change are reported to the user. However, this does not result in a cancellation of the order
change. If the user has authorized this change despite the warning, then now a system message
(ID=94) is sent to the responsible employee, who can be specified via a separate ENV switch. If the
responsible employee is not specified, the message goes to the user.
Since the information with regard to a shift of an ordered element of the BOM is only available at
the time of the change, the notification is also sent immediately after a change despite the
warning. If the changes of the document are discarded completely after the fact, the notification
cannot be taken back.




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                              46
5. Control server (ctrl_server)
The control server monitors and controls other background processes. Therefore, it is no longer
required for all background processes (e.g. intauf, rserv) to be permanently active, even if there is
nothing to do. This spares the computing resources. The control server writes its own Log to
$PROTOPFAD/c<Computer name>DDMM.
The CTRL server checks cyclically every 5 minutes whether the MaxBusyTime (ctrl_serv.par) of a
process is exceeded, that is, whether the time that has elapsed since the last report via X0W is
greater than the MaxBusyTime. In this case, a System message is sent via the call 'alcib meldnum
<manr> <meldid aus ctrl_serv.par>‘. This is logged accordingly in the ALMailYYMMDD log.


5.1. Control (ctrl_serv.par)
The ctrl server reads in the file $ALDATPFAD/ctrl_serv.par and using the data stored there, the ctrl
server decides what should be done.
The CTRL server checks cyclically every 5 minutes whether the MaxBusyTime of a process is
exceeded, that is, whether the time that has elapsed since the last report via *0W is greater than
the MaxBusyTime. In this case, a system message is sent via the call 'alcib meldnum <manr>
<meldid aus ctrl_serv.par>‘. This is logged accordingly in the ALMailYYMMDD log.
If the Ctrl_server determines that processes are hanging, it can be controlled via the variable
RESTART_IN_SERVERCHECK whether the CTRL-Server should try in this case to restart the
background process.
The file ctrl_serv.par is in the directory ga (ga- is a shortcut) and has the following structure:




                                                                                                                                                                                        monitoring_o
                                                                                                                                                                        restart_delay
                                                                                              starttime_hh




                                                                                                                           max_busy_ti
                                                                                                             starttime_m

                                                                                                             max_idle_ti




                                                                                                                                         meldmanr
                                                                        hostname




                                                                                                                                                    meldnum
                                 busykey
            startkey

                       stopkey
module




                                                                                   startscr
                                           endkey

                                                    exitkey

                                                              service




                                                                                                                                                              logfile
                                                                                                             me

                                                                                                                           me




                                                                                                                                                                                        nly
                                                                                                             m




Stock       L0B        L0S       L0W       L0E      L0X       lager     asteraix   wlager                         600      900           116        22022     wlh.log   0               00
booker                                                                             wlh


Example of a complete file:
Lagerbucher ^L0B^L0S^L0W^L0E^L0X^lager^asteraix^wlager wlh^600^900^116^22022^18:00^wlh.log^0^0^
Rueckmeldeserver^R0B^R0S^R0W^R0E^R0X^rserver^asteraix^rserv^60^900^116^22021^^rserv.log^0^0^
Intauf0    ^I0B^I0S^I0W^I0E^I0X^intauf_A^asteraix^intaufscr intauf 0^18000^900^116^22018^^intauf.log^0^0^
Intauf1    ^I1B^I1S^I1W^I1E^I1X^intauf_B^asteraix^intaufscr intauf 1^360^900^116^22018^^intauf1.log^0^0^
Intauf2    ^I2B^I2S^I2W^I2E^I2X^intauf_C^asteraix^intaufscr intauf 2^360^900^116^22018^^intauf2.log^0^0^
Intauf3    ^I3B^I3S^I3W^I3E^I3X^intauf_D^asteraix^intaufscr intauf 3^360^900^116^22018^^intauf3.log^0^0^
Intauf5    ^I5B^I5S^I5W^I5E^I5X^intauf_E^asteraix^intaufscr intauf 5^360^900^116^22018^^intauf5.log^0^0^
Intauf6    ^I6B^I6S^I6W^I6E^I6X^intauf_F^asteraix^intaufscr intauf 6^360^900^116^22018^^intauf6.log^0^0^
Intauf7    ^I7B^I7S^I7W^I7E^I7X^intauf_G^asteraix^intaufscr intauf 7^360^900^116^22018^^intauf7.log^0^0^
Intauf8    ^I8B^I8S^I8W^I8E^I8X^intauf_H^asteraix^intaufscr intauf 8^360^900^116^22018^^intauf8.log^0^0^
Intauf9    ^I9B^I9S^I9W^I9E^I9X^intauf_I^asteraix^intaufscr intauf 9^360^900^116^22018^^intauf9.log^0^0^
Intauf10    ^IAB^IAS^IAW^IAE^IAX^intauf_J^asteraix^intaufscr intauf 10^360^900^116^22018^^intauf10.log^0^0^
Repspool     ^D0B^D0S^D0W^D0E^D0X^repspool^asteraix^repspool^360^900^116^22020^^repspool.log^0^0^
Fibubucher ^F0B^F0S^F0W^F0E^F0X^fserv^asteraix^fserv^900^900^116^29801^^fserv.log^0^0^
RPC-Server ^C0B^C0S^C0W^C0E^C0X^alrpc^asteraix^alrpc^360^900^2028^34802^^alrpc.log^0^1^
PMS       ^P0B^P0S^P0W^P0E^P0X^pms^qm-x6^pms -pmp^360^900^99999^22019^^pmp0.log^120^0^




A+W Software GmbH                                   EN-CONFIG-A+W Enterprise System.docx                                                                                47
5.1.1. Monitoring
In the following table, you can see using the example of the stock booker how the fields idle and
busy time and the status are assigned. The description assumes that at the time of the CTRL
server start, the stock booker is not running.


Action                        Process                    Status      Idle time       Busy time
CTRL server start             CTRL server                STOPPED                 0              0
L0B -> Start stock booker     ALCIB-VG                   STARTING    n.a.            n.a.
L0W                           Stock booker               RUNNING     n.a.            ACT TIME
L0S                           Stock booker               WAITING     ACT TIME        n.a.
L0W                           Stock booker               RUNNING     n.a.            ACT TIME
L0S                           Stock booker               WAITING     ACT TIME        n.a.
L0E                           sctrl / CTRL server
                              internal                   STOPPING                0 n.a.


ALCIB-VG                      ALCIB foreground process or other background
                              process
Act time                      Current Unix time
n.a.                          no adjustment


The evaluation of these entries in the monitoring routine happens as follows:

1. For each background process, the following values are output:

          a. Process name

          b. Idle time = current Unix time - idle time

          c. Max-Idle-Time (ctrl_serv.par)

          d. Busy time = current Unix time – Busy-Time

          e. Max-Busy-Time (ctrl_serv.par)

2. For background processes with status RUNNING, STARTING, RESTARTED it is checked
   whether the process still exists; otherwise, the STATUS TERMINATED is assigned and there
   is an attempt to restart the process.

3. Checking the idle time
   For processes with status WAITING, the idle time is deducted from the current Unix time
   and compared to the value in MAX-Idle-Time (ctrl_serv.par). If the result is greater than
   the MAX-Idle-Time, the server is ended.
4. Checking the busy time
       For processes with status RUNNING and RESTARTED, the busy time is deducted

A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                               48
    from the current Unix time and compared to the value in MAX-Busy-Time
    (ctrl_serv.par). If the result is greater than the MAX-Busy Time, the message
    "booker is stopped" will be output and a mail sent to the employee stored in the
    ctrl_serv.par.
    Via the variable RESTART_IN_SERVERCHECK it is possible to control whether the CTRL-
    Server should try in this case to restart the background process.



5.1.2. System messages from the ctrl_serv.par
Re (31218): Background processes (ID 31); stand in $ALDATPFAD/ctrl_serv.par
Meldnum                           Text                               Log/module
900                               Trigger booking                    rserv.log
22021                             The return server is stopped!      rserv.log
22018                             Background order completing is     Intauf 0
                                  stopped!
22020                             The printer spooler is stopped!    repspool
22022                             The stock booker is stopped!       Stock booker
29801                             The FinAc server is stopped!       FinAc booker


The following rules apply (status as of: 1/28/2021):
If the client does not work with PMS, the PMS processes have to be removed from the
ctrl_serv.par.
An entry for alrpc has to have a 1 as the last parameter


5.1.3. Starting the ctrl_server
In the standard, the ctrl_server is started via the start routine together with all background
processes. If a manual start should be required, this can be done under UNIX in the A+W
Enterprise environment with the script "ctrlservstart". With internal client separation, this script
starts all relevant ctrl_server if necessary.
#347504: should it be required in rare cases to start the ctrl_server via the front end. This can be
the case, for example, if the A+W Enterprise environment is not required, however reports from
production are required. For this case, the script has to be attached to the individual programs.
In the path $ALCIBPRG/cmd lies the script "ctrlservstart", which has to be executed to start the
Ctrl server and thus also the alrpc service.
The script ctrlservstart has to be linked once with a symbolic link in the directory
$ALCIBPRG/spec/prg.
For this, this command has to be executed:
ln -s $ALCIBPRG/cmd/ctrlservstart $ALCIBPRG/spec/prg/prgctrlservstart


After that, the Ctrl server can be started via A+W Enterprise in the individual programs.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                   49
5.2. Error research
5.2.1. A background process is not started
A background process is not started and there is no appropriate start request in the CTRL server
log.
The variable NO_CTRL_REQUEST_FILTER may be helpful here. If this variable is not set, requests
that were sent by a process are forwarded only every 2 seconds, insofar as the same background
process should be started.
It should be set if in the CTRL server log no start request for starting a background process is
found and no error message occurs in the logs connect.prot and bgctrl for the time in question.


5.2.2. Background processes run in an endless loop
The affected background processes can no longer be contacted by the CTRL server.
A so-called backport can be opened for each socket communication. These backports are assigned
from a particular number range by the operating system. If this number range overlaps with the
port number range in which the A+W ports lie, the communication between CTRL server and a
background process can be interrupted. This is evident in that a background process that waits for
a new order from the CTRL server cannot wait for an incoming socket, but keeps right on working,
that is, runs in an endless loop. In the file bgctrl, the following entries will be found. Important for
the log analysis is that you look at the entry before the first message with errno 22 or search after
"errno = 98" in this file. Starting with Version 12.1, there is a script called errno, which outputs a
plain text for the errno codes. Please execute the script on the appropriate operating system AIX
or Linux.
      S: New SERVICE:repspool381
      S: 05.10 14:38:56 Error in bind() (errno = 98)
      05.10 14:38:56 Error in startup_server service=repspool381 haus='381'
      errno 98
      EADDRINUSE        98 /* Address already in use */
Solution
Adjustment of the ephemeral port:
S30_set_kernel_pars has to be entered in ALCIBPRG/spec/rc/<Rechnername> for this. After that,
the computer has to be rebooted. A manual starting of this script is not sufficient since in this case
there could still be processes that are already occupying an A+W port number.
In case of doubt, you can check using the command "/sbin/sysctl -n
net.ipv4.ip_local_port_range" whether the port numbers are set correctly. The second value
should be 41999 here.


5.2.3. What does the error 111 in the bgctrl log mean
The error (errno) 111 means connection refused, that is, no connection to the appropriate
background process could be established. This can be normal since on start, the CTRL server tries

A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                 50
to reach all dependent processes. If such a process is not active, this error appears in the log.
When running through the monitoring routine in the CTRL server, this situation may also arise. In
both cases, the error is not critical. In case of a problem, you have to look at the CTRL server log to
see which action the CTRL server has just executed.


5.2.4. ctrl_server cannot be stopped with exit_servers
The background processes are stopped with exit_servers. It can happen that exit_servers do not
stop the ctrl_server. The cause of this is usually that there is an incorrect PID in
$IPCDIR/ctrl<server>.log. The incorrect PID hapens if in xhaus there is an entry with
"hauptmandant" = <$HAUS> for which no ctrl_server is to be started. This can be a pseudo client
for suborders, for example (IBHAUS). However, in the hauptmandant field, there must be a 0.


5.3. Environment variables
BGCTRL_PROTO (Client reference: No)
Variable for switching on the expanded logging of the connection establishment to the CTRL
server
NO_CTRL_REQUEST_FILTER (Client reference: No)
This variable causes every request to be forwarded to the CTRL server to start a background
process. If this variable is not active, the triggering of the same background process (e.g. rserv) is
only forwarded to the CTRL server every two seconds. This should reduce the volume of requests
to the CTRL server. However, it can occasionally lead to records being left in front of the
corresponding background process if the job is processed faster than in 2 seconds.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                    51
6. watchdog
The 'watchdog' is actually no longer deployed/activated since the invention of the 'ctrl_server'.
And that was decades ago.
If I remember correctly, then there must be an entry in the startpar file so that the watchdog
starts up. However, this hasn't been inserted in a long time.
And even then, the current versions of the script '$ALCIBPRG/etc/alcib_startbg' do not react at all
if the watchdog is in the startpar file.
This can only mean that someone has started the process by hand (on the shell). Is there a
$ALDATPFAD/watchdog.par file there?




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                52
7. Number server
7.1. What do the IDs in the NR server log mean?
     From the 4th column of the nr_servDDMM log, you can see whether a query was
     sent to the number server or the number server has sent back its response. For the
     queries, the following IDs exist:
      •   NR_REQUEST        1
          o This is a query for the assignment of a number from a number range.
            The range can be seen in the last column of the nr_servDDMM log.
      •   NR_LOCK       2
          o This is a query to lock a number in a particular number range.
      •   NR_UNLOCK         3
          o A locked number is released again with this ID. The number is noted in
            the nr column.
      •   NR_STORNO         4
          o With this ID, a number assigned can be put back in the number pool.
            That is, it is assigned again with the next inquiry.
      •   NR_SERVEROFF 5
          o Will not be used. Can end the number server.
      •   NR_STATUS         6
          o Causes the number server to write a log according to $IPCDIR/nr_locks.
            This ID can be triggered via the menu element ALCIB > System > Number
            status.
   The following responses can be sent back by the number server:
      •   NR_OK        -101
          o       The operation (query ID) could be executed without errors.
      •   NR_LOCKED         -102
          o The number could not be locked since it was already locked by another
            user.
      •   NR_ERROR       -103
          o Incorrect query, e.g. the desired number range does not exist or an
            error occurred when accessing the database.
      •   NR_FATAL      -104


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                      53
            o Severe error, the number server is ended.


7.2. Pre-population of the next number to be
   assigned in a number range
If you want to adjust the next number of a number range to be assigned by the number server so
that it is used on restart, then you enter the number via update in the field neu_nr for the
respective number range and set the Status field to 1. On restart, the number server then takes
over the specified number -1 as the last one assigned. For the first query, the desired number can
then be assigned. The field akt_nr cannot be implemented directly since this field is updated by
the number server for queries with the last number assigned in the memory.


7.3. Adjustment of the limit values of a number range
If only the limits of the number range should be adjusted, this can be done directly via update to
the fields von_nr and bis_nr. For this, the flag status does not have to be set to 1. However, the
changed limits of the number range are only considered after a restart.


7.4. Releasing a locked number
With "alcib -nrexit <numberrange> <number> <manr> <pid>“, for the number range
<numberrange>, the number <number> can be released again without having to restart the
number server.
The information required for this can be found via the menu element ALCIB > System > Determine
i number status. By selecting the appropriate number range and examining the associated
number locks at the end of the output.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                 54
8. ZU_SERVER
8.1. Log $PROTOPFAD/zu_servMMDD
The lines that begin with in contain the inquiries from the client to the zu_server.
Here, the last digit in the log specifies the action:
    •   0 – request a module lock – not exclusive
    •   1 - request a module lock – exclusive
    •   2 – enter a main module (ALCIB, LAGER, LAPOOL)
    •   3 – release module lock again
The module is after the first pipe symbol.


The lines that begin with out contain the response of the zu_server:
    •   -101 – OK, that is, the module lock could be processed.
    •   -102 – No access, another user has locked the module exclusive
    •   -103 – Error in communication with the zu_server – e.g. zu_server not running or cannot
        be reached.
    •   -104 – No more license available – see AWD 84334


in 20.09 08:34:35 |DIBP|1663655675|sw-181643|CON000|rschepp|7077966|116|0|
out 20.09 08:34:35 ||0||||0|0|-101|
…
in 20.09 08:35:31 |DIBP|0|sw-181643|CON000|rschepp|7077966|116|3|
out 20.09 08:35:31 | |0| | | |0|0|-101|




A+W Software GmbH                 EN-CONFIG-A+W Enterprise System.docx                            55
9. Process guard
Problem solution documentation case 219445: Process for monitoring the background processes
Product/module: ALCIB / background processes (development version ALCIB 2012)
To guarantee more system stability for ALCIB 2012, a new background process called
Processguard has been implemented which runs regular checks to find out whether the other
background processes are still working. Should Processguard detect problems in connection with
another process, it tries to enable or restart this process. If the problem cannot be corrected this
way, a system report will be issued so that the system administrator knows straight away that
there is a problem. The following background processes can be monitored:
    •   Number server
    •   Access server
    •   Transfer server
    •   Control server
    •   EDI starter
    •   Background order processing
    •   PMS - order interface
    •   TRM CTRL
    •   Report server
For more information on the functioning and operation, please contact a member of our project
team.
For every process group to be monitored, there has to be an entry in table PROCESSGUARDINFO.
Gültige Valid entries for process groups are NR_SERVER, ZU_SERVER, UE_SERVER, CTRL_SERVER,
DFUE_STARTER, INTAUF, PMS, TRM_CTRL and RSERV. Additionally, a command can be entered in
the database for every process group which Processguard will be use to start processes for this
group if required. If there is no entry, the standard command will be used. Processguard is started
by the script start_processguard, closed by the script exit_servers , and will run just once per
system even in case of internal client splitting.
To incorporate the PROCESSGUARD into the automatic start routine, the line
        start_processguard/3/procguardlock$HAUS
must be entered in the control file
        ${ALCIBPRG}/spec/rc/`uname -n`/startpar.$HAUS
.


The configuration options for monitoring are:
    •   PROCGUARDINTERVAL
    •   PROCGUARD_ROWS_TO_CHECK
    •   PROCGUARDKILLALL


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                   56
    •   PROCGUARDFTEST
    •   PROCGUARDPROTO
For more information, please refer to the documentation on environment variables.
Right after the start, Processguard loads the process groups to be monitored from the database,
and saves them in an internal structure; this is done just once. In case of internal client splitting,
all site numbers of the system will be determined, and saved in an internal structure as well. The
interval in which the processes shall be monitored can be configured. During a monitoring cycle,
all process groups to be monitored will be checked, one after the other. The following groups can
be distinguished:
    •   Processes that exist just once per database (number-, access- and transfer server).
    •   Processes that exist per internal client (control server, EDI starter, TRM-CTRL, and report
        server).
    •   Processes that can exist several times per internal client (background process handling
        and PMS).
Please note that processes that may exist several times for every internal client, will be monitored
together for every client. When all process groups have been checked, Processguard will go to
sleep until the next monitoring session is due.
Follows a short description of how the monitoring of the individual process groups is
implemented.


9.1. Number server
The number server is checked by asking for a new number from the number area
processguard specially defined for Processguard. In case of problems, the process first checks
whether there is a log file for this process in directory IPCDIR . If so, PID will be loaded from this
file. If Processguard is entitled to close the process, it will do just this, and will also delete the log
file. If it is not entitled to do this, the process will check whether there is a process with this PID at
all. If not, the file will be deleted as well. Whenever errors occur during the loading of numbers,
Processguard will try to start the process by means of the defined command. After a break of 5
seconds, the process will ask for another number. If this fails again, system report number 31 will
be issued.
The number range is called "processguard" and already exists. Normally no change is required.


9.2. Access server
The access server is checked by asking for the authorization to access the module Modul TEKU. In
case of problems, the process first checks whether there is a log file for this process in directory
IPCDIR . If so, PID will be loaded from this file. If Processguard is entitled to close the process, it
will do just this, and will also delete the log file. If it is not entitled to do this, the process will
check whether there is a process with this PID at all. If not, the file will be deleted as well.
Whenever the demand for this authorization causes problems, Processguard will try to start the
process by means of the defined command. After a break of 5 seconds, it will ask again for the
access right. If this fails again, system report number 31 will be issued.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise System.docx                                   57
9.3. Transfer server
The transfer server is checked by asking for a package number. In case of problems, the process
first checks whether there is a log file for this process in directory IPCDIR . If so, the process and
the included PID will be closed, and the log file deleted. Processguard then tries to start the
process by means of the defined command. After a break of 5 seconds, it will ask again for a
package number. If this fails again, system report number 31 will be issued.


9.4. Control server
The control server is checked by sending a status request. In case of problems, the process first
checks whether there is a log file for this process in directory IPCDIR . If so, the process and the
included PID will be closed, and the log file deleted. Processguard then tries to start the process
by means of the defined command. After an interval of 5 seconds, the next status request will be
sent. If this fails again, system report number 31 will be issued. This will be done for every internal
client.


9.5. EDI starter
For the EDI starter, the process first checks whether directory IPCDIR includes a log file for the
process. If this is the case, it checks whether there is a process with the PID from the log file. If the
PID exists, the process assumes that EDI starter works as it should. If the PID does not exist, there
are problems with this process and the file is deleted. Under these circumstances and if there is
no file in the first place, Processguard will try to start the process by means of the defined
command. After an interval of 5 seconds, the next status request will be sent. If this fails again,
system report number 31 will be issued. This will be done for every internal client.


9.6. Background process handling
Unlike the other processes, background process handling is not directly addressed by the other
system elements but there is an interface table called AUFINT. For every monitoring session, a
defined number of records will be selected, sorted by input time. Then, the oldest record for
every internal client will be compared with the oldest record from the data pool of the previous
monitoring session. For the first monitoring after the start o the Processguard, the background
process processing can thus not be monitored. If during the comparison it is determined that this
is the record from the previous monitoring, it is assumed that at least one background process
processing of this client is not working properly. In this case, the item quantity (AUFINT.POSANZ)
and the code (AUFINT.STILL) are used to find out which background process handling is
responsible for this entry. The control server will then be asked to terminate these, and restart
them. Unlike the other process groups, the success of this step will not be checked in this interval.
The process just remembers that there has been a problem, and if this problem still exists during
the next process monitoring, system report number 31 will be issued.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                    58
9.7. PMS
This process is monitored by its interface table PMPIN. For every monitoring session, a defined
number of records will be selected, sorted by processing sequence as for background process
handling. Monitoring is done in the same way as for background process handling. In case of
problems, the control server will be asked to close and restart the process.
Defining the processing sequence in PMS is a complex process. This process exists in Processguard
only for PMS as an order interface (PMS 0). This means that if PMS is not used as an order
interface but as a real production system (PMS 1 and PMS 2), Processguard cannot monitor PMS.


9.8. TRM CTRL
This process is monitored by its interface table INTBEST. For every monitoring session, a defined
number of records will be selected, sorted by processing sequence as for background process
handling. Monitoring is done in the same way as for background process handling. In case of
problems, script pmptrmctrlstart will be loaded.


9.9. Report server
This process is monitored by its interface table RSERV. For every monitoring session, a defined
number of records will be selected, sorted by time of input, as for background process handling.
Monitoring is done in the same way as for background process handling. In case of problems, the
control server will be asked to close and restart the process.


9.10.            Environment variables
PROCGUARDFTEST (client reference: no)
With these variables the FTEST can be activated for the process processguard and the log depth
can be set.


PROCGUARDINTERVAL (client reference: no)
By default, the interval between two Process Guard monitoring runs is set to 600 seconds. This
can be adjusted here. Valid values are between 10 and 86400.


PROCGUARDKILLALL (client reference: no)
The Process Guard uses requests or monitoring to determine whether background processes are
still working correctly. If this is not the case, this process is terminated if it is still running and then
restarted. Exceptions are the number server and the access server, since an 'accidental'
termination during live operation has grave effects. Therefore, they are only terminated when this
variable is enabled.


PROCGUARDPROTO (client reference: no)



A+W Software GmbH                 EN-CONFIG-A+W Enterprise System.docx                                    59
A more detailed log can be activated for the Process Guard with this environment variable. The
log is called "procguard<MMTT>" and is located in the log directory.


PROCGUARD_MAX_WAIT_FILES (client reference: no)
(Case #183092): Maximum number of tolerated files in the WAIT directory of the EDI connection.
If this is exceeded, the Processguard sends system message 3. Values between 100 and 20,000 are
permitted. If a value < 100 is specified, a value of 100 is assumed. If a value > 20,000 is entered,
20,000 is assumed. Default is 6000.


PROCGUARD_ROWS_TO_CHECK (client reference: no)
The number of lines that the Process Guard checks when monitoring background processes with
interface table is stored in this variable. Default is 100.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                              60
10. Background process "intauf"
10.1.           Order transfer to A+W Production
10.1.1.         Default with cost calculation and stock forecast
The order is processed after saving in the order entry by the background process intauf (still -
3 or still -22). After that, it is transferred to the production system for calculation of the
machine and personnel costs and with corresponding configuration the stock forecast data.
As long as the order was not yet reported back by the production system, the order remains
locked with still -10. If the production system reports the data to A+W Enterprise, the order
will be processed again by intauf -10. Here, the machine and personnel costs are written
back to the order, new revenues and contribution margins are calculated.
Which parts of the BOM are considered within the material cost calculation is described in
detail in the "Prices" manual.
If the order was not released in the order entry, then it will be placed in the release pool.
With later release, there is another complete scheduling and production cost calculation.
If the order was released in the order entry and it cannot be processed successfully in A+W
Production (status 550 - scheduling error), then the order is NOT placed in the release pool.
In addition, the order is nevertheless available for the planning in the shipping control. The
flow can be changed through the configuration with the environment variables
AWC_POOL_NO_KOSTENKALK or AWC_CHECK_MARGIN.
See also "EN-CONFIG-A+W Enterprise Production Interface"



10.1.2.  No cost and stock forecast                                     if    not       released
    (AWC_POOL_NO_KOSTENKALK)
06.2012 // AWD 223221:
By configuring the ENV switch AWC_POOL_NO_KOSTENKALK = ON you can define that there will
be no separate production cost calculation for orders that were not released; this serves to relieve
the system. All orders that were put in the release pool will be processed by the background
process "intauf" and only placed in the pool with the existing material costs. With this
configuration, no stock forecast data for unreleased orders is generated for the "A+W Enterprise
Clarity Experience - Stock module". See section "Setting the time for the cost calculation and stock
forecast"
They include
    •   manually entered orders that were not released because the user did not have the
        necessary rights
    •   manually entered orders that were not released on purpose after a query
    •   external EDI orders that may not be released because of the configuration or because of
        other criteria


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                               61
    •   internal EDI orders that are not released because of the configuration


The process in A+W Production for the determination of the production costs and labor costs is
not run through at this time. When the orders from the pool are released, the cost will be
calculated in connection with scheduling, and will be written back to the order.


10.1.3.         Setting the time for cost calculation and stock forecast
May 2024
If you are working with the configuration WL_FORECAST_NOT_RELEASED_ORDERS, all unreleased
orders must be transferred to AWP for cost calculation so that stock forecast data for these
orders can be generated. Since this takes a while and also generates a burden in the import, the
system can now perform a transfer to cost calculation downstream via script call. For this, the
orders in question are presented to the background process "intauf" with still -47. It then starts
the transfer to cost calculation and generation of the stock forecast data. During this transfer,
however, the order is locked as during the "normal" transfer.
The script that presents orders to the background process for cost calculation can, e.g. be started
in the evenings outside of the normal order entry via Crontab. It should recognize that there
should be another transfer after order change, however not if the transfer for cost calculation is
done and a change was made on the same day.
An example of a transfer script and the associated stored procedure is available under
$ALCIBPRG/cmd/transfertocc and $ALCIBPRG/install/xsql/cust/ka/cu_transOrder2CC.sql


10.1.4.  Margin  check                           including           production             costs
    (AWC_CHECK_MARGIN)
[AW-126899]
Required program versions
A+W Enterprise 6 Export Service - 13.04.9272
A+W Enterprise 6 OrderXML Service - 13.04.9275
A+W PPS Webservice - 13.6.3676
Albwir.Alcim.Orders4Production.dll - v13.6.4535
Albwir.Alcim.CompleteScheduling.dll - v13.6.4534
Items4Alcim.dll - v13.6.5553
alcib – VNEXT


Environment variables:
AWC_CHECK_MARGIN = ON (not client-specific and not user-specific)
IP_AWC_TESTLAUF = OFF (or disabled) – This variable is out of date and should no longer be used.
A conversion to "AWC_CHECK_MARGIN" is urgently recommended!
ORDERXML_VERSION = "5.7"

A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                              62
AWC_POOL_NO_KOSTENKALK = ON and OFF possible
CHECK_MINUS_DB = 3
CHECK_DB_MANR = <manr>
MIN_DB_WERT=<Wert>
MODUL_KOSTENKALK = 1
The environment variables are evaluated with this function by the background process "intauf"
and may therefore not be set user-specifically,


further requirements
The import O4P must be active in A+W Production.


The goal of this configuration is that only orders with a valid contribution margin are released for
production and these do not have to be scheduled again via the OrderXML service with
immediate release. This should speed up the processing of the orders.
For this, the order is transferred with the type "128" via "ottranszus" to the Order XML service.
Released orders are transferred to A+W Production for cost calculation.
The order remains locked for changes in the foreground until the reporting from A+W Production
has occurred. If the cost calculation in A+W Production could not be executed successfully
("status 550 - scheduling error"), then there can be no release of the order via the export service
to A+W Production. The order lock is lifted. If this is the case, the order will NOT be returned to
the release pool. In addition, the order is nevertheless available for the planning in the shipping
control.
A+W Production calculates the personnel and machine costs for the entire order. There is no
stock forecast and no transfer of the PO data.
The costs are then transferred to A+W Enterprise. The A+W Enterprise background process
"intauf" sums up the production and material costs and calculates the contribution margin from
these.
Then there is a contribution margin check through "intauf" and A+W Enterprise decides whether
the order will actually be released for production. For this, the environment variable
CHECK_MINUS_DB must be activated.
    A) With a positive check, the order is transferred by "intauf" via the table "exportinfo" with
       the new interface type schnittstelle='PRODRELEASE' to the Export service. Thus, the
       Export service calls the new PPS webservice method "PublishTemporaryOrder()" in order
       to release the order in AWP for production.
        Since previously there was no stock forecast and no POs had to be generated, with the
        release via the PPS-WS method, a CompleteScheduling must be called to do this now. This
        is run through without program change including renewed cost calculation and after
        processing, the order is given again to "intauf". "intauf" sums up the costs again and
        unlocks the order.
        The orders released this way line up in the normal processing sequence and are not
        treated with priority.



A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                   63
    B) If the contribution margin check fails, there is no renewed release to A+W Production.
       The order is placed in the release pool in A+W Enterprise. In contrast to the standard
       configuration, the order remains in an internal pool in A+W Production so that the data
       can be accessed later.
        For a later release from the release pool or after an order change, the order is transferred
        again via the OrderXML service to A+W Production with type 128 (because, for example,
        dates must be recalculated).


In case of an order change after release, a new OrderXML transfer is also performed since here,
production-relevant data may have been changed.
If an order was only saved but not released, there is only a transfer for cost calculation (no type
128). Only if the order was released in A+W Enterprise is there a transfer with the new method
described here (type 128).
Within A+W Production, with this configuration the orders are not treated like a pure cost
calculation, but sooner like "reservation orders." This means that the order data is not deleted
after the cost calculation, but instead stored temporarily for renewed transfer.

Order cancellations
Caution: Any order cancellation after "cost calculation + reservation" is always done via the
OrderXML service.
CAUTION: Orders that are transferred with this configuration to A+W Production and NOT
released occupy capacities that cannot be planned for other orders and that may cause order
postponements. A later release can cause changes in delivery dates.


AWE OrderXML Service
If for an order in the table ottranszus in the field ottranszus.typ generally (that is, ottranszus.posnr
= 0 and ottranszus.tnr = 0) the value 128 is stored, the order is provided in the OrderXML file with
the new ID "OrderingTypeType.CostBasedProduction".
See also "EN-CONFIG-A+W Enterprise Production Interface"


AWE Export Service
If an order is marked in the transfer table exportinfo with the new interface type
exportinfo.schnittstelle='PRODRELEASE', the new PPS Webservice method
"PublishTemporaryOrder()" is called by the Export service in order to release the order for
production in AWP.


A+W Production
The order import (Orders4Production) must be active in A+W Production.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                 64
10.1.5.         Environment variables
AWC_CHECK_MARGIN (client reference: no)
Activates the solution that the orders are first transferred to A+W Production for cost calculation
including reservation and if after the cost evaluation of the order should be released, not
transferred again via OrderXML to A+W Production, but via the export service. There is no new
scheduling in A+W Production; instead, the order is only "activated". This way, it can be achieved
that the margin contributions are checked before the release and the order may eventually be
placed in the pool.


AWC_POOL_NO_KOSTENKALK (client reference: no)
If this environment variable is active, orders that were not released for the transfer to production
are also not transferred to production for cost calculation. This reduces the system load, but the
contribution margin consists exclusively of material costs
CHECK_DB_MANR (client reference: no)
The employee number of the employee who is notified is entered in the variable if the order
receives a negative marginal income due to additional production costs.
see “EN-CONFIG-A+W Enterprise”


CHECK_MINUS_DB (client reference: no)




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                  65
The orders that have received a negative contribution margin of MIN_DB_WERT due to
production costs are handled in a special way:
3 - in addition also the orders that are activated for the first time will be saved in the release pool
with corresponding note.
IMPORTANT! If =3, it is assumed that MODUL_KOSTENKALK=1 is active, not 3!
see “EN-CONFIG-A+W Enterprise”


MIN_DB_WERT (client reference: no)
The minimum contribution margin value for the evaluation is defined in the variable if
CHECK_MINUS_DB is active. If CHECK_MINUS_DB is active, but this variable is not, then a minimal
value of 0 is assumed.
see “EN-CONFIG-A+W Enterprise”


MODUL_KOSTENKALK (client reference: no)
This variable switches the production cost calculation on. It is used instead of a purchase price
calculation.
  1 - with PMS or AWP for determination of personnel and machine costs,
see “EN-CONFIG-A+W Enterprise”


ORDERXML_VERSION (client reference: no)
  OrderXML Version




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                 66
11. Shared Memory /Master Data Cache
There are two shared memory segments in A+W Enterprise. One is for the article master
data and one for the BOMs.
The size of these segments will be specified by the environment variables
SHMSIZEARTIKEL and SHMSIZESTRUKT. The segment size in kilobytes is stored in the
variables. In case of a change of the variable value, before loading the shared memory
again, the old shared memory segments must be deleted with the command ipcrm.
The A+W Enterprise shared memory serves to keep the access times to frequently used
articles short.
The most frequently-used article are determined by the program artcnt. A statistic is kept
in the table artstat, in which it is stored how frequently an article was used in a
purchasing or sales document. Based on this statistic, the program marks the articles that
should be loaded into the shared memory by a 1 in the shmflag field of the table Artikel.
With seminit 0 1 the semaphores are initialized; these check whether the shared memory
access is free and lock the access. After that, with shmladen 0 1 as many articles with
shmflag=1 are loaded into the shared memory as fit there. If frequently-used articles are
not in shared memory, you should consider a segment enlargement.
If the storage area for the shared memory article is larger than the space required to
accommodate all articles present in the table aufstrukt, then additional articles (without
particula condition) are marked with shmflag=1. That is, any other articles (e.g. shutdown
ones) are accommodated in the shared memory.
Based on the lower prices for main memory, it is advisable to make the article and BOM
shared memory so large that all articles and BOM elements can be loaded into it.
The 0 next to seminit and shmladen stands for the BOM shared memory and the 1 for the
article shared memory. Only the article shared memory is loaded with shmladen 1 .
Since the loading is shifted automatically to the background, any errors that occur are not
displayed through error messages; however, this can be achieved by setting the
environment variable NODISCONNECT=TRUE.
The command ipcs displays the existing semaphores and shared memory segments.
The A+W Enterprise semaphones and shared memories can be detetected from the
letters "affe" in the basic address. The basic address of the BOM shared memory is
0affe500, of the article shared memory 0affe501 and the semaphores 0affe000 bzw.
0affe001.
The basic address can be changed with the environment variable SHM_OFFSET, e.g., if
shared memories should be created for several clients.
Semaphores and shared memories with changed address are deleted ipcrm –s <Id> and
ipcrm –m <Id>. (With Id, the Id displayed by ipcs is meant.) These commands should be
used with the greatest caution since the deletion of semaphores or shared memories that
do not belong to AWE can have fatal consequences.
With the command shmproto, it is possible to examine the contents of the shared
memory segments. Three files are generated here:


A+W Software GmbH            EN-CONFIG-A+W Enterprise System.docx                        67
          shminfo contains information about both shared memory segments
          shmartikel contains all articles present in the article shared memory
          shmstrukt contains all elements present in the BOM shared memory
With the command shmsingle <artnr> it can be checked whether a particular article is in
the article shared memory. Shmsingle outputs, regardless of whether or not the article is
in the shared memory, the article data; the data is either taken from the shared memory
or database. Only in the last line of the output is it output whether or not the article is in
the shared memory.
Current information in the article shared memory.
If AWE should obtain the article data of an article from the database even though
shmsingle indicates that this article is in the article shared memory, then the article is
probably not in the BOM shared memory. In this case, an expansion of the BOM shared
memory can help.
In order to work without shared memory, the environment variable SHMOUT must be
set. Here it must be noted that only the use of the shared memory of the article master
data can be switched off.
If the variable is set, it is pointed out on program start by a message that you are not
working with the shared memory.
In this case, the program artcnt ends without doing anything with exit code 0.
The program artcnt:
Thanks to a Crontab entry, the program db_tuning is called, which in turn calls artcnt. The
call of artcnt is made with the following parameters:
artcnt faktor1 faktor2 log output [#articles that fit in the article shared memory]
               Via faktor1 and faktor2 it is possible to control how long an article remains
               in the shared memory even though it is not called again.
               This happens using the formula:
               artstatanz = (artstatanz * faktor1 + countartnr * faktor2) / (faktor1 +
               faktor2)
               artstatanz is 0 with first creation of the article and increases with the
               frequency with which the article is used.
               cauntartw is the frequency with which the article occurs in the table
               aufstrukt
               faktor1 and faktor2 are pre-populated with 1 and are generally not
               changed.
               The third parameter controls the log output; if there is a 0 here, no log is
               output, with 1 a log is written.
               Via the last parameter, the number of the articles that fit in the shared
               memory can be passed to the program.
               Starting with Version 2.11, the parameter can be omitted since the system
               determines the right number itself.



A+W Software GmbH             EN-CONFIG-A+W Enterprise System.docx                            68
11.1. Speeding up of access to third-party article
  names
[AW-166920] // alcib - 13.04.16789 / January 2024
Access to third-party article names was speeded up with a cache. It is filled successively
with the names used. When 250 elements have been cached, the least-frequent entries are
overwritten.

This logic is important precisely for multilingual multi-client systems, since here the
names must be determined client- and language-specifically.



11.2.           Configuration
SHMSIZEARTIKEL (client reference: no)
With this variable the size of the article shared memory can be defined. The information is given
in K-bytes. A value of 1024 corresponds to one megabyte. (Default: 512 KB)
ATTENTION: If this value should be changed, then the old shared memory segments for this client
must be deleted with ipcrm before another loading of the shared memory.
Before increasing the size of the shared memory, please check the available main memory under
full load so that the server is not swapped after the increase.


SHMSIZESTRUKT (client reference: no)
With this variable the size of the BOM shared memory can be defined. The information is given in
K-bytes. A value of 1024 corresponds to one megabyte. (Default 512 KB)
ATTENTION: If this value should be changed, then the old shared memory segments for this client
must be deleted with ipcrm before another loading of the shared memory.
Before increasing the size of the shared memory, please check the available main memory under
full load so that the server is not swapped after the increase.


SHMOUT (client reference: no)
If the variable is set, the shared memory is switched off.


SHM_OFFSET (client reference: no)
The variable controls shared memory: If a site is required in SHM = do not set a variable.
Multiple SHMs = each site has an OFFSET value of 1 - 19.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                69
12. Table aweprogversion
The table aweprogversion contains information about the current program statuses saved in the
AWE environment.
All programs with database access, that is Unix binfiles and ICE services, as well as the AWE
Windows services and the ERP Webservice, enter themselves into the table with their current
build information.
Key fields are: produktname , progname , ipadresse , hausnr.
For a product name, there can be several records in the table if there is a difference in the site
assignment (site number) or if access comes from another computer (IP address).
The program name (progname field) is only populated by the AWE Windows services and the ERP
Webservice. For Unix programs, there is a dash ("-") in the field.
The field is necessary because it is theoretically possible for the Windows components that the
same product is installed in different versions on one computer. In practice, this will probably not
happen any longer since only Version 13.4 has been released for a few years now.
The specification of the IP address can under some circumstances be "incorrect" or out of date
(see next subchapter).
In addition, the host name is saved in the aweprogversion.host field, which you can use to orient
yourself.


12.1.  Apparently                           incorrect              IP        address                 in
  aweprogversion
12.1.1.         Computer with several IP addresses
An apparently incorrect IP address in the aweprogversion.ipadresse field can be caused by having
several IP addresses available to the computer.
This would be conceivable if a computer has two network cards.
In one case at a customer's, however, two IP addresses were configured for one network card.
Here's a screenshot as an example:




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                  70
12.1.2.        Computer with dynamic IP address
For a computer with dynamic IP address, the IP address can change after a reboot.
With the command "ipconfig/all" on the command line, you can get an overview of the IP
addresses.
The entry "DHCP" indicates whether static or dynamic IP addresses are used.



12.1.3.        Computer with additional mobile phone network
If the customer is using the SmartCompanion, a special network will be set up for incorporating
mobile phones.
For access to the mobile phone network on the computer, another IP address is required, which
belongs to the corresponding subnetwork.




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                               71
13. Update
13.1.           Language-dependent descriptions
The table 'errmsg' is delivered completely with each update (with all languages).
In the normal update procedure, there is already a script 'upd_lang_spec' that enters language-
specific texts in a series of tables.
The field references from the table 'errmsg' are joined with the language from alcibspr.
Starting with QR2310: Due to MODUL_INTERNE_MANDANTENTRENNUNG, together with
MODUL_INTERNE_MANDANTENTRENNUNG_SPRACHE
We will provide complete messages for all languages upon delivery. For this, the unload will be
expanded with the creation. For the languages for which not all sentences exist, the missing
sentences will be added as copies of the German sentences in question. We initially thought that
we would use the English sentences as filler material. However, some of those are missing as
compared to the German entries. If necessary, I can also insert a two-step filling where the filling
is done first with English and then again with German sentences.
I inserted the (single-stage) expansion we discussed today (10/25/2023). With the official delivery
of QR2310, this would already be included.


The descriptions from the table artvermassspr go to the local language, which the customer can
define himself.
If the local language is changed in ongoing operation (not recommended!), the script
artvermassspr_korrekt has to be called with change of the local language.




13.2.           Bit2Byte – conversion
Starting with Version 2009, actually this conversion is necessary starting with 2008.2. Starting at
this time, the ALCIB back end always works with Unicode data. That is, the database has to
transfer the ISO data to Unicode data. Of course this conversion causes problems with bit vectors,
which would contain other codes according to the conversion via the database.




13.3.  Places after the decimal point in SA and PU
  (DFUE)
You can now set up the system such that size details support 10ths of mm. To do so, enter 10 for
variable IMP_CTRL_NTEL_MM. Version updates now run a script which ensures that 10ths of mm
entries are retained after the update. For this, the script adaptimpfldctrl is called during the
version update. This script must be called once manually during activation.Previously, you had to
manually run script set10telmm to get the same result.


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                   72
Remember to also set variable MASSFELD_RUNDUNG to 1. This is necessary to ensure that the
parts list equation properly computes the bottom part even if only one decimal place is available.
The variable can now also be set to the value 100.
Thus, the possible values are currently:
    •   10 = 10-th mm -> 1 place after the decimal point
    •   100 = 100-th mm -> 2 places after the decimal point




13.4.   Market      partner-specific                                       configuration
  (aldfuetyp and aldfuectrl)
The table contents of aldfuetyp and aldfuectrl are inserted for an AWE Backend installation or a
version update via the TABS_TO_LOAD logic (...install\data\TABS_TO_LOAD) and the lang_spec
logic (...install\cmd\lang_spec.list) automatically depending on the language.
The table contents are display in System > Data transfer > Document transfer > Configuration as
"Type of the EDI" (aldfuetyp) and "Control type" (aldfuectrl). The IDs stored there are saved in the
table mpdfuectrl depending on the MP.
If for the customer entries in the tables aldfuetyp and aldfuectrl are missing, you can insert them
manually after the fact. As a sample, use the entries of the tables on the development system
(asteraix 130 - status as of 07/26/2021).
The entries in the tables can be brought in case of doubt to the current status of the current
highest delivery version (delete of the old content, then execute of all insert statements,
unload/load of the al* tables); a version distinction is not required.


For the developer who adds entries, it applies: all relevant DBs are updated!
Status as of 02/10/2022, these are: alcib_140, alcib_1140, alcib_130, alcib_1130




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                  73
14. Quality release
14.1.          Installation with environment
14.1.1.        Requirements
   •   This logic only functions under Linux, not AIX
   •   Installation of the AWE Backend Update tool
           o   Copy directory \\jupiter\ALCIB_Install\AWE_Update_Tool to the Windows server
               to C:\tools or c:\temp.
   •   Backend
           o   Check whether /alcib/install/alcib_update.cmd exists. If it does not exist, then
               install/have it installed from the development environment
           o   /alcib/install/alcib_update.cfg – contains information about where and how the
               new packages can be obtained.
               Most entries are documented inline here. Only a few special entries will be
               mentioned here, for which inline would be too long:
                      INTERACTIVE="YES"
                       Switch is evaluated if the script is executed on the shell. If NO is here, the
                       answers to all questions must be transmitted via parameter (see "usage"
                       in the script). Therefore, recommendation: yes
                      ALCIBSERVICES="alcib"
                           •   See e.g. /etc/init.d
                      INFORMIXSERVICES="ifxsrvalcib"
                           •   See e.g. /etc/init.d
                      UPLOADDIR=/upload/${RELNO}
                           •   The logs of the update will be transmitted back to the upload
                               directory. It is on the FTP server from which the update packages
                               were downloaded.
           o   /alcib/install/alcib_update.pkgs – contain the information about which packages
               should be obtained with reference to the languages.




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                                 74
           o   If necessary, with the first call (.)suc /alcib/install/get_setup.cmd ausführen and
               answer all questions with yes.



14.1.2.        Procedure
   •   Start from c:\tools\AWE_Update_Tool\Albwir.Deployment.Config.AWEUpdate.exe. For
       future versions / you should put a shortcut on the desktop for this.
   •   The tool opens an SSH connection with user awserve from the Linux server. The report
       dialog must be filled out appropriately for this
       Server: Linux backend server
       User: cannot be changed. The update must absolutely be executed as awserv
       Password: Password for awserv on the Linux backend server
       Site no.: Client number that should be updated primarily. If several clients are installed on
       a server, it is decided on the following dialog whether they should also be updated.




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                                  75
   •   Green – version to be installed (Note 20.01.2023 IS: There is still a need for action here.
       That's not right yet)
   •   Client: Client number from xhaus
   •   ALCIBPRG: Main program directory configured for this client
   •   DB Version (yellow here) – installed version of the individual clients – this is the number
       from xhaus. vers_seqnr or alsqlhist.seqnr and reflects the sequence number of the last
       installed SQL script.



A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                                  76
    •   QR:
    •   Update: In this field, it is possible to define whether this client should be updated.
"Show protocol" button displays the output of the communication with the Linux server. You can
switch the client on the upper part of the dialog.
Caution for the selection of the client to be updated. Clients with other AWE versions may not be
selected, for example.
NEXT - Button




The maintenance should be activated on the systems to be updated so that no more users can log
on.




The upper part of this dialog shows all processes that are currently accessing the databases that
were uarked as to be updated. Currently, during the installation, no processes may access the
database.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                77
The middle of the dialog shows which background processes and services potential database
connections could establish.
Exit Servers – Button
Stops all background processes on the Linux server and updates the display.
Sometimes, not all background processes can be ended correctly. However, it is important that on
the middle part, there are no more A+W Enterprise background processes (User: alhi*), since
otherwise these start additional processes and thus establish database connects again. To end
these processes, you can use the "Need to kill" button in the last column of the middle part of the
dialog.
Need to Kill – Button
End background process with signal. There is no update of the dialog. This has to be done
manually with the "Refresh" button.


Send Stop to Windows Services
Sets the Windows services (such as the export service) into a maintenance mode. In it, the
services do not access the DB. The status is reset when the CTRL server is accessible again. It can
take a moment until the processes have ended their database connection. Use the "Refresh"
button to update the display.


If the top list is empty, the installation can be started with Next.
Next – Button




    •   Download latest from A+W FTP Server – activate if new packages should be loaded
    •   Install Binaries from Downloaded Packages – should also be activated in the standard.
Next – Button



A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                 78
There is another security query "Execute update script?" If the question is answered with "yes,"
the update starts.
Installation can be traced on the installation log window.
After installation finished
Next - Button




Next – Button




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                               79
Check whether all processes were started again.
Mode:
    •   Running – process is working
    •   Waiting – Process is in the normal wait interval
    •   Stop send – Process is informed that installation should proceed – Exit DB connections
    •   Stopped – Process has stopped working and is waiting for another connection to the CTRL
        server to be established
    •   Processing – Processing is in job processing right now


14.2.           AWE (Backend) updates as of Version 6.4
Starting with this version, backend binaries (hotfixes), if nothing else is explicitly agreed upon, will
be compatible with older backend environments. This will be ensured before release on the QS
system, which has an old environment status.
Such hotfixes can, in case of error at the customer's, be brought out via the Hotfix manager.
For new functionalities, generally new environment files and changed database structures are
required (identification ENV in the release notes). A backend update is required for these
environment changes. This update the whole environment completely. It provides the program
with access to new data structures.


A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                  80
The AWE Windows services, the ERP WebService, as well as the AWE frontend are connected to
the AWE database and to the back end servers (alrpc, ctrl_server, etc.); these should also be
updated in case of an AWE update. They are still developed so they are backwards compatible
and can cope even if there is an older DB status.




A+W Software GmbH             EN-CONFIG-A+W Enterprise System.docx                              81
14.3.           New QR - compatibility AWE/AWP/SN
With the publication of a new QR by the customer, it should be possible using the table listed here
(status as of 03/08/2023) what must be heeeded when updating the A+W components with
regard to compatibility.
If at all possible, A+W Enterprise components and A+W Production components should be
brought to the same QR status.
With regard to compatibility, you must pay special attention to the components that require an
SN installation (CAD Designer (Shapes)) for their functionality.
In A+W Enterprise these are:
  AWE Frontend                   \
  AWE Print Service                  = AWE-SN modules
  AWE CAD Service                /
Reference will be made to these three components in the table. They are combined under the
name "AWE-SN-Module"
For A+W Production, no components are distinguished for the compatibility examination. With
"AWP-SN", the installation of the A+W Production and the import together with an SN is always
meant below.
Digression AWP and SN:
Regarded formally, neither the A+W Production nor the A+W Production import absolutely need
an SN. However, the SN is necessary for an AWE-AWP installation in import if transferred orders
PO items or ordered subelements are included or if there are SN files in the order items.


1.   AWE and AWP have a main version < 6.
     AWE components and AWP are installed on the same computer or on different
     computers.
     You should update to Version 6.
     It is recommended that you update both systems to Version 6 at the same time.
     If you proceed in several steps, you must first update the production system (AWP).
     SN installations with different main versions are not very compatible.
     If a SN file is generated with the help of an SN with a higher version, it can no longer be
     opened by the SN with the lower version.
     If AWE SN modules and AWP SN are installed on the same computer, all components must
     absolutely have the same main version.
     Hopefully, this scenario will soon no longer be relevant because all customer installation
     will be using the main version 6.


2.   AWE and AWP have the main version 6.
     AWE SN modules or AWP-SN should get a QR update.
     The QR update can be installed. The updates can be done independently of one another in
     the AWE environment or in the AWP environment. The update of the SN represents no


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                               82
     problem in only one environment. (see further below for special cases for special QR)
     In the SN.ini, with the update of the SN, the entry "[Customer] FileVersion" remains
     untouched. This entry determines whether both SN installations in the AWE and AWP
     environment are compatible. As long as both SN installations are configured with the same
     "FileVersion", there is no problem with generating SN files both on the AWE side (via the
     iTOE) as well as on the AWP side and opening and editing each in the other environment.
     CAUTION: Individual QRs include such great changes that in these special cases the QRs in
     AWE SN modules and AWP-SN cannot be installed independently of one another.
     These QRs are listed separately in this table (see further below).
     Last special QR of this form: QR 11/22.
     Attention: A change of the "FileVersion" in the SN.ini will cause problems if after that
     there are SN installations on the customer system with different "FileVersion" settings.
     If a SN file is generated by an SN with higher "FileVersion", it can then no longer be
     opened/edited with an SN with lower "FileVersion". If you try to open this file with an SN
     in the foreground, you will get a correspondingly detailed message.
     If opening the SN file via the iTOE or in the background fails during scheduling, the error
     message that reaches the user may, under some circumstances, not clearly name the
     problem. In the log, however, you will find the message about the incompatible
     "FileVersion" in any case.
     Addition: The adjustment of the "FileVersion" is required in order to make new
     functionalities such as a new AW processing type available in SN. Which "FileVersion" is
     required for which functionality is evident from the SN release notes in question.
3.   Special case: SN hotfix/update after QR 11/21
     The SN API was expanded in the course of a ticket.
     If now just the SN is updated in the AWP environment, there is an error during import.
     The A+W Production must also be updated.
     See also [AW-105295].
     This case is only relevant if AFTER the QR date 11/21 an SN in the AWP environment is
     updated (regardless of whether with hotfix or QR setup). In this case, the AWP must
     absolutely be updated as well.
     Status of the information is as of 03/14/2022.
4.   QR 11/22
     With this release, the DXF import dialog was reworked.
     As long as an AWE QR < 11/22 is installed, the old DXF import dialog remains active. The
     version of the installed SN has no effect on this.
     As soon as an AWE QR >= 11/22 is installed, you will see the new DXF import dialog; here
     too, the version of the installed SN has no effect.
     The instructions listed below come from information from Techsoft (CAD area). See also
     feature #80807 in Azure DevOps.
     For systems with an AWP/SN installation QR < 11/22, it applies that:
         -   There may never be an update to AWP QR >= 11/22 without also updating the SN
         -   An update of the SN alone to QR >= 11/22 is possible if the version of the AWP is


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                               83
          at least QR 06/22 and all AWP hotfixes have been installed


   For systems on which both AWE-SN modules and AWP-SN with QR < 11/22 are installed,
   it applies that:
      -   As soon as AWE-SN modules were updated to QR >= 11/22, the version of the
          AWP-SN must be at least QR 06/22 and all AWP hotfixes must be installed




A+W Software GmbH           EN-CONFIG-A+W Enterprise System.docx                        84
15. SetupLauncher
15.1.           Properties
During the installation of Windows components with the SetupLauncher, it happened (status as of
03/25/2022) according to statements from planners and customers that there were problems
after the installation if ICE services (Booking, PatternViewer) were also running on the computer
on which the installation was done. The ICE services were no longer accessible after the
installation.
This phenomenon is probably related to the dependencies that are stored in the package.xml of
the setup in question. As soon as there is a dependency of "A+W Infrastructure 6 Collector
Services", the problem occurs.
In the package.xml of "A+W Infrastructure 6 Collector Services", there is a dependency of "A+W
Infrastructure 6 Middleware". The setup instruction to stop all IceGrid nodes before the
installation process is stored in the package.xml of "A+W Infrastructure 6 Middleware".
The suspicion is that stopping the IceGrid nodes in the installation process happens regardless of
whether then "A+W Infrastructure 6 Middleware" (or "A+W Infrastructure 6 Collector Services") is
actually installed or the installation is skipped because the installed version is already up-to-date.
Whether the stopped IceGrid nodes are also started again automatically if the "A+W
Infrastructure 6 Middleware" (or "A+W Infrastructure 6 Collector Services") is actually installed is
not known.
If the "A+W Infrastructure 6 Middleware" (or "A+W Infrastructure 6 Collector Services") is not
installed, the IceGrid nodes remain stopped after the installation and have to be restarted again.
As soon as there is a check next to the component "A+W Infrastructure 6 Middleware" (or "A+W
Infrastructure 6 Collector Services), the problem can occur.
The action instruction to prevent the problem is, after selection of the Windows components to
be installed, to manually remove the checkmark placed automatically for "A+W Infrastructure 6
Middleware" and "A+W Infrastructure 6 Collector Services" so that the IceGrid nodes are not
stopped during the installation.
There exists for this the Azure DevOps PBI 63048.




15.2.           Research on the setup process in general
If during the installation of Windows components there are problems via the Setup Launcher, it is
possible to analyze the setup process via the trace file of the SetupLauncher.
The trace file is in the directory %PROGRAMDATA%\A+W\Log. Name:
Albwir.Deployment.SetupLauncher_*




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                   85
15.3.   Research on the setup process for individual
  programs
For the individual programs installed via the SetupLauncher, there is a log file with the name of
the installed program (for example, "A+W Enterprise 6 Frontend.log) in the directory
"%PROGRAMDATA%\A+W\Installation Log".
The installation of the program in question is logged in this file. If there are errors during
installation, the log can provide useful information.




15.4.           Installation of the A+W Enterprise Frontend
During installation of the A+W Enterprise Frontend, the SetupLauncher often issues the message
that the server must be restarted in order to complete the installation.
The reason for this can be the running fxsshproxy service. A dll should be replaced, but it is being
used at the moment.
In "%PROGRAMDATA%\A+W\Installation Log\ A+W Enterprise 6 Frontend.log" you find the
message:
" The file C:\Program Files (x86)\A+W\A+W Enterprise 6 Frontend\fxsshproxy\bin\cygcrypto-
0.9.8.dll is being held in use. Close that application and retry. "


See also PF [AW-155106].




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                  86
16. Installation/update of Windows
 components
16.1.           ERP Webservice
The ERP webservice can be updated in ongoing operation.
However, the AWP import and booking engine should be stopped.
For safety's sake also the AWE B2B service.


16.2.           A+W Infrastructure & A+W iQuote
I sent a question catalog to Dirk Holzapfel a long time ago.
DIH: The whole topic is complex and can only be solved poorly with documentation or similar, for
the people on-site with the servers must understand the connections and the problems. Each
installation for each individual customer will be slightly different and there is no "standard"
answer. There are "greenfield" installation instructions if it is possible but everything else must
simply be well-prepared and thought through before starting out to execute 2 steps somewhere.
Here's the revised version:
Are there installation instructions?
    -   EN-INST-A+W Enterprise iQuote + EN-INST-A+W iQuote
    -   EN-INST-A+W Infrastructure BasicData
What's the story with installations in ongoing operation or system?
    -   Update/addition to a previously existing installation are possible at any time and should,
        thanks to the service structure, only cause short-term drop-outs of other components.
    -   For iQuote itself, there are installation instructions in which more or less precisely this
        case is depicted. iQuote web on a server in the Web.Configurator service on a server in
        the DMZ and the rest of the services on other computers (caution: here too, the majority
        are possible). In between VPNs with firewalls.
Installation of A+W Web.Configurator + iQuote on one server and the rest of the infrastructure +
production on another process server. All services communicate via an infrastructure. Is this
layout theoretically possible?
    -   For this, we have precisely the services structure that we can divide across computers and
        also have in case of load distribution on several computers. Especially since we cannot
        install the Linux things on the same computers. So everything's OK.
    -   Of course as usual, 1 ServiceLocator + infrastructure is correct. There is only one main
        node for the communication.
    -   Of course the installation of iQuote and configurator on one server is also possible, but
        questionable from the point of view of security. For with this, you open up the Ice services
        to the WAN/Internet world as long as the separate process computer should be in the
        WAN/Internet world. There are actually other instructions, whereby of course things


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                  87
        depend on the customer and application case. (ALW note: at Caleo, the A+W iQuote is on
        the WAN/Internet server, Web.Configurator on the Enterprise process server, and
        infrastructure, etc. on the production process server)
    -   The installation of the services on the Linux machines necessarily means that the
        appropriate port ranges in the firewall must also be opened there. However, this is
        documented on your side as far as I know.
    -   Our setups do this on Windows servers if the internal Windows firewall is used. If the
        customer is using different software, it must also be opened manually, but should be
        documented in the Infra instructions.
    -   Things work precisely the same way on the path between hardware firewalls (on the
        routers), with the jump from the web to a DMZ and then to the internal network, this
        would even be advisable to have. There too, the customer's ICT must be set according to
        circumstances.
Will the scripts for the A+W iQuote workflows be delivered completely if you install the
infrastructure once or only if you install A+W iQuote after the fact?
    -   The DB scripts for the workflows and the workflows can be in different places and I
        currently do not know how the solution is selected in the iQuote environment. They can
        be in the scripts for the Infra domains and are then triggered by the Workflow Service.
        They can be in the scripts of the Web domain, then the Configurator triggers services for
        them. But we also have services that sort of bring their "default" scripts along internally
        and update the DB when starting. So there are several possibilities.
    -   If, of course, the Infrastructure Database service was/is old and the FTP access has been
        deactivated (note ALW: can be set via the Config Tool infrastructure), then it can be that
        everything is not completely up-to-date. Whereby the service wouldn't even start.
    -   Note ALW: default workflows via new installation have always been a problem and
        caused the planners to have to install the workflows manually.


If we want to install a new Windows component, does the complete infrastructure have to be
booted up by the new .Net framework?
    -   The .NET framework must be brought out if the infrastructure is pulled to a new version
        or one of the other services or domains. That means that an old infrastructure would
        cope with new services from other domains or vice-versa, a new infrastructure would
        cope with old domains. Only if both of these things are installed on different computers.
        ICE is completely compatible between mixed services. Only the infrastructure domain
        must be updated completely since we could otherwise produce mistaken dependencies
        there. The exchange of an individual service for the new .NET version should be possible
        outside of the infrastructure (if the corresponding middleware is there).




16.3.           A+W CAD Services
The A+W CAD Services may not be confused with the A+W Enterprise CAD Service.
The A+W Enterprise CAD Service is a Windows service that is only active in the Enterprise
environment. It is responsible for the generation of SN files in the background.


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                  88
The A+W CAD services are a Windows service made available by technical development that units
different AWSOA services:
   -   CADSheetsService (provision of geometry data for items, currently used for reference
       marks and frame geometries in A+W Production, support of the DXF import – import of
       dimensions - in SN)
   -   CADDigitizing (iShape functionality)
   -   CADGeometry (provision of the shape catalog/shape preview images)


The CADGeometry service is used by A+W iQuote. When starting iQuote, the entire shape catalog
is loaded via CADGeometry.
Thus, the A+W CAD services must absolutely be installed when using iQuote.




A+W Software GmbH             EN-CONFIG-A+W Enterprise System.docx                            89
17. A+W licensees in AWE Windows
 programs/services
The release of AWE modules via an A+W license (LicenseClient/LicenseServer) is the exception in
A+W Enterprise.
An A+W license is currently (as of 01/06/2023) still required for programs/services that are used
both in AWE as well as in the AWB environment.
This affects:
    •   BMECat Import (special license for each hardware manufacturer)
    •   ERP Stock Service (special license for each third-party storage provider)


For details about the required licenses, see the relevant configuration document.


Special case AWRack
AWRack is, although long since terminated, still in use by some customers in the AWE
environment.
An A+W license is also required for AWRack.


Special case: A+W iQuote
There are 2 license modules for A+W iQuote.
On the one hand, there is the iQuote configurator; it allows the configuration and use of the
information module (history).
And the A+W iQuote Info module only. This module allows only the use of the information area,
with no possibility for configuration.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                90
18. AWE Windows Services - AWE trace
 settings for research
CAUTION! For all programs, when setting the trace level for the research, it applies that:
On the "Basic" tab, be sure to leave the category "AlbwirBasis" on trace level "Error"!


18.1.           ERP Webservice
For a detail research in the ERP webservice, set the logging as follows:
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




Generate additional research file -> env variable AWC_ERPDOC_FILE
The AWE env variable AWC_ERPDOC_FILE has to be activated with the value "201."
The ERP webservice does not have to be restarted after setting the variable.



A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                          91
By setting the variables, a return object is written as xml file to %ProgramData%\A+W\A+W ERP
Web Service. The file name of the return object contains the order number and a time stamp:
compsc_<auftrnr>_YYYY_MM_dd_HH_mm_ss.xml
The logic was developed with AWDesk #435600. In order to be able to use the functionality, the
ERP webservice has to be from 28.02.2019 or later.



18.1.1.         Research in case of incorrect POs
If an order-related PO is incorrect, usually a large quantity of data and logs are required to
research the problem. These include, among others:
    -   The OrderXML file of the order
    -   The OrderXML log
    -   The ERP Webservice log
    -   The return object
    -   Data from:
            o   awc_modparams
            o   bestparameter
            o   intbest / bestwun




18.2.           OrderXML Service
For a detail research in the OrderXML service, set the logging as follows:
The trace level category "AWEBasis" has to be on "Debug."
The trace level category "AWEOrderXmlService" has to be on "Info."
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                             92
18.3.           B2B Service
For detail research in the B2B service, set the logging as follows:
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                          93
18.3.1.         Research the eInvoicing export
To research the eInvoicing export, the following is required:
    -   Prerequisite: Correct configuration of the AWE B2B Service log
            o   Category "AlbwirBasis" with Trace Level "Error"
            o   Category "AWEBasis" with Trace Level "Debug"
            o   Category "ERPOpenTrans" with Trace Level "Debug"
    -   B2B Service log
    -   The generated eInvoicing file
If the relevant log is not available in the required log depth, the process of creation can be
initiated again:
    -   Either an existing record is updated for calculation with error status in the table ottransfer
        to steuerflag = 0




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                94
    -   Or an already processed record from the table ottransferok is unloaded and inserted with
        steuerflag = 0 again into the table ottransfer.
    -   Or a manual INSERT statement is executed in the shell
        ("document" can be 7 or 9 - invoice or credit):
        insert into ottransfer (auftrnr, vorgang, schnittstelle, steuerflag, filltime, lfdnr, serviceid,
        subnr, hausnr, routenr, ltplan, uzeit,
        doctype, subtype, comment, filename, serviceid2) values (<auftrnr>, <vorgang>, 'E-INV', 0,
        CURRENT YEAR TO SECOND, 0,
        0, 0, <hausnr>, 0, '31.12.1899', CURRENT YEAR TO SECOND, 1, 1, 'e-invoice', ", ")

        Caution: If the INSERT is executed in the Server Studio, there can be an error due to the
        ltplan value. Then an empty string (") can be transferred for ltplan.



18.3.2.         Research about the EDI export
To research the EDI export, the following is required:
    -   Prerequisite: Correct configuration of the AWE B2B Service log
            o   Category "AlbwirBasis" with Trace Level "Error"
            o   Category "AWEBasis" with Trace Level "Debug"
            o   Category "ERPOpenTrans" with Trace Level "Debug"
    -   B2B Service log
    -   The generated EDI export file
If the relevant log is not available in the required log depth, the process of creation can be
initiated again:
    -   Either an existing record is updated for order with error status in the table ottransfer to
        steuerflag = 0
    -   Or an already processed record from the table ottransferok is unloaded and inserted with
        steuerflag = 0 again into the table ottransfer.
    -   Or a manual INSERT statement in the Shell is executed:
        insert into ottransfer (auftrnr, vorgang, schnittstelle, steuerflag, filltime, lfdnr, serviceid,
        subnr, hausnr, routenr, ltplan, uzeit, doctype, subtype, comment, filename, serviceid2)
        values (<auftrnr>, 2, 'EDIEXP', 0, CURRENT YEAR TO SECOND, 0, 0,
        0, <hausnr>, 0, '31.12.1899', CURRENT YEAR TO SECOND, 1, 1, 'edi export' ", ")

        Caution: If the INSERT is executed in Server Studio, there can be an error due to the ltplan
        value. Then an empty string (") can be transferred for ltplan.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                      95
18.4.           Export Service
For detail research in the export service, set the logging as follows:
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                          96
18.5.           AWE CAD Service
For detail research in AWE CAD, set the logging as follows:
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                          97
18.6.           Print Service
For a detail research in the print service, set the logging as follows:
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                         98
18.7.            AWE front end
For a detail research in the AWE front end, set the logging as follows:
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




18.7.1.          Research about the FinAc export
Manual insert statement in the table fibutransfer.
After-the-fact generation of the export file
    •   Document
        insert into fibutransfer (fibutransid, status, hausnr, btyp, auftrnr, vorgang, subnr, mpnr,
        kuliflag, izeit, uzeit, serviceid, versuche, xmldatei, xmldatei2, sfill1, sfill2, lfill1, lfill2, cfill1)
        values (1, -1, <hausnr>, 2, <auftrnr>, <vorgang>, 0, 0, 0, CURRENT YEAR TO SECOND, '', '',
        0, '', '', 0, 0, 0, 0, '');




A+W Software GmbH                  EN-CONFIG-A+W Enterprise System.docx                                             99
Updating of the totals
insert into fibutransfer (fibutransid, status, hausnr, btyp, auftrnr, vorgang, subnr, mpnr, kuliflag,
izeit, uzeit, serviceid, versuche, xmldatei, xmldatei2, sfill1, sfill2, lfill1, lfill2, cfill1) values (-1007, -1,
<hausnr>, 7, 0, 0, 0, 0, 0, CURRENT YEAR TO SECOND, '', '', 0, '', '', 0, 0, 0, 0,0)




A+W Software GmbH                   EN-CONFIG-A+W Enterprise System.docx                                       100
18.8.           ERP Stock Service
For a detail research in the ERP stock service, set the logging as follows:
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                         101
To trace the „Panorama“ interface:




A+W Software GmbH             EN-CONFIG-A+W Enterprise System.docx   102
18.9.           FinAc Service
For a detail research in the FinAc service, set the logging as follows:
The trace level category "AWEFinAcService" has to be on "Debug."
Whether "AWEBasis" is also set to "Debug" must be decided on a case-by-case basis.
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                         103
18.10.          BMECat Import
For a detail research in the BMECat Import service, set the logging as follows:
The trace level category "ERPBMECatalog" has to be on "Debug."
The trace level on the "Basic" tab (category "AlbwirBasis") has to be set to "Error," since
otherwise the log will be too large.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                          104
18.11.          A+W Commercial 6 Converter Service
The setting of the logging is done with the "A+W Logging Config Tool".
For a detail research in the Converter service, set the logging as follows:




The trace level category "CommercialConvert" has to be on "Debug."




The trace level on the "A+W Enterprise" tab can also be set to Debug in order to evaluate basic
error analyses. And on the "SNLive" tab (category "CADLive"), Debug can be set for examinations
in the direction of the CAD service. These switches most affect the A+W iQuote screen generation.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                          105
A+W Software GmbH   EN-CONFIG-A+W Enterprise System.docx   106
18.12.          A+W iQuote 6 Services/Web
The setting of the logging is done with the "A+W Logging Config Tool".
For a detail research in A+W iQuote, set the logging as follows:




The trace level category "WebConfigurator" and "WebWeb" has to be on "Debug."




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx            107
The WebConfigurator services, which should be set as follows, belong to the A+W iQuote:




The trace level category "WebConfigurator" and "WebWeb" has to be on "Debug."




A+W Software GmbH             EN-CONFIG-A+W Enterprise System.docx                        108
18.13.         SN connection
18.13.1.       Trace AWE Frontend
With the Config tool of the AWE Frontend, the trace level for the various modules can be set.




For research of SNLive/iTOE/DXF problems, first the following categories of the tab "A+W
Enterprise Frontend" are set to the trace level "Debug":
- AWEBasis
- AWEModulesCADLive
Furthermore, on the "SNLive" tab, the category "CADLive" should be set to "Debug".


CAUTION:
On the "Basic" tab, be sure to leave the category "AlbwirBasis" on trace level "Error"!
On the "A+W Enterprise Frontend" tab, absolutely leave the category "AWEFrontendMain" and
"AWEFrontendNetIf" on trace level "Error"!




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                             109
18.13.2.        Trace AWE Frontend – long-term setting
On the debug level, the front end logs quickly become very large. For a longer-term setting for the
customer, use (with an appropriate Frontend version, see AWDesk #389547) the info level for the
category "AWEModulesCADLive". On this level, all SN transfer information is logged.




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                             110
18.13.3.        Trace SN




On the "SN" tab, set the category "CAD" to trace level "Debug".



18.13.4.        Research for the SNLive image file
Possible starting with AWE Frontend Version 6 (03/13/2016)
If the SNLive sketch in the front end is incomplete or cut off, it can be helpful to compare the
front-end view with the image file actually generated by SN. The image file is saved temporarily
and is retained until a new SNLive sketch is generated or the AWE Frontend is ended.
The temporary image file is stored in the temp user directory. You can reach the directory by
entering a "%temp%" in a File Explorer window on the path line. From there, you have to change
to the subdirectory "AWECADExchange". The name of the image file consists of the abbreviation
of the image type (for example, "BMP), the aufnr, the posnr, and the time stamp.
If you want to consult the temporary image file in the print service, of course you have to change
to the temp user directory of the print service user.



18.13.5.        Research with involved SN file
In case of problems with attached SN files, or macro or template files, please attach the affected
SN file or SN macro/template to the ticket.


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                               111
18.13.6.         Special things to note in the iTOE research
The logic of the iTOE is distributed across AWE and SN; within the AWE, there is a further
distribution across Backend and Frontend. Different developers are responsible for each of the
areas AWE Backend, AWE Frontend, and SN.
If there is a problem in the iTOE, it is usually not possible to decide immediately using the error
message in which of the 3 areas the cause of the problem lies. That's why there has to be as much
information as possible for research.
The basic information includes:
- the error description
- ftest and toeneu log (for research in the AWE Backend area)
- AWE Frontend log (for research in the AWE Frontend area)
- SN log (for research in the SN area)
- SN file (if a file is involved in the problem)


Finding the associated SN log
If the trace level for "AWEModulesCADLive" is set to "Debug", there is an entry in the frontend
log: "SN.Constructor(SN3): Process ID <...>".
The correct SN log can be found using this process ID: "SN_<date>.<processId>.x.awtrc


Experience has shown that in the end, precisely the log would have been important that you don't
have; that's why it's recommended that when you are reporting an iTOE problem, you should
send all logs along to Development right away.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise System.docx                           112
19. AWE Windows services - notes
19.1.            Error messages from the AlbwirBasis
It can happen that error messages appear from the AlbwirBasis in the logs of the AWE
Windows services; these have no further effect on the program flow.

In the AlbwirBasis, there is a reaction to a timeout error (-908), in that the connect attempt
is repeated. If the connect is successful, the error is not sent to the outside.

But in the log, the message causes confusion.

Here is an example from the ERP Stock Service:




19.2.           E-mail configuration
For the e-mail configuration, the following logic applies for the port used:
If no port is specified in the configuration, the default port 25 is used. If the SSL encryption is
active ("Enable SSL"), there is an automatic change to the port 587.
(Additional note: With "implicit SSL/TLS" there is also the case that there is a change to port 465.
However, this logic is not used in the AWE Windows Services.)




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                 113
To see in the log of the AWE Windows Service which port was used in the end, the trace level for
the Albwir.Basis must be increased to "Debug".



19.2.1.          E-mails are not sent
If no e-mails are sent from an AWE Windows Service, the cause of the problem is output as error
message in the log. For this, however, the AWE Windows Service must be current enough (build
date >= 06/25/2025).
To see in the log of the AWE Windows Service which port was used in the end, the trace level for
the Albwir.Basis must be increased to "Debug".


Problems with the remote certificate
With activated SSL encryption ("Enable SSL"), the configured e-mail server authenticates itself
with the client (AWE B2B Service) using a server certificate.
A server certificate is issued by an official certification office. It has a limited validity period.
If when sending an e-mail the following error message (B2B Service log) appears:
„
The underlying connection was terminated: No position of trust could be issued for the
protected SSL/TLS channel.
The remote certificate is invalid according to the validation procedure.
“
this indicates that the server certificate provided is flawed or expired.
This problem cannot be solved on the client page (AWE B2B service).
The customer must research why the certificate problems arise and whether the certificate is
expired and must be renewed.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise System.docx                                  114
20. Sketch "Product structure"
20.1.           General Information
In the master data articles and in the document entry, the product structure is depicted in a
sketch. Here is a sample depiction:




For the sketch, instead of "product structure", sometimes other names are used. These include:
"BOM depiction", "BOM viewer", "BOM image", "glass structure", and "side view".
The sketch is generated in the frontend and also in the Print Server if it is supposed to appear on
the printout. Both programs use the same logic for this.
The actual generation of the sketch is done by a Techsoft functionality, the
"Albwir.Alcim.ProductViewCreator.ViewCreator".
The information about the product structure will be stored in a string for transfer to
Frontend/Print Service.
For the display in AWE, the string is generated dynamically at the time the image is displayed and
transferred to the Frontend.
For the printout of the product structure in the Print Service, the string is selected from the
"kposp.bildcode" field.
The string is also called "Bildcode".
Example of an image code (not appropriate for the sample sketch above!):
"B200[100(cr<t5>)4210[220(<t15>)260()]100(<t5>)4210[220(<t15>)260()]100(cl<t5>)]"
For transfer to the "ViewCreator", in the logic module, which is incorporated both into the
Frontend and into the Print Service, the image code will be converted again into another format.
If there is an error during generation of the product structure sketch, instead of the correct
sketch, a dummy sketch with a big red exclamation point will be displayed.




20.2.           Search
If the product structure sketch is flawed or cannot be displayed, the cause is either in the AWE
Backend during the generation of the image code or in the Frontend/Print Service module during
the conversion of the image code into the ViewCreator format.
The ftest can be used for searching in the AWE Backend. The image code is output in the ftest.
In the Frontend/Print Service, the trace level must be set appropriately for searching.
Attention: There are only meaningful log entries starting with QR2406.


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                              115
Front end




Print Service




A+W Software GmbH   EN-CONFIG-A+W Enterprise System.docx   116
A+W Software GmbH   EN-CONFIG-A+W Enterprise System.docx   117
21. Package release dialog
21.1.           Binary activation
Under System > Activation / Enable > Binary Activation new program versions of A+W Enterprise
binaries can be activated. Binaries are programs that run in the Unix or Linux back end, e.g. alcib,
lapool, wlager etc.

On the dialog, first you select in the header for which program you would like to change the
program version. If you leave the selection empty, records will be displayed for all binaries for
which an activation is possible. For each program, that record is marked as active that is currently
active. In the Last activation column, it is indicated when an activation was made.

If the user selects another program version and exits the dialog after saving, then a script call for
the shell script activate_binary is generated from the selection in question and the script called.

In the script, the symbolic link is transferred from the previous program file to the new program
file. In case of success, an entry in the table bin_activation is made and a system message sent to
the user.

The special feature of this logic is that this way, you can reset a program version quickly and easily
if this should become necessary.

If the program version of the alcib binary is changed, the user is asked to restart the alcib since
only this way can the change become active.


21.2.           Package release
For an AutoUpdate system, it is first necessary to make available new program versions, hotfixes,
and environment variables.

Under System > Activation / Release > Package Release , various kinds of FTP packages can be
released. For this, you select in the header of the dialog whether you want to have all packages
displayed or only one that have not yet been released completely or only the latest packages.
Then you select the package type and can select a package name from a list. For the mode "only
newest packages", you can also leave the package name empty and then all available packages
are displayed in the table.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                 118
In the table, all records for this package are now displayed for which a release is possible if it has
not already been done. Released records are depicted with date and activated checkbox.
Packages once released cannot be released again.

Through selection of one or several records or with the "Select All" button and exiting the dialog
while saving, the selection of the call parameters for the shell script release_package is
determined and called. If the script call was successful, the release data is saved in the table
package_release.


21.2.1.         Configuration of autoupdate
/app/A+W/autoupdate/config/aweautoupd.cfg


21.2.2.         Logs
/app/A+W/autoupdate/log




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                119
21.2.3.         Troubleshooting
New binfiles are in the Buildbins directory, but they were not activated
During the autoupdate, the binaries are activated via the dfue_starter. It must be checked
whether corresponding files are in $DFUEDIR/wait and whether the dfue_starter runs for the
corresponding clients


21.3.           Requirements
It should actually be up-to-date for all customer installations, but for the sake of completeness,
the original requirements are listed here:

External call of a multilingual message dispatch

In order to be able to inform the user about success or lack thereof of the binary from the script
activate_binary, and this here in the user's language, the system message dispatch in alcib was
made available to the outside.

With the following call it is possible to use the system message functionality even outside the
back end.

alcib –meldnum_ext <alsysab.meldid> <mitarb.manr> <errno-Betreff> <errno-Body> <String-
Zusatz>

The prerequisite for this is that the corresponding values for message number, employee,
message numbers were also created in the database. A special FIX-license is therefore not
necessary in order not to limit the functionality.

For this case, the system message 84 "Binary Activation" was newly created.

User rights

For both dialogs, new module rights were set up. The Binary Activation dialog is controlled via the
SYBA module right. The Package Release dialog with the SYBR module right.

Installation instructions

The following SQL scripts must be run

130004012_bin_activation.sql

130004013_package_release.sql

130004018_bin_activation.sql

130004019_package_release.sql

The following environment files are required


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                 120
Skripte aus $ALCIBPRG/cmd

cmd/activate_binary

cmd/getbuildbins

cmd/release_package

cmd/getftppackages




21.4.            Housekeeping
The number of files (Binaries) in the directory $ALCIBBIN/buildbins increases with each hotfix
installed. A life span for these files has not been defined thus far. If space becomes important,
then it is possible to clean up this directory by calling the shell script 'cleanbuildbins.sh'. The script
removes all files that do not point to a symbolic link from $ALCIBBIN and those that no longer
exist as package in the initial repository of the hotfix distribution logic (Standard:
/app/A+W/autoupdate/repository/ftp-in).




A+W Software GmbH                 EN-CONFIG-A+W Enterprise System.docx                                 121
22. Informix error messages
22.1.           Informix errors in Windows services
22.1.1.   SQL0035N                    The file 'en_us\IBM.Data.Informix.xml'
    cannot be opened
INFORMIXDIR in setnet32 is not set correctly.
Solution:
    -   Set INFORMIXDIR in the setnet32
    -   setnet32: "Use my settings“ should NOT be checked


22.1.2.         Not enough space for parser stacks
When using A+W Windows services/Web services, there are still memory problems in interplay
with the Informix client SDK 3.50 TC 9.
The following exception occurs (sample):
2017-04-19 08:20:27.868 | [1160] | [0x00000008] | ERROR | AlbwirBasis             |
AMPSV016ABM0P\awserv | (null)         | (null) | "Exception occured in AWDataAdapter.Fill(): ERROR
[HY000] [Informix .NET provider]General error.Not enough space for parser stacks/n at
IBM.Data.Informix.IfxConnection.HandleError(IntPtr hHandle, SQL_HANDLE hType, RETCODE retcode)


Various AWDesk cases already exist about this problem, e.g.:
#357891
#395012
#374675
#395469


To solve the problem, the current Informix Client-SDK (Stand 28.01.2022: 4.10 TC11) must be
installed.
The currently valid Informix Client SDKs for A+W installations is made available via the current
SetupLauncher.
During update, before installation of the new Informix client SDKs, the old one must be
uninstalled completely. Two client SDKs installed concurrently cause additional problems.
For the correct procedure for updating the Informix client SDK, there is a special chapter in this
document called "New installation Informix Client SDK".




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                 122
23. New installation Informix client SDK (32-
 bit version)
Attention: first the old Informix client SDK must be removed completely(!) from the computer! An
update is done through uninstallation and new installation.


Procedure:
    •   Uninstall Informix client SDK (via Windows system settings: Uninstall programs/remove
        programs)
    •   Reboot computer
    •   Remove all old client directories (-> e.g. C:\Program Files (x86)\IBM\Informix\Client-SDK)
    •   Reboot computer; if directories cannot be deleted because files are still being accessed,
        reboot computer again
    •   Obtain the current Informix Client from sw_install (\\jupiter\SW_Install\v6\Diskset)
    •   Install the new client via the Setup Launcher
    •   Reboot computer


Then it's best to check again whether the Informix path is correct:
    •   Path-Variable? (-> environment variables)
    •   INFORMIXDIR in the setnet32 (very important, must be set correctly!)
    •   setnet32: "Use my settings“ should NOT be checked




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                123
24. Possibility for reaction in case nothing
 happens
By setting the environment variables
         FXUSERIDLEFACTOR
it is possible after a particular time to call up a function of the application without user inputs;
whose address is stored in the variables
         S_user_is_idle
. The function thus has the possibility to cancel the application. If no address is stored in the
variables, then no function is called and the mechanism remains without effect.
FXUSERIDLEFACTOR cannot be defined in seconds for technical reasons. You have to enter a
factor for FXREADTIMEOUT0.
FXREADTIMEOUT0 defines the time in seconds after which the application asks for news from the
front-end. After that time, the reading routine will be interrupted, and the system asks for news -
unless the reading route closes before because a character has been read.
Example
Startscript:
...
Possibility for reaction in case nothing happens 98
Possibility for reaction in case nothing happens 99
FXREADTIMEOUT0=60
FXREADTIMEOUT1=120
FXUSERIDLEFACTOR=5
export FXREADTIMEOUT0 FXREADTIMEOUT1 FXUSERIDLEFACTOR
# start application
...
application.c
void my_user_idle()
{
fprintf(stderr, "User is idle\n");
}
main()
{
...
S_user_is_idle = my_user_idle;
...

A+W Software GmbH                    EN-CONFIG-A+W Enterprise System.docx                              124
}
After FXREADTIMEOUT0 - that is, after 60 seconds - a life sign is required from the front end. This
must arrive within FXREADTIMEOUT1 - that is after 120 seconds. Otherwise the application is
aborted.
If 5 times (FXUSERIDLEFACTOR) one immediately after the other a life sign is requested – that is,
after FXUSERIDLEFACTOR * FXREADTIMEOUT0 = 5 * 60 = 5 min - the function my_user_idle() is
called. In this example, only a message is output by this function. If within this time a key is
pressed, then the internal counter is reset and the time begins anew. my_user_idle() is then
called 5 min. after the last keypress.
Problems
The inputs in edit controls of the FIX version starting with 4.0.0 are not sent to FIX right away.
Only when you exit the field are events sent to FIX. If a user remains for the time of
FXREADTIMEOUT0 in one and the same field, then FIX requests a life sign.
This is not problematic since FIX/Win generally sends the life sign. However, if the user remains in
the same field for the time FXUSERIDLEFACTOR * FXREADTIMEOUT0, then the function
S_user_is_idle is called - regardless of whether the user types in the field or does nothing.
For this reason, the value FXUSERIDLEFACTOR * FXREADTIMEOUT0 should be so large that the
user can enter a field value within this time without problems.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                125
25. Cancel in case of lack of activity
If the AWE front end cancels after 10-15 minutes of inactivity, then the network is probably set so
that the connection is severed after a particular idle time. Here, the process usually gets hung up
under Linux.
You can counteract this by activating the variables in the previous chapter so that the problem is
not ended accidentally, but instead, information ia sent to the front end within a relatively short
time span. This keeps the connection open.
e.g.:
FXREADTIMEOUT0=60
FXREADTIMEOUT1=120
FXUSERIDLEFACTOR=1440




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                              126
26. Front end
26.1.           Problem with SSH proxy connection
There can be problems with the communication via SSH proxy from the Windows front end in the
direction of Unix back end. After the login attempt, the following error message can appear:




If this message occurs, please check the following things:
    -   A+W Enterprise 6 Frontend Config Tool: “Use SSH Connect” must be on “Yes”.
            o   Check whether the Unix computer name in the Config Tool is correct
    -   Open services of the Windows computer and check whether the FXSSHPROXY_AWE
        service is running. If necessary, restart the service.
        Caution: This closes all open sessions.
    -   Pings the Unix computer via the Windows CMD box.
            o   No ping possible, then check firewall in Windows and switch off for testing; a port
                release is necessary if this is the problem
    -   In the installation directory, check the alcib.frc to see whether the SSH proxy setting is
        active
            o   C:\Program Files (x86)\A+W\A+W Enterprise 6 Frontend\Config\alcib.frc
            o   “fxsshProxy” entry must be present and not commented out; that is, no ! in front
                of it
    -   Check %APPDATA%\A+W\A+W Enterprise 6 Frontend, to see whether there might be an
        old alcib.frc file. This file must be deleted since the alcib.frc from the installation folder
        overwrites. (old load)
    -   Important is that the port number range that is set in the proxy (Registry adjustment
        necessary - see screenshot) does not overlap with the port number range that is stored in
        the config -frc file. This is specified by an entry in the prog file that is used to start the
        programs.
SSH proxy settings:




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                 127
FIXWIN port range setting:




A+W Software GmbH            EN-CONFIG-A+W Enterprise System.docx   128
26.2.  Communication                              with         SN/SNLive               sketch
  generation
26.2.1.    No SN sketches are displayed/the iTOE cannot be
    started
"There is no SN instance."
"Cannot connect to SN"
Under some circumstances, there is a problem with the registration of the SN. SN must be
registered again.
To do this, open a console with Admin rights, change to the path of the SN installation (generally
C:\Program Files (x86)\A+W\Techsoft\SN) and issue the following command:
SN -regserver


OR:
An SN has gotten hung up (SN.exe) -> check in the Task Manager.


See also AWDesk #451384 and PF [AW-130212]




26.3.   Error message when starting the front end:
  Missing font: "Bitstream Vera Sans Mono"
A+W Enterprise Frontend Setup: Font "Bitstream Vera Sans Mono" is missing after installation
Occurs during the installation of the AWE front end on the Wernberg test system (customer-side)
with PF [AW-172587].
After the reinstallation of the font (copied from another system), the front end can be started
again.
The cause is still unclear.
The file " Bitstream Vera Sans Mono.ffi", which is stored in the directory C:\Program Files
(x86)\A+W\A+W Enterprise 6 Frontend\Config, seems NOT to be important for the installation
process. This file cannot be installed as Windows font.




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                               129
27. Subscriber
The subscriber is an A+W-internal help program for correcting FinAc and statistics bookings. The
application is documented in a separate internal document
SharePoint A+W Clarity R&D - Dokumente\Interfaces\Enterprise\FinAc Interfaces\General\ AWE
FinAc Info Intern.docx




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                            130
28. Connecting a Linux server for AWE with
 an Active Directory domain
The AD connection is made with the System Security Services Daemon (sssd). The associated
configuration is made according to the Red Hat instructions.
        https://access.redhat.com/solutions/1350723
In addition to the details in the instructions, in the file /etc/sssd/sssd.conf, the following lines
must be added in the
        [domain] block:
        [domain/<MyDomain>]
        …
        override_homedir = /alcib/usr/alcib
        override_gid = 501
Furthermore, the 32-bit RPM package 'sssd-client-<Version>.eIX.i686' and its dependencies must
be installed. (X = 6, 7 or 8 depending on the Red Hat version)
    •   cd <Mountpunkt_der_Setup-DVD>/Packages
    •   yum install sssd-client-<Version>.elX.i686.rpm
For security reasons, it is recommended that you give the directory /alcib/usr/alcib on the Linux
server and the files in it the owner 'root' and revoke the write rights for group and others.
    •   cd /alcib/usr/alcib
    •   chown root:alcib . .??* *
    •   chmod go-w . .??* *




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                  131
29. Keyboard
Within A+W Enterprise, we will talk every now and then about so-called A<n> keys. In the era of
different keyboards, this was a possibility for calling the keys the same thing for all keyboards.
Today, when only PC keyboards are in use, this is actually no longer necessary, but it shouldn't be
reworked everywhere. Therefore, here is the keyboard template used then.




e.g. bottom line
In the documentation and in texts/keys in the application, there is talk of DETAIL or <A5>. This
refers to the "F5" key on the PC keyboard.
The number that follows the "A" is the little number at the bottom corner on the template.
A1 – F4 / menu
A2 – STRG+F3 / Copy field content
A3 – F11 / Jump key
A4 – Shift-F6 / Insert record
A5 – F5 / Detail
A6 – F6 / Add record
A7 – F7 / Delete record
A8 – F8 / First record
A9 – F9 / Suggestions (SELO)


A10 – F10 / Last record
A12 - Shift+F9 / Extra 4
A13 - Shift+F10 / Extra 5
A14 - Shift+F11 / Extra 6
A16 – Shift+F1 / (User) help
A17 - STRG+F2 / Old field content
A18 – STRG+F1 / (Define user help) – Defining the user help function is no longer supported
A19 - Shift+F8 / Special 3


A20 - Shift+F12 / Special 4
A21 - CTRL+F4 / System menu
A22 - CTRL+F5 / Sort menu




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                               132
A30 – F2 / Mode
A31 - Shift+F3 / Print
A34- CTRL+F6 / Insert row
A37 - CTRL+F7 / Delete row
A38 – F1 / Help
A39 – F3 / Start


A42 - Shift+F7 / Delete field content
A43 – F12 / Field back
A51 - Shift+F4 / Menu
A55 - Shift+F5


A60 - CTRL+F8 / Special 1
A61 - CTRL+F12 / Special 2
A62 - CTRL+F9 / Extra 1
A63 - CTRL+F10 / Extra 2
A64 - CTRL+F11 / Extra 3
A80 - Shift+F2




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx   133
30. Archiving of documents
    •   How does the A+W Enterprise archiving work?
    •   What do you have to pay attention to during the configuration?
    •   Which environment variables, tables, files, and logs are involved?
    •   What problems do we know of`?




30.1.           Intention
A+W Enterprise archiving is used to save then delete old documents from the database. First, the
invoices and credit notes (and, if configured, quotes as well) to be saved will be written into a file.
This file can be saved on tape via SYSTEM > SAVE ARCHIVES. After this, the saved cases will be
deleted from the database. There is no way of retrieving deleted cases! The backup can be used
to print archived invoices/credit notes, however.


30.2.           Process
The archiving process is started via the crontab entry "db_archiv all" (alternatively via the "daily-
cron logic"). Crontab entries of the user alcibnet can be displayed with the command sunet
crontab –l.
This daily process first writes all records intended for archiving into the table archivstat. The
system will find all cases older than a defined number of days. This number can be entered in the
environment variable ARCHIV_INTERVAL. If this variable is not set, a default value of 180 days is
used; that is, all invoices/credit notes are archived that are older than 180 days.

After the documents to be archived are written to the table archivstat, the writing of the report to
the file $DBPATHEXT/rechsave/al_archiv.dat begins. The maximum number of documents that
are processed for each batch is specified by the variable MAXVORGDEL. If this variable is not set,
the default of 1000 applies, i.e. a maximum of 1000 invoices/credit notes can be written every
night. The data records processed are marked in the table archivstat with a flag
(archivstat.statflag=1).

The file al_archiv.dat thus grows larger each day and should be backed up on tape after a time.
This is done via menu SAVE SYSTEM/ARCHIVES. This dialog shows the number of documents to be
archived. Enter the tape drive (e.g. /dev/rStp0) and press START to save archives. Once the files
(al_archiv.dat et.) have been saved successfully, they will be deleted from the hard disk. At the
same time, the saved documents are marked for deletion in table archivstat
(archivstat.statflag=2).
These records are deleted from the corresponding ALCIB tables by means of program db_archiv.
Here, the maximum number of records to be deleted in a night are also controlled via the variable
MAXVORGDEL.

All deleted documents are written with the date of the back-up run (date of the tape back-up) in
the table rechsave. On the SYSTEM > ARCHIVINGDOCU dialog, the archived (deleted) documents


A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                134
are displayed with the date of the back-up run.

After the invoices/credit notes were deleted, all records connected to these documents are
deleted from the database (orders, item records, BOMs, texts, etc. => unreferenced deletion).
This is started via db_archiv.


30.3.           Configuration
After an update (to version > 2.7) or in case of a new installation, archiving must be configured
together with the customer. You need to define the time for which documents shall be kept in the
database (set ARCHIV_INTERVAL), and whether quotes shall be archived as well (set
ARCHIVEQUOTE to ON). Also, variable MAXVORGDEL should not be too high (e.g. 500).

Essential: Since archiving is properly set only a long time after an update or the original
installation, you should check whether the table archivstat already contains records before you
start the configuration. If this is the case, archiving must be completely reset. For this,:
1) All records from the table archivstat must be deleted completely.2) The files "al_archiv.*" in
the $DBPATHEXT/rechsav must be deleted.
If the archiving should initially be deactivated (e.g., because it is still unclear with which settings
the customer wants to work), this can be achieved by setting the variable ARCHIV_INTERVAL to a
very high value (e.g. 10000). Even then, the table archivdat and the files al_archiv.* should be
deleted.

When all settings were made, the service or project team should check during the following days
whether everything is processed correctly.


30.3.1.         Environment variables

ARCHIVANGEBOT : If set, quotations are also archived.

ARCHIV_INTERVAL: The number of days up to which old documents shall be archived.
                         (Default value: 180)

MAXVORGDEL: Maximum number of records to be archived or deleted at a time.
                (Default value: 1000)
ARCHIV_DEVICE : Tape drive on which back-up should be made (e.g., /dev/rStp0).



30.3.2.         Tables
        archivstat: Contains the records to be archived. This means:

        archivstat.statflag=0 => Just transferred to archiving
        archivstat.statflag=1 => Report written (in file al_archiv.dat)
        archivstat.statflag=2 => Document was saved on tape and can be deleted.


A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                135
        rechsave: Includes all already-deleted documents with date of the tape back-up.



30.3.3.         Files
        $DBPATHEXT/rechsave/al_archiv.dat => includes the written reports
        $DBPATHEXT/rechsave/al_archiv.idx => index file, with help of which individual invoices in
        the
        Rücksicherung einzelne Rechnungen in der
        al_archiv.dat can be found in case of a possible back-up.
        $DBPATHEXT/rechsave/al_archiv.sql => Sql-Skript that is executed when backing up of
        tape
        and triggers an update on archivstat.statflag.

        This files are backed up on tape when storing the archive and then deleted.



30.3.4.         Unreferenced deletion
The unreferenced deletion deletes the following data:
    •   All records from the table "kauf" where the fields auftrnr or aufnr contain the values 0 or
        NULL (defective records)
    •   All records for invoices and credits (document 7 to 10) from the table "kauf" that were
        not booked (fakturakz=0) and were not entered completely (subnr = 99).
    •   All records for not completely processed (no record in kaufedit) rack invoices (still=-40)
        from the table "kauf" that are older than 60 days (kauf.edat edat<(today-60)).


30.4.           Logs

Various log and error files are stored in $PROTOPFAD:
rechrep.prot => logs the writing of all reports to al_archiv.dat and the deletion
of documents after successful tape back-up.
rechrep.err => possibly occurring errors are logged here.
rechsv.* => can also include error messages.
urefdel.prot => log of the unreferenced deletion.
urefdel.err => error during unreferenced deletion.




30.5.           Known Problems
Disk is full
The file al_archiv.dat can reach an immense size after some time, and use up the entire disk. In
connection with this, the system may fail to archive documents correctly (transfer to file).


A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                 136
Archives should therefore checked from time to time, and saved on tape if necessary. If you
suspect that the file al_archiv.dat does not contain all archived documents (file too small), you
should completely reset archives (see above).



Archiving keeps on running during the day, and interrupts the normal work process
Usually, archiving is terminated by rebooting at the latest. Some customers do not boot at all at
night, or start archiving after rebooting in the evening. In this case, table locks (especially in
connection with unreferenced deletion) may interrupt processing.

Long transaction in case of unreferenced deletion
If too many documents are deleted at once, a long transaction may occur when the related item
records, BOMs, text, etc. are deleted. This means that the number of records to be deleted at
once is too high. To avoid this, the variable MAXVORGDEL should be as low as possible (e.g. 500).

Archiving takes ages
If there are very many records to be archived (e.g. because a customer is updated from 2.7 to a
newer version, and had done no archiving before), it may takes ages to transfer the records to
archivstat. A combined index in table archivstat may help. This index can be created by the
command: create index ix_archivstat1 on archivstat (orderno, document, subno) In version 2.12,
this index will be available by default.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                                 137
31. Platform change AIX – Linux
In addition to installation of the new binary files, the following points must also be checked and
adjusted if necessary.


31.1.           Scripts $0
In Linux, '$0' is handled a bit differently. There, it contains the full path. That's why in case
instructions there is no branching - as hoped - in the right case with the script name, but in the '*'
case, which can then cause endless recursion.
The solution is to reformulate the case instruction. Instead of "case $0 in" you have to write
"case `basename $0` in".
This adjustment can be made even before the conversion since the formulation
"case `basename $0` in"
is also correct under AIX.




31.2.           Environment variables
For Linux, two new environment variables must be activated (DFUE_TAR_CMD (Wert: 'tar cPf')
and DFUE_UNTAR_CMD (Wert: 'tar xPf')) if you are working with the EDI.




A+W Software GmbH                EN-CONFIG-A+W Enterprise System.docx                                138
32. Set-up of the CORE dump generation
      The following actions must be executed so that core dumps are generated in case of
      program crashes.
           •    In the file $FXDIR/fix.rc, the following entry must be present (attention!
                There may be no | before the line with fix_handled_signals):
                    o ! Signals handled by FIX:
                      !     Comma-separated             list     of      integer     values
                      fix_handled_signals: 1
           •    In $ACIBPRG/spec/usrdefs, the following entry must be added:
                    o ulimit -c unlimited > /dev/null 2>&1
               (Sometimes the entry has other parameters.)
                In /etc/profile, any existing entry with ulimit –c 0 must be removed.
           •    The directory $ALCIBPRG must have write rights for the group.
      After the set-up, the program must first be restarted; only after that as with a signal
      will a DUMP file be generated. This is normally in the directory $ALCIBPRG and
      bears the name core.<PID>.


With newer Linux systems, however, the abrt Deamon must be installed and activated. For this,
the following package is required:
       abrt-2.10.9-24.el8.x86_64 : Automatic bug detection and reporting tool
       Repo      : rhel-8-for-x86_64-appstream-rpms
The abrtd normally writes the dumps to the directory /var/spool/abrt/.




A+W Software GmbH              EN-CONFIG-A+W Enterprise System.docx                             139
33. Message boxes and their meaning
33.1.           Message 15048 in the order entry
The message text is "This document is locked by the background document processing
(<number>/<number>).
This means that the document that you currently want to load will not be processed by the A+W
Enterprise background processes - here "intauf". The first number specifies the type of processing
(kauf.still; aufint.still). For the significance of the individual still-flats, consult the database
documentation. The second number specifies how often the document has already been
processed - e.g., because it has encountered an error.
If the message appears permanently, A+W Enterprise service must check why the document
cannot be completed by the background process.




A+W Software GmbH               EN-CONFIG-A+W Enterprise System.docx                              140

