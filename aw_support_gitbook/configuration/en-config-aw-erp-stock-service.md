---
title: "EN CONFIG A+W ERP Stock Service"
category: "configuration"
product: "A+W ERP Stock Service"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W ERP Stock Service"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration Instructions   A+W ERP Stock Service                                                                           english        A+W Software GmbH   EN-CONFIG-A+W ERP Stock Service.docx   - -INTERNAL-                                                                       1 Change history           Date        Author                Remarks                                    Version         2013-06-25 SVH                    Original version                           1.0"
source_file: "EN-CONFIG-A+W ERP Stock Service.pdf"
---


# EN CONFIG A+W ERP Stock Service

         Configuration Instructions


A+W ERP Stock Service




                                                                      english




   A+W Software GmbH   EN-CONFIG-A+W ERP Stock Service.docx   - -INTERNAL-
                                                                      1
Change history


        Date        Author                Remarks                                    Version
        2013-06-25 SVH                    Original version                           1.0
        2015-09-21 SVH                    Adjustment (AWDesk #338820)                1.1
        2017-03-15 SVH                    Chapters were re-arranged
        2018-03-16 SVH                    Lisec Interface (AWDesk #391319)
        2018-03-20 SVH                    AWE XTV feedback
        2018-06-04 SVH                    AWE XTV feedback
                                          Error during establishment of
        2018-08-16 SVH                    connection to the Hegla server
                                          Configuration of the cover sheet stock
                                          Addition to the documentation
        2019-04-02 SVH
                                          (#443136)
                                          Addition of problem handling
        2019-05-13 SVH
                                          (#443136)
                                          Addition to the documentation
        2019-08-26 SVH                    (#443136)
                                          -> a Hegla server counts as one stock
                                          Addition
        2019-09-04 SVH                    WL_KEINE_NEGATIVEN_BESTAENDE
                                          (#443136)
                                          STOCK_HEGLA_IGNORE_THICKNESS
        2019-12-04 SVH
                                          (#453768)
                                          PO logic (only AWE and only in
        2022-04-06 SVH                    connection with Hegla stock)
                                          [AW-76610]
                                          Notes about the documentation,
        2022-12-08 SVH
                                          reference to other documents
                                          In the Bystronic particularities, the
                                          documentation of the
        2023-01-24 SVH                    WL_PORT_COSTUNIT* variables was
                                          removed since this document was
                                          incorrect. The variables were not valid.
                                          Information about the Lisec stock
        2023-02-02 SVH
                                          system
                                          Differentiation of the "ERP Stock
        2023-02-08 SVH
                                          Service"



A+W Software GmbH            EN-CONFIG-A+W ERP Stock Service.docx                              2
        Date        Author                Remarks                                   Version
        2023-03-22 SVH                    [AW-135791] – Lisec connection
                                          [AW-147994] - Expansion of the docu
        2023-06-26 SVH
                                          for PO logic
                                          [AW-147159] – Lisec-connection – Info
        2023-07-20 SVH
                                          email
        2023-09-12 SVH                    [AW-157440] – Socket communication
                                          [AW-161492] – Hegla – time stamp of
        2023-12-06 SVH
                                          the last booking
                                          Additions: "inventory type", " No valid
        2024-01-15 SVH                    variant ID found", E-Mail, Panorama,
                                          order logic – open POs
                                          [AW-143894] – Activation/deactivation
        2024-01-26 SVH
                                          of the cyclical reconciliation
                                          [AW-171618] – AWB – Comparison
        2024-03-05 SVH                    with use of imperial dimensions in
                                          AWB
        2024-04-23 SVH                    Overview of used Hegla telegrams
                                          [AW-192587] – AWE – Booking and
        2024-05-29 SVH                    comparison for discontinued articles
                                          allowed.
                                          [AW-198448] - No external inventory
        2024-07-04 SVH
                                          for ERP item announced
                                          [AW-198448] – Lisec – treatment of
        2024-07-19 SVH
                                          glass types with inventory "0"
                                          [AW-199683] – treatment of PO items
        2024-07-23 SVH
                                          without third-party product code
                                          [AW-199683] – treatment of incorrect
        2024-07-25 SVH                    details in the "OrderListReference" in
                                          the "OrderListEntryBooked" telegram
                                          [AW-217449] – Verification of the
        2025-02-18 SVH
                                          connection to the external stock
                                          [AW-230073] – Goods receipt in the
        2025-06-10 SVH
                                          ERP system – change in the logic




A+W Software GmbH            EN-CONFIG-A+W ERP Stock Service.docx                             3
Content

1.   General information                                                 8
     1.1. Differentiation                                                9
     1.2. Availability                                                   9
     1.3. Benefits                                                       9
     1.4. Documentation                                                 12
                 Start-up with A+W Business                             12
                 Start-up with A+W Enterprise                           12
2.   General Installation                                               13
     2.1. Operating Systems                                             13
     2.2. Execution of the Config Tool                                  13
     2.3. Licensing                                                     13
3.   Installation with A+W Enterprise                                   14
     3.1. Bystronic connection with ALCIB 2011                          14
                  Installation of ALCIB stock                           14
4.   General Configuration                                              15
     4.1. Multi-site systems                                            15
     4.2. Socket communication                                          15
     4.3. Cyclical stock reconciliation (deactivation)                  15
     4.4. Special Features of Hegla Connection                          16
                 Configuration of the DB settings in the Config Tool    16
                 Configure the Hegla Connection in the Config Tool      16
     4.5. Special Features of Lisec Connection                          18
                 Configure the Lisec Connection in Config Tool          18
5.   Configuration with A+W Enterprise                                  20
     5.1. Environment variables                                         20
                 WL_PORTALLAGER                                         20
                 AWC_ALCIB_SERVER_NAME                                  20
                 AWC_PORT_CONTROL_SERVER                                20
                 WL_KEINE_NEGATIVEN_BESTAENDE                           20
                 STOCK_HEGLA_IGNORE_THICKNESS                           20
     5.2. Configuration of the Stock Booker                             21
     5.3. Master Data                                                   22
                 Third-party stock market partner                       22
                 Third-party item numbers                               22
                 Article Caching                                        22
                 Glass thicknesses                                      22
                 Determination of the AWE variant number                23
                 Portal stocks                                          23
                 Cover sheet stocks                                     24
                 Inventory change marker                                24
     5.4. XTV feedback                                                  24
     5.5. Special features of Hegla connection                          25
                 PO logic (Hegla goods receipts based on the AWE POs)   25
     5.6. Special features of Bystronic connection                      25
                 Master Data                                            25
6.   General Function Description                                       26

A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx         4
     6.1. Logging                                                                           26
     6.2. Sending e-mails                                                                   26
     6.3. GR stock logic                                                                    26
                  General                                                                   26
                  Configuration                                                             26
                  Process                                                                   27
     6.4. Special treatment of cover sheets                                                 27
     6.5. Cyclical stock reconciliation                                                     28
                  Behavior in case of non-processed records in the booking queue (wlh)      28
                  Treatment of negative stocks (see also #364470, #344044)                  28
                  ERP variants without external correspondence – " No external inventory for ERP
           item announced"                                                                  28
                  Error handling                                                            29
     6.6. Restrictions                                                                      29
                  XTV coupling                                                              29
                  Cyclical stock reconciliation                                             29
                  Inventory of portal stocks                                                29
                  Variable variants                                                         30
     6.7. Error handling                                                                    30
     6.8. License query                                                                     30
     6.9. Special features of Bystronic connection                                          30
                  IG stock logic                                                            30
                  OrderListRequest/OrderList/BookData telegram                              31
                  UnBookData telegram                                                       31
                  Cyclical stock reconciliation                                             31
                  Restrictions                                                              31
     6.10. Particularities of the Hegla stock connection                                    32
                  IG stock logic                                                            32
                  Booking the goods receipt                                                 32
                  Booking types (Hegla InventoryType)                                       33
                  Re-booking previously unbooked stock removals                             34
                  Time stamp of the last booking made                                       35
                  Special treatment of cover sheets (AWDesk #371602)                        36
                  Treatment of broken glass (AWDesk #371602)                                36
                  Handling of residual plates                                               37
                  Treatment of glass thicknesses (AWDesk #461784)                           37
                       Checking the connection to the Hegla server (AWDesk #459484, PF [AW-
           41702]) 38
                       PO logic [AW-76610]                                                  38
                       Restrictions                                                         38
                       Overview of used telegrams                                           39
     6.11. Particularities of the Lisec stock connection                                    40
                  Functional characteristics                                                40
                  Special treatment of cover sheets                                         41
                  Handling of residual plates                                               41
                  Treatment of broken glass                                                 41
                  Info e-mail                                                               42
                  Restrictions                                                              42
                  Information about the Lisec stock system                                  43
7.   Function description with A+W Enterprise                                              44


A+W Software GmbH              EN-CONFIG-A+W ERP Stock Service.docx                                5
     7.1. Process diagram                                                                   44
     7.2. Multi-site systems                                                                44
     7.3. Table wlportalsync                                                                44
     7.4. Table wlportalwewait                                                              45
                 Status values of the table wlportalwewait                                  46
     7.5. Tracing the bookings                                                              47
     7.6. Cyclical stock reconciliation                                                     47
                 Booking price                                                              47
                 Handling of incorrect booking records                                      47
     7.7. PO logic (only Hegla connection) [AW-76610]                                       48
                 General description                                                        48
                 Installation                                                               51
                 Configuration                                                              52
                 Open POs and "order list"                                                  54
                 Booking the goods receipt                                                  55
                 Booking the goods receipt in the ERP system                                55
                 "OrderListRequestResult" telegram                                          57
                 Overview using case descriptions                                           57
                 Error handling                                                             59
                 Restrictions                                                               60
                 Search                                                                     61
     7.8. Particularities of the Lisec stock connection                                     63
                 Treatment of glass types with inventory "0"                                63
8.   FAQs                                                                                   64
     8.1. Conversion of an existing stock to a portal stock                                 64
     8.2. Cover sheets                                                                      64
     8.3. Correct inventories and average prices                                            64
     8.4. Installations with A+W Business                                                   67
                  Tables and processes in A+W Business                                      67
                  Use of imperial dimensions in A+W Business                                67
     8.5. awtrc log of the ERP Stock Service                                                68
                  Orientation in the log                                                    68
                  PO/Goods receipt logic (Hegla, TechNord, Planning Stock)                  68
                  "inventory type" logging                                                  69
                  "Panorama" logging                                                        69
     8.6. Hegla log                                                                         69
     8.7. Measurement                                                                       69
     8.8. Verification of the connection to the external stock                              70
9.   Troubleshooting                                                                        71
     9.1. General                                                                           71
                  Installation via the SetupLauncher                                        71
                  Host name of the external stock server cannot be resolved by the Stock Service
          in the IP address                                                                 71
                  E-mails are not sent                                                      71
                  E-mails from the cyclical stock reconciliation seem to be sent twice      71
                  In the ERP system, no more bookings are made                              71
     9.2. General - A+W Enterprise                                                          73
                  Records with error status "-4" before the stock booker block the cyclical
          comparison                                                                        73


A+W Software GmbH              EN-CONFIG-A+W ERP Stock Service.docx                                6
               Records before the stock booker block the cyclical comparison               73
               Variant is not found in AWE: "No valid variant ID found"                    73
               AWE articles are not found                                                  73
   9.3. General - A+W Business                                                             74
               Cyclical reconciliation causes incorrect inventory                          74
   9.4. Hegla connection                                                                   74
               The Stock Service cannot establish a connection to the Hegla stock server 74
               Problems with connection data                                               74
               Problem with the Hegla interface version                                    74
               LogOn                                                                       74
               During communication with the Hegla server, there is a timeout              75
               Error when parsing the Hegla telegram                                       75
               A booking is rejected because it supposedly has a time stamp that is too old.78
               Store Balance - No external inventory for ERP item announced                79
               Apparently deviating quantities in ERP and Hegla                            79
               PO logic: empty order list in Hegla                                         79
               PO logic: open POs missing in the Hegla display                             80
               PO logic: good receipts from Hegla do not arrive in the ERP Stock Service 80
               PO logic: goods receipts from Hegla include a corrupt OrderListReference and
        can therefore not be booked in the ERP Stock Service                               80
               PO logic: log message "Error code 6, message: Authentication failed."       81




A+W Software GmbH            EN-CONFIG-A+W ERP Stock Service.docx                                7
1. General information
A+W ERP Stock Service is a module for reconciling a third-party stock with an A+W ERP stock.
Possible third-party stocks are currently Bystronic, Hegla, and Lisec stocks.
Via the corresponding configuration in the Config Tool of the ERP Stock Service, the link is
established between the third-party stock and ERP stock.
Because the communication of the third-party stocks with the ERP Stock Service relies on
different transfer protocols depending on the manufacturer, the configuration in the Config Tool
must be done a little differently:
->   In the Bystronic system, the stock numbers of the connected ERP stocks are known. Each
     transfer protocol of the Bystronic server includes the ERP stock number for which the
     protocol is sent; therefore, one Bystronic server can be linked to several ERP stocks.
->   In the Hegla system, the stock number of the connected ERP stock is not known. As a result,
     transfer protocols of the Hegla server do not include any ERP stock number; therefore, a
     Hegla server can only be linked to precisely one ERP stock.
->   In the Lisec system, the stock number of the connected ERP stock is not known. As a result,
     transfer protocols of the Lisec server do not include any ERP stock number; therefore, a Lisec
     server can only be linked to precisely one ERP stock.


Here, the assignment information is presented again in the form of a table:
      System                    Assignment                      Remark
                                Third-party server - ERP
                                stock
      Bystronic connection      1:n                             ERP stock numbers known in the
                                                                Bystronic server
      Hegla connection          1:1                             ERP stock number unknown in
                                                                the Hegla server.
                                                                Exception: GR stock logic, see
                                                                special description, Chapter 6
      Lisec connection          1:1                             ERP stock number unknown in
                                                                the Lisec server.




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                               8
1.1. Differentiation
The A+W ERP Stock Service may not be confused with other A+W programs that also have the
term "Stock Service" in their names.
    •   A+W Planning Stock Service
        More precisely: A+W Production Planning Stock Service
        This service is used in the production environment. With this service, the Residual Stock
        Manager (manual residual lite management) and Remaster (automatic residual
        management - Remaster is a Hegla brand name), data about residual lites is called up
        from the SOA database.
    •   A+W Commercial Stock Business Service
        More precisely: A+W Commercial Business Smart Companion Stock Service
        This service is only used by A+W Business.
    •   (Linux) Stock Service
        More precisely: Linux Enterprise Stock Service
        This service is only used by A+W Enterprise. It provides the data for the Smart Companion
        and the CX stock forecast.




1.2. Availability
The Stock Service 5 can be operated with the ERP programs ALCIB 2011 and A+W Enterprise 5.
Starting with Version 6, the Stock Service can also be made available for A+W Business.


1.3. Benefits
Ideally, the Stock Service results in a more precise inventory in the ERP glass stocks.
With the previous outward booking methods, the glass stocks (for belt dimensions) are subject to
a certain imprecision in the ERP systems. The previous outward booking methods are:
    •   Automatic outward booking for delivery note creation
    •   Automatic outward booking for completion reports from production
    •   Automatic outward booking based on prediction data
    •   Automatic outward booking for XTV report
    •   Manual outward booking
All outward booking processes have limitations with respect to the Stock Service.
    1. Automatic outward booking for delivery note creation:
            a. The quantities to be booked are calculated from the dimensions of the delivery
               note items (with cutting and correction factors, only approximate values are
               possible).
               In order to consider that only complete stock dimensions can be withdrawn from
               physical stock, in the ERP stock, a variable variant is used for the booking. (in


A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                               9
              practice, however, it has become clear that the complexity of the logic sooner
              scares customers off.)
          b. Breakage is not considered.
          c. If there is a long period between production and delivery of an order, there can
             be a similarly large time difference between the actual removal from physical
             stock and the outward booking of the corresponding inventory from the ERP
             stock.
          d. No automatic stock reconciliation can be performed during which the inventory in
             the ERP stock is reconciled with the inventories in the physical stock.
          e. No support of stock management due to lacking interplay with the stock
             prediction.


   2. Automatic outward booking for completion reports from production:
          a. The quantities to be booked are calculated from the dimensions of the glass to be
             produced (with cutting and correction factors, only approximate values are
             possible).
             In order to consider that only complete stock dimensions can be withdrawn from
             physical stock, in the ERP stock, a variable variant is used for the booking. (in
             practice, however, it has become clear that the complexity of the logic sooner
             scares customers off.)
          b. Breakage is not considered (or is there a switch for this?)
          c. No automatic stock reconciliation can be performed during which the inventory in
             the ERP stock is reconciled with the inventories in the physical stock.
   3. Automatic outward booking based on prediction data:
          a. The quantities to be booked are calculated from the dimensions of the order
             items (with cutting and correction factors, only approximate values are possible).
             In order to consider that only complete stock dimensions can be withdrawn from
             physical stock, in the ERP stock, a variable variant is used for the booking. (in
             practice, however, it has become clear that the complexity of the logic sooner
             scares customers off.)
          b. For large orders that are produced across a longer period, there is imprecision in
             the outward booking if for the order items no item split is executed or if there is
             no rescheduling.
          c. The outward booking is done in a nightly routine and considers only the
             preliminary production date and not the actual cutting date.
          d. No automatic stock reconciliation can be performed during which the inventory in
             the ERP stock is reconciled with the inventories in the physical stock.
   4. Automatic outward booking for XTV report:
          a. No automatic stock reconciliation can be performed during which the inventory in
             the ERP stock is reconciled with the inventories in the physical stock.
          b. No support of stock management due to lacking interplay with the stock
             prediction.



A+W Software GmbH             EN-CONFIG-A+W ERP Stock Service.docx                              10
             c. A manual removal for hand cutting or trade is not considered.
    5. Manual outward booking:
             a. There is no timely booking, generally booking is done once a day.
             b. Error due to incorrect entries are possible, either directly during the entry of the
                booking record or at the cutting tables, where lists with item numbers and
                quantities must be kept.
             c. No automatic stock reconciliation can be performed during which the inventory in
                the ERP stock is reconciled with the inventories in the physical stock.
With the use of the Stock Service:
    •    Timely outward booking is guaranteed (the booking is done precisely at the moment at
         which the lite is removed from the physical stock)
    •    Following from this, the precision of the inventory data in the ERP stock is increased
    •    Following from this, an effective materials management (material flow, order generation)
         is supported
    •    The stock management provides more accurate values at all times than all other outward
         booking methods
In the Stock Service, a daily stock reconciliation can be configured, which ensures that all
differences in the inventories that can occur due to careless GR booking are eliminated. The
inventories of the ERP stock are thus compared to the inventories of the physical stock. Leading
here is the physical stock.
If the customer was previously forced to execute a stock inventory at short intervals (once a
month) in order to determine the inventories and update them, this interval can now be extended
and thus the amount of work reduced.
For customers with a long inventory interval (e.g. once a year), the Stock Service automatically
produces much greater security in the inventory of the ERP stock.
The Stock Service can be configured very flexibly depending on customer needs. It is multi-site
capable, it can connect several external stocks and even different external stock systems (Hegla
and Bystronic).


Notes:
    •    In order to maintain precision of the average prices in the ERP stock, it is important that
         the customer books inward goods in the ERP in timely fashion. Unbooked inward goods in
         the ERP stock mean that the unbooked quantities are corrected with the daily stock
         reconciliation, whereby the inward booking is done at the current average price.


Special notes for A+W Enterprise:
    •    Stock forecast:
         The forecast data for a portal stock is adjusted using a current stock booker (version >=
         13.04.0634) and activation of XTV feedback for the portal stock.
         For XTV feedback, in this configuration, the prediction data is adjusted by the ERP
         Webservice in cooperation with the alrpc service.
         See chapter "XTV feedback."


A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                11
        If a stock booker < Version 13.04.0634 is used, the adjustment of the forecast data for a
        portal stock CANNOT be done by the XTV feedback.
        The XTV feedback for the portal stock has to be deactivated in any case. An adjustment of
        the forecast data has to be built in via customizing.




1.4. Documentation
         Start-up with A+W Business
The general configuration/functionality is described in this document.
The AWB-specific configuration/functionality is not described in this document.
Consult the general A+W Business configuration documentation for additional information.
For the configuration of the ERP Stock Service in the Config Tool, please consult the associated
installation instructions.



         Start-up with A+W Enterprise
The general and AWE-specific configuration/functionality is described in this document.
For the configuration of the ERP Stock Service in the Config Tool, please consult the associated
installation instructions.




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                               12
2. General Installation
There is a special installation instruction available at:
\\jupiter\SW_Install\<version>\InstallationDocumentation
It is available in SetupLauncher when the complete SW_Install directory is delivered for
installation.


2.1. Operating Systems
The Stock Service is approved for the server systems:
    •    Windows Server 2008 R2
    •    Windows Server 2012
    •    Windows Server 2012 R2


2.2. Execution of the Config Tool
See installation instructions.


2.3. Licensing
The installation of a LicenseClient on the server on which the Stock Service is running is necessary.
The Stock Service can only be operated with a valid license. A separate license must be available
for each third-party stock type.
 Third-party stock type       License module
 Bystronic                    App=2300; BA=1; ED=2300; Ver=2012; Modul=1
 Hegla                        App=2300; BA=1; ED=2300; Ver=2012; Modul=2
 Lisec                        App=2300; BA=1; ED=2300; Ver=2012; Modul=3




A+W Software GmbH                 EN-CONFIG-A+W ERP Stock Service.docx                            13
3. Installation with A+W Enterprise
3.1. Bystronic connection with ALCIB 2011
Attention. The following steps are only necessary in ALCIB Version 2011!


         Installation of ALCIB stock
       1. Install a current wlager binfile (buildnr > 776).
       2. Bring the database up to the correct status. Execute the SQL script from the
          installation directory of the ALCIB Version 2013
          "xsql/12/1/0/120100008_wlraum_sql" or execute the following update
          statement:
          "ALTER TABLE wlraum ADD (welnr INTEGER DEFAULT 0);"
       3. Add files to the stock area. The files must be retrieved from the appropriate
          language version ALCIB 2011. The following files must be installed:
               a. $PRG/lager/mfo/wlraump.mfo
               b. $PRG/lager/pan/wlraump.pan (language-dependent)
               c. $PRG/lager/sel/wlraum_welnr.sel (language-dependent)
               d. fx_texte/messages (language-dependent, date > 12.10.2011)
       4. Create the ALCIB environment variable WL_PORTALLAGER and activate it with
          "ON".




A+W Software GmbH              EN-CONFIG-A+W ERP Stock Service.docx                       14
4. General Configuration
4.1. Multi-site systems
As far as we know, there is (as of 03/29/22) no multi-site installation where several ERP multi-site
sites "talk" to stocks with third-party stock connection. The multi-site capability of the ERP Stock
Service is not guaranteed in such an installation.




4.2. Socket communication
Communication between a third-party stock and the ERP Stock Service takes place via a socket
connection.
The socket interface used by the ERP Stock Service (Panorama interface) accesses the port range
of the free dynamic ports on the customer system.
Thus, it is the customer's responsibility to determine which ports are available to the ERP Stock
Service for communication by configuring the dynamic port range.
Caution: It is also the customer's responsibility to ensure that the ports of the dynamic port range
are not blocked even in the firewalls and the routers that are located between ERP Stock Service
and the third-party stock server.
Note: In the configuration with a Hegla warehouse, in addition to the IP address of the Hegla
server, a port number (by default "10010") is also stored for communication. This combination of
IP and port is used by the socket interface to define the remote target system; beyond that, the
port number stored here has no meaning.
The port for the local system is still taken from the dynamic port range during communication.
netstat example (on the client computer / computer of the ERP Stock Service):
TCP 192.168.11.22:49876 192.168.33.44:10010 SYN_GESENDET
    -   the port „49876“ comes from the dynamic port range
    -   the port „10010“ comes from the configuration of the Hegla connection in the ERP Stock
        Service


See also PF [AW-157440].




4.3. Cyclical stock reconciliation (deactivation)
The cyclical stock reconciliation is a core component of external stock incorporation.
Since in individual cases it can nevertheless be necessary not to conduct this reconciliation
cyclically, it is possible via the Config Tool to deactivate the functionality.
The deactivation is done separately for each external stock type (Hegla, Lisec, Bystronic). Within a
stock type, the setting applies for all connected stocks.


A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                              15
See PF [AW-143894].




4.4. Special Features of Hegla Connection
           Configuration of the DB settings in the Config Tool
The configuration is described completely in the installation document. Here, an excerpt of this is
reproduced, which is required for the PO logic. (The detailed description of the PO logic is also
found in the separate chapter "Function description with A+W Enterprise".)
Checkbox „Use AWSOA“
Using the AWE purchaseservice
AWSOA Login Name
User for the use of the AWE purchaseservice, the stored name must exist in the AWE employee
master as login name (mitarb.loginname)
AWSOA Multisite ID
Client number of the purchaseservice in case of a multisite installation, the client numbers
available for selection are displayed in the drop-down menu of the field.
Date Range Into Past (days)
The number of days to search for open purchase orders in the past, starting from the current
date, is entered.
Date Range Into Future (days)
The number of days to search for open purchase orders in the future, starting from the current
date, is entered.



           Configure the Hegla Connection in the Config Tool
Stock ID
Per "Hegla communication," only one stock ID can be stored. That is, for each AWE portal stock, a
separate "Hegla communication" must be created.
From the point of view of the ERP system, a Hegla server represents precisely one Hegla stock. It
can be connected/synchronized with precisely one ERP stock in the configuration.
The configuration of several ERP stocks with one and the same Hegla servers by generating
several entries in the connections that only differ in the Client ID (but address the same Hegla
server, with the same IP and the same port), is NOT permissible.
Cover Sheet Stock ID
By specifying a cover sheet stock (stock number > 0), it is possible to configure a connected cover
sheet stock for a portal stock.
The defined stock number specifies the cover sheet stock. For stock number > 0 the developed
special logic (AWDesk #371602) for cover sheet applies. All cover sheets are booked to the cover
sheet stocks indicated here.



A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                               16
CAUTION: Each portal stock must be assigned a separate (exclusive!) cover sheet stock. It is not
possible that several portal stocks can share one cover sheet stock. If two portal stocks were
assigned to the same cover sheet stock, during the cyclical stock reconciliation, incorrect
inventories would arise.
Stock MP
Via a special stock market partner, the item numbers of the Hegla stock items are mapped to the
ERP item numbers. In different "Hegla communication" entries, the same stock market partner
can be used.


Interface Version
Hegla interface versions 2.1.0.0 or higher are supported.
If the customer has an interface subversion 2.1.x.y, „2.1.0.0“ must be selected in configuration.


The GR stock logic can only be activated with an interface version 2.2.0.0 or higher.
If the customer has an interface subversion 2.2.x.y, „2.2.0.0“ must be selected in configuration.


The stock logic can only be activated with an interface version 2.3.0.0 or higher.
If the customer has an interface version 2.3 or higher, „2.3.0.0“ must be selected in configuration.


Port number
Information from Hegla (Mr. Ridder, 2013-08-21):
The port number, via which the stock server communicates on the server system, is 10010 by
default and should be the same for all connected stocks.
For more information on ports, see also the separate chapter "Socket communication".
Client ID
Information from Hegla (Mr. Ridder, 2013-08-21):
With the client ID, it is communicated to the Hegla server which client is connecting to it. Even if
several "Hegla communication" records exist, the same client ID is entered in each one since from
the point of view of the Hegla server, the same client (ERP Stock Service) always connects.
The configuration of several ERP stocks with one and the same Hegla servers by generating
several entries in the connections that only differ in the Client ID (but address the same Hegla
server, with the same IP and the same port), is NOT permissible.
Generally, the client ID "1" can be used.
Measurement
Measurement unit during communication, presently just in "mm".
Ignore Broken Glass
Normally, this checkbox should not be checked. The treatment of breakage in Stock Service was
corrected with AWDesk #371602. Broken glass will be taken over into the ERP inventory during



A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                                17
the cyclical reconciliation. The inventory will be reduced if a breakage booking is reported from
the Hegla stock.
But if for some reason a customer cannot work with the corrected logic, check the checkbox and
the Stock Service will handle breakage as before the correction. Broken glass will be ignored both
during the cyclical reconciliation as well as during the breakage reports.


Allow Inward Stock Booking
The "Allow inward stock booking" checkbox must be enabled if the PO logic or GR stock logic is
used. If the checkbox is not enabled, the bookings that are sent by the third-party stock with the
telegram "OrderListEntryBooked" are rejected by the ERP Stock Service.




4.5. Special Features of Lisec Connection
         Configure the Lisec Connection in Config Tool
Interface Version
Configuration instructions
 Lisec interface version of the     Lisec version to be             Remark
 Lisec server                       configured in the A+W ERP
                                    Stock Service Config tool
 2.71 or higher (in this version    2.71                            "2.71" is the oldest of the
 nomenclature)                                                      versions listed here
 02.00.000 to 02.00.006             02.00.000                       Current versions use the
                                                                    notation "02.00.000" or
                                                                    "02.x.y"
 02.00.007 or higher                02.00.007                       see above


See also PF [AW-135791] and [AW-220804].


Client Name
The entered "Client Name" is an agreement on the name between the Lisec system and the ERP
Stock Service. The name can be selected at will, but must be known to the Lisec system.
Via the name, it is ensured in the Lisec system that only telegrams are sent to the client that are
suited for it.
See also PF [AW-135791].


Port number
Lisec must provide the port number to be used.
Measurement


A+W Software GmbH                  EN-CONFIG-A+W ERP Stock Service.docx                               18
Measurement unit during communication, presently just in "mm."
Cover Sheet Stock ID
See chapter "Configuring the Hegla Connection in Config Tool"




A+W Software GmbH              EN-CONFIG-A+W ERP Stock Service.docx   19
5. Configuration with A+W Enterprise
5.1. Environment variables
          WL_PORTALLAGER
In Version ALCIB 2011 (4.5), the env variable WL_PORTALLAGER must be activated so that the
portal stock logic is activated. The variable is only present in Version 2011. It serves as protection,
since for the use of the portal stock logic, the dialog for storage space management (wlraum)
must be adjusted.
Starting with Version AWE 5 (12.1) the logic is no longer clipped via WL_PORTALLAGER.


          AWC_ALCIB_SERVER_NAME
The variable must contain the name of the AWE (Unix/Linux) server.


          AWC_PORT_CONTROL_SERVER
In the variables, it must be stored on which port the Stock Service can communicate with the AWE
background processes.


          WL_KEINE_NEGATIVEN_BESTAENDE
This variable must be set in order to prevent bookings from external stock from creating negative
stock in the ERP stock.
If the variables are set, stock bookings that would lead to negative stock are rejected by the stock
booker and only processed after the next incoming booking.


          STOCK_HEGLA_IGNORE_THICKNESS
If the variable is active, the thickness of the Hegla article is not taken into account when searching
for the mapped article in the AWE stock. Mapping can only work if there are no thickness
variations in the Hegla system for article numbers.
The logic only works if an AWE stock is linked to a Hegla stock. For a link with A+W Business or for
other third-party stocks (Bystronic, Lisec), the logic is not made available. (AWDesk #453768)
With AWDesk #461784, with the "Ignore Thickness" checkbox in the Config Tool, it is possible to
not consider the glass thicknesses for article mapping in the Hegla stock connection. If the
checkbox is activated, the logic applies both in the connection with A+W Enterprise as well as with
A+W Business.
For the connection to A+W Enterprise, there is no hierarchy in the configuration. If either the
variable STOCK_HEGLA_IGNORE_THICKNESS or in the Config Tool the "Ignore Thickness"
checkbox is activated, the glass thicknesses are not considered during article mapping.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                20
5.2. Configuration of the Stock Booker
In order to specify the message recipient for system messages from the stock booker, the AWE
environment variable WL_MELD_EMPF must be activated. If the variable is not active, the system
messages are sent to the respective recorder of the stock booking. In the case of the Stock
Service, the recorder of bookings is always the user ID -1 (system). Messages go to the e-mail
address stored in the employee master data.




A+W Software GmbH             EN-CONFIG-A+W ERP Stock Service.docx                          21
5.3. Master Data
         Third-party stock market partner
Via the Master data > Market partner dialog, a special market partner of the type "Other" must be
created, which represents the stock connection to a particular third-party stock (Bystronic, Hegla,
or Lisec). Via this market partner, the third-party item numbers are assigned in the stock
connection below.


         Third-party item numbers
Via the Master data > Articles > F4 > Market partner details dialog, the third-party item numbers
of the connected stock must be assigned to the appropriate AWE article numbers. As market
partner, the previously-created third-party market partner is entered.
CAUTION:
Several entries for which different external article codes are assigned to one and the same AWE
article number are not permissible.
The determination of the external article code would then not be unambiguous when creating the
"OrderList"!


Hegla stock incorporation
Attention: doubled third-party item numbers for a third-party stock market partner (in artkuzu)
are permissible. Since the third-party article is defined by the combined key (item code, thickness
of the glass, height of the glass, width of the glass), an item code in artkuzu can be assigned to
several AWE article numbers.


Bystronic stock incorporation
No thickness information about the lites is transferred by Bystronic. Here, a Bystronic item
number must be assigned to precisely one AWE item number.


         Article Caching
Article/variant master data from AWE is cached in the Stock Service. After a change in the AWE
variant data, therefore, the Stock Service must be restarted so that the changes take effect.


         Glass thicknesses
Hegla stock incorporation
Since for the assignment of the Hegla article number to the AWE item number the glass thickness
transmitted by Hegla is part of the key, the glass thicknesses must be maintained correctly in AWE
(artikel.staerke), that is, they must match the Hegla glass thicknesses.




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                             22
         Determination of the AWE variant number
For the determination of the AWE variant number using width and height, the stored procedure
wlgetbitnur is called within the Stock Service. It determines the variant number
(artvarzu.bitnr/xxvar.bitnr) in the standard version delivered by A+W using the dimensions
transmitted taking into consideration a Delta range.
The ERP Stock Service and the A+W Enterprise Stock Booker interpret the return value of the SP
wlgetbitnr in the same way: a variant counts as determined if the return value of the SP > 0. The
return value corresponds to the variant number in A+W Enterprise.
Return values <=0 mean that no variant was found.
With PF [AW-135791] the logic for determining the AWE dimensional variant was adapted so that
in addition to the exchanged dimensions of width and height, an appropriate variant is searched
for if no variant with the original values could be found. This logic is not included in the SP
wlgetbitnr, but in the logic called up in the ERP Stock Service.
The logic was generally adjusted and affects all stock connections (Hegla, Lisec, and Bystronic).
Whether the same logic exists in AWB is not known at this point.


Digression:
Description of the logic in the standard version of the SP wlgetbitnr delivered by A+W
The return value of the SP is a numeric value.
A positive return value (>0) corresponds to the variant number determined in A+W Enterprise.
A return value <=0 means that no variant was found.
In the standard version of the SP wlgetbitnr, first there is a search for a variant with a dimension
Delta of 20 mm. If with this dimension Delta a variant is found, then this variant number will be
returned.
If no variant is found, the Delta is increased to 200 mm and then searched for again. If a variant
with the increased Delta is found, the variant number is delivered back as a negative value.
If no variant is found with the larger Delta, the value "0" is returned.
It is no longer possible to trace where the logic in wlgetbitnr that searches with the increased
Delta for a variant and in case of a hit returns the negative variant number comes from (status as
of 08/24/2024).
Important is that both the AWE Stock Booker and the ERP Stock Service ignore this negative
variant number and interpret any return value <=0 as "Variant not found".
The SP wlgetbitnr can be adjusted on the customer system according to the customer's wishes at
any time. Attention must only be paid that only positive return values count as variant numbers
found.



         Portal stocks
The third-party stock-connected AWE stocks must be marked as portal stock in the master data.
When creating a portal stock on the stock dialog Master data > Room, the stock type "normal"
must be specified for the stock and the toggle value "portal stock" selected in the field interface.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                              23
The specification of an IG stock may only take place if the user would like to work with the GR
stock logic of the Bystronic stock connection. For inward goods for a portal stock, the entry of an
GR stock causes automatic steering of the inward goods to the IG stock entered.
Configuration of GR stocks
In order to set up an interface stock on the stock room management dialog (STOCK > Master data
> Room), proceed as follows:
1. Set up a corresponding inward goods stock for the interface stock to be created. A inward
goods stock must be created as shelf stock. A GR stock will be assigned an interface stock in a 1:1
assignment. This means that precisely one GR stock belongs to an interface stock. The GR stock
cannot be assigned to a second interface stock.
2. Now define the interface stock. In the GR stock field of the interface stock, the stock number of
the corresponding IG stock must be specified.
Prevention of the automatic booking of prediction data
The marking of a stock as portal stock (interface: "portal stock") prevents the automatic outward
booking from stock based on the prediction data (wlppms table) within the nightly stock routine.


         Cover sheet stocks
The configuration of a cover sheet stock that differs from a portal stock can only be done in the
Hegla stock connection. In AWE, the cover sheet stock is created as "normal stock."
Each portal stock must be assigned a separate (exclusive!) cover sheet stock. If two portal stocks
were assigned to the same cover sheet stock, during the cyclical stock reconciliation, incorrect
inventories would arise.


         Inventory change marker
The inventory change marker has to be set to "AWP" for the stock articles kept in the portal stock;
this creates the forecast data using the calculated production date.
Attention: if the inventory change marker is set to "Delivery note/AWP," there can be doubled
bookings in the forecast data.


5.4. XTV feedback
With use of the Stock Service, previously the XTV reporting had to be deactivated since otherwise
removals from coupled stocks were made twice. As a result, the adjustment of the forecast data
coupled to it was also deactivated. This was changed with AWDesk #289178.
The XTV reporting - and thus the adjustment of the forecast data can now - with use of a current
stock booker (starting with build 13.04.0634) be used together with the Stock Service - for the
stock booker now checks the stock properties for removals with status 68 (PMS_ABGANG_EXT). If
the stock from which the removal should be made is a portal stock (WLRAUM.INTERFACE = 2), no
stock removal is made. In this case, the stock in question is a synchronized third-party stock that is
removed by the Stock Service. A corresponding entry in the stock booker log documents that this
removal is suppressed. The record is then deleted from the table wlh.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                               24
There is also a chapter on this topic in the "Enterprise Production Interface" configuration
instructions.




5.5. Special features of Hegla connection
         PO logic (Hegla goods receipts based on the AWE POs)
With a connected Hegla stock, the PO logic can be activated.
Here, the goods receipts are generated based on the open POs that exist in AWE. The logic is
described in detail in the special chapter "Function description with A+W Enterprise".




5.6. Special features of Bystronic connection
         Master Data
For the ByStore communication, it is necessary that all ALCIB tape measure and cover sheet
articles that should be booked into the ByStore interface stock be mapped to the appropriate
ByStore material number. The ByStore material number must be stored in the article master data
in the private fields (artikel.private_long1).




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                           25
6. General Function Description
6.1. Logging
The Stock Service protocol can be found in %PROGRAMDATA%\A+W\Log.


6.2. Sending e-mails
The Stock Service sends e-mails in order to inform about errors that have occurred. The sending
of an e-mail is recorded with a log entry in the Stock Service log (text "Send E-mail...", TraceLevel
"Info").
If no e-mail is received by the recipient although the sending is noted in the log and no error has
occurred, it must be checked whether the firewall is blocking the sending.


6.3. GR stock logic
         General
The GR stock logic was previously available in the Bystronic and Hegla stock connection. It was
conceived in order to prevent removals from the third-party stock being reported to the ERP
system by the Stock Service before the inward goods were booked in the ERP system. The
removal of lites from non-booked goods receipts results in incorrect inventories and incorrect
average prices.
In the respective third-party systems there is a logic that allows the removals for a goods receipt
only once the inward goods have been confirmed in the ERP stock. The query of the confirmation
starts with the third-party system.
The use of the GR stock logic is recommended in order to prevent incorrect inventories and
incorrect average prices. However, many customers decide against the logic nevertheless since
they feel restricted in the way they work by the forced confirmation of the ERP goods receipt.


         Configuration
The GR stock logic can only be used if, on the one hand, a GR stock is specified in the stock master
data for a portal stock configured in AWE and, on the other hand, the third-party stock system has
the appropriate logic to query the incoming goods.
Furthermore, the "Allow inward stock booking" checkbox must be enabled in the Config Tool if
the GR warehouse logic is used. If the checkbox is not enabled, the bookings that are sent by the
third-party stock with reference to the GR stock are rejected by the ERP Stock Service.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                               26
         Process
For the GR stock logic, for each goods receipt for a connected portal stock from a third-party stock
system, first the AWE incoming goods booking must be queried and confirmed before the goods
receipt stocks in AWE are finally booked to the portal stock.
The query for transferring the goods receipt stocks is initiated from the third-party stock system.
The query of the third-party system always refers to a stock order placed in AWE.
The flow of the handling of the goods receipt is designed as follows: upon the recording of the PO
in AWE, the goods are delivered sometime. The delivery note is compared to the PO. The included
cover sheets for the stacks are added to the PO after the fact. In case the purchase order is
already in local correction, this change however is only commercially relevant. While it is
transferred into the goods receipt, it cannot be transferred into the stock anymore due to the
status of the purchase order (local correction).
For the subsequent inward goods booking for the PO in AWE, the stock stored is analyzed for the
PO item. If the stock is an interface stock (interface = "portal stock"), the inward goods are
booked to the corresponding goods receipt stock (GR stock). The respective slot number is
composed of the order number and sub-number in the form "BBBBBBBB/SSS".
Here missing cover sheets can be booked manually via a slot inward booking into the respective
slot.
An automatic correction of cover sheets takes places through the nightly stock reconciliation.
After the goods receipt has been booked in the AWE GR stock, only then is it transferred to the
corresponding portal stock if the third-party stock system has queried the goods receipt via the
Stock Service and confirmed it.


6.4. Special treatment of cover sheets
The logic for special treatment of cover sheets (booking of the cover sheets to a separate cover
sheet stock) was previously only available in the Hegla stock connection.
In the ERP stock, cover sheets cannot be distinguished from normal lites. There is no marking that
identifies a cover sheet. For distinction, the lites can only be booked into different stocks in the
ERP system. A separate stock is configured for cover sheets.
The advantage of a cover sheet stock that deviates from the portal stock is thus that in the ERP
system the inventory of the portal stock is not falsified by cover sheets since under some
circumstances cover sheets may not even be available to production (e.g. due to low glass
quality).
Each portal stock must be assigned a separate (exclusive!) cover sheet stock. If two portal stocks
were assigned to the same cover sheet stock, during the cyclical stock reconciliation, incorrect
inventories would arise.
The flow for booking cover sheets is described in more detail in Chapter Special treatment of
cover sheets (AWDesk #371602).




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                               27
6.5. Cyclical stock reconciliation
The cyclical stock reconciliation ensures that the inventory of the ERP stock is synchronized with
the inventory of the third-party stock at least once a day. Here the third-party stock is the leading
stock. Ideally, the cyclical reconciliation determines that the inventories of both stocks are
identical. If this is not the case, the inventories of the ERP stock are reconciled with additions or
removals of the individual variants of the inventories in the third-party stock. All bookings are
made using the respective current average price.


       Behavior in case of non-processed records in the booking
     queue (wlh)
Before the stock reconciliation, the Stock Service checks whether there are records in front of
the stock booker for the current stock to be reconciled.
For non-processed records, the stock reconciliation waits for the processing. For security, in this
case the stock booker is started by the service.
If after 5 minutes there are still non-processed records in front of the stock booker, the
reconciliation is not performed for the complete current stock. Here it plays no role which
articles are affected by the non-processed records.
If an e-mail recipient is configured in the config tool, an appropriate notice is sent to him via e-
mail.
See also #330257


         Treatment of negative stocks (see also #364470, #344044)
There is no special treatment for negative stocks in the ERP stock.
If, for example, for a variant in the ERP stock the stock is -20 and the corresponding article in the
external stock indicates an inventory of 30, then the amount after the stock reconciliation will be
30.


        ERP variants without external correspondence – " No external
     inventory for ERP item announced"
During the cyclical reconciliation, the Stock Service queries the inventories of the connected third-
party stock. If no inventory is reported by the third-party system for an article that is kept in the
ERP stock (that is, no data record for this article is transmitted), the Stock Service cannot decide
whether the missing message for the inventory means that the inventory is 0 or whether there
was an error during the transmission. Therefore, in this case, the inventory is NOT changed in the
ERP system in this case.
In the log, a message with the following content is output: "No external inventory was
transmitted for the article variant X. The inventory of this variant in the ERP system will not be
changed."
An info is sent as e-mail in which the recipient is asked to check the master and transaction data
in the ERP stock.


A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                28
Message text in the original (English):
"No external inventory for ERP item announced (…): WARNING: No external inventory has been
announced for ERP item ID …, variant ID …, stock …, actual amount …. The amount won't be
changed automatically. Please review master data and stock data."



         Error handling
If during the stock reconciliation for an article an error occurs (e.g. no corresponding ERP article
data is found), the reconciliation for this article is skipped and continued with the next article.


Errors that cause a cancellation of the entire stock reconciliation are:

    •   Non-processed records in the booking queue during cyclical stock reconciliation => the
        stock reconciliation is not executed.
        Changed with #330257, for non-processed records, the stock reconciliation waits for the
        processing (but 5 minutes at most)

    •   Error records in the booking queue during cyclical stock reconciliation => the stock
        reconciliation is not executed.


6.6. Restrictions
         XTV coupling
With use of the Stock Service, it must be ensured that for the corresponding cutting tables, the
XTV coupling to this stock is deactivated, if the system works with stock booker version <
13.04.0634. With use of a stock booker from version 13.04.0634 on, the XTV coupling can be
deactivated.
See chapter "XTV feedback."


         Cyclical stock reconciliation
At the time of the stock reconciliation, all inward goods in the ERP stock and stock accesses in the
third-party stock must be matched to one another. If this is not the case, the deviating quantities
are booked as inventory difference, this has effects on the prices in the ERP stock.


         Inventory of portal stocks
With an external stock connection, it is essentially assumed that the external stock is the leading
stock (during cyclic reconciliation, the inventories in the ERP system are corrected based on the
data of the external stock).



A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                  29
The keeping of an inventory on the ERP side does not make sense for portal stocks. The nightly
stock reconciliation therefore does not check whether the stock for which the reconciliation is
executed is in inventory or not.


          Variable variants
Variable variants can’t be booked with this interface.


6.7. Error handling
Essentially for an error that has occurred, an e-mail is sent to the recipient stored in the
configuration.


Known errors are:

    •   No item mapping possible => The current booking is not executed.

    •   Non-processed records in the booking queue during cyclical stock reconciliation => the
        stock reconciliation is not executed.

    •   Error records in the booking queue during cyclical stock reconciliation => the stock
        reconciliation is not executed.


6.8. License query
Upon starting, the Stock Service checks whether for the configured stock connections there is a
valid license.
If the license check fails, no communication about the configured stock is established, however
the service continues to run since another licensed connection could be present.
An info e-mail is sent about the licensing problem.
Since the license check is not automatically repeated by the Stock Service, the service must be
restarted in order to perform another license check.


6.9. Special features of Bystronic connection
          IG stock logic
#337007
Previously invalid slot numbers (order number = 0) were not included.
With this process, a check is built in. If the order number = 0, the IG booking is not executed. A
corresponding note is in the Stock Service log, no e-mail is sent.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                30
         OrderListRequest/OrderList/BookData telegram
After the inward goods in AWE, all bookings that relate to this deliver will be initiated by
Bystronic. Bystronic first sends the telegram "OrderListRequest" with the number of the AWE
interface stock in order to query the inward goods for the stock. The Stock Service responds to
this with the "OrderList" telegram, which contains the inventories in the corresponding IG stock. If
an error occurs during the query of the IG stock in the Stock Service or if the "OrderList" cannot be
created because there are unbooked records for the IG stock in front of the stock booker, an
empty "OrderList" telegram is sent back to Bystronic. The error is logged by the Stock Service (log
file, see installation instructions) and the employee configured in the Stock Service receives the
error message via e-mail.
On the Bystronic page, there is now a reconciliation of the "OrderList" telegram with the goods
delivered. If a deviation is determined (incorrect cover sheet), it is possible to correct the
inventory in the ERP stock in the GR stock. The slot assignment for the new cover sheet must
absolutely be adhered to. Then, Bystronic must send another "OrderListRequest" telegram in
order to receive the updated "OrderList."
After the successful reconciliation of the "OrderList" telegram with the goods delivered, Bystronic
initiates the inward booking into the interface stock by sending the "BookData" telegram. The
Stock Service executes the appropriate outward bookings from the IG stock and inward bookings
to the interface stock. The booking price for the inward booking of a variant into the interface
stock is determined from the average price of the variant in the IG stock. No response telegram is
sent. Errors that occur are logged by the Stock Service and sent via e-mail.


         UnBookData telegram
Bystronic can then initiate outward bookings from the interface stock with the "UnBookData"
telegram. The outward booking types AUTO (production/cutting) and BREAK (break) are
processed. Both types equally cause an outward booking in the ERP stock. No response telegram
is sent. Errors that occur are logged by the Stock Service and sent via e-mail.


         Cyclical stock reconciliation
In a 24-hour rhythm, the Stock Service initiates a stock reconciliation of all interface stocks
configured in AWE. The service sends an "InventoryRequest" telegram for a stock to be reconciled
and receives a "StoreInventory" telegram as response, which contains the inventory of the
corresponding Bystronic stock. The Stock Service reconciles the inventories of the variants and
adjusts the stock of the AWE stock to the inventory of the Bystronic stock with inward or outward
booking orders. A stock reconciliation is not executed if there are flawed booking records in front
of the stock booker for the interface stock to be reconciled.


         Restrictions
Batch tracing
Batch tracing is not implemented. During the stock inward booking via interface,
Bystronic transmits a batch number, however this is not transmitted to the ERP system by
the Stock Service.
Thickness specifications

A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                              31
No glass thicknesses are transmitted by the Bystronic interface, as a result, these can also not be
considered for the data matching in the ERP system. This means that items that are distinguished
only by their thickness always have different material numbers in the Bystronic system.
No special treatment of cover sheets and breakage
With AWDesk #371602 the special treatment of cover sheets was implemented for Hegla
connection.
The analysis of Bystronic interface shows that the treatment of cover sheets and breakage can
NOT be supplied within the process by the Bystronic interface. The main reason is, that no
information regarding glass type (cover sheet/breakage/normal) was sent in the telegram of cyclic
stock reconciliation.


6.10.           Particularities of the Hegla stock connection
                IG stock logic
IG stock logic can only be used with a Hegla interface version 2.2.0.0 or higher.


                Booking the goods receipt
OrderListRequest/OrderListRequestResult/OrderListEntryBooked Telegramm (AWDesk
#338820)
After the inward goods in AWE, all bookings that relate to this delivery will be initiated by Hegla.
Hegla first sends the telegram "OrderListRequest" with the number of the AWE interface stock in
order to query the inward goods for the stock. The Stock Service responds to this with the
"OrderListRequestResult" telegram, which contains the inventories in the corresponding GR stock.
If an error occurs during the query of the IG stock in the Stock Service or if the "OrderList" cannot
be created because there are unbooked records for the IG stock in front of the stock booker, an
empty "OrderList" telegram is sent back to Hegla. The error is logged by the Stock Service (log file,
see installation instructions) and the employee configured in the Stock Service receives the error
message via e-mail.
On the Hegla page, there is now a reconciliation of the "OrderListRequestResult" telegram with
the goods delivered. If a deviation is determined (incorrect cover sheet), it is possible to correct
the inventory in the GR stock in the AWE stock. The slot assignment for the new cover sheet must
absolutely be adhered to. Then, Hegla must send another "OrderListRequest" telegram in order to
receive the updated "OrderList."
After the successful reconciliation of the "OrderListRequestResult" telegram with the goods
delivered, Hegla initiates the inward booking into the interface stock by sending the
"OrderListEntryBooked" telegram. The Stock Service executes the appropriate outward bookings
from the IG stock and inward bookings to the interface stock. The booking price for the inward
booking of a variant into the interface stock is determined from the average price of the variant in
the IG stock. No response telegram is sent. Errors that occur are logged by the Stock Service and
sent via e-mail.
OrderListReference
The “OrderListRequestResult” telegram contains in particular the “OrderListReference”.



A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                              32
In the GR stock logic, the reference consists of:
    •   Slot number
    •   Article number
    •   Variant number
    •   In format <Slot number>/< Article number>/< Variant number>
Example: Slot 224455/1, Article number 100004, Variant number 23
=> OrderListReference “224455/1/100004/23”


The OrderListReference is sent back by Hegla using the “OrderListEntryBooked” telegram to refer
to the respective element of the “OrderListRequestResult”.



                Booking types (Hegla InventoryType)
The Stock Service currently only books the following booking types (inventory changes) reported
active by the Hegla stock:
1 – Manual inward booking (only to cover sheet stock)
3 – External booking out of stock
4 – Automatic booking out of stock
7 – Breakage (if "Ignore Broken Glass" is configured)
This means that with the current Stock Service, NO inward bookings initiated by the Hegla stock
into the ERP stock are possible. Correction bookings (InventoryType 2) are also currently not
processed.


Removals
Logic adjustment with build 13.04.9880
Previously, for the processing of the InventoryChange telegram, the "Destination position" (target
position) was not evaluated.
This problem is now solved.
If an InventoryChange telegram is sent by the Hegla interface, now first the "Destination position"
is checked.
InventoryChange telegrams with a destination position <= 1000 are not processed further since
these are not removals from the stock.
Destination positions <= 1000 are stock locations within the stock. For cutting tables, destination
positions > 1000 are provided.
Only the destination positions > 1000 are now processed further as stock removals.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                             33
               Re-booking previously unbooked stock removals
When starting the Stock Service and after successful establishment of socket communication with
the Hegla server, there is a query of all bookings executed by the sending of the
GetInventoryChange telegram. All bookings are requested that have been executed in the Hegla
stock since the last booking transmitted.
When the ERP Stock Service receives the GetInventoryChangeResult telegram, it checks the
validity of the time stamp of each booking (see chapter "Time stamp of the last booking made").
Only records with valid time stamp are forwarded to the ERP system for booking. After a
successful booking, the time stamp for the query of the booking made is updated.




A+W Software GmbH              EN-CONFIG-A+W ERP Stock Service.docx                           34
                Time stamp of the last booking made
In the ERP system, the time stamp of the last booking made ("footprint") is saved for a portal
stock.
Each booking report from the Hegla stock is compared to the saved time stamp. The currently
reported booking in the ERP system is only made if the time stamp of the current booking is
greater than the saved reference time stamp. Each booking must be more recent than the last
booking made.
This logic exists to prevent out-of-date booking messages from creating new bookings in the ERP
system.
The complete time stamp set consists of:
    -   Portal stock number (stock_id)
    -   ID of the source item (Hegla) of the booked lite (key1)
    -   ID of the destination item (Hegla) of the booked lite (key2)
    -   Time stamp as string (key3)


In A+W Enterprise, the time stamp table is called "wlportalsync".
In A+W Business, the time stamp table is called "SYSADM.LG_LASTBOOKED".


For a Hegla connection, the following logic also exists:
If the ERP Stock Service is started, there is a check whether there are "passed-over bookings" that
must be rebooked.
For this logic, in the ERP Stock Service, there are log entries with the keyword
"WorkMissedInventoryChanges()". In the ERP system, the time stamp of the last booking made is
determined. Then in the Hegla stock, all bookings are queried whose time stamp is greater than
the last booking made in the ERP system. If the Hegla stock reports bookings for this query, these
are rebooked in the ERP system.
If in the ERP system no time stamp of the last booking made can be determined, the rebooking
logic is exited without further actions.
In the log, you will find the message "HeglaSyncSingle.WorkMissedInventoryChanges(): No
booking foot print existing => exit.".


Remark:
The time stamp in the ERP system is saved as string. The format of the string is specified
regardless of culture ("CultureInfo.InvariantCulture"): "MM/dd/yyyy hh:mm:ss".
The formatting has nothing to do with the transfer in the interface telegram.
Sample time stamp string: " 12/05/2023 08:39:27".




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                             35
                Special treatment of cover sheets (AWDesk #371602)
If a cover sheet stock was entered in the Config Tool for Hegla connection, the cover sheets will
be booked to this special cover sheet stock.
Caution: A cover sheet stock may only be entered if it is different from the interface stock.
Cover sheets are marked as such on the racks in the Hegla stock. For a lite to be booked, it can be
determined using the rack on which the sheet is located, and using the position of the lite on the
rack, whether or not it is a cover sheet.
Configuration without GR stock means that the ERP stock's inventory is updated by booking
telegrams and the cyclic reconciliation and then all bookings of cover sheets are made from the
corresponding cover sheet stock.
Configuration with GR stock and in the PO logic [AW-76610] means, when receipt of goods is
confirmed (OrderListRequestEntryBooked) the cover sheets are booked for a short period to the
portal stock and rebooked immediately from the portal stock based on a booking telegram
(InventoryChangeEvent) to the cover sheet stock. Following, all bookings of cover sheets - as in
configuration without GR stock - from cover sheet stock.


Restrictions
If in the Hegla stock an existing cover sheet is rebooked, that is, it goes from type "cover sheet" to
type "normal sheet," this information is not known immediately in the ERP system. Only with the
next cyclical reconciliation is the sheet booked into the portal stock instead of the cover sheet
stock.


                Treatment of broken glass (AWDesk #371602)
With Hegla connection, the "Ignore Broken Glass" checkbox can be enabled or disabled in the
Config Tool.
If the "Ignore Broken Glass" checkbox is disabled, broken lites that are reported by external stock
with an InventoryChangeEvent are removed from the ERP stock.
During the cyclical comparison, the broken lites are also booked in the ERP system.
If the "Ignore Broken Glass" checkbox is enabled, broken lites from external stock are NOT booked
in the ERP system.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                               36
                 Handling of residual plates
At the moment (status as of 07/25/2024), in the InventoryChangeEvent, the type "Restblatt" is
not recognized and there can therefore be no special treatment.
If the dimensions of a residual lite fit a variant, the lite is booked.
It can be that with PF [AW-176670] special treatment of the residual lites will be implemented.
In the interface description of Hegla, the telegrams GetInventoryChangeResult,
InventoryChangeEvent, GetRackLoadingResult, GetStockInventoryResult all receive the
parameter "Type". The information whether the lite is a residual lite is in "Type".




Currently, however, precisely the information that this is a residual lite is not transferred to
the ERP Stock Service by the A+W interface ("Panorama").




                 Treatment of glass thicknesses (AWDesk #461784)
By activating the "Ignore Thickness" checkbox in the Config Tool, the thickness of the Hegla article
is not considered in the Hegla stock connection when searching for the mapped article in the ERP
stock. Mapping can only work if there are no thickness variations in the Hegla system for article
numbers.
The logic only works if an ERP stock is linked to a Hegla stock. For other third-party stocks
(Bystronic, Lisec), the logic is not made available.
For the AWE connection, the same configuration option also exists via the environment variable
STOCK_HEGLA_IGNORE_THICKNESS (AWDesk # 453768). This type of configuration was made



A+W Software GmbH                 EN-CONFIG-A+W ERP Stock Service.docx                             37
available when it was not yet known that the same logic was also required in the AWB
connection. It is recommended that the configuration is preferably done via the Config Tool.


              Checking the connection to the Hegla server (AWDesk
        #459484, PF [AW-41702])
When starting the Stock Service, the socket connection to the Hegla server is established. The
Stock Service functions as a client. At the time of the cyclical reconciliation, it is checked whether
there is still a connection to the Hegla server. If not, there is an attempt to establish a connection.
In addition, it is checked every 30 minutes whether there is still a connection to the Hegla server.
If it is determined that the connection has been interrupted, there will be another attempt to
make a connection.
The cyclical check should prevent that the connection remains permanently interrupted after a
reboot of the Hegla server, and as a result that no bookings may be made in the ERP stock.



                 PO logic [AW-76610]
Instead of the GR stock logic, the PO logic can be configured in connection with A+W Enterprise.
This logic is only available if on the ERP side an A+W Enterprise is configured and a Hegla stock is
connected. A precise description of the logic is in section 7.


                 Restrictions
General
    •     Only dimension variants, but no color variants are considered.
    •     All referenced ERP items must keep dimension variants.
    •     Each Hegla stock will be synchronized with precisely one ERP stock. Here, a Hegla server is
          regarded as a Hegla stock.
Configuration of the communication in the Config Tool
From the point of view of the ERP system, a Hegla server represents precisely one Hegla stock. It
can be connected/synchronized with precisely one ERP stock in the configuration.
The configuration of several ERP stocks with one and the same Hegla servers by generating
several entries in the connections that only differ in the Client ID (but address the same Hegla
server, with the same IP and the same port), is NOT permissible.
Socket communication
All time stamps are requested by the Stock Service from the Hegla server in the format .
"dd.mm.yyyy hh:nn:ss" - that is, to the second.
Batch tracing
Since in the current Hegla interface no information about the batch is transmitted, no batches are
considered within the Stock Service.
Limitations of the reconciliation


A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                38
In the course of permanent stock-keeping, only outward bookings are processed. Inward bookings
take place on the basis of the inward goods in the ERP stock (only thus can a value stock-keeping
be guaranteed and a meaningful stock log arise). The inward booking of the inward goods in the
ERP stock must be done in timely fashion, in particular before an outward booking can take place
via the Hegla stock. The inward booking of the inward goods in the ERP stock must be done in
timely fashion.
Bookings from the Hegla stock for items not present in the ERP stock are rejected.
Bookings that would cause negative stocks are rejected by the stock booker if the env variable
WL_KEINE_NEGATIVEN_BESTAENDE is active. They remain as booking records with error flag in
the booking table wlh.
Re-bookings within the Hegla stock have no meaning for ERP stock.
Problems due to the decoupling of the commercial inward goods in the ERP stock from the
inward goods in the Hegla stock
In the long run, the stock connection only functions smoothly if the inward goods in the ERP stock
is executed in timely fashion with respect to the inward goods in the Hegla stock. If the
commercial IG is delayed, in the course of the day there can be a stock shortfall, so that the
booking records get stuck with the error status before the ERP booking process (if the env
variable WL_KEINE_NEGATIVEN_BESTAENDE is active). In this case, no nightly stock reconciliation
is executed.
If the shortfall in the commercial stock is corrected easily with a forced stock reconciliation, there
is an incorrect determination of the prices in the ERP stock. The solution is always the commercial
IG booking.
Handling of broken glass in inward stock booking
In GR stock logic Hegla announces the amount of broken glass in the telegram
“OrderListEntryBooked”. But the broken glass is ignored by the Stock Service and thus is not
considered in the booking. All lites, whether broken are not, are booked in.
Example: Hegla announces AMOUNT=10 and AMOUNT-BROKEN=3, which means that 3 of 10
booked glass lites are broken. The booking in AWE is 10 lites. The information about the broken
glass is dismissed.


Problems in case of deviation of the clocks on the Hegla server and the ERP Stock Service
process server
Both servers have to run synchronously so that the checking of the time stamp of a booking
transmitted by the Hegla server works correctly in the ERP Stock Service.
See also PF-Ticket [AW-58648].



                Overview of used telegrams
Here is an overview of the Hegla telegrams that are used in the communication with the ERP
Stock Service.
The socket communication with the Hegla stock is done via the A+W Panorama interface that is
integrated into the ERP Stock Service. The A+W Panorama intervace is supported by the


A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                               39
"Techsoft" department. For detailed information about implementation of the Hegla telegrams,
please consult the responsible Techsoft developer.
The telegrams are described in the Hegla interface documentation "Warehouse Management
System Interface 2.3.0.0_Rev2 -gb".
The completeness of the list is not guaranteed.
 Telegram name                            Use in the ERP Stock Service
 GetRacks                                 Cyclical reconcilation, racks
 GetRacksResult
 GetRackLoading                           Cyclical reconcilation, rack loading
 GetRackLoadingResult
 GetInventoryChange                       Request for bookings lost after connect
                                          with the Hegla server
 GetInventoryChangeResult
 InventoryChangeEvent                     Report of a removal
 OrderListRequest                         Request of the open POs or goods
                                          receipt
 OrderListRequestResult
 OrderListEntryBooked                     Report of the goods receipt by Hegla
 OrderListEntryBookedResult
                                          Report triggers a complete or partial
 OrderListUserEvent
                                          good receipt (only PO logic)




6.11.           Particularities of the Lisec stock connection
The Lisec connection contains cyclical stock reconciliation and the transfer of bookings (AWDesk
#391319).
The determination of the type of glass (normal glass/cover sheet/residual sheet) is done via the
master data of the last cyclical reconciliation. Changes to the master data therefore only affect
bookings after the next cyclical reconciliation.
Relevant tickets for booking are:
AWDesk #457700
PF [AW-63663]
PF [AW-107751]
The GR stock logic is not implemented.


                Functional characteristics
With the cyclical comparison, the entire inventory is queried by Lisec [GET_GLASS_STOCK].
For the inventory report by Lisec, the type of the glass (normal glass/cover sheet/residual lite) is
also communicated for each lite. This glass type is cached in the ERP Stock Service and used for all


A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                                40
following bookings. If in the Lisec system the type of glass has been changed in the meantime, this
change will only be noticed and become effective with the next cyclical comparison.
By stopping and then re-starting the ERP Stock Service, the updating of the cached glass types
(independently of the cyclical comparison) can be forced.


User interface version older than 02.00.007
With the Lisec interface version older than 02.00.007, bookings were processed via the inventory
change telegram (actions types "PUT_DOWN" and "REMOVE") .


Changes with Lisec interface version 02.00.007
With the Lisec interface version 02.00.007, removal bookings from the Lisec stock are processed
exclusively by the stock movement telegram (FROM_STOCK_ELEMENT - TO_STOCK_ELEMENT).
So that the logic takes, the Lisec interface version "02.00.007" must be selected in the Config
tool of the ERP Stock Service.
A glass is booked out of the stock if the element [TO_STOCK_ELEMENT] contains a value that is in
the number range 1010020001 to 1010029999.
This number range is reserved for the lines according to the Lisec interface description. If a glass
goes to the line, it counts as booked out of the stock.
Since via the stock movement telegram residual lites also go to the line, for the Lisec connection
the notification e-mail is suppressed, which is actually sent if an ERP variant for a removal booking
message cannot be sent.
It is assumed that this is a residual lite if no variant can be found. Residual lites are not booked.
See also PF [AW-135791] and [AW-220804].


                Special treatment of cover sheets
If a cover sheet stock was entered in the Config Tool for the Lisec connection, the cover sheets
will be booked at cyclical stock reconciliation to this special cover sheet stock.


                Handling of residual plates
Residual lites in the Lisec stock are not considered during the inventory updating (cyclical
synchronization and stock movement) in the ERP stock.
See also "Info e-mail" chapter.


                Treatment of broken glass
The handling of rejects was never discussed explicitly in the context of the interface. Right now (as
of 10/04/2023), it is not known with which telegram the removal booking of rejects is reported by
the Lisec stock.
If the rejects are reported by the stock movement telegram (starting with Lisec interface version
02.00.007) or the inventory change telegram (action types "PUT_DOWN" and "REMOVE")(Lisec



A+W Software GmbH                 EN-CONFIG-A+W ERP Stock Service.docx                             41
interface version older than 02.00.08) by the Lisec stock, they are booked in the ERP system so
that it is not known that this is a reject.
If the rejects are reported by another telegram or another action type, they are not booked in the
ERP system.




                  Info e-mail
For a Lisec connection, there is the special feature that for lites reported for removal booking, it
cannot be detected whether they are stock dimensions or residual lites. For each removal
booking, there is a search in the ERP system for an appropriate variant.
For residual lites, there should be no removal booking in the ERP system according to the
interface description. Since for a Lisec residual lite generally no ERP variant is found, the removal
booking is omitted. Normally, the ERP Stock Service sends an info e-mail if no appropriate variant
can be found in the ERP system for a removal booking message. In the case of the Lisec
connection, this e-mail is suppressed since otherwise incorrect info e-mails would be sent
constantly for residual lites in ongoing operation.
However, the side-effect of the suppressed e-mails is that there is no information via e-mail about
variant data that is actually missing. The message about a missing variant is always in the log of
the ERP Stock Service, however.
See PF [AW-147159] + [AW-135791].


Within the stock comparison, there is still information about lacking variants via e-mail.
See PF [AW-195424].


                  Restrictions
General
    •     Only dimension variants, but no color variants are considered.
    •     All referenced ERP items must keep dimension variants.
    •     Each Lisec stock will be synchronized with precisely one ERP stock. Here, a Lisec server is
          regarded as a Lisec stock.


Problems due to the decoupling of the commercial inward goods in the ERP stock from the
inward goods in the Lisec stock
In the long run, the stock connection only functions smoothly if the inward goods in the ERP stock
is executed in timely fashion with respect to the inward goods in the Lisec stock. If the commercial
GR is delayed, the correction is made with the next cyclical stock reconciliation, whereby there
can be an incorrect determination of the prices in the ERP stock. The solution is always the
commercial IG booking.




A+W Software GmbH                 EN-CONFIG-A+W ERP Stock Service.docx                                 42
                Information about the Lisec stock system
The Lisec version numbers follow the notation "02.00.000" or "02.x.y" (new crane system). ("2.71"
is an older version (old crane system).)
Between the crane systems, there are, among other things, mechanical differences.
For the current crane generation, V02.00.007 is required (status as of 02/02/2023).
With a converter, the old V2.71 can be used, however not all functions can be used with it.
A crane system recognizes 2 modes:
1. Glass stock for Lisec and glass info from third-party system
2. Glass stock with third-party system and start location from third-party system
In the documentation for V2.71, both modes are described.
With the conversion to the new crane system, the documentation was split. Each mode is
described in an individual document.
See also PF [AW-135791].




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                          43
7. Function description with A+W
  Enterprise
7.1. Process diagram
To understand the process, use the process diagram. Had initially been created and optimized for
Bystronic interface.




7.2. Multi-site systems
The multi-site capability of the ERP Stock Service is not guaranteed. In particular, in the tables
wlportalsync and wlportalwewait, there is no possibility to store the site number.
However, the configuration in the multi-site system will most likely work since in AWE the stock
numbers are unique across all multi-site sites.




7.3. Table wlportalsync
For the connection of a Hegla stock, it is necessary that the Stock Service notes the last booking
made. This occurs in the table "wlportalsync".
For the Bystronic connection, this table is not required. Nevertheless, it is kept generally so that
booking records for other stock connections (than Hegla) can be written to it. For the Hegla stock



A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                44
connection, 3 key fields are used in the booking record in order to mark a booking unique: 2
numeric and 1 alphanumeric.
There is no maintenance dialog because the data in the table is written exclusively (and deleted
again) by the Stock Service.
 Column name          Data type       Description             Note
 lnr                  integer         AWE stock number
 key1                 integer         Booking key 1           Hegla connection: numeric value
                                                              that describes the origin of the
                                                              stock dimension in the Hegla stock
 key2                 integer         Booking key 2           Hegla connection: numeric value
                                                              that describes the target location
                                                              of the stock dimension (cutting
                                                              table) in the Hegla stock
 key3                 string          Booking key 3, in the   Hegla connection:
                                      DB as CHAR(80)          Booking time stamp assigned down
                                                              to the second by Hegla




7.4. Table wlportalwewait
The table is only used by the PO logic [AW-76610] in the ERP Stock Service.
In the table, PO data is stored temporarily that is required by the Hegla system in order to be able
to book a receipt of goods there.
If the receipt of goods for a PO is completed in the Hegla system and the corresponding receipt of
goods has been triggered in A+W Enterprise, the entries for this PO in the table are deleted.
 Column name          Data type       Description             Remarks
 auftrnr              integer         P.O. number
 procedure            smallint        Document number         fix "2" (PO)
 posnr                smallint        Internal item
                                      number
 lfdpos               smallint        External item
                                      number
 artnr                integer         Article number
 bitnr                smallint        Variant number
 lnr                  integer         Stock number.
 bestmenge            integer         Open PO quantity        Open PO quantity for which a
                                                              receipt of goods is expected.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                              45
fwlmenge            integer         Third party stock      Current receipt of goods quantity
                                    receipt of goods       that was reported by the third-
                                    quantity               party stock.
status              integer         Status                 See special subsection "Status
                                                           values."
bemerk              char(30)        Remark
izeit               DateTime        Insert time
uzeit               DateTime        Update time



         Status values of the table wlportalwewait
UNDER CONSTRUCTION (SVH 03/25/2022)
Status           Name                        Description
0                New                         No receipt of goods from the third-party stock
                                             was reported.
1                Third-party stock goods     A receipt of goods from the third-party stock was
                 receipt                     reported.
2                ERP receipt of goods        A receipt of goods was booked in the ERP system.
101              ERP receipt of goods        There was an attempt to book a receipt of goods
                 error                       in the ERP system, but there was an error.
(error status)




A+W Software GmbH              EN-CONFIG-A+W ERP Stock Service.docx                            46
7.5. Tracing the bookings
The Stock Service creates all bookings to be made for the AWE stock booking (table wlh).
The status values used (wlh.b_status) are:
    •   Inbound stock: 29
    •   Outward stock: 30
These status values are reserved for bookings that are made in the AWE from external systems.
The bookings of the Stock Service can also be identified by the text "stock service," that is stored
with the booking in the field wlh.bemerk. The text can be seen in the stock report in the detail
view of a booking record.
Bookings that receive the status "StoBal" are generated during the cyclical (generally nightly)
stock reconciliation (= "Store Balance").
If via the Config Tool a separate cover sheet stock is configured, the bookings are made either for
the cover sheet or the normal lite stock. This is how the different notes "StoBal CoverSheet" and
"StoBal Normal" are created.
The notes "Unknown/Automati" and "Unknown/Breakage" refer to the removal bookings that are
made in the external stock based on production or breakage.




7.6. Cyclical stock reconciliation
         Booking price
If a newly-configured interface stock in AWE is replaced by a new nightly stock reconciliation, the
Stock Service can determine no booking price for the variants to be booked. In this case, the
booking records will be presented to the stock booker without booking price. The stock booker
detects the missing price and sets the records to error status -20004. The bookings can be
processed only after a price has been entered by hand in dialogue STOCK > Info system > Booking
status > Error, and the error has been reset.


         Handling of incorrect booking records
Previously, the cyclic reconciliation was not performed if there were error records (table wlh) at
the start time for stock reconciliation (wlh.fehler != 0).
The logic was changed with AWDesk #371602. In case of error records it is checked whether the
records were presented to the stock booker of the Stock Service. (identifiable by the field
wlh.bemerk with text "stock service“.)
Such error records do not prevent the reconciliation anymore. They are marked by writing a
special text to wlh.bemerk1. Then, the reconciliation is executed. If the reconciliation was
successful, the marked error records are deleted in wlh. In case of an error, the marking is deleted
from the error records and they remain in table wlh.




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                                 47
This change of logic shall prevent the reconciliation from being blocked by the new special
treatment of cover sheets. A problem may occur if a rebooking is made for a cover sheet, so that
it is an available normal lite and then it is booked. In the ERP system the lite would be in the cover
stock, but the booking would be executed in the interface stock. If there is no stock the booking
record remains before the stock booker.




7.7. PO logic (only Hegla connection) [AW-76610]
         General description
Instead of the GR stock logic, the PO logic can be configured in connection with A+W Enterprise.
This logic is only available if on the ERP side an A+W Enterprise is configured and a Hegla stock is
connected.
Minimum requirement of the Hegla interface version is 2.3.0.0
(Interface description in the Hegla document "Warehouse Management System Interface
2.3.0.0_Rev2 -gb".)
The logic for processing goods receipts for stock POs for a synchronized Hegla stock has changed
in this logic. Previously for booking of the receipt of goods in the Hegla stock the prerequisite was
that the corresponding receipt of goods was booked in A+W Enterprise beforehand. The logic has
been adjusted so that the receipt of goods in the Hegla stock happens without the existence of
the receipt of goods in A+W Enterprise. The data for booking in the Hegla stock is made available
from the A+W Enterprise PO.
The POs are entered separately in the ERP system in batches. An ERP PO item includes the
quantity of a batch as it should be booked into the Hegla stock. Separately, the cover sheets of
the batches are entered individually as PO items. If in the ERP PO separate items for stacks and
cover sheets with the same glass types are entered, these are now also sent as separate items to
the Hegla stock. Cover sheets of the same glass types are also to be entered separately so that
each cover sheet item always includes the quantity "1". A batch and an associated cover sheet are
not linked in the PO. No entry sequence is prescribed.
Each PO item that is sent to the Hegla stock also includes in the new telegram field "Reference"
the A+W Enterprise PO number (kauf.auftrnr).
Due to the separately kept PO items, it is ensured that during goods receipt in the Hegla stock, the
employee can book, using the ERP PO list, which he requests from the ERP system, each batch and
each cover sheet into the correct storage location and report the booking confirmation back to
the ERP system.
The PO list ("Order list") includes all open PO items in the configured period (-> see config tool).
After the receipt of goods has been executed in the Hegla stock, the booked quantities are
reported by the Hegla stock to the A+W ERP Stock Service. The report includes in each telegram
(OrderListReference field) the reference to the PO number and the item number. The reported
Hegla goods receipts are collected by the ERP Stock Service in the intermediate table
"woportalwewait" until each PO item has a report with the ACTUAL quantities or until a telegram
is sent by the Hegla system that includes the instruction that for a PO with open items, a partial
goods receipt or a goods receipt should be booked.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                              48
Then the associated goods receipt is initiated by the A+W ERP Stock Service and thus also the
stock receipt booking in A+W Enterprise.
If the ACTUAL quantities of PO quantities deviate or if the instructions for partial goods receipts or
goods receipts come explicitly from the Hegla system, an e-mail is sent to a configurable
employee (purchaser). In the e-mail, the quantity deviation with reference to the PO is described
so that the informed employee can place a complaint with the supplier.
Even if complete goods receipts were booked in the ERP system, a corresponding info e-mail is
sent.
For the PO logic, the prerequisite is that the stock POs for the coupled Hegla stock are entered
with prices (a price must be stored in each item), for without prices, there can be no booking in
the A+W Enterprise stock.




ICE / AWSOA
For the PO logic, the A+W ICE environment (AWE purchaseservice) is required. It must be installed
and configured in addition to the A+W ERP Stock Service.
The installation of the ICE service is described in the "Enterprise System" configuration document.


PLEASE NOTE:
    •   Open PO quantities – date restriction
        For the request for the "Order list," only POs are considered whose planned delivery date
        (kauf.ltplan) is in a particular date range:The date range can be configured via the config
        tool of the ERP Stock Service by specifying the number of days that should be searched in
        the past and in the future.


    •   Open PO quantities – Box items
        If a box item is included in a PO (that is, a box stock is assigned as default stock), then the
        PO is sorted out and not reported with the open POs.

    •   Open PO quantities – Maximum number
        There is no restriction on the number of the maximum open POs reported back.


    •   Open PO quantities – Order List Reference
        For the request of the "Order List", for each open PO item, a unique "OrderListReference"
        is generated from the AWE data. It has the structure:
        <Bestellnummer>/<externe Positionsnummer>/<Artikelnummer>/<Bitnummer>.
        For example: "123456/3/100004/23"

        Furthermore, in the "Reference" field, the number of the AWE PO is transferred.


    •   Goods receipt report from Hegla
        Using the unique "OrderListReference" it is possible to determine the associated AWE PO
        item from the telegram "OrderListEntryBooked" that Hegla sends.



A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                49
A+W Software GmbH   EN-CONFIG-A+W ERP Stock Service.docx   50
         Installation
Table wlportalwewait
If the A+W Enterprise environment is not up-to-date, the table wlportalwewait must be created.
Script: …\alcib\14\0\de\install\xsql\13\0\4\130004182_wlportalwewait.sql


AWE purchaseservice
A purchaseservice with build >= 13.04.2658 must be installed.
Source: srvalcib 130:/develop/alcib/13/0/de/al_bin/Linux.rel




A+W Software GmbH              EN-CONFIG-A+W ERP Stock Service.docx                          51
         Configuration
AWE environment variables
WARENEINGANG_EXTERN
The env variable WARENEINGANG_EXTERN must be activated with the value "ON."
The variable controls that when booking the goods receipt via the AWE purchaseservice, the data
in the table autwe is considered.


AUTWE_KOMPLETT_BLEIBT
The env variable AUTWE_KOMPLETT_BLEIBT must be activated with the value "ON."
The variable controls that when booking the goods receipt via the AWE purchaseservice,
complete goods receipts can be booked even if the item quantities that are reported via the table
autwe are not complete.


Master data in AWE
The stored GR stock for the portal stock used must absolutely be removed in the stock master
data.


Check of the open POs
If there are open POs for the Hegla portal stock for which no more delivery is expected, these POs
must be completed before the new logic is put into service.


Config tool
Here, only the special configuration settings for the PO logic are described. All other descriptions
are in the installation instructions.




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                               52
Use AWSOA
This checkbox controls the use of the AWE purchaseservice. It must be activated so that the PO
logic takes hold.


AWSOA Login Name
Here, the user for the use of the AWE purchaseservice is stored. The entry is absolutely
mandatory for the PO logic. The stored name must exist in the AWE employee master data as



A+W Software GmbH              EN-CONFIG-A+W ERP Stock Service.docx                              53
login name (field mitarb.loginname).
CAUTION: The user must have at least the right DIWK in AWE.


AWSOA Multisite ID
Here, the site number of the purchaseservice used is stored. In a multi-site installation, there are
several values to choose from. The possible site numbers are displayed in the drop-down menu of
the field. The default in a single site environment is "-1".


Date Range Into Past (days)
The number of days to search for open purchase orders in the past, starting from the current
date, is entered.


Date Range Into Future (days)
The number of days to search for open purchase orders in the future, starting from the current
date, is entered.



          Open POs and "order list"
To report the "order list" to the third-party system, the ERP Stock Service queries the open POs
from the AWE purchase service.
Here, it must be noted that an item of a PO no longer counts as open if there is already a partial
goods receipt for this item for the complete ordered quantity of the item. This item will no longer
appear in the "order list."
As a result, for this item no more goods receipt can be reported from the third-party system.
In contrast to this, in A+W Enterprise, in the goods receipt entry, the item of a PO is still displayed
if there has been a partial goods receipt for the complete item quantity. You can enter additional
goods receipt quantities for this item.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                54
          Booking the goods receipt
Telegrams: OrderListRequest/OrderListRequestResult/OrderListEntryBooked
After the goods receipt in the Hegla stock, all bookings that relate to this delivery will be initiated
by Hegla. First Hegla sends the telegram "OrderListRequest" in order to query the open POs in
A+W Enterprise. The ERP Stock Service responds with the "OrderListRequestResult" telegram,
which includes the open PO items.
On the Hegla page, there is now a reconciliation of the "OrderListRequestResult" telegram with
the goods delivered.
After the successful reconciliation of the "OrderListRequestResult" telegram with the goods
delivered, Hegla confirms the goods receipt by sending the "OrderListEntryBooked" telegram. The
confirmation is done precisely to the item.
For the goods receipts confirmed by Hegla with the "OrderListEntryBooked" telegram for the PO
items, the corresponding goods receipts are booked in A+W Enterprise.
OrderListReference
The “OrderListRequestResult” telegram contains in particular the “OrderListReference”
parameter.
In the PO logic, the reference consists of:
    •   P.O. number
    •   External item number
    •   Article number
    •   Variant number
Example: PO number 123456, item 1, article number 100004, variant number 23
=> OrderListReference "123456/3/100004/23"


The "OrderListReference" is sent back by Hegla using the “OrderListEntryBooked” telegram to
refer to the respective element of the “OrderListRequestResult”.
If the "OrderListReference" is empty or it contains an unknown value, the goods receipt cannot be
booked on the ERP side.




          Booking the goods receipt in the ERP system
The booking of the goods receipt in the ERP system can be triggered automatically or by
instruction of the external stock.
In the header of the goods receipt (kauf record), the current booking date is entered as goods
receipt date (kauf.ltplan and kauf.ltideal).


With A+W ERP Stock Service 6 - 13.04.9935 (10.06.2025), the logic of the automatic booking was
adjusted.

A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                55
Up to that point, a complete goods receipt was booked automatically in the ERP system if a goods
receipt for all PO references of a PO was reported by the external stock.
The quantities reported played no role. They could be smaller, larger, or equal to the PO
quantities.
With A+W ERP Stock Service 6 - 13.04.9935 (10.06.2025), the logic was changed so that a
complete goods receipt is only booked in the ERP system if a goods receipt is reported for all PO
references of a PO from the external stock AND the reported goods receipt quantities are equal to
or greater than the PO quantities.
If a goods receipt is reported for all PO references of a PO from the external stock AND the
reported goods receipt quantities are less than the PO quantities, a partial goods receipt is
booked automatically in the ERP system. In this case, additional partial goods receipts can follow.
In all other cases, that is, if goods receipts from external stock are not reported for all PO items,
there is only a goods receipt booking in the ERP system if the external stock triggers this booking
explicitly. The triggering is done by a special telegram (OrderListUserEvent).
For the logic, a purchaseservice build >= 13.04.7159 is required.
The booking logic is explained again in the "Overview using case descriptions" section.
Since the new logic was implemented without environment switch, the behavior of the service
changes during an update to the manner described, which has no additional consequences.
Only the marking of goods receipts changes in some cases. Some goods receipts that were
previously automatically marked as "complete" (liefkomp=2) in the ERP system now remain as
"not complete" (liefkompl=1) in the system.


Note for development:
Within the logic, it can be that the new function "SetGoodsReceivedComplete()" of the
purchaseservice is called. The call is logged in the log of the ERP Stock Service.
The function returns a bool (successfully executed (true) or error occurred (false)). In the
purchaseservice, the back end function "GoodsReceiptComplete(long auftrnr)" is called.Here, the
return value can have the following characteristics:
1 = PO not found
2 = PO locked
3 = Error on update
0 = Everything ok
The return value is logged in the log of the purchaseservice.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                               56
See PF [AW-230073].



           "OrderListRequestResult" telegram
        Name                      Designation                Comment
 1      OrderListReference        Purchase item              Structure:
                                  reference                  <Purchase number>/<External item
                                                             number>/<Article number>/<Variant
                                                             number>.
                                                             For example: "123456/3/100004/23"
 2      Amount                    Qty                        Open purchase amount
 3      ArticleCode               Article no.                Article number (in external stock)
 4      Width                     Width                      Width of the glass
 5      Height                    Height                     Height of the glass
 6      Thickness                 Thickness                  Thickness of the glass
 7      ArticleCodeCoverSheet     Article number of cover    fix: empty
                                  sheet
 8      CoatingSide               Coating side               fix: "0" (not defined)
 9      DeliveryOrderNr1          -                          fix: empty
 10 DeliveryOrderNr2              -                          fix: empty
 11 DeliveryOrderNr3              -                          fix: empty
 12 DeliveryOrderNr4              -                          fix: empty
 13 Quality                       Quality                    fix: "100" (default)
 14 QualityCoverSheet             Quality of cover sheet     fix: "0"
 15 ThicknessCoverSheet           Thickness of cover         fix: "0"
                                  sheet
 16 UniqueIdentificationList -                               fix: empty
 17 Wrapped                       -                          fix: "0" (not defined)
 18 Reference                     Reference                  Purchase number in A+W Enterprise




           Overview using case descriptions
 Case      Report from the Hegla stock              Action in A+W Enterprise
 1         A goods receipt is reported for all PO   Generation of the goods receipt for all PO
           references of a PO.                      items.



A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                             57
       Die gemeldeten Mengen spielen            Execution of the corresponding stock
       dabei keine Rolle. Sie können kleiner,   bookings.
       größer oder gleich den
                                                The PO counts as completed.
       Bestellmengen sein.
                                                The goods receipt is complete.
       Technical:                               => kauf.liefkompl = 2
       - Telegram OrderListRequest
                                                Es wird eine Info-E-Mail versendet.
       - Telegram OrderListEntryBooked for
       all items                                [AW-230073] - Outdated logic, no longer valid
                                                since A+W ERP Stock Service 6 - 13.04.9935
                                                (10.06.2025)
1      A goods receipt is reported for all PO   Generation of the goods receipt for all PO
       references of a PO.                      items as partial goods receipt.
       The reported goods receipt               Execution of the corresponding stock
       quantities are less than the PO          bookings.
       quantities.
                                                The goods receipt does not count as
       Technical:                               completed.
       - Telegram OrderListRequest              => kauf.liefkompl = 1
       - Telegram OrderListEntryBooked for
                                                An info e-mail is sent.
       all items
                                                [AW-230073] - Current logic, valid since A+W
                                                ERP Stock Service 6 - 13.04.9935 (10.06.2025)
2      A goods receipt is reported for all PO   Generation of the goods receipt for all PO
       references of a PO.                      items as complete goods receipt.
       The reported goods receipt               Execution of the corresponding stock
       quantities are equal to or greater       bookings.
       than the PO quantities.
                                                The goods receipt counts as complete.
       Technical:                               => kauf.liefkompl = 2
       - Telegram OrderListRequest
                                                An info e-mail is sent.
       - Telegram OrderListEntryBooked for
       all items                                [AW-230073] - Current logic, valid since A+W
                                                ERP Stock Service 6 - 13.04.9935 (10.06.2025)
3      A goods receipt was not reported for     Generation of the goods receipt for all
       all PO references of a PO; the PO was    previously reported PO items.
       reported as complete by Hegla.
                                                Execution of the corresponding stock
                                                bookings.
       Technical:                               The goods receipt counts as complete.
       - Telegram OrderListRequest              => kauf.liefkompl = 2
       - Telegram OrderListEntryBooked for
       one or several, but not all, items-
       Telegram OrderListUserEvent with
       UserAction "0" (= "complete")
4      A goods receipt was not reported for     Generation of a partial goods receipt for all
       all PO references of a PO; the good      previously reported PO items.
       receipts were reported as partial
                                                Execution of the corresponding stock
       goods receipts.
                                                bookings.


A+W Software GmbH            EN-CONFIG-A+W ERP Stock Service.docx                               58
                                                   The goods receipt does not count as
                                                   completed.
          Technical:
                                                   => kauf.liefkompl = 1
          - Telegram OrderListRequest
          - Telegram OrderListEntryBooked for
          one or several, but not all, items
                                                   The goods receipt in AWE are only completed
          - Telegram OrderListUserEvent with
                                                   if the message of the outstanding goods
          UserAction "1" (= "partial")
                                                   receipts have been produced by Hegla.


 5        A goods receipt was not reported for     The goods receipts reported by Hegla remain
          all PO references of a PO.               in the intermediate table.
          The state of the goods receipt is not
                                                   There are no bookings in AWE.
          declared.
                                                   As long as there are records in the
          Technical:
                                                   intermediate table, no cyclical stock
          - Telegram OrderListRequest
                                                   reconciliation is done.
          - Telegram OrderListEntryBooked for
                                                   An e-mail is sent that informs that for which
          one or several, but not all, items
                                                   POs there are still missing goods receipt
          - No additional telegram for this PO
                                                   reports and that a cyclical stock reconciliation
                                                   cannot be done in the current state.


For all goods receipt bookings and stock bookings in the ERP system, the reported ACTUAL
quantities from the Hegla stock apply.



         Error handling
Cyclical stock reconciliation (store balance)
With the PO logic, there can be intermediate states where goods receipt quantities are stored in
the table wlportalwewait for which no explicit goods receipt was triggered from the Hegla system.
If in this state a cyclical stock reconciliation is started, these data records are recognized in
wlportalwewait and the stock reconciliation is canceled.
An e-mail is sent in which it is described which data caused the cancellation of the reconciliation.


Non-availability of the AWE purchaseservice
The ERP Stock Service generally starts several attempts to establish communication with the A+W
purchaseservice.
If at the request of the open POs ("Order list") by the Hegla system the connect to the AWE
purchaseservice fails, an empty "Order list" is returned to Hegla. In the log of the ERP Stock
Service, there is then information about the cause of the error.
If an ERP goods receipt booking should be made and the connect to the AWE purchaseservice fails
in the process, the ERP Stock Service sends an e-mail that informs about which PO and which PO
items a goods receipt (partial or complete) with which quantities could not be booked. The e-mail
includes the request to book the failed goods receipt in the ERP system manually in order to
prevent inconsistent data.


A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                                  59
Goods receipt bookings in the Hegla stock with non-availability of the A+W Stock Service or the
AWE purchaseservice
According to statements from Hegla (status as of 03/29/2022), "...the operator on the Hegla
system always has the opportunity to make bookings completely manually..." if on request of the
open POs ("Order list") by the Hegla system no data could be delivered by the A+W ERP Stock
Service for some reason.


Treatment of PO items without third-party product code when sending the OrderList
If the Hegla system requests an OrderList, the third-party product code (= Hegla product code)
must be determined for each open PO item of the AWE order. For this, the artkuzu.kuartnr is
selected from the table artkuzu that is stored there for the PO article and the configured Hegla
market partner. If for an AWE article number no third-party product code can be found, this PO
item cannot be transmitted to the Hegla system. Hegla relies on its own product code.
The error is reported by the ERP Stock Service via an e-mail and is also listed in the log.
Previously (status as of 07/23/2024), a single error in the determination of the third-party product
code caused an empty OrderList to be reported to Hegla. This means even for POs not affected,
no goods receipt from third-party stock could be booked as long as the master data was not
corrected.
The logic has now been changed. Only the affected PO item for which no third-party article code
can be found will be removed from the OrderList. All other PO items are transferred to the third-
party stock in the OrderList.
An e-mail about the error is still sent and corresponding log messages are written.
See also PF [AW-199683].


Treatment of incorrect details in the "OrderListReference" in the "OrderListEntryBooked"
telegram
With the "OrderListEntryBooked" telegram, Hegla reports the goods receipt (quantity in pieces)
for a defined PO item.
In case of an incorrect "OrderListReference" in the "OrderListEntryBooked" telegram, the ERP
Stock Service cannot determine the AWE PO item.
The goods receipt cannot be processed in this case. A response telegram with the error number "-
1" (="Unknown order list reference") is returned to Hegla.
With the implementation for PF [AW-199683] (07/25/2024), now an info e-mail is also sent if the
"OrderListEntryBooked" telegram contains an incorrect "OrderListReference".



                Restrictions
    •   The new logic is only available for the coupling of an A+W Enterprise stock with a Hegla
        stock. In the coupling with other third-party stocks (Bystronic, Lisec) or with an A+W
        Business stock, the logic is not available.


A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                              60
    •   For the Hegla interface, the interface version 2.3.0.0 or higher must be configured.
        (Interface description in the Hegla document "Warehouse Management System Interface
        2.3.0.0_Rev2 -gb".)
    •   The new logic assumes installation of the A+W ICE environment.
    •   For the new logic, all POs for a coupled Hegla stock must absolutely be entered with
        prices, for goods receipts can only be booked if a price exists.
    •   The entry of the PO items was described above. A batch and an associated cover sheet
        are not linked in the ERP PO. This means that the batch doesn't know about its cover
        sheet and the cover sheet doesn't know about its batch. From the ERP point of view,
        these are completely independent items.
    •   Goods receipts for a PO may not be entered into the Hegla stock via a nightly (cyclical)
        stock reconciliation since otherwise incorrect inventories and under some circumstances
        incorrect prices will arise in the A+W Enterprise stock.
    •   The brief interruption of the socket communication between Hegla system and ERP Stock
        Service due to network problems cannot be prevented. In the worst case, there could be
        data losses here (telegrams are not received in the ERP system). Since this was not
        previously a problem in the operation of the interface, however, it is assumed that with
        the new adjustments, it is not necessary to count on such problems. A mismatch of the
        data on the ERP side would be corrected with the next cyclical reconciliation.
    •   As described above, an info e-mail is sent by the ERP Stock Service if for the Hegla goods
        receipts the ACTUAL quantities deviate from the PO quantities or if the instructions for
        partial goods receipts or goods receipts do not come explicitly from the Hegla system.
        This e-mail contains the PO number, PO item, and quantity deviation. Causes of the
        quantity deviation are not described. The employee in purchasing must learn about the
        causes from the stock employee in another way.



                Search
ERP Stock Service
For search purposes, the trace level of the ERP Stock Service can be adjusted. In the first step, the
trace level should be set as follows:




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                               61
If with this configuration the log is not yet meaningful enough, in the next step the category
"ERPServiceBasis" can be set to "Debut" and the trace level also increased to "Debug" on the
"Panorama" tab.


AWE purchaseservice
The following logs can be used for searching:
awsoa_purchaseservice* (PROTOPFAD)
waein* (PROTOPFAD)
free* (PROTOPFAD)


ftest:
AWSOAFTEST = 9
purchaseservie_*.test


Note about searching
Whether for the goods receipt the focus is on a partial goods receipt or a complete goods receipt
or whether the PO is completed or not can be detected on the database using the flag
"liefkompl":
The value "1" means partial goods receipt or not completed.

A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                             62
The value "2" means complete goods receipt or completed.


 Data                  Partial goods receipt/not completed        Complete goods receipt/completed
 Purchase order        kauf.liefkompl = 1                         kauf.liefkompl = 2
 Associated GR         kauf.liefkompl = 1                         kauf.liefkompl = 2
 GR items              kposp.liefkompl = 1                        kposp.liefkompl = 2




7.8. Particularities of the Lisec stock connection
          Treatment of glass types with inventory "0"
In cyclical stock reconciliation, there is a logic that prevents the inventory reconciliation if no
inventory from the external warehouse is reported for a variant. Since in this case it cannot be
distinguished whether the inventory in the external warehouse is "0" or whether for some
reasons the inventory message for the variant is missing, an e-mail is sent that the inventory
update was not carried out for the variant and it must be done manually.
With PF ticket [AW-198448], the logic for this Lisec stock connection was changed, so that during
cyclical reconciliation, all variants of an article in the ERP stock are set to inventory "0" if for the
external glass type that corresponds to this ERP article, the inventory "0" is reported by the
external warehouse.
The logic is (status as of 07/19/2024) only available with a configuration with A+W Enterprise.
The logic must (status as of 07/19/2024) be activated precisely according to the database. For
this, the env variable STOCK_LISEC_PROCESS_ZERO_GLASSTYPES must generally be set to the
value "ON".
Note: The env variable STOCK_LISEC_PROCESS_ZERO_GLASSTYPES should only be used in the test
phase of this functionality. If the logic works flawlessly, the control over the variable is removed
from the source code so that the functionality becomes standard behavior.
See also PF [AW-198448].




A+W Software GmbH                 EN-CONFIG-A+W ERP Stock Service.docx                                63
8. FAQs
8.1. Conversion of an existing stock to a portal stock
The customer already has two stocks in AWE, can I convert these stocks during
operation to the type "portal stock" without problems and then connect them to a
Hegla stock in the config?
It is not previously known that problems occur when the conversion is undertaken in ongoing
operation. However, it is preferable to perform the conversion when the operation is shut down,
and to perform a stock reconciliation right after the conversion.


8.2. Cover sheets
Is there a recommendation with the Hegla stock connection to work with a separate
cover sheet stock?
There is no recommendation to use a cover sheet stock. The customer must decide whether it
bothers him that in the ERP stock (portal stock) the inventories include cover sheets that are not
recognizable as such. The third-party stock recognizes the cover sheets in any case and knows
whether or not it can use them for production.


If a cover sheet is rebooked in the Hegla stock, from a cover sheet to a normal sheet, is
it (removed from the cover sheet stock and then) (re)booked into the portal stock as
normal sheet?
The "rebooking" is done with the next cyclical reconciliation. There is no immediate rebooking via
telegram by the Stock Service.


When working without GR stock logic and with cover sheet stock, when booking the
goods receipt into the ERP portal stock, a cover sheet could accidentally be booked to
the portal stock instead of the cover sheet stock. What happens then?
The inventories are corrected with the next cyclical reconciliation.




8.3. Correct inventories and average prices
Please explain briefly again why the timely goods receipt bookings are so important and
how this relates to the GR stock logic/PO logic.
With GR stock logic/PO logic
In case of a physical goods receipt (in the portal stock), the third-party stock system obtains the
confirmation of the associated goods receipt booking in AWE. Only once the commercial goods
receipt has been confirmed can removals be made for this goods receipt.


A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                                  64
Thanks to this logic, a deviation of the inventories in the third-party stock system and ERP stock is
prevented. The bookings to the ERP stock are made on goods receipt with the correct price (of the
order) and the removals from ERP stock are then made with the current average price.
During the cyclical reconciliation, the inventories in the ERP stock are adjusted to the inventories
in the third-party stock.
If the inventory of a variant must be increased, the receipt is done at the current average price.
If the inventory of a variant must be reduced, the removal is done at the current average price.


Without GR stock logic/PO logic
The goods receipt in the third-party stock system is uncoupled from the goods receipt in the ERP
stock. For correct inventories and correct prices in the ERP stock, the commercial goods receipt
must be booked for the physical goods receipt in timely fashion. A timely booking prevents
undesired effects such as incorrect inventories and incorrect average prices in the ERP stock. No
problems occur if the first removal booking for a goods receipt in the third-party stock is only
made after the goods receipt was booked in the ERP stock.
To demonstrate these, here are two scenarios that cause an incorrect average price.
Scenario 1:
 Action           Status         ERP stock                                        Third-party stock
                                 Quantity    Book price    Average                Quantity
                                                           price/piece
 Cyclical
 reconciliation
                  Inventories 100                          50                     100
 Goods receipt                                                                    60
 GR-1 in third-
 party stock
                  Inventories 100                          50                     160
 Removal in                                                                       20
 the third-
 party stock
 Removal in                      20          50
 the ERP stock
 via Stock
 Service
                  Inventories 80                           50                     140
 Goods receipt                   60          55
 GR-1 in ERP
 stock
                  Inventories 140                          52,14                  140


Scenario 2:


A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                                 65
 Action           Status         ERP stock                             Third-party stock
                                 Quantity Book price   Average         Quantity
                                                       price/piece
 Cyclical
 reconciliation
                  Inventories    100                   50              100
 Goods receipt                                                         60
 GR-1 in third-
 party stock
                  Inventories    100                   50              160
 Removal in                                                            20
 the third-
 party stock
 Removal in                      20          50
 the ERP stock
 via Stock
 Service
                  Inventories    80                    50              140
 Cyclical
 reconciliation
                  Inventories    140                   50              140
 Goods receipt                   60          55
 GR-1 in ERP
 stock
                  Inventories    200                   51,50           140
 Cyclical
 reconciliation
                  Inventories    140                   51,50           140


Here is the correct booking scenario:
 Action           Status        ERP stock                              Third-party stock
                                Quantity Book price    Average         Quantity
                                                       price/piece
 Cyclical
 reconciliation
                  Inventories   100                    50              100
 Goods receipt                  60           55
 GR-1 in ERP
 stock




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                   66
 Goods receipt                                                                 60
 GR-1 in third-
 party stock
                  Inventories   160                      51,88                 160
 Removal in                                                                    20
 the third-
 party stock
 Removal in                     20         51,88
 the ERP stock
 via Stock
 Service
                  Inventories   140                      51,88                 140




8.4. Installations with A+W Business
         Tables and processes in A+W Business
The following tables are booked in AWB for additions and removals:
SYSADM.FS_POOL_KOPF
SYSADM.FS_POOL
For each addition or removal, a header records with TYP=54 is written to the table
SYSADM.FS_POOL_KOPF.
Added to this is the data record in the table SYSADM.FS_POOL.
The tables FS_POOL_KOPF and FS_POOL are processed by the "AWB Exchange Service" ("AES").


In the Hegla logic, the time stamp of the last booking made is saved in the ERP system.
In AWB, the table SYSADM.LG_LASTBOOKED is used for this.



         Use of imperial dimensions in A+W Business
The ERP Stock Service has been expanded so that it is now also possible to perform the nightly
reconciliation of the stocks on imperial databases. Previously, only the manual addition and
removal worked.
See PF [AW-171618].




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                             67
8.5. awtrc log of the ERP Stock Service
            Orientation in the log
Cyclical reconciliation
To find the entries for cyclical reconciliation, search for "WorkStoreBalance".
To find all bookings made within the cyclical reconciliation, search for "BookStoreBalance".


Booking
To find booking made, search for "TraceBookingItem".
All stock bookings that the ERP Stock Service initiates have the following log entry (exemplary):
AWEStockBooking.BookStockMovement():
---------- ---------- ----------
WLH INSERT: hausnr 934, lnr 1, artnr 15015132, bitnr 1, b_anz 10, b_status 29, b_preis <0,00>
---------- ---------- ----------


OrderListRequest
An "OrderListRequest" only creates a GR booking in AWE if an "OrderListEntryBooked" telegram
comes from the third-party stock that can be processed successfully.


OrderList
To see which "OrderList" is sent to the third-party stock, search for
"HeglaSyncSingle.TraceOrderList"


Open POs
To see which open POs were found, search for
"NeStErpCommunication.TradeAwSoaPurchaseOrders".


OrderListUserEvent
"OrderListUserEvent" initiates either a partial goods receipt (OrderListUserAction=1) or a
complete goods receipt (OrderListUserAction=0).
No information is sent back to Hegla about whether the UserEvent on the ERP side could be
executed correctly.



            PO/Goods receipt logic (Hegla, TechNord, Planning Stock)
Goods receipts are booked by the AWE Purchase Service (Unix service).


A+W Software GmbH                  EN-CONFIG-A+W ERP Stock Service.docx                             68
If necessary, therefore, for research the log of the purchase service must be consulted.




          "inventory type" logging
The logging is done as usual in the awtrace file of the log directory.
For logging of a variant with all available data, the "inventory type" is specified, among other
things. The "inventory type" describes whether this is a removal or an addition (booking in).
During the cyclical comparison, the "inventory type" is not transmitted by the third-party system;
therefore, during logging of the data, "inventory type undefined" is written into the log.
This is not an error, but the expected behavior.



          "Panorama" logging
The ERP Stock Service uses the A+W Panorama interface for socket communication with external
stock systems. (For this purpose, appropriate dlls were incorporated into the ERP Stock Service.)
"Panorama" writes its own log messages, whose form (error, warning, debug) can be configured
using the Config Tool of the ERP Stock Service. The messages are integrated in the ERP Stock
Service log.
The Panorama interface is supported by Techsoft, not A+W Enterprise. Questions that relate to
Panorama log messages that occur in the environment of the Panorama interface are also
handled by Techsoft.




8.6. Hegla log
On the Hegla page, there is the log "SocketComm*.trc".
The asterisk (*) stands as placeholder for a digit. It can be that the digit is the "ClientId". But this is
just an assumption.
What exactly is logged there is unclear. In any case, the log exists.
See also PF [AW-169430].




8.7. Measurement
When the ERP Stock Service starts communication with the external stock, the measurement unit
is also specified in the communication.
Currently, this is always "mm".




A+W Software GmbH                 EN-CONFIG-A+W ERP Stock Service.docx                                  69
8.8. Verification of the connection to the external
   stock
In the Hegla, Bystore, and Lisec stock connection, there is a check at 30-minute intervals whether
the connection to the external stock is intact. If there is no more connection and this cannot be
established again, an info e-mail with a corresponding message is sent.
See PF [AW-217449].




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                            70
9. Troubleshooting
9.1. General
          Installation via the SetupLauncher
Sometimes it happens that during the installation of the ERP Stock Service via the SetupLauncher,
there is an installation error ("General Installer Error"). This probably has to do with the fact that
the already running service cannot be stopped within a defined time range.
In this case, simply reinstall the ERP Stock Service. The second time around, the error message will
not occur.


          Host name of the external stock server cannot be resolved by
        the Stock Service in the IP address
    •    It is safest to store the IPv4 address directly in the configuration
    •    If the string "localhost" cannot be resolved, instead you can also try to assign the host
         name an empty string.
    •    For an explanation, see also MSDN Dns.GetHostAdresses()



          E-mails are not sent
If there is no obvious error in the log, such as a missing recipient address or a missing SMTP
server, you must search in the installation environment for the cause.
Possible sources of error: unknown/incorrect IP address, firewall.



          E-mails from the cyclical stock reconciliation seem to be sent
        twice
Check whether in the Hegla or Lisec connection a cover sheet stock that is identical to the
interface stock is entered in the config tool. If so, remove the cover sheet stock.
See also AWDesk #428744.



          In the ERP system, no more bookings are made
Error pattern:
In the ERP system, no more bookings are made even though the ERP Stock Service is running.




A+W Software GmbH                 EN-CONFIG-A+W ERP Stock Service.docx                               71
The telegrams from the external system are received in the ERP Stock Service, but they are not
processed.
Here are some sample messages that are output for Hegla connection in the ERP Stock Service
log:

…AWDataSource.OpenNewDatabaseConnection(): Opening database exception (type: Informix)
Undefined database error! ERROR [08004] [Informix .NET provider][Informix]Attempt to connect
to database server (alcib) failed. NativeError: -908Informix code -908
Additional statement information: No additional information was given!
Error code: -908
…HeglaSync.PrepareSyncs(): Hegla communication (Stock ID 2) dismissed.
“
And also:
“
…HeglaSync.ProcessTelegram(): Telegram could not be processed. No valid Hegla communication
found.
”
Or:
“
…HeglaSync.ProcessTelegram(): Telegram could not be processed. - No valid communication
configuration found. Check configuration and restart ERP Stock Service.
”
Explanation:
If the ERP Stock Service is started, it reads the DB connection from the associated config file. It
checks for each configured DB connection whether the connect can be established.
If in the customer system the ERP database is "slow", there can be a timeout error when
establishing the connection (Informix code -908).
The ERP Stock Service classifies the DB connection as "invalid" and removes it from the cached list
of DB connections used.
Only when the ERP Stock Service is restarted are all configured connections checked again.
If there is no restart of the ERP Stock Service, the connection that encountered a timeout error
remains invalid and the telegrams for this connection are not processed.

Solution:
The ERP Stock Service must be restarted.
After that, check in the ERP Stock Service whether one of the error messages listed above occurs
again.
See PF [AW-218557].




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                 72
9.2. General - A+W Enterprise
       Records with error status "-4" before the stock booker block
     the cyclical comparison
The wlh error status "-4" indicates that a removal from stock cannot currently be made because
the stock is too low or is zero. As soon as an incoming booking has been made for the article, the
stock has increased so that the removal is possible, the removal will be performed automatically.
The error record doesn't exist anymore then.
The next cyclical comparison can be performed without additional manual intervention.



       Records before the stock booker block the cyclical
     comparison
Check whether another connected system (Dynopt) has reported stockplates to the ERP system.
The Dynopt report can be deactivated in xopton.cfg with the switch WriteXoptRueckmeldung=0.
See also [AW-112396].



         Variant is not found in AWE: "No valid variant ID found"
If a variant reported by the external stock in AWE is not found, this can have various causes.
The determination of the variant is done by execution of the SP "wlgetbitnr". Here, taking into
account a deviation (Delta), the glass dimension in the table xxvar (xxvar.bitnr) and the associated
stock variant in the table artvarzu is selected.
If no variant can be found, the table entries in xxvar and artvarzu must be checked.



         AWE articles are not found
Check whether the third-party system product code is stored as customer article of the stock
market partner in the AWE master data (table artkuzu).
Until 05/29/2024: Check whether the AWE article has been discontinued. (See AWDesk #453436.)
Starting in June 2024: Bookings and stock comparison are permitted for discontinued articles. The
still flag from the artikel table will NOT be heeded. (See PF [AW-192587].)




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                             73
9.3. General - A+W Business
          Cyclical reconciliation causes incorrect inventory
Is A+W Business configured with the dimension unit "inch"?
See PF [AW-161492].




9.4. Hegla connection
           The Stock Service cannot establish a connection to the Hegla
        stock server

          Problems with connection data
Check connection data (IP address, port number). Perhaps the port has to be released.


          Problem with the Hegla interface version
The Hegla interface version that was set in the config tool of the Stock Service is not compatible
with the version of the connected Hegla server.
The effect is that during establishment of connection to the Hegla server, an error message is
returned. The error message is only visible in the log if in the config tool of the Stock Service, the
trace level of "Panorma" is set to info.
Message in the log:
Hegla stockmaster client | "RECV: SetMsgError;MsgId=2;ReplyMsgId=50001;Error=4


Solution: either the Hegla interface version in the config tool of the Stock Service must be
converted or the Hegla server must be adjusted.
See also AWDesk #428744.


          LogOn
The ERP Stock Service transfer to the Panorama interface
    -    IP
    -    Port
    -    Client ID
    -    Interface Version
    -    Measurement



A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                74
The "DateTimeFormat" is specified by the Panorama interface and transferred to the Hegla
server.


Examples from the ERP Stock Service log:
… "----- HeglaSync.GetSocketCommIf(): IP 10.2.52.162, port 10010, client ID 1 " …
| Panorama              |…| Hegla stockmaster client | "SEND:
LogOn;MsgId=50001;ClientId=1;InterfaceVersion='LV.2.3.0.0';Measurement=0;DateTimeFormat='
dd.mm.yyyy hh:nn:ss' " …



        During communication with the Hegla server, there is a
     timeout
Symptoms:
In the interface log HeglaStockmasterComm.txt there is an appropriate entry, e.g.:
05-09-2013 13:56:57 error, Albwir.Edi.StockService: HeglaSyncSingle.ProcessTelegram(): Time
out in GetRackLoading [XMME]


05.09.2013 13:56:27.208 Info | HeglaStockmasterClient(10.22.0.192:10010): SEND:
GetRackLoading;MsgId=50101;Location=18;
05.09.2013 13:56:27.520 Info | HeglaStockmasterClient(10.22.0.192:10010): RECV:
SetMsgError;MsgId=102;ReplyMsgId=50101;Error=50;


Solution:
The cause is probably a DB problem with the Hegla server.
There can be inconsistent data (e.g. articles booked on racks that are not present in the glass data
table).
The precise analysis and troubleshooting can only be done by Hegla. To solve the problem, you
must contact Hegla Customer Service.
Caution: Hegla requires the time of the error and the Hegla error code for analysis of the
problem. Both details are in the ERP Stock Service log (*.awtrc) at the point where the timeout
error is logged.



            Error when parsing the Hegla telegram
Solution:
In most cases, the telegram must be adjusted by Hegla. To solve the problem, you must contact
Hegla Customer Service and describe the error pattern.




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                              75
The entry in the ERP Stock Service log generally looks like this:
"stockmaster client | "ReadTelegrams(): ErrorMessage=HeglaTelegram.Parse: Telegram is not
parsed correctly…"
Here is a complete sample log message:
********
2019-05-10 11:50:10.282 | [21492] | [0x0000000A] | ERROR | Panorama               | IP\SYSTEM
| (null)    | Hegla stockmaster client | "ReadTelegrams(): ErrorMessage=HeglaTelegram.Parse:
Telegram is not parsed correctly
InventoryChangeEvent;MsgId=40;InventoryType=5;ArticleCode='30634';Width=6000.00;Height=3
210.00;Thickness=9.00;Quality=0;Amount=1;SourcePos=30;SourceItemIndex=0;DestPos=32;Booki
ngDateTime='10.05.2019 11:50:42';DeliveryOrderNr1='Bestand';DeliveryOrderNr2='Keine
Angabe';DeliveryOrderNr3=' ';DeliveryOrderNr4='
';SequenceNumber=0;OptNumber=0;OPT_Variante='0
';OPT_Teilenummer='0                             ' [XMME10003]. Telegram could not be read
[XMME]:
InventoryChangeEvent;MsgId=40;InventoryType=5;ArticleCode='30634';Width=6000.00;Height=3
210.00;Thickness=9.00;Quality=0;Amount=1;SourcePos=30;SourceItemIndex=0;DestPos=32;Booki
ngDateTime='10.05.2019 11:50:42';DeliveryOrderNr1='Bestand';DeliveryOrderNr2='Keine
Angabe';DeliveryOrderNr3=' ';DeliveryOrderNr4='
';SequenceNumber=0;OptNumber=0;OPT_Variante='0
';OPT_Teilenummer='0                             ';Crc=0x26E34BC1 " | " " | " " |
********


9.4.6.1. No double quotation marks
The reason for the error message is that the string values, especially the date specifications of the
telegram are enclosed in single quotation marks. The interface expects double quotation marks,
however.
Solution:
The telegram can only be adjusted by Hegla.
See also AWDesk #443136.


9.4.6.2. Optional values
Optional (customizing) telegram values can cause problems with parsing in connection with
"BookingDateTime".
Solution:
The telegram can only be adjusted by Hegla.
See also AWDesk #443136.




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                              76
9.4.6.3. Optional values in the middle of the telegram
Optional (customizing) telegram values in the middle of the "InventoryChangeEvent" telegram can
cause problems when parsing.
This has happened with the optional parameters "Type=0;Orientation=0".


The misleading error message is:
2024-09-03 03:53:44.610 | [7024] | [0x0000003F] | ERROR Hegla stockmaster client |
"ReadTelegrams(): ErrorMessage=HeglaTelegramParameter.Parse: Invalid
parameter=0;Orientation=0;DeliveryOrderNr1='1111111';DeliveryOrderNr2='
';DeliveryOrderNr3=' ';DeliveryOrderNr4=' ';SequenceNumber=0;OptNumber=0 ErrMsg=Str2TVal:
String is not masked with double quotes. [XMME10034] [XMME10008]. Telegram could not be
read [XMME]:
InventoryChangeEvent;MsgId=61;InventoryType=4;ArticleCode='20114';Width=6000.00;Height=3
210.00;Thickness=4.00;Quality=0;Amount=1;SourcePos=1;SourceItemIndex=0;DestPos=1002;Boo
kingDateTime='03.09.2024
03:53:45';Type=0;Orientation=0;DeliveryOrderNr1='1111111';DeliveryOrderNr2='
';DeliveryOrderNr3=' ';DeliveryOrderNr4=' ';SequenceNumber=0;OptNumber=0;Crc=0x697712D1
"|""|""|


Solution:
The telegram can only be adjusted by Hegla.
See PF [AW-202313].



9.4.6.4. Invalid parameter – value UInt32 too large/small
The entry in the ERP Stock Service log is:
„ stockmaster client | "ReadTelegrams(): ErrorMessage=HeglaTelegramParameter.Parse: Invalid
parameter …“
Here is a complete sample log message:
********
2020-06-16 06:56:14.040 | [2968] | [0x00000008] | ERROR | Panorama                 |
HOFFMANNGLAS\SYSTEM | (null)           | Hegla stockmaster client | "ReadTelegrams():
ErrorMessage=HeglaTelegramParameter.Parse: Invalid
parameter=SourcePos=26;SourceItemIndex=0;DestPos=0;BookingDateTime='16.06.2020
07:01:06';DeliveryOrderNr1=' ';DeliveryOrderNr2=' ';DeliveryOrderNr3=' ';DeliveryOrderNr4='
';SequenceNumber=0;OptNumber=0 ErrMsg=The value for a UInt32 was too large or too small.
[XMME10008]. Telegram could not be read [XMME]:
InventoryChangeEvent;MsgId=628;InventoryType=2;ArticleCode='';Width=3000.00;Height=40.00;
Thickness=20.00;Quality=0;Amount=-
1;SourcePos=26;SourceItemIndex=0;DestPos=0;BookingDateTime='16.06.2020
07:01:06';DeliveryOrderNr1=' ';DeliveryOrderNr2=' ';DeliveryOrderNr3=' ';DeliveryOrderNr4='
';SequenceNumber=0;OptNumber=0;Crc=0xEE093DA0 " | " " | " " |



A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                       77
********
The “ArticleCode” is missing (probably not the problem) / "Amount" is < 0
Solution:
The telegram can only be adjusted by Hegla. To solve the problem, you must contact Hegla
Customer Service.
See also PF [AW-41499].

The socket interface was adjusted with PF ticket [AW-109536] so that a negative "Amount" no
longer causes an error message.


Other case:
„
2024-10-18 08:24:13.456 | [17268] | [0x00000008] | ERROR | Panorama                |
SCHOLLGLAS\awservice59 | (null)       | Hegla stockmaster client | "ReadTelegrams():
ErrorMessage=HeglaTelegramParameter.Parse: Invalid
parameter=Type=0;DeliveryOrderNr1='212297';DeliveryOrderNr2=' ';DeliveryOrderNr3='
';DeliveryOrderNr4=' ';BookingDateTime='2024-09-04 10:05:03' ErrMsg=The value for a UInt32
was too large or too small. [XMME10008]. Telegram could not be read [XMME]:
GetRackLoadingResult;MsgId=28;ReplyMsgId=98826;MaxCount=3;ActCount=3;ArticleCode='1040
0';Width=6000.00;Height=3210.00;Thickness=4.00;
Quality=100;Location=1;ItemIndex=3;Amount=8;Available=-
1;Type=0;DeliveryOrderNr1='212297';DeliveryOrderNr2=' ';DeliveryOrderNr3='
';DeliveryOrderNr4=' ';BookingDateTime='04.09.2024 10:05:03';Crc=0x58C2EAD5 " | " " | " " |
“
In "Available" a negative value occurs in the telegram. In the Hegla interface description, the
following is documented:




       A booking is rejected because it supposedly has a time stamp
     that is too old.
Solution 1:
Check time on the Hegla server and on the computer on which the ERP Stock Service is running.
Both servers have to run synchronously so that the checking of the time stamp works correctly.
See also PF [AW-58648].




A+W Software GmbH               EN-CONFIG-A+W ERP Stock Service.docx                              78
Solution 2:
The reconciliation time stamp from (wlportalsync (AWE) or SYSADM.LG_LASTBOOKED (AWB)) is
incorrect for some reason.
The incorrect record must be deleted from the table.
See also PF [AW-161492].



          Store Balance - No external inventory for ERP item announced

9.4.8.1. External inventory is "0"
This is the standard behavior, not an error.
See also "ERP variants without external correspondence".



9.4.8.2. Checking glass thicknesses
The glass thicknesses in the ERP system and in the Hegla system do not match.
In A+W Enterprise, the glass thickness is stored in the artikel.staerke field.
See also PF [AW-139939].



          Apparently deviating quantities in ERP and Hegla
During a comparison of the quantities of a variant in the ERP system and in the Hegla stock, the
cover sheets in the Hegla stock may not be overlooked. If in the ERP system you are working
without special cover sheet stock, it can otherwise seem that the inventories of a variant do not
match.
See also PF [AW-170630].



                PO logic: empty order list in Hegla
When working with PO logic, the "Use AWSOA" checkbox must be activated in the Config Tool of
the ERP Stock Service in the AWE database connection. When the box is checked, the Config Tool
checks whether the connection to the required AWE purchaseservice can be established.
If the connection cannot be established, a corresponding message is displayed and the "Use
AWSOA" checkbox is disabled automatically so that the entire PO logic is also disabled.
As a result, the ERP Stock Service relies on the configured goods receipt stock as soon as Hegla
sends an "Order List Request" to the Stock Service.
Since with this error pattern, there is generally no goods receipt stock configured, the following
messages occur in the ERP Stock Service log:


A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                                79
…
HeglaSyncSingle.WorkOrderListRequest(): No goods receipt stock -> empty order list sent
HeglaSyncSingle.TraceOrderList(): No order list items exist.
HeglaSyncSingle.WorkOrderListRequest(): OrderList is empty.
…
The Stock Service cannot provide any order list to Hegla as long as the configuration has not been
corrected.
See also PF [AW-147994].



                PO logic: open POs missing in the Hegla display
By activating the env variables AWSOA_SMC_PO_FROMRO"UTEONLY, a restriction with regard to
the route becomes active.
So that the open POs are displayed correctly in Hegla, the current version of the AWE
purchaseservice must be installed.
See also PF [AW-169430].



            PO logic: good receipts from Hegla do not arrive in the
     ERP Stock Service
With the Hegla interface version 2.3.0.0, the PO logic was made to run successfully in a customer
installation.
For an additional installation, there were then problems with the telegrams sent by Hegla.
Message from Hegla about this (02/08/24): "It seems as if the server in ... were incorrect since it
does not itself hold to the log. For in the version 2.3.0.0, the parameter is defined, but it is not
sent along."
The problem can only be solved on the Hegla side.
See PF [AW-169430].



            PO logic: goods receipts from Hegla include a corrupt
     OrderListReference and can therefore not be booked in the ERP
     Stock Service
Due to an update on the Hegla server, it can happen that the telegrams for the goods receipts are
broken. They contain an incorrect OrderListReference and cannot be booked.
The problem can only be solved on the Hegla side.
See PF [AW-199683].




A+W Software GmbH                EN-CONFIG-A+W ERP Stock Service.docx                              80
           PO logic: log message "Error code 6, message:
     Authentication failed."
The purchaseservice (Unix) must be checked.
-> Check in the log whether the DB connect could be established.


Error message in the log of the purchaseservice:
10:42:20: D purchaseserver::Login(User alcim, *) called
10:42:20: D Logfile wrote for AppID=purchaseserver with ReturnCode=0
10:42:20: D awsoabasis::ValidateUser called!
10:42:20: D awsoabasis::ValidateUser: Selecting User number
10:42:20: E awsoabasis::ValidateUser: Selecting User number failed: SC: -404, SCISAM: 0
10:42:20: D purchaseserver::Login() User and/or Password does not match
10:42:20: D purchaseserver::Login() done
10:42:20: D
10:42:20: D purchaseserver::GetOpenPurchaseOrders(From 4.12.2024, To 25.12.2024) called
10:42:20: D awsoabasis::ValidateAuthenticationToken token = 0, user = alcim,
machine:process=PS-BERLIN:4312, ClientVersion=Not Specified (<= 2.7.43)
10:42:20: D awsoabasis::GenerateAuthenticationToken token=5300
10:42:20: E Authentication failed.


Error message in ERP Stock Service log:
2024-12-11 11:42:26.235 | [152460] | [0x00000007] | INFO | ERPStockService             |
SCHOLLGLAS\awservice59 |           |      |
"NeStErpCommunication.GetOpenPurchaseOrders(): call
GetOpenPurchaseOrdersForStockLocation() (1) " | " " | " " |
2024-12-11 11:42:26.281 | [152460] | [0x00000007] | ERROR | Core                 |
SCHOLLGLAS\awservice59 |           |      | "Error Code 6, Message: Authentication failed. " | "
An exception occured:
Type: AWSOA.Core.Exceptions.CoreException
Message: Authentication failed.
Source: mscorlib
Auto-Traced in constructor: at AWSOA.Core.Exceptions.CoreException..ctor(Int32,
System.String, System.Exception)
  at System.RuntimeMethodHandle.InvokeMethod(System.Object, System.Object[],
System.Signature, Boolean)
  at System.Reflection.RuntimeConstructorInfo.Invoke(System.Reflection.BindingFlags,
System.Reflection.Binder, System.Object[], System.Globalization.CultureInfo)


A+W Software GmbH                 EN-CONFIG-A+W ERP Stock Service.docx                        81
  at System.RuntimeType.CreateInstanceImpl(System.Reflection.BindingFlags,
System.Reflection.Binder, System.Object[], System.Globalization.CultureInfo, System.Object[],
System.Threading.StackCrawlMark ByRef)
  at System.Activator.CreateInstance(System.Type, System.Reflection.BindingFlags,
System.Reflection.Binder, System.Object[], System.Globalization.CultureInfo, System.Object[])
  ...
"|""|




A+W Software GmbH              EN-CONFIG-A+W ERP Stock Service.docx                             82

