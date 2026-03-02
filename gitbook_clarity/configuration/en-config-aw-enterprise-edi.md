---
description: "EN CONFIG A+W Enterprise EDI"
---



# EN CONFIG A+W Enterprise EDI

    Configuration Instructions


A+W Enterprise EDI




                                     english




                             - -INTERNAL-
Change history

Date        Author            Comments                               Version
2018-02-15 Ina Seifert        Initial version                        1.0
                              6.8.19. Rabatte
                              Wenn die Umgebungsvariable
                              RABATTLOGIK_2005 aktiv ist, werden
                              die Vorgangsrabatte innerhalb der
                              Bestellübertragung NICHT übertragen.
                              Im Empfangshaus werden für den
2019-02-18 Alexander Weil                                            1.1
                              Auftrag die Rabatte für den Kunden
                              „Sendendes Haus“ neu aus den
                              Stammdaten ermittelt. Der Endkunde
                              des Auftrages wird dabei nicht
                              ausgewertet.
                              Standortübergreifende BDE
2019-06-12 Alexander Weil     6.8.5 SN-Datei Übertragung             1.2
2019-12-17 Alexander Weil     6.8.5 SN-Datei Übertragung - Upgrade   1.3
                              Product set transfer
2020-01-28 Ina Seifert
                              Private fields retained
2020-06-23 SVH                #422752 – A+W EDI Export
2020-09-16 Ina Seifert        E/Z rules for frame exchange
2020-12-15 Ina Seifert        Extension of MP interface
                              Format adjustment, receipt of goods
2022-05-06 Elena Tempelfeld
                              section inserted
09.10.2023 Ina Seifert        New message 95
2024-07-16 André Münch        Connection to Oxygen
                              [AW-169965] – PO export to A+W
2024-09-05 SVH
                              Business
                              Oxygen Change for Purchase Order and
2025-03-11 André Münch
                              Purchase Requisition
Content

1.   General                                                          11
     1.1. Overview of the supported transfer types                    11
     1.2. PO transfer vs. PO export                                   11
2.   Basic configuration                                              13
     2.1. Checklist                                                   13
     2.2. Table Xhaus                                                 13
          2.2.1. General                                              13
          2.2.2. Table structure                                      14
          2.2.3. Field description                                    15
     2.3. Directory structure / required files                        19
     2.4. Master data                                                 20
          2.4.1. Market partner                                       20
     2.5. Environment variables                                       20
     2.6. Housekeeping                                                25
3.   Error research                                                   27
     3.1. Reports                                                     27
          3.1.1. Article replication                                  27
          3.1.2. Market partner replication                           28
          3.1.3. Key replication                                      28
     3.2. Research options                                            28
          3.2.1. Status in the table intbest                          28
          3.2.2. -2041: Missing shipping address                      35
     3.3. Additional problems and their possible cause(s)Z            35
     3.4. Checking the transfer                                       38
4.   Purchase order generation                                        39
     4.1. Pure trade site                                             39
           4.1.1. Postponement                                        39
           4.1.2. Special checking of the environment variables       39
           4.1.3. Logs                                                40
     4.2. Environment variables                                       42
     4.3. Configuration Options                                       42
     4.4. PO grouping for direct orders                               43
     4.5. Delivery Address                                            44
           4.5.1. No direct shipment                                  44
           4.5.2. Direct shipment                                     44
     4.6. Document takeover                                           44
     4.7. Preventing deletion of the dispatch notification            45
     4.8. Entered by                                                  47
     4.9. Parallel order generation (case 174883)                     47
     4.10. Shipping information                                       48
     4.11. Spacer and muntin orders                                   48
           4.11.1. Basic information                                  48
           4.11.2. Dimensions                                         49
           4.11.3. AIR                                                49
     4.12. Breakage orders                                            49
           4.12.1. Reject place                                       50
           4.12.2. Reject per labels                                  50

A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx        3
           4.12.3. Missing breakage type from A+W Production                               51
     4.13. Site-spanning PDC                                                               51
     4.14. Complaint details                                                               51
     4.15. Discounts                                                                       51
     4.16. Error research                                                                  51
5.   Order linking                                                                         53
     5.1. Introduction                                                                     53
     5.2. Master data                                                                      53
          5.2.1. Configuration Options                                                     53
          5.2.2. Distributor                                                               55
          5.2.3. Production site                                                           55
          5.2.4. Process                                                                   55
          5.2.5. SN File Transfer                                                          57
6.   PO transfer                                                                            58
     6.1. Introduction                                                                      58
     6.2. Master data                                                                       58
          6.2.1. Configuration Options                                                      58
          6.2.2. Item master data                                                           60
          6.2.3. Distributor                                                                60
          6.2.4. At the production site                                                     60
     6.3. Process                                                                           61
     6.4. Release of transfer - Version 2007 up to AWE6 October 2024                        61
     6.5. Flexible control of the direct transfer                                           62
     6.6. Local correction (DFUE_IB_BESTELLSPERRE)                                          63
          6.6.1. DFUE_IB_BESTELLSPERRE = OFF                                                65
          6.6.2. Direct order yes and direct transfer yes                                   65
          6.6.3. Direct order yes and direct transfer no                                    66
          6.6.4. Direct order no and direct transfer yes                                    67
          6.6.5. Direct order no and direct transfer no                                     68
          6.6.6. DFUE_IB_BESTELLSPERRE = 0 when printing                                    68
          6.6.7. Direct order yes and direct transfer yes                                   68
          6.6.8. Direct order yes and direct transfer no                                    69
          6.6.9. Direct order no and direct transfer yes                                    70
          6.6.10. Direct order no and direct transfer no                                    70
          6.6.11. DFUE_IB_BESTELLSPERRE =1 when sending                                     71
          6.6.12. Direct order yes and direct transfer yes                                  71
          6.6.13. Direct order yes and direct transfer no                                   72
          6.6.14. Direct order no and direct transfer yes                                   72
          6.6.15. Direct order no and direct transfer no                                    73
          6.6.16. DFUE_IB_BESTELLSPERRE =2 receipt for the scheduling in the receiving site
          booked in the sending site                                                        74
          6.6.17. Direct order yes and direct transfer yes                                  74
          6.6.18. Direct order yes and direct transfer no                                   74
          6.6.19. Direct order no and direct transfer yes                                   75
          6.6.20. Direct order no and direct transfer no                                    76
          6.6.21. DFUE_IB_BESTELLSPERRE =3 PMS- receipt for the production scheduling in the
          receiving site booked in the sending site                                         76
          6.6.22. Direct order yes and direct transfer yes                                  77
          6.6.23. Direct order yes and direct transfer no                                   77


A+W Software GmbH               EN-CONFIG-A+W Enterprise EDI.docx                                4
           6.6.24. Direct order no and direct transfer yes                                  78
           6.6.25. Direct order no and direct transfer no                                   79
           6.6.26. DFUE_IB_BESTELLSPERRE =4 PMS- fixed via the production job creation in the
           receiving site booked in the sending site                                        80
           6.6.27. Direct order yes and direct transfer yes                                 80
           6.6.28. Direct order yes and direct transfer no                                  81
           6.6.29. Direct order no and direct transfer yes                                  81
           6.6.30. Direct order no and direct transfer no                                   82
           6.6.31. DFUE_IB_BESTELLSPERRE =5 PMS- released via the production job confirmation
           in the receiving site booked in the sending site                                 83
     6.7. Cancellation – Version 2007                                                       84
     6.8. Special features of program behavior                                              84
           6.8.1. Changes in the order/PO after successful PO transfer                      84
     6.9. Functional range                                                                  86
           6.9.1. Determination of the order number at the production site (iboffset, own number
           range) 86
           6.9.2. Route finding                                                             86
           6.9.3. Free customer orders                                                      87
           6.9.4. Document transfer - Version 2007                                          87
           6.9.5. SN File Transfer                                                          89
           6.9.6. References - Version 2007                                                 90
           6.9.7. Customer PO number (kauf.exaufnr)                                         91
           6.9.8. Private fields                                                            92
           6.9.9. Configurable document fields                                              92
           6.9.10. Fixed private fields in the order header (kauf._private_*)               92
           6.9.11. Report for delivery date shifts at the production site                   92
           6.9.12. Shipping information                                                     94
           6.9.13. Entered by                                                               95
           6.9.14. Prices PU becomes SA                                                     95
           6.9.15. Supply types                                                             96
           6.9.16. Supplier for supply type "PO"                                            96
           6.9.17. Objects                                                                  97
           6.9.18. Text                                                                     97
           6.9.19. written back                                                             97
           6.9.20. Site-spanning PDC                                                        97
           6.9.21. Exchange/addition rules                                                  98
           6.9.22. Complaint details                                                        98
           6.9.23. Setting of the kauf.org* fields                                          98
           6.9.24. Spacer reduction (SR)                                                    99
     6.10. Environment variables                                                            99
     6.11. Error handling                                                                  100
7.   Generating suborders                                                                101
     7.1. Function Description                                                           101
     7.2. Configuration                                                                  101
     7.3. Process                                                                        101
     7.4. Error handling                                                                 101
8.   Order shifting                                                                      102
     8.1. Test system                                                                    102
          8.1.1. General configuration                                                   102


A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                 5
          8.1.2. General deviating functionalities                                 103
9.   Invoice transfer                                                              106
10. Product set transfer                                                           107
11. Change log (kaufedit)                                                          108
12. Status reporting from the production client                                    109
    12.1. Triggering status transfer for internal client separation                109
    12.2. Reports                                                                  109
    12.3. Configuration                                                            109
    12.4. Status overview                                                          110
    12.5. Status 206 – postponement of delivery date                               110
    12.6. Status(503): Transfer to the production site                             110
    12.7. Status(551): Order scheduled in production                               110
    12.8. Status(552-556): Order in production                                     111
    12.9. Status(307): Order packed                                                111
    12.10.     Status: Order dispatched                                            111
    12.11.     ADHOCSQL for determination of production information for internal
    reference orders                                                               111
    12.12.     Message on PO date postponement                                     112
13. Balance scheduling                                                             113
    13.1. Structure of the salden.dat file                                         113
    13.2. Default flow                                                             114
    13.3. Internal client separation (AWD #388239)                                 114
    13.4. Update of the totals by the AWE FinAc Service                            114
    13.5. Logs                                                                     115
    13.6. Problem handling                                                         115
          13.6.1. Totals are not stored                                            115
          13.6.2. The value in fibu_op does not match salden.dat                   115
          13.6.3. Error: data for client X instead of for Y                        116
14. Messages                                                                       117
    14.1. Overview                                                                 117
          14.1.1. Report 22 (article replication)                                  118
          14.1.2. Message 31                                                       119
          14.1.3. Message 50                                                       120
          14.1.4. Message 51                                                       120
          14.1.5. Message 55                                                       120
          14.1.6. Message 67                                                       121
          14.1.7. Message 95                                                       121
          14.1.8. Old reporting system (ibin.meld)                                 121
15. External Order Interface/EDI import                                            123
    15.1. Introduction                                                             123
    15.2. Checklist                                                                123
    15.3. Configuration – AWE master data                                          124
    15.4. General procedure                                                        124
    15.5. File processing                                                          125
    15.6. Item implementation / Product referencing                                129
          15.6.1. Default data and prefixes (table exbartyp)                       129


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                      6
     15.7. Article assignment / article implementation                                        132
           15.7.1. Evaluation of the replacement/addition rules                               134
     15.8. BOM change                                                                         138
           15.8.1. Customer-specific BOM change                                               140
     15.9. Special order interfaces                                                           141
           15.9.1. Default order interface i000filter                                         141
           15.9.2. Kermi order interface                                                      142
     15.10.      Product sets                                                                 142
     15.11.      Configuration Options                                                        143
           15.11.1. Parallel processing                                                       143
           15.11.2. Templates                                                                 146
           15.11.3. Exchange/addition rules for spacer exchange                               147
           15.11.4. Invoice address                                                           148
           15.11.5. Restriction violations                                                    148
           15.11.6. Post-processing                                                           148
           15.11.7. Release                                                                   148
           15.11.8. Packing type                                                              149
           15.11.9. Dimensional precision                                                     149
     15.12.      Error handling                                                               150
           15.12.1. Missing item dimensions                                                   150
           15.12.2. File is not imported - no error message                                   150
           15.12.3. Missing orders from a file with several orders                            151
     15.13.      Test function external standard interface (under construction)               152
           15.13.1. Configuration                                                             152
           15.13.2. Process                                                                   155
           15.13.3. Log                                                                       156
     15.14.      Environment variables                                                        156
16. PO export / A+W EDI export                                                                 159
    16.1. Activation                                                                           159
    16.2. Installation                                                                         159
          16.2.1. A+W Enterprise B2B Service                                                   159
          16.2.2. AWE back end and database                                                    160
    16.3. Configuration                                                                        160
          16.3.1. Market partner master data                                                   160
          16.3.2. External customer number                                                     160
          16.3.3. Configuration of settings across suppliers and supplier-specific export settings
                  161
          16.3.4. Stored Procedures                                                            163
          16.3.5. Country code                                                                 165
    16.4. Overview of flow                                                                     166
          16.4.1. Initiation through entry in the table ottransfer                             166
          16.4.2. Processing by the B2B Service                                                166
    16.5. Transfer table ottransfer                                                            166
          16.5.1. Back-up table ottransferok                                                   167
    16.6. Imperial measurements                                                                167
    16.7. Export to A+W Business                                                               167
          16.7.1. Configuration of the sending market partner in A+W Business                  167
    16.8. Data Mapping                                                                         167
    16.9. Generation of the export file                                                        167
          16.9.1. Basic configuration                                                          168


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  7
           16.9.1. Overwriting of the basic configuration                          168
           16.9.2. Placeholders (wildcards) in the file paths                      170
           16.9.3. Placeholders (wildcards) in file names                          170
           16.9.4. Housekeeping                                                    171
     16.10.     Special explanations for the export logic in the AWE B2B service   171
           16.10.1. Language                                                       171
           16.10.2. Product Types and Product Groups                               171
           16.10.3. Export of articles                                             171
           16.10.4. Export of shapes                                               172
           16.10.5. Export of muntins                                              172
           16.10.6. Export of steps                                                172
           16.10.7. Export of gas                                                  173
           16.10.8. Export of processings (B1 record)                              173
           16.10.9. Export of item texts (T1 - record)                             173
           16.10.10. Export of attached files (DL and PL record)                   173
     16.1. Sending e-mails                                                         174
     16.1. Logging and research                                                    174
17. Order import (intauf)                                                          175
    17.1. Introduction                                                             175
    17.2. General procedure                                                        175
    17.3. Functional range                                                         175
          17.3.1. Logic for distribution of the order imports                      175
    17.4. Environment variables                                                    175
18. Master data replication                                                        177
    18.1. Checklist                                                                177
    18.2. Basic principles for all replications                                    178
    18.3. Special feature of internal site separation                              179
    18.4. Configuration                                                            179
          18.4.1. Table xhaus                                                      179
    18.5. Logs                                                                     179
          18.5.1. Log database table                                               179
          18.5.2. Article replication                                              180
          18.5.3. Key replication                                                  181
          18.5.4. Market partner replication                                       181
    18.6. Market partner replication                                               181
          18.6.1. Table xhaus                                                      181
          18.6.2. Tables, triggers, and stored procedures                          181
          18.6.3. Configurable fields                                              183
          18.6.4. Plausibility check                                               183
    18.7. Article replication                                                      184
          18.7.1. Table xhaus                                                      184
          18.7.2. Trigger – Stored Procedure – Tables                              184
          18.7.3. Tables to be transferred                                         187
          18.7.4. Local tables                                                     188
          18.7.5. Special features for tables                                      189
          18.7.6. Local fields                                                     194
          18.7.7. Foreign-language subsidiaries                                    194
          18.7.8. Article description as local field                               194
          18.7.9. Replication of the foreign-language article description          195


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                      8
          18.7.10. Plausibility check                                                       196
          18.7.11. Transaction logic                                                        196
          18.7.12. Master data maintenance                                                  196
          18.7.13. Environment variables                                                    196
          18.7.14. Error research                                                           198
    18.8. Key replication                                                                   198
          18.8.1. Table xhaus                                                               199
          18.8.2. Installationsscript prep_keyreplication                                   199
          18.8.3. Table replichaus                                                          200
          18.8.4. Table replictab                                                           201
          18.8.5. Special logic alenv table (#377840)                                       202
          18.8.6. Creating the tables, triggers, and stored procedures without prep_keyreplication
                  204
          18.8.7. Required tables (rp_table)                                                204
          18.8.8. Required stored procedures (SP)                                           206
          18.8.9. Required triggers                                                         207
          18.8.10. Deleting data records                                                    208
          18.8.11. Troubleshooting                                                          208
19. External market partner interface                                                      210
    19.1. Interface structure                                                              210
    19.2. Environment prerequisites                                                        214
    19.3. Restrictions of the interface                                                    216
    19.4. Interface table                                                                  217
    19.5. Process                                                                          217
          19.5.1. Log                                                                      217
    19.6. Local fields/Transfer of 0 values                                                218
          19.6.1. Resetting numeric values to 0 (default) (case 185124)                    218
          19.6.2. Local fields for active env variable DFUE_MPDFUE_IGNORE_FLD1             218
          19.6.3. mp.sprkz as local field                                                  218
    19.7. Address logic                                                                    219
          19.7.1. New address logic                                                        219
          19.7.2. Standard shipping address                                                220
          19.7.3. Post box postal code/post box (cf. 173629)                               220
    19.8. Handling of special fields                                                       220
          19.8.1. Ignore change code – Field 1                                             221
          19.8.2. Market partner number field 2                                            221
          19.8.3. Changed referencing                                                      221
          19.8.4. Country (fields 12 and 13)                                               221
          19.8.5. Company limit / Assu. limit– field 19 / 97                               222
          19.8.6. Currency – field 21                                                      222
          19.8.7. Discount condition (SkontoX) – fields 22 / 118 / 119                     222
          19.8.8. Sales revenue representative - field 33                                  224
          19.8.1. Active flag (mp.still) - field 34                                        224
          19.8.2. Delivery stop – field 86                                                 225
          19.8.1. Invoice stop – field 87                                                  225
          19.8.2. Bank account – field 101, 108                                            225
          19.8.3. Entry stop - field 112                                                   226
          19.8.4. Market partner – group assignment – field 113                            226
          19.8.5. Department – field 120                                                   227
          19.8.6. Cost center – field 121                                                  227


A+W Software GmbH               EN-CONFIG-A+W Enterprise EDI.docx                                    9
     19.9. Control possibilities (environment variables)                              228
     19.10.     Descriptions of problems                                              231
           19.10.1. Empty file                                                        231
           19.10.2. Load failed                                                       232
           19.10.3. Local fields are not considered                                   232
20. Status reporting from financial accounting                                        233
21. Receipt of goods                                                                  234
    21.1. Incoming goods inspection                                                   234
    21.2. External receipt of goods (e.g. SAP)                                        234
          21.2.1. Configuration                                                       234
          21.2.2. Process                                                             235
          21.2.1. Housekeeping                                                        237
          21.2.1. Interface structure                                                 237
          21.2.2. Log                                                                 238
22. SAP Oxygen coupling                                                                240
    22.1. General                                                                      240
          22.1.1. General switch (alenv)                                               240
          22.1.2. Tables                                                               240
          22.1.3. Stored Procedure "cu_sgg_generic_material"                           241
          22.1.4. Stored Procedure "cu_sgg_wlraumtosap"                                242
          22.1.5. Stored Procedure „ cu_sgg_wlraum “                                   242
    22.2. Import of customers and suppliers                                            242
    22.3. Import of stock POs                                                          242
    22.4. Import of articles and variants                                              242
    22.5. Export of purchase orders                                                    242
    22.6. Export of orders                                                             243
          22.6.1. Creation of the cost carrier (WBS)                                   243
          22.6.2. Transfer of the orders                                               243
    22.7. Export of delivery notes                                                     243
    22.8. Export of invoices and credit notes                                          243
    22.9. Export of receipt of goods                                                   244
    22.10.     Export of stock transactions and finished messages                      244
          22.10.1. Stock correction and stock correction takeback (type 551 + 552)     244
          22.10.2. Inventory (differences) (type 711 + 712)                            244
          22.10.3. Rebookings (type 301)                                               245
          22.10.4. Stock removal for order (type 291)                                  245
          22.10.5. Receipt of goods by production in dispatch warehouse (type Z01 + Z02)245
    22.11.     Export of PO wishes                                                     246
    22.12.     Export of cost records                                                  246




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                           10
1. General
Frequently, there is a desire for a company-wide, central master data management, automatic
order processing within a company with several branch offices, and automatic order scheduling
for external orders.
A+W Enterprise provides special transfer functions that allow these various requirements to be
fulfilled.
Central components of all transfer are the program trm_ctrl and the table xhaus, which includes
all necessary information about the clients for data exchange.
Without trm_ctrl (but with the table xhaus), only the online master data replication and the goods
receipt and invoice transfer work.




    1.1.         Overview of the supported transfer types
    •   Master data replication (article, market partner, key, product sets)
    •   Transfer of Orders and Purchase orders
    •   Transfer of External purchase orders
    •   Takeover of incoming goods and purchase invoices for existing orders
    •   Reporting of order status values
    •   Distribution of messages
    •   Transfer of invoice data to external FinAc systems




    1.2.         PO transfer vs. PO export
What are the basic differences between internal PO transfer and PO export?


Function/area                      Internal PO transfer             PO export
Article master data                Must be identical between the    Different item master data
                                   two clients.
                                   Rudimentary evaluation of the
                                   replacement/addition rules
Item referencing                   Does not take place              Takes place via customer
                                                                    article and
                                                                    replacement/addition rules
Status reports                     Detailed status messages from    No status reports
                                   the production site.



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                              11
Local correction    Configuration via            Configuration via
                    DFUE_IB_BESTELLSPERRE        BESTELLFREIGABE
Program file        trm_ctrl                     Export: A+W B2B Service
                                                 Import: i000filter; trm_ctrl




A+W Software GmbH   EN-CONFIG-A+W Enterprise EDI.docx                           12
2. Basic configuration
    2.1.        Checklist

Housekeeping                      Individual script for cleaning up individual directories, especially
                                  also $DFUEDIR/proto/*
Tabelle xhaus                     Versions check/set all clients.
                                  bytevektor check/set all clients.
                                  This must be set correctly in the sender and in the recipient.
Directory structure               $DFUEDIR
                                  The subdirectory $DFUEDIR/proto/<Mandant> is important
Market partner master data        Type of the EDI/direct order
Connection (FTP)                  It's important that alcibnet has the right for ftp on the
                                  xhaus.host of the other sites.
PMSPURCHASETRIGGER                Has to be set if this is purely a distributor.




    2.2.        Table Xhaus
        2.2.1.           General
In the table xhaus, data for all clients that communicate with one another via A+W Enterprise is
saved.
xhaus can thus be called a site management table from which A+W Enterprise draws all data
required for communication.
In all connected sites, the table xhaus must be maintained accordingly. Sites that are not entered
in the table xhaus are not available to the system for automatic data exchange.
After each change to the table xhaus, the ue_server and the dfue_starter must be ended and
started again.
Special attention must be paid to the correct creation of the fields kunr, linr, host, hausart, vers,
subvers, and patch, as well as iboffset, bytevektor, and dfuedirpath since these have a central
effect on order linking and PO transfer.
In all sites participating in the order linking and PO transfer, the table xhaus must be adjusted
accordingly.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                     13
      2.2.2.         Table structure
No.   Table field    Description                            Reference to remarks   from
                                                                                   version
1     haus           Number of the site/sub-site            haus                   < 4.0
2     hnr            Number of the site/sub-site            hnr                    < 4.0
3     hname          Short name for the site                hname                  < 4.0
4     kunr           Customer number of the site            kunr                   < 4.0
5     linr           Supplier number of the site            linr                   < 4.0
6     host           Host name of the server                host                   < 4.0
7     hausart        Flag for evaluation of iboffset and    hausart                < 4.0
                     environment variables
8     vers           ALCIB Version                          vers                   < 4.0
9     subvers        ALCIB Subversion                       subvers                < 4.0
10    patch          ALCIB Patch                            patch                  < 4.0
11    dbart          Flag for replication                   dbart                  < 4.0
12    region         Region affiliation                     region                 < 4.0
13    socketmd       SOCKETMD from alenv                    socketmd               < 4.0
14    shmoffset      Shared memory offset of the site                              < 4.0
15    servmaster     Name of the computer on which the                             < 4.0
                     server processes are running
16    netz           Network recognition                                           < 4.0
17    sprkz          Local language of the site                                    < 4.0
18    informixserv   Name of the Informix server            informixserver         < 4.0
      er
19    iboffset       Offset of the document numbers of      iboffset               < 4.0
                     the site
20    bytevekt       Byte vector flag                       bytevekt               4.0
21    dfuedirpath    EDI directory of the site              dfuedirpath            4.2
22    hauptmanda     Client ID within the internal client   hauptmandant           4.2
      nt             separation
23    clientlocale   Value of the CLIENT_LOCALE system      clientlocale           4.4
                     variables of the site
24    vers_seqnr     AWE database version of the            vers_seqnr             6.0
                     corresponding client




A+W Software GmbH              EN-CONFIG-A+W Enterprise EDI.docx                         14
        2.2.3.           Field description
haus
Number corresponds to the system variables $HAUS (site)
hnr
At least since Version 4.0, haus and hnr are always assigned the same value (the site number). In
older versions, these values can deviate from one another.
hname
Name of the site. This is displayed, among other things, on the title line of the A+W front end. In
addition, it can be displayed in the subject line of system e-mails (ALMAIL_MANDANT_BETREFF)
or for the establishment of the mail domain server (AWMAIL_XHAUS_DOMAIN).
kunr
The number corresponds to the customer number in the market partner master data. A site's
customer number should be identical in all sites.
If a company has 3 branch offices in Berlin, Dresden, and Munich, the Berlin branch office should
be kept with the same customer number in the Dresden branch office as in Munich. It is possible
to deviate from this recommendation, but the result is more configuration and management
work. (see environment variable IB_KUEMPF).
Depending on the configuration, this number is also used to determine the sender address for the
form dispatch. See section "Determination of the sender address" in "EN-CONFIG-A+W Enterprise
Print Service"
linr
The number corresponds to the supplier number in the market partner master data. A site's
supplier number should be identical in all sites. The supplier number is used within the order
coupling and the PO transfer as well as internal accounting and automatic goods receipt
generation. In particular in the course of internal accounting, there can be problems if the
supplier numbers are not unique company-wide.
QR 2406:
The supplier number is also used in the course of "XRechnung" to identify the seller. If you want
to work with "XRechnung" but not with internal EDI, the supplier number can also be entered
negative.
"XRechnung" see "EN-CONFIG-A+W Enterprise B2B Service"
host
Host name of the server on the network on which the site was installed and to which the transfer
files should be sent.
hausart
For installations, the field is always assigned 10 or 11.
The difference between 10 and 11 lies in the evaluation of the field iboffset. With hausart=11, the
field is not evaluated.
Site types between 0 and 10 are no longer supported and will cause errors.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  15
vers
Version number (for example 4 in Version 4.3.2)
All version fields must be set correctly in all participating sites. E.g.
Site 1 and site 2 work with internal order transfer
Site 1 works with Version 4.5.1
Site 2 works with Version 6.0.4
In site 1:
In the xhaus record for site 1, vers=4;
In the xhaus record for site 2, vers=6;
In site 2:
In the xhaus record for site 1, vers=4;
In the xhaus record for site 2, vers=6;
subvers
Subversion (for example, 3 in Version 4.3.2)
All version fields must be set correctly in all participating sites. E.g.
Site 1 and site 2 work with internal order transfer
Site 1 works with Version 4.5.1
Site 2 works with Version 6.0.4
In site 1:
In the xhaus record for site 1, subvers=5;
In the xhaus record for site 2, subvers=0;
In site 2:
In the xhaus record for site 1, subvers=5;
In the xhaus record for site 2, subvers=0;


patch
Patch (for example, 2 in Version 4.3.2)
All version fields must be set correctly in all participating sites. E.g.
Site 1 and site 2 work with internal order transfer
Site 1 works with Version 4.5.1
Site 2 works with Version 6.0.4
In site 1:
In the xhaus record for site 1, patch=1;
In the xhaus record for site 2, patch=4;
In site 2:


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx       16
In the xhaus record for site 1, patch=1;
In the xhaus record for site 2, patch=4;


dbart
ID for the master and client database for item, market partner, and key replication.
2 – Country or sub-master database for 2-stage master-client logic
1 – Master database
0 – Client database
-99 – Pseudo site (not a regular site)
- is required as price client for internal client separation starting with version AWE 6.
- is used as pseudo site for self-transfer (environment variable IBHAUS)
- Used as pseudo client for several call centers due to multilingualism (capacitative client
assignment) – work in process
- For these sites, no background processes are started.
- One employee-client assignment is possible


The value "2" for sub-master only plays a role in the sub-master itself. It identifies for itself that
dbart=2 is entered in its xhaus record.
Example:
The sites 70, 80, and 90 exist.
90 is master (for site 80)
80 is sub-master (for site 70)
70 is "only" client
xhaus entries in site 90:
    •   haus 90, dbart 1
    •   haus 80, dbart 0
    •   haus70, dbart 0


xhaus entries in site 80:
    •   haus 90, dbart 1
    •   haus 80, dbart 2
    •   haus70, dbart 0


xhaus entries in site 70:
    •   haus 90, dbart 0



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                     17
    •    haus 80, dbart 1
    •    haus70, dbart 0


region
The association of a site with a region is evaluated, e.g. in the FinAc interface.
Socketmd
The respective SOCKETMD of the client from alenv. Important for central number assignment.
shmoffset
         Shared memory offset of the site
Servmaster
Name of the computer on which the server processes are running Important for central number
assignment.
Netz
Network detection
sprkz
Language ID (local language of the site)
Informixserver
Name of the database server on the net. This is required for the master data replication.
Order entry also uses this for the database access.
iboffset
If iboffset is greater than 0, then the new order number for documents that are sent by this site
via order linking or order EDI is the document number sent plus iboffset.
bytevekt
If the site works with byte or bit vectors (1 - byte vector => environment variable BYTE_VEKTOR is
set).
dfuedirpath
The value of $DFUEDIR for the corresponding site is set. If the field is not filled, it is assumed that
the directory is identical with $DFUEDIR of the sender.
Important is the maintenance of this field if EDI should take place between Windows sites and
UNIX sites or between 2 Windows sites on different installations. The path for the Windows sites
must be entered in SFU notation.
hauptmandant
The field must be maintained due to the internal site logic.
If the value stored here is equal to hnr, it is a main site.
If the value stored here is not equal to hnr, but is greater than 0, it is an internal site whose main
site is specified in this field.
The main site defines the database name (alcib_<hauptmandant>)



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                     18
For pseudo sites (e.g., IBHAUS) for which no background processes, especially no ctrl_server must
run, a 0 must be entered here.
See case 135188
All xhaus entries with the same main client will be updated accordingly with a QR update (version
information). If there is something incorrect here (e.g, in preparation for a future move or
because you just copied another record), it can happen that an internal EDI no longer works after
a QR update.


A+W Enterprise 6: Apparently now for the Singlesite_Installations the main client must be set
equal to the client number so that the order entry works.


clientlocale
The valid Informix client country setting must be saved for each site entered. With internal EDI, a
code set conversion is done if necessary using this data.
In the new field clientlocale of the table xhaus, the CLIENT_LOCALE value of the appropriate site
must be stored (upper and lower case plays no role).
If no value is stored for a site in xhaus.clientlocale, the EDI assumes that conversion should be to
the code set ISO8859-1.
See case 168856
vers_seqnr
The EDI must know in the respective client which database structure exists in the site
connected via EDI. Since database changes are no longer attached solely to the A+W
Enterprise Version (fields vers,subvers, and patch), there is now another field vers_seqnr.
The seqnr of the last SQL file listed on the database is entered in this field. Therefore, it is
important that the SQL scripts are always executed seamlessly in the correct sequence.
This information controls central functionalities within the internal document transfer.
The update routine tries to update these values for accordingly all relevant xhaus entries.
For this, however, it is necessary that all databases be available to one another for SQL
commands. If this is not the case, the update must be done manually after an update.
After each change to the table xhaus, the ue_master (or ue_server) and the dfue_starter must
be ended and started again.


    2.3.        Directory structure / required files
    •   In the directory $DFUEDIR/ proto (e.g. /usr1/alcibnet/proto), there must be a
        subdirectory that has the same name as the site number (xhaus.haus) for each site
        participating in the transfer (also internal sites!). For single-digit site numbers, a 0 must be
        placed in front of the directory name (e.g. site 2 => directory $DFUEDIR/proto/02) This
        subdirectory must have write and read rights for the user alcibnet.
    •   In the directories $DFUEDIR/dat (e.g. /usr1/alcibnet/dat) and $DFUEDIR/wait (e.g.
        /usr1/alcibnet/wait ) there must be one subdirectory per .testmount (the dot is



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                   19
        important). Parallel to the directory $DFUEDIR/wait, there must also be a subdirectory
        $DFUEDIR/waitx. All directories must have write rights for the user alcibnet.
    •   In the directory /usr1/alcibnet/bin there must be an appropriate file
        trm_ctrl_<mandantennummer> for each site participating in the transfer. This file must
        be created as a link to the file trm_ctrl_<haus>.
    •   To enable a transfer between 2 servers, the file .netrc must have a corresponding entry
        for the user alcibnet in the directory /usr1/alcibnet.
    •   In the directory $ALCIBPRG/cmd, there must be a script "FT". It must be possible to
        execute the script with the user alcibnet.
    •   It must be possible to execute the system commands compress / uncompress, uuencode /
        uudecode and tar from alcibnet.
    •   The database settings DBDATE and DBMONEY must be identical for all participating sites.




    2.4.        Master data
        2.4.1.           Market partner
Within the market partner (xhaus.linr, xhaus.kunr) the field "Type of the EDI" and the field "Direct
order" must be set accordingly.
Direct order "yes" means that the order is generated immediately and not via the order pool.


    2.5.        Environment variables
DFUE_IB_BESTELLSPERRE (version 2007):
The variable controls when internal POs go into local correction.
0 - print; 1 - send; 2 - receipt; 3 - scheduling; 4 - job created; 5 - job confirmed


DFUE_IB_OWN_AHAM (client reference: no)
For the internal DFUE it is assume that the item master data is identical in its essential properties.
Therefore, the AHAM is transferred unchanged by default. To achieve that the local SR is used in
the receiving site and the dependent data (spacer and muntin size) is recalculated, the variable
must be activated. ID 134840
The logic works starting with Version 4.2 also for triple and quadruple IG, see case 204646.
This function may not be configured together with an MD_MIN_AHAM.
DFUE_PROTO_NOBUFF
Normally for performance reasons, the EDI logs are written buffered. This can mean that with
crashes due to program errors, not all messages are found in the log. With the setting of these
variables, all logs of the EDI are written unbuffered. For differentiated treatment, see
DFUE_RESEARCH.



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 20
DFUE_RESEARCH
With these variables, various research modes of the trm_ctrl can be switched on. Up to 10 areas
are separated by | (pipe)Currently available:
trm_ctrl
ibout – export of the data (also for PO generation) to the distributor
        – Protocol $DFUEDIR/proto/[<hausnr>/ibout>/]ibout*

ibin     – storage of the data (also PO generation and external EDI)
         – Protocol $DFUEDIR/proto/[<hausnr>/ibin/]ibin*

filter   – reading in of external interfaces via interface filter (external EDI)
         – Protocol $DFUEDIR/proto/[<hausnr>/edi/]<filter>*

mp_replicate     – Market partner replication
                 – Protocol $PROTOPFAD/MP_replic<mmdd> (in client)

art_replicate    – Article replication
                 – Protocol $PROTOPFAD/ArtReplik_replic<mmdd> (im Client)
rechrueck        – report from financial accounting
                 - Log $PROTOPFAD/Rechrueck_<mmdd>_<hhmm>
rueck, mp,


fibu, ibi_unl - moves unload files of the _i-tables to $DFUEDIR/proto
ibout_unl: moves unload files of the _-tables to $DFUEDIR/proto/unl_ .res ATTENTION:
ON: extended recording for all EDI areas.
If this variable is set, the log for this area will be unbuffered (s.a. DFUE_PROTO_NOBUFF,
REPLICATE_PROTO)


DFUE_TRM_SIMULTAN
Simultaneous trm_ctrl for external order scheduling and PO generation.


IB_ALLOWIB (client reference: no)
Allow orders to your own site via pseudo supplier. In addition, the environment variable
IBHAUS has to be activated (see section "generating suborders")


IB_DFUE_NACHBEARB (data transfer)
From trm_ctrl, after booking an entry, a script is started with set variables. Here, another script
can be called per order customer (kauf.kunr). The definition is stored in the table
dfue_nachbearb. The script itself must be in $ALCIBPRG/cmd or $ALCIBPRG/spec/cmd.
Parameter paknr,exaufnr,auftrnr,hausnr,parhausnr
Is overwritten for external order scheduling of EDI_SQL.


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                 21
If with external EDI neither of the two variables is set but there is an entry in dfue_nachbearb,
then the reprocessing is done.
Attention: see "Post-processing" section


IB_EXREF (client reference: no)
The variable influences the structure of kaufexaufnr (external reference) for the document
transfer (NOT for order generation!)
  0: exaufnr=auftrnr sender's order no (PO number for PO EDI)
  1: exaufnr=bestnr the sender's PO number appears at the target site
  2: exaufnr=auftrnr/bestnr both numbers appear at the target site
  3: exaufnr=bestnr/auftrnr both numbers appear at the target site

  4: exaufnr is transferred unchanged
  Caution: not set or 0 corresponds to the previous logic (see also PILK_51922)


IB_EKVK_SHIFT
For the internal order transfer, it is also possible by setting this variable that one of the price fields
of the original order from poskost is written to kpos.dfuenstpreis and transferred. The name of
the field to be used has to be entered in the variable; the only valid fields are "stkprs" and
"stkprsfw." With entry of "nstpreis," kpost.nstpreis is written to kpos.dfuenstpreis and
transferred.


IBHAUS (client reference: no)
Site number from xhaus for the internal pseudo suppliers for production suborders. The client
number may not be the same as the own client number.
In addition, the environment variable IB_ALLOWIB has to be activated. (see section "Generating
suborders")


IB_KUEMPF: must be set if the customer number of the distributor at the production site is not
the same as the customer number that was entered in the xhaus entry for the production site at
the distributor. With a set variable, when scheduling an order at the production site, used as
customer number, default debtor and calculation debtor from the local xhaus entry. If the
variable is not set the customer number sent from the distributor is used as customer number.


IB_NOBESTINTBEST (client reference: no)
  For internal orders and in active ordering, since 2.7 except for the order in the receiving system,
an order is also generated in the sending system. This is not always desired! (additional
document, data, goods receipt, etc.) With this variable, the generation of the local order
document can be switched off




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                   22
IB_NO_IN_DOCUCHECK: Within the order scheduling for PO transfer, documents to be
transferred are copied from a temporary directory of the EDI on the document server. After that,
the program checks whether all defined documents have arrived there. If a document is missing,
the order is not released. If this variable is set, the check does not take place.


IB_NO_OUT_DOCUCHECK: Within the order scheduling for PO transfer, documents to be
transferred are copied from the document server to a temporary directory of the EDI. After that,
the program checks whether all defined documents for the PO are available in this directory. If a
file is missing, the transfer is cancelled. If this variable is set, the check is not done.

IB_XUSR (client reference: no)
  The employee who made the entry is retained by the EDI.
  Caution: the employee must be present in the target system!
  Caution: INTAUF_MANEU overrides these variables
  Attention: In combination with IB_EUSR.
  IB_EUSR for purchase orders, IB_XUSR: for orders (in the receiving site)


IB_ZVERS (client reference: no)
This variable is used to activate the order postponement to a test client. If this variable is set, the
column intver in intbest is evaluated by trm_ctrl. Using the shell script "intver," orders for
postponement can be placed in intbest.
Attention: No other activity should be booked to intbest!
 The orders are registered in the target system with parhausnr+=100 so that no messages are sent
to the sending system!
In addition, the orders in the target system are not transferred to intauf with still -1 (NEUKAUF),
but rather with still -3 (TXT_KOMPL), which means that some functions (e.g. E/A rules, price
calculation) will not take place during the import. (see section "Order shifting")


INTAUF_ALTEK
  active : After an order transfer, the PU prices transmitted in advance in the sender
       are taken over in the recipient as SA prices
  inactive: After an order transfer, the SA prices in the receiving site
       are determined anew
  x|y|z : if site numbers are entered separated by | (pipe)
       for these sites in advance after an order transfer,
       the PU prices are taken over in the recipient as SA prices.
       For all other sites, the prices are not taken over.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  23
INTAUF_CHECK_DFUE_RESTRIKT: If this variable is set, for all incoming EDI orders (external and
internal), there is a dimension restriction check. If an existing restriction is violated, then the order
is not released, but placed in the release pool with an appropriate notation. In addition, an
appropriate entry in the document notes is generated for the dimension restriction violated.
Processing restrictions (article dimensioning) are always checked.
Starting in July 2025: BOM restrictions will also be checked
INTAUF_DFUE_WUNSCHLIEFERANT (client reference: no)
For ext.DFÜ, the desired supplier is taken over (item) if a BA is of the type "PO".
Std logic: only if 1st procurement type is "PO"


INTAUF_FREITEK: This variable controls whether and which orders scheduled via EDI are released
directly and which are put into the release pool.
EXTERN: The orders from external order input interfaces are not released directly, but rather
placed in the release pool.
INTERN: The group-internal EDI orders (order linking and order transfer) are not released
immediately, but rather placed in the release pool.
ON : All EDI orders are placed in the release pool


IB_EUSR (client reference: no)
  If set, the eusr in kauf (user) is no longer set to -1 (System) for orders transferred. (ON,
RELEASE, UNCHANGE, ORDER)
  Caution: then all employees have to be present everywhere on the network!
  Attention: In combination with IB_XUSR.
  IB_EUSR for purchase orders, IB_XUSR: for orders (in the receiving site)
  Caution: INTAUF_MANEU overrides these variables
  Value RELEASE see AWDesk 198581, UNCHANGE #358345
  \\jupiter\DOKU_DocuWare\ALCIB-PMS\DFUE\Bestellübertragung_Uebersicht.doc Note:
The variable BESTPOOL_INTERN must be deactivated, for the variable creates chaos with active
BESTELLDFUE. BESTELLDFUE already includes the logic of collective POs for internal supplier via
PO pool (see case 240821).


INTAUF_BEARBCOPY_BA_HALTEN = ON: If this switch is active, the processing steps marked as
'can be passed on' in master data will adopt the processing type from distribution instead of
loading it from the production site's master data as for all other elements.


INTAUF_VSGLM_BA_HALTEN=ON: If this switch is active, the processing steps marked as 'can be
passed on' in master data will adopt the processing type from distribution instead of loading it
from the production site's master data as for all other elements.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                   24
INTAUF_MANEU (client reference: no)
  If this variable is active, all EDI orders are assigned user -1 (that is the system service).
Otherwise, the user of the sending site is retained.
  Caution: this variable overrides the variables IB_EUSR and IB_XUSR
INTAUF_LIEFERART (client reference: no)
If variables are set, the delivery type is redrawn for internal EDI:
        ON = for order generation at the production site and PO generation at the distributor
        1 = Only for order generation at the production site
        2 = For PO generation at the distributor


INTAUF_VERPACKART (client reference: no)
  If the variable is set, with internal EDI, the packaging type is re-transmitted for rack planning):
        ON = for order generation at the production site and PO generation at the distributor
        1 = Only for order generation at the production site
        2 = For PO generation at the distributor


MD_MIN_AHAM (client reference: order)
For the internal EDI it is assume that the item master data is identical in its essential properties.
Therefore, the SR is transferred unchanged by default. Local production lines can require that a
particular SR not be underrun. To achieve this, a minimal SR can be defined client-specifically.
This function may not be configured together with DFUE_IB_OWN_AHAM.


PMSPURCHASETRIGGER (client reference: no)
If ALCIB works with a different production system than PMS, PMS can continue to be used as an
order switch, i.e. to trigger internal and external order proposals. In this case, however, no
statuses, such as incoming goods messages, may be booked on the PMS side. The order blocking
may only be carried out from ALCIB or the other production system. Requirements for the
background process - with the exception of order scheduling - are therefore ignored when
variables are active, and feedback messages are prevented as far as possible.


    2.6.         Housekeeping
Under the stipulation that the external and internal EDI can run in parallel in principle and that
the attached files can be used several times, the scheduling process cannot clean up the incoming
directory and the intermediate directories for additional files. This has to be done in a
housekeeping script that runs at night. The script has to check whether scheduling is still open
(table ialf_jobctrl.status != 30). If there is no more scheduling to be processed, then the incoming
directory and the directory /usr1/alcibnet/dat/EDI/<dfuetyp> can be cleaned up.


Status in ialf_aufctrl and ialf_jobctrl

A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                   25
10 – Order generated for job
20 - Order complete, but not the whole job
30 - Order and job complete
40 - Order will be processed by trm_ctrl
50 - aufnr was assigned in ibin
300 – Error in the interface
310 - Error in the interface, but nevertheless processed by trm_ctrl
320 – Error in exbin()
330 – Error in ibin()
340 - Error in filter post-processing




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx   26
3. Error research
    3.1.         Reports
The DFÜ reports are primarily in $DFUEDIR/proto. Depending on the configuration, in this
directory there are subdirectories for the individual clients installed on the server
($DFUEDIR/proto/<xhaus.hnr>). In the precise client directory, there are, in turn, thematic
subdirectories
global, edi, ibin, ibout, exbin, edi_misc.
Environment variable: DFUE_TRM_SIMULTAN, DFUE_JOBCTRL


QR22/02
Since A+W Enterprise release 6 December 2019, the master data replication can log in its own
tables and generate from this a log e-mail for the end user (#377851 // [AW-7851]). With the
further expansion of this function in other modules of the EDI, it became necessary that in
addition to the log tables dfue_protokopf and dfue_protodetail, there must also be back-up tables
and a function to delete old data.
When the process to be logged is done and the e-mail for the end user was generated, the
relevant records (key: dfue_protokopf.id) is pushed out of the tables dfue_protokopf and
dfue_protodetail to dfue_protokopfok and dfue_protodetailok. There, they are still available for
searches. However, it can happen in these tables that the original key dfue_protokopf.id is no
longer unique.
Old data records can be deleted from the *ok tables with the normal A+W Enterprise deletion
function for unreferenced records. By default, the records are deleted after 365 days. This
deadline can be defined with the environment variable DFUE_PROTOTAB_INTERVAL.
    •   If the environment variable is not active, the deletion deadline is 365 days.
    •   If in the environment variable a value less than zero is entered, the data will never be
        deleted.
    •   If in the environment variable a value between 0 and 14 is entered, the deletion deadline
        is 14 days.
    •   If in the environment variable a value greater than 14 is entered, the deletion deadline is
        this number of days.


        3.1.1.           Article replication
The log $PROTOPFAD/ArtReplik<mmdd> writes the article replication. The logging is done in
English. The logging level can be switched with the environment variable
DFUE_RESEARCH=art_replicate to an expanded mode, a so-called developer mode. The log is
written buffered by default. If the expanded log is switched on, then it is written unbuffered. If
you would like the default protocol to be written unbuffered as well, then the environment
variable DFUE_PROTO_NOBUFF has to be set.




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                27
          3.1.2.           Market partner replication
The log $PROTOPFAD//MP_replic<mmdd> writes the market partner replication. The logging level
can be switched with the environment variable DFUE_RESEARCH=mp_replicate to an expanded
mode, a so-called developer mode.


          3.1.3.           Key replication
The key replication writes a log to $PROTOPFAD/ Key_replic_<date>_<time>. If the
environment variable REPLICATE_PROTO is set, an expanded logging can be switched on.


      3.2.         Research options
In the reports, especially the document transfer, errors are marked with the keyword "ERROR"
and warnings with the keyword "WARNING." If a possible error cause and remedy are known,
appropriate instructions are provided with the keyword "HELP."
With the environment variable DFUE_RESEARCH, it is possible to place the individual logs on a
higher degree of detail (see "Environment variables").
The system can be configured so that a special error is generated. This is primarily intended for
tests within development.
DFUE_ARISE_ERROR (client reference: no)
  If this variable is set and has a value greater than 0, an error is provoked at a particular point in
the EDI.
       1 - after converting the aufnr in _* tables (ibout)
    100 - end kauf_insertgroup (ibin) ;
    101 - after insert into aufint (ibin)
    102 - after script call in dfue_nachbearb (ibin)
    103 - all the way at the end (ibin)
    104 - simulation of active MODUL_STAPELLOGIK (ibin and ibout)


          3.2.1.           Status in the table intbest
The error status of the EDI is entered in the table intbest in the field sendeseq:
Positive values in the sendeseq field mean that the document has already been sent, however the
receiving site has not sent confirmation of the receipt.
The procedures specified here for eliminating a problem currently represent the best knowledge
as recommendation and do not absolve you of the obligation to prior research and weigh all
possible consequences (especially in case of data manipulations).


Error status           Cause                           Remedy
0                      New entry                       Please check whether the EDI was started
                                                       (process: dfue_startert $HAUS). If the process

A+W Software GmbH                     EN-CONFIG-A+W Enterprise EDI.docx                                   28
                                             is not running, it can be started with
                                             'starterstart'.
                                             For additional notes, see the logs
                                             $DFUEDIR/ueber_err$HAUS and
                                             $DFUEDIR/proto/ibout_proto$HAUS.
-1              Entry is being processed     This is a temporary state when the EDI begins
                                             to process a dataset. If this state should last
                                             longer, it must be checked whether a process
                                             trm_ctrl 10 ...$HAUS ... is running. If this is the
                                             case, it must be checked in the log
                                             $DFUEDIR/proto/ibout_proto$HAUS why and
                                             where the process is hanging. It is possible
                                             that the process must be ended.
                                             If no abovementioned process is running, the
                                             sendeseq can be reset to 0. Here it must be
                                             heeded that no doubled records arise in the
                                             table. Key on this table is "kaufnr, gruppe,
                                             poskonr,posnr, tupnr, sendeseq, storno".
-2              There can be several         For the precise cause, see
                causes of this error. The    the log $DFUEDIR/proto/ibout_proto$HAUS.
                EDI classifies the various
                                             If the following line is in the ibout log, then
                errors as temporary
                                             you have to check the ibin log for the cause.
                errors (e.g. locking of an
                order by an employee)        called ibin(pknr,-2,dest) for purchase order!
                                             (rc=-2)
                                             23.03 17:18:28: ERROR -2 in create
                                             PO/Enquiries (ibin)
                                             With each start of the EDI, there is an attempt
                                             to re-process these records. Starting the EDI
                                             can be forced with the script pmptrmctrlstart.
-3 (only with   Error during update of       Only for BESTELLDFÜ: The error cause could be
BESTELLDFUE)    the sendeseq to 0 by the     in REPERROR or in the file that was generated
                report ekueb.rep             from the form printing during file printing.
                                             After checking the data, either delete entries
                                             from intbest and transfer the purchase order
                                             again via Purchasing – Form printing or set
                                             sendeseq = 0 (WARNING: Here you must heed
                                             that no doubled records arise in the table. Key
                                             on this table is "kaufnr, gruppe, poskonr,posnr,
                                             tupnr, sendeseq, storno")
-15             IO_LOAD_ERROR:               For the more precise cause, see the log
                                             $DFUEDIR/proto/ibin_proto$HAUS.
                An error occurred when
                loading the data in the      Up to version 2007:
                receiving site
                                             e.g. insert _ikuaz fehlgeschlagen SC=-206,
                                             CISAM=-111



A+W Software GmbH             EN-CONFIG-A+W Enterprise EDI.docx                                    29
                                         Load from _tables : SC=-206
                                         => generation of the parallel tables _kuaz and
                                         _ikuaz from the regular table kuaz mittels
                                         ‚alias_temp kuaz’
                                         WARNING: This may only be done if no EDI
                                         order and no order generation is being
                                         processed by intauf.
                                         Starting with Version 2007, the tables are
                                         generated dynamically in the program.
-1007          MASTERDATA_ERROR:         Create master data at the receiving site or
               Items are contained in    adjust document at the sending site.
               the sent document that
                                         Can also be informed about messageID 68
               are not included in the
               master data at the
               receiving site.
-1100          Select on kpos produces   For the precise cause, see the log
               error                     $DFUEDIR/proto/ibout_proto$HAUS (older
                                         versions < 3.2 $DFUEDIR/ueber.err).
                                         “ERROR: SC 100 CISAM 0 during search item!”
                                         there is another aufnr in intbest.internr than in
                                         kpos for the document. The cause can be that
                                         a PO was re-generated before the transfer.
                                         This should have been caught, except ...
                                         If necessary more precise examination of how
                                         the data inconsistency occurred is required.
                                         Solution: remove intbest entry and set
                                         document again.
-2002          IO_NOT_FOUND_ERROR        For the precise cause, see the Log
               at the sender.            ibout_proto* (older versions < 3.2
                                         $DFUEDIR/ueber.err).
               Required data was not
               found for export.         Previously occurred causes:
                                         In the order, special items were entered that
                                         require additional data. Therefore, the field
                                         kpos.gvkz!=0. However, the relevant item of
                                         the corresponding record does not exist in the
                                         table kposgv. It must be examined how the
                                         order was entered or has been changed in
                                         order to determine the cause of the missing
                                         record within the order entry.
                                         If necessary, the relevant item must be re-
                                         entered.
                                         Remove the order from the table intbest and
                                         after the correction, it is provided anew by the
                                         system for transfer.


A+W Software GmbH          EN-CONFIG-A+W Enterprise EDI.docx                                 30
-2003          Database error when           Please check in the Log ibout_proto<haus>
               exporting an order            which error is the one in question (table, error
                                             number). Using the error number listed there,
                                             the corresponding causes must be researched
                                             and measures taken to eliminate these (e.g.
                                             data correction for SC = -284; adjustment of
                                             the database structure with SC = -217; order
                                             correction with SC=100 (expected files are
                                             missing))
-2020          Different suppliers for the   A PO in the PO pool was generated with
               same group/PO number          different suppliers. This should actually not be
                                             possible. In case of this error, message 47 is
                                             sent. Please ask the user how he generated
                                             the PO. How is BESTPOOL_GRUPPIEREN set?


               Different number of           sendeseq=0 is still in intbest, but -2020 is in
               records to be processed       the ibout* log
                                             Get data from intbest (2 rows copied)
                                             …
                                             ERROR (-2020): Intbest fetch (1) > count (1)
                                                           ==> !! EXIT !!
                                             Checks the field intever; it must be between 0
                                             and 4. Is the variable IB_ZVERS set? If so, see
                                             section "Order shifting"
-2025          Error when accessing files    FOPEN_ERROR, that is,
               or writing files
                                                 -  the log file for status exchange
                                                    between the clients could not be
                                                    written. The file is written to
                                                    $DFUEDIR/dat
                                                 - or the packing of the sn files did not
                                                    work
                                                 - or the packing of attached files
                                                 - or ...
                                             without ibout log, you will not find the precise
                                             cause.
-2028          Purchase order not yet        Check whether the purchase order is already
               released or already           in the status "local correction – ordered" or in
               transferred.                  the status "local correction – transferred". If
                                             the status "ordered" does not yet exist or if
                                             the status is already "transferred", a transfer
                                             of the purchase order is not possible. Please
                                             correct the status of the purchase order. For
                                             this case, the message No. 46 can be sent.
                                             Please check the setting
                                             DFUE_IB_BESTELLSPERRE.


A+W Software GmbH           EN-CONFIG-A+W Enterprise EDI.docx                                   31
                                            If the supplier is VKKopplung, but a PO is
                                            provided for transfer
               Starting with QR 2406 –
               incorrect transfer type
-2029          Missing delivery date        Attention:
               (field intbest.termin)
                                            Delete the relevant record from intbest and
                                            possibly bestpool and re-do the date
                                            calculation in the PMS.
                                            Or
                                            Set a known date in the table intbest.
-2030          For purchase order           Check the data and configuration. See also
               transfer,                    #447449
               sender=recipient
                                            NO_LAGERBEST is probably not set and
                                            internal order transfer configured. Why is
                                            NO_LAGERBEST not set. Why do you need the
                                            PO. The recommended workflow is to
                                            generate only a stock-filling order without PO
                                            and then to trigger the incoming stock booking
                                            via the packed message from production.
-2040          During the order             The status is transmitted back during the order
               scheduling, it is checked    transfer to the distributor as status -1007
               whether all item and
               BOM articles also exist in
               the article master data
-2041          Address not present          The delivery address of the retail order no
                                            longer exists in the master data. Please correct
                                            the order.
-2042          Doubled records in           To eliminate the problem, it must be clarified
               awc_bestetikett              with production which labels/glass should
                                            actually be ordered in which quantities. Then
                                            the data must be corrected/deleted in the
                                            tables "awc_bestetikett", "intbest", and if
                                            necessary, "bestpool".
                                            Should not happen anymore starting with
                                            "A+W Enterprise 6 Export Service -
                                            13.4.12027" (June 2025)
-2050          General SN file FTP          Please check ibin log.
               transfer error.
                                            Possible causes:
                                                 -   No FTP active on the Windows
                                                     computer Please check the ftp
                                                     connection with the user alcibnet
                                                     manually
                                                 -   Is the Windows computer correctly on
                                                     the .netrc of the user's alcibnet. On
                                                     the .netrc, it has to be precisely as in


A+W Software GmbH           EN-CONFIG-A+W Enterprise EDI.docx                                   32
                                                  the environment variable
                                                  DFUE_DATEI_REF_PFAD or
                                                  DATEI_REF_PFAD (including or
                                                  excluding domain specification)
                                              -   FTP log in /tmp/ftp*
                                              -   It has to be heeded that in the
                                                  DFUE_DATEI_REF_PFAD variables, /
                                                  instead of \ are to be used for the
                                                  path specification.
-2051          Check failed, whether SN   Please check ibin log.
               file is present in the
                                          A fixed subpart should be ordered. In the
               article master data for
                                          article master data (master data - article - F4 -
               transfer.
                                          article dimensions), no valid SN file is entered
                                          or the copying of the SN file failed
                                          Possible causes:
                                              -   No FTP active on the Windows
                                                  computer Please check the ftp
                                                  connection with the user alcibnet
                                                  manually
                                              -   Is the Windows computer correctly on
                                                  the .netrc of the user's alcibnet. On
                                                  the .netrc, it has to be precisely as in
                                                  the environment variable
                                                  DFUE_DATEI_REF_PFAD or
                                                  DATEI_REF_PFAD (including or
                                                  excluding domain specification)
                                              -   FTP log in /tmp/ftp*
                                              -   It has to be heeded that in the
                                                  DFUE_DATEI_REF_PFAD variables, /
                                                  instead of \ are to be used for the
                                                  path specification.
-2052          Copying the SN files via   Please check ibin log.
               FTP failed
                                          Possible causes:
                                              -   No FTP active on the Windows
                                                  computer Please check the ftp
                                                  connection with the user alcibnet
                                                  manually.
                                              -   FTP log in /tmp/ftp*
                                              -   Is the Windows computer correctly on
                                                  the .netrc of the user's alcibnet. On
                                                  the .netrc, it has to be precisely as in
                                                  the environment variable
                                                  DFUE_DATEI_REF_PFAD or
                                                  DATEI_REF_PFAD (including or


A+W Software GmbH           EN-CONFIG-A+W Enterprise EDI.docx                                 33
                                                    excluding domain specification)
                                                -   It has to be heeded that in the
                                                    DFUE_DATEI_REF_PFAD variables, /
                                                    instead of \ are to be used for the
                                                    path specification.
-2053          Check failed, whether file   Please check ibout-log and copy_docu_files*.
               is present for transfer.
                                            Start transfer with DFUE_RESEARCH=ibout.
                                            Then a lot of the ftp connection is also written
                                            in /tmp/ftp*.
                                            Possible causes:
                                                •   No FTP active on the Windows
                                                    computer Please check the ftp
                                                    connection with the user alcibnet
                                                    manually
                                            In the ftp log, there is an attempt to open the
                                            connection with the USER "bin". FTP log in
                                            /tmp/ftp*.
                                            Possible cause
                                                •   Is the Windows computer correctly on
                                                    the .netrc of the user's alcibnet. On
                                                    the .netrc, it has to be precisely as in
                                                    the environment variable
                                                    DFUE_DATEI_REF_PFAD or
                                                    DATEI_REF_PFAD (including or
                                                    excluding domain specification)
                                                •   It has to be heeded that in the
                                                    DFUE_DATEI_REF_PFAD variables, /
                                                    instead of \ are to be used for the
                                                    path specification.
                                            For research also the log


-2701          During the purchase          The purchase order generation tries to change
               order generation it was      an existing purchase order for the order and
               determined that more         supplier. If, however, there are already several
               than one purchase order      purchase orders for an order and supplier, the
               exists for an order and a    system can no longer decide which purchase
               supplier, split              order may be changed. Here, manual
                                            intervention is necessary (e.g. cancellation of
                                            existing purchase orders)
-9000          Provoked errors within       Deactivate environment variable
               the program                  DFUE_ARISE_ERROR.




A+W Software GmbH           EN-CONFIG-A+W Enterprise EDI.docx                                  34
        3.2.2.            -2041: Missing shipping address
[AW-109920]: trm_ctrl - 13.04.9110 // 05.2023
If a PO is generated and/or transferred for an order with an invalid shipping address the
generation of the new document is interrupted with the temporary error -2 and the system tries
again later. This could cause a high number of error e-mails and a high system load. Therefore,
this error is now set to its own, new error status -2041.
In this case, the shipping address in the order and/or in the market partner must be corrected.
Then the error status can be reset in the table "intbest" and the generation/transfer started again
(pmptrmctrlstart).




    3.3. Additional problems and their possible
       cause(s)Z
Problem                    Cause                    Remedy
The send purchase          The dfue_starter of      Check in the directory $LOCKDIR whether a
orders remain in the       the relevant site is     file starterlock$HAUS is present. If this file is
table intbest with         not running (check       present, but the corresponding dfue_starter
sendeseq = 0.              with the command:        is not running, this file must be deleted.
                           "ps –ef | grep
                                                    If the dfue_starter is not running, it must be
                           dfue_starter" or "ps
                                                    started with the command "starterstart" in
                           –ef | grep alcibnet")
                                                    the environment of the affected site.
                                                    Log: $DFUEDIR/proto/start_proto<$HAUS>
The send orders            The directory            The processing files for the dfue_starter are
remain in the table        $DFUEDIR/wait            in the directory $DFUEDIR/wait. The files to
intbest with sendeseq      contains too many        be processed end with .r$HAUS. All files can
= 0, although the          files.                   be deleted that are older than one day and
corresponding                                       only end with the ending .$HAUS. The
dfue_starter is running                             content of the .r$HAUS files must be
                                                    checked. Of the files that can only call
                                                    trm_ctrl_* <Parameterlist>, all files but for
                                                    one with an identical parameter list can be
                                                    deleted.
                                                    For all other files, an individual case check in
                                                    cooperation with the customer is required.
The records for PO         No *.r<hausnr> file is   In the table xhaus, the hausart has a value
generation remain in       generated in             less than 10. In addition, the environment
intbest with positive      $DFUEDIR/wait, but       variable(s) DFUE_DBTYP_* are activated.
sendeseq. No PO is         rather a file *.rh or
                                                    The xhaus. hausart< 10 is no longer
generated                  *.rp
                                                    supported. Please update the hausart in
                                                    xhaus to 10 or 11 and restart the ue_server
                                                    and the dfue_starter



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                    35
Error –206 in loadext()   An absolutely          A _ and/or _i table is missing. (only up to
in ibin_proto<haus>       necessary table does   Version < 2007)
                          not exist
                                                 In the script
                                                 $ALCIBPRG/install/cmd/prep_dfuetabs (älter
                                                 prep_ibtabs) all tables are listed for which
                                                 the underscore tables must exist. In case of
                                                 doubt, this script must be updated at the
                                                 customer with the one from Linden.
                                                 After that, the script or an alias_temp
                                                 <Table> can be executed. Here, attention
                                                 must be paid that there is an OK next to each
                                                 "create ...".
                                                 WARNING: This may only be done if no EDI
                                                 order and no purchase order generation is
                                                 being processed by intauf since the
                                                 intermediate files are deleted (drop _
                                                 tables)
                                                 Starting in Version 2007, the - and i-tables are
                                                 generated dynamically as TEMP tables and
                                                 they are no longer present after ending of
                                                 the trm_ctrl.
The transfer works,       Error in uudecode      Install Uudecode on a computer where it
but the table intbest                            works.
will not be emptied in
the sending site.
The entries from the      The environment        There are only entries in
table intbest for         variable IB_MKBEST     $DFUEDIR/proto/ibout_proto<$HAUS>,
generating a purchase     is not set.            however none in ibin_proto<$HAUS>.
order disappear,
                                                 In the extended log mode
however no purchase
                                                 (DFUE_RESEARCH=ibout), the variable
orders are generated
                                                 definitions are at the beginning:
                                                 : ** IB_GRUPPE using groups during
                                                 processing: NO
                                                 : ** IB_MKBEST create purchase
                                                 orders: NO
After saving the          No start file          The environment variable
purchase orders from      *.r<$HAUS> nach        PMPTRMCTRLSTART contains the script for
the order pool, these     $DFUEDIR/wait is       the automatic start of the trm_ctrl. In
are not processed         written                general, the script is also called
automatically although                           pmptrmctrlstart.
the dfue_starter is
                                                 PMPTRMCTRLSTART=“pmptrmctrlstart“
running




A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                  36
After generation of an     The order was not       INTAUF_CHECK_DFUE_RESTRIKT: If this
order at the sending       released                variable is set, there is a restriction check for
site, no purchase          automatically           all incoming EDI orders (external and
order/work plan is         (kauf.tekapkz=0)        internal). If an existing restriction is violated,
generated                                          then the order is not released, but placed in
                                                   the release pool with an appropriate
                                                   notation. In addition, an appropriate entry in
                                                   the document notes is generated for the
                                                   restriction violated.
                                                   INTAUF_FREITEK: This variable controls
                                                   whether and which orders scheduled via EDI
                                                   are released directly and which are put into
                                                   the release pool.
A transferred order     Different logic for        Check DFUE_PAKID_HOSTBASE. The value of
cannot be processed at generation of file          the variables must be identical in the sending
the receiving site. The names.                     and receiving sites.
information is in the
ibin log that the file
with the name <xxx>
could not be
found/opened
A transferred              Data structure and      The version information in the respective
document cannot be         structure of the load   data records of the table xhaus must be
processed at the           file to not fit         checked. These must be consistent in the
receiving site. The        together.               sender AND in the recipient (xhaus) In
information is in the                              particular, the field vers_seqnr hast to be
ibin log that the load                             correct for all participants.
has failed.Log intbest
                                                   Site A orders in site B. Thus, in site B the data
Einlagern (kposp) LOAD
                                                   record for site A has to be identical to the
fehlgeschlagen Error
                                                   data record of site A in site A.
Code: -1
SC=0 CISAM=0,ERRM:><
A change transmission      The status delivery     In the EDI, this status must be checked since
does not result in a       planning exists         her no question can be posed as in the
change of the order at                             foreground.
the production site
even though it is not in
local correction. The
message 55 fx_texte
23030 : "Caution:
order %d=%d from site
%d change failed -
already released!" is
sent




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                     37
    3.4.        Checking the transfer
All PO generations and document transfers to another site (internal EDI) will be written to the
table intbest and processed there by the trm_ctrl.
For this, various State flags are written to the table in the course of the processing. In addition,
messages are sent for successful and/or faulty processing. Which messages are sent to whom can
be configured (see section "Messages")
In the application, you can use the menu element "System - Data Transfer - Document Transfer -
Check Transfer" to view the faulty and successful transfers.
When the dialog opens, a selection menu appears:
    a) Orders whose transfer is in progress
        All transfers are displayed here that have a positive send sequence. This means that the
        transfer was made, but the recipient has not yet sent confirmation of the receipt.
    b) Orders with faulty transfer
        All transfers are displayed here that have a send sequence less than -2. This means that
        an error occurred during the transfer. The send sequence specifies which error occurred.
        (see section "Status in the table intbest"
    c) Orders that have not yet been transferred
        All transfers are displayed here that have not been started yet.
    d) Transferred orders
        All transfers are displayed here that are in the table "intbestok". This means that the
        transfer was processed successfully.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                38
4. Purchase order generation
Within an order, it can be decided using the supply type of an item or a BOM part whether this
part should be ordered. After the order has been scheduled and analyzed by the production
system, order proposals are created according to the master data and configurations.
The order proposals are ALWAYS created by the production system!
For clients with own production, the order proposals are created by A+W Production.


    4.1.        Pure trade site
If an A+W Enterprise site is a pure trade site without its own production, the PMS production
system can function as an order gate. For this, the environment variable PMSPURCHASETRIGGER
has to be activated. This variable can only be activated globally. This process is also called "PMS0"
With use of an internal client separation, it is now possible for individual clients (trade operations)
to have the orders created via the ALCIB order gate. For this, for the appropriate clients the
environment variables ORDERXML and AWC_ALCIM_ANBINDUNG have to be deactivated and the
environment variable PMSPURCHASETRIGGER has to be global.
The environment variable MODUL_PROD_SPAETE_AENDERUNGEN may not normally be active.
Since this can be necessary for other clients of a multi-site system, however, starting with build
pms - 13.04.8431, this no longer disturbs the processing in the retail clients.


        4.1.1.          Postponement
If within A+W Enterprise the order gates (without connection to A+W Production) were used,
previously the delivery date of an order was not shifted if the delivery date of the PO was before
the delivery date of the order.
Within the order gates, the delivery date is calculated for an order including customer and
supplier handling time. If the incoming goods date calculated this way is later than the delivery
date of the order, now with appropriate configuration, the delivery date of the order is shifted to
the next possible delivery date.
#375089: environment variable for the order PMEKAUF and in dispatch PMEMELDTERMINVER


        4.1.2.          Special checking of the environment variables
  PMSPURCHASETRIGGER (client               ON             Has to be active for pure trade sites
  reference: no)                                          (without AWC connection)
  MODUL_KOSTENKALK                         2              May absolutely not be 3
                                                          Is not evaluated client-specifically
  PMEINLASTUNG                             disable
  PMEINLASTUNGNEU                          disable        Not "OFF" und enable =1 but rather
                                                          enable=0, otherwise no update of the
                                                          shipping date in kauf


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  39
                                                         PF [AW-138928]
  PMPGLASALL                              disable
  PMXAWPOOL                               disable
  PMQCIMIN                                disable
  PMPHPOSANZ                              disable
  PMETERM                                 check          4, otherwise no update of the shipping
                                                         date in kauf
  PMPGLASALL                              disable
  ORDERXML                                disable        Can also be deactivated for multisite
                                                         client-specific.
  AWC_ALCIM_ANBINDUNG                     disable        Can also be deactivated for multisite
                                                         client-specific.
  PMEKAUF                                 check          Writes new date back to the order (only if
                                                         PMETERM=4 and PMEINLASTUNGNEU is
                                                         deactivated (enable=0))
  PMEMELDTERMINVER                        check
  PMEGESCHART                             Check          May be necessary if for drop shipments
                                                         no handling time should be considered.
  PMPBESTTERMIN                           Check          May be necessary if for drop shipments
                                                         no handling time should be considered.
  PMELTPLANMAXDIFF                        Check
  PMENEXTTOURTERMIN                       Check
  PMHSLEEPTIME                            5              Was on 30 for AGC. Causes with a lock via
                                                         the NR_Server, so that it waits this
                                                         number of seconds before it tries to set
                                                         the lock again.



        4.1.3.          Logs
The process PMS is used for the date calculation. The logs are largely written in Alcib language.
PMEPROTOBASIS (client reference: no)
Detail degree of the log generation in the general service functions in the scheduling area (rough
scheduling).
   0 = no messages at all
   1 = only report errors
   2 = normal user log
   3 = expanded log for development
   4 = excessive log with all messages




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  40
PMEPROTOBAUM (client reference: no)
Detail degree of the log generation in the tree management functions in the scheduling area
(rough scheduling).
   0 = no messages at all
   1 = only report errors
   2 = normal user log
   3 = expanded log for development
   4 = excessive log with all messages

PMEPROTODASCH (client reference: no)
Degree of detail of log generation in the functions surrounding the date determination (date and
shift) in the scheduling.
   0 = no messages at all
   1 = only report errors
   2 = normal user log
   3 = expanded log for development
   4 = excessive log with all messages

PMEPROTOENTRY (client reference: no)
Detail degree of the log generation in the general external service functions in the rough
scheduling area.
   0 = no messages at all
   1 = only report errors
   2 = normal user log
   3 = expanded log for development
   4 = excessive log with all messages

PMEPROTOVGZ (client reference: no)
Detail degree of the log generation in the general functions default time calculation in the rough
scheduling.
   0 = no messages at all
   1 = only report errors
   2 = normal user log
   3 = expanded log for development
   4 = excessive log with all messages

PMHTESTLEVEL (client reference: user)
The variable contains the test level for a test message log for the background process PMS. This
corresponds to the test protocol in the foreground when you type "ESC f t". In the foreground the
test level is queried.
The test messages are written to the file "<Process-ID>.test". This is located in the folder that can
be reached with "gft" from a UNIX shell.
 A test level 3 generates a message each time a function is entered or exited. A test level of 9
(maximum) also generates a message for each event.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  41
    4.2.        Environment variables
  RAHMEN_BESTELLUNG_GLASMASS                check     For active A+W Production, replaces the
  (client reference: no)                              variable PMFZKRAHMENAHAM, which was
                                                      evaluated by PMS. When ordering
                                                      spacers/grids/muntins, data is calculated
                                                      according to glass dimensions.
  PMSPURCHASETRIGGER (client               ON         Has to be active for pure trade sites
  reference: no)                                      (without AWC connection)
  EK_REKLAMATION                            check     EK_REKLAMATION (client reference: no)
                                                      A complaint order does not automatically
                                                      result in a complaints PO. If this
                                                      environment variable is active, old logic is
                                                      reactivated, that is, a complaint orders
                                                      creates a complaint PO. This only applies to
                                                      Purchasing without prior grouping in the
                                                      purchase order pool.
  DFUE_IB_ADDITIONALGRP                     check         Client reference: no
                                                      If POs are generated without the PO pool,
                                                      parts to be ordered are combined per order,
                                                      supplier, and delivery type.
                                                      If this variable is activated, the "splitcode"
                                                      field for the grouping is also evaluated. The
                                                      "splitcode" field in the table intbest is
                                                      populated individually by the SP
                                                      "cu_pogetsplitcode". The SP is called by the
                                                      ERP
                                                      Webservice.
                                                           See "EN-CONFIG-A+W Enterprise EDI"
                                                           [AW-157565]




    4.3.        Configuration Options
The definition of the individual settings is made under
System > Data Transfer > Transfer Document > Configuration
Or in the market partner master data via the "EDI configuration" menu or F5 on the field "Type of
EDI."
With "Type of EDI" - 102 "PO generation," currently the following settings are possible:


Control type         Name                     Description


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  42
4                    Local Notification        If there is a notification for a PO, but the PO is not
                                               in local correction and this PO is corrected via
                                               order change, the notification's data is retained.
                                               Otherwise it is deleted. The control type is
                                               created for the supplier for which the PO is
                                               generated. Precise specification: ID 126756



    4.4.        PO grouping for direct orders
[AW-157565] // March 2024
If POs are generated without the PO pool, parts to be ordered are combined per order, supplier,
and delivery type. If this grouping is not sufficient, but you don't want to work with the PO pool,
there is now an additional customer-specific grouping criterion.
The function is activated with an environment variable. In addition, there must be a stored
procedure "cu_pogetsplitcode". This SP receives the parameter <Auftragsnummer (kauf.auftrnr)>,
<Vorgang (5)>, <Stücklistennummer (kpos.poskonr)>, <interne Positionsnummer (kpos.posnr)>,
<Stücklistenelement (aufstrukt.tnr)>, <Lieferant (aufstrukt.linr)> and returns a 2-digit character
string as additional grouping criterion.


For this, the tables "awc_bestproto", "intbest" and "intbestok" were expanded to include the field
"splitcode". The "splitcode" is the additional grouping criterion.Via the SP mentioned above, the
"splitcode" field is populated in the table "intbest" and "awc_bestproto" (return value of the SP).
It is taken over in the PO, but it is not visible there.
It is mandatory that the splitcode for an order part is always identical; otherwise PO changes
cannot be made correctly.
This function is only supported for direct POs (ID in the supplier master data).
If within the internal EDI you are working with order coupling, this function cannot be used.
If within the internal EDI you are working with this function, it must be activated for all
participating clients. However, it is possible that the SP returns no (or an empty) splitcode for the
parts to be ordered.
The function cannot be used if you are using one-type documents (article group) with the
function.


DFUE_IB_ADDITIONALGRP=ON
Cannot be used if PRODTYP_TEST is active.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                     43
    4.5.        Delivery Address
        4.5.1.          No direct shipment
If this is not a direct shipment, the delivery address in the PO is determined according to the
following sequence:


- Default delivery address of the supplier of the PO
- Default delivery address of the sending site
- Invoice address of the sending site
=> This way, there is no PO without delivery address!
The delivery address from the order is taken over in the end customer address.
If one of the addresses should be cancelled, this cancellation code is not considered within PO
generation. If a cancelled address is in an existing order, then it is also taken over into the PO and
a resulting order.


        4.5.2.          Direct shipment
If in the order there is a delivery address, the delivery address is taken over into the PO.
If the order contains no explicit delivery address, the delivery address in the PO is determined
according to the following sequence:


- Default delivery address of the supplier of the PO
- Default delivery address of the sending site
- Invoice address of the sending site
=> This way, there is no PO without delivery address!


If one of the addresses should be cancelled, this cancellation code is not considered within PO
generation. If a cancelled address is in an existing order, then it is also taken over into the PO and
a resulting order.


    4.6.        Document takeover
[AW-66053] – Release April AWE 6


Within the order entry, it is possible to attach files manually on the order and item level.
However, these files were not taken over into an order-related PO.
With the current version of A+W Enterprise, you can define both in the master data (Master Data
- Keys - System - Document Types) as well as in the order entry on the "Document assignment"
dialog that a document should be taken over into the PO. To do this, you need to place a

A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 44
checkmark in the "Best" field. If the checkmark is already set in the master data for the document
type, this is taken over into the order; however it can also be changed there.




If a document is marked so that it should be taken over into the PO, then the document is copied
to the PO during PO generation. This means,
    •   that if after the PO generation the document that was assigned to the order is changed,
        this change is not automatically in the associated PO.
    •   If the document that was assigned to the PO is changed, this change is overwritten in case
        of a change of the PO based on an order change.
The copying of the documents from the order to the PO is done analogously to Document
transfer within PO transfer.
Prerequisite is a functional FTP connection for the user "alcibnet" from the A+W Enterprise back
end to the server, which is defined in the variables DATEI_REF_PFAD or DFUE_DATEI_REF_PFAD.
Here, special attention has to be paid to a correct entry in the .netrc of alcibnet. In the .netrc, the
host name has to be precisely as in the variables DFUE_DATEI_REF_PFAD or DATEI_REF_PFAD
(including or excluding the domain). In addition, it has to be heeded that in the
DFUE_DATEI_REF_PFAD variables, / instead of \ are to be used for the path specification.
Furthermore, it can be defined whether it should be checked before the transfer whether all
documents defined for the PO to be generated are available. (IB_NO_OUT_DOCUCHECK - check
during the export of the purchased parts / IB_NO_IN_DOCUCHECK - check during the generation
of the PO). Attention has to be paid that both of these variables are also evaluated for the internal
PO transfer.


    4.7. Preventing                        deletion              of        the         dispatch
       notification
If an order-based PO is modified based on an order change, a possible existing dispatch
notification should be retained.
Here there must be a distinction whether a collective dispatch notice or dispatch notice with
different delivery dates exists. Here only the delivery date, not, however, the OC number of the
supplier, is checked.
If for an existing PO some items have already been dispatched but others have not, the PO is
treated as if there are different delivery dates.
Below is a detailed list of which data is modified at what time and in which form by the automatic
PO change if there is already a dispatch notice. Data that is not listed here is treated according to
the previous default logic. This also applies for future expansions of the dispatch notice/PO.
1. The delivery date for the entire PO is retained and not adjusted according to the new data.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  45
This can cause differences between production planning and PO. If the planned delivery date is in
the past or if it does not fit the route, there is a recalculation of the delivery date of the PO as
previously. The recalculation is done within the background process intauf
2. OC number of the supplier (item-specific):
If there is a collective dispatch notice (uniform delivery date), then the supplier's OC number is
retained for old items even if the quantity ordered has changed. For new items, the OC number is
taken over from the first existing items.
If there is already a dispatch notice with different delivery dates, the supplier's OC number is
retained for old items even if the quantity ordered has changed. For new items, the OC number is
left blank
3. Delivery date (item-specific):
If there is a collective dispatch notice (uniform delivery date), then the delivery date is retained
for old items even if the quantity ordered has changed. For new items, the delivery date is taken
over from the first old item.
If there is already a dispatch notice with different delivery dates, the delivery date is retained for
old items even if the quantity ordered has changed. For new items, the delivery date is left blank.
4. Confirmed quantity (item-specific):
If there is a collective dispatch notice (uniform delivery date), then the confirmed quantity is
retained for old items even if the quantity ordered has changed. For new items, the confirmed
quantity is set equal to the quantity ordered.
If there is already a dispatch notice with different delivery dates, the confirmed quantity is
retained for old items even if the quantity ordered has changed. For new items, the confirmed
quantity is set to 0.
5. Quantity ordered (item-specific):
Here there is no distinction according to collective dispatch notice or dispatch notice with divided
dates. The quantity ordered is retained for old items even if the quantity to be ordered has
changed. For new items, the quantity to be ordered is taken over from the order as previously.
6. Note (item-specific):
Here there is no distinction according to collective dispatch notice or dispatch notice with divided
dates. The note is retained for old items. For new items, the item remains blank.
Due to the changes listed above, there can be deviations between order and PO, especially with
respect to the quantity to be ordered and confirmed.
If the dispatch notice cannot be retained, the PO generation is continued nonetheless and a
message is sent to the message recipient of the message 47 - "Incorrect PO generation." In
parallel, appropriate log entries are made in the log $DFUEDIR/proto/ibin_proto<$HAUS>.
The message is phrased as follows:
RE: incorrect PO generation
Text: No: 32572: When changing the PO 213477/5, the existing dispatch notice could not be
taken over. Please check the log $DFUEDIR/proto/ibin_proto80.
The entire logic described here does NOT apply for POs that are created again after returning to
the PO pool.
EDI configuration:

A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                  46
Type of the EDI -> 102 - PO generation
SteuerID      ->   4 - set local dispatch notice for the supplier




    4.8.           Entered by
The employee (kauf.eusr) of a generated purchase order can be populated in various ways.
Without explicit configuration, the employee is -1 "System."
           Distributor / Sender / Purchase order generation
       a) Fixed purchasing employee
              For this, the environment variable EK_MANR must be set to the desired employee
              number. This variable is evaluated by the background process intauf. If with this
              configuration you wish to achieve that this fixed employee is also transferred to the
              production site for internal purchase orders, then the environment variable IB_EUSR =
              UNCHANGE must be set (starting with AWE5). If the variable IB_EUSR is not set for
              this configuration, then for internal purchase order transfer, the employee -1 is sent
              to the production site.
       b) Employee from the order
              For this, the environment variable IB_EUSR = ON or IB_EUSR = ORDER must be set.
              Here it must be noted that then the environment variable EK_MANR has no more
              effect for order-related purchase orders. Furthermore, it applies that for collective
              purchase orders, the employee from any one is used in the order that occurs in the
              purchase order.
       c) Employee who released the order
              For this, the environment variable IB_EUSR = RELEASE must be set. Here it must be
              noted that then the environment variable EK_MANR has no more effect for order-
              related purchase orders. Furthermore, it applies that for collective purchase orders,
              the employee from any one is used in the order that occurs in the purchase order.
              CAUTION: All configurations described above are overridden by the environment
              variables INTAUF_MANEU.
              For POs that are generated via the PO pool, the employee is taken over who
              generated the POs in the PO pool (intauf).
See also„PO transfer – User“


    4.9.           Parallel order generation (case 174883)
With Version 4.5 (2011), the order generation (dfuetyp 10, empfaenger 0) can be executed in
parallel.The logic is also coupled to the environment variable DFUE_TRM_SIMULTAN. This means
that with an activated variable, both the external scheduling as well as the order generation are
executed in parallel mode.




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                 47
    4.10. Shipping information
For generation, the shipping type is always re-determined from the master data.
The delivery type and packaging type are retained as usual. However, the behavior can be
changed via environment setting.
INTAUF_LIEFERART (client reference: no)
If variables are set, the delivery type is redrawn for internal EDI:
        ON = for order generation at the production site and PO generation at the distributor
        1 = Only for order generation at the production site
        2 = For PO generation at the distributor


INTAUF_VERPACKART (client reference: no)
  If the variable is set, with internal EDI, the packaging type is re-transmitted (for rack planning):
        ON = for order generation at the production site and PO generation at the distributor
        1 = Only for order generation at the production site
        2 = For PO generation at the distributor


INTAUF_DFUE_VERPACKART (client reference: no)
If this variable is active, then with external order scheduling, the packaging type is filled via
interface.


NEW_PACKING_LOGIC (client reference: no)
Activates the logic of inheritance of the packaging type:
ON or 1: Customer-specific setting: The packaging type is always inherited from the header in the
positions.
Furthermore, the packaging type for order generation in the production site, PO generation in
trade and external order scheduling will NOT be re-populated, even if the abovementioned
variables are set.
2: If the packaging type is changed in the header, there is a query as to whether this change is also
inherited by the positions. In addition, with appropriate configuration (see above), the packaging
type is determined anew from the master data and transferred via external order interfaces.


    4.11. Spacer and muntin orders
        4.11.1.          Basic information
Order-related, only frames can be ordered correctly. Spacers are generally triggered via stock POs.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                     48
In order to order frames correctly, correct master data is required. See also "DE-CONFIG-A+W
Enterprise"


        4.11.2.        Dimensions
See the activities as of 06/14/2012 in AWDesk #256754.
For the logic, there is also a section in the ConfigurationDocumentation EN-Config-A+W
EnterpriseProductionInterface.pdf:
Dimensions of purchased spacers
Dimensions of the purchased parts are reported by AWP. This also applies to purchased spacers
and muntins. A correct calculation of dimensions require the new step entry in AWE and a
respective setting for AWP-works.
Especially for spacers: The dimensions in AWP refer to the outside edge of the spacer. But AWE
needs the dimensions up to the inside edge of the spacer. Before a purchase order for spacers is
created, the Web Service calculates the spacer dimensions up to the inside edge. (Available from
version 2011 in a certain patch version of ALRPC service and ERP webservice ).


There are individual customers who, instead of the inside edge, expect the glass dimension. There
are also switches for this RAHMEN_BESTELLUNG_GLASMASS. If this switch is active, then the
intauf changes the dimensions on PO generation. he data is corrected again by aham/2 and the
new shape parameters are calculated.


        4.11.3.        AIR
In order to get the AIR for an ordered spacer without size variants from the IG of the order into
the PO, the environment variable RAHMEN_BESTELLUNG_SZR must be set. If the variable is set, in
the process of order generation (intauf still=-11) the intauf determines the AIR from the order
item and transfers it to the PO.
Furthermore, the mandatory dimension details must be maintained in the item master data.




    4.12. Breakage orders
Caution: This function must not be used when internal suppliers work with SA linkage and
offset.
Within the PO generation via the PO pool and in manual PO entry, you can specify a breakage
reason. If the breakage reason is entered during PO generation via the PO pool or during
automatic PO generation, then during the PO generation a new PO is generated and it is not
checked whether there is already a PO for the order item.


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                49
        4.12.1.         Reject place
Release February 2021: In addition to the breakage reason, there is now also a breakage location.


        4.12.2.         Reject per labels
Release February 2022 [AW-61247]: The function of remake ordering from A+W Production can
book breakage also per label. If A+W Production writes these labels to awc_bestetikett, then the
data is taken over in the PO in the table bestetikett. Labels taken over receive the status 1 in the
table "awc_bestetikett".


            4.12.2.1.           Multiple breakage report per label
[AW-180470] // QR2406
The production labels can be taken over within the function of the breakage POs. The
specification expects that each production label is only reported broken once (see release
February 2022 [AW-61247]). A repeated breakage report without previous PO generation is not
allowed. Since a restriction check is not accepted within the PDC reading by the customer, a check
has been built into the PO generation.
If a label is reported broken several times without having a PO generated previously, the PO
generation encounters the error -2042 - doubled labels. An appropriate log entry is made.
To eliminate the problem, it must be clarified with production which labels/glass should actually
be ordered in which quantities. Then the data must be corrected/deleted in the tables
"awc_bestetikett", "intbest", and if necessary, "bestpool". (up to June 2025 - see entry further
below)
[AW-195776] // QR2503
For the breakage report of an ordered lite from A+W Production, the data for a second report of
breakage is entered twice in the PO tables. This caused problems further down the line. With this
change, a reject message for a label that has already been reported is ignored. For the goods
received message to A+W Production for a reported broken lit with label, the record is removed
so that starting at this time, another break can be reported again.
A+W ERP Web Service 6 - 13.4.9458
A+W Enterprise 6 Export Service - 13.4.11218

Removing the PO labels reported from the production system on goods receipt

For the transfer of the goods receipt of PO items with labels, the labels are now removed that
were reported on goods receipt. This way, these can be reordered with another breakage report.
In the course of the booking, the status is set to 2 in the table awc_bestetikett and deleted in the
end.

Juni 2025 // A+W Enterprise 6 Export Service - 13.4.12027




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                    50
        4.12.3.         Missing breakage type from A+W Production
[AW-209098] // QR2503
Breakage remakes without breakage type
If a breakage remake order is generated from A+W Production, a breakage type should be
entered there. This is then transferred to the A+W Enterprise-table fields bestwun.bruch or
intbest.bruch and taken over from there into the PO. Precisely when a breakage renake should be
processed without type via the PO pool, this could cause the PO generation to be impossible and
rejected with the message 14421 - "Order: xx item y transfer not possible since this is already
ordered!"
This program behavior has been adjusted. The breakage fields in A+W Enterprise will now always
be pre-populated with 1 if no other booking reason is transferred.
A+W ERP WebService 6 - 13.04.9299



[AW-144582] // QR 2506
Incorrect processing parameters for breakage order

If several ordered and processed lites of an order item are reported broken at the same time, it
can happen that for the processings, incorrect parameters reported by A+W Production were
taken over. This problem has been corrected. In the course of correction, it is now necessary that
in case of breakage orders, all items receive their own BOM number from the system. This means
that starting now, all items within a breakage remake receive their own BOM numbers.



    4.13. Site-spanning PDC
The "Site-spanning PDC" is documented in "EN-CONFIG-A+W Enterprise".



    4.14. Complaint details
A complaint order does not automatically result in a complaints PO. If the environment variable
EK_REKLAMATION is active, old logic is reactivated, that is, a complaint orders creates a complaint
PO. This only applies to Purchasing without prior grouping in the purchase order pool


    4.15. Discounts
See "EN-CONFIG-A+W Enterprise.pdf" section "Discount logic 2005" and section "Cost calculation"


    4.16. Error research
Incorrect delivery address in    During PO generation, a           Environment variable
                                 recipient is written to intbest


A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                               51
the receiving site/in the PO   even though PU EDI is      BESTELLDFUE is not active.
                               entered for the supplier




A+W Software GmbH              EN-CONFIG-A+W Enterprise EDI.docx                       52
5. Order linking
    5.1.        Introduction
Within A+W Enterprise, there is a distinction between order linking and PO transfer. Parallel to
this is the "central quotation database."
During the PO transfer, a purchase order in the distributor becomes an order in the distributor
(sending site). This PO is then transferred to the production site and an appropriate order is
created there. Changes to the PO before the transfer are transferred to the production site.
During order linking, the concern is that an order in the production site (recipient) is generated
from an order in the distributor (sending site). Depending on the system configuration
(environment variable IB_NOBESTINTBEST), a PO is also generated at the distributor with the
supplier number of the production site. However, a direct change to the PO has no effects on the
order at the production site.
In this document, the terms "distributor" and "production site" will be used.
In connection with order linking, "distributor" refers to the site that enters the end customer
order. A distributor is not exclusively a distribution branch office without its own production. A
distributor can also have its own production, but it orders products from another branch office
from product lines or for capacity reasons.
This is opposed to the "production site." This is the branch office that produces products for
upstream branch office and supplies them to the end customer or the upstream branch office.
The production site does not enter the end customer order. A production site is not exclusively a
production branch office without its own distribution. A production site can also have its own
distribution, however it receives POs from other branch offices for product line or capacity
reasons.
Thus, the definitions "distributor" and "production site" always only apply for a concrete order for
a branch office.
It is urgently recommended that you use PO transfer instead of order linking. Currently, lacking
functionalities are being handled via case 321444. In the medium term, the goal is to terminate
order linking.
New functionalities that are available both in the order coupling and in the order transfer will only
be explained in the "Order transfer" section.
The function of the "central quotation database" is available if the PO transfer or the order linking
is configured and the environment variable ANGBDB is set accordingly.


    5.2.        Master data
        5.2.1.          Configuration Options
The definition of the individual settings is made under
System > Data Transfer > Transfer Document > Configuration



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  53
Or in the market partner master data via the "EDI configuration" menu or F5 on the field "Type of
EDI."
With "Type of EDI" = 100 "SA coupling," currently the following settings are possible:


Control type        Name                      Description
5                   Individual number         Set at the production site
                    range
                                              If this configuration is set for a customer, the new
                                              number for the order to be scheduled is not
                                              obtained from the normal order number range
                                              "kaufex.mfo," but rather from the number range
                                              "kaufdfue."
                                              Caution: The number ranges kaufex.mfo and
                                              kaufdfue must absolutely be disjunct.
                                              This function cannot be used together with an
                                              offset!
                                              ID 132679
48                  Retention of local        Set at the production site
                    order fields
                                              If this configuration is set for a customer, in case
                                              of order changes via internal EDI, the local fields
                                              in kauf._private_* are retained. If this
                                              configuration is not set, the values will be taken
                                              over from the distributor.
                                              see also DISABLE_COPY_PRIVATE_CHAR1
                                              If this variable is set, with the first transfer and if
                                              the configuration 48 is not activated, the field
                                              kauf._private_char1 is emptied.
                                              The private item fields (kposp.private*) or the
                                              configurable private fields (kaufprvfld,
                                              kposprvfld) remain unaffected by this.
                                              #454898
65                  No site assignment in     Is set at the distributor.
                    the call center
                                              If this configuration is set for a customer, on order
                                              scheduling via internal EDI, there is no automatic
                                              site assignment in the call center. The order
                                              remains in the release pool of the call center.
                                              See also "EN-CONFIG-A+W Enterprise EDI"
                                              section "Release pool"




A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                      54
        5.2.2.          Distributor
For the PO transfer, it is necessary that the production site be created as supplier in the market
partner master data. Decisive for the linking of orders is the "EDI type" field on the "Delivery" tab.
This field has to be set to "VKKopplung."
Moreover, the production site has to be entered in table xhaus with the same supplier number.
Special attention must be paid to the correct setting of the fields kunr, linr, host, hausart, vers,
subvers, and patch as well as iboffset, bytevektor, and dfuedirpath since these have a central
effect on the order linking.
In all sites participating in the order linking, the table xhaus must be adjusted accordingly.


After each change to the table xhaus, the ue_master (or ue_server) and the dfue_starter must
be ended and started again.



        5.2.3.          Production site
For the order linking, it is necessary that the distributor be created as customer in the market
partner master data. Decisive for the linking of orders is the "EDI type" field on the "Delivery" tab.
This field has to be set to "VKKopplung."
Moreover, the dealer has to be entered in table xhaus with this customer number.
If the customer number of the distributor at the production site is not the same as the customer
number that was entered in the xhaus entry for the production site at the distributor, the
environment variable IB_KUEMPF has to be set at the production site.
We will not go into details regarding system configuration at this point. For the complete set-up of
the internal order linking, see section "Basic configuration"


        5.2.4.          Process
The complete internal process of transfer will not be depicted here, but rather only how it
appears from the user's point of view.
Basically, all order items entered at the distributor that bear the procurement type purchase
order and have been stored as suppliers of the associated production site, are transferred
automatically to the production site after release.
At the same time, depending on the configuration (environment variable IB_NOBESTINTBEST) at
the distributor, an internal PO with reference to this order is generated. It includes the associated
order number as third-party number and can thus also be called up in the order management via
the third-party number search ("F5" after entering order management) and the order number.
Employees can be informed via message about the success of generation of the PO and/or the
sending. (see also „Messages“).
The production system decides whether, what, and for when the order is intended using the
master data and the order data.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                   55
If orders are not released after entry, they are not transferred. They are reflected in the "release
pool" (menu: Sales/Release Order/Release) with the specified release note.
After transfer, the order appears in the production site. Via appropriate system configuration
(environment variable INTAUF_FREITEK) it is possible to control whether the orders in the
"release pool" (menu: Sales/Release Order/Release) received via internal order linking remain
marked with the note "EDI order" or are released directly. If the orders initially remain in the
"release pool," they must be released explicitly later (after they have been checked).
Employees can be informed via message about the success of order scheduling. (see also
„Messages“).
The order receives a new order number at the production site. Depending on the system
configuration (environment variable IB_EXREF), the order receives the order number and/or the
PO number of the sending site or the third-party number of the sending site. If the third-party
number includes the order number of the sending site, it is possible using the third-party number
search ("F5" after order entry) to find the order in the company's own system. Thus, the order can
be called up at the production site both using the company's own as well as the original number.
Depending on the system configuration (environment variable IB_XUSR, INTAUF_MANEU), the
user of the order at the production site is the employee '-1', that is, the system service or the
same one as at the distributor.
As soon as the order is released at the production site, the production planning and scheduling
takes place. If the date is thus shifted, this change is reported to the distributor (in the order
status), however the original order is not changed automatically. Depending on the configuration
of the Messages, there is also an active message to an employee.
As long as the order at the production site is not in a production job, changes can be made at the
distributor at any time (recognizable given the status "correction" at the top right on the entry
screen). These changes are transferred automatically and made at the production site. Any local
change at the production site is thus overwritten. Employees can be informed actively about the
receipt of an order change and an associated overwriting of a local change (see "Messages").
Only if the order is planned at the production site in a production job or if it is already in a
confirmed job (and thus receives the order status "fixed - local correction" or "produced - local
correction") is this status reported back to the distributor. Only starting at this moment are no
more changes possible without consulting production. That is, the person entering the order must
heed the status!
The following possibilities for order tracing are available:
( IS: 20/11/2018: Must be reworked!)
As explained above, in the order entry at the top right, the order status (correction status) is
displayed; this must absolutely be heeded.
Furthermore, in the order "SHIFT+F10" it is possible to see the order status (scheduling status).
Here you find information about whether and which site the order has been scheduled.
Furthermore, there is also information here about delivery date shifts, etc.
If in the order status you press "F2," then you will see additional statuses displayed (alternative:
menu "SHIFT+F4" -> order statuses).
In addition, in the item part, information about the finished (available), delivered and invoiced
quantities can be displayed by pressing "F2" twice in the item area.



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                    56
At the production site, furthermore, the EDI orders can be restricted in the "release pool" (menu:
Sales/Release Order) via the department number of the employee -1.
In connection with the EDI, various messages are sent by the system via the mail system.
Therefore, it is important to check the message receipt in the mail system regularly (incoming
messages are indicated by an envelope symbol in the left lower area of the screen, and there is
also an acoustic signal). However, it is recommended that you configure the system so that
system messages are sent as e-mails.
For the determination of document numbers in upstream and downstream sites, on the menu
Sales/Overview/Number Determination it is possible to display the document number at the
company's site insofar as only the number of the other site is known and to display the number at
the other site insofar as only the company's number is known.


        5.2.5.         SN File Transfer
CAUTION: If the transfer of SN files is configured, you must make sure that there is NO
adjustment of the SN file for purchased sub-elements. This way, no cutting correction is inserted
into the SN file and parts are removed that are not relevant for the sub-element purchased




A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                  57
6. PO transfer
    6.1.        Introduction
Within A+W Enterprise, there is a distinction between order linking and PO transfer. Parallel to
this is the "central quotation database."
To achieve as close a coupling between the distributor and production site with as much flexibility
as possible for changes, the PO transfer can be used.
In this context, there are different times at which a PO in the distributor may no longer be
changed. This time depends on the production organization in the production site and the close
nature of the coupling between distributor and production site.
During the PO transfer, a purchase order in the distributor becomes an order in the distributor
(sending site). This PO is then transferred to the production site (receiving site) and an
appropriate order is created there. Changes to the PO before the transfer are transferred to the
production site.
In this document, the terms "distributor" and "production site" will be used.
In connection with the PO transfer, "distributor" refers to the site that enters the PO. A distributor
is not exclusively a distribution branch office without its own production. A distributor can also
have its own production, but it orders products from another branch office from product lines or
for capacity reasons.
This is opposed to the "production site." This is the branch office that produces products for
upstream branch office and supplies them to the end customer or the upstream branch office.
The production site does not enter the end customer order. A production site is not exclusively a
production branch office without its own distribution. A production site can also have its own
distribution, however it receives POs from other branch offices for product line or capacity
reasons.
Thus, the definitions "distributor" and "production site" always only apply for a concrete PO for a
branch office.
The function of the "central quotation database" is available if the PO transfer or the order linking
is configured and the environment variable ANGBDB is set accordingly.
Prerequisite for the PO transfer is that the article master data in the trade and production site
are identical. There is no referencing of third-party numbers.
In case of different article master data, a PO transfer via the "A+W EDI Export" module can be
executed in the format of the standard interface. See also "A+W EDI-Export" using "B2B
Service" and A+W default order interface with i000filter.


    6.2.        Master data
        6.2.1.          Configuration Options
The definition of the individual settings is made under
System > Data Transfer > Transfer Document > Configuration


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                   58
Or in the market partner master data via the "EDI configuration" menu or F5 on the field "Type of
EDI."
With "Type of EDI" = 101 "PO transfer," currently the following settings are possible:


Control type         Name                      Description
1                    Direct PO transfer        Is set at the distributor's If a PO for an internal
                                               supplier is created automatically, it is provided
                                               immediately after completion by the intauf for
                                               the transfer (entry in the table intbest).This
                                               setting may not be used if you are working with
                                               grouping in the PO pool.
                                               ID 110318
                                               October 2024: alcib AND trm_ctrl
                                               The direct transfer can also be used for suppliers
                                               who are not on direct order
2                    Transaction-spanning      Is set at the distributor's Documents assigned to a
                     documents                 PO without position reference are transferred ID
                                               102235
                                               Note: The document types must be identical

3                    Item-specific             Is set at the distributor's Documents assigned to a
                     documents                 PO with position reference are transferred ID
                                               102235
                                               Note: The document types must be identical
5                    Individual number         Set at the production site
                     range
                                               If this configuration is set for a customer, the new
                                               number for the order to be scheduled is not
                                               obtained from the normal order number range
                                               "kaufex.mfo," but rather from the number range
                                               "kaufdfue."
                                               Caution: The number ranges kaufex.mfo and
                                               kaufdfue must absolutely be disjunct.
                                               This function cannot be used together with an
                                               offset!
                                               ID 132679
48                   Retention of local        Set at the production site
                     order fields
                                               If this configuration is set for a customer, in case
                                               of order changes via internal EDI, the local fields
                                               in kauf._private_* are retained. If this
                                               configuration is not set, the values will be taken
                                               over from the distributor.
                                               see also DISABLE_COPY_PRIVATE_CHAR1
                                               If this variable is set, with the first transfer and if


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                      59
                                               the configuration 48 is not activated, the field
                                               kauf._private_char1 is emptied.
                                               The private item fields (kposp.private*) or the
                                               configurable private fields (kaufprvfld, kposprvfld)
                                               remain unaffected by this.
                                               #454898
65                    No site assignment in    Is set at the distributor.
                      the call center
                                               If this configuration is set for a customer, on order
                                               scheduling via internal EDI, there is no automatic
                                               site assignment in the call center. The order
                                               remains in the release pool of the call center.
                                               See also "EN-CONFIG-A+W Enterprise EDI"
                                               section "Release pool"



         6.2.2.          Item master data
Prerequisite for the PO transfer is that the article master data in the trade and production site are
identical. There is no referencing of third-party numbers.
In case of different article master data, a PO transfer via the "A+W EDI Export" module can be
executed in the format of the standard interface. See also "A+W EDI-Export" using "B2B Service"
and A+W default order interface with i000filter.


         6.2.3.          Distributor
For the PO transfer, it is necessary that the production site be created as supplier in the market
partner master data. Decisive for the PO transfer is the "Type of EDI" field on the "Delivery" tab.
This field has to be set to "EK 1:1" or "EK 1:n."

Starting with version 2007:
In the EDI configuration ((F5 on the "Type of EDI" field or menu: System - Data Transfer - Transfer
Document – Configuration) it can be defined whether
     •   the internal PO should also be transferred immediately after it is created
     •   whether a document assigned to a PO should be transferred too (ID 102235)
Moreover, the production site has to be entered in table xhaus with the same supplier number.
Special attention must be paid to the correct creation of the fields kunr, linr, host, hausart,
hausart, subvers and patch as well as on the fact that these have a central effect on the PO
transfer.


         6.2.4.          At the production site
For the PO transfer, it is necessary that the distributor be created as customer in the market
partner master data. Decisive for the PO transfer is the "Type of EDI" field on the "Delivery" tab.
This field has to be set to "EK 1:1" or "EK 1:n."

A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                    60
Moreover, the dealer has to be entered in table xhaus with the same customer number.
(see also "Distributor")
After each change to the table xhaus, the ue_master (or ue_server) and the dfue_starter must be
ended and started again.
If the customer number of the distributor at the production site is not the same as the customer
number that was entered in the xhaus entry for the production site at the distributor, the
environment variable IB_KUEMPF has to be set at the production site.
We will not go into details regarding system configuration at this point. For a complete set-up of
the internal PO transfer, see "Basic configuration" and the "Environment variables" section at the
end of this document.




    6.3.        Process
The complete internal process of transfer will not be depicted here, but rather only how it
appears from the user's point of view.
For the system administrator and planner: Before beginning or changing a component
(trigger/start/local correction) in this process, please consider the whole process and read. All
components work together here.


    6.4. Release of transfer - Version 2007 up to
       AWE6 October 2024
In EDI control, it is now possible to define that the PO for a market partner shall be transferred
right after it has been generated. In this case, intauf enters all items of the PO into the table
intbest.
If a PO has already been transferred (status: PO transferred (503) exists), then changed, the intauf
enters this PO into the table intbest regardless of the configuration "direct PO transfer." It does
not do this if the PO is already on "local correction" (status: PO generated exists).
If a PO that should actually be transferred but is in local correction runs through intauf, the
message 46 is sent.
Subject: Incorrect PO transfer
Text: PO 4711 cannot be transferred. It was already released.
This can also happen with incorrect configuration.
If you are working with the configuration that the internal PO is created via the PO pool (direct
order in the supplier master data = no and MODUL_EINKAUF=3), then the PO will be placed into
local correction immediately upon generation. Variable DFUE_IB_BESTELLSPERRE may not be set!
Similarly, in this case, it may not be configured that the POs are transferred immediately after
generation. The transfer must be initiated separately by a report.
Caution: Depending on the configuration (DFUE_IB_BESTELLSPERRE) there can be a state in which
the PO was already transferred but the status "PO transferred" does not yet exist. In this case a



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 61
change is not transferred automatically; instead, it must be provided for the transfer like a newly
created PO.
Regardless of this function, a PO can be entered as previously via the special printing "internal PO
transfer" (report ekueb.rep) or manually into the table intbest.




    6.5.        Flexible control of the direct transfer
October 2024 and QR2406 (alcib and trm_ctrl)
Control of the automatic transfer and local correction has been reworked completely. It can now
be used esepecially flexibly within the internal client separation.


"Entry" field for POs:
For flexible control of the PO transfer and of local correction for POs, it is absolutely necessary to
recognize where a PO was generated. For this function, the previously unused field "Entry" in POs
is used. It can assume the following values:
0 – old PO
1- Manual
2 - PO pool
3 - Direct generation
You are urgently warned that this field may not be changed. It handles the central control of PO
transfer and booking of the local correction.


In EDI control, it is now possible to define that the PO for a market partner shall be transferred
right after it has been generated. This setting is only possible supplier-specifically or across
suppliers. A client-specific setting is not possible.
If the direct transfer is defined for a supplier, the background process "intauf" enters all items of
the PO into the table "intbest".
If for a client the environment variable DFUE_IB_BESTELLSPERRE is deactivated or equal to 0
(DRUCK) and at the same time direct transfer is defined, then the PO is only provided by "intauf"
for the transfer if the PO is generated via the PO pool and not yet transferred. Another transfer
after a manual change to a PO generated via the PO pool does not happen.
If an internal PO is created via the PO pool, then the PO will be set to local correction immediately
after generation. If in this case direct transfer is set for the supplier, then the PO is provided once
for the transfer regardless of the environment variable DFUE_IB_BESTELLSPERRE (until the status
"Transfer PO").
If a PO has already been transferred (status: PO transferred (503) exists), then changed, the intauf
enters this PO into the table intbest regardless of the configuration "direct PO transfer" as long as
the PO is not in local correction (Status: PO generated exists).
If a PO that should actually be transferred has the incorrect status, the message 46 is sent.
Subject: Incorrect PO transfer


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                    62
Caution: Depending on the configuration (DFUE_IB_BESTELLSPERRE) there can be a state in which
the PO was already transferred but the status "PO transferred" does not yet exist. In this case a
change is not transferred automatically; instead, it must be provided for the transfer like a newly
created PO.
Regardless of the "direct transfer" function, a PO can be entered as previously via the special
printing "internal PO transfer" (report ekueb.rep) or manually into the table "intbest." However,
the configuration of DFUE_IB_BESTELLSPERRE must be heeded here.
It is not recommended that status bookings be made by yourself using scripts or reports on the
configuration. This can hinder control of the local correction and cause errors.

See also the explanations about the individual settings of DFUE_IB_BESTELLSPERRE further below


    6.6.        Local correction (DFUE_IB_BESTELLSPERRE)
An overall process observation between distributor and production site is absolutely mandatory
for this. If internal POs are executed for various internal suppliers, it must be noted that the
environment variable DFUE_IB_BESTELLSPERRE cannot be defined supplier-specifically and site-
specifically.

October 2024 + QR 2406 (alcib and trm_ctrl): The environment variable DFUE_IB_BESTELLSPERRE
can now be set client-specifically. However, this is not recommended and must be tested
intensively with the individual business process

See also the explanations about the individual settings of DFUE_IB_BESTELLSPERRE further below

In addition, it should be noted that the environment variable BESTELLFREIGABE is only relevant
for external POs and has no effects on the internal POs.

There are currently several ways:
•   Locking the PO before the start                    of   the    transfer    by    the    user
    (DFUE_IB_BESTELLSPERRE=0 or not active)
•   Locking the PO on start of the transfer by the system (DFUE_IB_BESTELLSPERRE=1)
•   Locking the PO after successful order scheduling in the production site by the
    system (DFUE_IB_BESTELLSPERRE=2)
•   Locking the PO after the status 101 "STATUS_PMS" was transferred from the
    production site to the distributor. (DFUE_IB_BESTELLSPERRE=3)
•   Locking the PO after the status 300 "FIXED" was transferred from the production
    site to the distributor. (DFUE_IB_BESTELLSPERRE=4)
•   Locking the PO after the status 302 "RELEASED" was transferred from the
    production site to the distributor. (DFUE_IB_BESTELLSPERRE =5)

Prerequisite: Configuration of the status reporting from the production site to the distributor (call
of the script SDFUEDIR/bin/rueckmeld)


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                 63
QR 2403 // trm_ctrl - 13.04.10213

If within the production site a status has been reset (PO release, job creation), then this
cancellation of a status is not transferred to the distributor. This way, an existing local correction
could not be eliminated there. With the new trm_ctrl, canceled status bookings can also be
transferred to the distributor. In the distributor, a transfer of a cancelled status only causes a
cancellation of the status of the local correction of the PO if DFUE_IB_BESTELLSPERRE >= 4.

QR 2406 // alcib - 13.04.17435

If internal POs and thus also the corresponding order items go into "local correction", this
depends on the system configuration described here. Thus there are also various possibilities for
resetting the "local correction" of an internal PO.

If internal POs are set into local correction very early (printing (0) to scheduling (3)), a resetting is
now only possible by cancelling the PO in the PO management. Here, you must ensure in advance
that the resulting production order was also cancelled in the production client so that it is not
produced twice. When cancelling the internal PO, there is an appropriate query about this.

If an internal PO is only set into "local correction" with the job creation or release, this status can
only be reset by cancelling the status in the production site.

Points to be clarified:

How are internal POs generated?

If internal POs are created via the PO pool, they are in local correction right away. In this case,
DFUE_IB_BESTELLSPERRE may not be set !=0.

October 2024 / QR2406: If a PO is generated via the PO pool, this is set immediately into local
correction regardless of DFUE_IB_BESTELLSPERRE and it is also transferred once. Both direct
transfer and manual initiation are possible.

When should an internal PO go into local correction?

If a PO is in local correction, a transfer of changes is no longer possible. Cancellations will also no
longer be transferred. It must be clarified between the distributor and production site how
planning will be done and by when changes may be transferred.

How does the start of the transfer work?

If the start of the transfer of the PO is done via the Form print menu element or if a generated PO
should be transferred immediately (see "configuration possibilities - direct PO transfer").

November 2020: If the POs are initiated via printing for transfer and DFUE_IB_BESTELLSPERRE > 0,
then the PO no longer goes into local correction even if BESTELLFREIGABE = 2. The environment
variable BESTELLFREIGABE applies for more than external POs.

October 2024 / QR2406: A direct transfer is also possible for PO pool POs.



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                      64
When is scheduling done in the production site?

Are internal orders in the production site released directly or only with manual release? Which
effects would changes after release for production planning have?

How does production planning work?

If pots are generated for planning, it must be noted that this does not trigger any reporting to
AWE. When will a job be created? Which effects would a change between pot creation and job
generation have?

Only when all of these questions are clarified is it possible to decide how the environment
variable DFUE_IB_BESTELLSPERRE must be set.



Starting with version 2007: AWD #110318

If internal POs are handled via the PO pool, this variable may not be > 0!!!
(only applicable until October 2024)
Up to AWE6 alcib November 2020: Similarly, the PO transfer is via the
printout.
In order to enable a change transfer of POs, the environment variable DFUE_IB_BESTELLSPERRE
must be set accordingly.
If the variable DFUE_IB_BESTELLSPERRE is not set, then a transfer of the PO only takes place if the
PO was released manually before a transfer and is thus in "local correction."
If a PO is in local correction, a cancellation is also not transferred
If you are working with the configuration that the internal PO is created via the PO pool (direct
order in the supplier master data = no and MODUL_EINKAUF=3), then the PO will be placed into
local correction immediately upon generation. Variable DFUE_IB_BESTELLSPERRE may not be set
(until October 2024). Similarly, in this case, it may not be configured that the POs are transferred
immediately after generation (until October 2024). The transfer must be initiated separately by a
report.


        6.6.1.           DFUE_IB_BESTELLSPERRE = OFF

        6.6.2.           Direct order yes and direct transfer yes
This setting is not recommended.
Disadvantage:
    -   Many error e-mails
    -   A lot of manual reworking/manual release and transfer to separate work steps or via
        customizing.
    -   No change and cancellation transfer: Here there is a risk that during cancellation of the
        order at the distributor, the dependent order in the production site is not cancelled!


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                   65
    -   Cancellation of the info status from production site is not cancelled at the distributor
Advantages:
    -   order-related POs are generated immediately and changed for order changes.


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately and changed for order changes (direct order: yes). Since direct transfer is on "yes,"
the background process "intauf" also tries to provide the PO directly for the transfer. Since the PO
is not in local correction, however, this is not possible (DFUE_IB_BESTELLSPERRE = OFF). The e-
mail 46 Subject: PO transfer failed is sent.
The PO can then be approved manually and provided manually or via printing for the transfer.
Here there is a risk that during cancellation of the order at the distributor, the dependent order in
the production site is not cancelled!


Manual:
If a PO is entered manually, the background process "intauf" tries to provide the PO directly for
the transfer. Since the PO is not in local correction, however, this is not possible
(DFUE_IB_BESTELLSPERRE = OFF). The e-mail 46 Subject: PO transfer failed is sent.
The PO can then be approved manually or via printing and provided manually or via printing for
the transfer.


Purchase order pool:
The supplier can be entered manually in the PO pool. If the PO is processed by "intauf," it provides
the PO for transfer. Since orders from the PO pool are in local correction immediately, the PO is
transferred.
Problem at this point: If the status booking was not booked by rserv, the PO will also not be
written to intbest. The user is informed about this via system mail no. 46. The PO can then be
approved manually or via printing or provided via printing for the transfer.
Here there is a risk that during cancellation of the order at the distributor, the dependent order in
the production site is not cancelled!




        6.6.3.          Direct order yes and direct transfer no
This setting is not recommended.
Disadvantage:
    -   Manual release and transfer to separate work steps or via customizing.
    -   No change and cancellation transfer
Advantages:


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                66
    -   order-related POs are generated immediately and changed for order changes.


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately and changed for order changes (direct order: yes).
The PO can then be approved manually and provided manually or via printing for the transfer.
Manual:
If a PO can be entered manually, it can then be approved manually and pprovided manually or via
printing for the transfer.
Purchase order pool:
The supplier can be entered manually in the PO pool. The PO can then be approved manually and
provided manually or via printing for the transfer.



        6.6.4.          Direct order no and direct transfer yes
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
    -   Error e-mails and other process for manual POs
    -   PO pool POs are not always transferred immediately and must be initiated manually
Advantages:
    -   Order-related POs are transferred immediately after generation


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, the background process "intauf" tries to provide the PO directly for
the transfer. Since the PO is not in local correction, however, this is not possible
(DFUE_IB_BESTELLSPERRE = OFF). The e-mail 46 Subject: PO transfer failed is sent.
The PO can then be approved manually and provided manually or via printing for the transfer.
Purchase order pool:
A triggered PO will be provided immediately for transfer
Problem at this point: If the status booking was not booked by rserv, the PO will also not be
written to intbest. The user is informed about this via system mail no. 46.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                 67
        6.6.5.          Direct order no and direct transfer no
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
    -   Different processes for order-related and manual POs
Advantages:
    -   Complete process control by the user
    -
Order-related
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO can be entered manually, it can then be approved manually and pprovided manually or via
printing for the transfer.
Purchase order pool:
A triggered PO can then be provided manually or via printing for the transfer.


The following statuses will be written:
Order: When generating the PO, the status 502 – PO generated (info follow-up document) is
written for the order. At the same time, for each item of the order that exists in the PO, a status
301 - PO is generated (lock).
PO: When generating the PO, the status 301- PO generated (lock) is written for the PO.
        During the transfer of the PO, immediately after starting the transfer, the status 503 –
PO transferred for the PO is written. Starting from this point in time, the PO can no longer be
transferred again.



        6.6.6.          DFUE_IB_BESTELLSPERRE = 0 when printing
The internal PO generated is set to "local correction" by printing. At the same time, all items in
the PO of the order associated with the PO are set to "local correction" in the order.
After that, the PO can be transferred until the receipt for successful scheduling in the sending site
has been booked from the receiving site.


        6.6.7.          Direct order yes and direct transfer yes
This setting is not recommended.
Disadvantage:
    -   Many error e-mails

A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  68
    -   Manual release and transfer
    -   No change and cancellation transfer
Advantages:
    -   order-related POs are generated immediately and changed for order changes.


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately and changed for order changes (direct order: yes). Since direct transfer is on "yes,"
the background process "intauf" also tries to provide the PO directly for the transfer. Since the PO
is not in local correction, however, this is not possible (DFUE_IB_BESTELLSPERRE = 0). The e-mail
46 Subject: PO transfer failed is sent.
The PO can then be approved via printing and provided for the transfer.
Manual:
If a PO is entered manually, the background process "intauf" tries to provide the PO directly for
the transfer. Since the PO is not in local correction, however, this is not possible
(DFUE_IB_BESTELLSPERRE = 0). The e-mail 46 Subject: PO transfer failed is sent.
The PO can then be approved via printing and provided for the transfer.
Purchase order pool:
The supplier can be entered manually in the PO pool. If the PO is processed by "intauf," it provides
the PO for transfer. Since orders from the PO pool are in local correction immediately, the PO is
transferred.



        6.6.8.          Direct order yes and direct transfer no
This setting is not recommended.
Disadvantage:
    -   Manual release and transfer
    -   No change and cancellation transfer
Advantages:
    -   order-related POs are generated immediately and changed for order changes.


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately and changed for order changes (direct order: yes).
The PO can then be approved via printing and provided for the transfer.
Manual:
If a PO is entered manually, it can then be approved via printing and provided for the transfer.
Purchase order pool:


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                69
The supplier can be entered manually in the PO pool. The PO can then be approved manually and
provided manually or via printing for the transfer.



        6.6.9.          Direct order no and direct transfer yes
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
    -   Error e-mails and other process for manual POs
Advantages:
    -   Order-related POs are transferred immediately after generation


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, the background process "intauf" tries to provide the PO directly for
the transfer. Since the PO is not in local correction, however, this is not possible
(DFUE_IB_BESTELLSPERRE = 0). The e-mail 46 Subject: PO transfer failed is sent.
The PO can then be approved via printing and provided for the transfer.
Purchase order pool:
A triggered PO will be provided immediately for transfer



        6.6.10.         Direct order no and direct transfer no
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
    -   Different processes for order-related and manual POs
Advantages:
    -   Complete process control by the user
Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, it can then be approved via printing and provided for the transfer.



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                 70
Purchase order pool:
A triggered PO can then be provided manually or via printing for the transfer.


The following statuses will be written:
Order: For the generation of the PO, no additional status is written.
        When printing the PO, a status 502 – PO generated (info follow-up document) is written.
At the same time, for each item of the order that is present in the PO, a status 306 – PO printed
and 301 – PO release (lock) are written.
Order: For the generation of the PO, no additional status is written.
        When printing the PO, a Status 306 – PO printed and a status 301 – PO released (lock)
are written. No statuses are written for the items.
        If the receipt for a successful scheduling is booked, the Status 503 – PO transferred for
the PO is written. Starting from this point in time, the PO can no longer be transferred again.



        6.6.11.         DFUE_IB_BESTELLSPERRE =1 when sending
If internal POs are handled via the PO pool, this variable may not be > 0!!! (only until October
2024)
Up to AWE6 alcib November 2020: Similarly, the PO transfer is via the printout.
The internal PO generated is set to "local correction" by the start of the transfer. At the same
time, all items in the PO of the order associated with the PO are set to "local correction" in the
order.
After that, the PO can be transferred until the receipt for successful scheduling in the sending site
has been booked from the receiving site.


        6.6.12.         Direct order yes and direct transfer yes
This setting is not recommended.
Disadvantage:
    -   No change and cancellation transfer
    -   Order is in local correction immediately after release
Advantages:
    -   Order-related POs are generated and transferred immediately


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately (direct order: yes). Since direct transfer is on "yes," the background process "intauf"
also tries to provide the PO directly for the transfer. As soon as the transfer starts, the PO and
thus the order are put in local correction.


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  71
Manual:
If a PO is entered manually, the background process "intauf" provides the PO directly for the
transfer. As soon as the transfer starts, the PO is put in local correction.
Purchase order pool:
The supplier can be entered manually in the PO pool. If the PO is processed by "intauf," it provides
the PO for transfer. The PO is transferred.


        6.6.13.         Direct order yes and direct transfer no
This setting is OK
Disadvantage:
    -   Manual transfer
    -   No change and cancellation transfer
Advantages:
    -   order-related POs are generated immediately and changed for order changes.


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately and changed for order changes (direct order: yes).
The PO can then be approved via printing or manually or provided manually for the transfer. As
soon as the transfer starts, the PO and thus the order are put in local correction.


Manual:
If a PO is entered manually, it can then be provided via printing or manually for the transfer. As
soon as the transfer starts, the PO is put in local correction.


Purchase order pool:
The supplier can be entered manually in the PO pool. The PO can then be approved manually and
provided manually or via printing for the transfer.



        6.6.14.         Direct order no and direct transfer yes
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
Advantages:
    -   POs are transferred immediately after generation



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  72
Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, the background process "intauf" provides the PO directly for the
transfer. As soon as the transfer starts, the PO is put in local correction.
Purchase order pool:
A triggered PO will be provided immediately for transfer



        6.6.15.         Direct order no and direct transfer no
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
Advantages:
    -   Complete process control by the user
Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, it can then be provided via printing or manually for the transfer.


Purchase order pool:
A triggered PO can then be provided manually or via printing for the transfer.


The following statuses will be written:
Order: For the generation of the PO, no additional status is written.
        When printing the PO, no additional status is written for the order. At the same time, for
each item of the order that is present in the PO, a status 306 – PO printed is written.
          When the export of the PO is finished, the status 502 – PO generated (info follow-up
document) is written for the order. At the same time, for the items of status 301 – PO generated
(lock) is written.
Order: For the generation of the PO, no additional status is written.
        When printing the PO, a Status 306 – PO written is written for the PO. No statuses are
written for the items.
         When the export of the PO is finished, the status 301 – PO released (lock) is written. At
this point in time, the PO has not yet been scheduled in the receiving site.



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  73
        If the receipt for a successful scheduling is booked, the Status 503 – PO transferred for
the PO is written. Starting from this point in time, the PO can no longer be transferred again.



        6.6.16.   DFUE_IB_BESTELLSPERRE =2 receipt for the
            scheduling in the receiving site booked in the sending site
The internal PO generated is set to "local correction" by the confirmation of the successful
scheduling (not release) at the receiving site. At the same time, all items in the PO of the order
associated with the PO are set to "local correction" in the order. Up to this point in time, the PO
can be changed and transferred.
If internal POs are handled via the PO pool, this variable may not be > 0!!! (until October 2024)
Up to AWE6 alcib November 2020: Similarly, the PO transfer is via the printout.


        6.6.17.         Direct order yes and direct transfer yes
This setting is not recommended.
Disadvantage:
    -   No change and cancellation transfer
    -   Order is in local correction immediately after release
Advantages:
    -   Order-related POs are generated and transferred immediately


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately (direct order: yes). Since direct transfer is on "yes," the background process "intauf"
also tries to provide the PO directly for the transfer. As soon as the transfer starts, the PO and
thus the order are put in local correction.
Manual:
If a PO is entered manually, the background process "intauf" provides the PO directly for the
transfer. As soon as the transfer starts, the PO is put in local correction.
Purchase order pool:
The supplier can be entered manually in the PO pool. If the PO is processed by "intauf," it provides
the PO for transfer. The PO is transferred.


        6.6.18.         Direct order yes and direct transfer no
This setting is OK
Disadvantage:
    -   Manual transfer



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  74
    -   No change and cancellation transfer
Advantages:
    -   order-related POs are generated immediately and changed for order changes.


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately and changed for order changes (direct order: yes).
The PO can then be approved via printing or manually or provided manually for the transfer. As
soon as the transfer starts, the PO and thus the order are put in local correction.


Manual:
If a PO is entered manually, it can then be provided via printing or manually for the transfer. As
soon as the transfer starts, the PO is put in local correction.


Purchase order pool:
The supplier can be entered manually in the PO pool. The PO can then be approved manually and
provided manually or via printing for the transfer.



        6.6.19.         Direct order no and direct transfer yes
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
Advantages:
    -   POs are transferred immediately after generation


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, the background process "intauf" provides the PO directly for the
transfer. As soon as the transfer starts, the PO is put in local correction.
Purchase order pool:
A triggered PO will be provided immediately for transfer




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  75
        6.6.20.          Direct order no and direct transfer no
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
Advantages:
    -   Complete process control by the user
Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, it can then be provided via printing or manually for the transfer.


Purchase order pool:
A triggered PO can then be provided manually or via printing for the transfer.


The following statuses will be written:
Order: For the generation of the PO, no additional status is written.
When printing the PO, no additional status is written for the order. At the same time, for each
item of the order that is present in the PO, a status 306 – PO printed is written.
During the export of the PO, no additional status is written.
If the receipt for a successful scheduling is booked, the Status 502 – PO generated (info follow-up
document) is written. At the same time, for the items of status 301 – PO generated (lock) is
written.
Order: For the generation of the PO, no additional status is written.
When printing the PO, a Status 306 – PO printed is written for the PO. No statuses are written for
the items.
During the export of the PO, no additional status is written.
If the receipt for a successful scheduling is booked, the status 301 – PO released (lock) and 503 –
PO transferred for the PO are written. Starting from this point in time, the PO can no longer be
transferred again.



        6.6.21.   DFUE_IB_BESTELLSPERRE =3 PMS- receipt for the
            production scheduling in the receiving site booked in the
            sending site
The internal PO generated is set by the booking of the status "production scheduling" from the
production site in the distributor in the receiving site to "local correction." At the same time, all


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                    76
items in the PO of the order associated with the PO are set to "local correction" in the order. Up
to this point in time, the PO can be changed and transferred.
If internal POs are handled via the PO pool, this variable may not be > 0!!! (until October 2024)
Up to AWE6 alcib November 2020: Similarly, the PO transfer is via the printout.


        6.6.22.         Direct order yes and direct transfer yes
This setting is only recommended if the production site approves internal orders manually.
(environment variable: INTAUF_FREITEK)
Disadvantage:
    -   If release is made directly in the production site, then there are no change and
        cancellation transfer
    -   If release is made directly in the production site, the order is in local correction
        immediately after release
Advantages:
    -   Order-related POs are generated and transferred immediately
    -   with manual release in the production site, also change and cancellation transfer


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately (direct order: yes). Since direct transfer is on "yes," the background process "intauf"
also tries to provide the PO directly for the transfer. As soon as the order was scheduled in the
production site, the PO and thus the order is placed in local correction.
Manual:
If a PO is entered manually, the background process "intauf" provides the PO directly for the
transfer. As soon as the order was scheduled in the production site, the PO is placed in local
correction.
Purchase order pool:
The supplier can be entered manually in the PO pool. If the PO is processed by "intauf," it provides
the PO for transfer. The PO is transferred.


        6.6.23.         Direct order yes and direct transfer no
This setting is OK (environment variable: INTAUF_FREITEK)
Disadvantage:
    -   Manual transfer
    -   If release is made directly in the production site, then there are no change and
        cancellation transfer
    -   If release is made directly in the production site, the order is in local correction
        immediately after release
Advantages:

A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  77
    -   Order-related POs are generated and transferred immediately
    -   with manual release in the production site, also change and cancellation transfer


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately and changed for order changes (direct order: yes).
The PO can then be approved via printing or manually or provided manually for the transfer. As
soon as the order was scheduled in the production site, the PO and thus the order is placed in
local correction.


Manual:
If a PO is entered manually, it can then be provided via printing or manually for the transfer. As
soon as the order was scheduled in the production site, the PO is placed in local correction.


Purchase order pool:
The supplier can be entered manually in the PO pool. The PO can then be approved manually and
provided manually or via printing for the transfer.



        6.6.24.         Direct order no and direct transfer yes
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
Advantages:
    -   POs are transferred immediately after generation


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, the background process "intauf" provides the PO directly for the
transfer. As soon as the order was scheduled in the production site, the PO is placed in local
correction.
Purchase order pool:
A triggered PO will be provided immediately for transfer




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  78
        6.6.25.         Direct order no and direct transfer no
This setting is OK
Disadvantage:
    -   No change and cancellation transfer
Advantages:
    -   Complete process control by the user
Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, it can then be provided via printing or manually for the transfer. As
soon as the order was scheduled in the production site, the PO is placed in local correction.
Purchase order pool:
A triggered PO can then be provided manually or via printing for the transfer.


The following statuses will be written:
Order: When generating the PO, no additional status is written.
        When printing the PO, no additional status is written for the order. At the same time, for
each item of the order that is present in the PO, a status 306 – PO printed is written.
        During the export of the PO, no additional status is written.
       If the receipt for a successful scheduling of the PO is booked, no additional status is
booked for the order.
If in the receiving site the status 101 – PMS-receipt (or higher up to 499) is booked and then
booked in the sending site, status 502 – PO generated (info follow-up document) is written for the
order. At the same time, for the items of status 301 – PO generated (lock) is written.


Order: For the generation of the PO, no additional status is written.
When printing the PO, a Status 306 – PO printed is written for the PO. No statuses are written for
the items.
During the export of the PO, no additional status is written.
If the receipt for a successful scheduling is booked, the Status 503 – PO transferred for the PO is
written.
If in the receiving site the status 101 – PMS-receipt (or higher up to 499) is booked and then
booked in the sending site, status 301 – PO generated (lock) is written.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                   79
        6.6.26.   DFUE_IB_BESTELLSPERRE =4 PMS- fixed via the
            production job creation in the receiving site booked in the
            sending site
The internal PO generated is set by the booking of the status "job creation" from the production
site in the distributor in the receiving site to "local correction." At the same time, all items in the
PO of the order associated with the PO are set to "local correction" in the order. Up to this point
in time, the PO can be changed and transferred.
Caution: With this configuration, the triggering of a PO at the receiving site does not trigger local
correction at the sending site. Only a PO release at the receiving site triggers the local correction
If internal POs are handled via the PO pool, this variable may not be > 0!!! (until October 2024)
Up to AWE6 alcib November 2020: Similarly, the PO transfer is via the printout.


        6.6.27.          Direct order yes and direct transfer yes
This setting is recommended.
Disadvantage:
    -   Complete automation. Everyone must adhere to the processes
    -   Manual changes/planning will be overwritten by changes at the distributor
Advantages:
    -   Complete automation
    -   Order-related POs are generated and transferred immediately
    -   Change and cancellation transfer
    -   Complete flexibility


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately (direct order: yes). Since direct transfer is on "yes," the background process "intauf"
also tries to provide the PO directly for the transfer. Changes to the order are also transferred
immediately to the PO and production order after release.
If in the production site the order is planned in a job or if a PO is released, the PO and the order at
the distributor are set into local correction. If the job is dissolved again or the PO canceled/reset,
then the PO and order at the distributor are free again.
Manual:
If a PO is entered manually, the background process "intauf" provides the PO directly for the
transfer. Changes are also transferred immediately to the production order
Purchase order pool:
The supplier can be entered manually in the PO pool. If the PO is processed by "intauf," it provides
the PO for transfer. The PO is transferred.



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                      80
        6.6.28.         Direct order yes and direct transfer no
This setting is OK
Disadvantage:
    -   Manual transfer
    -   Manual changes/planning will be overwritten by changes at the distributor
Advantages:
    -   Order-related POs are generated immediately
    -   Change and cancellation transfer
    -   Complete flexibility


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is generated
immediately and changed for order changes (direct order: yes).
The PO can then be approved via printing or manually or provided manually for the transfer. If
there are changes to the order after the transfer, these are transferred directly


Manual:
If a PO is entered manually, it can then be provided via printing or manually for the transfer. If
there are changes to the PO after the transfer, these are transferred directly


Purchase order pool:
The supplier can be entered manually in the PO pool. The PO can then be approved manually and
provided manually or via printing for the transfer.



        6.6.29.         Direct order no and direct transfer yes
This setting is OK
Disadvantage:
    -   No change and cancellation transfer for order-related POs
Advantages:
    -   POs are transferred immediately after generation


Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  81
If a PO is entered manually, the background process "intauf" provides the PO directly for the
transfer. If there are changes to the PO after the transfer, these are transferred directly
Purchase order pool:
A triggered PO will be provided immediately for transfer



        6.6.30.         Direct order no and direct transfer no
This setting is OK
Disadvantage:
    -   No change and cancellation transfer for order-related POs
Advantages:
    -   Complete process control by the user
Order-related:
If an order with purchased parts is entered, after release of the order, the PO is not generated
immediately, but rather placed in the PO pool.
Manual:
If a PO is entered manually, it can then be provided via printing or manually for the transfer. If
there are changes to the PO after the transfer, these are transferred directly
Purchase order pool:
A triggered PO can then be provided manually or via printing for the transfer.


The following statuses will be written:
Order: When generating the PO, no additional status is written.
        When printing the PO, no additional status is written for the order. At the same time, for
each item of the order that is present in the PO, a status 306 – PO printed is written.
        During the export of the PO, no additional status is written.
       If the receipt for a successful scheduling of the PO is booked, no additional status is
booked for the order.
        If in the receiving site the status 300 – PMS fixed (or higher up to 499) is booked and then
booked in the sending site, status 502 – PO generated (info follow-up document) is written for the
order. At the same time, for the items of status 301 – PO generated (lock) is written.


Order: For the generation of the PO, no additional status is written.
When printing the PO, a Status 306 – PO printed is written for the PO. No statuses are written for
the items.
During the export of the PO, no additional status is written.
If the receipt for a successful scheduling is booked, the Status 503 – PO transferred for the PO is
written.


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                   82
If in the receiving site the status 300 – PMS fixed (or higher up to 499) is booked and then booked
in the sending site, status 301 – PO generated (lock) is written.
Caution: With this configuration, the triggering of a PO at the receiving site does not trigger local
correction at the sending site. Only a PO release triggers the local correction



        6.6.31.     DFUE_IB_BESTELLSPERRE =5 PMS- released via the
            production job confirmation in the receiving site booked
            in the sending site
This configuration is no longer supported. If necessary, the entire workflow
must be discussed with development.
The internal PO generated is set by the booking of the status "job confirmation" from the
production site in the distributor in the receiving site to "local correction." At the same time, all
items in the PO of the order associated with the PO are set to "local correction" in the order. Up
to this point in time, the PO can be changed and transferred.
Caution: With this configuration, the triggering of a PO at the receiving site does not trigger local
correction at the sending site. Only a PO release triggers the local correction
If internal POs are handled via the PO pool, this variable may not be > 0!!! (until October 2024)
Up to AWE6 alcib November 2020: Similarly, the PO transfer is via the printout.
This configuration is not recommended since the transfer of changes for production orders
already in local correction is questionable and causes increased communication and correction
effort.
The following statuses will be written:
Order: When generating the PO, no additional status is written.
        When printing the PO, no additional status is written for the order. At the same time, for
each item of the order that is present in the PO, a status 306 – PO printed is written.
        During the export of the PO, no additional status is written.
       If the receipt for a successful scheduling of the PO is booked, no additional status is
booked for the order.
        If in the receiving site the status 302 – PMS release (or higher up to 499) is booked and
then booked in the sending site, status 502 – PO generated (info follow-up document) is written
for the order. At the same time, for the items of status 301 – PO generated (lock) is written.


Order: For the generation of the PO, no additional status is written.
When printing the PO, a Status 306 – PO printed is written for the PO. No statuses are written for
the items.
During the export of the PO, no additional status is written.
If the receipt for a successful scheduling is booked, the Status 503 – PO transferred for the PO is
written.


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                    83
If in the receiving site the status 302 – PMS release (or higher up to 499) is booked and then
booked in the sending site, status 301 – PO generated (lock) is written.
Caution: With this configuration, the triggering of a PO at the receiving site does not trigger local
correction at the sending site. Only a PO release triggers the local correction


    6.7.        Cancellation – Version 2007
If a PO is canceled (manually or by the system (supplier change in order)), the cancellation is
transferred as long as the PO is not in local correction. If the PO is already in local correction, the
cancellation is not transferred.
If a cancellation is transferred although the associated order is already in local correction in the
receiving site, the order will not be cancelled and appropriate messages will be sent (see
"Messages in the EDI").




    6.8.        Special features of program behavior
        6.8.1.     Changes in the order/PO after successful PO
            transfer
The following requirements must be met:
In the distributor, an order A with PO items must be entered for an internal supplier. For this, a
PO B is generated at the distributor and it is then transferred to the production site so that an
associated order C was generated there.
If in the production site no locks were set and transferred, in case of subsequent changes (header
or item level), the following happens:
    •   If order A is changed, whether in the order header, in a PO item or in a production item,
        then PO B is updated according to the current data in order A. Order C in the production
        site is then updated according to the current data in PO B.
    •   If PO B is changed, order C is updated at the production site according to the current data
        in PO B.
    •   Changes in order C have no effects on the data in order A or PO B.
    •   Order A, PO B, order C form a chain in which a change made later further forward in the
        chain overwrites each change made earlier further backward in the chain. Here it is not
        important whether the change in a document affects the process header or a particular
        item.
        Whether a change is transferred from the distributor to the production site and there
        causes a change of the corresponding order is controlled by several factors. The main
        factor is the "local correction" of the PO or of the production order. For more
        information, see the "Local correction (DFUE_IB_BESTELLSPERRE) section. In addition,
        during the change of a production order, there is also a check by the internal document
        transfer of the status "303 - Dispatch planning". If it is present for an order to be changed,
        the change is rejected and the message 55 sent.


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                      84
Example:
Status 1:
  Item      Order A                        PO B                  Order C
  1         12 pcs. (purchase order)       12 pcs.               12 pcs. (production)
  2         4 pcs. (purchase order)        4 pcs.                4 pcs. (production)
  3         20 pcs. (production)


=> change in PO B: item 1 now 18 pcs.


Status 2:
  Item      Order A                        PO B                  Order C
  1         12 pcs. (purchase order)       18 pcs.               18 pcs. (production)
  2         4 pcs. (purchase order)        4 pcs.                4 pcs. (production)
  3         20 pcs. (production)


=> Change in order C: item 2 now 2 pcs.


Status 3:
  Item      Order A                        PO B                  Order C
  1         12 pcs. (purchase order)       18 pcs.               18 pcs. (production)
  2         4 pcs. (purchase order)        4 pcs.                2 pcs. (production)
  3         20 pcs. (production)


=> Change in order A: item 3 now 50 pcs.


Status 4:
  Item      Order A                        PO B                  Order C
  1         12 pcs. (purchase order)       12 pcs.               12 pcs. (production)
  2         4 pcs. (purchase order)        4 pcs.                4 pcs. (production)
  3         50 pcs. (production)




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                    85
    6.9.        Functional range
        6.9.1.    Determination of the order number at the
            production site (iboffset, own number range)
At the production site, the orders to be scheduled receive the next free order number from the
local order number range.
Deviating from this, it is possible to configure the system so that the order number is determined
depending on the sending site. For this, in the table xhaus, in the record for the sending site, the
field iboffset is set to a value greater than "0" (zero). With this setting, for the processes that are
received from the site, the local order number is calculated from the sent number plus
xhaus.iboffset.
It must be noted that the local number range for the manual order entry and the individual
number ranges that arise from the settings in xhaus do not overlap.
If the calculated number already exists (e.g. in case of overlap of number ranges) but this is not a
change transfer, the scheduling is cancelled with an appropriate error message. Message 58 is
sent.
In addition, with this configuration it can happen that due to multiple changes at the distributor
(e.g. supplier changes), an order should be scheduled that was already cancelled (ID 120220). In
this case, the previously canceled document is "reactivated." This situation will be recorded in the
"changes" log with mode 13 "Cancellation deleted."
The "Offset function" may not be used with breakage orders within order coupling.
Furthermore, this function cannot be used within the order coupling for multisite installations if
several internal suppliers are used in an order.
Furthermore, it can be configured for internal EDI that the new order number is used from a
separate number range. (see "Configuration options")
If this configuration is set for a customer, the new number for the order to be scheduled is not
obtained from the normal order number range "kaufex.mfo," but rather from the number range
"kaufdfue." It is not possible to define an individual number range per customer. Here there is no
distinction whether the order was transferred via order linking or PO transfer.
Caution: The number ranges kaufex.mfo and kaufdfue must absolutely be disjunct.


If the newly assigned number already exists (e.g. in case of overlap of number ranges) but this is
not a change transfer, the scheduling is cancelled with an appropriate error message. Message 58
is sent.
This function cannot be used together with an offset! (ID 132679)


        6.9.2.           Route finding
#196831 - MODUL_REGIONALROUTEN
When orders are created after an internal transfer, the route defined by the sending site can be
adopted. This is done by setting the switch INTAUF_ROUTEALT or
INTAUF_ROUTEALT_DIREKTAUSLIEFERUNG and INTAUF_ROUTEALT_HAUSART. The direct or

A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                      86
collection route can also be defined for the receiving site in general (switch
INTAUF_DIREKTROUTE and INTAUF_ABHOLROUTE or by defining the corresponding routes at the
receiving site) to automate the setting of the new route at the receiving site.

If the route shall not be adopted from the sending site, it will be determined at the receiving site
as described in item "Calculation and optimization in background" (see "EN-CONFIG-A+W
Enterprise" - section "Shipping region"). You can define per client (irrespective of the setting
described in "Calculation and optimization in background") whether the date requested by the
customer or the route priority shall be the decisive factor for route selection.
Transferred orders that shall be directly shipped from production site to customer (the order has
been defined as a drop shipment by the sending site, or a direct shipping route has been entered)
will be defined as direct shipments; the program first loads the internal route from the receiving
site's master data (or it is determined by the switch INTAUF_DIREKTROUTE). If the post code of
the shipping address is known however, the area is determined by means of the new allocation,
and the route for this area is added. For calculating the date, the above-described optimization
will be started.
See also: EN-CONFIG-A+W Enterprise – section “Shipping region”



        6.9.3.          Free customer orders
If a document is marked as free, this identifier is transferred to the production site. However, a
"free order" does not automatically become a "free PO". However, a PO set manually to "free PO"
becomes a free order at the production site.


        6.9.4.          Document transfer - Version 2007
(ID 102235)
Already with Version 3.2 it is possible to assign documents to a PO. Starting with Version 2007, it
is now also possible to transfer these documents. In order to activate the function, in the EDI
configuration ((F5 on the field "Type of EDI" or menu: System - Data Transfer - Transfer Document
– Configuration) it can be defined whether
    •   whether a document assigned to a PO across documents should be transferred too
    •   whether an item-specific document assigned to a PO should be transferred too
As an additional requirement, the variable DATEI_REF_PFAD oder DFUE_DATEI_REF_PFAD must
be set. In these variables, it is defined on which server and in which directory the files assigned to
a PO are saved. The variable DFUE_DATEI_REF_PFAD overrides the variable DATEI_REF_PFAD for
the EDI. DFUE_DATEI_REF_PFAD must be set if the URL notation in DATEI_REF_PFAD for access
from the EDI is not possible.

In the variables DFUE_DATEI_REF_PFAD, the specification of server and directory is made in the
notation "<server>!<absoluter Pfad>." It has to be heeded that in the DFUE_DATEI_REF_PFAD
variables, / instead of \ are to be used for the path specification.

For this function, the environment variables can be defined client-specifically (#453094).
If neither of the environment variables is set, there is no document transfer.


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 87
Similarly, a transfer only takes place if the production site has the ALCIB version 2007 or higher.
Furthermore, it can be defined at the distributor whether it should be checked before the transfer
whether all documents defined in the database for the PO to be transferred are available.
(IB_NO_OUT_DOCUCHECK)
A corresponding configuration is also possible at the production site. (IB_NO_IN_DOCUCHECK)
(see section: configuration options)

A functioning FTP connection for the user alcibnet is required. Here, special attention has to be
paid to a correct entry in the .netrc of alcibnet. In the .netrc, the host name has to be precisely as
in the variables DFUE_DATEI_REF_PFAD or DATEI_REF_PFAD (including or excluding the domain).
It has to be heeded that in the DFUE_DATEI_REF_PFAD variables, / instead of \ are to be used for
the path specification.

The procurement of the files to be transferred is done primarily via ftp. For this, within the PO
export and the order import, the script copy_docu_files is called with the parameters
1. Call: 0 – first call; >0 subsequent calls
2. Mode: "get" – get files from document server or "put" create the files on the document server
3. Host: Name of the document server
4. Source directory
5. Target directory
6. File list of the files to be copied with relative path (<auftrnr>/<posnr>/<file>)
7. Last call: 0 – no 1- yes


gerufen. Within the PO export, this script creates the documents to be transferred (table kaufref)
from the document server in a temporary directory of the EDI
($DFUEDIR/dat/<sender>/<paket>/<send_auftrnr>/<send_posnr>). Within the order export, it
copies the files transferred from a temporary directory of the EDI
($DFUEDIR/dat/<sender>/<paket>/<ziel_auftrnr>/<ziel_posnr>) on the document server into the
corresponding subdirectories.
By default, this copying of the files is done via ftp. For this, another script "write_ftp_file" is called,
which writes a ftp command file. This is then executed using the script ftp_pcfile_ctrl.
(Script chain: copy_docu_files => write_ftp_file => ftp_pcfile_ctrl)
Then, depending on the configuration, it is checked whether the files to be copied into the
temporary directory (export) or to the document server (import) have arrived. Currently there is
no check whether the file size is correct.
During the import, the check is done using the script ftp_lsdirpc_sd. If the access to the document
directory is not required via ftp, the check can also be done in the script copy_docu_files itself and
the program-side check switched off.
If the script copy_docu_files or the subsequent check fails, the PO export is cancelled.
During the order or PO import, an error in this script or in the subsequent check does not cause
the cancellation of the scheduling. The order will be scheduled, but not released. With
appropriate configuration, the message 59 is sent to a defined employee. (see „Messages in EDI“)


A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                   88
          6.9.5.           SN File Transfer
The developments from cases #430912 (ISO as sub-element) and #437924 (SN files for fixed
articles) are a prerequisite for the new logic of taking over SN files of ordered sub-elements in
purchase order generation and transmission. The SN transfer for stock fill entries was expanded
with case #454842.
As developed with the above mentioned cases, this development also concerns the ordered lower
part insulating glasses. Since it is not possible to attach SN files to sub-parts, a logic was
developed which checks whether an SN file exists in the master data of the ordered sub-part
insulating glass. If this is the case, then this SN file is attached to the order when the order is
generated and is also transferred when the order is transferred.

PO creation:

Site a)
          - The system checks whether the item article in the purchase order (BOM sub-parts of the
          order) is a fixed article (article.prodbemass = 3).
          - If it is a fixed article, the system checks whether there is an SN file in the article master
          data for this article. This is done by checking whether an SN file (article number.sn e.g.
          "4711.sn") exists in the path $DFUE_ARTIKELBILD_PFAD\SN\.
          - If an SN file exists for the respective article, this file is copied from the current path to
          the TOE SN file path ($DFUE_SNFILES_DIR\TOE\<YYY>\<MM><DD>\) and renamed to
          match the purchase order (<aufnr>_<posnr>.sn e.g. "27001_1.sn").
          - The database field kposp.brokefile is then updated with the SN file and its subdirectories
          (e.g. "TOE/2019/4/10/4711"), and the database field kposp.snstatus is set to 100.

PO transfer

Haus a)
          - First, the file name is determined from the database (kposp.brokefile).
          - Then the packet is created with the SN file and transferred to site b.

Site b)
          - The transferred package with SN file is unpacked.
          - The order is created.
          - The sent SN files are renamed with the new number range of site b
          (<ordno>_<itmno>.sn e.g. "52001_1.sn").
          - The new SN file name is updated in the database (kposp.brokefile).
          - Finally, the renamed SN file is moved to the TOE-SN file directory of site b
          ($DFUE_SNFILES_DIR\TOE\<YYYY>\<MM>\<DD>\).


The prerequisite for using the new logic is an FTP server on the Windows computer and a working FTP
connection for user: alcibnet.

Environment variables:



A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                      89
          - IB_MIT_SN_DATEIEN must be set to "ON" so that the SN files are also transferred in the
          order transmission. The variable must be enabled both in sending and in receiving client.
          - DFUE_SNFILES_DIR the Windows path of the iTOE SN files must be entered. The variable
          must be enabled both in sending and in receiving client.
          o Notation <server>!<relative or absolute directory>
          - DFUE_ARTIKELBILD_PFAD the Windows path for the article pictures must be entered.
          o Notation <server>!<relative or absolute directory>

FTP scripts

The following scripts are required for this logic on the Unix machine:

          - ftp_lsdirpc_sd: Creates a list of files in an existing Windows directory.
          - ftp_mdirpc_sd: Creates a Windows directory.
          - ftp_topc_sd: Transfer file from Unix to Windows machine.
          - ftp_frompc_sd: Transfer file from Windows to Unix system.

Stock filling orders (#454842)

The SN transfer logic has also been extended for stock fill orders. The settings described in 6.8.5
SN-Datei Übertragung must also be set up for the stock fill orders. If a filling order is now
generated via the warehouse, the article master is used to check whether an SN file is available
and this is moved via FTP into the iTOE folder structure
($DFUE_SNFILES_DIR\TOE\<YYYY>\<MMM>\<DD>\) with a new name.

Troubleshooting

Problems with user rights (#455262)
alcibnet user rights must be set up for the server in question, otherwise there can be problems
with calling the FTP script.
FTP log in /tmp/ftp*: If on the FTP server a binary user is requested, frequently the entries in the
.netrc of the alcibnet user were not present. There is no binary user! The server on the .netrc, it
has to be precisely as in the environment variable DFUE_DATEI_REF_PFAD or DATEI_REF_PFAD
(including or excluding domain specification). It has to be heeded that in the
DFUE_DATEI_REF_PFAD variables, / instead of \ are to be used for the path specification.


          6.9.6.          References - Version 2007
Within the PO transfer, the producer must know which element of the original BOM (of the order)
has been ordered. This information was previously available in the table bpos, however, it is not
available for orders. This is why this reference information is transferred into an extra table
kposref.
Specifically, this involves the following information:
Reference to document created (order at the producer's, PO at the distributor)
auftrnr        External document number

A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                 90
vorgang       Document type (2 - P.O., 5 - Order)
subnr        Element counter
posnr        Internal item number (refers to kpos.posnr)
aufnr        Internal document number (refers to kpos.aufnr)

References to the document this transfer is based on
Order at PO creation
PO at PO transfer

refauftrnr      External document number
refaufnr       Internal document number (refers to kpos.aufnr)
refvorgang      Document type (2 - P.O., 5 - Order)
refposnr       Internal item number (refers to kpos.posnr)
reflfdpos       Serial item number

References to the original document this transfer is based on
Order at PO creation
Order or PO at PO transfer
orgauftrnr       External document number
orgaufnr        Internal document number (refers to kpos.aufnr)
orgvorgang       Document type (2 - PO, 5 - order)
orgposnr       Internal item number (refers to kpos.posnr)
orglfdpos       Continuous item number
orgtnr         BOM element number (refers to aufstrukt.tnr)



        6.9.7.         Customer PO number (kauf.exaufnr)
The assignment of the field is controlled via the environment variable IB_EXREF. For the order
transfer
  0: exaufnr=auftrnr sender's order no (PO number for PO EDI)
  1: exaufnr=bestnr the sender's PO number appears at the target site
  2: exaufnr=auftrnr/bestnr both numbers appear at the target site
  3: exaufnr=bestnr/auftrnr both numbers appear at the target site

  4: exaufnr is transferred unchanged
     When using the PO transfer, it must be heeded that during the PO generation, the external
     customer reference of the order is not retained; instead, it is overwritten with new values in
     the PO.




A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                91
        6.9.8.            Private fields

        6.9.9.                    Configurable document fields
Since Version 2007, private fields can be defined on the document header and item level. In the
definition of the fields, it is possible to set whether these entries should be retained by internally
transferred documents.
The evaluation of the "EDI" identifier (table: kflddef.dfuekz) is done in intauf. This is how the
settings at the recipient are determined. The receiving site decides whether it wants to have the
data from the upstream site or not. If the field is checked (=1) in the recipient, the sender's data is
retained.
This function is used by the KAUF (-1), NEUUPDATE (-6) and NEUBEST (-11).
In principle, for internal EDI (order linking, PO generation, PO transfer), the records from the
sending site are taken over into the receiving site. If then a function is called, the local settings in
the table 'kflddef' are checked. For fields for which the 'dfuekz' is set to local (=0), the value
transferred is deleted and if present, the pre-assignment is made.


        6.9.10.         Fixed private fields in the order header
            (kauf._private_*)
If at the production site orders are changed via internal EDI, then all changes made manually to
this order are lost. This behavior can now be switched off via configuration for the private
document fields (kauf._private_*).
The configuration can be done at the production site for customer distributor or all customers.
For this, in "System - Data transfer - Document transfer - Configuration" the entry "Type of the
EDI" = 100 "Order coupling" or 101 "Order transfer" with the control type 48 "Private document
fields retained (kauf._private_*) must be activated.
If this configuration is set for a customer, in case of order changes via internal EDI, the local fields
in kauf._private_* are retained. If this configuration is not set, the values will be taken over from
the distributor.
To be noted here is the changed function of the environment variables
DISABLE_COPY_PRIVATE_CHAR1 in this context.
If this variable is set, with the first transfer and if the configuration 48 is not activated, the field
kauf._private_char1 is emptied. If the variable and configuration 48 are active, the field is only
emptied on initial storage and it is retained with each additional transfer.
The private item fields (kposp.private*) or the configurable private fields (kaufprvfld, kposprvfld)
remain unaffected by this.


        6.9.11.           Report for delivery date shifts at the production
            site
If at the production site there is an automatic delivery date shift (e.g. initial scheduling and
delivery date calculation), the order status 206 - delivery date shift is booked by the system. If the



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                      92
status return is configured and this status 206 is transferred to the distributor, the message 67
can be sent there.
       •   67 – delivery date shift at the production site (starting with ALCIB-VERSION 2008) (also
           goes to the person entering the document (order/PO)
The status return is logged in $DFUEDIR/proto/rmin* (distributor) and rmout* (production site)
If in production there is a delivery date shift due to manual rescheduling, the status 206 delivery
date shift is also booked and forwarded to the distributor.
In case of a manual delivery date shift in the order entry, the status 206 is not written. For this
reason, there is also no status transfer and thus no notification of the distributor. In case of a
manual delivery date shift, we assume a previous personal agreement about the shift between
the relevant employees.
CAUTION: Only a transfer with the status 206 takes place. This status can trigger a message. There
is no automatic shifting of the PO or the upstream order since this must be discussed with the
customer and the production in question.


The status is forwarded by the production order at the production site via the PO to the
distributor until the order at the distributor.
e.g.
Order 1 at the distributor was entered and released for 07/18. The capacity planning in A+W
Production calculates 07/28 as the earliest possible date and shifts the order accordingly.
        Status 206 is booked with the new delivery date
Now a PO 11 is triggered for this order, which is transferred to the production site. At the
production site, a new order 2 is generated and scheduled.
The capacity planning in A+W Production calculates 08/02 as the earliest possible date and shifts
the order accordingly.
        Status 206 is booked with the new delivery date
This status is now transferred to the distributor and triggers the message 67 there. At the same
time, the status is displayed both in the associated PO as well as in the distributor order.


Distributor order




Purchase order




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                 93
        6.9.12.          Shipping information
For generation at the production site, the shipping type is always re-determined from the master
data.
The delivery type and packaging type are retained as usual. However, the behavior can be
changed via environment setting.
INTAUF_LIEFERART (client reference: no)
If variables are set, the delivery type is redrawn for internal EDI:
        ON = for order generation at the production site and PO generation at the distributor
        1 = Only for order generation at the production site
        2 = For PO generation at the distributor


INTAUF_VERPACKART (client reference: no)
  If the variable is set, with internal EDI, the packaging type is re-transmitted for rack planning):
        ON = for order generation at the production site and PO generation at the distributor
        1 = Only for order generation at the production site
        2 = For PO generation at the distributor


INTAUF_DFUE_VERPACKART (client reference: no)
If this variable is active, then the packaging type is filled via interface for the external order
scheduling.


NEW_PACKING_LOGIC (client reference: no)
Activates the logic of inheritance of the packaging type:
ON or 1: Customer-specific setting: The packaging type is always inherited from the header in the
positions.
Furthermore, the packaging type for order generation in the production site, PO generation in
trade and external order scheduling will NOT be re-populated, even if the abovementioned
variables are set.
2: If the packaging type is changed in the header, there is a query as to whether this change is also
inherited by the positions. In addition, with appropriate configuration (see above), the packaging
type is determined anew from the master data and transferred via external order interfaces.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                    94
        6.9.13.          Entered by
The employee (kauf.eusr) of a generated purchase order can be populated in various ways.
Without explicit configuration, the employee is -1 "System."
         Distributor / Sender / Purchase order generation
        d) Fixed purchasing employee
             For this, the environment variable EK_MANR must be set to the desired employee
             number. This variable is evaluated by the background process intauf. If with this
             configuration you wish to achieve that this fixed employee is also transferred to the
             production site for internal purchase orders, then the environment variable IB_EUSR =
             UNCHANGE must be set (starting with AWE5). If the variable IB_EUSR is not set for
             this configuration, then for internal purchase order transfer, the employee -1 is sent
             to the production site.
        e) Employee from the order
             For this, the environment variable IB_EUSR = ON or IB_EUSR = ORDER must be set.
             Here it must be noted that then the environment variable EK_MANR has no more
             effect for order-related purchase orders. Furthermore, it applies that for collective
             purchase orders, the employee from any one is used in the order that occurs in the
             purchase order.
        f)   Employee who released the order
             For this, the environment variable IB_EUSR = RELEASE must be set. Here it must be
             noted that then the environment variable EK_MANR has no more effect for order-
             related purchase orders. Furthermore, it applies that for collective purchase orders,
             the employee from any one is used in the order that occurs in the purchase order.
             CAUTION: All configurations described above are overridden by the environment
             variables INTAUF_MANEU.


Production site/Recipient/Order generation
Without configuration, the employee who sends from the distributor (see above) is deleted and
set to -1 "System."
If you would like to take over the employee from the distributor unchanged, then the
environment variable IB_XUSR must be set. However, this assumes that all employees company-
wide have unique employee numbers and are available in all databases.


CAUTION: All configurations described above are overridden by the environment variables
INTAUF_MANEU.
See also„PO creation – User“


        6.9.14.          Prices PU becomes SA
IB_EKVK_SHIFT
For internal order transfer, the setting of these variables


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 95
can also cause one of the price fields from the original order
to be written from poskost to kpos.dfuenstpreis and transferred. The name of the
field to be used must be entered in the variables; permissible
are only the two fields "stkprs" and "stkprsfw."
With entry of "nstpreis," kpost.nstpreis is written to kpos.dfuenstpreis
and transferred.


INTAUF_ALTEK must be set appropriately at the distributor.


        6.9.15.         Supply types
AWDesk #214611
The supply types are determined anew for internal EDI at the production site by the background
process "intauf" using the local master data.
However, it is possible to configure the system so that the supply type for laminated glass is
already met at the distributor.
is going to be produced and/or processed, you can now pass on these decisions regarding the
supply types to the producing site.
This includes the decisions as to whether laminated glass stock sizes shall be produced or taken
from stock, and where the processing steps for the laminated units to be applied to individual
elements shall be performed. The rule for this is defined in case # 213140.
Please note that this applies only to the processing of laminated glass, not to the processing steps
the system has been passed on to the elements at distribution. These will be removed at the
production site, and will be passed on again based on the production client's master data.
However, you can prevent the supply type of the processing step on the laminated glass level
from getting a new supply type after the transfer; instead it adopts it from the distributor, then
passes it on to the elements.
IMPORTANT!
There is no mixed version in which the supply types are sometimes adopted and sometimes
loaded from the production site's master data. Once the system has been configured to adopt the
supply types for laminated glass stock sizes and/or processing steps from distribution, this applies
to all orders. You can change this later of course, for the production client.
INTAUF_BEARBCOPY_BA_HALTEN = ON: If this switch is active, the processing steps marked as 'can
be passed on' in master data will adopt the processing type from distribution instead of loading it
from the production site's master data as for all other elements.
INTAUF_VSGLM_BA_HALTEN=ON: If this switch is active, the processing steps marked as 'can be
passed on' in master data will adopt the processing type from distribution instead of loading it
from the production site's master data as for all other elements.


        6.9.16.         Supplier for supply type "PO"
AWDesk #89959


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                96
For orders created via EDI, the suppliers are determined according to the following hierarchy in
intauf:
1. Item is a dimension variant and has a variant-specific supplier
(table: artvarzu) . if not ->
2. Item is a color variant and has a color-specific supplier
(table: artfarbzu). If not ->
3. Item has a desired supplier (table: artkuzu). If not ->
4. Default supplier from master data


        6.9.17.         Objects
If an object (kauf.objnr) is included in a document to be transferred, it is transferred unchanged.
For this, the object master data of the participating site must be synchronized.
There are 2 configuration options for this:
IB_OBJTEST               client reference: no
  When scheduling transactions, it is checked whether there is an object to be transferred in the
local master data. If not, the object number is set to 0 and thus the newly-created order is not
assigned an object.


INTAUF_STDOBJNR          client reference: no
  For the internal transfer, the default object is entered into the newly generated order
regardless of the object transferred.


        6.9.18.         Text
Within the PO transfer, all texts (manually entered, generated texts, and configured texts) are
transferred. The identifier "generated" is not changed here. At the production site, generated
texts are deleted and re-generated using the configurations at the receiving site. Manually
entered texts are retained.


        6.9.19.         written back
If the environment variable RABATTLOGIK_2005 is active, the order discounts are NOT transferred
within the PO transfer. In the receiving site, the discounts for the customer "sending site" are
determined anew from the master data for the order. The end customer for the order is not
evaluated here.


        6.9.20.         Site-spanning PDC
The site-spanning PDC enables the transfer of a label number to individual locations, each of
which has its own production system and therefore cannot process the labels from the other
system.
During the order generation in one's own location, the label number generated and the PDC
quantity identifier are drawn from the table bestparameter and written to the table
kposzusatz.barcode_char. In the A+W Enterprise-internal order transfer, now the table

A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                   97
KPOSZUSATZ is transferred with the label number and the PDC quantity identifier in the order to
the production site.
Functionality is not provided for the SP coupling. (#411794)
The "Site-spanning PDC" is documented in "EN-CONFIG-A+W Enterprise".



        6.9.21.         Exchange/addition rules
See also "EN-CONFIG-A+W Enterprise" section "Replacement/addition rules" "Internal
EDI".

        6.9.22.         Complaint details
If a PO includes complaint details, these are transferred 1:1 in the order to the production order.
Therefore, it is necessary that the complaint master data (codes) are synchronized between the
sites.
If you don't want this transfer, the environment variable VK_REKLAMATION has to be activated.


        6.9.23.         Setting of the kauf.org* fields
The setting of the fields kauf.orgkunr, kauf.orname, etc. is controlled via the market partner
master data. Important is that it is documented (preferably in the market partner notes) why the
setting is the way it is since the setting in other evaluations (forms, SP, production transfer) can be
relevant.
If the transferred PO is an order-related PO for only one order, then the data of the ORIGINAL
customer from the order is in the ord fields. This data will then be transferred this way to the
production site. At the production site, you can recognize using kauf.hausnr != kauf.parhausnr
that it is a transferred PO. The corrrect customer number of the production site from xhaus is in
kauf.kunr (see also IB_KUEMPF).
At the production site, you can control using the field DFUE-Typ in the customer data record for
the distributor whether the original customer data is retained or should be overwritten with the
customer data "prodution site".
Customer EK 1:1
The corresponding customer "distributor" at the production site is on "EK 1:1". This means that
generally the end customer is not specified and that the supplier designation from the distributor
in the production site is not overwritten (in my opinion, sooner an unusual setting).
Customer EK 1:1
The corresponding customer at the production site is on "EK 1:n". This means that generally the
end customer is not specified and that the supplier designation from the distributor in the
production site is overwritten with the appropriate customer name.
The setting EK 1:1 or EK 1:n does not necessarily control whether or not a PO may contain only
one order. With a setting EK 1:1 in the PO pool, several orders can be combined into a PO and
vice-versa.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  98
        6.9.24.          Spacer reduction (SR)
Local SR
For the internal EDI it is assume that the item master data is identical in its essential properties.
Therefore, the AHAM is transferred unchanged by default. To achieve that the local SR is used in
the receiving site and the dependent data (spacer and muntin size) is recalculated, the variable
must be activated.
This function may not be configured together with MD_MIN_AHAM
Minimum SR
February 2025 // alcib - 13.04.19494
After transfer of a document (internal document transfer), the spacer reduction dimension (SR) in
the receiving company is checked in the generated order.
The minimum value for the SR can, depending on the client, be stored in an environment variable.
When processing the transferred orders (intauf still-1), the SR per edge is checked and adjusted
according to the stored restrictions. If the SR per edge has a smaller value than the configured
minimum value, this value is adjusted; otherwise, the values are taken over. The dimensions of
the spacer are recalculated (shape set, frame step set).
If the item has asymmetrical muntins, an order information is attached to the order, which
indicates that the grill pattern should be checked.
The value of the switch is treated exactly like SR ($11) in the IG master data: <ENV-value>/2 per
edge.
This function may not be configured together with the "local" SR (environment variable
DFUE_IB_OWN_AHAM).




    6.10. Environment variables
This section will only discuss environment variables that are significant especially for the PO
transfer. Environment variables that apply for generally for the EDI will be listed in the "Basic
configuration" section.
BESTELLDFUE (client reference: no)
In principle, the PO transfer is permissible. Whether a supplier is connected via order coupling or
PO transfer is defined in the supplier master data (type of the EDI).
DFUE_IB_BESTELLSPERRE (client reference: no)
The variable controls when internal POs go into local correction.
0 - print; 1 - send; 2 - receipt; 3 - scheduling; 4 - job created; 5 - job confirmed
  precise description in AWD ID 110318
  If internal POs are handled via the PO pool, this variable may not be > 0!!! The same applies if
the PO transfer is done via the printout.
IB_EXREF (client reference: no)



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                    99
  The variable influences the structure of kaufexaufnr (external reference) for the document
transfer (NOT for PO generation!)
  0: exaufnr=auftrnr sender's order no (PO number for PO EDI)
  1: exaufnr=bestnr the sender's PO number appears at the target site
  2: exaufnr=auftrnr/bestnr both numbers appear at the target site
  3: exaufnr=bestnr/auftrnr both numbers appear at the target site

  4: exaufnr is transferred unchanged
  Caution: not set or 0 corresponds to the previous logic.


IB_NO_IN_DOCUCHECK (client reference: no)
  Within the order scheduling or PO generation during PO transfer and PO generation,
documents to be transferred are copied from a temporary directory of the EDI to the document
server. After that, the program checks whether all defined documents have arrived there. If a
document is missing, the order is not released. If this variable is set, the check does not take
place.


IB_NO_OUT_DOCUCHECK (client reference: no)
Within order outsourcing, documents to be transferred are copied from the document server
into a temporary EDI directory. Then, the program checks whether all documents defined in the
database for the order are all documents defined in the database for the order. If a file is missing,
the transfer is cancelled. If this variable is set, the check is not done.


VK_REKLAMATION (client reference: no)
If the variable is active, the complaint details are not transferred.


    6.11. Error handling
Problem                           Cause                                 Remedy
Incorrect/not implemented         Incorrect/missing intauf              Environment variable
supply type                       process (has to be -1)
                                                                        IB_ZVERS check
Incorrect delivery address in     During PO generation, a               Environment variable
the receiving site/in the PO      recipient is written to intbest       BESTELLDFUE is not active.
                                  even though PU EDI is
                                  entered for the supplier




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 100
7. Generating suborders
    7.1.        Function Description
The generation of suborders is intended for multi-stage production. For example, LAMI with TG is
sold to a customer. The operation manufactures the TG and the LAMI itself. In this scenario, an
internal production order is required for the production of the TG as suborder to the original
customer order. With the introduction of PMS and A+W Production, the generation of production
suborders is no longer required since this multi-stage production is supported in the production
system.
Meanwhile, there is an exception. This is the IG function in the IG. Currently (as of January 2020),
this construction is not supported by A+W Production. For this reason, A+W Enterprise has to
generate a special production order for the IG in the BOM.


    7.2.        Configuration
There must be an extra xhaus entry with its own site number and its own (pseudo) supplier.
The internal pseudo supplier must have the type of EDI PU 1:1 and direct purchase order = yes.
The environment variable IB_ALLOWIB must be active.
The client number of the xhaus entry of the pseudo supplier must be in the environment variable
IBHAUS.


    7.3.        Process
The (pseudo) supplier is entered in the main order. A PO is generated for this supplier. When this
PO is then transferred, a suborder is generated. Generated suborders will be transferred to the
background process intauf with still=-1 (NEUKAUF).


    7.4.        Error handling
If type of EDI is on "None." This process does not work. A PO but no suborder is generated.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                               101
8. Order shifting
Within the document transfer, there are possibilities for shifting orders instead of transferring
them. The use cases for this are on the one hand the shifting of orders to a test system to avoid
doubled entries and on the other hand, the shifting of internal orders due to capacity bottlenecks


    8.1.         Test system
Generally it should be noted that this is a test function. Expansions are possible to only a
limited extent, but with lower priority and insofar as they do not compromise the default
function.
The receiving system treats the incoming orders principally not as EDI orders, but sooner as
manually entered orders (see section "Generally deviating functionalities").
If this logic is configured (IB_ZVERS less than 100 or greater than 32000) or if incorrect records
are written to the table "intbest" (e.g. intver less than 100), it can cause the normal order
generation or PO transfer to stop working. You can see this in the log ibout*.
CAUTION This function may not run in parallel to normal operation; it must be activated only
for a particular time period! (up to 04/2025)
Generally, the provision of a test system is recommended. Here, master data adjustments,
program updates, system configuration, and similar can be tested without danger. In order to
enable a realistic text, however, it is often necessary to have real orders available in the system. In
order to reduce the work required for entry, A+W Enterprise offers the opportunity to shift
orders.
For this, it is necessary that the item and market partner master data in the target system be
largely consistent with the target system.


        8.1.1.           General configuration
It is assumed that the general document transfer is configured. Here, only deviations for this
special function will be discussed.


Up to 04/2025 (trm_ctrl build < 13.04.12564)
Environment variable IB_ZVERS must be set in the sending clients. The environment variable is
not evaluated site-individually. If the variable is active, the order shifting to a test client will be
activated. If this variable is set, the "intver" column in the table "intbest" will be evaluated by
trm_ctrl. Using the shell script "intver," orders for shifting can be placed in intbest.
Caution: no other activity may be booked (order generation, document transfer) to intbest
table! (up to trm_ctrl 04/2025)


Starting in 04/2025 (trm_ctrl - 13.04.12564)
Environment variable IB_ZVERS must be set in the sending clients. The environment variable is
not evaluated client-specifically. In the variables, a value between 100 and 32000 must be


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                     102
defined. The value "ON" is no longer supported and corresponds to a deactivated function. If the
variable is active and has a value between 100 and 32000, the order shifting to a test client will be
activated. trm_ctrl evaluates the column "intver" in the table "intebest". Orders - and only orders
that are in the table intbest with intbest.intver=$IB_ZVERS with sendeseq=0 will be transferred to
the test system. If an error occurs here, a corresponding error status is set. Records with an error
status (sendeseq!=0) are not transferred. This also affects records with temporary errors
(sendeseq=-2)
Using the shell script "intver" (version newer than 04/2025 and QR2503), orders for shifting can
be placed in intbest. The script is only an internal aid. It is created permanently for the current
data structure of the table intbest.
No cancellations are transferred!


Starting in 07/2025 (alcib – 13.04.20590)
Normally the table "ktechw" is not transferred within the PO and order transfer. For the normal
transfer (intauf -1 and intauf -7), the values are regenerated by the background process "intauf".
For order shifting to the test system, this does not happen. If you need the entries in the table
"ktechw" (e.g. if you are using the "Logistic Optimizer"), then the environment variable
"INTAUF_KTECHW_TEST" must be activated.



        8.1.2.          General deviating functionalities

            8.1.2.1. Customer Data
The customer data and delivery date are not changed.


            8.1.2.2. Site number
The orders are booked in the target system with parhausnr = parhausnr + 100 so that no reports
to the sending system are made! However, if the source site number is greater than 899, then
booking is done with parhausnr = parhausnr - 100.


            8.1.2.3.Customizing / price calculation / procurement
                 types
In the target system, the orders are not handled like orders via internal EDI, but rather like
manually entered ones. This means that they are not processed by intauf with -1 (NEUKAUF), but
rather with -3 (TXT_KOMPL). This means that there is
    -   no new price calculation
    -   no material cost calculation. The costs are sent along.
    -   no implementation of the supply types
    -   Customizings (vorgangs_sql) for internal EDI (still = -1) do not work


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                 103
    -   Orders are not released
    -   Customer data is not changed
    If you would like a new price calculation, you must use the script vorgangs_sql to transfer the
    order scheduled to intauf again with still -4 (PRS_KOMPL). In order to distinguish the order
    from manually entered orders, you can evaluate kauf.parhausnr (parhausnr = parhausnr +
    100)


            8.1.2.4. New orders vs. Change of order
Analogous to the "normal" internal document transfer, in the recipient, the order number can be
assigned normally from the order number range, from its own number range (mpdfuectrl) or via
offset.
Just as for normal document transfer, it applies that if an order is transferred multiple times, a
new order is not created each time; instead, the existing order is adjusted. If you would like to
transfer the same set orders again and receive new orders for these, you must either cancel the
old orders or remove the reference (kauf.parauftrnr) in the target system.


            8.1.2.5. Entered by
Regardless of the definition of the variables IB_EUSR, the person entering the orders is
transferred unchanged. The test system can be configured such that the person entering the
order is also retained there (environment variable IB_XUSR / see „PO transfer – User“)


            8.1.2.6. Release
The scheduled orders are not released. The environment variable "INTAUF_FREITEK" is
not evaluated since these by definition are not EDI orders. They are in the release pool
without a release marking.


            8.1.2.7. Status
Within the order shifting, the codes "delivered" and "calculated" are transferred since this
information is saved in the table "kauf" and currently is not changed.
Other status (e.g. ordered, job created) are not transferred since the tables "kaufstat" and
"kposstat" in which these stati are noted are not transferred.


            8.1.2.8. Discounts
Discounts (table kaufrab) are neither transferred not determined anew.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  104
            8.1.2.9. Document attachments                          / Motiv files
Document attachments on the order header or item level (table kaufref) are transferred
exclusively with PO transfer and product set replication. This also affects motive files for
processings (poszu.dateiname).


            8.1.2.10.            Technical values
The technical values are not transferred.
Normally the table "ktechw" is not transferred within the PO and order transfer. For the normal
transfer (intauf -1 and intauf -7), the values are regenerated by the background process "intauf".
For order shifting to the test system, this does not happen. If you need the entries in the table
"ktechw" (e.g. if you are using the "Logistic Optimizer"), then the environment variable
"INTAUF_KTECHW_TEST" must be activated.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                              105
9. Invoice transfer
The definition of the individual settings is made under
      System > Data Transfer > Transfer Document > Configuration
Or in the market partner master data via the "EDI configuration" menu or F5 on the field "Type of
EDI."
With "Type of EDI" = 104 "Invoice transfer," currently the following settings are possible:


Control type            Name                          Description
6                       Internet address              So that an invoice can be transferred via ERP webservice to
                        (webservice)                  another (customer) webservice, the URL of the receiving
                                                      webservice is stored here client-specifically.
                                                      ID 127053


With Version 2011 (4.5), the EDI type 105 "Document transfer" replaces the EDI type 104.
The following configurations are required so that a document (invoice/delivery note) is
transferred to a target webservice in openTRANS format via ERPWebservice and can be
stored in the target database:
Control type            Name                          Description
6                       Internet address              Customer-specific URL of the receiving webservice
                        (webservice)
                                                      ID 127053
7                       Database name                 Name of the receiving database
8                       DB_LOCALE                     DB_LOCALE Setting of the receiving database


For more information, see "EN-CONFIG-A+W Enterprise B2B Service ERP WS" and the
documentation in Sharepoint:
https://awsoftwaregmbh.sharepoint.com/:w:/r/sites/AWClarityRD/Shared%20Documents/Interfa
ces/Enterprise/B2B%20Interfaces/DE-
A+W%20Enterprise%20Cust%20Auto%20Goods%20Receipt.docx?d=w10900c1fb5f645278125dda
31105c10f&csf=1&web=1&e=eQMeMy




A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                             106
10. Product set transfer
With A+W Enterprise 6 Build 01.02.2020, product sets can be transferred via internal EDI. For this,
the product sets must be created in the master data and then entered into the table via individual
scripts/procedures. Here it must be noted that the field intver must be = 3.
insert into intbest values
(sender,kauf.aufnr,kauf.auftrnr,kpos.poskonr,kpos.posnr,0,0,today,0,empfaenger,1,0,0,0,kauf.still
,3,0,0,0,0,kauf.auftrnr,kauf.kunr, kpos.laenge,
kpos.breite,kpos.szr,0,kpos.menge,kpos.modnr,0,0,0,0)
Products sets that are transferred via internal EDI
    -   are not transferred to the CAD service
    -   are not transferred to A+W Production
    -   Retain the customer number
    -   The field input is set to "Representative" (not EDI) in order to achieve a separation from
        product sets created via external EDI.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  107
11. Change log (kaufedit)
The PO generation writes an "entered" record for the generation of the PO for the employee -2.
Then the PO is transferred to intauf and it writes an "entered" record for the employee -1. Then
the PO for the transfer is transferred to the EDI. Here, an "entered" record is now written with the
export. For suborders, this is the client of the (pseudo) supplier, for the normal transfer it is the
sending client.
In the receiving site, it is then "entered" by intauf and written by "Kostenkalk". For suborders, the
receiving site is the same as the sending site. For suborders, this creates a somewhat confusing
display. If other changes are made, it becomes very strange since POs and suborders are not
change, but rather always generated anew (retaining the order no), which means that the
"entered" records load again.

With regular transfer, the "old" records are deleted and only the current ones taken over into the
production order. Thus, there is no loading there. For suborders in the same site, however, this is
not possible since it is not possible to distinguish which are the regular change records of the
"receiving site" and which are those of the sending site since both are identical.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                               108
12. Status reporting from the production
 client
    12.1. Triggering status transfer for internal client
      separation
See "EN-CONFIG-A+W Enterprise Internal Client Separation" section "Status report"


    12.2. Reports
EDI status reports
Path:
$DFUEDIR/proto
Name:
rmout_proto<haus>_<MMdd>
rmin_proto<haus>_<MMdd>
rmupd_proto<haus>_<MMdd>


Caution: With internal client separation, starting with … only logs for the calling clients and no
longer for sender and recipient are written.


    12.3. Configuration
PRODUKTIONSSTATUS_ADHOCSQL (client reference: no)
AWDesk #132455: Group and ID of the ad hoc SQL, which can be called up with Shift-F5 from the
production status to display the production status of suborders.
 The first statement of the SQL specified here must have two parameters, since these are passed
from the program!
  1. Param: kauf.auftrnr
  2. Param: kpos.posnr


RMELD_LOGIC (client reference: no)
The variable controls the transfer of statuses from production to trade. If the variable can assume
the following values:
 1 - The status "packed" (307) from production becomes the info status "ready for dispatch" in
trade (557).




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  109
    12.4. Status overview
Name                  Status              Transfer-            Next status        Remark
                                          relevant
Delivery date         206 – kaufstat      Yes                  X                  This status is
                                                                                  booked if the
                                                                                  production must
                                                                                  postpone a
                                                                                  delivery date
                                                                                  automatically
                                                                                  during
                                                                                  scheduling or if
                                                                                  the delivery date
                                                                                  is postponed due
                                                                                  to a manual
                                                                                  rescheduling in
                                                                                  production.
STATUS_VERPACKT 307                       Yes                  557 (Config)
                                                               307




    12.5. Status 206 – postponement of delivery date
See also section "Report for delivery date shifts at the production site"




    12.6. Status(503): Transfer to the production site
If an order-related PO is transferred internally and the acknowledgement for this transfer is
received, then the information status "503 – Transfer purchase order" is written to the associated
sales order. This status is displayed item by item in the order information – Tab: Associated prod.



    12.7. Status(551): Order scheduled in production
If the production order resulting from the purchase order is then successfully scheduled in
production, the information status "551 - Scheduling successful" is written to the associated sales
order. This status is displayed item by item in the order information – Tab: Associated prod.


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                              110
    12.8. Status(552-556): Order in production
If the production order resulting from the purchase order is then planned in production, the
information status "552 - Planned," "553 - Finely planned," "554 - Released for production," "556 -
Produced" is written to the associated sales order. This status is displayed item by item in the
order information – Tab: Associated prod.


    12.9. Status(307): Order packed
If the production order resulting from the purchase order is then packed in production, with the
appropriate configuration in the associated sales order, the information status "557 - Item
packed" is written to the associated sales order. This status is displayed item by item in the order
information – Tab: Associated prod.

For the implementation of the packed status, the environment variable RMELD_LOGIC=1 must be
set.



    12.10. Status: Order dispatched
After the production order is reported in the production company as out of the site, with the
appropriate configuration, the information status "558 - Dispatched" is written to the associated
sales order.
In the order information - "Dispatch" tab, the traffic light display is installed analogous to the
display in dispatch, with the following meanings:
Yellow - packed,
Half blue - on transport,
blue - delivered,
Red - locked.
On the traffic light field, there is a tool tip with the information about the display colors.



    12.11. ADHOCSQL for determination of production
      information for internal reference orders
A new ADHOCSQL (GRP 1, ID 87) was made available, which determines the internal order
references and displays their production information.
It can be executed by clicking the "Int.Order" button of the "Process information" dialog,
"Production" tab (accessible e.g. via Sales > Overview > Order information).
This is a two-stage SQL, that is, by clicking the "Int.Order" button, you get the production
information about the direct suborders of the current order. Through positioning on one of the
suborders and pressing F5, you go one level deeper and get the information about the suborders
of the current suborder. Another level is not implemented.



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                               111
The environment variable PRODUKTIONSSTATUS_ADHOCSQL must be activated with "1 87".
The ADHOCSQL "1 87" can only be used with configured PO EDI. (For configured order transfer,
the stored SQL must be modified.)
For detailed information see \\jupiter\Doku_DocuWare\ALCIB-PMS\SQL-
SYSTEM\User_Manuals\SQL\ErweiterungendesADHOCSQL.doc


    12.12. Message on PO date postponement
[AW-137151] // October 2023
If in an existing PO the date is postponed manually (PO management) or via notice, then the
status 204 (WARENEINGANGSTERMIN) is reported to the PO and in the order. This status is also
transferred if the PO from an order arose from the internal transfer. This status can be seen in the
PO and in the order under document information.
If the status 204 - goods received date is transferred to the upstream distributor, the sending of
the e-mail ID 95 can be configured there using the System menu.
For more precise information, see configuration instruction "EN-CONFIG-A+W Enterprise System"
section "Messages" and section "Messages" and "EN-CONFIG-A+W Enterprise" section "Dispatch
notification".




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  112
13. Balance scheduling
See also "EN-CONFIG-A+W Enterprise Interne Mandantentrennung"
If you are using the FinAc service, depending on the FinAc, a different balance takeover may be
used. See the individual FinAc interface description and/or the description of the FinAc service.


    13.1. Structure of the salden.dat file
The salen.dat file is in the directory /fibudat/transfer/
(for corporate groups as subdirectory the site number)
All values must always be transferred in the system currency!


Field      Digits              Field          Direction
 No.     fro    to    Dec.    length Typ direction                               Description
          m                           e
  1       1      3      0        3       n        rb       Company number
  2       4      4               1                         Field separator
  3       5     12      0        8       n        rb       Customer number
  4      13     13               1                         Field separator
  5      14     29      2       16       n        rb       Balance - open items, credit with -
  6      30     30               1                         Field separator
  7      31     37      0        7       n        rb       GCI limit or "0"
  8      38     38               1                         Field separator
  9      39     45      0        7       n        rb       Credit limit or "0"
  10     46     46               1                         Field separator
  11     47     53      0        7       n        rb       Liability on bills or "0"
  12     54     54               1                         Field separator


"^" should be used as field separator.
Example for credit: -123.45
Last, an empty line should be included since otherwise the counting of the lines does not
work on some systems.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                 113
    13.2. Default flow
Via the script $DFUEDIR/bin/sendesald, the trm_ctrl of type 4 is started. There is an environment
variable FIBU_ZENT that specifies which is the FINAC central office. The variable is currently not
read out site-specifically. If the site read in matches the environment variable, the script
"fibu_salden" is called. This script reads in the "salden.dat" file. It retrieves the salden.dat file
from a customer-specific defined directory, manipulates this file customer-specifically somewhat,
and stores it as EDI package. Then, trm_ctrl loads the manipulated file into the "salden" table
With the help of ALCIB environment variables, it is set whether AKV limit and/or credit limit are
taken over.
AKV_LIM_TO_ALCIB
KRED_LIM_TO_ALCIB
DFUE_LIMITS_IGNORE (#154307)
The liability on bills is taken over according to kuplus and flows, if it is filled, into the limit check
(environment variable WECHSELOBLIGO).




    13.3. Internal client separation (AWD #388239)
The balance files must be imported client-specifically if the client-specific limit check is configured
(environment variable LIMITS_MANDANTENTRENNUNG). The correct site number must be in the
salden.dat file. As previously, there is also an appropriate implementation via the control file
$ALDATPFAD/cssmandant.par.

If the environment variable LIMITS_MANDANTENTRENNUNG is set, the environment variables
LIMIT_ZENTRALE_DB and BUCHE_SALDEN_ZENTRAL may not be active .

For the site-individual balance scheduling, the open items from the FinAc are written and if
configured the limits in the limits table. If a customer is only in the mp table, but not created in
the limits table, then there is no takeover of the open items for this site.


    13.4. Update of the totals by the AWE FinAc
      Service
If the FinAc transfer from documents is configured via the FinAc service, there is an updating of
the totals via the FinAc Service.

After the transfer of transaction data (invoices/credits), there is a check whether the open items
must be updated. In the table kuplus or limits, depending on the env variables
KUPLUS_ACTIVE_FIELDS, the values in "fibu_op" and "op" and "op_brutto" are updated.

For a detailed description of the logic, see the configuration document of the FinAc Service.




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                       114
    13.5. Logs
The logs for balance takeover are in $DFUEDIR/proto and are called fb*proto<Site>. In addition,
there are the new logs $DFUEDIR/proto/<site>/<type>/fibuout_proto*
$DFUEDIR/proto/<mandant>/<type>/fibuin_proto*
$DFUEDIR/proto/<mandant>/<type>/fibuupd_proto*
Depending on the program version, type="global" or "fibu"




    13.6. Problem handling
        13.6.1.          Totals are not stored
Log fibuin*
Log entry
fb_sldi: insert into totals (sr %d =?= fr %d)
If the numbers sr and fr are different, there is no storage. If the numbers deviate just by 1, it helps
if an empty line is inserted at the end of the interface file.
*1) – alleged number of lines in the interface file => fr
*2) – sr = number of lines that were loaded in the table "salden"




        13.6.2.          The value in fibu_op does not match salden.dat
Fictitious example:
The balance scheduling runs at 11:00 PM. It contains fibu_op of 1000€ for customer A. The
balance scheduling now sets fibu_op=1000€. At the same time, in op or op_brutto, there is a total
of 500€ of invoices that were created today but not yet transferred to the FinAc.
At 12:30 PM, the transfer of the invoices/credits runs and the FinAc (FinAc service or trm_ctrl)
that transfers the invoices/credits from the day before to the FinAc. Here, fibu_op is increased by
op or op_brutto. Thus, 1500€ is in fibu_op. The next morning at 9:00 AM, this no longer matches
the salden.dat from 11:00 PM, but it is completely correct from a data-technical point of view.




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                               115
        13.6.3.         Error: data for client X instead of for Y
With QR2302, the message in "ERROR: Data for site X instead of site Y“ was changed and shifted
from the log "fbsl_proto<site>" into "fibuin_proto<site>_<mmdd>."
The cause for this message can be that in the table "salden" there is still data from another client.
This can especially happen when starting a new client or when converting to multisite without
"LIMITS_MANDANTENTRENNUNG."
If there is no balance storage running, the table "salden" can be emptied.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                116
14. Messages
    14.1. Overview
Sending and acknowledging document transfers can be monitored. This way, a system
administrator can be notified if documents are sent to connected sites, but were not
acknowledged in a defined time.
The message about not acknowledged transfer packages arrives three times at an interval of 30
minutes. It goes to the employee with the employee number specified in
$ALDATPFAD/watchdog.par for the EDI starter.
For this, an entry for the dfue_starter must be made in the control file
$ALDATPFAD/watchdog.par. This entry contains among other things the text for the subject line
of the e-mail and the employee number to whom the e-mail should be sent.
${IPCDIR}/repspool.akt^${IPCDIR}/ starter.log^PO transfer not confirmed!!! ^^<manr>^15^0^0^
You can also configure the message via the system messages (CTRL F4 menu - mail system -
system messages - message assignment - message number 31).


Message number (table: "alsysab")
    •   10 - order from associated site or from external customer was received (alternative
        separate configuration via 51 (external) and 53 (internal))
        If both message 10 and message 51/53 are configured, the information arrives in
        duplicate.
    •   15- Order sent
    •   18 - Order to be transferred was already invoiced. The initiator of the message is the
        author of this order. (omitted starting with ALCIB 2008)
    •   19 - Document to be transferred is locked. The initiator of this message is the locking user.
    •   20 - PO was created. If the variable IB_MBESTRD is active, the one who initiated the
        message is the one who entered the order that belongs to this PO.
    •   21 - quotation received
    •   22 - Flawed article transfer
    •   31 – transfer not yet acknowledged
    •   46 - PO cannot be transferred. (for PO transfer, not for linking of orders)
    •   47 - An error occurred while creating a PO for this order / also for dispatch notification
    •   48 - Document could not be transferred to a connected site (error at the sending plant).
    •   49 - Message on failed additional order processing during order import (if the variables
        EDI_SQL or IB_DFUE_NACHBEARB are configured)
    •   50 - Message on a missing, customized entry in table dfue_nachbearb for additional order
        processing during order scheduling



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  117
    •   51 - order received via external interface (cannot be configured together with message
        10, otherwise message appears doubled)
    •   53 - order received from connected site (cannot be configured together with message 10,
        otherwise message appears doubled)
    •   54 - Created PO is a rush order If this message applies, message 20 will not be sent.
    •   55 - order change /cancellation of order was received/local change overwritten (receiving
        company)
    •   56 -the received document is a rush order
    •   57 - PO was cancelled/local change overwritten.
    •   58 - Error while saving an order (error on the receiver's side).
    •   59 - Incorrect EDI: general error
    •   62 - check external order scheduling: spacer exchange and gas were sent simultaneously.
        (starting with ALCIB version 2006)
    •   63 - incorrect master data definition for external order storage (starting with ALCIB
        VERSION 2006)
    •   65 - interface reporting file could not be processed correctly (starting with ALCIB VERSION
        2007)
    •   67 – delivery date shift at the production site (starting with ALCIB-VERSION 2008) (also
        goes to the person entering the document (order/PO)
    •   68 – incorrect EDI: incorrect scheduling at the production site (starting with ALCIB Version
        2008)
    •   71 – Note: check external order scheduling – this message is sent if the external order
        scheduling could not process a file.
    •   85 – article transfer was successful (article replication)
    •   86 – market partner transfer was successful (market partner replication)
    •   87 – code transfer was successful (code replication)
    •   95 – goods receipt date shift in the production company for an order for job


To send messages from various clients to the same user, the user -1 system should get a generally
applicable name with the individual clients. For example, you can add the client number or client's
short name at the start or end of the name (e.g.32_system service for the system service of client
32). This shows the client who sent this message. In addition (especially for internal client
separation) or alternatively the environment variable ALMAIL_MANDANT_BETREFF="ON" can be
set. If this variable is set, the site number and name of the site (from the table xhaus) is placed in
front of the actual subject text in the subject line.


        14.1.1.         Report 22 (article replication)
ID 117358:




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                               118
Article replication generally takes place automatically. In the subsidiaries it is not always known
whether and how many products must be transferred. If the transfer did not work, frequently this
was noticed too late.
Starting with Version 2007, for the message 22 "Article transfer failed", a message recipient can
be defined.
This message recipient receives a message if the article replication did not work completely. The
message has the following structure:
Subject: Article transfer failed
Message text: The following products were not replicated:
           10500055,
           43214321,
           99111104,
           99112233,
Depending on the configuration, the following message texts may appear:
"Caution, the transfer of the article master data to client <Site> failed! (SC=<SQL-error code>)"
"Article types from the 'mandatory dimensions' were not replicated."
"Article types from the 'article dimensioning' were not replicated."
"Processing types from the 'article dimensioning' were not replicated."

Starting with 2012.1: "For the following articles, master data errors (SN macro definition) were
found: 00000000, 00991231, 00001231, 00001239, 09991232, 09981231,
Here, as many product numbers and messages are listed until the message has reached a length
of 1000 characters.If more than the 1000 characters are required, this is indicated with " ..." .
For a precise analysis of what and why the transfer failed, the transfer log
$PROTOPFAD/ArtReplik<mmdd> is available.
see also Log database table


        14.1.2.          Message 31
Sending and acknowledging document transfers can be monitored. This way, a system
administrator can be notified if documents are sent to connected sites, but were not
acknowledged within 30 minutes.
The message about not acknowledged transfer packages arrives three times at an interval of 30
minutes. It goes to the employee with the employee number specified in
$ALDATPFAD/watchdog.par for the EDI starter and to the employee of the message 31.
For this, an entry for the dfue_starter must be made in the control file
$ALDATPFAD/watchdog.par. This entry contains among other things the text for the subject line
of the e-mail and the employee number to whom the e-mail should be sent. If the recipient of the
message should only be configured via the message system, an employee number=0 can be
entered in the watchdog.par.
${IPCDIR}/repspool.akt^${IPCDIR}/ starter.log^PO transfer not confirmed!!! ^^<manr>^15^0^0^
You can also configure the message via the system messages (CTRL F4 menu - mail system -
system messages - message assignment - message number 31).



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                119
The message text is fixed in the script dfuemeldung. You must copy the script to spec/cmd and
enter the message there in English. Currently, no message goes to the author.


           14.1.3.        Message 50
This message is sent within ibin() if:

     a)    This is an internal order transfer and
     b)    The variable IB_DFUE_NACHBEARB is active and
     c)    The table "dfue_nachbearb" exists and
     d)    The select on the table "dfue_nachbearb" produces no result (SC=100 - no record
           found)

Or

     a)    This is an external order transfer and
     b)    The variable EDI_SQL is not active and
     c)    The table "dfue_nachbearb" exists and
     d)    The select on the table "dfue_nachbearb" produces no result (SC=100 - no record
           found)


           14.1.4.        Message 51
#449692
In the external standard interface it is now possible to send the incoming order e-mail to the
employee (MP.SACHMANR) as well. To use this logic, the environment variable
DFUE_SACHBEARB_MAIL must be activated.


           14.1.5.        Message 55
This message is sent to the receiving company. If the environment variable IB_EUSR_SYSMELD is
active, kauf.eusr is the initiator of the e-mail. Otherwise, the initiator = 0


Message 55 is sent if
     1. there is an error during the check whether this is a new or changed order.
        (check_old_new())
           "Order %d from site %d - please check!"
     2. a cancellation for an order already in (partial) local correction comes.
           "Caution: order %d = %d from site %d should be cancelled. However, it is in production"
     3. an order is cancelled
          "Order %d=%d from site %d was cancelled!"
     4. an order for which a change comes is in local correction. Here, the status "303 - Dispatch
        planning" is also checked.



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                            120
        "Caution: order %d=%d from site %d change failed - already released!"
    5. the check for local correction has failed.
        "Caution: order %d=%d from site %d check for local correction incorrect"
    6. an order for which a change comes was changed at the production site
        "Caution: order %d=%d from site %d local correction was overwritten"



         14.1.6.         Message 67
If at the production site there is an automatic delivery date shift (e.g. initial scheduling and
delivery date calculation), the order status 206 - delivery date shift is booked by the system. If the
status return is configured and this status 206 is transferred to the distributor, the message 67
can be sent there.

    •    67 – delivery date shift at the production site (starting with ALCIB-VERSION 2008) (also
         goes to the person entering the document (order/PO)

The status return is logged in $DFUEDIR/proto/rmin* (distributor) and rmout* (production site)

See also section "Report for delivery date shifts at the production site"


         14.1.7.         Message 95
[AW-137151] // October 2023
If in the production site there is a manual change of the goods receipt date of a downstream PO
(AVIS, order management), the status 204 - goods receipt shift for the PO and the affected orders
is booked. If the status return is configured and this status 204 is transferred to the distributor,
the message 95 can be sent there.

    •    95 - Internal EDI: goods receipt postponement

QR 24/02 (February 2024): To whom the message is sent can be configured via the message
configuration and the environment variable "AVISE_MAIL".

The status return is logged in $DFUEDIR/proto/rmin* (distributor) and rmout* (production site)

See also "EN-CONFIG-A+W Enterprise" section "Dispatch notification".


         14.1.8.         Old reporting system (ibin.meld)
The distribution of reports for the internal order EDI can either be done in the file ibin.meld (old
system) or in the ALCIB reporting system.


Up to version 2011



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                   121
If the distribution of the reports should be maintained in A+W Enterprise, the file ibin.meld must
include an entry with dummy recipient for each report type so that the report can be sent. If this
file contains more than one recipient per report type, the report in question is sent multiple times
to the report recipient stored in A+W Enterprise.


The file ibin.meld in $ALDATPFAD includes the reference to the employees who receive the
reports from the order transfer (trm_ctrl). The structure is:
<Typ> < manr> <signal>
If signal=1, a report of the type <Typ> is sent to the employee <manr> and a signal to open the
postbox is sent.
If signal=0, the signal is omitted.
Caution: if the hausnr of the employee in mitarb != is the own hausnr, a transfer of the report to
the hausnr is triggered from mirarb. With incorrectly maintained master data, this can cause a
significant number of reports since the report that of the unsuccessful transfer can also not be
transferred successfully.
Entries for up to 10 employees are possible. The defined types so far are:
0 - orders or quotations have arrived/were generated
1 - orders or quotations were changed/cancelled
2 - not used
3 - not used
4 - the report received has the rush identifier
Recommended is the setting of signal for type 4 and possibly for type 1. Type 0 should only be
used for rare order receipts!
Example:
0 1234 0
1 1234 1
4 1234 1
0 343 0
1 343 0
4 343 0
Employee 343 does not have to react directly, but would like to have an overview of the orders.




A+W Software GmbH                     EN-CONFIG-A+W Enterprise EDI.docx                           122
15. External Order Interface/EDI import
    15.1. Introduction
The external order interfaces handle the automatic bilateral transfer of orders between customer
and glass producer. A+W offers primarily a general standard interface, which both conveys in-
house products between one another (Cantor – A+W Enterprise, A+W Business – A+W Enterprise,
A+W Enterprise – A+W Enterprise), and is filled by various third-party companies, e.g. 3E. In
addition, it is also possible in consultation between customer, glass producer, and A+W to
develop special solutions based on the general interface logic.
The complexity of the individual interfaces ranges from very simple (forwarding of simple orders
without exchange, shapes or muntins) and the generation of confirmation data records for
scheduling of the orders in A+W Enterprise. The automatic splitting and pre-sorting of the EDI
orders across different production lines can also be implemented individually. Which possibilities
the individual interface offers must be clarified explicitly if necessary since the interfaces are also
enhanced constantly.
The external order interfaces handle only the generation of new documents (orders, quotations);
none of the interfaces is in a position to make changes to existing orders or to cancel existing
orders!




    15.2. Checklist

Housekeeping                      Individual script for cleaning
                                  up individual directories
Tableexbartyp                     Default values for item Default shape from exbartyp
                                  referencing via interface must exist in the shape
                                                            master data.
                                                                    Default article for frame
                                                                    exchange absolutely has to be
                                                                    of type frame/colored frame.
                                                                    You should work with prefixes
                                                                    from the very beginning since
                                                                    an adjustment after the fact is
                                                                    difficult.
Startroutine                      Start script                      Clarification           and
                                                                    documentation of the process
                                  Cron entry
                                                                    how the files come from the
                                  Individual program                customer to the computer
                                                                    and how the scheduling is
                                                                    started.
BOM change                        DFUE_OPT_POSKONR


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  123
Processing replacement            DFUE_BEA_NEU                      Replacement      rules   for
                                                                    processings are supported. If
                                                                    the variable is not set, no
                                                                    replacement      rules   for
                                                                    processings may be created.
                                                                    This would cause defective
                                                                    BOMs.
                                                                    Price and print ID from E/A
                                                                    rules are transmitted along
                                                                    with the order (otherwise
                                                                    not, but rather permanently
                                                                    defined)
Parallel processing of files or DFUE_JOBCTRL                        Only if the interface is
storage of files for different                                      adjusted       for     parallel
customers in a call                                                 processing and this variable is
                                                                    set is it possible. Otherwise,
                                                                    only one customer may be
                                                                    edited with a call.




    15.3. Configuration – AWE master data
The customer for the purchase order, which is imported via EDI into AWE, has to be created in the
AWE master data.


    15.4. General procedure
The automated scheduling of third-party orders via EDI takes place in several steps:
First the order data is imported by the actual filter program into intermediate tables. These
intermediate tables all begin with the abbreviation _ialf_ (z.B. _ialf_kauf, _ialf_kpos, ...). In this
phase, the input raw data for the background processing is prepared by the trm_ctrl (step 2). This
step is logged in $DFUEDIR/proto/[<hausnr>/edi/]<filter>*.
After the actual filter has performed its task, the orders are processed further by the trm_ctrl
function exbin(). Here, all the data from the _ialf tables in the A+W Enterprise data structured is
implemented. This is also where the item implementation takes place. This step is logged in
$DFUEDIR/proto/[<hausnr>/exbin/]exbin*.
Then, another step is performed by the trm_ctrl function ibin(). Here, the order number is
assigned and the data finally written to the A+W Enterprise data structure. This step is logged in
$DFUEDIR/proto/[<hausnr>/ibin/]ibin*.
After the trm_ctrl has finished its work, the order is forwarded to the background process
"intauf." In this step, the BOMs are established, for example, and required additional data from
the item and market partner master data determined. During establishment of the BOM, the
intauf evaluates the exchange/additional rules written by trm_ctrl.
The trm_ctrl itself does not generate any BOMs or other data that depends on these. It only
forwards information via the exchange/additional rules for changes to the master data BOMs.

A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  124
    15.5. File processing
The interface programs receive files with order data that are placed in the input directory for
processing. For each interface (and/or each customer), an individual input directory that is in the
directory $DBPATHEXT/extern can be defined.
WARNING: The parallel call of the interface program is only permitted if the interface is
prepared for this and the environment variable DFUE_JOBCTRL is active! Otherwise, care must
be taken in the calling script that there is no parallel call. In addition, only files of one customer
may be processed per call. If different customers' files are processed, the item references in the
order are incorrect.
Below the input directory, there is a directory "save" in which the processed files are backed up.
NB: During each installation of an interface, care must be taken that this back-up directory is
managed appropriately (cleaned out from time to time)!

Only standard interface:

Starting with Version AWE 6, depending on the processing status, it is possible to shift the
interface files from the program reading the information in into 2 different subdirectories. Here
the environment variables DFUE_ERROR_SUBPATH and DFUE_SUCCESS_SUBPATH must be set.

In the environment variables DFUE_ERROR_SUBPATH and DFUE_SUCCESS_SUBPATH the
directories are specified in which the import routine should move the interface files. This function
also requires the configuration of DFUE_JOBCTRL.

If one of the variables named above is set, then only one order (a K1 order) may be contained per
interface file. If there are several orders in a file, the file will be moved to DFUE_ERROR_SUBPATH.

WARNING: The parallel call of the default filter is only allowed if the environment variable
DFUE_JOBCTRL is active! Otherwise, care must be taken in the calling script that there is no
parallel call. If DFUE_JOBCTRL is activated and one of the variables DFUE_ERROR_SUBPATH or
DFUE_SUCCESS_SUBPATH is set, only one order per interface file may be sent.

If DFUE_JOBCTRL is active and DFUE_ERROR_SUBPATH or DFUE_SUCCESS_SUBPATH are not set,
then the calling script must ensure that transfer files are not imported several times. The danger
is that in a call many/large files are read in, which require several seconds for processing.

The transfer files may only contain printable characters in ASCII format (see development
#423337) and must naturally satisfy the interface description; they are stored in the input
directory on arrival. How these files arrive doesn't matter in principle; they can be stored via ftp,
as e-mail attachment or created manually via editor. However, it must be ensured that the files
can be read directly by the UNIX server (Samba, ftp). And in addition, in each case it must be
ensured that the storage process does not process any files that have not yet been transferred
completely. Some filters (e.g. the default filter) evaluate the file themselves for this: only files that
include an end mark are completely transferred and will be processed.

Only default interface


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  125
The import routine of the default filter itself checks the files transferred. The following is checked:

    -   Is the file transferred a regular file (and not a directory).
    -   If it is a regular file, there is an attempt to open the file for writing (file rights).
    -   If the file can be opened for writing, it is locked (parallel processing).
    -   If the file could be locked, there is a check whether the file end marking #END# is present.

If an error occurs in the cases described above, this is noted in the log
$DFUEDIR/i000filter_proto<site>_<mmdd>[_<hhmm_<pid>] and the file is skipped. (It is NOT
moved to the ERROR subdirectory. It remains in the original directory. The file is not moved to the
ERROR subdirectory since errors in the checks described above either prevent a moving or the file
is processed by another process).

Furthermore, the import routine checks the presence

-of the file header record FH
-of the order header K1
-of the item header P1.

If in the transferred file there is no FH, K1 or P1 record present, the file is moved to
DFUE_ERROR_SUBPATH.

At the start of the scheduling process, the input directory is checked by the start script to see
whether the files to be processed are available there. If so, they are fed in for further processing
(via command line parameters of the filter call) and then shifted to the back-up directory and kept
there.
The filter programs are started by shell calls, whereby command line parameters must be passed
to them. Which parameters are to be passed how is very filter-individual and can therefore not be
discussed in detail here. In the course of adjustments and additions, the programs are equipped
bit by bit with simple help texts so that it is worthwhile to start a search with "i<nam>filter –h."
During import, the files to be processed are naturally transferred to the filters, but under some
circumstances also the customer number (e.g. ianafilter) or a work mode (generally "1" for
import).

Sample solution

A Unix Cron job is defined for the user alcibnet. It runs every 5 minutes within standard working
hours on all days of the week.

Cron entry
#INPUT EDI orders
*/5 7-18 * * * /usr1/alcibnet/bin/get_edi_order <site>


The script /usr1/alcibnet/bin/get_edi_order generates a task file $DFUEDIR/wait/get_edi.$$.r$1.
This file is then processed accordingly by dfue_starter.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                126
Within the task files for the dfue_starter, the script $ALCIBPRG/spec/cmd/auto_start_i000filter is
called. This script is linked to the script $ALCIBPRG/spec/cmd/call_i000filter and
$ALCIBPRG/spec/cmd/cleanup_indir.
NB: The script cleanup_indir is no longer required if you are working with DFUE_ERROR_SUBPATH
and DFUE_SUCCESS_SUBPATH.
auto_start_i000filter:
The script checks the input directory $DBPATHEXT/edi/i000filter for interface files with the
extension*.edi *.ASC *.asc and assigns the variable FILES all files found.
If files exist, the variable DFUE_FILTERSTART is assigned the value “call_i000filter” and the
trm_ctrl is started with the parameters for the external EDI.
Protocol: $DFUEDIR/proto/ i000_proto<site>
The trm_ctrl itself then starts the script call_i000filter. The script call_i000filter starts the interface
program “i000filter” for all files in the variable FILES.
Depending on the configuration, the files are shifted to the subdirectories.
The sample configuration is available in the development environment. The sample configuration
must be adjusted to the individual circumstances at the customer.



Scripts:
get_edi_order
[ -z "$DFUEDIR" ] && DFUEDIR=/usr1/alcibnet
[ -z "$ALCIBPRG" ] && ALCIBPRG=/develop/alcib/13/0/de/
echo "$ALCIBPRG/spec/cmd/auto_start_i000filter" > ${DFUEDIR}/wait/get_edi.$$.r$1
echo "#END#" >> ${DFUEDIR}/wait/get_edi.$$.r$1


auto_start_i000filter
#Logging:
  HAUS=`gethnr`
  PROTO=`getalenv "DFUEDIR"`/proto/i000_proto$HAUS
  echo "<>---<>---<>---<>---<>---<>---<>---<>---<>---<>---<>" >> $PROTO
  echo $0 $* started at `date` >> $PROTO


  #search for files to be processed:
  cd $DBPATHEXT/edi/i000filter
  echo going to spool directory: rc=$? >> $PROTO
  echo Spool Directory is `pwd` >> $PROTO
  FILES=""
  FILES=`ls *.edi *.ASC *.asc`


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                   127
     echo search for files: rc=$? >> $PROTO
     if [ -z "$FILES" ]
          then
          echo nothing to do >> $PROTO
          exit 0
     fi


     DFUE_FILTERSTART="call_i000filter"
     INDIR=`pwd`
     export INDIR
     export DFUE_FILTERSTART
     export FILES
     export PROTO


#NB: So that the screen structure in ALCIB does not get
# confused, the trm_ctrl must be called with suhup.
     echo start trm_ctrl at `date` >> $PROTO
     sunet suhup trm_ctrl 20 1 20 0 $HAUS $HAUS 0
     echo call to trm_ctrl: rc=$? >> $PROTO
;;
call_i000filter)             #Call filter from trm_ctrl
     #Logging:
     HAUS=`gethnr`
     PROTO=`getalenv "DFUEDIR"`/proto/i000_proto$HAUS
     echo "---" >> $PROTO
     echo $0 $* started at `date` >> $PROTO
     echo "calling i000filter 1 $FILES 2>&1 >> $PROTO"
     i000filter 1 $FILES 2>&1 >> $PROTO
     echo call to filter: rc=$? >> $PROTO
     export INDIR
     export FILES
     export PROTO
# cleanup_indir /* siehe DFUE_ERROR_SUBPATH DFUE_SUCCESS_SUBPATH */
;;
cleanup_indir)              #Clean processed files


A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx   128
     #Logging:
     HAUS=`gethnr`
     PROTO=`getalenv "DFUEDIR"`/proto/i000_proto$HAUS
     echo "---" >> $PROTO
     echo $0 $* started at `date` >> $PROTO
       cd $INDIR
       echo going to $INDIR: rc=$? >> $PROTO
       echo moving files to save: $FILES >> $PROTO
       mv $FILES save/ 2>&1 >> $PROTO
       echo moving files: rc=$? >> $PROTO
;;
Esac



Internal client separation

Taking into consideration the restrictions defined in "DE-CONFIG A+W Enterprise Internal Client
Separation," the scheduling of the external orders can be done directly on an internal client
(#428675). For this, care must be taken that in the script "auto_start_i000filter" the trm_ctrl is
called with the appropriate site number (parameters 5 and 6). The best way for this is the call via
the cron with the appropriate parameter for get_edi_order <site> since here the entire
environment for the sites is established.
Calling the script "auto_start_i000filter" directly via the menu item "Individual programs" usually
leads to the storage in the main client. To avoid this, a separate *.prog file must be created for
each internal client in the frontend configuration, which is then used for storage.


      15.6. Item implementation / Product referencing
          15.6.1.           Default data and prefixes (table exbartyp)
The table exbartyp is a central control table and must be maintained. In it, default values are
specified for each interface type. No maintenance dialog exists for this table.
The table includes the fields dfuetyp, artyp, prefix, defartnr
In the "defartyp" field, a key value defined by A+W is entered per interface.


Interface                   Key value                Binary file
FENDATA                     0                        ifenfilter
ANALYTIC                    1                        Only up to AWE 5
EGOKIEFER                   2                        iegofilter



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                             129
SGPI                    3                        Only up to AWE 5
SKANDINAVIA             4                        iskafilter
VELFAC                  5                        ivelfilter
HUEPPE                  6                        ihuefilter
WIRUS                   7                        iwirfilter
KERMI                   8                        ikerfilter
WINDOWMAKER             9                        iwinfilter
KLAES                   10                       Only up to AWE 5
DUSAR                   11                       Only up to AWE 5
LIDO                    12                       Only up to AWE 5
BREUER                  13                       Only up to AWE 5
BRAND                   14                       Only up to AWE 5
TELEGLAS                15                       itelfilter
IVB                     16                       Only up to AWE 5
STDFILTER               17                       Only up to AWE 5
KONFILTER               18                       Only up to AWE 5
I000FILTER              19                       i000filter               A+W standard
                                                                          interface
IKORFILTER              20                       Only up to AWE 5
VEROMCO                 21                       iverfilter


In the "artyp" field, a key value defined by A+W is entered per item type and interface. These are
not the item types of the A+W Enterprise item master data, but rather different objects that the
external order interface handles.
Trade                            0                                NIU (Not In Use)
IG                               1                                Currently used for all items
Muntins                          2
Shapes                           3                                Default shape must exist in
                                                                  the shape master data
Replacement                      4
Default customer                 5
Pressure compensation            6                                Pressure compensation: a
                                                                  prefix is absolutely necessary!
Spacer                           7
Gas                              8
Processing                       9



A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                  130
Color                             10
Dimensional variant               11
Entered by                        12
Other articles                    13
Step                              14
Project                           15
Product set item                  16
Product set customer              17
Width                             18                                starting with QR 07/2021 -
                                                                    trm_ctrl - 13.04.6133
Height                            19                                starting with QR 07/2021 -
                                                                    trm_ctrl - 13.04.6133
Employee                          20                                Employee in orders that come
                                                                    in via external EDI if no
                                                                    employee is sent via the
                                                                    interface (kauf.eusr)


A free text is entered in the "prefix" field. For the implementation, the customer item number in
the A+W Enterprise item number is required. The prefix is added before the search for the
customer item number.
It is urgently recommended that you work with prefixes for article replacement from the very
beginning. Changes after the fact are time-consuming and error-prone.
Example: customer IG item 1234 and customer muntin item 1234
"iso" is in the prefix for ISO and "spr" in the prefix for muntins. For the implementation in the
A+W Enterprise items, now in case of the item, an item is searched for in which 'iso1234' is found
in "customer item number." In the case of the muntin item, an item is searched for in which
'spr1234' is found in "customer item number." Without this prefix, in this case the
implementation would not work.
This is especially important if the same customer article and item article as well as the BOM
article is sent (e.g., LAMI as item as well as part of an IG). If you are working without "prefix", it
will not work to import the LAMI as item article.
For clarification:
    a) Without prefix:
                 An ISO "A" is sent with a LAMI exchange "AB". Now the system searches with
        the customer article "A" iin artkuzu and kuaz and with the customer article "AB" in
        kuaz.
        A LAMI "AB" is sent as item article. Now the system searches with the customer
        article "AB" in artkuzu and kuaz.
    b) With prefix "iso" for item article:
                 An ISO "A" is sent with a LAMI exchange "AB". Now the system searches with
        the customer article "isoA" in artkuzu and kuaz and with the customer article "AB" in
        kuaz.


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                131
       A LAMI "AB" is sent as item article. Now the system searches with the customer
       article "isoAB" in artkuzu and kuaz.
    c) With prefix "aus" for glass replacement:
                An ISO "A" is sent with a LAMI exchange "AB". Now the system searches with
       the customer article "A" in artkuzu and kuaz and with the customer article "ausAB" in
       kuaz.
       A LAMI "AB" is sent as item article. Now the system searches with the customer
       article "AB" in artkuzu and kuaz.


In the "defartnr" a default value is entered depending on the item type and interface. In case a
referencing of customer details cannot be executed, this default value is taken over into the
order. Thus the order is in the system and it can be changed accordingly and it does not have to
be entered completely manually.
Item designation
If in the master data – item master data – market partner details or master data – market partner
master data – item assignment for a market partner and item an "external designation" is
maintained, this is taken over into the order. This applies for items and muntins.
     Table „artkuzu“
Caution: If the environment variable "KUBEZ_STCKLST" is set, this customer-specific item
designation is also taken over during the manual document entry into the generated texts.


    15.7. Article assignment / article implementation
FILTER
During the preparation of the order data, each customer article number is provided with a prefix
in order to prevent a situation where a customer article number is identical to an ALCIB article
number. Which prefix this is can be defined in the table exbartyp per interface. In the filter, if
necessary implementation is done according to the E/A debtor number (not for each filter), as
well as the model assignment. The data prepared this way is stored in the _ialf intermediate
tables ("_ialf_kauf", "_ialf_kpos" etc.). After the filter program has finished its work, trm_ctrl
takes over the further manipulations in the 2nd step 9exbin). The article assignment and article
replacement take place in this second step:
Item articles and muntins are executed via the "article execution" in the market partner master
data (table _artkuzu)
Master data - Market partner - <Menu> - Article assignment
Master data - Articles - <Menu> - Market partner details
Processings, accessories, and exchange glass is referenced via the additional exchange rules.


exbin
For each incoming customer article number, an assignment rule is searched for in the table
artkuzu and the ALCIB article number stored there is entered instead of the kuartnr in the item;
search key is kunr+kuartnr. If an error occurs here (no rule found or several rules present), the
dummy article number stored in the table exbartyp is used. If this is the case, then the system can


A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                 132
be configured so that this order is still scheduled, but not released (environment variable
DFUE_DUMMYART_NORELEASE). The airspace (dimension 3) and the spacer deduction dimension
(dimension 11) are stored in the table artkuzu. (However, the default interface allows the
takeover of individual sheets airspaces from the itnerface.)
In addition, the system can be configured so that after a failed implementation, it is checked via
the table artkuzu whether the article transferred is an ALCIB article (environment variable
DFUE_OHNE_ARTKUZU).
After the basic assignment has been made, the program checks whether there are E/A rules for
this article. If this is the case, they are applied. At least for some interfaces, it is also possible to
initiate an exchange from the outside; that is, it can be recognized whether an incoming article is
a BOM exchange article for the current header article. For this, a rule is searched for analogously
in the table kuaz and applied. Here only the market partner-specific exchange/addition rules are
evaluated. The general exchange/addition rules are not applied. The exchange/addition rules
from the tables artkuzu and kuaz determined for an order or imported from the interface file are
written to the table _ikuaz, where the order completing (process "intauf") reads them out and
processes them in step 4. Key is the internal order number (aufnr) and item number (posnr), so
that the rules can be applied item by item. Processed orders are not deleted from this table. If
excess data quantities have accumulated, then the table can be emptied if no orders are currently
being processed by the internal or external EDI or the order completing. Here, you should be
absolutely sure that there are no entries yet to be processed; that is, only delete the table content
if there are no order before intauf! However, this should not normally be necessary since this
table (starting with ALCIB 3.0) is incorporated into the deletion routine of the autorechsave
program.
If an interface allows exchange to the fullest extent, the following picture arises:
a) Customer orders his article, etc. for which there is a simple mapping to an ALCIB article. The
   mapping is done using the table artkuzu; since there is no entry in kuaz, this article is taken
   over unchanged.
b) Customer order his article xyz, for which there is also an ALCIB-internal exchange/addition.
   After the mapping with artkuzu, the relevant entry is found in kuaz and the addition is made.
c) Customer orders his article abc with exchange by his article def. In this case, the system finds
   another entry for this article def in kuaz, with which this case is processed. Each additional
   addition rule found overrides the previous one (b overrides a, c overrides b).

Customer
                                                ALCIB


                  artkuzu
uvw     ------------------------------->        500044
                  artkuzu
xyz     ------------------------------->        500044               (basic article)
                  +kuaz -----------------> - 100004, + 300005        (exchange)




                  artkuzu


A+W Software GmbH                          EN-CONFIG-A+W Enterprise EDI.docx                          133
abc     ------------------------------->        500044                                (basic article)
                  +kuaz ------------------> - 100004, + 300005                        (exchange)
+ def                          + kuaz ----->             - 100004 + 300008     (customer exchange)


After successful data preparation, the orders get actual order numbers (here, external and
internal order transfer run together) and they are placed by intauf for further processing in the
table aufint.


The coordination of the entire procedure is done with a start script to be created during the
installation. In this script, a) the incoming directory has to be searched for files to be processed, b)
the filter program called with the files found as command line parameter, c) the trm_ctrl is
started for the actual scheduling, and d) the processed files are captured. For the script there is a
general template (currently: "start_edi03"), which should be used if possible since it already uses
the new transaction logic (starting with ALCIB 2.12). According to the old variant, the script first
searches for files and starts the filter program, then calls the trm_ctrl, and captures the files last.
If necessary, it is checked beforehand with select on _ialf_kauf whether a scheduling is already
running and in this case interrupted; but there is no transaction backup between the individual
part steps. (before beginning and after completion of each scheduling, the intermediate tables are
deleted!)


According to the new logic, after reading in the files to be processed, first the trm_ctrl is called,
which then calls the filter and then continues with the actual scheduling. Thus, the entire process
is incorporated into the general transaction backing up of trm_ctrl. trm_ctrl gets the necessary
parameters to start the filter in the form of dynamic environment variables from the script. For
more details, see the script itself.


With regard to muntins, the following particularity has to be noted: muntin articles have to be
created as meta-parts so that the muntin takeover in intauf works correctly.



        15.7.1.             Evaluation of the replacement/addition rules
At the beginning of this section, reference was made to the fact that not all functions that support the
exchange/addition rules in the manual order entry are also supported within the external EDI.
Therefore, it will be documented explicitly here what is possible within the external EDI.
In connection with external data transfer, the E/A rules will be used to convert customized article
numbers into A+W Enterprise article numbers, and to complete the BOM.
The entries will be read in connection with the conversion of the items, processing, and accessories.
For conversion, all records will be used the customer number of which (or A/Z debtor) matches that of
the order, and the customized article number of which matches the transferred one, or is empty. The
general exchange/addition rules are not applied. If the field "customer individual article number" "is
empty", the system might use too many entries. This may happen if orders for one customer are
transferred, and also entered manually in A+W Enterprise.
With the appropriate configuration, analysis of the E/A rules can be limited. If environment variable
DFUE_NEW_KUAZ is set, the system will only read entries for item conversion if the customer number
of which matches that of the order, and the customized article number matches the transferred one,


A+W Software GmbH                          EN-CONFIG-A+W Enterprise EDI.docx                            134
or if the customer number matches that of the order, and the customized article number is empty, and
the product number is 99999999 or matches the converted item article. For processings and
accessories, only entries will be read the customer number of which matches that of the order, and
the customized article number of which matches the transferred one.
Converting an existing, external data transfer to the new function requires extensive tests with the
individual data.

Without variables, all rules of a customer for which the customer item number is empty or
corresponds to the one sent. The product number is not taken into account here.
from kuaz where
        kunr=$ialffk_sq_rkund and
    (kuartnr matches $artkuzukuartnr or kuartnr=" ")
    and kuliflag = 0;



With variable DFUE_NEW_KUAZ: All rules of a customer for which the customer article number
corresponds to the one sent OR all rules of a customer for which the customer article number is
empty and the (product number=99999999 or product number corresponds to the header article
sent.
from kuaz where
  kunr=$ialffk_sq_rkund and
    (kuartnr matches $artkuzukuartnr or
         (kuartnr=" " and
             (prodnr = 99999999 OR prodnr = $kposartnr)
         )
    )
              and kuliflag = 0;


In the standard, only additional rules for processings are supported. If replacement rules are present,
these can cause defective BOMs in the order.
Exchange rules
#373344 (A+W Enterprise 6):
i000filter build 13.04.0423 (Jan/2018)
trm_ctrl build 13.04.0423 (Jan/2018)
Replacement rules for processings are only applied if the environment variable DFUE_BEA_NEU is
active. This variable does not control any more.

Evaluation of the assembly position
Within the external standard interface, the assembly position (S1 record - pattern side) for a
replacement glass can be transmitted.
Starting with interface status i000filter Build 13.04.2130 and trm_ctrl Build 13.04.2150, another
evaluation of the assembly position for exchanged glass applies.




A+W Software GmbH                        EN-CONFIG-A+W Enterprise EDI.docx                            135
If no patterned side is defined in record S1 of the interface file (field is empty or a 0 is
transferred), the patterned side from article reference (exchange / additional rules) is used. If no
assembly position is defined, the assembly position of the master data BOM is retained for
multiple glasses (IG, LAMI).
The definition of field 15 'Pattern side' is as follows:
 Empty or 0 - no defined pattern side - The assembly position of the article referencing is adopted
(kuaz.pos), if none is defined there, the assembly position of the master data BOM is retained.
1 - The structure points inwards. This means:
     Glass 1 = assembly position 2
     Glass 2 = assembly position 3
     Glass 3 = assembly position 5
2 - The structure points outwards. This means:
     Glass 1 = assembly position 1
     Glass 2 = assembly position 4
     Glass 3 = assembly position 6
It is important that the article master data is created correctly. It is imperative that glasses always
have an assembly position within an IG BOM. For LAMIs, an installation item must always be
available if several fixed dimensions are on one BOM level. If there is no assembly position, no
correct glass replacement can be performed by the external EDI.


Insulated glass examples:
In the item master data, the IG is created with 2 glasses, A and B, with the assembly positions 2
and 3.
Now, a glass C is sent via interface as replacement for glass A. In the replacement rules, only the
item implementation, but not the assembly position is defined.



Now there are 4 scenarios depending on which value is transferred in field 15 (structure side) of
the S1 record in the interface file.
Value in Assembly           Reasons
the       position of
interface glass C in
          the order
00           2              No AP was sent and none was defined in the E/A rules => AP from
                            master data is retained
01           2              Assembly position was sent via the interface
(inside)
02        1                 Assembly position was sent via the interface
(outside)
             2              No AP was sent and none was defined in the E/A rules => AP from
<empty>                     master data is retained


A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                               136
If this glass C is sent as replacement for glass B, then the table looks as follows
Value in the        Assembly position of       Reasons
interface           glass C in the order
00                  3                          No AP was sent and none was defined in the E/A rules
                                               => AP from master data is retained
01 (inside)         3                          Assembly position was sent via the interface
02 (outside)        4                          Assembly position was sent via the interface
 <empty>            3                          No AP was sent and none was defined in the E/A rules
                                               => AP from master data is retained


Now, a glass D is sent via interface as replacement for glass B. In the replacement rules, the item
implementation and the assembly position are defined.



Now there are 4 scenarios depending on which value is transferred in field 15 (structure side) of
the S1 record in the interface file.
Value in the        Assembly position of       Reasons
interface           glass C in the order
00                  4                          No AP was sent and but AP 4 is was defined in the E/A
                                               rules
01 (inside)         3                          Assembly position was sent via the interface
02 (outside)        4                          Assembly position was sent via the interface
 <empty>            2                          No AP was sent and but AP 4 is was defined in the E/A
                                               rules
Price relevance
This is implemented customer-specifically. For the default interface, see detailed descriptions in
"DE-A+W EDI Import.pdf" section "4 A+W Enterprise import-specific function description" -
"BOM (S1)" - "Price relevance"


Procurement type

alcib - 13.04.10373 (June 2021)

        For product exchange via exchange/addition rules, with manual entry of the customer's
        desired supplier it is always taken over if for the product the procurement type = "PO" is
        permitted (one of the possible procurement types). For EDI orders, by contrast, the
        desired supplier is taken over if PO is created as the preferred procurement type. With a
        setting, you can adjust the logic for EDI orders to the manual entry and here too have the
        desired supplier taken over if one of the procurement types for the product is "PO."
Environment variable: INTAUF_CHECK_DFUE_WUNSCHLIEFERANT


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 137
Restrictions
    -   The field kuaz.ausvekt: "Auswertungsvektor" may not be filled with
        "0000000000000" if any entry about quantity or other parameters are
        transmitted. In this vector, the 1st and 2nd places are reserved for evaluation
        of Anzahl1 and Anzahl2.
    -   The effect of the exchange/addition rule is limited; you can't define any rules
        with conditions such as "exchange article X for article Y in a product Z only if
        article AA is also present in the BOM."
    -   You also cannot enter any rules for the article types of the product. Such as "In
        all IGs, article X should be exchanged for article Y." Either, you can create it
        generally:
        Exchange article X for article Y" - but this will also apply if article X occurs in
        another product.
        Or for all IGs, create an individual record.
    -   For evaluation of the EDI E/A rule, the records are always resorted by article
        type due to the muntins. This way, you can avoid first adding the muntins to
        the inner frame and then having the inner frame go lost due to the exchange.
        Thus, it is very important that muntin records refer to the article type frame
        (210 or 211). The exchange of the frames occurs directly via the article number,
        however.



    15.8. BOM change
Environment variable: DFUE_OPT_POSKONR
CAUTION: If the DFUE_OPT_POSKONR variant greater than 1 is used, an interface version greater
than or equal to 2.2.014 is assumed.

For searches examining why a BOM change has taken place or not, the Log
$DFUEDIR/proto/[<Mandan>/exbin]/exbin* is required.

Generally it should be noted that within the external order interface, the same function for BOM
change CANNOT be applied as for the manual document entry.

With external order scheduling, items with the same glass structure are provided with the same BOM
number.
The standard behavior within the external order scheduling with respect to BOM header change is as
follows:
The BOM header will be changed generally if one of the following conditions applies to two
consecutive items:

    1. The item article changes between two consecutive items
    2. In the current item, there is a glass replacement, however not in the item immediately
       preceding

A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                               138
    3. One of the replacement sheets changes between two consecutive items
    4. The pattern direction of one of the replacement sheets changes between two consecutive
       items
    5. The item includes a Georgian bar
    6. The item includes an addition or replacement for a processing step or accessory (e.g.
       spacer, gas)
    7. The product designation changes between 2 items one right after another (ID 119818)
    8. 06/19/2024: trm_ctrl - 13.04.11194: If using the E/A rules for the header article additional
       articles are inserted into the BOM without doing this via an S1 record in the interface file.
        [AW-175319]


As a result of conditions 5, 6 and 8, all order items may get a new BOM header although the
BOMs are identical. This happens for instance if all items were ordered with Georgian bars, and all
Georgian bars of the items are identical. Or, the standard spacer is replaced by the same special
spacer in all items.
This behavior wastes system resources and paper.
We have therefore developed a method to minimize the number of BOM changes.
With appropriate system configuration (CFUE_OPT_POSKONR), the BOM header will generally be
changed if one of the following conditions applies to two consecutive items:

    1. The item article changes between two consecutive items
    2. In the current item, there is a glass replacement, however not in the item immediately
        preceding
    3. One of the replacement sheets changes between two consecutive items
    4. The pattern direction of one of the replacement sheets changes between two consecutive
        items
    5. The product designation changes between 2 items one right after another (ID 119818)
    6. The AIR and/or AIR2 between 2 consecutive items changes
    7. The item contains an addition or replacement for a processing step or accessory that does
        not belong to type "Frame", "Muntin", "Stamp" or "Spacer." (stamp and spacer for
        DFUE_OPT_POSKONR > 1 => see below)
    8. One of the inside spacers (atyp 210 / 211) changes between two consecutive items
        (maximally two spacers will be checked). (only default interface (i000filter) and Vermonco
        interface)
    9. One of the inside spacers changes between two consecutive items (maximally two
        spacers will be checked).
    10. The current item includes a Georgian bar while the previous item does not, and vice
        versa.
    11. One of the Georgian bars changes between two consecutive items (maximally two bars
        will be checked).
    12. The Georgian bar colour changes between two consecutive items (maximally two bars will
        be checked).
    13. The muntin color changes between two consecutive items (maximally two muntin articles
        will be checked).
    14. Starting with QR 2304: Between 2 items that follow one another directly, the frame
        changes in which a muntin is installed. (see additional note below)
    15. The product color of the item article changes between two consecutive items
    16. One of the stamp article changes between two consecutive items (maximally three stamp
        articles will be checked). (only default interface (i000filter) and Vermonco interface)


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                              139
    17. Starting with trm_ctrl 13.04.1758 and i000filter 13.04.1757: between 2 directly
        consecutive items, one of the spacers changes (a maximum of 3 spacers (atyp 220) are
        checked). (only default interface (i000filter) and Vermonco interface)
    18. Starting with trm_ctrl at the end of July 2021 [AW-57149]: If the background iTOE was
        activated, then it is also checked whether the template changes between 2 subsequent
        items. If this is the case, then a new BOM number is assigned. Here it is not checked
        whether the template includes additional processings that change the BOM. The external
        order interface has no access to the content of the templates.
    19. 06/19/2024: trm_ctrl - 13.04.11194: If using the E/A rules for the header article additional
        articles are inserted into the BOM without doing this via an S1 record in the interface file.
        [AW-175319]


    DFUE_OPT_POSKONR = 1 > check of the conditions 1 – 15 and 18-19
    DFUE_OPT_POSKONR = 2 > check of the conditions 1 – 16 and 18-19
    DFUE_OPT_POSKONR = 3 > check of the conditions 1 – 19

Note about point 14: Within the interface, there are 2 possibilities for attaching a muntin to the
first frame.
     a) The muntin is sent directly after the first frame (ialf_spross.rahmenpos=[2|4])
     b) The muntin is not sent directly after the frame (ialf_spross.rahmenpos=0)

Point b) is still supported for compatibility reasons. If in 2 items that follow one another directly
both different ways are used, then within the order, this creates different BOMs since in this case
the interface does not determine the frame.

The change of BOM upon a change of airspace/airspace2 and of the color was added to avoid
having to check the complete BOM. The reason is that usually, the BOM should be changed if the
supply type of a variant or color article changes. For Georgian bars and spacers, the system now
assumes that variants always refer to the color or the airspace. This also applies to the BOM
elements of the spacer or Georgian bar. To avoid having to analyse the BOM structure of the
Georgian bar and the spacer, as well as the corresponding variants and supply types, the change
of BOM now depends on the relevant criterion (colour/airspace).
Generally, during external order scheduling, the comparison described above will only take place
with only two directly consecutive items. If the standard spacer is maintained for the first item
(BOM 1),and changed for the second item (BOM 2), while the standard spacer is used again for
the third item, BOM 3 will be used for item 3; not(!) BOM 1.
ATTENTION: If Georgian bar or spacer variants should be selected not with standing the color or
the airspace/airspace2, this function cannot be used and will cause severe errors.
Prior to(!) switching to the new function, intensive tests with real base data and interface files will
be necessary.


        15.8.1.         Customer-specific BOM change
[AW-212532] // July 2025 // trm_ctrl - 13.04.12975
CAUTION: The use of this function can cause defective BOMs and orders and therefore must be
tested precisely. In addition, within the stored procedure, there must be appropriately
meaningful documentation or a reference to such.



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                140
If the environment variable DFUE_OPTPOSKO_SP is active and the Stored Procedure (SP)
"cu_dfue_optposko“ exists, this SP is called with the parameters AUFNR, VORGANG, HAUSNR
(ibin). No return value is expected.
Within this SP, the field POSKONR in the tables KPOS and KSPROSS can be adjusted individually.
Here, the content of the tables _ikuaz, kuaz, struct should be analyzed.
The following restrictions must be heeded here:
    A) Within the table _IKUAZ (order-specific exchange/addition rules), the rules for the first
       POSNR of a BOM are written. If the item 3 and 4 have the same BOM, then for the
       POSNR=3 there are records in _IKUAZ.
    B) Within the BOM assignment, it is decided permanently in the program (exbin) whether a
       BOM assignment via a customizing may be changed or not. In this case, the field
       kpos.handshake is set to 1.
        1 - BOM number (POSKONR) may not be changed with customizing
If this setting within the customizing is ignored, it can cause defective BOMs.
The code is set to 1:
    -   Generally if this is a product set creation (vorgang= 14)
    -   GEnerally if the environment variable "DFUE_GLAMA_FEBA" is active
    -   The item article changes
    -   It is a product set item
    -   If the article name of the item article changes
    -   If within the item article glass is exchanged via the interface
    -   If the structure code of one of the lites changes via the interface
    -   If it is a stock size bundel item
    -   If the assembly position changes coated glass
    -   If it is a dog door


    15.9. Special order interfaces
A+W supports various order interfaces. These have individual structure and functions. There is
individual documentation for the respective interfaces.


        15.9.1.    Default                                order                        interface
            i000filter
The interface description and the essential functional characteristics are described in a separate
document (EN-A+W EDI Import.pdf).
        Known restrictions
    •   No foil exchange in LAMI is possible
    •   For multiple glazing, a maximum of 3 lites can be processed. If more lites are sent,


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                141
    •   No exchange of glass and foils in LAMI in IG is possible
    •   No targeted processings on glass in multiple glasses are possible
    •   No pure muntin orders are possible
    •   There are restrictions with regard to the use of product sets. Details are documented in
        the interface documentation "DE-A+W EDI Import.pdf" section 4.


        15.9.2.         Kermi order interface
This is a customer-specific interface. The corresponding documentation is on the SharePoint
under \A+W Clarity R&D - Dokumente\Interfaces\Enterprise\External Order Interfaces\A+W
Kermi.pdf
Adjustments to this interface are made exclusively at the request of the customer using it.


    15.10. Product sets
Within the external EDI, product sets can be supported. For information about how this is handled
in the individual interfaces, see the individual interface descriptions.
In principle, the following restrictions and prerequisites apply:
    •   For this, A+W Enterprise must be configured for the entry of product sets.
    •   The product set name may not contain the following characters:
        ''      (0x20) space (SPC)
        '\t'    (0x09) horizontal tab (TAB)
        '\n'    (0x0a) newline (LF)
        '\v'    (0x0b) vertical tab (VT)
        '\f'    (0x0c) feed (FF)
        '\r'    (0x0d) carriage return (CR)

    •   Each product set may consist of precisely one item.
    •   Dimensions of the product can be changed
    •   Within the product set, only the exchange of the header item is possible while retaining
        the processings defined in the product set. (see DFUE_PRODSET_EXCHANGE_RESTRICT)
    •   Within the product set it is possible to change the shape dimensions and the shape
        number.
    •   Transfer of consignment is possible.
    •   Transfer of customer item (kuposnr) is possible.
    •   The takeover of an item price is possible (February 2020)
    •   Transfer of item texts is possible (starting in October 2020)
    •   The takeover of file attachments is possible (January 2021): here, however, you have to
        make sure that the attached document is not copied into a new order-specific directory,
        but rather remains in the old storage location. In the new order, reference is made to the
        storage location from the product set with a reference. This means that if the document is



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                               142
        changed, it is changed in the product set and in all orders generated via external EDI in
        which the product set was used.


If a packaging type is entered in the product set on the item level, it will also be taken over into
the order. Regardless of INTAUF_DFUE_VERPACKART.
For information about how the data has to be transferred and how the functions work in detail,
see the individual interface descriptions.
Data details that are not listed explicitly here can currently not be changed via interface.


     15.11. Configuration Options
        15.11.1.         Parallel processing
Caution: heed compatibility list
WARNING: The parallel call of the interface program is only permitted if the interface is
prepared for this and the environment variable DFUE_JOBCTRL is active! Otherwise, care must
be taken in the calling script that there is no parallel call. In addition, only files of one customer
may be processed per call. If different customers' files are processed, the item references in the
order are incorrect.
If you are working with the following interfaces in the appropriate versions, the configuration can
be converted to parallel processing. In this case, scheduling can be done into each site directly.
No    Filter                       Parallel
.
1     i000filter                   starting with 4.5 (2011)
2     Iskafilter                   starting with 4.3 (2008.2)
3     Iverfilter                   starting with 4.3 (2008.2)
                                   23.11.2022: No longer in
                                   AWE6
4     Iegofilter                   starting with 13.0 (AWE 6)
5     Ifenfilter                   starting with 13.0 (AWE 6)
6     Ihuefilter                   starting with 13.0 (AWE 6)
7     Ivelfilter                   starting with 13.0 (AWE 6)
8     Iwirfilter                   starting with 13.0 (AWE 6)
9     Itelfilter                   starting with 13.0 (AWE 6)
10    Ikerfilter                   starting with 13.0 (AWE 6)
11    Iwinfilter                   starting with 13.0 (AWE 6)




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                   143
Requirements
(installation package Version 2011)
New tables
The following tables must be present
    •   ialf_jobctrl
    •   ialf_aufctrl
    •   ialfversion: In the table, the field "lcleanzeit" must be present. If it is not present, an
        appropriate script must be executed.
Old tables
The table _kuaz may not be present. If it is, it must be deleted with a "drop table" statement.
Number ranges
The number ranges
    •   ialfaufnr
    •   erriaufnr
must be created DISJUNCT(!)in the table nr_kreise.


Installation of a parallel filter and the parallel trm_ctrl
Version 2008.2
In Version 4.3.3, an ISKA filter (build >= 8) may only be installed together with a trm_ctrl (build >=
20).
Before the first start-up of a parallel filter Version 4.3.3 (build >= 8), the table ialfversion may NOT
contain a data record.
If the filter has run once, it should be checked as a test whether the table "erri_kauf" is now
present.
If the table is not present, you must check in the filter log why the "create table" statement was
not executed.
Version > 2008.2
If the installation of all tables has gone properly, next it should be checked as a test how the lock
level for the transfer and error tables is set:
        select tabname, locklevel from systables where tabname like '%_ialf_%';
Lock level should be "R" (row) so that with parallel filter running there are no insoluble lock
situations.
After installation, the external order scheduling works as usual as long as no additional
environment variables were activated.
If the environment variable "DFUE_JOBCTRL“ was activated, the filter can be executed several
times in parallel.
The filling of the _ialf tables happens as usual, with the difference that the aufnr used during the
scheduling is obtained from a special number range (ialfaufnr).



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                 144
Log:
(see also 1.1 Logs)
Change with case 177216:
With switched on variable DFUE_JOBCTRL
Filter now writes process logs in proto subdirectories, specifically filter log ->
$DFUEDIR/proto/<haus>/edi/


With switched-on variable DFUE_TRM_SIMULTAN
trm_ctrl now writes process logs in proto subdirectories, specifically:
ueber_err log -> proto/<haus>/global/
ibin log -> proto/<haus>/ibin/
ibout log -> proto/<haus>/ibout/
exbin log -> proto/<haus>/exbin/
The logs are no longer combined automatically. For this, an appropriate script must be started.
(see case)


The logs are no longer combined automatically.


Filling the erri tables (only iskafilter)
If the environment variable DFUE_FILL_ERRITAB (with active DFUE_JOBCTRL) has been activated,
particular errors in the ISKA filter cause the error tables (erri tables) to be filled.
The erri tables are a table set that is structured exactly as the set of the _ialf tables. If a particular
error occurs in an order or in an order item, the whole order or the whole order item is
transferred with all order header data to the erri tables. The order thus receives an aufnr from the
number range "erriaufnr."
For each error item, a separate error order is generated in the erri tables.
Then the scheduling of the current file is continued.
The following defined errors create an entry in the erri tables:
    •    No valid product set could be found in the master data (error 3001)
    •    The object number of the current sash record does not fit the object number of the order
         (error 3002)
    •    The current setid cannot be found in the master data for the configurable fields (error
         3003)
    •    The number of item records of a transfer master record does not match the number of
         item records for the product set in the master data (error 3004)
    •    The number of item records of a glass spec master record does not match the number of
         item records for the product set in the master data (error 3005)
    •    For a transfer master record, for the transferred ACOS item, no ALCIB item number was
         found in the master data (error 3006)



A+W Software GmbH                     EN-CONFIG-A+W Enterprise EDI.docx                                145
The error cause (error number) that caused an entry in the erri tables is stored in the table
erri_aufzu. If the error only affects one item of an order and the remaining order can be
scheduled in ALCIB< erri_aufzu includes the assignment to the ALCIB order in the field alcibaufnr.
Control tables:
For each filter run, the tables ialf_jobctrl and ialf_aufctrl are filled.
ialf_jobctrl
The table includes information about which file was imported.
ialf_aufctrl
The table includes the information about which orders within which jobs (a job corresponds to a
scheduling file) were imported.
In the table, the orders are also stored that refer to an entry in the erri tables. The error orders
are marked with the status 400.
Parallel mode of the trm_ctrl
If the environment variable DFUE_TRM_SIMULATN was activated, the trm_ctrl can be executed
several times in parallel for external scheduling (dfuetyp 20).
As opposed to the usual version of the trm_ctrl, the parallel trm_ctrl always forwards the orders
to be scheduled individually (in completed documents) to intauf.


         15.11.2.         Templates
In order to work with templates within the external default order interface, the "A+W Enterprise
CAD Service" must be installed and configured. How it is installed and configured is documented
in the appropriate installation and configuration instructions for the service.
EN-CONFIG-A+W Enterprise CAD Service.pdf
EN-INST-A+W Enterprise CAD Service.pdf
In order to apply templates,
    1. MODUL_SN_TEMPLATE must be active
    2. SNFILES_DIR must be defined and activated
    3. SN_CADFILES_DIR activate
    4. SN templates are created and stored in $DATEI_REF_PFAD/template. Caution: Here the
       environment variable will be evaluated globally and not client-specifically.
    5. Templates must be created in the CAD service configuration (A+W Enterprise 6 CAD
       Service Config Tool).
    6. Enter template name and SN parameter name in the A+W Enterprise master data under
       Master Data > Keys > Product > Template parameters. Important here is that the
       sequence of the parameters per template is defined precisely in the sequence in which
       they will later be transferred in the V1 record. The entry in the "Parameters" column is
       used for the sequence. If you receive data in the inch format, it must be defined in the
       "Inch" column whether the parameter is transferred in inches and then may be converted
       to the metric system.




A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                 146
    7. Depending on the configuration, with #452522 (AWE 6 - Status as of end of October
       2019), it is no longer required that a template is assigned in the item master.
    8. The template name is sent in the field SN Name in the M1 record (configuration).
    9. Depending on the configuration, with #452522 (AWE 6 - Status as of end of October
       2019), it is no longer required that with the use of a template, a shape number > 0 must
       absolutely be used. If all dimension parameters in the M1 record are empty or equal to 0
       and only the field SN Name is assigned, it is possible that the field Shape number is empty
       or equal to 0.

        Depending on the configuration, the template name is specified via the "SN Name" field
        of the M1 record. This also absolutely conditions the use of a shape number > 0. The use
        of a shape number > 0 has appropriate effects on the price calculation and production
        flows in the further process. Therefore, this restriction has also been removed. If in the
        M1 record the field "SN-Name" is assigned, but all dimension parameters are empty or
        equal to 0, it is also possible to send the shape number field empty or equal to 0. If an
        empty shape number field is sent, in the further process flow, a shape number = 0 is used.
        Even if a shape is used in the template, in this case the order item would retain the shape
        number=0. There is no check and no shape synchronization between the template file and
        the item information.

    10. The parameter for the template is sent in V1. Here, the sequence of the parameters sent
        must absolutely be synchronized with the master data definition (point 6).



        15.11.3.        Exchange/addition rules for spacer exchange
#380927 With spacer exchange, the exchanged spacer is always put in with Anzahl1=1 and
Anzahl2 = 0. Now there can be branch offices where for various reasons it is necessary that the
spacer is put in with Anzahl1=2 and Anzahl2 =2.
To achieve this, the system can be configured (environment variable DFUE_FRAME_KUAZ) so that
the population of the quantity it not sent via the interface alone, but can also be populated from
the master data. With appropriate configuration, the Anzahl1 is assigned the quantity from the S1
record. Then there is a check if Anzahl1=0, then use Anzahl1 from the E/A rules and if Anzahl2=0,
then use Anzahl2 from the E/A rules.


#422717 For the external standard interface (i000filter), the print code for inside spacers was
always set to 1. The code was therefore always active. The flag was thus always active.
Now a possibility is offered with the environment variable "DFUE_FRAME_KUAZ" to use the print
flag (kuaz.druckkz) from the exchange/addition rules.
If the environment variable "DFUE_FRAME_KUAZ" is now set to ON, the value maintained in the
"Print" column in the dialog exchange/additional rules (Master Data > Market Partner >[F4] >
Exchange/Additional Rules) is evaluated.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                               147
        15.11.4.         Invoice address
Normally, the invoice address/customer address is taken over from the market partner master
data. With appropriate configuration (environment variable: DFUE_ORGFELDER), the address data
is included via the interface.
alcib - QR 04/2022
If, however, the environment variable VK_STEDEB_ADRESSE is active, the address is always used
from the master data of the FinAc debtor.
Please see the custom interface description.


        15.11.5.         Restriction violations
August 2021
For orders that are scheduled via external EDI, the processing parameters are checked
according to stored restrictions. Each item is checked up to the first restriction violation. If
there is at least one violation, the order will not be released.
If the dimension restrictions are violated for an EDI order, then this information is stored
in the order as a note. This way, the user knows the reason for the lock. Analogously, it is
now possible to configure that the violation of the restrictions is taken over as a note in
the order for the processing parameters. Since the check here only applies up to the first
violation per item, only this violation is documented in the notes.

INTAUF_INFO_DFUE_BARBRESTRIKT = ON
INTAUF_CHECK_DFUE_RESTRIKT = ON



        15.11.6.         Post-processing
With the environment variables EDI_SQL and IB_DFUE_NACHBEARB, you can change orders
between the trm_ctrl and the intauf individually. Attention must be paid here that at this point,
not all data for an order is available. Thus, at this point there is no BOM, for example. Similarly,
the value of kauf.eingang is still 0 (zero) and not 4.


        15.11.7.         Release
trm_ctrl - 13.04.6902 (Jan 2022)
If orders are scheduled via the external order interface, then you can control with the
environment variable INTAUF_FREITEK whether they should be released immediately or first put
into the release pool. Here, no differentiation between individual customers is possible.
Within the EDI post-processing (environment variable EDI_SQL or IB_DFUE_NACHBEARB), this can
only be done customer-specifically. If within the post-processing you set the field kauf.tekapkt to -
99, the order will be placed in the release pool subsequently. Attention must be paid that you
only set the field kauf.tekapkz=-00 if it is 0 or 66. If the field already has another value, then there
are already other reasons why an order should not be released (e.g. dummy article, discount, test
order).


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                   148
[AW-156214] alcib - 13.04.14857 ( April/2023)
EDI orders remain in the release pool of the call center
Due to the new configuration DFUE_CALLCENTER_STAY and within the configuration of the
document transfer (System - Data Transfer - Document Transfer - Configuration) (id = 65)
for customers, it can be specified that all orders that are scheduled via external or internal
EDI in the CALLCENTER site, the automatic site assignment is ignored (id = 65). The
orders are placed in the call center's release pool.

See also "EN-CONFIG-A+W Enterprise EDI" section "Release pool"


        15.11.8.        Packing type
Whether the packaging type can be provided via the external interface depends on the interface.
Within the default interface, the transfer of the packaging type is only possible customer-
specifically. See "EN-A+W EDI Import"
INTAUF_DFUE_VERPACKART (client reference: no)
If this variable is active, then during external order scheduling, the packaging type is filled via
interface.


NEW_PACKING_LOGIC (client reference: no)
Activates the logic of inheritance of the packaging type:
ON or 1: Customer-specific setting: The packaging type is always inherited from the header in the
positions.
Furthermore, the packaging type for order generation in the production site, PO generation in
trade and external order scheduling will NOT be re-populated, even if the abovementioned
variables are set.
2: If the packaging type is changed in the header, there is a query as to whether this change is also
inherited by the positions. In addition, with appropriate configuration (see above), the packaging
type is determined anew from the master data and transferred via external order interfaces.


        15.11.9.        Dimensional precision
Whether the dimension transferred is taken over in mm or more precisely can be configured via
environment variables (DFUE_NTEL_MM, IMP_CTRL_NTEL_MM, …). In addition, it depends on the
interface used. For more precise details, see the interface documents for the interface in
question.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                               149
    15.12. Error handling
        15.12.1.          Missing item dimensions
2021-07-07 [AW-77997]
Missing item dimensions for documents that were created by external EDI can cause significant
disturbances in the further process. Therefore, when scheduling external documents, a plausibility
check was built in. This plausibility check checks whether, depending on the quantity unit, the
required item dimensions (width, height) are present. If the dimensions are not present, the
scheduling of the document is interrupted with an error.
Via the control table exbartyp, default dimensions can be defined for this case, so that the
scheduling does not cancel, but the order is scheduled and can then be reworked manually. (artyp
18 and 19)



        15.12.2.          File is not imported - no error message
It happens every now and then that files are not imported and no error message is issued. In this
case, the interface log must be checked. Frequently the import breaks off at an umlaut or there is
a shifting of the field contents.
Example:
The files have the incorrect encoding for umlauts. Due to the "ä" in the article description, the
items are shifted. And therefore, a size variant = 0 is detected.
Example default interface (item shift):
                 p1_PRODNR=3U0724C4C4000
                  p1_PRODBEZ1=Heat protection 4/12/4/12/4 Ug = 0
                  p1_PRODBEZ2= .7
                  p1_PRODBEZ3=
                  p1_FARBE=
                  p1_KURZBEZ=
                  p1_KUPOS= 1
                  p1_MENGE=10 p1_BREITE=790        p1_HOEHE=890
                  p1_STKPREIS=0 p1_STRUK_VERLAUF=0 p1_STRUK_SEITE=0
                  p1_KOMM= 1216460/M+K STEINACH
                  p1_GES_EINBAU_STAERKE=0 p1_KANTSCHUTZ=0 p1_FALZMASSABZG=0
                  p1_KZ_GESPERRT=0      p1_KOSTENLOS=0 p1_EINF_RUECKSCHN=0
                  p1_BESCH_SEITE=0           p1_MASS_VARIANTE=<0                          >
                  p1_BESCHAFFUNGSART=0 p1_PREISRELEVANZ_KZ=0 p1_PREIS_TYP=0

Example of customer-specific interface (log breaks off the import at the umlaut)
The name of the customer includes an "ü"

07.04 15:12:15: first line to convert:->'K13059538 Metallbau Thomas Gr'
07.04 15:12:15: Function crawl_K1() starts
07.04 15:12:15: Header K1 read: record type:<K1>
              customer no: <3059538 >
              name 1 : <Metallbau Thomas Gr> name 2: <>
              street : <> ort : <>


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                               150
              country: <>
              attn : <> depart: <>
07.04 15:12:15: nach look ahead: 1 -1


The cause in both cases is that the file has the incorrect file encoding. Which end coding is
supported depends on the special interface and version.
For the default interface, in the latest version (April 2022)
         "No encoding is entered in the FH record; as a result it should be ASCII."
         From the interface docu about the FH record: field can be filled with the coding file. If the
         field is empty, the old processing will be used. Only AWE accepted entries: ISO8859-1,
         ISO8859-2, ISO8859-15, UTF-8, 819, 1250, 1252, 57372.
In which encoding the file is present can be determined with the command on the Unix shell.
file <File>


         15.12.3.        Missing orders from a file with several orders
For various reasons, within the external EDI, a maximum of 20 orders can be processed in a run
(job from ialf_jobctrl). If then additional orders must be processed within the same job, the EDI
independently inserts a restart after $DFUEDIR/wait. If, however, the dfue_starter is not running,
this restart is not executed.
The situation can be determined from the log entry in exbin*.
exbin log:
…
05.10 11:22:32: --- process loop ends ---
05.10 11:22:32: Stop process (Max. loop 20 reached)
05.10 11:22:32: try to restart trm_ctrl <sunet suhup exec /usr1/alcibnet/bin/trm_ctrl_l 20 1 20 0
<site> <site> 0> returns 0
05.10 11:22:32: <T> start: <exbin cleanup jobctrl>: Act. level 1
05.10 11:22:32: 0 records deleted from ialf_jobctrl (rc = 0)
05.10 11:22:32: <T> commit: <exbin cleanup jobctrl>: Act. level 0
05.10 11:22:32: *** Finish exbin() with code 0 ***

dfue_starter log
$DFUEDIR/proto/start_proto<site>
…
0410110344 <host>:suhup exec /usr1/alcibnet/bin/trm_ctrl_<site> 20 1 20 0 <site> <site> 0
0410151019 <host>:suhup exec /usr1/alcibnet/bin/trm_ctrl_<site> 10 1 8 0 0 0 0
0410151038 <host>:suhup exec /usr1/alcibnet/bin/trm_ctrl_<site> 10 1 8 0 0 0 0
Cancellation due to logfile not present on Mon Oct 4 15:11:45 CEST 2021
DFUE starter with PID = 57213256 no longer running
DFUE starter for <site> started on Tue Oct 5 15:00:08 CEST 2021



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                               151
Write process number 55640386 in /alcibdat/<site>/ipc/starter.log
0510150008 <host>:suhup exec cd /usr1/alcibnet
0510150009 <host>:suhup exec /usr1/alcibnet/bin/trm_ctrl_<site> 20 1 20 0 <site> <site> 0
0510150011 <host>:suhup exec /usr1/alcibnet/bin/trm_ctrl_<site> 20 1 20 0 <site> <site> 0




    15.13. Test function external standard interface
      (under construction)
The external order interfaces run completely automatically in the background. The result depends
heavily on the developments during the order entry in the foreground and the interface
development. In addition, there are effects of master data definitions and system configurations.
It is nearly impossible to keep an eye on these relationships at all times and from everywhere.
Thus, in the past, there were situations in which external orders were saved incorrectly due to
updates, master data changes, and configuration changes. These errors are frequently only
discovered at the construction site. Therefore, a tool was developed with which you can save a
defined record of interface files and can compare the results with the previously created
reference orders. This tool can be used within development, QA, and also at the customer's.
Orders from interface files that are called with these changed call parameters are not released in
principle and receive as initial comment the text "Test order". They can, if you wish, be released
manually. Currently there is no process for suppressing the release or producing these test orders
on the program-side.
Note: This function is a module that should be used by IT technicians or developers. It is not
intended as a tool for end users.


        15.13.1.        Configuration
To use the test tool, some configurations must be made.
Prerequisite is the presence of the current environment with the tables edicheck* and the
current program version of the trm_ctrl and the standard interface (i000filter). (QR November
2020 (Step 1 Count), October 2021 (field comparison), QR March 2024 (final))
This program is not backward-compatible. If you use the binary version from October 2021, the
environment also has to be correct.
Furthermore, for all tables to be checked the primary keys in the table documentation (table
alfield) have to be maintained correctly.
Currently only the standard interface is supported. If other order interfaces should be supported,
this has to be developed separately.
    a) A separate start script analogous to the existing start script has to be created in that the
       interface or the trm_ctrl is called with the new call parameters (see Process). The
       standard order interface has the call type 5 for this and the trm_ctrl the dfuetyp 25. If you
       are working with the variables DFUE_FILTERSTART, this call has to be adjusted for the new
       call type.



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                              152
    b) In the vorgangs_sql, a section has to be added that makes an update of the status in the
       table edichecktransfer with intauf -7 or -10.

        if [ $5 -eq -7 ]
        then
             echo "Set status for EDI test orders to 30 (intauf -7)" >>/tmp/vorsql.out
             isql $DBNAME - << %EOF
                  update edichecktransfer set status = 30, inserttime=current [, comment=’Processed by intauf’ ]
        where auftrnr = $1 and vorgang = $3 and status = 20;
        %EOF
        fi


Reference processes
For the flow of the test, reference procedures have to be defined in advance. These are
procedures that were stored correctly via external interface. Within the tests, these procedures
are tested later on. The reference procedures are entered under System – Data Transfer –
Interface Test - Reference Procedure.
Since the test orders are not released, the reference orders should also be scheduled with the test
option and not released. Otherwise, there can be differences in synchronization if you check not
released against released orders.




EDI – this is the definition of the interface with which the procedure was stored. Currently only 19
- A+W standard interface (i000filter) is supported.
Procedure – what is the procedure type (order, quotation) of the procedure. Currently, only
orders and quotations are supported. (kauf.vorgang)
Number – the external procedure number of the reference procedure (kauf.auftrnr)
File name – name of the interface file with which the reference procedure was generated and that
is read in again during the test. The specification is made without directory.
Seqnr – Sequence number of the order within the file if several orders are generated within a file.
Site – client number for which the document was generated
Comment – free comment field, e.g. for describing briefly what is special about this procedure.
The data is saved in the table EDICHECKREFERENCE.
Checking the number of records
For the flow of the test, test criteria have to be defined in advance. The first test criterion is the
number of data records per table. This can be, e.g. - number of items in the order or number of
BOM elements per item. This would be a first rough plausibility check. These test criteria are
entered under System – Data Transfer – Interface Test – Count-Tables. Here the table that should
be checked is specified and the keys relevant for the count (e.g. kpos - aufnr; aufstrukt - aufnr,
poskonr) are entered. The specification of the keys are not the primary keys of the table.


A+W Software GmbH                       EN-CONFIG-A+W Enterprise EDI.docx                                          153
Not all key combinations are supported. Currently supported are:
Key field 1: auftrnr, aufnr, txtnr
Key field 2: posnr, poskonr
The data is saved in the table EDICHECKCOUNT.
CAUTION: heed Special features for tables


Checking the data in the data records
After the first check "Checking the number of records" has run successfully, there is a check of
individual data. It is not possible or necessary to check all data for each customer. The data to be
checked has to be defined in advance. The test criteria are entered under System – Data Transfer
– Interface Test – Check Data.
The tables and table fields to be checked are entered on this dialog. For this, the sequence
number per field is required. This number has to be unique per table. The level controls the
processing and the test codes. Currently, the following levels are supported:
Header: e.g. table kauf
Item: e.g. table kpos
BOM: e.g. tables aufstrukt, poszu.
For the setting of the level, there is no plausibility check. Here, the user must know what he is
setting, otherwise the check will fail (e.g., if you would set the level "BOM" for the table kauf).


Prerequisite: for all tables to be checked, the primary keys in the table documentation (table
alfield) have to be maintained correctly.
CAUTION: heed Special features for tables




Special features for tables
Table ksprpar: Here it must be noted that this table currently is not available for checking the data
since this table has no unique key with fields that refer to themselves in kauf, kpos or auftstrukt.




A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                154
Table poskost: here you must heed that the number of data records also depends on production.
In particular, if one of the two orders was not transferred to production for cost calculation, there
will be data differences here.


        15.13.2.          Process
In principle, the flow is analogous to the normal order scheduling. In order to mark the schedule
as test schedule, new call parameters have been deployed.
For the external order interface, there is a new call type 5. Its effect is that, in addition to the
normal scheduling, the table _ialf_edichecktransfer is filled.
Call: "i000filter 5 <File>"
Then the trm_ctrl also has to be called with a new dfuetyp 25 (instead of 20)
Call "trm_ctrl 20 1 25 0 <site> <site> 0"
The trm_ctrl transfer the order as usual to the order background processing 'intauf'. After the
order has been processed by intauf, the status is set to 30. For this, an adjustment of the
vorgangs_sql is necessary (see "Configuration" section)
After the run-through, the table edichecktransfer is filled.
auftrnr          external order number (reference to kauf.auftrnr)
aufnr            internal order number (reference to kpos.aufnr and kauf.aufnr)
vorgang          5 – order (reference to kauf.vorgang)
filename         file name that was read in (without path specification)
sequence         the how-many order from <filename>
status -         INTERFACE_CREATED          10 /* interface has written the order */
                 ORDER_CREATED              20 /* if order complete through exbin */
                 ORDER_READY                30 /* if order complete through intauf */
comment          Kommentar �
inserttime       when was the record written/changed

If you now want to check the orders that are in edichecktransfer with status 30, the new program
"edicheck <hausnr>" has to be called. Currently, there is no automated or menu-assisted call for
this.
The program reads in all orders with status 30 and checks them against the corresponding order
in edicheckreference. The link is made via the fields "filename, sequence, vorgang and hausnr."
If the check was successful, the status is set to 40 in edichecktransfer with the comment =
"Successful count check . In case of an error, the status is set to 50 with the comment = "Error during
count check." or "Error NO reference order found."

If the first check with regard to "Count" was successful, the check of the specified Data is
conducted. If the check was successful, the status is set to 40 in edichecktransfer with the
comment = "Successful field check". In case of an error, the status is set to 50 with the comment
"Error during field check." or "Error NO reference order found."
For more details about what went wrong with a check, see the log.




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                  155
          15.13.3.        Log
Depending on the configuration of the EDI, the log is written to
$DFUEDIR/proto/edicheck_proto<site>_<mmddhhmm>_<pid>
or
$DFUEDIR/proto/<site>/edicheck/edicheck_proto<site>_<mmddhhmm>_<pid>
. A standard or extended version of the log can be written. To activate the extended logging, the
environment variable DFUE_RESEARCH has to contain the value "edicheck".


      15.14. Environment variables
DFUE_JOBCTRL (data transfer)
With an activated variable, the parallel execution of several filters is possible. (prerequisite is the
adapted program logic, see also the overview table "Requirements")
DFUE_ERROR_SUBPATH (client reference: no)
In this variable, a subdirectory can be specified into which the incorrectly processed file should be
moved. The path specification is relative to the initial directory. If the subdirectory is parallel to
the initial directory, then it must be specified with " " (e.g. ../error). Currently the variable is only
evaluated by the default filter DFUE_JOBCTRL must be activated for correct functioning..
see also DFUE_SUCCESS_SUBPATH
DFUE_FILL_ERRITAB (data transfer, only iskafilter)
With these variables, the filling of the erri tables is activated in the iskafilter. With switched-on
variables, particular errors that have previously caused the cancellation of the scheduling, are
caught specially. The relevant data record is saved in the error tables (same structure as _ialf
tables). The scheduling of the file is continued. The variable is only evaluated if the env variable
DFUE_JOBCTRL is active.
DFUE_OPT_POSKONR (client reference: no)
This variable controls the number of BOM headers for orders that are scheduled via external EDI.
If the variable is set to 1, then the following is checked between 2 items
     AIR/AIR2,2 spacer, spacer color,2 Georgian bars, Georgian bar color, item color
If the variable is set to 2, then the stamp is also checked.
If the variable is set to 2, then the spacer is also checked.
DFUE_SACHBEARB_MAIL (client reference: no)
  If this environment variable is enabled, the system message 51 sent from the EDI is also sent to
the employee.
DFUE_SUCCESS_SUBPATH (client reference: no)
In these variables, a subdirectory can be specified into which the successfully processed file
should be moved. The path specification is relative to the initial directory. If the subdirectory is
parallel to the initial directory, then it must be specified with " " (e.g. ../archive). Currently the
variable is only evaluated by the default filter DFUE_JOBCTRL must be activated for correct
functioning..


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                    156
see also DFUE_ERROR_SUBPATH
DFUE_TRM_SIMULTAN (data transfer)
Simultaneous trm_ctrl for external order scheduling and PO generation.
DFUEDIR
DFUE_JOBCTRL
DFUE_OHNE_ARTKUZU (client reference: No)
Within the external EDI, for each customer who sends orders via external EDI a conversion of the
customer item number into an AWE item number is stored (artkuzu/kuaz). If the customer already
makes a conversion and sends A+W Enterprise item numbers, then setting this environment
variable means that there does not have to be a repeated assignment in A+W Enterprise. This
means that if the conversion is stored in A+W Enterprise, it is used. If no conversion is stored, the
number sent is used as A+W Enterprise number.
The environment variable can be set individually in the calling script. Here it must be noted that
for parallel configuration or for DFUE_JOBCTRL, trm_ctrl-calls from other scripts can also process
the orders. DFUE_OHNE_ARTKUZU is evaluated both in i000filter as well as in exbin().
Is evaluated for
    -   Item article
    -   Spacer replacement
    -   Gas replacement
    -   Georgian bar replacement
    -   Stamp
    -   Spacer and other articles


INTAUF_CHECK_DFUE_RESTRIKT (client reference: no)
If the variable is active, EDI orders with restriction violation are not released and are in the release
pool with the corresponding comment.
INTAUF_INFO_DFUE_BARBRESTRIKT (client reference: no)
With external EDI, the violation of the restrictions is written for the processing parameters as note
in the order. The 1st violation per item is always documented.


MODUL_SN_TEMPLATE (client reference: no)
(AWDesk #160653): storage of template parameters via the V1 record of the standard interface.
With active variable, the parameter string transferred in the V1 record is interpreted as a
succession of numeric values of the format 7.1. The values read out are saved as parameter 1 to
73 in the table kpostemplate.
SN_CADFILES_DIR (client reference: no)
If this variable is active, then the *.sn files are divided across several directories
($SNFILES_DIR/YMM/DD*.sn).



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                157
Caution: in the iTOE, the variable is not evaluated. SN files generated by the iTOE call are written
to the $SNFILES_DIR/TOE/YYY/MM/DD directory by default.
SNFILES_DIR (client reference: order)
The variable must absolutely be configured if you are working with SN files. It contains the path to
the SN files. SN, CAD Service and AWP must also have access to the stored directory. In the
configuration of the AWP there is a corresponding variable in which the identical file path must be
stored. Depending on the configuration of the AWP, these are different variables. (case:
#398256)




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                               158
16. PO export / A+W EDI export
The PO export is the writing of the PO information in the A+W standard format. See also "EN-A+W
EDI Import.pdf."
The flow of the PO export can be configured within A+W Enterprise.
Currently, the interface version 02.2.032 is released. An adjustment to newer interface versions
will not be made immediately. If a customer requires a more current interface version, it has to be
requested explicitly from Development.
Which data records are currently supported is documented in the interface documentation "EN-
A+W EDI Import".
To be added is that the A+W Enterprise export can currently export more information than the
A+W Enterprise import can import. This especially affects the complexity of deep BOMs for
multiple glass and pure muntin POs (in the frame or muntin patterns)
If a file written by the A+W Enterprise export should be imported into A+W Enterprise, the
specific requirements and master data circumstances have to be checked in detail in advance.
There are different requirements for the import in A+W Business than for the import in A+W
Enterprise.
See PF [AW-199351] + [AW-169965].




    16.1. Activation
There is a price list module for the EDI export.
The logic is activated via the module variable MODUL_EDIEXPORT.
If the variable is active, the EDI "EK Export" can be configured for suppliers. The activation of the
variable may not be done by the customer independently; it must be done by the responsible
planner. Simply activating the variable is not sufficient for being able to put the EDI export into
operation. Additional configuration steps are required.




    16.2. Installation
        16.2.1.         A+W Enterprise B2B Service
The export files are generated by the A+W Enterprise B2B service, which has to be installed for
this in the currently released Version 6 from SW_Install. In addition, in the A+W Enterprise B2B
Service, the generation of the export files has to be activated. The installation and basic
configuration of the B2B Service is described in the installation document "A+W Enterprise B2B
Service."
For explanation of the general functioning of the B2B service, please see the configuration
document "A+W Enterprise B2B Service."



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                159
        16.2.2.         AWE back end and database
Table aldfuectrl
The table aldfuectrl must be up-to-date. Entries up to ID 68 must be present.


fx_texte/messages
fx_texte/messages must be up-to-date.




    16.3. Configuration
        16.3.1.         Market partner master data
The use of the PO export must be defined within the supplier master data. For this, for the
supplier on the tab "Delivery," the "Type of EDI" must be set to "PU export." Furthermore, you
can define on this field with F5 or in "System - Data - Transfer - Document Transfer -
Configuration" whether an export file should also be written directly during the automatic PO
generation. For this, for the supplier (or supplier 0), an entry for the EDI type 116 "PO export" and
the control type 47 "Direct PO export" must be created. The checkmark must be placed in the
Value field.


        16.3.2.         External customer number
In addition, for the supplier in the "External customer number" field (mp.extkundnr), you must
enter which customer number the orderer has for this supplier. This customer number is then
transferred in the K1 record in field 4 "Customer number".
Caution:
Since the customer number is specified in the K1 record as a numeric data field, only numeric
customer numbers can be transferred.
If the external customer number in the AWE master data includes alphanumeric characters and
therefore cannot be converted into a number, no value is determined and a "0" is transferred in
the K1 record.
In the log of the B2B service, you will find the corresponding error message.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                160
        16.3.3.    Configuration of settings across suppliers and
            supplier-specific export settings
The definition of the individual settings is made under
System > Data Transfer > Transfer Document > Configuration
Or in the market partner master data via the "EDI configuration" menu or F5 on the field "Type of
EDI."
The settings can either be stored supplier-specifically or across suppliers. The supplier-specific
setting always takes priority over the cross-supplier setting.
With "Type of EDI" = 116 "PO export", currently the following settings are possible:


Control Name                                     Description
type
47         Direct PO export                      Is set at the distributor.
                                                 Optional
                                                 If a PO for a supplier is created automatically, it is
                                                 provided immediately after completion by the intauf
                                                 for the creation of an export file (entry in the table
                                                 ottransfer).
                                                 If such a PO is changed, it is not provided again for the
                                                 export. The provision must be done manually.
                                                 For manually entered POs, no export file is created
                                                 automatically. The provision must be done manually.
                                                 ID 422752
49         Interface Version                     Is set at the distributor.
                                                 Optional
                                                 This is the A+W EDI interface version that should be
                                                 generated.
                                                 Only selected interface versions are supported.
                                                 Currently only Version 02.2.032

                                                 Default: 02.2.032
50         File extension                        Is set at the distributor.
                                                 Optional
                                                 File extension
                                                 Default: "out"
51         Inches as fractions                   Is set at the distributor.
                                                 Optional
                                                 Default: 1 (corresponds to "metric")
                                                 Other values > 0 (z.B. 16, 32, 64) are interpreted as
                                                 inch fractions.


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  161
52      File name                        Is set at the distributor.
                                         Optional
                                         Description, see chapter „Generation of the export
                                         file“.
53      File encoding                    Is set at the distributor.
                                         Optional
                                         Supported entries: ISO8859-1, ISO8859-2, ISO8859-15,
                                         UTF-8, 819, 1250, 1252, 57372

                                         Default: "UTF-8"
54      Basic path                       Is set at the distributor.
                                         Optional
                                         Description, see chapter „Generation of the export
                                         filei“.
55      Basic path file                  Is set at the distributor.
                                         Optional
                                         Description, see chapter „Generation of the export
                                         filei“.
56      Basic path back-up file          Is set at the distributor.
                                         Optional
                                         Description, see chapter „Generation of the export
                                         filei“.
57      Basic path old file              Is set at the distributor.
                                         Optional
                                         Description, see chapter „Generation of the export
                                         file“.
58      Subdirectory                     Is set at the distributor.
                                         Optional
                                         Description, see chapter „Generation of the export
                                         file“.
59      Subdirectory file                Is set at the distributor.
                                         Optional
                                         Description, see chapter „Generation of the export
                                         file“.
60      Subdirectory back-up file        Is set at the distributor.
                                         Optional
                                         Description, see chapter „Generation of the export
                                         file“.




A+W Software GmbH             EN-CONFIG-A+W Enterprise EDI.docx                         162
61         Subdirectory old file                 Is set at the distributor.
                                                 Optional
                                                 Description, see chapter „Generation of the export
                                                 file“.
62         Always send e-mail                    Is set at the distributor.
                                                 Optional
                                                 Flag: always send an info e-mail after PO export. (in
                                                 case of error, an info e-mail will be sent regardless of
                                                 the setting.)
                                                 Default: 0 (= do not send an e-mail in case of success)
                                                 E-mail address is stored in the B2B service.
                                                 Description, see chapter „Sending e-mail“.
66         Export to A+W Business                Is set at the distributor.
                                                 Optional
                                                 The checkbox is activated for A+W Business trade
                                                 partners; that is, if the recipient of the PO export
                                                 imports the exported file into A+W Business.
                                                 [AW-169965]
67         Sending company number                Is set at the distributor.
                                                 Obligatory if "Export to A+W Busiiness" is active.
                                                 Is only evaluated if "Export to A+W Business" is active
                                                 (supplier configuration ID 66).
                                                 The company number is stored here, which is
                                                 specified for the file sender in A+W Business of the file
                                                 recipient in the master data.
                                                 [AW-169965]
68         Receiving company number              Is set at the distributor.
                                                 Obligatory if "Export to A+W Busiiness" is active.
                                                 Is only evaluated if "Export to A+W Business" is active
                                                 (supplier configuration ID 66).
                                                 The A+W Business company number of the file
                                                 recipient is stored here.
                                                 [AW-169965]




        16.3.4.         Stored Procedures
For the determination of special field content, the use of stored procedures is provided in the
interface. Thus, the field content can be placed customer-specifically and flexibly. If the stored


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  163
processes named are not present, the fields remain empty or are filled with default values
according to interface descripotion "EN-A+W EDI Import" section "A+W Enterprise Export-specific
field notes".
If a SP is present, it is also executed. No special activation is required.
Caution: The stored procedures are not included in the installation scope of delivery.
The naming conventions of the stored procedures are
Cu – Customer – may be adjusted by the customer
Edi- External Data interface
<field> – for which field the SP is called
Xx – record type (fh, k1)
The following stored procedures have currently been implemented. The stored procedures are
not included in the installation scope of delivery.
Record     Field                               Stored Procedure
type
FH         7 – User-defined field              cu_edi_cust_record_fh (key_auftrnr INT,
                                               key_vorgang SMALLINT , key_subnr SMALLINT,
                                               key_still SMALLINT)
                                               RETURNING CHAR(100);
K1         16 – User-defined field             cu_edi_cust_record_k1 (key_auftrnr INT,
                                               key_vorgang SMALLINT , key_subnr SMALLINT,
                                               key_still SMALLINT)
                                               RETURNING CHAR(100);
P1         2 - Product number                  cu_edi_prodnr_record_p1 (key_auftrnr INT,
                                               key_vorgang SMALLINT , key_aufnr INT, key_posnr
                                               SMALLINT)
                                               RETURNING CHAR(64);
P2         17 – User-defined field             cu_edi_cust_record_p2 (key_auftrnr INT,
                                               key_vorgang SMALLINT , key_aufnr INT, key_posnr
                                               SMALLINT)
                                               RETURNING CHAR(100);
BC         2 – Barcode                         cu_edi_barcode_record_bc (key_auftrnr INT,
                                               key_vorgang SMALLINT , key_aufnr INT, key_posnr
                                               SMALLINT)
                                               RETURNING CHAR(500);
S1         6 – product number (except          cu_edi_prodnr_record_s1 (key_auftrnr INT,
           for shape)                          key_vorgang SMALLINT , key_aufnr INT, key_posnr
                                               SMALLINT, key_poskonr SMALLINT, key_tnr
                                               SMALLINT)
                                               RETURNING CHAR(64);
S1         6 – product number for              cu_edi_shape_record_s1((key_auftrnr INT,


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                            164
          shapes                            key_vorgang SMALLINT , key_aufnr INT, key_posnr
                                            SMALLINT, key_poskonr SMALLINT, key_modnr
                                            SMALLINT)
                                            RETURNING CHAR(64);
S1        21 – User-defined field           cu_edi_cust_record_s1 (key_auftrnr INT,
                                            key_vorgang SMALLINT , key_aufnr INT, key_posnr
                                            SMALLINT, key_poskonr SMALLINT, key_tnr
                                            SMALLINT)
                                            RETURNING CHAR(100);
T1        There is a peculiarity here       cu_edi_txt_art_t1(key_auftrnr INT, key_vorgang
                                            SMALLINT , key_aufnr INT , key_posnr SMALLINT,
          Here, the SP defines whether
                                            key_artnr INTEGER)
          a whole sentence is written.
          One SP per text type is called:   RETURNING SMALLINT, CHAR(480), CHAR(1);
               -   Supplementary            cu_edi_txt_artobjekt_t1(key_auftrnr INT,
                   Article Texts            key_vorgang SMALLINT , key_aufnr INT , key_posnr
                                            SMALLINT, key_artnr INTEGER, key_objnr INTEGER)
               -   Object Article Texts
                                            RETURNING SMALLINT, CHAR(480), CHAR(1);
               -   Supplier Article Texts
                                            cu_edi_txt_artlief_t1(key_auftrnr INT, key_vorgang
          The SPs deliver the type          SMALLINT , key_aufnr INT , key_posnr SMALLINT,
          (=print item) and the text, as    key_artnr INTEGER, key_mpnr INTEGER)
          well as the text flag.
                                            RETURNING SMALLINT, CHAR(480), CHAR(1);
          Type ( 1=before item, 2=after
          item, 3=product)



T2        There is a peculiarity here       cu_edi_txt_lief_t2(key_auftrnr INT, key_vorgang
          Here, the SP defines whether      SMALLINT , key_subnr SMALLINT, key_still
          a whole sentence is written.      SMALLINT, key_mpnr INTEGER)
          One SP per text type is called:
                                            RETURNING SMALLINT, CHAR(480), CHAR(1);
               -   Supplier texts
          1 - Header texts
          2 – Footer texts

          The SP delivers the type
          (=print item) and the text, as
          well as the text flag.


        16.3.5.         Country code
For export to A+W Business (supplier configuration ID 66), for the correct transfer of the country
identifier, the ISO code of the country must be maintained in the address records (table
xxland.iso).



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                            165
    16.4. Overview of flow
        16.4.1.          Initiation through entry in the table ottransfer
In A+W Enterprise, the PO export/EDI export is initiated by an entry in the table ottransfer. The
ottransfer record is then processed asynchronously by the B2B Service.
There is no initiation of the generation of EDI export files for several POs.
The EDI export can basically be triggered with PO generation or printing of the PO. Decisive here is
the configuration of the env variable BESTELLFREIGABE.
If for a supplier "Direct PO export" is configured (tax type 47), then a record is written to
ottransfer by the intauf directly during the PO generation. If a PO is changed manually after the
fact, there is no additional automatic triggering of the export. If another export is required, it
must be initiated manually.
If the EDI export should be done while printing, a suitable report must be created, which then
writes the appropriate export record to the ottransfer table. The standard report poexport.rep
with form type 127 can be used.
A triggering of the export with PO release is not implemented as of today (05/12/2020).


Local correction
The generation of the EDI export file has no influence on the local correction status of the PO.
When a PO goes into local correction is decided independently of the EDI export functionality.


        16.4.2.          Processing by the B2B Service
The B2B Service polls the transfer table ottransfer at a configurable interval. One export file is
generated per EDI export record (PO). If there is an error during processing, the ottransfer record
remains in the table ottransfer with error status (ottransfer.steuerflag). With successful
processing, an export file is generated and the record processed is removed from the table
ottransfer.


    16.5. Transfer table ottransfer
The B2B Service obtains its work orders from the table ottransfer. This table is a universal transfer
table that is queried both by the OrderXML Service as well as by the B2B Service. The general
transfer type is detected from the entry in the field ottransfer.schnittstelle. EDI export records
contain the entry "EDIEXP" here.
During processing by the B2B Service, the service update the time stamp (ottransfer.uzeit) and
processing status (ottransfer.steuerflag) in the current ottransfer record.
If an export file was generated, the file name including file path is added in the field
ottransfer.filename.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 166
        16.5.1.         Back-up table ottransferok
The table ottransferok has the same structure as the table ottransfer. In it, the successfully
processed EDI export records are backed up and kept for a time.
The records in ottransferok are cleaned up with a clean-up logic. That is, the time period can be
stored in the config tool of the B2B Service for which the records in ottransferok should remain.
(for configuration see installation instructions for the B2B service.) Older records will be deleted.


    16.6. Imperial measurements
If imperial measurements should be written to the export file for a supplier, the corresponding
configuration is required. The switch with ID 51 supplier-specific has to be configured in System-
>Data Transfer->Document Transfer->Configuration (see "Configuration " chapter).




    16.7. Export to A+W Business
During export to A+W Business, there are a few particularities to be noted. Whether an export is
to A+W Business is set in the supplier configuration with the ID 66.


        16.7.1.  Configuration of the sending market partner in
            A+W Business
Complete BOM
In the AWB market partner master data, it is possible to configure whether the sending customer
must always store a complete BOM in the file.
If "complete BOM" is not active, it is sufficient to send only the exchange/additional articles in the
file. Unsent BOM elements cause gaps in the numbering (AWE tuple numbers) of the elements
sent. These gaps are explicitly necessarily.




    16.8. Data Mapping
See EN-A+W EDI Import – section "A+W Enterprise Export-specific field notes".




    16.9. Generation of the export file
The export file is written with a configurable file name to a configurable directory.
The configuration possibilities are varied and can be specified supplier-specifically. However, no
special configuration is required. There is a default logic according to which the file path and
name are generated.



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 167
With repeated EDI export for one and the same PO, an already existing export file is marked as
"old" and shifted to an appropriate folder /old.


CAUTION: The following logic (writing marked in RED) is currently NOT implemented.
After FTP transfer of an export file, the file is shifted to a back-up folder.



        16.9.1.          Basic configuration
The only necessary setting is made in the config tool of the B2B Service (see installation
instructions "A+W Enterprise B2B Service"). There, the basic path of the A+W EDI export is
specified. Path and name of the export file are determined according to the following scheme:
<Basic path>\<company number>\<supplier no.>\AWE_P<PO
number>_YYYYMMDD_HHmmss.out
"AWE" and "P" are fixed components of the file name. "AWE" is the prefix. The "P" stands for
"purchase" and indicates the next PO number.
Example:
Export basic path: C:\awediexport
Site number: 10
Supplier number: 112233
PO number: 777888
Time stamp of the generation: 01.05.2020 13:41:57
=> Complete file name: C:\awediexport\10\112233\AWE_P777888_20200501_134157.out


The path and name of the old file for repeated EDI export for one and the same file is:
<Basic path>\<Company number>\<Supplier no.>\old\old_<Original file name>.out
For the example described above, there arises the following complete old file name:
C:\awediexport\10\112233\old\old_AWE_P777888_20200501_134157.out


CAUTION: The following logic (writing marked in RED) is currently NOT implemented.
The path and name of the back-up file after FTP transfer is:
<Basic path>\<Company number>\<Supplier no.>\save\<Original file name>.out
For the example described above, there arises the following complete back-up file name:
C:\awediexport\10\112233\save\AWE_P777888_20200501_134157.out



        16.9.1.          Overwriting of the basic configuration
The overwriting of the basic configuration can be done across supplier or supplier-specifically
with:


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                             168
System > Data Transfer > Transfer Document > Configuration
Or in the market partner master data via the "EDI configuration" menu or F5 on the field "Type of
EDI."
Here it should be noted that if a component of the directory structure is overridden, the other
components also have to be defined. For example, this means that if the general subdirectory (ID
58) is overridden, then the directory for the old files (ID 61) and the save files (ID 60) also has to
be defined since otherwise the files remain in the normal subdirectory and are not moved.
Configuration of the file extension
The file extension is configured via the switch with ID 50.


Configuration of the basic path
The basic path is configured via the switch with ID 54. If there is no additional overwriting, the
configured basic path is used (combined with any configured subdirectory) for the files generated,
for the old files, and for the back-up files.
It can be overridden for the generated files by the ID 55 "Configuration of the basic path", old files
by ID 57 "Configuration of the old file basic path" and the back-up files by ID 56 "Configuration of
the back-up file basic path".
Configuration of the subdirectory
The subdirectory is configured via the switch with ID 58. If there is no additional overwriting, the
configured subdirectory is used in combination with the basic path for the files generated, for the
old files, and for the back-up files.
It can be overridden for the generated files by the ID 59 "Configuration of the basic path", old files
by ID 61 "Configuration of the old file basic path" and the back-up files by ID 60 "Configuration of
the back-up file basic path".
Configuration of the file basic path
The basic path is configured via the switch with ID 55. It is used (combined with any configured
subdirectory) for the files generated. It overrides for the files the ID 54 "Configuration of the basic
path".
Configuration of the old file basic path
The old file basic path is configured via the switch with ID 57. It is used (combined with any
configured subdirectory) for the old files. It overrides for the files the ID 54 "Configuration of the
basic path".
Configuration of the back-up file basic path
CAUTION: The following logic (writing marked in RED) is currently NOT implemented.
The back-up file basic path is configured via the switch with ID 56. It is used (combined with any
configured subdirectory) for the back-up files. It overrides for the files the ID 54 "Configuration of
the basic path".
Configuration of the file subdirectory
The file subdirectory is configured via the switch with ID 59. It is used in combination with the
basic path for the files generated. It overrides for the files the ID 58 "Configuration of the
subdirectory".


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 169
Configuration of the old file subdirectory
The old file subdirectory is configured via the switch with ID 61. It is used in combination with the
basic path for the old files. It overrides for the files the ID 58 "Configuration of the subdirectory".
Configuration of the back-up file subdirectory
CAUTION: The following logic (writing marked in RED) is currently NOT implemented.
The back-up file subdirectory is configured via the switch with ID 60. It is used in combination with
the basic path for the back-up files. It overrides for the files the ID 58 "Configuration of the
subdirectory".
Configuration of the file name
The file name is configured via the switch with ID 52. It is used as name for the files generated,
the old files, and the back-up files. The file name has to contain the PO number of the exported
PO and a time stamp (see placeholders/wildcards in file names). If the PO number or time stamp
are not included in the file name via a placeholder, they are added automatically during
generation of the file name.
Automatically added components of the file name are distinguished from other file names with an
underscore ("_").
The PO number is always added at the beginning of the file name. The PO number is preceded
with a "P" (= "purchase") for identification.
The time stamp is always added at the end of the file name. The time stamp used always has the
format "YYYYMMDD_HHmmss."


         16.9.2.         Placeholders (wildcards) in the file paths
There are 2 defined placeholders that can be used in the file paths:
$SITE$          The placeholder “$SITE$” is replaced in the file path by the site number (company
                number) of the current PO.
$SUPPLIER$      The placeholder “ $SUPPLIER$” is replaced in the file path by the supplier number
                of the current PO.



         16.9.3.         Placeholders (wildcards) in file names
There are 4 defined placeholders that can be used in file names:
$SITE$                   The placeholder “$SITE$” is replaced in the file name by the site number
                         (company number) of the current PO.
$SUPPLIER$               The placeholder “ $SUPPLIER$” is replaced in the file name by the supplier
                         number of the current PO.
$PO_NUMBER$              The placeholder "$PO_NUMBER$" is replaced in the file name by the PO
                         number of the current PO.
$DATE_TIME$              The placeholder "$DATE_TIME$" is replaced in the file name by the
                         current time stamp (format "YYYYMMDD_HHmmss").




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 170
        16.9.4.          Housekeeping
Currently, there are no clean-up routines for the directories used. That's why the customer is
responsible for cleaning up the directories.


    16.10. Special explanations for the export logic in
      the AWE B2B service
        16.10.1.         Language
Currently there is no localization for the supplier language. All names are currently exported in
the system language of A+W Enterprise.


        16.10.2.         Product Types and Product Groups
For the record type S1 (BOM record), the fields "Produktart" and "Produktgruppe" are filled. The
meaning of the fields is described in the documentation for the A+W EDI Import.
A hard-coded logic in the B2B service determines in the standard logic product type and group a
BOM article using its article type (artikel.atyp).
In AWE, the configurable fields "PRODUKTART" and "PRODUKTGRUPPE" are also available for
articles. If for an article in the configurable fields an article type > 0 and/or an article group > 0 is
stored, the standard logic is taken out of force and the values from the configurable fields are
taken over.


        16.10.3.         Export of articles
    •   Glass
        For multiple glasses (IG, LAMI), the FD glass of the first BOM level is always exported.

        Lites below TG or float are not exported.
        Processings below TG are not exported.

        Stock dimensions are not exported.

        For a LAMI BOM with stock dimensions (LM), the LM is not exported and all BOM
        elements below the LM are ignored. Lites below a LM are never exported.
        For export to AWB, LAMI BOMs are handled separately, the 2 LAMI fixed dimensions (FM)
        include under another (processed and un processed LAMI-FM). IN this case, only the
        superior LAMI-FM (processed LAMI-FM) in the BOM is exported. The subordinate LAMI-
        FM            (unprocessed       LAMI-FM)           is         not          exported.
        All BOM elements under the unprocessed LAMI-FM are evaluated according to the
        general logic.

    •   Foils
        Foils are only exported if the PC flag is set.

A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                   171
    •   Frame/spacer
        Frames are always exported

    •   Muntins
        Muntins are always exported.

    •   Gas
        Gas is always exported.

    •   Accessory
        Accessory is only exported with set EA flag.

    •   Processings
        Processings are only exported if the EA flag is set.
        Processings below TG are not exported.

    •   Metaparts
        If there is a metapart in the BOM, then this is skipped and the BOM below it is evaluated
        analogous to the criteria described.




        16.10.4.        Export of shapes
If an item in the A+W Enterprise was entered as a shape, then by default, an M1 records is always
written. This is sufficient for an import into A+W Enterprise. If, however, the export file is
imported into A+W Business, then for shapes, an S1 record with a corresponding shape article
number is required. Writing the S1 record for shapes (product type 12/product group 5) is only
done if the SP cu_edi_shape_record_s1() exists and does not return an empty string.
The shape S1 record is always written as last S1 record.


        16.10.5.        Export of muntins
Muntins are exported independently of the E/A flag. Muntins always have to hang on muntin
patterns. The muntin pattern can be ordered as an item or below the frame. The scheduling of
muntins without glass is currently not possible in A+W Enterprise.


        16.10.6.        Export of steps
In order to order stepped glass, 2 data records are required. On the one hand, a S1 record that
contains the stepped article and the M1 record that includes the step difference dimensions. For
the export of steps from AWE, both an S1 record as well as an individual M1 records are written
for each stepped glass. This has to do with the internal data structure of A+W Enterprise. Here,
the step difference dimensions are saved separately for each glass. In addition, the structure of
the interface is identical if the glass is stepped differently (step in LAMI).
During the export of steps, it has to be heeded that the import of steps in A+W Enterprise is
restricted. The import of step levels is not possible.



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                             172
        16.10.7.         Export of gas
Gas is exported independently of the E/A flag. If gas is created as metapart, the metapart is not
exported, but rather the article of the type gas (260) within the BOM of the metapart. Depending
on the positioning of the gas article (next to or in the frame), the level field is filled in the
interface. If the file written is read into A+W Enterprise, this has to be configured appropriately
(for details, see environment variable DFUE_GAS_LEVEL in the documentation "DE-A+W EDI
Import.pfd").


        16.10.8.         Export of processings (B1 record)
Only A+W standard processings (artikel.awtyp > 0) are exported.

Processings are only exported if the EA flag is set. Here, there will be no configuration in the first
step.

The specific field notes for the B1 record with regard to the individual processing types are
described in the A+W EDI Import document.
If there is a metapart in the BOM, then this is skipped and the BOM below it is evaluated
analogous to the criteria described.
Which A+W processing types are currently supported is described in the A+W EDI Import
document.


        16.10.9.         Export of item texts (T1 - record)
Item-related texts are in A+W Enterprise
        - Item texts
        - Article texts
        - Supplementary article texts (SP)
        - Project article texts (SP)
        - Supplier article texts (SP)
        -
By default, only manual item texts and manual article texts are exported. The item and article
texts generated are not exported.
The extended article texts can be exported via the call of special Stored Procedures.


        16.10.10. Export of attached files (DL and PL record)
Attached files are always exported. If an attached file cannot be copied because it is not present
or the file or directory rights are not present, the export interrupts the writing of the export file.
A DL record is written if a file was attached to the PO on the order header level (kaufref.posnr=0).
A PL record is written if several files were attached to the PO on the item level (kaufref.posnr!=0).
The file to be exported is copied to the same directory as the export file. Here,
vorgang,auftrnr,posnr are added to the file name. The changed file name is written to the export
file.


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 173
    16.1. Sending e-mails
The B2B Service always sends an info mail if an error occurs during PO export.
Recipient of the e-mail is the person who entered the PO. In addition, in the config tool of the B2B
Service, additional recipients can be entered for the info mail (see also the installation instructions
"A+W Enterprise B2B Service").
Optionally, an info mail can also be sent if a PO export was executed successfully. For this, the
switch with ID 62 cross-supplier or supplier-specific has be configured in System->Data Transfer-
>Document Transfer->Configuration (see "Configuration" chapter).


    16.1. Logging and research
The B2B Service writes a log (trc file) into the log directory %programdata%\A+W\Log.
For researching for PO export in AWE (up to the entry in the table ottransfer), a ftest must be
activated.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                174
17. Order import (intauf)
    17.1. Introduction

    17.2. General procedure

    17.3. Functional range
        17.3.1.         Logic for distribution of the order imports
The goal of the logic is at a company that as many orders are imported via external interfaces or
as many orders are transmitted to associated sites in order to achieve a load distribution across
different intauf processes.
For the use of this logic, the following environment variables are required:
Old version: IB_INTAUFNO, INTAUF_GRENZ1 - 4
New version: INTAUF_DFUE, INTAUF_GRENZ1 – 4, INTAUF_DFUEGRENZ1 – 4
Additional explanations under the individual environment variables for 16.4.


    17.4. Environment variables
IB_INTAUFNO
For the old distribution logic (IB_INTAUFNO), two values are stored in the variables IB_INTAUFNO
separated by a pipe.The first value specifies which intauf should process the external order
import.The second value specifies which intauf should execute the import of transferred orders.
According to these two values, the trm_ctrl uses the *GRENZ* variables to specify the value for
the field posanz in the table aufint and executes a sctrl call for the correct intauf.
IB_INTAUFNO                                   aufint.posanz                    sctrl
1st value – external, 2nd value -
internal
1                                             INTAUFGRENZ1-1                   I0B
2                                             INTAUFGRENZ1+1                   I1B
3                                             INTAUF_GRENZ2+1                  I2B
4                                             INTAUF_GRENZ3+1                  I3B
5                                             INTAUF_GRENZ4+1                  I5B


INTAUF_GRENZ1 - 4




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                               175
With the old distribution logic (via IB_INTAUFNO), the INTAUF_GRENZ* variables are evaluated
for the external import and for the order transfer.
The *GRENZ* variables specify the number of items up to which a particular intauf is responsible
for the processing of the import.
INTAUF_DFUE
The env variable INTAUF_DFUE activates the new distribution logic (developed for NSG) and
overrides the variable IB_INTAUFNO, which previously activated an older, more limited
distribution logic.
INTAUF_DFUEGRENZ1 - 4
With the new distribution logic (via INTAUF_DFUE), both INTAUF_DFUEGRENZ* variables as well
as the INTAUF_GRENZ* variables are evaluated.
The INTAUF_DFUEGRENZ* variables are evaluated for external order import and order
transfer.The INTAUF_GRENZ* variables are evaluated for PO generation.
The *GRENZ* variables specify the number of items up to which a particular intauf is responsible
for the processing of the import.
With the new distribution logic (INTAUF_DFUE), the intaufs 6 to 10 (A) are used for the external
order import and order transfer; for PO generations, the intaufs 0 to 3 and 5.
Depending on how many *GRENZ* variables are assigned values, the field posanz in the table
aufint is also assigned according to the *GRENZ* variables and the corresponding intauf started.
The distribution does not take place according to the real number of items, but rather "evenly"
across all intaufs.
                                       aufint.posanz                          sctrl
External order import                  INTAUF_DFUEGRENZ1-1                    I6B
                                       INTAUF_DFUEGRENZ1+1                    I7B
Order transfer
                                       INTAUF_DFUEGRENZ2+1                    I8B
                                       INTAUF_DFUEGRENZ3+1                    I9B
                                       INTAUF_DFUEGRENZ4+1                    IAB
Order generation                       INTAUFGRENZ1-1                         I0B
                                       INTAUFGRENZ1+1                         I1B
                                       INTAUF_GRENZ2+1                        I2B
                                       INTAUF_GRENZ3+1                        I3B
                                       INTAUF_GRENZ4+1                        I5B




A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                 176
18. Master data replication
The master data replication in A+W Enterprise is divided into
    •   Article replication
    •   Market partner replication
    •   Key replication
    •   Product set transfer
In addition to this master data replication developed within A+W Enterprise, the INFORMIX
Enterprise replication is available for the replication of data and the use of database synonyms.


    18.1. Checklist
BYTE_VEKTOR                                       The replication may only be done between
                                                  databases that are set identically with
                                                  regard to the environment variable
                                                  BYTE_VEKTOR. If this is temporarily! not
                                                  possible (e.g. during a conversion phase),
                                                  then it must! All tables with byte vector
                                                  fields (e.g. the table “artxtzu” (variable
                                                  RP_ARTXTZU = ON)) are excluded from the
                                                  replication.
Xhaus                                             Master/client setting
Database configuration                            The participating databases require direct
                                                  contact.
Internal site separation                          Start only on main site; master is external site
Trigger and SPs on main table                     Depending on replication
Master data maintenance                           In the article or market partner master data, it
                                                  must be maintained which data records
                                                  should be replicated in which subsidiary
Environment variables for tables to be
replicated
Language                                          If language-dependent data should be
                                                  replicated, the language keys must be
                                                  identical (Master Data - Keys - System Keys -
                                                  Languages) and alsysinfo.landesspr must be
                                                  maintained correctly.
Local fields                                      Which fields should be defined as local in the
                                                  subsidiaries?




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                  177
    18.2. Basic principles for all replications
A client can only have one master, the master - client relationship is a 1:n relationship. Who is the
master for a client is in the table xhaus and per client database (important for internal client
separation), there can only be one master.
In order to be able to set up the A+W Enterprise master data replication between two
databases, it is necessary that these databases can communicate with one another via
SQL. For this, it is necessary that:
        a) If the databases are on different computers, these computers are known to
           one another.
        b) The   $INFORMIXSERVER                has      to      be      entered       in     the
           $INFORMIXDIR/etc/sqlhosts
        c) The port of the service (/etc/services) that is entered for the other
           INFORMIXSERVER in the sqlhosts has to be accessible.
        d) The nettype of the INFORMIXSERVER that wants to establish the
           connection has to be *tcp (not *shm)
            e.g.
            Entry in sqlhosts:
            awentwdb2_alcib_tcp         ontlitcp      awentwdb2                   sqlexec

            Entry in services:
            sqlexec      1525/tcp

            test:
            $> telnet awentwdb2 1535
            Trying 194.39.65.64...
            Connected to awentwdb2.
            Escape character is '^]'.
            Connection closed by foreign host.

      To be noted is also that a replication between a database that is on BYTE_VEKTOR
      and a database that does not have this setting is not possible or will result in data
      errors. An exception from this can only occur in the special case that no tables with
      BYTE_VEKTOR fields are replicated (see AWD #84596).
      Other restrictions are that DB_LOCALE, DBLANG, DBMONEY and DBDATE are
      identical between the master database and the client database.
      Starting with Version 2009 (4.4), it is possible to replicate between databases with
      different DB_LOCALE. For this, the variable RP_DB_LOCALE_MASTER on the client
      has to be activated and contain as value the DB_LOCALE of the master. (#180439)
      Another basic prerequisite is that the database structure in the master be
      identical to or more up-to-date than the database structure in the client.

A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                 178
    18.3. Special feature of internal site separation
If the internal site separation "MODUL_INTERNE_MANDANTENTRENNUNG" is configured, the
replication can only be started on a main client (xhaus.haus = xhaus.hauptmandant).
Furthermore, the associated master client can only be an external client (xhaus.hauptmandant =
0).


    18.4. Configuration
      Replication in ALCIB currently supports table names and field names up to 18
      characters. Replication cannot handle long table and field names (from
      INFORMIXVERSION 9.x) at present.

        18.4.1.         Table xhaus
      Which database is the master database is defined in the table xhaus. For this, in the
      data record for the master, the field "dbart" has to be set to 1. If you are working
      with a 2- or multi-stage replication (central master and country master), then the
      settings are as follows.
      In the end client:
      Data record for the client: dbart = 0
      Data record for the master: dbart =1

      In the country master:
      Data record for the country master: dbart = 2
      Data record for the central master: dbart = 1

      In the central master:
      Data record for the central master: dbart = 1
      All other data records have to be set to dbart=0.
      As another field for the article replication, the field “informixserver” has to be
      maintained appropriately for the own and master in the table xhaus
      ($INFORMIXSERVER).


    18.5. Logs
        18.5.1.         Log database table
Starting in August 2019 (replicate build 13.04.3175)




A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                           179
     A database logic has been added to the replication logging so that important
     information is stored in the new tables DFUE_PROTOKOPF and
     DFUE_PROTODETAIL.
     This logic is currently supported by key replication, article replication, and market
     partner replication.
     The information from the database is additionally reported to a registered
     employee as a result by e-mail at the end of the respective replication. The set-up of
     this system message must be set to message group 4 (EDI) and the respective
     message number.
Message         Description
number
22              Article transfer failed

85              Article transfer successful
78              Market partner transfer failed

86              Market partner transfer successful
81              Key transfer failed

87              Key transfer successful

New system e-mail values (table ALSYSAB):

MELDID                  GROUP                        ERRNO
85                      4                            37713             Article transfer
                                                                       successful
86                      4                            37714             Market partner
                                                                       transfer successful
87                      4                            37715             Key transfer successful


     In parallel, the log files are still written.

         18.5.2.       Article replication
     The log $PROTOPFAD/ArtReplik<mmdd> writes the article replication. The logging is
     done in English. The logging level can be switched with the environment variable
     DFUE_RESEARCH=art_replicate to an expanded mode, a so-called developer mode.
     The log is written buffered by default. If the expanded log is switched on, then it is
     written unbuffered. If you would like the default protocol to be written unbuffered
     as well, then the environment variable DFUE_PROTO_NOBUFF has to be set.
     Build alcib - 13.04.14359 (2023-01-20)
     If DFUE_RESEARCH=art_replicate is active, a ftest log will also be written since there
     are functions in the replication that are also used in the front end.


A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                           180
       In addition, a new environment variable RP_ARTTEST was created. With these
       environment variables, currently an expended logging for the table "artbezfremd" is
       switched on. Since this logging is associated with additional data procurement, it
       should only be activated if there are actually problems in this environment. The
       scope of the variables can be expanded if needed.



        18.5.3.           Key replication
       The key replication writes a log to $PROTPFAD/<site>/ Key_replic _mmdd_hhss.
       (old) If the environment variable REPLICATE_PROTO is set, an expanded logging can
       be switched on.
       (new) If the environment variable DFUE_RESEARCH="key_replicate" is set, an
       expanded logging can be switched on.

        18.5.4.           Market partner replication
       If DFUE_RESEARCH=mp_replicate is active, a ftest log will also be written since
       there are functions in the replication that are also used in the front end.
       Starting with build: alcib - 13.04.18318



    18.6. Market partner replication
The configuration of the market partner replication is currently described in a separate document.
And it will be transferred to this document by and by.
\\jupiter\Doku_DocuWare\ALCIB-PMS\DFUE\Replikation\Marktpartnerreplikation_DE.doc



        18.6.1.           Table xhaus
The table "xhaus" is a central table for all replications. It will therefore be described at the
beginning of the chapter.


        18.6.2.           Tables, triggers, and stored procedures
For the market partner replication, in the master on the table "mp", one trigger apiece
must be created for the actions insert, update, and delete. These triggers, in turn, call a
stored procedure that makes the corresponding entries in the table rp_mp.
For the market partner replication, there must be a table rp_mp with the following
structure
Mpnr            integer          Market partner number mp.mpnr

A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                               181
Kuliflag      smallint        Market partner type mp.kuliflag
Site          smallint        Target site xhaus.hnr
Upinsdel      smallint        Type of change: 0=delete, 1=insert, 2=update
Ackflag       smallint        Processing status: 0 – unprocessed, 1 – in process or error
Usr           char(8)         Employee who made the last change (loginname)
mod_time    datetime year to minute     Time of the last change

. This is the table that contains all market partners that should currently be replicated. It
is filled via trigger with each change of a market partner.

Example for trigger and SP:
      create table rp_mp (
         mpnr integer,
         kuliflag smallint,
         haus smallint,
         upinsdel smallint,
         ackflag smallint,
         usr char(8),
         mod_time datetime year to minute
       );

      create index ix_rp_mp1 on rp_mp (mpnr, haus,ackflag) ;
      create index ix_rp_mp2 on rp_mp (haus);

      create procedure cu_mprepl(pkey char(20), pkuliflag smallint, pupinsdel smallint)
        define xh,hh smallint;
        set isolation to dirty read;
        if pkuliflag=0 then
               foreach select hausnr into hh from limits where kunr=pkey and hausnr in
                            (select haus from xhaus where dbart != 1)
                         let xh=(select distinct haus from rp_mp
                          where mpnr=pkey and kuliflag=0 and haus=hh);
                         if xh is null then
                                   insert into rp_mp
                                   (mpnr,kuliflag,haus,upinsdel,ackflag,usr,mod_time)
                                   values (pkey,0,hh,2,0,user,current);
                         else
                                   update rp_mp set
                                   mod_time=current, usr=user
                                   where mpnr=pkey and kuliflag=0 and haus=hh;
                         end if;
                 end foreach;
          else
          if pkuliflag>0 then
               foreach select hausnr into hh from limits where kunr = pkey and hausnr in
                           (select haus from xhaus where dbart != 1)
                         let xh=(select distinct haus from rp_mp
                                   where mpnr=pkey and kuliflag=pkuliflag and upinsdel=pupinsdel
                                     and haus=hh);


A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                             182
                       if xh is null then
                                 insert into rp_mp
                                 (mpnr,kuliflag,haus,upinsdel,ackflag,usr,mod_time)
                                 values (pkey,pkuliflag,hh,pupinsdel,0,user,current);
                       else
                                 update rp_mp set mod_time=current, usr=user
                                 where mpnr=pkey and kuliflag=pkuliflag and
                               haus=hh and upinsdel=pupinsdel;
                       end if;
              end foreach;
        end if;
      end if;
      end procedure;

      create trigger mp_u update on mp referencing
              new as post
              for each row
              (execute procedure cu_mprepl(post.mpnr ,post.kuliflag,2 ));

      create trigger mp_i insert on mp referencing
              new as post
              for each row
                ( execute procedure cu_mprepl(post.mpnr ,post.kuliflag,1 ));

      create trigger mp_d delete on mp referencing
              old as pre
              for each row
              (execute procedure cu_mprepl(pre.mpnr ,pre.kuliflag ,0 ));



        18.6.3.        Configurable fields
When configurable partner fields are replicated (table mpcomfld) with negative field numbers,
the client will keep the field numbers.
This replication logic requires in versions 2009 and 2011 the setting of environment variable
MPCOMFLD_WITH_SELO. If MPCOMFLD_WITH_SELO is set for the client, this logic must be
enabled in the master too; replication will be aborted otherwise when it comes to replicating the
configurable fields.



        18.6.4.        Plausibility check
For the subsequent plausibility check, all market partners are checked, not just those that were
just replicated.
    a) Invoice address: it is checked whether for all market partners the invoice address
       (mp.rechadrnr) is also present in the table adr. In the process, closed market partners and
       closed addresses are also checked.



A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                 183
    b) Default delivery address: it is checked whether for all market partners the default delivery
       address (mp.stdadrnr) is also present in the table adr. In the process, closed market
       partners and closed addresses are also checked.
Closed addresses are replicated.




    18.7. Article replication
        18.7.1.          Table xhaus
The table "xhaus" is a central table for all replications. It will therefore be described at the
beginning of the chapter.


        18.7.2.          Trigger – Stored Procedure – Tables
Which articles must be transferred in which clients is defined within the Item master data (see
below). If an article defined as to be transferred is changed in the article master data, then there
are 2 possibilities for whether this article is actually entered in the table rp_artike and thus
transferred.
      Triggers for the table "artikel"
      For this path, the articles are generally entered after each change for the transfer
      into the table "rp_artikel". There is no query. This ensures that all changes are
      always entered in the connected clients in timely fashion.
      For the article replication, in the master on the table "artikel", one trigger apiece
      must be created for the actions insert, update, and delete. These triggers, in turn,
      call a stored procedure that makes the corresponding entries in the table rp_artikel.
      Example for trigger and SP:
      create table rp_artikel (
         artnr integer,
         haus smallint,
         ackflag smallint,
         usr char(8),
         mod_time datetime year to minute
       );

      create index ix_rp_artikel1 on rp_artikel (artnr, haus,ackflag) ;
      create index ix_rp_artikel2 on rp_artikel (haus);

      create procedure cu_artikelrepl(pkey char(20))
        define xh,hh smallint;
        set isolation to dirty read;
        foreach select hnr into hh from artrepsteuer where artnr=pkey and

A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                               184
          hnr in (select haus from xhaus where dbart != 1)
          let xh=(select distinct haus from rp_artikel where artnr=pkey
               and haus=hh);
          if xh is null then
             insert into rp_artikel (artnr, haus, ackflag, usr, mod_time)
             values (pkey, hh, 0, user, current);
          else
             update rp_artikel set ackflag=0, usr=user, mod_time=current
             where artnr=pkey and haus=hh;
          end if;
      end foreach;
    end procedure;

    create trigger artikel_u update on artikel referencing
      new as post
      for each row
        ( execute procedure cu_artikelrepl(post.artnr ));

    create trigger artikel_i insert on artikel referencing
      new as post
      for each row
        ( execute procedure cu_artikelrepl(post.artnr ));

    create trigger artikel_d delete on artikel referencing
      old as pre
      for each row
        ( execute procedure cu_artikelrepl(pre.artnr ));

    Triggers for the table "artisnu"
    (04.01.2022: This variant is currently in use at customer 24)
    For this path, the user can decide whether an article is entered directly after its
    change for the transfer into the table "rp_artikel". An appropriate query can be
    configured via the environment variable "ARTIKELUEBERTRAGUNG". If the
    environment variable with the value 1 is active, then after each saving of the article,
    an entry is made in the table "artisnu". If the variable is active with the value 2, then
    when saving an article, the query is made whether the article should be transferred
    to the connected client. Only if the question is answered with "Yes" is the entry
    made in the table "artisnu".
    The query and the entry in the table "artisnu" are made regardless of whether the
    article includes an entry in the replication data.
    If you would like to use this possibility, then an insert trigger must be created on the
    table "artisnu" that then calls a SP that makes the appropriate entry in the table
    rp_artikel. The insert trigger for the table artikel and the associated SP can serve as
    template.


A+W Software GmbH              EN-CONFIG-A+W Enterprise EDI.docx                          185
    The triggers on the table "artikel" may then no write an entry to rp_artikel.
    Similarly, the cleansing of the table "artisnu" must be done independently since the
    article replication no longer uses this table. It is a component of the old, file-based
    article transfer. This cleaning can be done, for example, with a delete trigger on the
    table "rp_artikel".
    create trigger cu_rp_artikel_del delete on rp_artikel
      referencing old as old
      for each row
        ( execute procedure cu_trd_rp_artikel(old.artnr ,old.haus ));


    SP „cu_trd_rp_artikel“
    CREATE PROCEDURE cu_trd_rp_artikel(p_artnr INTEGER , p_haus INTEGER )
    DEFINE v_new_chk INTEGER ;
    DEFINE v_chk        INTEGER ;


    SELECT COUNT(*)           INTO   v_chk
    FROM rp_artikel
    WHERE artnr = p_artnr ;


    IF v_chk IS NULL OR v_chk = 0
     THEN
             DELETE FROM artisnu
             WHERE artnrf = p_artnr
              AND artnrt = p_artnr ;
    END IF


    SELECT COUNT(*)           INTO   v_chk
    FROM rp_artikel ;


    IF v_chk IS NULL OR v_chk = 0
     THEN
             DELETE FROM artisnu ;
    END IF
    END PROCEDURE;




A+W Software GmbH               EN-CONFIG-A+W Enterprise EDI.docx                        186
         18.7.3.            Tables to be transferred
 For each table of the article master data there is an environment variable that controls whether
 or not the data from this table should be replicated. Here, precise attention must be paid whether
 the replication is done with active or inactive variable. The different evaluation is required for
 reasons of compatibility. If new tables are added, the ones in A+W may not simply be
 incorporated into the replication; instead, the customer must decide whether he needs this data.
 Starting with 2012.1: In addition, the replication checks whether the table to be replicated is a
 database synonym in the client (systable.tabtype='S'). If this is the case, then this is noted in the
 log and the table is not replicated. If the table "artikel" is recognized as synonym, then the
 complete article replication is canceled.
 Attention: If, for example, it is configured that formerly the table "nsteuer" is to be transferred,
 then the transfer does not take place if only one of the tables "artvermass", "artvermassspr",
 "artpreiseig" is a synonym. This constellation also affects the transfer of texts, private fields, fixed
 products, etc.
 Maximally, the following tables are replicated (status as of January 2011):


      Table                   Variable                           Replicate if      LOCAL/ADDLOCAL
1     Article
2     Artliefzu               RP_ARTLIEFZUART                    ON                Default: local records are
                                                                                   retained.
                                                                                   (artliefzu.orghaus=<client>)
3     Artkuzu                 RP_ARTKUZUART                      OFF               Default: local records are
                                                                                   retained.
                                                                                   (artliefzu.orghaus=<client>)
4     Artvarzu                RP_ARTVARZU                        OFF               Via extra variable
                                                                                   RP_SAVE_LOCAL_LINES
5     Artfarbzu               RP_ARTFARBZU                       OFF               Via extra variable
                                                                                   RP_SAVE_LOCAL_LINES
6     musskenn                RP_MUSSKENN                        OFF
                              RP_MUSSKENNATYP_TRANS ON
7     Strukt                  RP_STRUKT                          OFF               Yes/yes via environment
                                                                                   variable
8     Nsteuer                 RP_NSTEUER                         OFF
      from 2011 on:           RP_NSTEUERATYP_TRANS               ON
      artvermass,             RP_NSTEUERAWTYP                    OFF
      artvermassspr,
      artpreiseig
8.1   Artvermass.datei        RP_ARTIKEL_DATEI                   ON
      (the file specified


 A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                    187
     here, not the          (note also
     database               DATEI_REF_PFAD,
     content)               DFUE_DATEI_REF_PFAD)
9    modparam               RP_MODPARAM                         OFF
10   artbezfremd            RP_ARTBEZFREMD                      OFF
11   Artxtzu                RP_ARTXTZUART                       OFF
12   Arteinbau              RP_ARTEINBAU                        OFF
13   defformel              RP_DEFFORMEL                        OFF
14   Artkenn                Is currently not replicated
15   Artprvfld              RP_ARTPRVFLD                        OFF
16   Artmemo                RP_ARTMEMO                          OFF
17   Pstrukt                RP_PSTRUKT                          OFF
18   Pposzu                 Together with pstrukt
19   Pparam                 Together with pstrukt
20   pstufparam             Together with pstrukt
21   Psprpar                Together with pstrukt
22   Pspross                Together with pstrukt
23   pfremdposzu            Together with pstrukt
24   Artpiczu               RP_ARTPICZU                         OFF
25   Arttechw               RP_ARTTECHW                         OFF


        18.7.4.          Local tables
Various system settings allow to exclude individual tables from replication in the recipient's
(Client) database. Local data will not be overridden by headquarters in case of another
replication. (see Tables to be transferred – environment variables)
It might be better for certain tables to be dispatched by headquarters when a new article is
defined; amendments will not be applied to the client, however.
If in environment variables, the keyword "LOCAL" is entered for a table, this table will be
transferred when the article is transferred for the first time. If the article is changed, changes in
this table will not be transferred.
The site (client) - not the master - decides whether an article is new (does it already exist, or
not?).
In connection with the BOM, this means:
Variable RP_STRUKT="ON" is set.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                    188
             •   A new article is transferred by headquarters. The article now exists at
                 the site, but without a BOM.
             •   The site enters its own BOM.
             •   When this article is transferred again by headquarters, the BOM will not
                 be included. The locally defined BOM will be kept.
The variable RP_STRUKT="LOCAL" is set.
             •   A new article is transferred by headquarters. The article now exists at
                 the site, and has a BOM.
             •   The site changes and completes the BOM sent by headquarters.
             •   When this article is transferred again by headquarters, the BOM will not
                 be included. The locally defined (amended) BOM will be kept.
The variable RP_STRUKT="LOCAL" is set.
             •   A new article is transferred by headquarters. The article now exists at
                 the site, and has a BOM.
             •   At the site, this BOM dispatched by headquarters is NOT changed.
             •   When this article is transferred again by headquarters, the BOM will not
                 be included. The locally defined (unchanged) BOM will be kept.

        18.7.5.           Special features for tables
ARTVERMASS (SN macro)
ID 251282
If the article size is replicated, the information on the SN macro to be used is replicated as well.
This field cannot be defined as a local field in article replication. If the field for the SN macro file is
entered as a local field in the replication configuration, this entry will be ignored.
Apart from that, all SN files will be transferred with are listed in the article sizes of the articles to
be transferred. This transfer can be prevented by setting the environment variable
RP_ARTIKEL_DATEI.
For transferring the SN files, article replication requires ftp access to the directory defined in
environment variable DFUE_DATEI_REF_PFAD or DATEI_REF_PFAD.
If the directory defined in variable DATEI_REF_PFAD cannot be accessed by ftp, environment
variable DFUE_DATEI_REF_PFAD must be set which defines the directory which is entitled to ftp
access. The notation in this variable is:
<hostname>!<directory>
The "exclamation mark“ between the host name and the directory is mandatory!
Once the variable DFUE_DATEI_REF_PFAD is set, DATEI_REF_PFAD will not be analyzed any more
in article replication
ATTENTION: Replication reads the environment variable for the path details in master data
(reading of SN files) as well as on the –client (writing of SN files).

A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                    189
At the end of article master data replication there is a plausibility check for the article
dimensioning records by means of awtyp=1900 "macros“. The program checks if all files defined
in local master data also exist in the locally defined directory. Similarly, it is checked that all
entries have a file entry. This check cannot be switched off. If replication detects a master data
record on the client which contains a SN file that does not exist in the defined directory, system
message 22 "Local item master data" is dispatched. This email contains the article numbers for
which the defined SN file could not be found in the directory in question.


How does the replication of the processing types )tables artvermass, artvermasspr, artpreisig)
work starting with Version 2011 (case 174319)?
The replication of the processing types is controlled with the same environment variables as
previously (RP_NSTEUER, RP_NSTEUERATYP_TRANS, RP_NSTEUERAWTYP).
If within the article master data adjustments to the processing types for an article are made, the
replication is done via the article (trigger for filling the table rp_artikel). If changes are made to an
article type, the replication is initiated via the table rp_nsteuer; therefore, triggers must be
installed on the tables artvermass, artvermassspr, artpreiseig, which fill the table rp_nsteuer.


PSTRUKT
The replication of the table pstrukt requires in the versions 2.12 and 3.0 an extension of the
environment: The files rp_pstrukt.mfo and rp_pstrukt.pan must be placed in the appropriate
subdirectories of the article area. Then by setting the variables RP_PSTRUKT the replication of the
table is SWITCHED ON.
Starting with version 3.1, the replication of this table is included by default in the article
replication, so that starting with this version, the setting of the variables SWITCHES OFF the
replication of the table pstrukt. A manual environment change is then no longer necessary.
artcomfld / artprvfld (case 159503)
Both the key table artcomfld, in which all private article fields are defined, as well as the article
table artprvfld include, in addition to the key "fldnr" also the fields "fldpos, fldtyp, fldbez".
For the article replication, the table artcomfld is always transferred.
The records from the table artprfld are only transferred during replication if the program detects
that these are "new" records that were not yet created in the client.To detect an "old" record, the
fldnr/fldnrz is compared. If the fldnr is already known, fldpos and fldtyp of the current record are
retained in the client. Through this logic, there can be discrepancies in the article master data if in
the master the field sequence (fldpos) of the private fields is changed after the fact (after articles
have already been transferred with the old field sequence).
It is urgently recommended that you not change the field sequence after the fact!
Similarly, we would like to warn you urgently against creating local records with active replication
of the private fields in the client. Since in the client the fields are created without reference to the
field number of the master (fldnrz), as a result there can be "doubled" records.
As soon as an article with such inconsistent data is called in the article master data, the artprvfld
data is corrected automatically with the next saving.
Of course the correction then only affects selected articles.




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                  190
If you check the master data directly on the database tables, you will find the correct field
sequence for the private fields only via the fldnr (from artprvfld) through a select on the table
artcomfld.
In the private fields, starting with version 2009, it is possible to define selos. This makes a data
structure change necessary in the completed version. The function is only available in 200, 2011
and AWE 5 if ARTCOMFLD_WITH_SELO is set (a manual adjustment of the environment is
required). For the replications, this means if a client is working with the selos function and has set
this variable, the logic must also be configured on the master and the environment adjustment
must be undertaken!
Starting with version AWE 6, the variable is no longer required. In this version, the function is
standard.
For the replication, it must be heeded that only the database contents are replicated. The selo
files used are not transferred too.


musskenn/nsteuer records for article types
So far,article replication allowed to define whether the records for product-related dimensioning
and compulsory sizes should be replicated. This definition did not include the product-related
data. The system can be configured so that the article type records are also replicated in case of a
change.
CAUTION: While installing the additionally required database objects(triggers) in the tables
musskenn and nsteuer, no user must be active
To configure the replication for article types from 'nsteuer' and 'musskenn':
Required tables:

        a) rp_nsteuer for ‚nsteuer’ article types
           Attention: the field types atyp, awtyp, mtyp are new. Please check the current
           version.

            create table rp_nsteuer
             (
               atyp smallint,
               awtyp integer,
               mtyp smallint,
               haus smallint,
               upinsdel smallint,
               ackflag smallint,
               usr char(8),
               mod_time datetime year to minute
             );

      create index ix_rp_nsteuer on rp_nsteuer (haus);

      create procedure cu_rpnsteuer(patyp smallint, partnr integer, pawtyp integer)
              define xh,hh smallint;

              set isolation to dirty read;
              if partnr=0 then


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                191
                     foreach select distinct hnr into hh from artrepsteuer where
                             hnr in (select haus from xhaus where dbart=0)
                             let xh=(select distinct haus from rp_nsteuer where atyp=patyp
                     and
                              awtyp=pawtyp and haus=hh);
                             if xh is null then
                                       insert into rp_nsteuer (atyp, awtyp, haus,
                                                ackflag, usr, mod_time)
                                       values (patyp, pawtyp,hh, 0, user, current);
                             else
                                       update rp_nsteuer set ackflag=0,
                                                usr=user, mod_time=current
                                       where atyp=patyp and awtyp=pawtyp and haus=hh;
                             end if;
                     end foreach;
           end if;
    end procedure;

    Die Trigger werden neu auf artvermass generiert und nicht auf die View nsteuer

    create trigger artvermass_u update on artvermass
        referencing new as post
            for each row
               ( execute procedure cu_rpnsteuer (post.atyp ,post.artnr ,post.awtyp ));

         create trigger artvermass_i insert on artvermass
           referencing new as post
           for each row
             ( execute procedure cu_rpnsteuer (post.atyp ,post.artnr,post.awtyp ));

         create trigger artvermass_d delete on artvermass
           referencing old as pre
           for each row
             ( execute procedure cu_rpnsteuer (pre.atyp ,pre.artnr ,pre.awtyp ));


      b) rp_musskenn für ‚musskenn’ Artikeltypen

         create table rp_musskenn
          (
            atyp smallint,
            haus smallint,
            ackflag smallint,
            usr char(8),
            mod_time datetime year to minute
          );

    create index ix_rp_musskenn on rp_musskenn (haus,atyp);

    create procedure cu_rpmusskenn(patyp smallint, partnr integer)


A+W Software GmbH              EN-CONFIG-A+W Enterprise EDI.docx                             192
            define xh,hh smallint;
            set isolation to dirty read;

           if partnr==0 then
                     foreach select distinct hnr into hh from artrepsteuer where
                             hnr in (select haus from xhaus where dbart=0)
                             let xh=(select distinct haus from rp_musskenn
                                       where atyp=patyp and haus=hh);
                             if xh is null then
                                       insert into rp_musskenn (atyp, haus, ackflag, usr,
                                       mod_time)
                                                values (patyp, hh, 0, user, current);
                             else
                                       update rp_musskenn set
                                                ackflag=0, usr=user, mod_time=current
                                                where atyp=patyp and haus=hh;
                             end if;
                     end foreach;
             end if;
    end procedure;

         create trigger musskenn_u update on musskenn referencing
           new as post
           for each row
               (
               execute procedure cu_rpmusskenn (post.atyp ,post.artnr
           ));

         create trigger musskenn_i insert on musskenn referencing
           new as post
           for each row
               (
               execute procedure cu_rpmusskenn (post.atyp ,post.artnr
           ));

         create trigger musskenn_d delete on musskenn referencing
           old as pre
           for each row
               (
               execute procedure cu_rpmusskenn (pre.atyp ,pre.artnr
           ));

    Trigger and SP on tables 'nsteuer', 'artvermass' (new) and 'musskenn' to fill the tables
    'rp_nsteuer' and 'rp_musskenn'.
    CAUTION: While installing the additionally required database objects(triggers) in the tables
    'musskenn' and 'nsteuer', no user must be active




A+W Software GmbH               EN-CONFIG-A+W Enterprise EDI.docx                              193
         18.7.6.          Local fields
In addition, for each replicated table, it can be decided whether there are so-called "local" fields
within the table. A local field is defined by the fact that data that exists in the client is not
overwritten by data from the central office. For initial replication, a default value can be specified.
The local fields are defined in "System - Data Transfer - Local Fields" (table artiecs).
Database fields that are not integrated into screens are not accepted as local fields in the
replication logic (e.g. shmflag from table artikel). With specification of such a field in the local
fields, the replication fails.
with the new replication logic (RPTableMemrel_*-Funktionen) the problem that database fields
that are not integrated into screens may not be defined as local does NOT occur anymore. (See
also case 155676)
In addition, there are fields that are not accepted by the program as local fields. If these fields are
defined as local fields, the definition is ignored during replication and the field is nevertheless
replicated.
Starting with 2012.1 - artvermass.macroname -> appropriate comment in the log


         18.7.7.          Foreign-language subsidiaries
At larger companies, it is possible that individual subsidiaries work in different countries and thus
in different languages. Nevertheless, it should be possible to maintain central article master data.
In this case, in the central location, it is primarily the article descriptions in the language of the
central office that are maintained. After that, there are 2 paths for supplying foreign-language
subsidiaries with correct article master data.


         18.7.8.          Article description as local field
The first path would be to define the article descriptions at the foreign-language subsidiary as
local fields and to maintain the descriptions in the subsidiary.
Benefits
        The benefits of this path:
    •    The employee who maintains the master data in the central office does not need any
         knowledge of a foreign language
    •    Only a few employees must maintain master data in the central office
    •    Only the articles in the subsidiary must be maintained that are actually used.
Drawbacks
        The drawbacks of this path:
    •    If there are several subsidiaries with the same foreign language, there is twice the effort
         for data maintenance
    •    If foreign-language customers (with regard to the language of the subsidiary) are also
         served, the foreign-language data must also be maintained several times.
    •    Different translations in different subsidiaries.




A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                   194
Requirements
        In order to be able to change the article descriptions in the subsidiary, the article
        descriptions in the subsidiary must be defined as local fields (System - Data Transfer - Local
        Fields). Here, the use pf each field within the subsidiary/central office must be examined.
        The fields for the article descriptions are in the "article" table
    •    artbez1
    •    artbez2
    •    artbez3
    •    kurzbez

        and in the table artbezfremd
    •    langbez1
    •    langbez2
    •    langbez3



         18.7.9.    Replication                 of      the       foreign-language               article
             description
        The second path is the maintenance of all foreign-language descriptions in the central office
        and transfer to the subsidiaries.
Prerequisite
        So that language-specific article descriptions are transferred correctly, the descriptions in
        the article master data under "additional descriptions" for all relevant languages must be
        maintained appropriately (table artbezfremd).
        Furthermore, it is necessary that the language keys are maintained identically in all
        subsidiaries. That is, if in the central office French was set to the language key 2, this is also
        necessary in the subsidiary (key replication or synonym).
        In addition, in the ALCIB system table "alsysinfo", the field "landespr" must be filled with
        the correct value for the local language (from the own language key master data).
        Lastly, in the subsidiary, the environment variable
        ARTIDFUE_UPDATE_ARTBEZFREMD="ON" must be set so that the language-specific entries
        from the table artbezfremd are taken over into the article master data (table artikel).
        The table artbezfremd must be replicated.


Environment variables
ARTIDFUE_UPDATE_ARTBEZFREMD
After article transfer, the language-specific entries from the menu item "Further descriptions" are
transferred to the article master if the variable is active. Here the local language from alsysinfo is
evaluated.
RP_ARTBEZFREMD



A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                  195
This variable controls the replication of the data from table artbezfremd from the head office to
the corresponding site. If this variable is not set (default), the artbezfremd data will be transferred
at replication.



        18.7.10.        Plausibility check
At the end of the replication, it is checked in the client whether all dependencies defined in the
master data are also present. The lack of data is only sent as an e-mail warning (message 22) and
not treated as replication error.
This means that the problem is reported via mail insofar as the mail (number 22) is configured.
However, the replication takes place nevertheless. However, the article cannot be used correctly
in the client and the master data should be adjusted.
The following data is currently checked:
                  -   Exchange/addition formula in the article (artikel.azformel) - table formel
                  -   Formula in the BOM (strukt.erbkz) - table formel


        18.7.11.        Transaction logic
With the start of the replication on the client, each article to be transferred from the table
rp_artikel of the master is stored in a separate transaction.


        18.7.12.        Master data maintenance
Within the master data maintenance, it has to be defined for each article to be replicated
whether it has to be replicated in the clients. For this, in Master Data - Article the menu (F4) has
to be called up and the element "Article - Data synchronization" - "Replication data" selected.
On this dialog, the client sites have to be entered on which the article should be replicated. At the
same time, you can specify here which supply type, production duration, which supplier and
which delivery time the article should have in the client. However, the specification of this data
only makes sense if it is an article that does not have variants.


        18.7.13.        Environment variables
Caution: There are environment variables that switch the replication on and there are variables
that switch the replication off. Please heed the documentation of the variables precisely.
Furthermore, it must be noted that the environment variables are evaluated in the Client - NOT
in the master. If the evaluation takes place in the master, this is mentioned explicitly.
ARTIDFUE_UPDATE_ARTBEZFREMD
After article replication, the language-specific entries from the menu item "Further descriptions"
are transferred to the article master if the variable is active.After article transfer, the language-
specific entries from the menu item "Further descriptions" are transferred to the article master if
the variable is active. Here the local language from alsysinfo is evaluated.
Note that RP_ARTBEZFREMD may not be set!


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                   196
ARTICLE TRANSFER (client reference: no)
The variable applies for the article replication: Should article changes and new inclusions be
transferred to other sites?
0 - no, 1 - yes, 2 - optional
In addition to the variables, other individual configurations are required. See EN-CONFIG-A+W
Enterprise EDI.pdf section: Article replication - Triggers/Stored Procedure


RP_ARTTECHW (client reference: no)
The variable controls the transfer of data from table arttechw within article replication. It is set in
client. If the variable is set (default), the arttechw data will not be replicated. In the default setting
(ON), the data is not replicated because the technical values must be activated explicitly as a
module. Replication of the technical values must then be activated explicitly by deactivating the
variable.
RP_ARTBEZFREMD
This variable controls the replication of the data from table artbezfremd from the head office to
the corresponding site. If this variable is not set (default), the artbezfremd data will be transferred
at replication.
RP_ARTVARZU (client reference: no)
This variable controls the replication of the data from table artvarzu from the headquarters to
the corresponding sites. If this variable is not set (default), the artvarzu data will be transferred at
replication.


RP_NSTEUER
This variable controls the replication of the data from table nsteuer from the headquarters to the
corresponding sites. If this variable is not set (default), the nsteuer data will be transferred at
replication.
RP_NSTEUERATYP_TRANS (data transfer)
This variable controls article replication of article types from table nsteuer from headquarters to
the relevant site. If the variable is not set (default), the article type data from nsteuer is NOT
transferred during article replication. s.a RP_NSTEUER
RP_NSTEUERAWTYP (data transfer)
This variable controls the article replication of the A+W processing type data from table nsteuer
from the headquarters to the corresponding site. If the variable is not set (default), the A+W
processing type data from nsteuer is transferred during article replication.
RP_MUSSKENN
This variable controls the replication of the data from table musskenn from the headquarters to
the corresponding sites. If this variable is not set (default), all customer-related data will be
transferred at replication.
RP_MUSSKENNATYP_TRANS



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                  197
This variable controls the article replication of the article types from table musskenn from the
headquarters to the relevant site. If the variable is not set (default), the article type data from
musskenn is NOT transferred during article replication.



        18.7.14.         Error research
Standard supplier is not replicated
For replication, the standard supplier from the master is not transferred to the client, although a
standard supplier is maintained in the master and the supplier assignment was also replicated.
Here, the supplier is probably missing in the replication data for the article (see "Master data
maintenance")


A table is not replicated
Problem: A master data table is not replicated by the master on the client even though the
appropriate environment variable is set.
Research: Please heed the documentation of the environment variables precisely. There are
variables that switch the replication on and there are variables that switch the replication off.
Furthermore, it must be noted that the environment variables are evaluated in the Client -- NOT
in the master. If the variable is evaluated in the master, then this is mentioned explicitly in the
documentation of the environment variable.




    18.8. Key replication
For the alenv special logic, the standard installation may not be used for the key replication!
The key replication is a possibility to replicate any tables. Up to ALCIB – Version 2006, only tables
can be replicated for which the primary key consists of a maximum of 4 fields. Starting with ALCIB
– Version 2007 this restriction was expanded to 8 fields (ID 115729).
Starting with ALCIB -Version 3.2, this type of replication also supports local fields, analogously to
the market partner and article replication.
The program for key replication is started on the receiving site. It requires no transfer parameters
in order to find the transferred tables. The key replication determines the tables to be replicated
and the entries from them to be replicated independently.
The key replication works analogous to the market partner and article replication with direct
database connection between the master database and the client database.
Which database is the master database is defined in the table xhaus.
The key replication currently supports only database tables and database fields up to a length of
18 characters (restriction up to INFORMIX Version 7). The field content of key fields may not
currently exceed 20 characters (rp_* table).
30.03.17 Case #393597: The field content of key fields may not currently exceed 40
characters (rp_* table).


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  198
The deletion of key data is not supported (see section "Deleting data records")

        18.8.1.          Table xhaus
The table "xhaus" is a central table for all replications. It will therefore be described at the
beginning of the chapter.


        18.8.2.          Installationsscript prep_keyreplication
Starting with Version AWE 6, there is a script for support of the configuration =>
prep_keyreplication
The execution of the script is done in command line mode in the shell. It must be executed in the
master database environment.
Before the script is started, a few preparations are required:
        •   Read this documentation - completely!
        •   Check whether there is already a table rp_<Tabelle> and whether it can be
            deleted
        •   Check whether there is already a stored procedure (SP) pr_<Tabelle> and
            whether it can be deleted. Here you must check whether the SP only fills
            the table rp_<Tabelle> or executes other database or protocol operations.
        •   Check whether there is already a trigger or one of the triggers tri_<Tabelle>,
            tru_<Tabelle> and trd_<Tabelle> and whether they can be deleted. Here
            you must check whether the triggers only call the SP rp_<Tabelle> or
            execute other functions.
        •   Possible updating of the table documentation (tables altab and alfield:)
            The English development site is always the most up-to-date
            (Status as of 26.06.2017: site 1140)
        • The existing database scheme should be backed up with
          dbschema
        usage:
            prep_keyreplication (new|add) (|drop) (|notrigger) (|nosp) (all|<sitelist>)
                  -   new:          replace existing entries in table 'replichaus'
                  -   add:         append entries to table 'replichaus'
                  -   drop:        drop existing rp_tables and recreate
                  -   notrigger: do not create trigger on keytables
                  -   nosp:        do not create stored procedure for keytables
                  -   all:         add entries for all client sites within table 'xhaus'
                  -   <sitelist>: list of client sites (separated by blanks)


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                               199
    In the first step, the script creates the table replichaus (if it does not exist) and fills it
    according to the parameter specifications with the tables and clients to be
    replicated.
    Which tables are entered, that is, for which tables the replication should be set up,
    must be defined in the file ${ALDATPFAD}/keytables.dat. One standard is in
    ${ALCIBPRG}/cmd/keyreplication/keytables.template (for the tables included in this
    file, as of 12/17/2014, the keys maintained in altab were checked(Version 1130) )
    The script ensures that no doubled records are included in the table.
    If you would like to replicate individual tables for different clients, it may be
    necessary to remove the excess entries manually.
    Then the required rp_ tables are created in the right structure for all tables entered
    in the table replichaus. Via the parameter 'drop' it is possible to define whether an
    existing rp- table should be deleted and recreated (WARNING: check first whether
    there is any data to be replicated in there). If the parameter "drop" is not specified,
    the existing table is retained.
    Which key fields in the rp_ table must be created is defined via the table
    documentation of the table (table: alfield field: alkey).
    In the next step, the required stored procedure (SP) is created. Here it is first
    checked whether there is already an SP with the name pr_<keytable>. If there is
    already an SP, no SP is created for this table.
    With the "nosp" option, you can ensure that no SPs are created. In this case, the SPs
    must be created manually as described above and existing SPs must be expanded
    accordingly.
    (You can also delete the existing SPs after appropriate checking)


    In the next step, the required triggers are created. Here it is first checked whether
    there is already an insert, delete or update trigger on the key table (there is no
    individual check). If there is already a trigger, no triggers are created. Existing
    triggers are not deleted by the script.
    With the "notrigger" option, you can ensure that no triggers are created. In this
    case, the triggers must be created manually as described above and existing triggers
    must be expanded accordingly.
    (You can also delete the existing triggers after appropriate checking)

      18.8.3.        Table replichaus
    First, the table replichaus in the master database must be generated and filled. In
    the table, the table names must be entered and for them the site number of all sites
    for which this table is to be transferred. One record per table and site must be
    created.

A+W Software GmbH              EN-CONFIG-A+W Enterprise EDI.docx                               200
     This table is accessed within the SPs in order to determine the receiving site for
     each data change.
     This means that only the changes from the table are transferred that are entered in
     the table replichaus and the changes are only transferred to the sites for which the
     corresponding entry exists in this table.
     Starting with Version AWE 6, there is a script for support of the configuration =>
     prep_keyreplication
     usage:
     prep_keyreplication (new|add) (|drop) (|notrigger) (|nosp) (all|<sitelist>)
     - new:       replace existing entries in table 'replichaus'
     - add:       append entries to table 'replichaus'
     - drop:      drop existing rp_tables and recreate
     - notrigger: do not create trigger on keytables
     - nosp:     do not create stored procedure for keytables
     - all:      add entries for all client sites within table 'xhaus'
     - <sitelist>: list of client sites (separated by blanks)

       18.8.4.         Table replictab
Control table for key replication:
       Name                   Type               Description

       Ackflag                Smallint           Status flag
                                                 0 - To be processed
                                                 1 - In progress
                                                 2 - Error
       Haus                   Smallint           Target site for the replication


       Key                    Char(18)           Key column 1 for the table to be replicated
                                                 Key columns 1-8 form the primary key
                                                 of the table to be replicated
       key1                   Char(18)           Key column 2
       key2                   Char(18)           Key column 3
       key3                   Char(18)           Key column 4
       key4                   Char(20)           Key column 5
       key5                   Char(20)           Key column 6



A+W Software GmbH               EN-CONFIG-A+W Enterprise EDI.docx                          201
        key6                   Char(20)            Key column 7
        key7                   Char(20)            Key column 8
        mod_time               Datetime            Change date
        numkey                 Smallint            Number of key columns
        tabname                Char(40)            Table to be replicated


For document #444408, the database field tabname was increased to CHAR(40).



        18.8.5.         Special logic alenv table (#377840)
Key replication has been enhanced for replicating the table "alenv".
A new data field "R" = Replication has been added to the environment variable dialog ([CTRL] +
[F4] > Environment variables). This data field ("alenv.replicate") is provided with a checkbox and
controls whether you want to release the current data record for replication. Note that you can
only replicate or release data records with employee no. = 0 (ALENV.MANR) and site = 0
(ALENV.HAUS).
Replicated environment variables can no longer be changed in the client system. To prevent
employees from creating new environment variables on client systems, we have added a new
employee right. The employee right "SYEI - Create System Environment Variables" can be used to
revoke an employee's right to change (create/delete/change) new environment variables
When working with a Master - Sub-Master - Client structure, the setting "Data set is released for
replication", which is carried out in the master, also applies to the sub-master. This means that a
data set that is replicated from the master to the sub-master is also necessarily replicated to the
client. In the sub-master, further data records can be additionally released for replication in the
client
In order for the replication logic to work, some environmental and database adjustments must be
made. Please contact an A+W employee in this regard.
Replication of environment variables can be very dangerous and can lead to problems on the
client system, so please work very carefully with them!
Note/regard
•   -    This logic does not prevent the manipulation of the environment variables via database
    update. An environment variable that should be replicated into the client system and now
    locked could be manipulated afterwards.
•   It is possible that an environment variable is linked to another environment variable
    (ALENV.VALUE=$VARIABLE). In this case, you must ensure that you replicate both variables
•   The deletion of environment variables is not replicated
•   The table ALENVTXT is not replicated, but updated via setup update.
•   What happens if different clients need different ENV variable configurations?




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                               202
            o   Then these environment variables must be reconfigured. With replication you can
                only transfer "general data"
•   What happens to all employee-related variables?
            o   Only environment variables with employee no. = 0 (ALENV.MANR) and Haus = 0
                (ALENV.HAUS) can be replicated. Specific settings, such as employee or site, must
                be reconfigured
•   Are variables overwritten that are set differently for any reason?
            o   If an environment variable is replicated from the master system and is created in
                the client with the same conditions, the replication overwrites this variable with a
                database update.


Installation
      !!!The alenv replication may not be published with the standard installation
      method!!!
      The message files and the alenv table must be delivered again.
      The following environment files must be exchanged: alenv.mfo, alenv.1.mfo and
      alenv.2.mfo, alenv.pan, alenv.2.pan.
      The following database scripts must be executed: 130004069_alenv.sql,
      130004070_alenvproto.sql, 130004071_aledvmodule.sql, 130004072_rp_alenv.sql.
      The environment variable RP_ALENV_LOGIC must be activated in the master and
      the client.
      The script prep_alenv_replication must be executed. You can NOT use the existing
      script for key replication: prep_keyreplication!!!
      The script prep_alenv_replication can be called with three parameters: 
      prep_alenv_replication (master/client) (all/sitelist) (drop).
       1. The first parameter determines the location of your system (master or
          client). This tells the script which actions it may or may not perform.
          Currently, only one master device is required. If the script is called on a
          client, the script is interrupted with the message "Script can only be run on
          a master site".
       2. With the second parameter you define which clients you want to enter in
          the replichaus table or into which clients you want to replicate data from
          the master system.
       3. With the third parameter you can give the command that the existing
          triggers and stored procedures are dropped before the current versions are
          created.
          The following triggers are affected: trd_alenv, tri_alenv, tru_alenv.
         The following stored procedures are affected: pr_alenv, syinsupdel_alenvproto,
      pre_alenv_replicate

A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                               203
      Example:
     Setting up the master and a client entry (1140) in the replichaus:
     prep_alenv_replication master 1140
     Setting up the master, multiple client entries (1140, 130, 121) in the replichaus and
     dropping the SPs and trigger è prep_alenv_replication master 1140 130 121 drop
     Help: prep_alenv_replication -help
      Notes:
     pr_alenv: This SP writes to the rp_alenv and replictab tables. It is the counterpart to
     the dynamically generated pr_* procedures from key replication.
     syinsupdel_alenvproto: This SP writes to the alenvproto table. This logic was
     previously anchored directly in the above triggers.
     pre_alenv_replicate: This SP cleans up the rp_alenv table. It is called by the key
     replication and deletes all entries that do not contain an ALENV.REPLICATE indicator
     more.
Starting the transfer
     The transfer is started as for the standard key replication.



       18.8.6.   Creating the tables, triggers,                           and       stored
           procedures without prep_keyreplication
     The step creation of the rp_ tables is supported by the script "prep_keyreplication".
     The script will be explained at the beginning of the section.
     The installation steps explained in this section must be executed on the master
     database.

       18.8.7.          Required tables (rp_table)
     Der Feldinhalt von Schlüsselfeldern darf aktuell 20 Zeichen nicht
     überschreiten.(ALW 30.03.17 Vorgang #393597)
     The field content of key fields may not currently exceed 40 characters.
     For the key replication, it is necessary that there be an rp_* table for each table to
     be replicated. If the employee table "mitarb" should be replicated, for example,
     there must be a table rp_mitarb.
     The structure of the rp_* tables looks like this:


   <Key field1> char(40)
   [<Key field2> char(40)]


A+W Software GmbH              EN-CONFIG-A+W Enterprise EDI.docx                          204
   [<Key field3> char(40)]
   [<Key field4> char(40)]
   [<Key field5> char(40)]
   [<Key field6> char(40)]
   [<Key field7> char(40)]
   [<Key field8> char(40)]
   , haus              smallint
   , upinsdel          smallint
   , ackflag           smallint
   , usr               char(40)
   , mod_time          datetime year to minute


     The key fields depend on which primary keys exist in the regular table to be
     transferred. Using the example of the table "mitarb", the table rp_mitarb looks like
     this:


   manr                char(40)
   haus                smallint
   upinsdel            smallint
   ackflag             smallint
   usr                 char(8)
   mod_time            datetime year to minute


         If you were to replicate the table mp within the key transfer, the table rp_mp
         would be structured like this:


   mpnr                char(40)
   kuliflag            char(40)
   haus                smallint
   upinsdel            smallint
   ackflag             smallint
   usr                 char(8)
   mod_time            datetime year to minute



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                       205
     The data type of the key fields is always "char(40)", even if the key fields have
     another data type in the regular table. The field content of key fields may not
     currently exceed 40 characters.
     The additional fields haus, upinsdel, ackflag, usr, and mod_time are mandatory and
     have the following meaning:


   haus              To which site should the transfer be made
   upinsdel          If the data record was entered anew, changed or deleted
                     0 – deleted
                     1 – entered anew
                     2 - changed


   ackflag           is a new entry or if the entry is edited
                     0 – new entry
                     1 – entry is being transferred
                     2 – entry with which there were problems during transfer
   usr               login name of the employee who made the entry
   mod_time          date and time at which the entry was made.


     If a data record is changed several times in a row before it is transferred, the fields
     "usr" and "mod_time" are filled with the data from the last change.
     Which are the primary keys of a table m ust be documented in the table
     documentation (altab, alfield). If this should not be the case, each person who
     notices this bears the responsibility to correct this for the tables he has researched
     (ALTAB in the English development environment) The field content of key fields
     may currently not exceed 40 characters.



         18.8.8.     Required stored procedures (SP)
     The table rp_<table> is filled using a SP pr_<table>. The SP is called via the triggers
     named in the "Required triggers" section.
     If there is already an SP by this name for other functions, a renaming is not
     absolutely mandatory. However, these abbreviations correspond to the notation
     recommended by A+W. In the case that there is already an SP with this name, an
     installation with the script "prep_keyreplication" may only be possible with
     conditions.



A+W Software GmbH              EN-CONFIG-A+W Enterprise EDI.docx                           206
      18.8.9.        Required triggers
    Within the key replication, is possible the complete tables should not be
    transferred, but only the changed data records. For this reason, change triggers
    must be created for each table to be transferred. There should be one trigger for
    the action "insert" (new record is created), "update" (existing record is changed),
    and "delete (existing record was deleted). The triggers begin according to the action
    with the abbreviation tri_ (insert), tru_ (update), and trd (delete), followed by the
    name of the table for which the trigger is created (e.g. tri_mitarb - insert trigger in
    the table mitarb). If there are already triggers for these actions for other functions,
    a renaming of triggers with this notation is not absolutely mandatory. However,
    these abbreviations correspond to the notation recommended by A+W. In the case
    that there are already triggers, an installation with the script "prep_keyreplication"
    may only be possible with conditions.
    The triggers execute the same SP in which the insert or update to the table rp_*
    was made.
    Update trigger:
    create trigger tru_<tabelle>
    update on <tabelle>
    referencing old as pre new as post
       for each row
             (execute procedure
             pr_<tabelle>(pre.<Key field1>[,pre.>Key field2>[,pre.<Key field3>[,...]]])),
           (execute procedure            pr_<tabelle>(post.<Key field1>[,post.Key
           field2>[,post.<Key field3>[,.
           ..]]]));

    ??? Is the doubled call required for any logs ???

    Insert Trigger:
    create trigger tri_<tabelle>
    insert on <tabelle>
    referencing new as post
        for each row
              (execute procedure
              pr_<tabelle>(pre.<Key field1>[,pre.>Key field2>[,pre.<Key field3>[,...]]])),
         (execute procedure
          pr_<tabelle>(post.<Key field1>[,post.Key field2>[,post.<Key field3>[,.
            ..]]]));
    If there are already change triggers that execute other actions, the call of the SP
    must be built into the existing trigger. In this case, an execution of the installation
    with the script "prep_keyreplication" may only be possible with conditions.




A+W Software GmbH             EN-CONFIG-A+W Enterprise EDI.docx                               207
          18.8.10.        Deleting data records
The deletion of key data is not supported
June 2025 // replicate - 13.04.10729
Within the key replication, the table 'floskel' can also be replicated. Here, however, there is the
peculiarity that individual lines must be deleted during replication if necessary. Generally the
deletion of key data within the replication is not currently implemented.
In order to do justice to the particularity of the table 'floskel', the deletion of data records is
permitted explicitly only for the table "floskel". For this, depending on the current installation, the
stored procedure and the triggers must be adjusted for the table.
The stored procedure must contain a code as parameter whether the deletion is of lines.
e.g.
create procedure pr_floskel(pkey char(20),pkey1 char(20),pkey2 char(20), upinsdel smallint)


Depending on this, for the insert in the table rp_floskel, the field "upinsdel" must be set to 0 for
records to be deleted.
e.g.
insert into rp_floskel (code,manr,line,haus,upinsdel,ackflag,usr,mod_time)
values (pkey,pkey1,pkey2,hh,upinsdel,0,user,current);


In the triggers that call the stored procedure, the call must also be expanded to include another
parameter.
e.g.
for deletion trigger
FOR EACH ROW(
         EXECUTE PROCEDURE pr_floskel(pre.code, pre.manr, pre.line,0));


for insert or update trigger
FOR EACH ROW(
       EXECUTE PROCEDURE pr_floskel(post.code, post.manr, post.line, 2));



          18.8.11.        Troubleshooting
For each table to be replicated, there is a corresponding rp_* table with the field ackflag.
The field can contain the following values
0 – must be transferred
1 – is currently being transferred


A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                 208
2 – general error
2000 + (SC*-1) – database error
For more precise details, the log must be inspected.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx   209
19. External market partner interface
The market partner interface is a general interface for taking over market partners (customers,
suppliers, others) from third-party systems into A+W Enterprise. Here, it is not possible and
especially not necessary to fill all fields of the A+W Enterprise market partner master data with
this interface. A re-entry in A+W Enterprise is therefore nearly always necessary.
Within an installation with internal client separation, the call of the market partner scheduling is
only possible for the main client (client that makes available the database number and is in
xhaus.hauptmandant).


     19.1. Interface structure
                                     Max                        IMPDFUE-
Field No. Description     Type                  Values                         ALCIB-Field   Comment
                                     Length                     Field
                                                N=New,                         <no
1         New or Change A            1                          New                          Config
                                                C=Change                       storage>
          Market partner
2                        N           8          <required>      Mpnr           mp.mpnr       Config
          Number
3         Matchcode       A          10                         Mpmc            mp.mpmc
                                                1=Customer;
4         Partner Flag    N          1                          kuliflag       mp.kuliflag
                                                2=Supplier
          Customer
5                         A          35                         Name           mp.name
          Name
6         Tax key         N          4                          VAT            mp.mwst
7         Address Code    N          4                          anrede         mp.anrede
                                                                               mp.zhd /
          Contact person
8                        A           35                         Attn           mp.vname / Config
          addr info
                                                                               mp.branche
                                                                               mp.str /
9         Street          A          35                         Str                       Config
                                                                               mp.zhd
10        Postcode        A          11                         ZIP            mp.plz
                                                                               mp.ort /
11        Place           A          35                         Place                     Config
                                                                               mp.str
          Country
12                      A            3                          kfzcode         mp.kfzcode   Config
          shortcut
13        Country       A            35                         land           mp.land     Config
14        Language Code N            2                          sprkz          mp.sprkz
                                                                               mp.stddebn
15        Std Debtor      N          8                          stddebnr
                                                                               r
16        Std User        N          5          not in use      stdvertr       mp.stdvertr
                                                                               mp.versand
17        Dispatch Key    N          5                          versandart
                                                                               art
                                                                               mp.verpack
18        Packing Key     N          5                          verpackart
                                                                               art
          Private
19                      N            12                         firmlimit      mp.firmlimit Config
          Company Limit
                                                                               mp.limpruef
20        Limit Check flag N         1                          limpruefkz
                                                                               kz
21        Currency        A          3                          waehrung       mp.waehru Config


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                   210
                                      Max                   IMPDFUE-
Field No. Description        Type              Values                      ALCIB-Field     Comment
                                      Length                Field
                                                                           ng
          Cash Discount
22                       N/A          3 / 10                skonto1        mp.skonto1 Config
          Key
          Number of days
23                       N            3                     zahlziel       mp.zahlziel
          for payment
          Kind of                                                          mp.zahlngm
24                       N            3                     zahlngmerk
          payment                                                          erk
                                                                           mp.rechnun
25        Type of invoice N           1                     rechnungsart
                                                                           gsart
          Minimum                                                          mp.relimwe
26                          N         10                    relimwert
          Order Amount                                                     rt
          Part delivery
27                          N         1                     teiliefkz      mp.teilliefkz
          flag
28        Part invoice flag N         1                     teilfakkz      mp.teilfakkz
          Gross prices                                                     mp.preisdrk
29                          N         1                     preisdrkz
          print flag                                                       z
          Discount print
30                          N         1                     rabdrkz        mp.rabdrkz
          flag
          Position                                                         mp.kndposk
31                          N         1                     kndposkz
          reference flag                                                   z
          Glazing price                                                    mp.verglasu
32                          N         1                     verglasung
          calc flag                                                        ng
                                                                           mp.vertrerlo
33        Agent              N/ A     5                     vertrerloe                  Config
                                                                           e
34        Active flag        N        1        not in use   still          mp.still     Config
          Add/exchange
35                           N        1                     azkz           mp.azkz
          flag
          Processing                                                       mp.explbear
36                           N        1                     explbearbkz
          price print flag                                                 bkz
37        Statistics Flag    N        1        not in use   statkz         mp.statkz
          Divers market
38                           N        1                     divers         mp.divers
          partner flag
          Condition                                                        mp.kbranch
39                           N        4                     kbranche
          Branch Code                                                      e
                                                                           mp.kwrtrau
40        Region             N        4                     kwrtraum
                                                                           m
          Telephone
41                           A        20                    telefon        mp.telefon
          number
42        Fax Number         A        20                    faxnr          mp.faxnr
                                                                           mp.massyst
43        Metric system      N        1                     massystem
                                                                           em
44        Label text key     N        2                     etikett        mp.etikett
45        Route Code         N        3                     routenr        mp.routenr
46        Handlings time     N        2                     hzeit          mp.hzeit
          Project must
47                           N        1                     objmuss        mp.objmuss
          flag
48        BTW Number         A        20                    steuernr       mp.steuernr
          Private key for
49                           A        15                    fibukey        mp.fibukey
          finac trans
                                                                           mp.innenma
50        Internal user      N        5                     innenmanr
                                                                           nr
51        External User      N        5                     aussenmanr     mp.aussen

A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                            211
                                      Max                   IMPDFUE-
Field No. Description        Type              Values                       ALCIB-Field    Comment
                                      Length                Field
                                                                            manr
                                                                            mp.sachma
52        Internal user      N        5                     sachmanr
                                                                            nr
          ALCIB field                                                       mp.stdvergl
53                           N                              stdverglas
          stdverglas                                                        as
          Private field                                                     mp.private_
54                           N        8                     private_long1
          long 1                                                            long1
          Private field                                                     mp.private_
55                           N        8                     private_long2
          long 2                                                            long2
          Private field                                                     mp.private_
56                           A        15                    private_char1
          char 1                                                            char1
          Private field                                                     mp.private_
57                           A        15                    private_char2
          char 2                                                            char2
          Position of cust                                                  mp.routepo
58                           N        3                     routeposnr
          on route                                                          snr
                                                                            mp.statdeb
59        Statistic debtor N          8                     statdebnr
                                                                            nr
          Order                                                             mp.waehrpr
60                           N        1                     waehrprs
          calculation flag                                                  s
          Currency Print                                                    mp.waehrdr
61                           N        1                     waehrdru
          Key                                                               ukz
          Call before
62                           N        1                     anruf           mp.anruf
          delivery
          Prod seq
                                                                            mp.prodfolg
63        ordered by         N        2                     prodfolge
                                                                            e
          partner
          Driving time in
64                           N        2                     anfahrt         mp.anfahrt
          days
65        Delivery type      N        4                     lieferart       mp.lieferart
          External
66        supplier           A        15                    exlinr          mp.exlinr
          number
          Supplier
67        number of          N        8                     lieflinr        mp.lieflinr
          customer
          Type of price
68                           N        1                     prsdarst        mp.prsdarst
          printing
          Grouped
69                           N        1                     lsammel         mp.lsammel
          delivery paper
          Condition                                                         mp.konddeb
70                           N        8                     konddebnr
          debtor                                                            nr
          Std partner for
71                           N        8                     azdebnr         mp.azdebnr
          add/exch rules
          Order conf /                                                      mp.sprosse
72                           N        1                     sprossenab
          xbar papers                                                       nab
          External
                                                                            mp.extkund
73        customer           A        30                    extkundnr
                                                                            nr
          number
74        Fax j/n            N        1                     faxokay         mp.faxokay
75        Quality class      N        2                     qklass          mp.qklass
76        Quality class      N        2                     qzuverl         mp.qzuverl
77        Quality class      N        2                     qzeit           mp.qzeit


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                          212
                                     Max                     IMPDFUE-
Field No. Description       Type                Values                      ALCIB-Field   Comment
                                     Length                  Field
78        Quality class     N        2                       qpreis         mp.qpreis
79        Quality class     N        2                       qqual          mp.qqual
80        Quality class     N        2                       qservice       mp.qservice
81        Quality class     N        2                       qberat         mp.qberat
82        Quality class     N        2                       qkulanz        mp.qkulanz
                                                                            mp.qbonita
83        Quality class     N        2                       qbonitaet
                                                                            et
          Geographic
84                        N          4                       region         mp.region
          region
          Reference must                                                    mp.exaufmu
85                        N          1                       exaufmuss
          flag                                                              ss
          Delivery stop                                                     mp.liefersto
86                        N          1          1 - Yes      lieferstop                  Config
          flag                                                              p
          Invoice stop                                                      mp.fakturas
87                        N          1          1 - Yes      fakturastop                 Config
          flag                                                              top
          Commission                                                        mp.kommm
88                        N          1                       kommuss
          must flag                                                         uss
          Direct purchase                                                   mp.direktbe
89                        N          1                       direktbestkz
          flag                                                              stkz
          Alternative                                                       mp.routenr
90                        N          3                       routenr2
          route                                                             2
          Alternative                                                       mp.routenr
91                        N          3                       routenr3
          route                                                             3
          Alternative                                                       mp.routenr
92                        N          3                       routenr4
          route                                                             4
          Limit of
                                                                            mp.srechlim
93        grouped         N          10                      srechlimit
                                                                            it
          invoice
          Grouped
94                        N          1                       srechart       mp.srechart
          invoice type
95        Email address A            80                      email          mp.email
                                     50
                                     Starting
          KvK Nummer                                                        mp.firmnam
96                     A             with QR                 firmname
          Company name                                                      e
                                     2410
                                     150
97        insurance limit   N        12,2                    akvlimit       mp.akvlimit Config
                                                                            mp.limverfal
98        Insured up to     D        10         dd.mm.yyyy   limverfall
                                                                            l
99        Addressline 2     A        35                      branche        mp.branche Config
                                                                            mp.ort
100       Addressline 4     A        35                      address4                  Config
                                                                            QR2406:
                                                                            mp.vname
                                                                            bankv.bnam
101       name (bank)       A        35                      bvbname                   Config
                                                                            e
          place of
102                       A          35                      bvsitz         bankv.sitz
          business (bank)
          bank code
103                       N          8                       bvblz          bankv.blz
          number
          account                                                           bankv.konto
104                       A          20                      bvkontonr
          number                                                            nr


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                              213
                                      Max                        IMPDFUE-
Field No. Description        Type                Values                          ALCIB-Field   Comment
                                      Length                     Field
                                                                                 bankv.kfzco
105        country symbol A           3                          bvkfzcode
                                                                                 de
106        IBAN            A          40                         bviban          bankv.iban
           bank
107        identification  A          20                         bvbic           bankv.bic
           code (BIC)
           standard bank                         0 (false) / 1                   <no
108                        N          1                          bvstdbv                       Config
           flag                                  (true)                          storage>
109        Addressline 109 A          35                         address109      mp.str        Config
           P.O.Box Zip
110                        A          11                         address110      mp.pfplz      Config
           Code
111        P.O.Box         A          10                         address111      mp.postfach Config
                                                                                 mp.erfassto
112        Order stop flag N          1          1 - Yes         erfasstop                   Config
                                                                                 p
           Customer
113        group             A        3                          group           grpzu.grpnr Config
           assignment
                                                                                 <no
114        P.O.Box place     A        35                         address114                    Config
                                                                                 storage>
           print indicator
                                                 0 (false) / 1                   mp.sumkom
115        for Printout      N        1                          sumkomis                  AWE 6
                                                 (true)                          is
           sub-total
           last date of
                                                                                 mp.ltzschuf
116        credit limit      D        10         dd.mm.yyyy      ltzschufa                     AWE 6
                                                                                 a
           enquiry
           object-oriented                       0 (limit check)
                                                                                 mp.objlimit
117        limit check or    N        1          / 1 (order      objlimitpruef                 AWE 6
                                                                                 pruef
           via order                             check)
           Cash Discount
118                          N/A      3                          skonto2         mp.skonto2 Config
           Key 2
           Cash Discount
119                          N/A      3                          skonto3         mp.skonto3 Config
           Key 3
120        Department        N/A      15                         Abtnr           mp.abtnr    Config
121        Cost center       N/A      30                         Kostenst        mp.kostenst config
122        Mobile            N/A      20                         Mobile          Mp.mobile


      19.2. Environment prerequisites
Prerequisite for the use of this interface is a functioning EDI environment (xhaus entries,
trm_ctrl_* scripts, EDI directory environment...)
As additional settings for this interface, the following points are required:

      1. Setting of the environment variable DFUE_MPDFUE_INDIR. This variable defines the
         interface directory in which the interface program expects the transfer files. In the
         defined directory, there must be a subdirectory <$HAUS> and <$HAUS/save>. In the
         environment variables, the directory is specified without these subdirectories. If the
         variable is not defined, the program uses the directory $DFUEDIR/fibudat/transfer/.




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                   214
        The corresponding interface directory must have read and write rights for the user
        alcibnet.

    2. There are various ways to start the market partner scheduling:

    a) The external system that makes the interface file available sends a trigger file to
       $DFUEDIR/wait. This file must correspond to the naming convention *.r<ALCIB-
       Hausnummer>. The file is structured as follows:
       /usr1/alcibnet/bin/trm_ctrl_<site> 10 1 23 0 <site> <site> 0 </dev/null >>
       /usr1/alcibnet/proto/custprot.<site>
       #END#
        Alternatively, there can be a script (e.g. getcust) in the directory $ALCIBPRG/spec/cmd
        geben that starts the trm_ctrl startet and sends the external program in the trigger file
        only the call of the script.
        Script getcust:
       umask 0
       if [ ! -f /usr1/alcibnet/dfue_lock ]
       then
             exec /usr1/alcibnet/bin/trm_ctrl_$1 10 1 23 0 $1 $1 0 </dev/null
       >>/usr1/alcibnet/proto/custprot.$1
       fi

        Triggerfile:
        getcust <ALCIB site no.>

Note (12/10/2007): getcust apparently works with two parameters (site number and file name).
The trigger file that is placed in the wait directory can be called anything. Important is only the
extension r<siteno.>, so that it is processed by the correct EDI starter. For example,
customer_interface_start.r100
This file in the wait directory must in any case have read and write rights for alcibnet.
The getcust call (getcust <site> <file>) is in the file.
WARNING! The file must have an end identifier (last line #END#)!
For example:
getcust 100 awemp.test
#END#
Via the trigger file, the getcust is called automatically by the user alcibnet, so that the problem
that uudecode empties the Z file should not occur.
Via the env variable S_A_EXCHANGEDIR, it is controlled where the file to be imported is picked
up.


The advantage of this variant is less system load since there is only a call if there is really
something to do. Furthermore, it is ensured that the interface has been written completely.

    b) Within the operating system, a crontab entry is configured, which in the end also calls
       the scrips getcust described in a).



A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                215
        The disadvantage of this version is that system calls are made without there being a file
        for processing. In addition, it can happen that a file is touched that has not yet been
        transmitted completely.

    c) A manual call is attached within the ALCIB menu element Individual programs.
        The disadvantage of this path is that somebody has to remember to start the scheduling
        and a substitution rule must also be established.




    19.3. Restrictions of the interface
The market partner interface currently does not support the scheduling of site-specific data
(multi-site configuration). The interface only stores the market partner record for the main site
without the site-specific information.
The interface file can include as many market partners as desired. If, however, more than 100
new market partners are sent in an interface file, only the first 100 market partners with their
numbers are listed in the communication mail. For all other market partner n umbers, see the log
$DFUEDIR/mpin*.
Each data record in the interface file must end with a CR+LF; in particular, this must be the case
for the last record. The interface file must be present in the Unix file format (line-end format).
01.12.2022: The market partner interface can now also process files in DOS format (line-end).
        Field separator:         The fields are separated with the separator '^'.
                                 The interface itself converts the interface file in order to executed
                                 a "load" and in the process, replaces all "^" with "|". Therefore,
                                 "^" and "|" are the only characters that may not occur in the
                                 interface data.

                                 Note: the last field also ends with a field separator.
        Field length:            There is no fixed field length (use of a field separator). The defined
                                 length is a maximum length that arises from the A+W Enterprise
                                 data structure.
      Field orientation: All fields must be specified left flush.
        Empty fields:            In "empty" numeric fields, the interface requires the number 0
                                 (zero). In alphanumeric fields, no entry is required (one field
                                 separator follows another directly)
                                 Additional information in section "Reset numeric values"
        Date format:             data details must be specified in the format "dd.mm.yyyy."
                                 Whereby dd is the day, mm the month, and yyyy the year.
        Decimal details:         within decimal details, the "." (dot) must be used as decimal
                                 separator.(example: 1425.25)




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 216
    19.4. Interface table
For scheduling of the MP data, the interface table impdfue is filled. The table is regularly
generated with the delivery of an A+W Enterprise via sql script. The functionality of the interface
is thus only guaranteed if alcib and trm_ctrl have the same release version number.
impdfue includes 108 columns (status as of 12/20/2020). The last column is called "bvstdbv."
The last 8 columns with the prefix "bv" were added in order to be able to store bank details.
Starting with ALCIB 2009: the table impdfue is adjusted independently by scheduling to the
currently required structure. For this, the existence of the last required field is checked. If this is
not there, the table is regenerated completely. Therefore, it can happen that when first starting
the scheduling, a database error SC -217 is documented for a field in the log, which, however, is
present for subsequent checks.




    19.5. Process
When A+W Enterprise creates a new market partner, it is created with the appropriate
information from the interface file. At the same time, it is deactivated (mp.still=1). This is
necessary since not all required information is provided via the interface.
The interface program sends a message to a defined employee (environment variable
DFUE_MPDFUE_MAILTOO with the first 100 market partners, who were created anew.
If A+W Enterprise changes a market partner, only the fields are changed whose fields in the
interface are not empty (see also environment variables and section "Local fields"). In this case,
no message is sent that the market partner has been changed.
In the case that the external system sends a value not equal to "empty" for a field that should be
local in A+W Enterprise, you can use the "local fields" in A+W Enterprise. For this, the field with
the table "impdfue" (NOT! "mp") must be entered on the dialog "A+W Enterprise – System – Data
transfer local fields." At the same time, the environment variable
DFUE_MPDFUE_USE_LOCALFIELDS="ON" must be set.
Caution: heed note in the chapter "Local fields for active env variable
DFUE_MPDFUE_IGNORE_FLD1"!


        19.5.1.          Log
The interface program writes the following process log: $DFUEDIR/proto/mpout_proto<site>,
$DFUEDIR/proto/mpin_proto<site>
$DFUEDIR/proto/mpmsg<site>.




A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                     217
    19.6. Local fields/Transfer of 0 values
Within the external market partner interface, data in the A+W Enterprise market partner master
data is not overwritten if in the interface no information is sent along for the affected field (0 - for
numeric fields, '<empty>' - for alphanumeric fields).
Now it is possible that external maintenance programs cannot be adjusted sufficiently,
nevertheless all fields in the ALCIB market partner master data should be protected.
The system can now be configured so that fields that are defined as local are not overwritten in
case of changes (environment variable DFUE_MPDFUE_USE_LOCALFIELDS). Within the new
inclusion via the interface, there is no function change. In this case, the data is taken over as it is
sent. There is also no evaluation of the default values within the local fields.
The local fields are maintained for the table "impdfue" (!! not mp!!) under "System" - "Data
transfer" - "Local fields."
Caution: heed note in the chapter "Local fields for active env variable
DFUE_MPDFUE_IGNORE_FLD1"!



        19.6.1.   Resetting numeric values to 0 (default) (case
            185124)
Starting with Version 4.4 (2009), numeric values of the MP master data can be set via the
interface to '0' if the value '-1' is transferred in the appropriate interface field.


        19.6.2.  Local  fields for  active                                      env         variable
            DFUE_MPDFUE_IGNORE_FLD1
Caution: in Versions 2011 and 2012 (4.5 and 12.5), the local fields do NOT work together with
active DFUE_MPDFUE_IGNORE_FLD1 (see also AWDesk #343734)
In Version 2009 with AWDesk #346776, the program has been adjusted so that the local fields
work together with active DFUE_MPDFUE_IGNORE_FLD1.
Starting with Version 6 (13.2) with AWDesk #391805, the program has been adjusted so that the
local fields work together with active DFUE_MPDFUE_IGNORE_FLD1.


        19.6.3.          mp.sprkz as local field
In versions < 6.4, the customer language is not retained if mp.sprkz is declared as a local field;
instead, the language is drawn from alsysinfo.sprkz. In order to retain the customer language, the
env variable DFUE_MPDFUE_USE_KUSPRACHE must also be activated with ON.
Starting with Version 67.4, the customer language is retained with mp.sprkz as local field even
without setting the env DFUE_MPDFUE_USE_KUSPRACHE.
See also AWDesk #392072.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  218
    19.7. Address logic
The storage of particular address fields in the A+W Enterprise-MP master data is done depending
on an environment variable.
Until Version 2008.2 (4.3), the storage of the interface fields 8, 9, 11, 13, 99 and 100 was
controlled via the variable DFUE_MPDFUE_UK_ADDRESS.
Starting with Version 2009 (4.4), the variable DFUE_MPDFUE_ADDRESSVARIANT replaces the
variable DFUE_MPDFUE_UK_ADDRESS.
It now controls the storage of the interface fields 8, 9, 11, 99, 100 and 109.



        19.7.1.           New address logic
(Case 148094)
The MP interface was expanded with ALCIB Version 2009 (4.4) to include the field "address line
109"; here, the number 109 stands for the sequential field number of the new field in the
interface file. The new field has a length of 35 characters.
With appropriate configuration in the A+W Enterprise market partner master data, the field
"address line 109" is taken over to "mp.str."
The new environment variable DFUE_MPDFUE_ADDRESSVARIANT replaces or overrides the
environment variable DFUE_MPDFUE_UK_ADDRESS.
If the variable DFUE_MPDFUE_ADDRESSVARIANT is deactivated or not present, the variable
DFUE_MPDFUE_UK_ADDRESS is evaluated.
DFUE_MPDFUE_ADDRESSVARIANT has the following characteristics:

            o     0 -> the address fields in table mp are assigned according to default logic
            o     1 -> the address fields in table mp are assigned according to UK address logic

            o     2 -> the address fields in table mp are assigned according to the logic
                  described here (address logic 2, text further below)




Field                        Variant 0 (default)        Variant 1 (UK logic)     Variant 2
Field 8 (contact person
                             mp.zhd                     mp.vname                 mp.branche
addr info)
Feld 9 (street)              mp.str                     mp.zhd                   mp.zhd
Feld 11 (place)              mp.ort                     mp.str                   mp.ort
Feld 99 (Addressline 2)      mp.branche                 mp.branche               <Niu>
                             <Niu>
Feld 100 (Addressline 4)     starting with QR2406       mp.ort                   <Niu>
                             mp.vname



A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                             219
Feld 109 (addressline
                             <Niu>                        <Niu>                    mp.str
109)
Feld 110 (P.O. Box Zip
                             mp.pfplz                     <Niu>                    <Niu>
Code)
Feld 111 (P.O. Box)          mp.postfach                  <Niu>                    <Niu>
Feld 114 (P.O. Box
                             Mp.pfort                     <Niu>                    <Niu>
place)


The logic described here is also available in ALCIB Version 2007 (4.1).


        19.7.2.           Standard shipping address
Within the external market partner interface, the default shipping address is set equal to the
invoice address. This is not always desired. Therefore, the interface can now be configured so that
with the storage of a market partner, no standard shipping address is set.
MPDFUE_NOSTDADR (client reference: no)
  If this variable is active with the value ON, for market partners that are stored via the market
partner interface, no standard shipping address is set. If the variable is not active or if it contains a
different value than ON, then the standard shipping address is set equal to the invoice address.


        19.7.3.           Post box postal code/post box (cf. 173629)
The interface is in a position to take over values for post box postal code and post box.
The new fields are expected in field number 110 (post box postal code) and 111 (post box) of the
interface file.


     Field               Data type             ALCIB field                Description
     no.
     110                 CHAR(11)              mp.pfplz                   Post box postal
                                                                          code
     111                 CHAR(10)              mp.postfach                P.O. box




    19.8. Handling of special fields
Some interface fields of the general market partner interface of A+W Enterprise are processed
specially before they are saved in the A+W Enterprise database (market partner master data).
The special processing takes place if the appropriate A+W Enterprise environment variable is set.




A+W Software GmbH                    EN-CONFIG-A+W Enterprise EDI.docx                                220
        19.8.1.          Ignore change code – Field 1
In the first field of the interface, it is defined whether this is a new market partner or whether an
existing market partner should be changed. Not all external systems are in a position to send this
identifier correctly. Therefore, it is possible to configure the system so that this field is ignored on
import and the interface itself determines whether it is a new creation or a change.
For this, the environment variable DFUE_MPDFUE_IGNORE_FLD1 has to be activated.
Caution: heed note in the chapter "Local fields for active env variable
DFUE_MPDFUE_IGNORE_FLD1"!



        19.8.2.          Market partner number field 2
The A+W Enterprise market partner number is sent in the second field of the interface. Not all
external systems recognize this number. Therefore, starting with A+W Enterprise 6 (build status
01/01/2021), the system can be configured so that with a new creation, the market partner
number is determined from the appropriate number range (kunde.mfo, lief.mfo). In this case, the
fields “Standard ”, “Statistic debtor”, “Conditions debtor” and “Exchange/additional debtor”
(stddeb, statdeb, konddeb, azdeb) are set equal to the market partner number determined.
To do this, the environment variable DFUE_MPDFUE_USE_NR_SERVER has to be activated.
See also chapter "Changed referencing" (DFUE_MPDFUE_REFERENCE_FLD)
Attention: This function can only be used together with the function "Ignore change"!


        19.8.3.          Changed referencing
The A+W Enterprise market partner number is sent in the second field of the interface. Not all
external systems recognize this number. Therefore, starting with A+W Enterprise 6 (build status
01/01/2021), the system can be configured so that in a field you can define yourself in the table
"mp", an external reference is defined.
For this, the corresponding field has to be defined in the environment variable
DFUE_MPDFUE_REFERENCE_FLD .
See also chapter "Market partner number" (DFUE_MPDFUE_USE_NR_SERVER).
Attention: This function can only be used together with the function "Ignore change"!


        19.8.4.          Country (fields 12 and 13)
If the field 12 "Länderkürzel" is changed, the field 13 "Land" also has to be changed via interface
file. The field is not updated via the key table.
Within the external market partner interface, in field 12 the A+W Enterprise country code
(xland.kfz) is expected. However, frequently external systems work with the 2-digit ISO country
code and can therefore only transfer it. The system can now be configured such that the interface
expects the ISO country code and using the table xland undertakes a conversion to the A+W
Enterprise country code.
To do this, the environment variable DFUE_MPDFUE_USE_KFZISO has to be activated.

A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  221
        19.8.5.          Company limit / Assu. limit– field 19 / 97
DFUE_MPDFUE_CHECK_LIMITCUR
Within the external market partner interface, in fields 19 and 97 the appropriate limit in the A+W
Enterprise site currency (MODUL_WAEHRUNG) is expected. However, frequently external
systems keep the limit in market partner currency and can therefore only transfer this. The
system can now be configured such that the interface checks whether the market partner
currency (interface field 21) matches the site currency (MODUL_WAEHRUNG). If this is not the
case, then possibly transferred limits will be converted into site currency.
If for a change transfer the market partner currency of the site currency should be changed into
another one, the limits are not sent, however; there is no conversion.
To do this, the environment variable DFUE_MPDFUE_CHECK_LIMITGCUR has to be activated.


        19.8.6.          Currency – field 21
Within the interface field 21 (waehrung), the A+W Enterprise short description of the currency is
expected (xwaehr.kurzbez). This is implemented with the storage using the table xwaehr in the
ALCIB currency number xwaehr.wnr. If the environment variable DFUE_MPDFUE_USE_FIBUKEY is
set, the FinAc code (xwaehr.fibuschl) is expected instead of the short description.



        19.8.7.          Discount condition (SkontoX) – fields 22 / 118 /
            119
        (AWDesk 137173)
Within the external market partner interface, in field 22 the A+W Enterprise code for the payment
condition (xxskonto.zahlbed) is expected. However, frequently external systems work with
different alphanumeric codes and can therefore only transfer these. The system can now be
configured such that the interface expects the external code and using the table
cu_mpdfue_zahlbed undertakes a conversion to the A+W Enterprise code. To do this, the
environment variable DFUE_MPDFUE_CU_ZAHLBED has to be activated.
In this case, the type of the interface field changes to alphanumeric and the maximum length to
10 characters.
Structure of the table
      cu_mpdfue_zahlbed (
      zahlbed        smallint
      fremdbez        char(10)
      comment         char(35)
      )
With case 137173, a CU maintenance dialog was made available for the table.
Please copy the included files into the following directories:
- cu_mpdfue_zahlbed.mfo nach CUST/mfo
- cu_mpdfue_zahlbedk.mfo nach CUST/mfo
- cu_mpdfue_zahlbed.mly nach CUST/mly


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                222
- cu_mpdfue_zahlbedk.mly nach CUST/mly
- cu_mpdfue_zahlbed.sel nach CUST/sel

AFter that, the dialog cu_mpdfue_zahlbedk.mfo has to be attached to the desired place with
customizing.

Attention: the dialog cannot prevent the entry of duplicate records. That is, the operator is
responsible for ensuring that only one record is stored per payment condition on the screen.

With case 244101, the table and maintenance dialog were expanded.
cu_mpdfue_zahlbed (
  zahlbed smallint,
  fremdbez char(5),
  comment char(35),
  accountref char(2)
)


Expanded discount logic - skonto2 and skonto3
With case [AW-59013] (A+W Enterprise 6 – Release 01.01.2021) the table – not the maintenance
dialog – was expanded.
cu_mpdfue_zahlbed (
 zahlbed smallint,
 fremdbez char(5),
 comment char(35),
 accountref char(2),
    zahlbed2 smallint,
    zahlbed3 smallint,
)


The expansion is not absolutely necessary. The following changed function applies if the
environment variable DFUE_MPDFUE_CU_ZAHLBED is active:
    a) The field 22 "Skontoschlüssel" is filled, the fields 118 "Skontoschlüssel 2" and 119
       "Skontoschlüssel 3" are not filled.
           a. If the fields zahlbed2 and zahlbed3 in the table cu_mpdfue_zahlbed are not filled,
                then as previously, only the field mp.skonto1 = cu_mpdfue_zahlbed.zahlbed
                where cu_mpdfue_zahlbed.fremdbez= <Feld 22> is occupied.
           b. If the fields zahlbed2 and/or zahlbed3 in the table cu_mpdfue_zahlbed are filled,
                     mp.skonto1 = cu_mpdfue_zahlbed.zahlbed where
                        cu_mpdfue_zahlbed.fremdbez= <Field 22>
                     mp.skonto2 = cu_mpdfue_zahlbed.zahlbed2 where
                        cu_mpdfue_zahlbed.fremdbez= <Field 22>
                     mp.skonto3 = cu_mpdfue_zahlbed.zahlbed3 where
                        cu_mpdfue_zahlbed.fremdbez= <Field 22>

      b) The field 22 "Skontoschlüssel" is filled, the fields 118 "Skontoschlüssel 2" and/or 119
         "Skontoschlüssel 3" are also filled.


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                              223
                          mp.skonto1 = cu_mpdfue_zahlbed.zahlbed where
                           cu_mpdfue_zahlbed.fremdbez= <Field 22>
                          mp.skonto2 = cu_mpdfue_zahlbed.zahlbed where
                           cu_mpdfue_zahlbed.fremdbez= <Field 118>
                          mp.skonto3 = cu_mpdfue_zahlbed.zahlbed where
                           cu_mpdfue_zahlbed.fremdbez= <Field 119>

Attention: if you would like to use this expanded discount function, it is absolutely necessary that
the current interface structure is sent with 119 fields.


         19.8.8.           Sales revenue representative - field 33
(AWDesk 244101)
If the environment variable AGC_SAP_INTERFACE_VERSION is set to a value greater than or equal
to 6, the external sales representative (alphanumeric, maximum 5 characters) is transformed into
a numeric A+W Enterprise sales representative (mp.vertrerloe). The corresponding A+W
Enterprise key is selected from the cu table cu_g_sap_salesrep (column manr).
cu_g_sap_salesrep should have the following structure:
cu_g_sap_salesrep (
    sapsalesrep CHAR(5),
    manr INTEGER
)
If the mapping table cu_g_sap_salesrep is not found or if a corresponding data record cannot be
found, the sales representative is set to 0 in A+W Enterprise (mp.vertrerloe).


         19.8.1.           Active flag (mp.still) - field 34
According to the current interface description, the "active flag" (still) is not evaluated. Newly
transferred market partners are always scheduled deactivated (still=1), since if necessary not yet
all required data was transferred via interface.


[AW-75341] – August/2021

The interface was adjusted as follows.

If a market partner is transferred anew, it is scheduled deactivated as previously (still=1). If a
market partner is transferred as a change, the field "active flag" is evaluated as follows:

-1 – The market partner is activated (still = 0);

0 – The market partner remains unchanged

1 – The market partner is deactivated (still = 1)

This adjustment is bracketed out for reasons of compatibility with a new environment variable
DFUE_MPDFUE_USE_STILL.


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                224
        19.8.2.         Delivery stop – field 86
(AWDesk 244101)
Available starting with ALCIB Version 2009 and higher
If the environment variable DFUE_MPDFUE_UNBLOCK_WITH_ZERO is set, the customer's
delivery stop flag (mp.lieferstop) is reset if a zero is transferred in interface field 86. If the
variable is not set, the flag can be taken back for an existing customer only by sending "-
1"in the interface field.

        19.8.1.         Invoice stop – field 87
(AWDesk 244101)
Available starting with ALCIB Version 2009 and higher
If the environment variable DFUE_MPDFUE_UNBLOCK_WITH_ZERO is set, the customer's
delivery stop flag (mp.fakturastop) is reset if a zero is transferred in interface field 86. If
the variable is not set, the flag can be taken back for an existing customer only by sending
"-1"in the interface field.

        19.8.2.         Bank account – field 101, 108
(Case 138785)
Starting with Version 4.2 (ALCIB 2008), by default it is possible to transmit bank details in the
interface by default.
The interface logic detects transferred bank details if the field 101 ("Bank name") is filled. Such
banking details are stored, regardless of whether an account number or routing number was also
transferred. (same logic as on A+W Enterprise dialog "Banking details")
Since it is essentially possible to create several sets of banking details for a market partner and
one of the sets of banking details can be marked as main banking details, there is a differentiated
control logic for storage via the field 108 ("Default banking details") and the environment variable
DFUE_MPDFUE_BANKV.
If field 108 in the interface data record is not assigned, a transferred set of banking details is
stored as main banking details. The logic as described in the comments about the environment
variables DFUE_MPDFUE_BANKV applies.
If field 108 is assigned the value 1 (default banking details = TRUE), the logic described above also
applies.
If field 108 is assigned the value 0 (default banking details = FALSE), the scheduling happens as
follows:
    -   If there are no banking details, the banking details are stored in A+W Enterprise
        regardless of the value in DFUE_MPDFUE_BANKV. However, these do NOT become the
        main banking details.


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 225
     -    If there are already banking details and DFUE_MPDFUE_BANKV is active with value 1
          (ADD), another set of banking details is created. It does NOT become the main set of
          banking details

     -    If there is already a set of banking details and DFUE_MPDFUE_BANKV is active with
          value 2 (ERR), the storage of the current market partner is interrupted with an error.

     -    If there are already banking details and DFUE_MPDFUE_BANKV is active with value 0
          (UPDATE), the banking details are ignored and not stored. The storage of the current
          market partner is done entirely normally.


          19.8.3.          Entry stop - field 112
         (AWDesk 244101)
Available starting with ALCIB Version 2009 and higher
If the environment variable DFUE_MPDFUE_UNBLOCK_WITH_ZERO is set, the customer's order
stop flag (mp.erfasstop) is reset if a zero is transferred in interface field 112. If the variable is not
set, the flag can be taken back for an existing customer only by sending "-1"in the interface field.



          19.8.4.          Market partner – group assignment – field 113
(AWDesk 244101)
Available starting with ALCIB Version 2009 and higher
If the environment variable AGC_SAP_INTERFACE_VERSION is set to a value greater than
or equal to 6, the external group assignment (alphanumeric, maximum 3 characters) is
transformed into a numeric A+W Enterprise group assignment (xxgrp.grpnr). The
corresponding numeric A+W Enterprise key is selected from the cu table cu_g_sapseg
(column grpnr).
cu_g_sapseg should have the following structure:
cu_g_sapseg (
    grpnr SMALLINT,
    sapseg char(3)
)
If in the table cu_g_sapseg no numeric A+W Enterprise group number can be found, no error
occurs. A message is written to the mpout-logfile and no group assignment is made for the
customer.
A group assignment is only made if the selected numeric A+W Enterprise group is greater than or
equal to 1000.
If a group assignment cannot be made because the numeric A+W Enterprise group in the master
data (table xxgrp) was not found, the saving of the customer is canceled. A message is written to
the mpin-logfile.


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                   226
The group assignment logic only tolerates a group assignment with grpnr >= 1000. If an existing
market partner is updated via the interface and a group number >= 1000 is sent in the interface
file and there are already two (or more) different group assignments for the market partner with
grpnr >= 1000, all group assignments >= 1000 are deleted and a new group assignment is added
to the table grpzu. The grpzu.klasskz is taken over from the master data (table xxgrp).
If an existing market partner is updated via the interface and a group number >= 1000 is sent in
the interface file and there is already a group assignment for the market partner with grpnr >=
1000 (deviating from the group number in the interface file), the existing group assignment is
updated (grpzu.grpnr changes), the existing klasskz is retained.



        19.8.5.        Department – field 120
[AW-138254] // September 10, 2023
In field 120 "Department," the A+W Enterprise department number can be transferred. By
default, the interface expects a department number from the A+W Enterprise master data (table
abteilung.abtnr). The interface does not check whether the department transferred exists in the
department master data. It is taken over unchecked.
With the environment variables "DFUE_MPDFUE_ABTNR" a transformation of the department
sent into an A+W Enterprise department number can be configured.
If the environment variable is "1", the interface expects the department abbreviation from the
A+W Enterprise department master data (table abteilung.abtid). In this configuration, the
customer is responsible for ensuring that the department abbreviation is unique. If the
transformation of the department abbreviation into a department number cannot be made, the
department number 0 will be processed by the interface.
If the environment variable is "2", the interface expects an external department abbreviation. This
is translated into an A+W Enterprise department number using the table "cu_mpdfue_abtnr". The
table has at least the following structure
cu_mpdfue_abtnr(
abtnr integer
,fremdbez char(15)
,comment char(30)
)
No maintenance dialog for this table is provided by A+W. If the transformation of the external key
into a department number cannot be made, the department number 0 will be processed by the
interface.



        19.8.6.        Cost center – field 121
[AW-138254] // September 10, 2023
The A+W Enterprise cost center can be transferred in the field 121 "cost center". By default, the
interface expects a cost center from the A+W Enterprise master data (table kstelle.kostenst). The


A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                                 227
interface does not check whether the cost center transferred exists in the master data. It is taken
over unchecked.
With the environment variables "DFUE_MPDFUE_KOSTENST" a transformation of the cost center
sent into an A+W Enterprise cost center can be configured.
If the environment variable is "1", the interface expects an external cost center key. This is
translated into an A+W Enterprise cost center using the table "cu_mpdfue_kostenst". The table
has at least the following structure
cu_mpdfue_kostenst(
kostenst char(30)
,fremdbez char(15)
,comment char(30)
)
No maintenance dialog for this table is provided by A+W. If the transformation of the external key
into a cost center cannot be made, the cost center "<empty>" will be processed by the interface.




     19.9. Control possibilities (environment variables)
DFUE_MPDFUE_ABTNR (client reference: no)
  By default, the external market partner interface expects an A+W Enterprise department
number in the field "Department". If this environment variable is
    1 - instead the department abbreviation is expected (abteilung.abtid)
    2 - there is a transformation using the table cu_mpdfue_abtnr


DFUE_MPDFUE_CHECK_LIMITCUR
Within the external market partner interface, in field 19 and 97 the appropriate limit in the A+W
Enterprise site currency (MODUL_WAEHRUNG) is expected. However, frequently external systems
keep the limit in market partner currency and can therefore only transfer this. The system can
now be configured such that the interface checks whether the market partner currency (interface
field 21) matches the site currency. If this is not the case, then possibly transferred limits will be
converted into site currency.
If for a change transfer the market partner currency of the site currency should be changed into
another one, the limits are not sent, however; there is no conversion.
DFUE_MPDFUE_CU_ZAHLBED
Within the external market partner interface, in field 22 the ALCIB code for the payment condition
(xxskonto.zahlbed) is expected. However, frequently external systems work with different
alphanumeric codes and can therefore only transfer these. The system can now be configured
such that the interface expects the external code and using the table cu_mpdfue_zahlbed
undertakes a conversion to the ALCIB code.
DFUE_MPDFUE_FNAME



A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                               228
The interface program tries to work through all files in the defined input directory
(DFUE_MPDFUE_INDIR). With this variable, the system can be configured so that only files with
the suffix defined in these variable are processed. The ending is entered without the dot. If, e.g.
only files of the screen *.ext should be processed, then the value "ext" has to be defined here.
DFUE_MPDFUE_IGNORE_FLD1
Within the external market partner interface, the specification is expected in field 1 whether this
market partner is a new market partner or whether an existing market partner should be
changed. However, external systems cannot always make this information available correctly. The
system can now be configured so that the interface ignores the specification in field 1 and decides
itself whether this is a new creation or a change.
Caution: heed note in the chapter "Local fields for active env variable
DFUE_MPDFUE_IGNORE_FLD1"!
DFUE_MPDFUE_INDIR
This variable defines the interface directory in which the interface program expects the transfer
files. In the defined directory, there must be a subdirectory <$HAUS> and <$HAUS/save>. In the
environment variables, the directory is specified without these subdirectories. If the variable is
not defined, the program uses the directory $DFUEDIR/fibudat/transfer/.
DFUE_MPDFUE_KOSTENST (client reference: no)
  The external market partner interface expects an A+W Enterprise cost center in the field "Cost
center". If this environment variable is
  1 - there is a transformation using the table cu_mpdfue_kostenst
DFUE_MPDFUE_MAILTO
E-mail address of the person who is to be informed about an incorrect data import at the market
partner interface.
A complete e-mail address including domain should be stored in the variables.
Only as an aside:
ALCIB can also be configured so that it communciates to the mail server that it should complete
addresses:


AWMAIL_EXPN_RECIPIENT
This variable controls whether the recipient's mail address is to be expanded or not when e-mails
are sent. The expansion takes place via the mail server. Here the execution of the command expn
must be allowed. Only then can AWmail pass this information along. But then the mail server
must also be configured appropriately.


DFUE_MPDFUE_NOMAIL
By setting these variables, the sending of info mails is switched off when creating new market
partners via market partner EDI.
DFUE_MPDFUE_UK_ADDRESS
Changed takeover of the address fields within the external market partner interface (see
comment in Excel sheet)


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                   229
DFUE_MPDFUE_UNBLOCK_WITH_ZERO
If the environment variable is set, the fields invoice stop (mp.fakturastop), entry stop
(mp.erfassstop) and delivery stop (mp.lieferstop) are reset if a 0 (zero) is sent in the interface. If
the variable is not set, this identifier can only be reset by sending "-1".
DFUE_MPDFUE_USE_FIBUKEY
Within the interface field 21 (waehrung), the A+W Enterprise short description of the currency is
expected (xwaehr.kurzbez). This is implemented with the storage using the table xwaehr in the
ALCIB currency number xwaehr.wnr. If this environment variable is set, the FinAc code
(xwaehr.fibuschl) is expected instead of the short description.
DFUE_MPDFUE_USE_KFZISO
Within the external market partner interface, in field 12 the A+W Enterprise country code
(xland.kfz) is expected. However, frequently external systems work with the 2-digit ISO country
code and can therefore only transfer it. The system can now be configured such that the interface
expects the ISO country code and using the table xland undertakes a conversion to the A+W
Enterprise country code.
DFUE_MPDFUE_USE_KUSPRACHE
In the case that in the market partner interface the language transferred = 0, then with set
variable, the customer's language is retained. If the customer is transferred for the first time (new
entry), the language = 0. If the variable is not set and the transferred language is 0, then the
national language of the storing client is entered as the customer language. If the language in the
interface file is != 0, then in any case this will be entered as the customer language
DFUE_MPDFUE_USE_LOCALFIELDS
If this variable is active, local fields for the table impdfue are evaluated within the external market
partner interface. For change transfers, fields defined as local fields are not changed. Default
values are currently not considered. The local fields are not evaluated for new systems. Values
transferred for new systems are stored as transferred.
See also section "Local fields"
DFUE_MPDFUE_USE_NR_SERVER (client reference: no)
The A+W Enterprise market partner number is sent in the external market partner interface in
field 2. If this is not known in the external system, it can be defined with this environment variable
that the market partner number for new market partners is determined from the corresponding
number range in A+W Enterprise.
s.a DFUE_MPDFUE_REFERENCE_FLD
DFUE_MPDFUE_USE_STILL (client reference: no)
  Within the external market partner interface, field 34 is not evaluated by default. If this
environment variable is active, the field is evaluated as follows in case of change (not new
creation):
  -1 – The market partner is activated (still = 0);
  0 – The market partner remains unchanged
  1   The market partner is deactivated (still = 1)


DFUE_MPDFUE_REFERENCE_FLD (client reference: no)

A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                     230
The A+W Enterprise market partner number is sent in the external market partner interface in
field 2. If this is not known in the external system, the field from the table mp can be defined in
this variable via which the referencing between the external system and A+W Enterprise is done.
e.g. private_char1
DFUE_MPDFUE_BANKV
The variable controls how a transferred set of banking details is handled for storage. Possible
values are:
0 or deactivated (UPDATE) => bank details are added as main bank details or overwrite existing
main banking details
1 (ADD) => banking details are also saved and become the main banking details
2 (ERR) => if there a set of main banking details already exists, the storage of the market partner is
rejected. If no main banking details are assigned, the banking details are created as main banking
details.
The variable is evaluated together with the flag "Standardbankverbindung" (field 108) in the
interface data record. See section "Banking details."


MPDFUE_NOSTDADR (client reference: no)
  If this variable is active with the value ON, for market partners that are stored via the market
partner interface, no standard shipping address is set. If the variable is not active or if it contains a
different value than ON, then the standard shipping address is set equal to the invoice address.




    19.10. Descriptions of problems
        19.10.1.         Empty file
Problem: The interface file was processed in the first step (log $DFUEDIR/proto/mpout*)
(implementation of the currency, etc. and copied to $DFUEDIR/dat. After that, the program
reports that the file was empty.
Log except mpout*:
…
data successfully copied from /usr1/alcibnet/fibudat/transfer/493/SAP_CLIENT_4.txt to
/usr1/alcibnet/dat/0002.493.493.02
Data file was empty - nothing to transmit!


Solution: The interface file contains no or the incorrect line end character.
Open the file with vi and note the message at the bottom of the screen.
If the message "incomplete last line" appears there or there is an ^M at the end of the line, the
file has to be corrected.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                  231
        19.10.2.         Load failed
Problem: When storing the interface, in the 2nd step (log $DFUEDIR/proto/mpin*) there was an
error message during the load.
Log excerpt mpin*:
…
Begin messages from al_load():
Too many values in input set.
End messages from al_load().
ERROR: Load failed - error code -1!
…
Solution:The table structure of the table "impdfue” is not correct. Restart interface since the
interface adjusts the table structure by itself. If the error occurs again, the table structure has to
be compared to the structure at A+W.
(Tip: start the comparison at the end)



        19.10.3.         Local fields are not considered
Problem: The fields defined as local are overwritten with values from the interface
Solution: Check the log – in the top log, the state of the environment variables is documented. It
must be checked whether the environment variable DFUE_MPDFUE_USE_LOCALFIELDS is active
(set). If the variable is active, check whether the local fields were defined correctly for the
interface. The local fields are maintained for the table "impdfue" (!! not mp!!) under "System" -
"Data transfer" - "Local fields."




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 232
20. Status reporting from financial
 accounting
[AW-74011] It happens every now and then that invoices and credit notes are generated and
booked in A+W Enterprise, but these cannot be taken over into financial accounting for a variety
of reasons. The causes are on both sides. Therefore, a function was created that only performs
the booking process in A+W Enterprise if financial accounting has given its OK. The function has to
be released with a new environment variable. Speak to your project team about this.
The functionality is documented in "EN-CONFIG-A+W Enterprise.pdf".




A+W Software GmbH                EN-CONFIG-A+W Enterprise EDI.docx                              233
21. Receipt of goods
    21.1. Incoming goods inspection
There is a possibility via a control pool to generate receipt of goods and purchase invoices based
on the underlying PO and a received invoice.
This customer-specific solution is described in the following document:
https://awsoftwaregmbh.sharepoint.com/sites/AWClarityRD/Shared%20Documents/Interfaces/E
nterprise/B2B%20Interfaces/DE-
A+W%20Enterpprise%20%20Cust%20Auto%20Goods%20Receipt.docx?web=1




    21.2. External receipt of goods (e.g. SAP)
        21.2.1.         Configuration
      For this interface, some new binfiles and tables are required.
              1. The new binfile "SAPtoAlcibinterface" must be present in $ALCIBBIN.
              2. The binfile alcib must be up-to-date (A+W Enterprise 6)
              3. The script "getnextsafile" must be executable in $ALCIBPRG/cmd or
                  $ALCIBPRG/spec/cmd.
              4. The table "autwe" must exist.
              5. The environment variable "KEINE_WLAGER_BUCHUNG" must be active
                  if there should be no stock booking for receipt of goods.
              6. Environment variable S_A_EXCHANGEDIR defines the interface
                  directory for all interface files that are sent by SAP to A+W Enterprise.
              7. In the interface directory $S_A_EXCHANGEDIR, the subdirectories
                  'done', 'failed', and 'history' must exist.
              8. The EDI processing directory $DFUEDIR/wait must exist and the process
                  dfue_starter must process it (general EDI prerequisite also for order
                  generation, etc.)
              9. The interface file must be stored with the defined name
                  s_a.GRN.<yyyymmddhhmmss.<nnnnnn>.<working site>.<transfer site>
                  in the defined interface directory $S_A_EXCHANGEDIR. Another trigger
                  file with the ending ".r<transfer site>" must be written to
                  $DFUEDIR/wait. The trigger file contains
      sap_to_alcib <filename>
      #END#




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                              234
      21.2.2.       Process
    It is not necessary to write/rename the file since the second line #END# lets it be
    known unambiguously whether a file was written completely. Only files with this
    second line "#END" are processed.
    The ALCIB polling daemon "dfue_starter" processes the file and starts the script
    "sap_to_alcib". This script sends the file to another server <working site> if this is
    required due to entries in the xhaus table of the client <transfer site>. Then the file
    is stored in the directory ./done or ./failed, as defined above.


    sap_to_alcib
    The script must be installed on all clients in $ALCIBPRG/cmd or
    $ALCIBPRG/spec/cmd. The script must have execution rights. The script is linked to
    the script alcib_to_sap. The script itself requires a second script
    get_host_from_xhaus. This script must be installed on all sites in $ALCIBPRG/cmd.
    The script must have execution rights.
    This script sap_to_alcib handles all transfer from SAP to ALCIB. If the file given as
    parameter has the ending .<transfer site>, the script checks in the xhaus table of the
    site the master on which the site specified in the file name is located
    get_host_from_xhaus). After that, the file is copied to a file or transferred via FTP,
    whereby the ending .<transfer site> is omitted and a file with the ending .r<working
    site> is generated in the appropriate wait directory in order to start the further
    processing (the processing is started using the interface name, which is also part of
    the file name)
    Example:
    s_a.GRN.20040718123247.123456.130.199
    is copied or transferred via ftp to the client 130 and renamed
    s_a.GRN.20040718123247.123456.130
    in addition, a file s_a.GRN.20040718123247.123456.130.r130
    with the content
    SAPtoAlcibinterface
    #END#
    is generated in /usr1/alcibnet/wait on the server where the client 130 is installed.
    The dfue_starter for client 130 then starts the interface "Good receipt for POs" for
    client 130.
    The script writes the log to
    $DFUEDIR/proto/asa`date +%y%m%d`_proto${HAUS}
    and


A+W Software GmbH             EN-CONFIG-A+W Enterprise EDI.docx                           235
    $DFUEDIR/proto/s_a.${INTERFACE}.`date +%y%m%d`_proto${HAUS}. $INTERFACE is
    the interface file code. (e.g. GRN for goods receipt)


    get_host_from_xhaus
    The script must be installed on all servers and all clients (master and production) in
    $ALCIBPRG/cmd or $ALCIBPRG/spec/cmd. The script must have execution rights.
    The script determines the server name for the site transferred as parameter from
    the table "xhaus". The script is used by the script "sap_to_alcib".
    get_env_from_site
    The script must be installed on all servers and all clients (master and production) in
    $ALCIBPRG/cmd or $ALCIBPRG/spec/cmd. The script must have execution rights.
    The script determines the value for the environment variable transferred as
    parameter for the sites transferred and the employees transferred from the table
    "alenv". It's important that the client transferred is available via SQL via
    xhaus.informixserver.


    The program "SAPtoAlcibinterface" reads the interface files. This binary uses the
    script "getnextsafile" in order to find the right interface file in the right sequence.
    After that, the interface data is written to the table "autwe":
    auftrnr                 A+W Enterprise PO number(field 2 in the interface)
    ltplan                  Shipping date of the supplier (field 8)
    lieferschein            Supplier's delivery note number
    posnr                   A+W Enterprise internal item number (field 3)
    geliefert               Delivered quantity per item (field 5)
    liefkompl               Complete flag: 1- item delivered completely (field 9)
    fehlerflag              Error status if the booking fails
    kianz                   Number of boxes (only if NEUE_KISTENLOGIK on)
    blattanz                Number of lites per box (only if NEUE_KISTENLOGIK on)
    exaufnr                 external reference (field 4)


    After reading the file, checking the values, and inserting into the table "autwe" the
    booking function is called. This function reads the table "autwe" and creates a
    receipt of goods in A+W Enterprise.
    There is always only one receipt of goods in A+W Enterprise. If a second receipt of
    goods is sent by SAP (partial receipt of goods) or an existing receipt of goods is
    changed, the previous receipt of goods is canceled and a new one created with the
    special values. SAP has to send the complete current values per item each time.


A+W Software GmbH             EN-CONFIG-A+W Enterprise EDI.docx                               236
      Attention! The cancellation of the receipt of goods has no influence on the
      inventory.
      After creating the receipt of goods, the data records are removed from the table
      autwe. If the booking was successful, the interface file is pushed into the
      subdirectory /done. In case of a failed booking the file is pushed into the
      subdirectory /failed.
      An interface file may always contain only one receipt of goods (a PO). For each
      article, only one data record per interface file is possible.
      The standard ALCIB receipt of goods booking starts a stock booking if this is a stock
      product. If these bookings are no longer needed (because SAP sends the stock
      receipt in another way), you must set the environment variable
      KEINE_WLAGER_BUCHUNG="ON".

        21.2.1.          Housekeeping
To clean up the interface directories the following must be installed:
    1. The script SAPhistory must exist in $ALCIBPRG/spec/cmd or $ALCIBPRG/cmd and have
       execution rights.
    2. Create a script D<n>sapcleanup in the individual cron directory (e.g.
       /alcib/cron/daily/<site>) to clean up the directories daily. If only cleaning up on the
       weekends is required, then the script W<n>sapcleanup (e.g. /alcib/cron/weekly/<site>)
       can be created. The script in question includes the call "SAPhistory".
The script “SAPhistory” generates 10 subdirectories in $S_A_EXCHANGEDIR/history and
$A_S_EXCHANGEDIR/history if these do not exist. After that, it deletes all files from history/10
with each call and pushes all files from history/<n> to history/<n+1>. At the same time, all files
from the "done" subdirectory are pushed to history/1.
This means, if the script is called once a day the interface files will be kept for 10 days. If the script
is called once a week, the files are retained for 10 weeks.
The files from the subdirectory ".failed" are not moved. This directory must be checked manually
and cleaned up.
Deviating from this, an individual clean-up can also be configured. However, there is no automatic
cleaning up without configuration.



        21.2.1.          Interface structure
Receipt of goods for POs (AWDESK 89021 / AWDESK 89470)
Field Description            Type      Max        Values              ALCIB
No.                                    Length
1      Movement Type         Num       3          101-Receipt,        1 - Goods receipts
                                                  102-Receipt         2 - Invoice
                                                  Reversal, 122-      3 - credit note
                                                  Vendor Return


A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                                  237
                                                no see ALCIB



2      PO number            Num       8         to identify PO      alcib order no
3      item no              num       5         to identify PO      alcib item no
                                                item
4      ref no               char      20        (SAP- refenz no)    -> kauf.exaufnr
5      Quantity             Num       10        9999999,99          -> kpos.menge
6      Price                num       10,2      9999999,99          only invoices and credit notes
                                                                    net price per piece (each)
7      credit marker        num       1                             only for Credit notes
                                                                    0 - only values
                                                                    1 - values and quantitys
8      aktion date          Num       8         ddmmyyyy            -> edat, bdat
9      final flag           num       1                             0 - no final
                                                                    1 - final



Notes for the goods receipt
- in ALCIB there is only a goods receipt
- for the goods receipt, the total quantities are transferred to ALCIB (including complete identifier
- corrections, cancellations, partial goods receipts also specify the total quantity
Alcib cancels the lten goods receipt and generates a new one with the total quantity. There is no
history.
Attention! The cancellation of the receipt of goods has no influence on the inventory.
- Within an interface file, there may only be either records with item number > 0 or a record with
item number = 0 . A mixture is not allowed.
Without separators, the files are expected in the file with a permanently defined length. Each line
is only one item and each file contains only one PO. A mixture of item lines and a PO completion
line in a file is not possible.
A PO can be marked as completely delivered. For this function ALCIB expects the ALCIB PO no.,
ALCIB item no. = 0 , and completion ID=1. In this case, no data record with an item number larger
than 0 may be present in the interface file. If there are data records with item no.=0 and item no.
greater than 0 the data records with size 0 are ignored.


        21.2.2.          Log
The interface writes a log to $PROTOPFAD/SAP_ALCIB_EK_<mmdd>. The booking
function writes the standard booking log $PROTOPFAD/frei<mmdd>.
Error messages in the SAP_ALCIB_EK_* log:


A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 238
    1 – Umgebungsvariable WARENEINGANG_EXTERN nicht gesetzt (nicht mehr
    erforderlich)
    2 – table "autwe" is empty
    3 – PO not found in A+W Enterprise
    4 - PO already completely delivered
    5 – PO cancelled
    6 – Supplier not found in database
    7 – Supplier cancelled
    8 – PO locked by another user
    9 – Old PO cannot be cancelled
    10 – There is more than one receipt of goods
    11 – PO cannot be completed.




A+W Software GmbH            EN-CONFIG-A+W Enterprise EDI.docx            239
22. SAP Oxygen coupling
    22.1. General
All imports are executed via a call of the A+W ERP REST service.
All exports are processed via the A+W Enterprise Export Service. So that data is written to the
booking table exportinfo, the switch MODUL_OXYGEN must be set.


        22.1.1.           General switch (alenv)
DFUE_MPDFUE_REFERENCE_FLD                            Database field in table mp, in which the SAP
                                                     reference for customers and suppliers is saved.
OXYGEN_BASEURL                                       Basic address of the Mulesoft server for exports
OXYGEN_USER                                          User name for Mulesoft server
OXYGEN_PASSWORD                                      Password for Mulesoft server
OXYGEN_COMPANYCODE                                   SAP Company Code Mapping
OXYGEN_PLANT                                         SAP Plant Mapping
OXYGEN_WBSCOUNTRYCODE                                SAP WBS Country Code Identifier
OXYGEN_PURCHASEORG                                   SAP Purchase Organization
OXYGEN_COSTCENTER                                    SAP Cost Center for Purchase


        22.1.2.           Tables
The following tables must be created in the system:
    •   wltooxygen
              o   Detail table for exportinfo.
              o   The link is made via the column exportid -> exportinfo.longwert1
              o   Use of the columns see chapter 22.9
    •   cu_pr_artdfue (Should already be present)
              o   Reference from AWE article number/variant to SAP material code
Description                         Database field                   Type
AWE article number                  artnr                            Integer
AWE variant                         varnr                            Short integer
SAP material code                   artdfue                          String(20)
Used by all interfaces in which fixed material codes from or to SAP are transferred.
    •   cu_sapadrnr



A+W Software GmbH                   EN-CONFIG-A+W Enterprise EDI.docx                             240
              o   Reference of AWE address to SAP address
Description                        Database field                  Type
AWE address number                 adrnr                           Integer
SAP address                        exadrnr                         String(20)
Filled by customer/supplier import and used during order export.
       •   cu_sapbaufnr (Should already be present)
              o   Reference from AWE PO to SAP PO
Description                        Database field                  Type
AWE PO number                      Baufnr                          Integer
SAP PO                             exaufnr                         String(20)
Filled by the interface PO import and transferred during PO generation to the external order
number.
       •   cu_sapraufnr
              o   Reference from AWE invoice to SAP invoice
Description                        Database field                  Type
AWE invoice number                 raufnr                          Integer
SAP invoice                        exaufnr                         String(20)
Is filled during invoice export with the SAP invoice number. For credit notes, this number must be
used for the SAP credit note.
       •   cu_sapbmnrbez
              o   Reference from AWE machine to SAP machine
Description                        Database field                  Type
AWE machine number                 bmnr                            Integer
Site                               Haus                            Integer
SAP machine name                   sapbez                          String(20)
Used for the reporting of machine cost records to SAP.


           22.1.3.        Stored Procedure "cu_sgg_generic_material"
This procedure returns the SAP code for the generic material for an item
Description                        Database field                  Type
Document number                    auftrnr                         Integer
Document type                      vorgang                         Short integer
Item number                        lfdpos                          Short integer
Return is a string with maximum 20 places that determines the code for generic material in SAP.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                            241
          22.1.4.       Stored Procedure "cu_sgg_wlraumtosap"
This procedure returns the SAP storage location for an AWE storage location. If the AWE storage
location is 0, the SAP storage location for the production should be returned.
Description                        Database field                    Type
AWE storage location number        lnr                               Integer
Return is a string with maximum 20 places that determines the code for the storage location in
SAP.


          22.1.5.       Stored Procedure „ cu_sgg_wlraum “
This procedure converts the SAP storage location into the AWE storage location.
Description                        Database field                    Type
SAP storage location               Called on import                  String(20)
Return is an integer value with the AWE storage number.


    22.2. Import of customers and suppliers
Trigger: REST service is called by SAP.
During import of customers/suppliers, the SAP reference is saved in the field that is specified in
the environment variable (alenv)


    22.3. Import of stock POs
Trigger: REST service is called by SAP.


    22.4. Import of articles and variants
Trigger: REST service is called by SAP.


    22.5. Export of purchase orders
Trigger: When setting the PO lock
The trigger creates an entry in the table exportinfo with the following details:
Interface                                             „OXYGENPURCHASEORDER“
Auftrnr                                               P.O. number
Docum.                                                Document number (2)
Haus                                                  SITE




A+W Software GmbH                  EN-CONFIG-A+W Enterprise EDI.docx                                 242
    22.6. Export of orders
          22.6.1.       Creation of the cost carrier (WBS)
Trigger: Successful scheduling in the production system (currently deactivated at customer
request)
The trigger creates an entry in the table exportinfo with the following details:
Interface                                           „OXYGENWBS“
Auftrnr                                             Order number
Docum.                                              Document number (5)
Haus                                                SITE


          22.6.2.       Transfer of the orders
Trigger: Run release in the prodution system (currently deactivated at customer request)
The trigger creates an entry in the table exportinfo with the following details:
Interface                                           „OXYGENSALES“
Auftrnr                                             Order number
Docum.                                              Document number (5)
Haus                                                SITE



    22.7. Export of delivery notes
Trigger: Delivery note created or together with invoice? (currently deactivated at customer
request)
The trigger creates an entry in the table exportinfo with the following details:
Interface                                           „OXYGENDELIVERY“
Auftrnr                                             Order number
Docum.                                              Document number (6)
Subnr                                               Sequential number of the delivery (1, 2, ...)
Haus                                                SITE



    22.8. Export of invoices and credit notes
Trigger: When booking the invoice/credit note (currently deactivated at customer request)
The trigger creates an entry in the table exportinfo with the following details:



A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                 243
Interface                                           „OXYGENBILLING“
Auftrnr                                             Invoice or credit note number
Docum.                                              Document number (7=invoice, 9=credit note)
Haus                                                SITE




      22.9. Export of receipt of goods
Trigger: Receipt of goods is booked
The trigger creates an entry in the table exportinfo with the following details:
Interface                                           „OXYGENRECEIPTOFGOODS“
Auftrnr                                             Receipt of goods number
Docum.                                              Document number (3)
Subnr                                               Sequential number of the receipt of goods (1, 2,
                                                    ...)
Haus                                                SITE



      22.10. Export of stock transactions and finished
        messages
          22.10.1. Stock correction and stock correction takeback
              (type 551 + 552)
Trigger: Stock removal booking with breakage reason
The trigger creates an entry in the table exportinfo with the following details:
Interface                                           „OXYGENSTOCKSCRAP“
Longwert1                                           Key for details in table wltooxygen
Haus                                                SITE
Table wltooxygen
Lnr     Artnr    Varnr   B_menge me         tolnr   kostenst auftrag      lfdpos Zuhaus Exportid
1       100004   23      4.8          4     0       BREAK                                    2


          22.10.2.       Inventory (differences) (type 711 + 712)
Trigger: Inventory completion
The trigger creates per stock article, which has a difference, an entry in the table exportinfo with
the following details:

A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                                244
Interface                                           „OXYGENSTOCKINV“
Longwert1                                           Key for details in table wltooxygen
Haus                                                SITE
Table wltooxygen
Lnr    Artnr     Varnr   B_menge me         tolnr   kostenst auftrag      lfdpos Zuhaus Exportid
1      100004    23      4.8          4     0                                              3
1      100002    5       -19.26       4     0                                              3


        22.10.3.         Rebookings (type 301)
Trigger: Stock rebooking was booked or goods were sent from one site to another site
The trigger creates an entry in the table exportinfo with the following details:
Interface                                           „OXYGENSTOCKMOVE“
Longwert1                                           Key for details in table wltooxygen
Haus                                                SITE
Table wltooxygen
Lnr    Artnr     Varnr   B_menge me         tolnr   kostenst auftrag      lfdpos Zuhaus Exportid
1                        4.8          4     0                   4711      1        15      1
1      100004    23      4.8          4     2                                              2


        22.10.4.         Stock removal for order (type 291)
Trigger: Report of glass cutting (XTV reporting) (currently deactivated at customer request)
The trigger creates an entry in the table exportinfo with the following details:
Interface                                           „OXYGENCONSUMPTION“
Longwert1                                           Key for details in table wltooxygen
Haus                                                SITE
Table wltooxygen
Lnr    Artnr     Varnr   B_menge me         tolnr   kostenst auftrag      lfdpos Zuhaus Exportid
1      100002    5       1.04         4     0                   4711      1                4


        22.10.5. Receipt of goods by production in dispatch
            warehouse (type Z01 + Z02)
        Trigger: Finished report of an item from the production system
The trigger creates an entry in the table exportinfo with the following details:


A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                            245
Interface                                           „OXYGENPRODUCED“
Longwert1                                           Key for details in table wltooxygen
Haus                                                SITE
Table wltooxygen
Lnr    Artnr     Varnr   B_menge me         tolnr   kostenst auftrag      lfdpos Zuhaus Exportid
0                        30.6         4     0                   4711      1                 5



      22.11. Export of PO wishes
Trigger: PO request created from PO pool or PO changed.
The trigger creates an entry in the table exportinfo with the following details:
Interface                                           „OXYGENPURCHASEREQ“
Auftrnr                                             Inquiry number.
Docum.                                              Document number (1)
Haus                                                SITE



      22.12. Export of cost records
Trigger: Run release in the production system (currently deactivated at customer request)
The trigger creates an entry in the table exportinfo with the following details:
Interface                                           „OXYGENPRODCOST“
Auftrnr                                             Order number
Docum.                                              Document number (5)
Haus                                                SITE




A+W Software GmbH                 EN-CONFIG-A+W Enterprise EDI.docx                             246

