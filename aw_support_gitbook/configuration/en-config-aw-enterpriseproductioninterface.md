---
title: "EN CONFIG A+W EnterpriseProductionInterface"
category: "configuration"
product: "A+W EnterpriseProductionInterface"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W EnterpriseProductionInterface"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration                       _    A+W Enterprise 6 Production Interface                                       english                               - -INTERNAL- Change history           Date        Author   Remarks                                                 Version                              #314985: Ignore kmodparam.refflag for whole glass         2013-03-14 PG        systems. New section „Ganzglasanlagen und               2012.1_13                              Modelldaten“"
source_file: "EN-CONFIG-A+W EnterpriseProductionInterface.pdf"
---


# EN CONFIG A+W EnterpriseProductionInterface

      Configuration
                      _



A+W Enterprise 6
Production Interface




                                  english




                          - -INTERNAL-
Change history


        Date        Author   Remarks                                                 Version
                             #314985: Ignore kmodparam.refflag for whole glass
        2013-03-14 PG        systems. New section „Ganzglasanlagen und               2012.1_13
                             Modelldaten“
                             #288831: Evaluation of
                             AWC_ANGEBOT_DEF_TERMIN to determine the
        2013-01-10 PG                                                                2012.1_12
                             default date                          for
                             quotations without appointment specification.
                             #278789: If switch MODUL_DOPPELSCHICHT is active,
        2013-11-15 PG        all installation positions at lower levels        2012.1_11
                             are evaluated in a simple glass hierarchy.
                             #292040: New section <ORDER -
        2013-11-05 PG        USER_DEFINED_EXTENSIONS - UDXAWORDERINFOS - 2012.1_10
                             ERP_INFOS>
                             #267331: DB field name macroname is now file name

                             DATEI_REF_PFAD replaces also
        2013-08-22 PG                                                                2012.1_9
                             SN_MAKRO_BASISPFAD and SN_MOTIV_BASISPFAD

                             #280668: Treatment of sting fields, that are NULL
                             Patch 5.2
                             #201980: New processing type 1910 surface macro
        2013-08-01 PG                                                                2012.1_8
                             #267331: Addtional motif parameter for surface
                             processings 1200, 1205, 1210, 1215, 1220, 1225
                             Due to #281878: Explicit spacer geometries
                             (steps/back cuts) can alos be transferred if variable
        2013-07-09 PG                                                                2012.1_7
                             ISO_RAHMEN_MODELL is set (not only for
                             MODUL_VERSIEGELUNGSTIEFE)
                             Due to #274633: SP cuxmltransfer can prevent that
                             an order is transferred (see chapter 0 „Übergabe
                             verhindern“)
        2013-05-23 PG                                                                2012.1_6
                             Due to #289718: For processings with
                             <...PROCESSING - side> is filled with the layer
                             information
                             Due to #276862 Correction 1.8 „Anhang: A+W-
        2013-04-10 PG        Bearbeitungstyp-Informationen“: Processing              2012.1_5
                             parameter A/B for corner processings exchanged.
                             Chapter Fehler! Verweisquelle konnte nicht
                             gefunden werden. „Fehler! Verweisquelle konnte
        2013-03-22 PG        nicht gefunden werden.“ extended because the            2012.1_4
                             performance declaration number was transferred as
                             item text (due to AWDesk 274142)



A+W Software GmbH   EN-CONFIG-A+W EnterpriseProductionInterface.docx                       2
        Date         Author   Remarks                                               Version
                              Disable item split extended in chapter 1.4.7
        2013-03-05 PG                                                               2012.1_3
                              „Positionssplit“ (due to AWDesk 275242)
                              0 „XSD-konforme OrderXML-Dateien“ (due to
        2013-02-26 PG                                                               2012.1_2
                              AWDesk 251817)
                              Notes regarding processing type 1900 (due to
        2012-11-30 PG                                                               2012.1_1
                              AWDesk 264532)
        2012-10-25 PG         Original edition for version 2012.1 (AWDesk 199448)   2012.1
        2017-11-01 SVH        Internal site separation                              6
        2017-01-15 RS         Change of site allocation in the order
        2018-05-14 SVH        Weight of main and sub parts
        2018-05-16 RS         Feedback chapter extended
        2018-05-17 RS         Status allocation rack feedbacks
        2018-05-23 SVH        Cost centers / Cost calculation
                              PMVERSANDSTEUER and
        2018-06-04 RS
                              AWC_GESTZU_BUCHEN_OHNE_VERPACKTMELDUNG
                              Adjustments to the extended workbench (AWDesk
        2019-06-17 SVH
                              #439718)
                              New adjustments to the extended workbench
        2019-07-22 SVH
                              (AWDesk #439718)
        2019-08-26
                     SVH      Description AWC_ERPDOC_FILE

                              Adjustments to the extended workbench (AWDesk
        2019-10-02 SVH
                              #451780)
        2019-11-21 SVH        UV protection (awtyp 1650) (AWDesk #454284)
        2019-11-28 SVH        Other articles (atyp 999) (AWDesk #454469)
        2020-04-03 SVH        Addition to meta elements with extended workbench
                              Bestewun lock logic + UPDATE_KAUF_BEI_BEST
        2020-05-06 RS         added


        2020-07-20 TS         AWC_IGNORE_AWERACKSTATUS added
        24.07.202    TS       Flow for rack bookings: (#459400)
                              Distinction of configured and non-configured
        2020-09-21 SVH
                              processing parameters (AWDesk #456954)




A+W Software GmbH    EN-CONFIG-A+W EnterpriseProductionInterface.docx                        3
Content

1.   Transfer to OrderXML                                                    7
     1.1. General Information                                                7
           1.1.1. Amendments compared to the previous version                7
     1.2. Process Overview                                                   8
           1.2.1. In ALCIB                                                   8
           1.2.2. Windows Service                                            8
           1.2.3. Details                                                    9
     1.3. Installation and configuration                                    16
           1.3.1. Configuring the process                                   16
           1.3.2. Fileless transfer via AWSOA Planning Import Service       19
           1.3.3. Starting the process                                      19
           1.3.4. Updating to a higher version                              19
           1.3.5. Tracing                                                   20
           1.3.6. Activation in ALCIB                                       22
           1.3.7. Technical data                                            24
     1.4. Environment variables                                             25
           1.4.1. ORDERXML_NOSTOCKPLATES                                    25
           1.4.2. ORDERXML_PROCPOSTDEF_LEVELDOWN                            25
           1.4.3. ORDERXML_ENDCUSTOMER_DETAILS                              25
     1.5. Information in OrderXML                                           25
           1.5.1. How to read the documentation text file                   26
           1.5.2. OrderXML files                                            27
           1.5.3. Gathering information on elements                         32
           1.5.4. Determination of processing information                   53
           1.5.5. Customised information                                    61
           1.5.6. ALCIB Environment switch                                  78
           1.5.7. Item split                                                83
           1.5.8. Cancellation                                              84
           1.5.9. References in reports                                     85
          1.5.10. OrderXML files for purchase orders                        86
          1.5.11. OrderXML transfer just for production cost calculation    88
          1.5.12. Items with supply type "none" in the OrderXML interface   89
          1.5.13. Ordered glass                                             90
          1.5.14. End customer information                                  90
     1.6. Internal site separation                                          91
          1.6.1. Company change in the order after transfer to AWP          91
     1.7. A+W Processing Types                                              93
          1.7.1. UV protection (awtyp 1650)                                 93
          1.7.2. Configure/non-configured processing parameters             94
     1.8. AWE item types                                                    94
          1.8.1. Other articles (atyp 999)                                  94
     1.9. Extended Workbench (EWB)                                          94
     1.10. Interesting facts                                                95
           1.10.1. Error reports in the Windows service log                 95
           1.10.2. No orders are processed                                  96
           1.10.3. List of form vectors                                     96
           1.10.4. Invalid special characters                               97
           1.10.5. Manual transfer of orders                                97




A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx         4
           1.10.6. Processing step assembly or cutting                                       97
           1.10.7. If the database is inaccessible                                          100
           1.10.8. Glass door systems and shape data                                        101
           1.10.9. Weight of main and sub parts                                             101
     1.11. Other documents                                                                  102
     1.12. Annex: A+W processing Type Information                                           103
2.   AWP Connection                                                                         106
     2.1. Overview                                                                          106
          2.1.1. Motivation and goals of this development                                   106
          2.1.2. Components of the connection                                               106
          2.1.3. Process description of the connection                                      107
     2.2. Functions                                                                         108
          2.2.1. Postponement of delivery date                                              108
          2.2.2. Calculation of dates for the receipt of goods                              109
          2.2.3. Order generation                                                           110
          2.2.4. Cost calculation                                                           115
          2.2.5. Stock forecast                                                             115
          2.2.6. Consideration of item splits when the successful scheduling is confirmed   116
          2.2.7. Status confirmations production                                            117
          2.2.8. Status feedback racks                                                      118
          2.2.9. Provision of cost centers                                                  121
          2.2.10. Treatment of orders with high priority (AWDesk #447496)                   121
     2.3. Data structure                                                                    121
          2.3.1. awc_bestproto                                                              121
          2.3.2. awc_fertigmeldungen                                                        121
          2.3.3. awc_modparams                                                              122
     2.4. Environment variables                                                             122
          2.4.1. AWC_ALCIM_ANBINDUNG                                                        122
          2.4.2. AWC_ART_HZEIT (PMCHZEITART)                                                122
          2.4.3. AWC_MIN_HZEIT_KUNDE (PMEDASCHMINHZEITKUND)                                 122
          2.4.4. AWC_MIN_HZEIT_LIEFERANT (PMEDASCHMINHZEITKUND)                             122
          2.4.5. AWC_DEF_ROUTENABFAHRT (PMEDASCHROUTENABFAHRT)                              122
          2.4.6. AWC_BESTELLEN_BIS (PMEHEUTEBZEIT)                                          122
          2.4.7. AWC_FIXIERT_AB (similar to PMXCIMRMSTATI)                                  123
          2.4.8. AWC_FREIGEGEBEN_AB (similar to PMXCIMRMSTATI)                              123
          2.4.9. PMVERSANDSTEUER                                                            123
          2.4.10. AWC_URL_PRODUKTIONSBERICHT                                                123
          2.4.11. AWC_GESTZU_BUCHEN                                                         123
          2.4.12. AWC_GESTZU_BUCHEN_OHNE_VERPACKTMELDUNG                                    123
          2.4.13. AWC_IGNORE_PACKINGMESSAGE                                                 123
          2.4.14. AWC_IGNORE_AWERACKSTATUS                                                  124
          2.4.15. AWC_WAEIN_UEBERMITTLUNG                                                   124
          2.4.16. AWC_BUCHE_KPOSPROD                                                        124
          2.4.17. AWC_ALCIB_SERVER_NAME                                                     124
          2.4.18. AWC_PORT_RPC_DIENST                                                       124
          2.4.19. AWC_PORT_CONTROL_SERVER                                                   124
          2.4.20. AWC_IGNORIERE_GESTELLMELDUNG                                              124
          2.4.21. GESTELL_BDE                                                               124
          2.4.22. AWC_RACKSTOCK_REGPOINT_TYPE                                               125
          2.4.23. AWC_NACHBEST_MANR                                                         125



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                         5
        2.4.24. PMEINBTERMINAENDMANR                                                    125
        2.4.25. PMEZKBESTELLT                                                           125
        2.4.26. SPLIT_POSKOST_COSTS                                                     125
        2.4.27. BEST_LOCK_TEST                                                          125
        2.4.28. BEST_LOCK_TEST_SPERRE                                                   126
        2.4.29. KAUFUPDATE_BEI_BEST                                                     126
   2.5. Switch in ALCIM                                                                 126
        2.5.1. Switch for loading OrderXML files.                                       126
        2.5.2. Switches without Common base                                             127
        2.5.3. Additional ALCIM switches for ALCIB-ALCIM communication                  128
   2.6. System messages                                                                 130
        2.6.1. Status 73 - Scheduling or rescheduling failed                            130
        2.6.2. Status 74 - Postponement of delivery date                                130
        2.6.3. Status 43 - A broken product contains purchase order parts which have to be
        reordered                                                                       130
   2.7. Logging                                                                         130
        2.7.1. Report (CompleteScheduling) about the ERP Webservice                     130
   2.8. Appendix                                                                        130
        2.8.1. Stock forecast in version 2009 and configuration options                 130
        2.8.2. Generation of remake purchase orders                                     131
        2.8.3. Workflow of background processes                                         134




A+W Software GmbH     EN-CONFIG-A+W EnterpriseProductionInterface.docx                        6
1. Transfer to OrderXML
1.1. General Information
This document describes the general process of creating OrderXML files based on ALCIB
information. This document requires knowledge of the internal processes and data structures in
ALCIB (A+W Enterprise 5). This document is therefore meant only for project engineers, not for
customers.
OrderXML files are used to transfer order/quotation data to other systems by means of a defined
interface. This version (available on the basis of A+W Enterprise 5 (ALCIB 2012.1)) allows to
transfer the order and quotation data to a production system, e.g. ALCIM.
The transfer to ALCIM necessitates ALCIM-Capacity. This replaces PMS and the direct data import
into ALCIM completely.
This is the basis for information which will be found in the OrderXML files and also for the
information gathered by means of direct data import. All data are directly loaded from A+W
Enterprise 5 (ALCIB), not from PMS.
This document also handle the subject of data gathering.
Terminology: OrderXML files can be created for orders as well as for quotations if configured
accordingly. To simplify matters, we are going to use only the term 'orders' while meaning both
orders and quotations. We will draw your attention to any distinctions should they be necessary.

Creating OrderXML files for purchase orders is a special feature however which shall be dealt with
in a separate chapter.


1.1.1. Amendments compared to the previous version
This chapter briefly lists the main amendments as compared with the previous version, 2011 (3.6).
    •   The A+W Enterprise 5 OrderXML service is based on ALCIB database version 2012.1.
    •   The service's configuration tool automatically makes the necessary Informix Setnet
        entries. The ODBC data source is set up at the same time.
    •   If a patch is installed within this version, a previous uninstallation of the service is no
        longer necessary; provided the service is installed via the A+W-Setuplauncher.
    •   AW processing type 1900 (SN macro) can be imported
    •   The switch PMEHANDLE_GERADE_EP is assumed to be active by default so that the BOM
        below an element with an even assembly position will be transferred in reverse sequence.
    •   ORDERXML_VERSION="5.0" indicates that ALCIM can validate the OrderXML file; it is XSD
        compliant. Requires current ALCIM and current OrderXML service (ID 12.1.2).
    •   The item split based on the kposgest data can be switched off using the switch
        ORDERXML_IGNORIERE_KPOSGEST (from version ID 12.1.3).
    •   The AW processing type 1910 (SN surface macro) can be used, provided ALCIM and ALCIB
        are from service pack 5.2 (from version ID 12.1.8, switch ORDERXML_VERSION must be
        set to "5.1").




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                            7
    •    Transfer of SN motif parameters for processing types 1220, 1205, 1210, 1215, 1220, and
         1225, provided ALCIM and ALCIB are from service pack 5.2 (from version ID 12.1.8, switch
         ORDERXML_VERSION must be set to "5.1").
    •    Section <ORDER - USER_DEFINED_EXTENSIONS - UDXAWORDERINFOS - ERP_INFOS> will
         now be filled. This means for the transfer to ALCIM, that a user and an entry date are
         transferred to ALCIM (available as of version ID 12.1.10).
    •    Up to now, the current date was transferred for quotations without an appointment
         specification. To avoid a general shift in A+W Capacity, today's date plus 14 days will be
         transferred in the future. Switch AWC_ANGEBOT_DEF_TERMIN can be used to define a
         different number of days (available from version ID 12.1.12).

Information on Version Changes

If the ALCIB version is 2012.1, the OrderXML service should be updated as well in order to use all
new functions. If this is impossible for internal reasons, OrderXML service version 2011 can still be
used but new functions may be missing. On the other hand, the OrderXML service version 2012.1
cannot be used in connection with a lower ALCIB version because of the changed structures in
ALCIB which are completely supported by the OrderXML service.


1.2. Process Overview


      ALCIB                             ALCIB OrderXML
     Datenbank                                                    OrderXML
                                          (Windowsservice)
  (Datenbankprozess)

                                                                             Ausgabeverzeichnis


Fig. 1: The process in general

The above graph shall visualise the general process.


1.2.1. In ALCIB
After an order or quotation is changed in ALCIB, a record with the order number is written in
transfer table ottransfer.
The table is a mere transfer table. This means. the entries just say that an OrderXML has to be
created for a certain order number.


1.2.2. Windows Service
On a Windows PC, the service A+W Enterprise 5 OrderXML must be started. This service takes
over the control.
    •    It checks if there is an order ready to be processed. If so, information is loaded from the
         ALCIB tables and compiled in OrderXML format.



A+W Software GmbH           EN-CONFIG-A+W EnterpriseProductionInterface.docx                           8
    •   The Windows service saves this information in an OrderXML file.
    •   Successfully processed, the order record is deleted from the transfer table or, in case of
        an error, the record is marked by an error status.
This process is repeated as long as there are orders to be processed. If no order left to be
processed, the Windows service switches to waiting mode. After a - configurable - wait, the
service checks again whether there are orders to be processed.
The OrderXML service directly imports from the ALCIB database. For reasons of performance, it
should therefore be installed on the server of the ALCIB database. Please also note that the
OrderXML service needs writing rights to write the files. Access rights to the target directory must
not be switched off by the Firewall.


1.2.3. Details
Transfer Tables

So far, just one transfer table has been mentioned. Actually, there have to be three tables which
have to be filled to guarantee the running of the process. These are:
    •           Ottransfer: This is the actual transfer table which defines the orders for which
                OrderXML files have to be created.
    •   Ottranssav: Serves for internal control of order cancellations. An order cancellation does
        not have to be transferred for instance if the order had not been transferred. In
        connection with internal site separation, the program notes the number of the site that
        was the last to receive the order.
    •   Ottranszus: ALCIB can provide the OrderXML service with additional information.
The following sub-chapters describe the tables in detail.

Tranfer table ottransfer

The table ottransfer is a global transfer table which is now also used for the OrderXML functions.
An entry in this table informs the OrderXML service of the orders for which a OrderXML files shall
be written.
If this is successful, the record is deleted from the table. In case of an error, the record gets an
error status.
The table consists of the following fields:
    •   Ordno             Number of the quotation or order
    •   Document          5 if the document is an order
                          4 if it is a quotation
    •   Interface       Defines the interface for which this entry is meant. Orders for the
        OrderXML interface are marked by the text ‚ORDXML’.
    •   Control flag Processing status:
                          0: ready for processing
                          1: being processed



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                             9
                    400: Data completely read, Windows service to create the file
                    Statuses over 400 indicate an error:
                    401: Error while selecting from table kauf
                    402: Error while selecting from table kpos
                    403: Error while selecting from table kposp
                    404: Error while selecting from table kposgest
                    405: Error while selecting from table aufstrukt
                    406: Error while selecting from table kspross
                    407: Error while selecting from table poszu
                    408: Error while selecting from table kmodparam
                    409: Error while selecting from table kstufparam
                    410: Error while selecting from table ksprpar
                    411: Error while selecting from table kaufref
                    412: Error while selecting from table ktechw
                    413: Error while selecting from table ottranssav
                    414: Error while selecting from table ottranszus
                    433: Error while selecting from table alsysinfo
                    434: Error while selecting from table modelle
                    435: Error while selecting from table xfarbe
                    436: Error while selecting from table xxfarbe
                    437: Error while selecting from table artvermass
                    438: Error while selecting from table xsprzu
                    439: Error while selecting from table route
                    440: Information status: For purchase orders, the "customer number"
                    must be specially determined. If
                           this does not work, the OrderXML file will still be created.
                           The customer information has to be checked though.
                    458: Can only happen if items with supply type
                           'none' shall not be transferred. For orders
                           which include only items with supply type 'none',
                           no OrderXML file will be created. The order will be marked
                           by this number.
                    459: Error while compiling the item data
                    460: Program error while compiling the data
                           for the node ORDERType and following.
                    461: Program error while compiling the data
                           for the node ORDER_INFO and following.
                    462: Program error while compiling the data
                           for the node ORDER_ITEM_LIST and following.
                    463: No items found to
                           be transferred.
                    464: Program error while compiling the data
                           for the node ORDER_ITEM and following.
                           (e.g. wrong supply type (included) for
                           the main article)
                    465: Program error while compiling the
                           BOM data
                           (e.g. wrong data in aufstrukt; tnr > 999).
                    466: BOM of an item is blank
                    467: Program error while compiling the data for elements



A+W Software GmbH   EN-CONFIG-A+W EnterpriseProductionInterface.docx                      10
                          468: No elements found in the BOM
                          469: Program error while compiling the data for processing steps

                          470: Invalid supply type
                          471: Cancellation information not transferred because there has been
                          no transfer before.
                                This status serves for information only and is actually no
                                error.
                          472: The array that shall take the BOM data, the relevant elements,
                                and their processing steps, is too small. This
                                program error must be passed on to development.
                          496: Transfer completed, but the note in ottranssav could
                                not be made.
                          497: OrderXML service failed to serialize the compiled
                                data for file creation.
                          498: Windows service could not write the reported data
                                in a file.
                          499: Updating the control flag failed.
    •   Filltime:         Time stamp which shows when ALCIB has submitted the order for
        processing.
    •   Serno:           Orders are generally processed in Filltime sequence. This field can be
        used to influence this sequence. An entry with a higher Serno has priority over an entry
        with a lower Serno. AWE prioritizes by default: Rush orders have top priority, and
        standard orders have priority over orders which are only transferred for cost calculation
        purposes. These rules can be customized however by means of the SP cu_orderxmlpriori
        (see chapter 1.3.5 „Aktivierung im ALCIB“).
    •   Serviceid:        In case of redundant systems (there are several computers with
        OrderXML service), a service uses its unique ID to reserves the order it has been
        processing. Simultaneously running services realize that they must not process this order.
        The "unique ID“ for an OrderXML system can be configured in the Windows service
        configuration file. The entry in the transfer table can also be made directly with a
        configurable ID (see chapter 0 „Parallele OrderXML-Systeme“).
Error status in the control flag?
If the field steuerflag has a status of over 400, this denotes an error. For detailed analysis, the
trace level of the OrderXML service (switches Albwir.Alcib.AlOrderXMLService and
Albwir.Alcib.Basis) must be raised, and the Windows service must be rebooted. The order in
question has to be resubmitted by setting steuerflag is set to 0 for the order by manual update to
table ottransfer. If the order status after repeated processing is again over 400, it is possible to
search for "error" entries in the OrderXML service.
If an email shall be issued in case of an error, this can be configured. See chapter 0 "Wenn bei der
Erstellung der OrderXML-Datei ein Fehler auftritt“.

Transfer table ottranssav

By means of table ottranszus ALCIB can provide the service with additional information for which
the service would have to be provided with complex definition mechanisms otherwise. These are
e.g. the width and height of the surrounding rectangle for shape records for which the shape files
would be required. Extensions are possible. The table is structured as follows:



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                        11
    •   Ordno        Number of the quotation or order
    •   Document 5 if the document is an order
        4 if it is a quotation
    •   Posnr       Item number. Depending on the type or the contents of the record, this
        information can show the internal item number or the BOM header number.
    •   Eno          If information on a certain element or a certain processing step is listed, this
        field shows the tupel number of the article in the BOM.
    •   Typ          Tells the OrderXML service the type of data used for this record. Currently
        valid:
        1         = Shape data
        2         = Informs the OrderXML service that this order
                  is transferred only for cost calculation.
                  The entry will be deleted once the order
                  has been released (see chapter 1.4.11
        „OrderXML-Übergaben rein zur Produktionskostenermittlung“).
        3         For purchased elements for which no supplier was entered in
                  the order, the standard supplier is determined and noted here).
                  Downstream programs (Capacity,
                  P.O. creation) can easily access this. The risk that another supplier
                  is determined is lower, the more as lots of tables have to be checked at that
                  point (artvarmdzu, artfarbmdzu, artvarzu, artfarbzu, artmdzu and artikel ).
    •   Serno         Several records may have to be transferred for one piece of information. In
        this case, this field defines the sequence in which the OrderXML service must read the
        data.
    •   Shpno        Shape number
    •   Width        Width
    •   Height       Height
    •   Edges        Number of edges of the present shape that can be processed.
    •   Date         Preparation for the transfer of special dates. E.g. earliest purchase date or
        similar.
    •   Filler       For extensions.

One Service per site (independent DBs, sites)

The term sites is chosen on purpose because a distinction has to be made here between internal
clients and external clients.
With internal site separation , all sites are in the same ALCIB database. For the service, this is a
site. The OrderXML files are saved in separate sub-directories in this case, based on the order's
site number. No additional configuration is required.
Several sites are different ALCIB databases. A separate OrderXML service (installed on different
computers) is required per site.

Several Orders at Once



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                             12
So far, the description assumed that the process is executed by order. This is the standard.
The process can be configured so that the service gathers the information for several orders at
once.
The advantage of this configuration is that the service can remember data for determining several
orders. For a second, third, ... The data do not have to be determined once more in this case for a
second, third, ... order with similar bills of material. This helps to increase the performance.
Please note that lots of data have to be kept in the memory for this function. If more memory is
used than is available, this will result in an error.
Also, it will take longer until the first OrderXML file is available because all information has to be
gathered before the files for the relevant orders can be written.
The number of orders to be gathered can thus be configured. The number should be matched to
the customer's requirements. The most reasonable figure mainly depends on the size the
customer's order usually have as the gathering of order data with lots of items will take longer
than gathering the data for orders with two or three items only. These figures are based on
experience, and can probably be got right only after some time.
Note: The configuration that a certain number of orders has to be gathered at the same time is of
course not mandatory; the system does not wait until this requirement is met. If less orders are
available, the available ones are processed and the system correctly realises that there are no
more orders at present.

Cancelled orders

OrderXML files are also written for cancelled orders. But only if this is necessary, i.e. if the order
had already been transferred. This is detected based on the data in table ottranssav. If this table
shows a line for the order, this means that it has been transferred and the cancellation must be
transferred as well.
After cancellation, the record is deleted from table ottranssav.

Change of site in connection with internal site separation

If ALCIB uses internal site separation, it needs to be checked if the site which is to produce the
order has been changed since the last transfer. In table ottranssav, the OrderXML service does
not only note whether an order has been transferred, but also the receiving site.
Before every transfer, the noted site number is compared with the current site number in the
order. If this has changed, two OrderXML files are written: The first one is used to cancel the
order at the original site and the second is the actual file for the transfer to the right production
site.
Relevant for determining this is the field hausnr in table kauf.
Note: This is an internal process during which the OrderXML service notes the progress in the
transfer tables. This is why the data in the transfer tables must not be manipulated as long as the
order is being processed (discernible by ottransfer.steuerflag>0 and <401).

Parallel OrderXML Systems




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                              13
OrderXML files in ALCIB can be written by several OrderXML services at once. This option can be
used
    •   For failsafety: If one of the computers on which an OrderXML service is installed fails,
        further OrderXML files will be written by a second, redundant system.
    •   Load distribution for big sites: If the data volume is very large, the systems share the task
        of creating OrderXML files; orders are sooner available in the production system.
The following requirements must be met:
For every OrderXML service there must be a separate computer on which the Windows service is
installed.
OrderXML files should be saved by all OrderXML services in the same directory to guarantee the
transfer sequence to the target system (e.g. order transfer and order cancellation). It needs to be
checked that all OrderXML services have writing rights for this directory.
Every OrderXML service must be allocated a unique service ID by means of appropriate
configuration. This allocation also activates the logic (see chapter 0 „Weitere Einstellungen für
den Windows-Service“).
The unique service ID permits to reserve orders in the transfer table for a certain OrderXML
system. As long as an order is processed by one OrderXML service, it cannot be acccessed by any
other OrderXML service. This also applies if the order is changed in ALCIB in the meantime. Only if
the first write request for this order is completed, the next can be started; this ensures that the
transfer sequence is kept.
With regard to failsafety please note: If one OrderXML service fails during the write process, it
may happen that the current order remains locked. In this case, a manual update of the serviceid
in transfer table ottransfer to 0 is required (for all entries for this order).

Definition of the reading service

The system can be configured so that even ALCIB - which presents the order - decides which
OrderXML service is going to process the order. This can be useful if the distribution of load shall
be influenced; very large orders shall only be processed by service 1 for example while all other
orders are processed by service 2. This function can also be used for transfers to various
production systems.
Configuration is made by creating the SP cu_orderxmlservid. This SP receives two parameters:
    •   INTEGER         Order number (kauf.auftrnr)
    •   SMALLINT        Document type (kauf.vorgang)
It has to return a SMALLINT value. The value returned by the SP must be the ServiceID allocated to
the relevant OrderXML service. The value is entered in field ottransfer.serviceid so that the order
is only processed by this OrderXML system.
Please note that the ALCIB processes (including INTAUF) have to be rebooted when the SP is
changed or created.
The SP will not be loaded if the order already appears with a service ID in the transfer table. In this
case, the entry is made by the existing service ID so that the transfer sequence per order is
guaranteed as well as the fact that an order is not processed by two systems at the same time.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                          14
The SP is optional. If it has not been created, the system will not load it; the entry will always be
made with ServiceID 0. The OrderXML systems themselves will reserve the orders in this case.

If an error occurs while the OrderXML file is created

If an error occurs while an OrderXML file is created, this is noted with a code in field steuerflag in
table ottransfer. From a patch version on, a notification can be sent by email as well. If the
OrderXML file interface is used in connection with ALCIM Capacity (if AWC_ALCIM_ANBINDUNG is
set), an error status is also noted in ALCIB for the document in question, and the document can be
processed again.
Email dispatch must be set up. If the system has been configured accordingly, the following email
will be dispatched if the OrderXML could not be created: "Order 231087: Transfer to external
program failed!. (OrderXML Error 402)". The text in brackets at the end of the message always
informs the user that this is an OrderXML error, stating the error number. This error number can
be used to locate the error. For detailed information please refer to the OrderXML service log; the
appropriate error codes can be found in chapter 0 „Übergabe-Tabelle ottransfer“ as described for
the field steuerflag.
To dispatch an email telling the user that the OrderXML file could not be created, please enable
the following switches in ALCIB:
    •   ORDERXML_MESSAGEMANR: Define a user number to be treated as the initiator of the
        message. The message will be sent to this user or to several users defined in the email
        system for report number 45 (group PMS).
    •   AWC_ALCIB_SERVER_NAME: The ALRPC background process in ALCIB is ordered to
        dispatch the message. To address it, enter the name of the server on which the ALRPC
        process is run.
    •   AWC_PORT_CONTROL_SERVER: The ALRPC background process in ALCIB is ordered to
        dispatch the message.If the process does not work, the CTRL_SERVER must start it. This is
        why this switch needs the socket port number of CTRL_SERVER. It can be found in the
        "services" file of the ALCIB server.
    •   AWC_PORT_RPC_DIENST: The ALRPC background process in ALCIB is ordered to dispatch
        this message. To address it, this switch needs the socket port number of ALRPC. It can be
        found in the "services" file of the ALCIB server.
In case of a link with ALCIM Capacity, the switches AWC_ALCIB_SERVER_NAME,
AWC_PORT_CONTROL_SERVER, and AWC_PORT_RPC_DIENST have probably been set already.

OrderXML service waiting for order lock

After transfer to production from ALCIB, editing of orders can be configured, e.g. vorgangs_sql.
The order will remain locked in the number server until editing is finished.
Amendments based on the editing of the order can be relevant for production. The OrderXML
service will therefore wait for the number server lock now and will create an OrderXML file for the
order after the lock has been removed.
This is standard behaviour now which can be switched off if the order is not edited, or if the
amendments are irrelevant for production.
The following switches must be active and set to enable the waiting for the number server lock:




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                              15
    •   AWC_ALCIB_SERVER_NAME: Name of the computer on which the ALCIB background
        processes are run.
    •   AWC_PORT_NR_SERVER: Port number of the number server which is used to
        communicate with the number server (see services file).
To switch off the wait for the number server lock, activate the switch ORDERXML_SPERRMODUS
and set it to '1'.


1.3. Installation and configuration
The elements to be installed for this interface are described in detail in a separate document,
\\Jupiter\doku_docuware\Interfaces\OrderXml\AusAlcib\2012\Inst_ALOrderXMLService_12_1.do
c. These are
    •   Installation of this service.
    •   Fill in the configuration file for this service.
Please stick to the defined sequence.
The installation document also describes the different configuration options. The present
document shall handle these in closer detail. We distinguish
    •   Configuration options defining the start and process of the interface. These are listed in
        this chapter.
    •   Configuration options determining the contents of the OrderXML files. These are
        described in chapter 1.4 „Informationen im OrderXML“.


1.3.1. Configuring the process
Installation of the service includes a configuration file in which the entries have to be made. These
entries can be made by hand (writing rights provided) or by means of a configuration tool. This
tool is automatically started by the SetupLauncher; it can also be started by hand in the
Windowsstart menü in All programs > Albat+Wirsam > Config Tools.
The database settings are made in the second dialog of the OrderXML service:




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                          16
In the configuration file, the switches have the following names:
The switch DB/Server defines the name of the database server.
Db/Host The name of the database host is required for Informix Setnet settings. This is only done
by the configuration tool however. The setting will be saved in the file for the next call of the
tool.The setting will be saved in the file for the next call of the tool.
Db/Service is the port number for database communication. It is necessary for the Informix
Setnet settings and for setting up an ODBC data source. This is only done by the configuration tool
however. The setting will be saved in the file for the next call of the tool.The setting will be saved
in the file for the next call of the tool.
The switch DB/Database defines the name of the ALCIB database.
DB/User defines the name of a database user.
DB/Password defines the password of the current database user. Important: The password must
be entered in the configuration file must be encoded. Encoding is automatically done by the
configuration tool. This is why we recommend using the configuration tool for this first step.
The switch DB/ClientLocale requires input of the Client Locale and the switch DB/DBLocale
requires the database Locale. The format is e.g. „en_US.CP1252 ".
Db/DSN is a name for an ODBC data source; the name can be selected at random. It is necessary
for the Informix Setnet settings and for setting up an ODBC data source. This is only done by the
configuration tool however. The setting will be saved in the file for the next call of the tool.The
setting will be saved in the file for the next call of the tool. If the export service is also installed on
this PC, you should choose the same name there.




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                              17
The first dialogue of the configuration tool defines where the OrderXML files shall be saved.




In the configuration file it is called:
OrderXML/ExportFilepath is the directory into which the Windows service is to write the
OrderXML files. The directory must be created before starting the service for the first time.
In case of internal site separation, sub-directories are expected in this directory, matching the
site number (hnr) of the corresponding sites.

Further Settings for the Windows Service

The following settings in the Windows service configuration file can be used to influence the
process.
    •    MaxNumOrders
    •    OrderXMLEncoding
    •    PollingIntervall
    •    ServiceID
These switches have a default value that can be used to start with. The settings depends very
much on the individual conditions and from the customer’s practical values. This is why the values
can be adapted later on.
The service works cyclically. All orders in the transfer table will be processed after which the
service waits a certain time until he checks if there are new orders in the table. The switch
PollingIntervall defines the waiting time.




A+W Software GmbH           EN-CONFIG-A+W EnterpriseProductionInterface.docx                        18
The switch MaxNumOrders mainly defines the number of orders that shall be processed at once.
The number of orders defined by MaxNumOrders is processed by means of a query. The
advantage is that master data can be noted, and processing is much quicker. The files will
however be written only after all data have been gathered. Availability of the first file is therefore
delayed.
This switch has to be changed only if the database connection is too slow, in order to prevent
access.
The switch OrderXMLEncoding defines the Encoding by which the OrderXML files shall be
created. After the installation, there must be a test with sample orders. In the OrderXML files,
there are special characters, control characters, but also non-Latin character sets to be checked. If
they do not match the characters entered, another character set can be selected. The standard
setting will produce the OrderXML file in UTF8 format which will be the correct format for the
transfer to ALCIM.
If several computers are equipped with OrderXML service which are using the same ALCIB
database for reasons of redundancy, these services must be distinguished by unique IDs. This IDs
has to be defined for every service in the switch ServiceID. It is used to reserve a recently
imported order so that the second service realises that this order is already being processed.
If there is one OrderXML system, the setting ‚0’ is correct; this setting prevents the check as to
whether an order is already being processed by another system.
The Windows service has to be rebooted after changing the settings in the configuration file.


1.3.2. Fileless transfer via AWSOA Planning Import Service
With the latest version of the OrderXML services (status as of May 2021), it is possible in the
configuration program to set the transfer to the Planning Import Service so that it is fileless. This
can be set in the configuration program instead of the output path. If you select the "AWSOA
Planning Import Services" option, you have to select a Planning Import Service in the multisite
selection. If one exists, it always has the number "1". If there are several available, you can select
the corresponding site number. With this mode, no more file (and thus also no drive approval) is
required. However, the "files" processed are stored, now as before, in the appropriate folder
("Archive" or "Problem") after the import. The files have the extension ".stream".
Currently, the Planning Import Service is not in a position to call different production services.


1.3.3. Starting the process
After installation and configuration, the A+W Enterprise 5 OrderXML service can be started. This is
done in the Windows start menu: Settings > System control > Administration > Services. It may be
necessary to change the start type to ‚Automatic’.


1.3.4. Updating to a higher version
Updating the A+W Enterprise 5 OrderXML service in this way is not planned.
To install a new version please stick to the following sequence:
    •   Uninstall the service in System control > Programs and functions. The configuration file
        will be kept in the original program path.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                           19
    •   Install the new diskset for the SetupLauncher and install the ALCIB-OrderXML service
        using the SetupLauncher.
    •   SetupLauncher automatically starts the configuration tool. The configuration file of the
        previous version can be used as an input template. It should not be copied from the
        earlier versions 2.0, 2009 or 2011 however because it has been changed meanwhile.
    •   Now delete the installation path of the old version.
If only a patch update is required (i.e. with the same version number 2012, but a higher build
number), it is not necessary to uninstall the existing service. Prerequisite is that the installation is
handled by the A+W SetupLauncher.


1.3.5. Tracing
Recording can be switched on after the setup, to check the setup or search for errors. The entire
process – from starting the service and determining the switches via searching for orders,
gathering information and writing the file – is noted in the OrderXML service's log file.
Recording of the service can be enabled in its configuration file (manual change or - much simpler
- using the configuration tool).
Note:
Tracing is useful for searching and should be used especially in the set-up phase. Recording should
however be switched off during operation. Tracing is quite time-consuming.

Switches for the Windows Service Tracing

Tracing is set in the third dialogue of the configuration tool which is accessible in the
Windowsstart menu, All Programs > Albat+Wirsam > Config Tools.




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                           20
The settings can be found in the configuration file of the Windows service. The configuration file is
found in the installation directory of the Windows service and is called
AWAlcibOrderXMLService.exe.config. The following settings are available:
The switch AWTrace/Path defines the directory in which the trace file shall be written. The
directory has to be created before the service is started.
AWTrace/Filename defines the name of the trace file.
AWTrace/MaxSize determines the maximum size of the trace file.
AWTrace/FileMode specifies what will happen when the log file has reached the maximum size:
With the setting backup, the current file is saved and a new log file is started. The previous backup
will be changed. If the setting is timestamp, the time stamps are integrated in the file name; when
the maximum size has been reached, a new file is opened with a new time stamp; this way, all
logs will be saved.
Section <switches> of the configuration file determines the log depth, separately for
    •   Albwir.Basis, i.e. basic functions like database communication.
    •   The Windows service Albwir.Alcib.AlOrderXMLService itself: The search for orders,
        selection and compiling of data, and the writing of the OrderXML file is recorded.
    •   Albwir.Alcib.Basis: The ALCIB bill of material is changed into a hierarchy that can be
        handled by OrderXML. This means that the elements to be adopted are determined, and
        the processing steps that influence them.

Which ALCIB data can be found in OrderXML, and where



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                         21
The OrderXML log itself can be used to create Documentation on where certain information from
ALCIB can be found in OrderXML. The trace level of the switch Albwir.Alcib.AlOrderXMLService
must be set to 4 for this purpose. There should be just one order, containing only one item, for
this purpose. Search the trace file for the lines marked „Verbose“. For every node in the
OrderXML file, the system describes the ALCIB information it is filled with.
The log file needs to be viewed with a text editor for this purpose that can show lines of infinite
length without line feeds.


1.3.6. Activation in ALCIB
The OrderXML interface can be enabled from ALCIB 2008.2 upwards. Using this service in
Version 2012 requires ALCIB Version 2012 (A+W Enterprise 5) or higher. To enable the process in
ALCIB please set the following ALCIB-ALENV switch:
    •   ORDERXML: Defines that a case is submitted to the service for processing after input.
        The first parameter defines the version; an unequal entry means that only orders shall be
        transferred while an even input means that both orders and quotations shall be
        transferred. Currently valid entries: 1, 2.
The following switches are mandatory for the process:
    •   MODUL_KOSTENKALK: This variable must be '2' only if the transfer is not made to ALCIM
        by ALCIMCapacity. This way, the background process after the release of the order is
        adapted to the OrderXML transfer or to the fact that there shall be no transfer to PMS.

        Entries ‚1’ or ‚2’ in connection with ALCIM-Capacity permit a preliminary transfer just for
        production cost calculation in case the order shall not be released right away. (also see
        chapter 1.4.11 „OrderXML-Übergaben rein zur Produktionskostenermittlung“)
    •   BYTE_VEKTOR
        The byte vektor environment is necessary for determining the relevant edge for
        edgework, and the right forms for text.
    •   SPROSSENGITTER: Please use the Georgian bar function in ALCIB for ordering Georgian
        bars.
    •   MODUL_NEUE_STUFEN: The new step logic should be active. This permits a more detailed
        transfer of step information and also shows the positions of the stepped elements.
    •   ISO_RAHMEN_MODELL
        If a spacer record is available, the correct spacer width and height to be transferred can
        be determined.
There are further ALENV variables in ALCIB which make sure that the data can be read correctly. A
special tool allows to influence the imported data. Both features are described in chapter 1.4
„Informationen im OrderXML“.
If ALCIB transfers orders to the OrderXML service, they are prioritised by default so that rush
orders will always be processed first while standard orders will be handled before orders that are
just transferred for cost calculation purposes. Prioritisation is done in the field lfdnr in table
ottransfer. The higher the entry here, the earlier will the order be processed by the OrderXML
service.
Should these hierarchy levels be insufficient, a customised solution can be set up by means of SP
cu_orderxmlpriori .




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                            22
This SP receives four parameters:
    • INTEGER           Order number (kauf.auftrnr)
    • SMALLINT          Code for the document type:
                        5=Order
                        4=Quotation
                        2=P.O.
    • SMALLINT        message type
                      0=Order transfer
                      1=Order cancellation
                      2=Order change
        4=Order change (currently without difference to 2)
                      28=Cost calculation for order only
                      29=Offer transfer
                      2002=Offer transfer (currently without difference to 29)
                      2001=Order transfer
    • SMALLINT          1 if it is an rush order
                        0 otherwise


The SP must return a
    • SMALLINT          This is the value transferred to ottransfer.lfdnr. The
                        higher the value, the higher the document priority.
Please note: If the SP cu_orderxmlpriori is created anew or changed, the relevant ALCIB
processes (including intauf) have to be rebooted.
If several OrderXML systems are used, you can define which system is going to process which
order. This special function is described in chapter 0 „Parallele OrderXML-Systeme“.
If an email is to be dispatched to inform someone in case of an error, this can be configured. Also
see chapter 0 „Wenn bei der Erstellung der OrderXML-Datei ein Fehler auftritt“.
Before processing an order, the OrderXML service usually waits until the locked order has been
released by means of the number manager so that the data saved from ALCIB can still be
processed by vorgangs_sql. The appropriate configurations are described in chapter 0 „OrderXML-
Dienst wartet auf Auftragssperre“.

Preventing Transfer

In certain circumstances it may be necessary to prevent the transfer of orders. For example:
    •   Items with the supply type "none" will get no status. This way, the order can always be
        changed even if all production-relevant items have been completed. In this case, the item
        shall not be transferred to the production system again after a change.
    •   Only certain quotations shall be optimized; calculation of quotations is not required. This
        means that only the relevant quotations have to be transferred to production. The
        transfer of other quotations shall be prevented.
The criteria as to when the transfer should be prevented, depend on the customer. This is why
there is an SP for checking the criteria in order to prevent the transfer.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                        23
When defining the criteria please take into account that production cost calculation and
scheduling will take place only if the quotation is transferred to the production system. Preventing
the transfer as such is therefore inadvisable.
The transfer can be prevented by order using the SP cuxmltransfer. This SP receives two
parameters:
        INTEGER      Order number (kauf.auftrnr)
        SMALLINT     Code for the document type:
              5=Order
              4=Quotation
              2=P.O.
It has to return:
        SMALLINT        It should return '1' by default. In this case, an OrderXML
              file will be created for the transaction.
              If the SP returns '0', no file will be created.
If the SP defines that no file shall be created, this will be noted in the log of the OrderXML service
together with a warning. This record will not be updated in table ottranssav either.
Only the transfer record will be removed from table otttransfer. The transaction lock - which is
always set up to the complete transfer - is removed and the document can be edited in ALCIB.
After creation and test, the SP must be enabled by means of the tool ALINFOTOXML (see also
chapter 1.4.5"Kundenindividuelle Informationen"). Since this logic has been introduced only by a
patch version of the OrderXML service, the SP cuxmltransfer may not be listed in the tool yet. In
this case please use an SQL editor in the ALCIB database to make sure that there is no record with
id=42 in table alpooltoxml. Then, a record with
insert into alpooltoxml (id, spname, frei) values (42, 'cuxmltransfer', 1)
can be inserted. When the tool ALINFOTOXML is switched on again, the SP can be enabled or
disabled as usual.
The version code at the bottom of the file shows whether this logic is already available in the
customer's version of the OrderXML service. It must be at least 12.1.6.


1.3.7. Technical data
The described OrderXML function is based on the following versions:
    •   A+W Enterprise 5 (ALCIB 2012.1)
    •   A+W Enterprise 5 OrderXML-Service 2012 (12.1)
    •   ALCIB-Data 12.0
    •   ALCIB-Basis 12.0
    •   Edi-Order-Data 12.0
The service writes the data by „InvariantCulture“. This is why they do not depend on the
computer locale. The reading process must take this into account especially when converting
decimals transferred as part of text (e.g. the processing quantity, field „quantity“).




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                         24
1.4. Environment variables
1.4.1. ORDERXML_NOSTOCKPLATES
     With activation, all stockplate items (atyp >= 180 and < 190) in the OrderXML transfer are
     filtered out of the BOM and not transferred to production. The range also includes the foil
     stock dimensions. The variable became necessary due to very complex, deep BOMs with
     LAMI stock dimensions under additional LAMI stock dimensions.
     See AWDesk #448684.


1.4.2. ORDERXML_PROCPOSTDEF_LEVELDOWN
        Site reference: order
        If the variable is active, for an ordered parent part, processing that takes place after the
        defining processing is transferred in the OrderXML file on the glass below the ordered glass
        (e.g. on the float below a tempered safety glass). In no case may the procurement type of
        the ordered glass be changed to "Production" after the fact in A+W Production with this
        logic.
        See AWDesk #461345


1.4.3. ORDERXML_ENDCUSTOMER_DETAILS
       Client reference: no
If this variable has the value ON, the optional node EndCustomerOrderDetails
is also written when writing the Order XML file.
The prerequisite for this is that the connected sites have common
MP master data.
   For details, please see #345567



1.5. Information in OrderXML
\\Jupiter\doku_docuware\Interfaces\OrderXml\AusAlcib\2012\DokuInfosOrderXMLAlcib.txt is a
text file which describes how every piece of information filled in by the Windows service in
OrderXML is determined in ALCIB (this file can be read with a text editor, without line feeds). If
this file is not available, this information can be created anytime "on site" by setting the tracing to
"Verbose" for the recording of the OrderXML service (see chapter 0 „Welche ALCIB-Daten sind im
OrderXML wo zu finden“). If you are looking for certain information in ALCIB for instance, you can
either load the text file or the log into a text editor. All text editors usually offer a search function:
If the name of the ALCIB database field is entered as a search pattern, the editor proceeds to the
appropriate position if the information is adopted; the relevant OrderXML node is shown at the
start of the line.
We therefore refrain from listing the data in this chapter. This chapter offers information on
    •     Where are the OrderXML files written




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                            25
    •   What is necessary to write the data correctly
    •   How the data are gathered.
    •   How can the written information be influenced (SPs, text attachments)
    •   Which ALCIB Alenv switches are analyzed for compiling the OrderXML information.


1.5.1. How to read the documentation text file
Example excerpt from documentation file DokuInfosOrderXMLAlcib.txt:
         <ORDER ITEM - USER EXTENT - MainLineItemID=
                 If SP exists and is usable cupmawpphauptpos(auftrnr, aufnr, 0, posnr, poskonr) is called,
                 else item reference created from kpos.posnr and rack sequence: to pool_pos.h_pos>



This excerpt describes how the information “MainLineItemID” for an item is filled in.
Unlike here, where line feeds were added to the excerpt, the documentation file shows all
information in one line. Only in places where there are many alternatives, the description of a
node or a piece of information can spread over several lines. The description will be indented in
this case.
The above example should be read as follows:
        <ORDER ITEM - USER EXTENT – MainLineItemID:
is the node, i.e. the position of the information in the OrderXML file.




= If SP …rack sequence:
Describes how the information is gathered. In this case, this is alternatively done directly by
means of the data from ALCIB or by SP. Apart from the name of SP it also shows the parameters
used to load it.
: to pool_pos.h_pos>:
If possible there is a hint on where to find the information in ALCIM if the OrderXML file is
imported into ALCIM .



A+W Software GmbH              EN-CONFIG-A+W EnterpriseProductionInterface.docx                              26
1.5.2. OrderXML files
OrderXML files are created by order. This means that there is one file per order, and this file
includes information on all relevant items.

Directory

The directory in which the files are to be saved must be defined in the Windows service
configuration file (see chapter 1.3.1 „Konfiguration des Ablaufs“).
Important: Before starting the Windows service for the first time, this directory must be created
and writing rights granted.
Internal site separation
For internal site separation, further directories have to be created below the configured directory.
The names of the directories match the corresponding site numbers (like kauf.hausnr). Writing
rights must exist for these directories as well.

File name

The names of the OrderXML files follow a defined pattern. An example: Order237715i0e5t2010-
12-12 17-35-24.xml.
The name consists of the following elements (explained based on this example):
Order                   Fixed string defining that this is an order format. The file can include
                        orders as well as quotations.
237715                     Unique order number acc. to order entry system.
i                          Separator and code defining that an item number may follow (i = item).
0                          The item number is always 0 because orders are always saved completely
                           in files, i.e. with all their items (the file does not include cancelled items).
e                       Separator and code that the document type comes next.
5                       The number matches the document type defined in ALCIB. „5“ represents
                        an order while „4“ denotes a quotation.
t                       Separator and code defining that a time stamp will follow.
2010-12-12 17-35-24     Time stamp showing when the compilation of information has begun. The
                        time stamp consits of: year – month – day hour – minute – second.
.xml                    Fixed suffix of the OrderXML file.

Versioning

We distinguish two version numbers:

OrderXML structure version

Both the ALCIB-OrderXML service and the reading program have to know the basic structure of
the OrderXML so that information is created in the right place, and can be read from there. If this




A+W Software GmbH           EN-CONFIG-A+W EnterpriseProductionInterface.docx                             27
structure changes, both systems may have to be adapted so that the created file can still be read
by the receiving system.
If the receiving system does not know the new structure yet, the switch ORDERXML_VERSION can
be set in ALCIB. The version known to the receiving system must be defined there.
The version defined in the switch, completed by a patch version, appears in the header of the
OrderXML file for control purposes:




The version shown in the file consists of three numbers:
       •   Main version (in this figure, 4): This number changes when the structure of the OrderXML
           is completely revised.
       •   Sub-version (in this figure, 0): This number changes after certain information has been
           added and if the new information can only be read after the receiving system has been
           updated.
       •   Patch version (in this figure, 0001): This number changes with every extension of the
           OrderXML structure even if creating the new information does not mean that an order,
           receiving system can no longer read the OrderXML file.
In the switch ORDERXML_VERSION, only the main version and sub-version of the receiving system
- separated by a dot - have to be entered, e.g. "4.0“. Setting this switch means that only
information known in the OrderXML structure up to this version, will be saved in the OrderXML
file. Newer versions will be suppressed and the file can still be read by the receiving system.

The following versions can be set at present:

4.0:          This is the first version. All reading programs should be able to handle this version. This
              is why this value is used by default if the switch is not set.
4.1:          The A+W processing type catalog has been completed by the processing types 1960
              (edge masking) and 1970 (edge silk screening). The extension of the OrderXML pattern
              Version 4.1 includes these types.
              Set the switch ORDERXML_VERSION to ‚4.1’ if you are sure that the receiving system
              knows these processing types too. Otherwise, leave the original setting of the switch:
              Processing steps of the types 1960 and 1970 will be transferred as general processing
              without parameters. 4.2: The current version created by the OrderXML service as a
              standard. It has not been changed as compared with Version 4.1.
5.0:          Corresponds to version 4.2. With setting to this version, ALCIM synchronizes the
              OrderXML file with the XSD file before importing. As a result, faulty files can be
              detected at an early stage and do not lead to a failure of scheduling. The version may
              only be set if the ALCIM is up to date (see release note #251817).




A+W Software GmbH           EN-CONFIG-A+W EnterpriseProductionInterface.docx                          28
5.1:          The processing type surface macro (1910, new since #201980) and the motif
              parameters for surface processings (1200, 1205, 1210, 1215, 1220, and 1225; new
              since #267331) are only available in all modules (ALCIB, ALCIM, SN) from SP5.2. A
              transfer may only take place if all modules have at least this status. If this is
              guaranteed, the switch ORDERXML_VERSION can be set to "5.1".

Version contents

In a version, new requirements can arise for certain pieces of information. This could be the
section for example which might be determined by another ALCIB table field than before. This
kind of change is documented plus the information from which version code they are available.
This version number is defined at the end of the OrderXML file (in this figure, e.g. 3.5.6). It can be
used to check whether the new requirement can already be handled by the existing OrderXML
service, or if a new service needs to be installed.




The version number in Version 2012 will therefore start by „12.1.“, followed by the corresponding
patch number.

Structure of Contents

The structure of an OrderXML file is described in a separate document. In the present document
we shall only explain how to retrieve information imported from ALCIB.
Order information in an OrderXML file can be split into four sections:




       •   Order header
           includes details like the order number, input information, and delivery dates



A+W Software GmbH           EN-CONFIG-A+W EnterpriseProductionInterface.docx                        29
    •   List of items
        List of all order items.
    •   Order summary
        shows the number of items.
    •   A+W-specific extensions
        includes e.g. order-related text plus references to document links.
For every item, the List of items offers




    •   Information on the item article
    •   A+W-specific extensions
The A+W-specific extensions for an item include




    •   Information on the item, especially the item reference ID.
    •   Production list
        is a list list of relevant elements. These are usually glass, film, spacers or cast resin,
        Georgian bars, and purchased elements.




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                          30
    •   Customer reference
        This is the item-specific text
    •   Reference texts
The following groups of information are available for every product (element) on the product list:




    •   Information on the element
        Especially the element reference or bomID
    •   List of sub-products
        Lists the element references for the imported elements which can be found in the ALCIB
        BOM right below the actual element. These references can be used to re-establish the
        ALCIB BOM hierarchy in the production system.
    •   Product elements
        Includes all information on the element. This information depends on the element type
        and are therefore different for glass, film, spacers, Georgian bars, or other purchased
        elements.
        This section also includes the step information.
    •   Geometries
        Width and height of the shape parameters if necessary.
        The sizes were determined on a commercial basis. Produktion-related amendments like
        cutting corrections for example have to be determined in the production system itself.
    •   Processing list
        This is where processing steps are allocated to the elements depending on the processing
        type, on the processing step's position in the BOM, and on the sequence of processing
        steps in the BOM
    •   List of tupel-specific text
        This also includes the special codes and special text
The following information is provided for every processing step that can be allocated to an
element




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                        31
    •   The reference
        to guarantee clear identification in reports (matches the tupel number in the BOM)
    •   A sequence
        The sequence of processing steps matches the sequence shown in the BOM.
    •   Texts
    •   And the data for the processing article
        The shape in which these are presented depends on whether the processing step is
        allocated to an A+W processing type.



XSD-compliant OrderXML files

Starting with a patch version, ALCIM is able to validate OrderXML files before import; i.e. to check
whether the OrderXML file is compliant with the XSD file. This way, the system can detect and
report faulty files early so they don't cause problems during import.
To use this feature, set the ALCIB ORDERXML_VERSION control to "5.0". The entry "5" at the start
enables validation.
Prerequisite for using this function is an up-to-date ALCIM. The OrderXML service has to be up to
date as well; this is identified by the version code "12.1.2" at the bottom of the file.


1.5.3. Gathering information on elements
This chapter does not expound on every single detail of the elements; these are avaible from the
documentation file. It describes the elements relevant for transfer, how the BOM hierarchy is
handled by the OrderXML file, and how an element can be clearly identified. We are also going to
explain how special bits of information are gathered, especially if there are several alternatives
depending on the system configuration.

Import-Relevant Element Types

The following element types will be imported:
    •   Sheets: These are only cut sizes, i.e. the article types from 100 to (exclusively) 180, and
        200.
        Stocksizes are not relevant as articles for production. Only the processing step 'cutting'
        and the thickness of the stocksize are generally required to calculate the thickness of the
        whole product. The properties of the stocksize are otherwise identical with those of the
        cut size. This is why stocksizes can be ignored.
        This is e.g. also true for laminated glass which - depending on the stocksize's supply type -
        can be cut or produced. In this case, the ALCIB BOM for laminated glass shows the
        stocksize and below the stocksize, the individual sheets and films. If laminated glass shall
        be cut (supply type of the stocksize is 'stock'), the OrderXML file includes only the
        laminated glass cut size and the processing step 'cutting'. If the laminated sheet shall be
        produced (supply type of the stocksize is 'production'), the laminated glass, the individual
        sheets, and the film will be imported while the intermediate layer containing the stocksize
        in the ALCIB BOM will be ignored.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                         32
   •   Laminated glass file, article type 176. Only the film elements are imported. Film packets
       also have article type 176. They should be defined as meta elements the BOM of which
       includes the individual film layers. The OrderXML file transfers the individual film layers,
       ignoring the meta element as it were.
       The film layers can also be entered directly in the BOM, between the sheets. Prerequisite
       is the correct assembly position for every film layer.
   •   IG spacers, article type 210 or 211
Parts with Atyp 220 will not be transferred via the OrderXML interface. These therefore cannot
be ordered order-related! The CompleteScheduling here then encounters an error, because
according to the AWE BOM, this part would have to be ordered, but it is not included in the
AWP report.
   •   Cast resin: This is the spacer between the individual sheets of a cast resin product which is
       also responsible for the thickness of the product. Its article type is usually 340. If this
       cannot be guaranteed, the article can be allocated a special PMS type in article master
       data. This PMS type can be customised by means of the switch PMCGHDICKETYP.
       Note: The valid PMS types are still defined in PMS. Allocation can only be made in article
       master data.
   •   Georgian bars: If the BOM includes Georgian bars, one element will be imported in place
       of the Georgian bar pattern. The structure is described in the sections below this element.
       See example:




       The grid is imported as the Georgian bar element (article type 225). If the grid function in
       ALCIB is not used, the first Georgian bar article found in table kspross will be imported




A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                         33
        (article type 230 and meta element). The switch PMXAWPOOLSPROSSEN can be used for
        grouping in this case. This switch defines that for all Georgian bar articles allocated to a
        certain PMS type, the same article shall be used as the Georgian bar element. If the first
        Georgian bar article in kspross is allocated to a PMS type and if this PMS type is defined in
        the switch's value list, the defined article number is imported as an element.
    •   Wood (article type 701) is handled like glass.
    •   Other elements/accessories: The following article types are recognised as accessories:
        270: Edge protection
        280: Capillary inlay
        300: Film
        320: Colour/varnish layer
        370: Glass bricks
        380: Multiplex glass
        600: Rails
        610: Pipes
        800: Accessories
        820: Metal sheets
        830: Fittings
        840: Locks
        850: Handles
        870: Alarm wires.
        provided that these are actual elements (artikel.teilflag=1)
Gas (article type 260) and sealants (240) are not imported as separate elements but appear as bits
of information in connection with spacers.

Handling of the ALCIB BOM Hierarchy

As described in chapter 0 „Inhaltlicher Aufbau“, the item information in the OrderXML file always
lists the elements relevant for import.




The above example shows an IG unit. Below the IG there is a single annealed sheet, a spacer, and
another single annealed sheet. Below the spacer, a Georgian bar is attached.
The above element list does not tell us how the elements are arranged with regard to their
hierarchy.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                          34
The reading program should always start with the first element on the element list. This is always
the main element of the ALCIB BOM. In the example above, this is the element with the BOM-ID
(element reference) „0040010001“, from the ALCIB BOM's point of view, the IG unit.
Below this element there is a list of sub-products:




This list shows element references (BOM-ID) of the elements directly below the IG unit in the
ALCIB BOM (three elements: glass, spacer, glass). This means that after the IG unit, the element
with BOM-ID "0040010002“ could be read next, i.e. the first single annealed sheet. Had this
element sub-elements as well, its product information would also include a sub-product list with
the relevant BOM-IDs. In our example, no further elements are to be found below the glass, the
sub-product list is empty.
Only the spacer (the element with BOM-ID 0040010003) shows a sub-product list, with a
reference to the Georgian bar's BOM-ID:




Meta elements in the AWE BOM

Meta elements (marked by element flag 2 in article master data) are actually meant to unite
several processing steps in one, or to depict structures within which the element is only relevant
for pricing while the processing step is relevant for production. Principally, there can be glass
META elements.
Please note that META elements will be generally ignored if their supply type is „Production“. If
they have another supply type, they will be adopted as an element (to be ordered or withdrawn
from stock). In case of ordered META processing steps, the material in question will be adopted as
a processing step, and the BOM is not broken down any further.
If EDI supply types are used, the supply type „Production before EDI" means - if the META
element lies below the purchased element - that the supply types for all types on the BOM level
below the META element will get a "before EDI" supply type. Supply type „Production“ however
means – in connection with an incomplete BOM - that the META element and the entire tree
below it are not relevant for production but are included in the purchase order.
If glass is used as a META element, please check the uniformity and feasibility of article types. Real
glass should never occur below a META stamp in the BOM for instance, and a genuine laminated
sheet should not occur below a META element of the type 'float glass fixed size'. Glass can only be
recognised reliably if the META element which BOM it belongs to also includes a glass article type,
and the article type of the META glass has to match the article type of the subordinate as well as
the superior glass.
Main elements defined as META elements will always be adopted as an element, and will not be
overlooked.
For special treatment of meta elements with active extended workbench, see chapter "Extended
workbench."

Element Reference / BOM ID



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                         35
Each element is clearly identified by an element reference. In the OrderXML file, this is the
information „bomID“.
As described above, the reading program can use this reference to determine the BOM hierarchy
of the elements.
The reference is mainly important for reports to ALCIB which refer to a certain element. This
reference can be used to identify this element in ALCIB.
The reference is structured as follows:
    •   The first three digits
        define the internal item number (kpos.posnr)
    •   The next three digits
        are a serial number in the item. This is usually „001“. If the item is split to several racks
        however (there are several entries for this item in kposgest), this number is a counter for
        the rack.
    •   The last four digits
        are the tupel number, i.e. a unique number in the ALCIB BOM.

Information Details

This chapter describes in detail the gathering of special element information. Development shall
be pleased to receive any suggestions regarding the extension of these functions.

Step information

We recommend to enable the new step input method in ALCIB (switch MODUL_NEUESTUFEN).
The reason: Even for more complex bills of material, steps can be clearly assigned, and different
step reductions can be defined for the individual elements.
This also influences the import into OrderXML:
Old step input
The old step input method is restricted to the input of a record for step reductions for the main
element. Stepped sheets are marked in the bill of material.
Import works in the same way:
Step parameters are adopted in the „STEPPING“ element of the main element. The parameters
can be used to define the stepped edge.
Even stepped sheets have a „STEPPING“ element which serves to mark the stepped sheets. The
values in these elements are however 0. This is correct because the calculated geometry is
adopted for all sheets.
New Input of Steps
Import here is also made in the same way as input in ALCIB.
The same geometry is adopted for all sheets, i.e. that of the glass for which the reference
geometry has been entered.
The reference glass is marked in the geometry record by "3" in the "Valuation" element.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                           36
For the stepped sheets, a "STEPPING" element is available in which the actual step reductions are
defined.




Edges are numbered anti-clockwise in both cases. This means that the first step reduction applies
to the bottom edge, the next size for the next edge to the right, and so on.
The signs for the stepped differ from those in ALCIB. Negative signs in the OrderXML mean that
the sheet gets smaller while no sign means that the sheet gets bigger.
More steps for the production system
Depending on the shape, the number of steps in the ERP and in the production system can vary.
The example of a circle shows why. A circle cannot be cut or processed in just one go: Four moves
are necessary. For each of these moves, the corresponding step must be known so that the
production system needs for moves here (e.g. for the transfer to the machine driver).

With regard to the input, the steps must be identical so make sure that a circle remains after the
step reduction. This is why just one step can be entered in ALCIB.
This means for the OrderXML interface that this one step must be extended to four.
This principle is not just true for a circle but for all shapes that include a radius. The following
table shows the shapes to which this extension applies. The second columns shows the number of
steps (per shape) an OrderXML file plans for the shape. The third column defines the field in the
ALCIB table kstufparam from which the appropriate step information is loaded. The fourth column
shows the field of the ALCIM table pool_modell into which the step is adopted (if it is not changed
by ALCIM-SNDraw later).
Please note that adoption is not made 1:1: While the values for steps in ALCIB and in OrderXML
are entered in millimetres, they will be converted into micrometres for ALCIM. For spacers, the
steps are defined up to the inside edge of the spacer in ALCIB while in OrderXML and in ALCIM
they are required up to the outside edge, i.e. reduced by the spacer thickness.



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                        37
Especially for spacers and Georgian bars, the OrderXML file also allows for a cutback element
(CUTBACK). This is extended to the same quantity as the steps. While the information for steps is
loaded from the dmass fields of the ALCIB table kstufparam, the cutback information is loaded
from the corresponding diff fields of the same table. The entry there is made in 10ths of
millimetres and is converted to millimetres for the OrderXML file.
          Shape number        Step number         Table field from       Table field in
                                                  ALCIB kstufparam       ALCIM pool_modell
          60                  1                   dmass1                 stufeneinzug1
                              2                   dmass1                 stufeneinzug2
                              3                   dmass1                 stufeneinzug3
                              4                   dmass1                 stufeneinzug4
          61                  1                   dmass1                 stufeneinzug1
                              2                   dmass1                 stufeneinzug2
                              3                   dmass1                 stufeneinzug3
                              4                   dmass1                 stufeneinzug4
          62                  1                   dmass1                 stufeneinzug1
                              2                   dmass2                 stufeneinzug2
                              3                   dmass2                 stufeneinzug3
          63                  1                   dmass1                 stufeneinzug1
                              2                   dmass2                 stufeneinzug2
                              3                   dmass2                 stufeneinzug3
          74                  1                   dmass1                 stufeneinzug1
                              2                   dmass2                 stufeneinzug2
                              3                   dmass2                 stufeneinzug3
                              4                   dmass2                 stufeneinzug4
                              5                   dmass2                 stufeneinzug5
                              6                   dmass2                 stufeneinzug6
          75                  1                   dmass1                 stufeneinzug1
                              2                   dmass1                 stufeneinzug2
                              3                   dmass1                 stufeneinzug3
                              4                   dmass1                 stufeneinzug4
                              5                   dmass1                 stufeneinzug5
                              6                   dmass1                 stufeneinzug6
                              7                   dmass1                 stufeneinzug7
                              8                   dmass1                 stufeneinzug8
          78                  1                   dmass1                 stufeneinzug1
                              2                   dmass1                 stufeneinzug2
                              3                   dmass1                 stufeneinzug3
                              4                   dmass1                 stufeneinzug4
          81                  1                   dmass1                 stufeneinzug1
                              2                   dmass1                 stufeneinzug2
                              3                   dmass1                 stufeneinzug3
                              4                   dmass1                 stufeneinzug4
                              5                   dmass1                 stufeneinzug5
                              6                   dmass1                 stufeneinzug6




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                       38
        Shape number       Step number      Table field from     Table field in
                                            ALCIB kstufparam     ALCIM pool_modell
                           7                dmass1               stufeneinzug7
                           8                dmass1               stufeneinzug8
        123                1                dmass1               stufeneinzug1
                           2                dmass4               stufeneinzug2
                           3                dmass3               stufeneinzug3
                           4                dmass3               stufeneinzug4
                           5                dmass3               stufeneinzug5
                           6                dmass3               stufeneinzug6
                           7                dmass3               stufeneinzug7
                           8                dmass3               stufeneinzug8
                           9                dmass3               stufeneinzug9
                           10               dmass2               stufeneinzug10
        124                1                dmass1               stufeneinzug1
                           2                dmass4               stufeneinzug2
                           3                dmass3               stufeneinzug3
                           4                dmass3               stufeneinzug4
                           5                dmass3               stufeneinzug5
                           6                dmass3               stufeneinzug6
                           7                dmass2               stufeneinzug7
        125                1                dmass1               stufeneinzug1
                           2                dmass4               stufeneinzug2
                           3                dmass3               stufeneinzug3
                           4                dmass3               stufeneinzug4
                           5                dmass3               stufeneinzug5
                           6                dmass3               stufeneinzug6
                           7                dmass2               stufeneinzug7
        126                1                dmass1               stufeneinzug1
                           2                dmass4               stufeneinzug2
                           3                dmass3               stufeneinzug3
                           4                dmass3               stufeneinzug4
                           5                dmass3               stufeneinzug5
                           6                dmass3               stufeneinzug6
                           7                dmass2               stufeneinzug7
        127                1                dmass1               stufeneinzug1
                           2                dmass4               stufeneinzug2
                           3                dmass3               stufeneinzug3
                           4                dmass3               stufeneinzug4
                           5                dmass3               stufeneinzug5
                           6                dmass3               stufeneinzug6
                           7                dmass2               stufeneinzug7
        133                1                dmass1               stufeneinzug1
                           2                dmass2               stufeneinzug2
                           3                dmass2               stufeneinzug3
                           4                dmass2               stufeneinzug4




A+W Software GmbH      EN-CONFIG-A+W EnterpriseProductionInterface.docx              39
          Shape number         Step number         Table field from        Table field in
                                                   ALCIB kstufparam        ALCIM pool_modell
                               5                   dmass2                  stufeneinzug5
                               6                   dmass2                  stufeneinzug6
          136                  1                   dmass1                  stufeneinzug1
                               2                   dmass2                  stufeneinzug2
                               3                   dmass2                  stufeneinzug3



Spacer

STEPPING Element
A step record can exist even for spacers. Prerequisite is that the explicit spacer geometry function
is active (MODUL_NEUESTUFEN and MODUL_VERSIEGELUNGSTIEFE or ISO_RAHMEN_MODELL).
The shape geometry which is adopted for the spacer matches that of the reference geometry (see
above „Steps: New step input“). The element „Valuation“ identifies the reliable spacer geometry
by 10.




In this case, the „STEPPING“ element of the spacer includes values which - together with the
shape sizes - describe the external spacer sizes. It is imported from ALCIB:
    •   If special reductions have been defined: The sizes from table kstufparam minus the spacer
        thickness defined in article master data. The step sizes consist of the defined spacer
        reductions and the defined steps (if applicable).
    •   If no special reductions or steps have been defined, half of the spacer reduction defined
        for the item will be adopted for every shape edge. The spacer thickness defined in article
        master data will be deducted.
Note:
The spacer reduction in ALCIB (kpos.aham) always describes the inside edge of the spacer.
To determine the external sizes, the spacer thickness is therefore deducted. This is loaded from
article master data; if it is 0 there, a standard thickness of 7 will be deducted.
CUTBACK element
The „CUTBACK“ element in an OrderXML file describes the spacer cutback. If no special SP has
been defined for the sealing depth, the values from table kstufparam - like for the „STEPPING“
element - or, if these are not available, half of the spacer reduction is adopted per edge. The




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                          40
imported values include the actual spacer reductions up to the inside edge of the spacer, i.e. they
do not include step reductions, and the spacer thickness is not deducted either.
Width and height of the surrounding rectangle
For the OrderXML function, the switch ISO_RAHMEN_MODELL should be set in ALCIB. At order
entry, a spacer record is created on principle. This is the basis for importing synonymous widths
and heights for the surrounding rectangle:
The width and height of the spacer describe the size of the inside edge of the spacer.
Gas
Gas (article type 260) is usually not imported as a separate element. (Exception: If gas is
purchased based on the BOM, a gas P.O. element will be created to inform the production system
that it needs to wait for this element.)
Gas is considered to be part of the spacer information.




The gas article should therefore preferably be located below the spacer in the ALCIB BOM. This
applies especially to triple IG where this is the only way to guarantee a clear allocation to the
spacer.
This structure is not mandatory however. Gas can also be added directly below the IG unit in the
BOM. If an IG unit includes two spacers and two gas articles, the first gas article is allocated to the
first spacer and the second gas article, to the second spacer.
Sealant
Sealants (article type 240) are usually not imported as a separate element. (Exception: If the
sealant is purchased based on the BOM, an additional P.O. element will be created to tell the
production system that it needs to wait for this element.)
Sealants are considered to be part of the spacer information.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                           41
It must therefore be possible to allocate the sealant to the spacer in the ALCIB BOM. This applies
especially to triple IG. The system will mainly search for a sealant the assembly position of which
matches that of the spacer.
If no assembly position can be defined, the sealant article should be located below the spacer in
the ALCIB BOM. It can thus be clearly allocated.
If both is not the case, the system searches for the sealant - with assembly position 0 - directly
below the IG unit in the BOM. If in that case, IG consists of two spacers and two sealant articles,
the first sealant article is allocated to the first spacer and the second sealant, to the second
spacer.
Basic rule: Maximally one sealant is imported per spacer. If more sealants are found, the
sequence in the BOM defines which of them will be imported: The first sealant will always be
imported.
Note:
For variable sealing depths, ALCIB also knows shape records and step records for the sealant.
These will be ignored here because they mainly serve to create text in ALCIB.
Sealant in a standard ALCIB BOM has a predefined structure: The sealant itself is a META element
(article type 240, element flag 2) the BOM of which includes an element (article type 240, element
flag 1) and a processing step.




The sealing data – like name and sealing type - are generally determined for the article number of
the actual META element. If the ALCIB environment switch ORDERXML_VERSIEGELUNGSDATEN is
active however and shows and entry of ‚1’, the data for the sealant element's article number are
determined by means of its BOM (in the example above, Thiokol).
Alternatively, the sealing type can be determined by the SP cupmawptdichttyp If this SP has
been defined and is active, its result has priority over the entry in master data. The SP receives the
following parameters (in this sequence):
    •   INTEGER: The first parameter is the external order number kauf.auftrnr.
    •   INTEGER: The second parameter is the internal order number kauf.aufnr.
    •   SMALLINT: The third parameter is the internal item number kpos.posnr.
    •   SMALLINT: The fourth parameter is the BOM header number kpos.poskonr.
    •   SMALLINT: The fifth parameter is the tupel number of the spacer aufstrukt.tnr.
The expected return value is
    •   SMALLINT: the numerical value of the sealant type
expected.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                            42
The the SP has been defined and tested, it can be released by means of the program
ALINFOTOXML (see chapter 1.4.5 „Kundenindividuelle Informationen“. After that, the sealing
type is determined by means of the SP.
Please note that this SP is loaded for all spacer articles: Not only for IG spacers but also for cast
resin and fire protection glass fillings. If the SP value for these types shall not be taken into
account, the value returned must be ‚-1’.
Spacer Type
In the OrderXML file, the spacer type is found in in the information junction <ORDER ITEM - USER
EXTENT - PRODUCT - PRODUCT_ELEMENTS - Item Spacer - typeID>.
The spacer types are loaded from article master data by default. For production, e.g. for bender
control, a more detailed distinction or a different numbering of spacer types may be necessary. In
this case, spacer types can be determined by customer.
A SP called cupmawptrahmentyp must be defined for this purpose. It receives the following
parameters (in just this sequence):
    •   INTEGER: The first parameter is the external order number kauf.auftrnr.
    •   INTEGER: The second parameter is the internal order number kauf.aufnr.
    •   SMALLINT: The third parameter is the internal item number kpos.posnr.
    •   SMALLINT: The fourth parameter is the BOM header number kpos.poskonr.
    •   SMALLINT: The fifth parameter is the tupel number of the spacer aufstrukt.tnr.
The expected return value is
    •   SMALLINT: the numerical value of the spacer type
expected.
The the SP has been defined and tested, it can be released by means of the program
ALINFOTOXML (see chapter 1.4.5 „Kundenindividuelle Informationen“. After that, the spacer type
is determined by means of the SP.
Please note that the SP will be loaded for all spacer articles: This does not only apply to IG spacers
but also for cast resin and fire protection glass fillings.
Rahmenfarbe
IG spacers cannot be allocated Colours because they are kept in size variants. To specify the
colour, an article can be added to the BOM of the spacer which is then allocated the colour. This
article has to have a certain article type which can be defined - by customer - by means of the
switch PMQCIMTYPRAHMENFARBTEXT. (However, this should not be the article type of the
spacer.)
The first article of this article type in the spacer's BOM serves to specify the color. The color
allocated here is adopted as the color number. As the color name, the manually entered text in
table poszu will be adopted. If this field is blank, the color name is adopted from the color code
table.
Alternatively, the spacer color can be deteremined by SP cupmawptrahmenfarb . If this SP has
been defined and is active, its result has priority over the the entry for the specified colour article.
The SP receives the following parameters (in this sequence):
    •   INTEGER: The first parameter is the external order number kauf.auftrnr.
    •   INTEGER: The second parameter is the internal order number kauf.aufnr.



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                              43
    •   SMALLINT: The third parameter is the internal item number kpos.posnr.
    •   SMALLINT: The fourth parameter is the BOM header number kpos.poskonr.
    •   SMALLINT: The fifth parameter is the tupel number in the BOM of the spacer
        aufstrukt.tnr.
The expected return value is
    •   SMALLINT: the numerical value of the spacer color
expected.
The color name is determined by means of this colour number in the color code table.
The the SP has been defined and tested, it can be released by means of the program
ALINFOTOXML (see chapter 1.4.5 „Kundenindividuelle Informationen“. After that, the spacer
color is determined by means of the SP.
Please note that this SP will be loaded for all spacer articles: Not only for IG spacers, but also for
cast resin and fire protection glass fillings. If the SP value for these types shall not be taken into
account, the value returned must be ‚-1’.
Georgian bars
Presentation of information
If an item includes Georgian bars, an element record describing the pattern will be loaded. The
information on this element record includes the whole structure, arranged by:
Horizontal bars
Horizontal sections
Vertical bars
Vertical sections
Since a "Georgian bar pattern“ is described, we recommend to enable the grid function at ALCIB
order entry. (This is mandatory if Georgian bars can be purchased). This way, the article loaded as
an element will always be clear.
If the grid function is not used in ALCIB, the first Georgian bar article found in table kspross will be
loaded instead.
Alternatively, the switch PMXAWPOOLSPROSSEN can be used for grouping in this case. It defines
that for all Georgian bar articles allocated to a certain PMS type, the same article shall be used as
the Georgian bar element. If the first Georgian bar article in kspross is allocated to a PMS type and
if this PMS type is defined in the switch's value list, the defined article number is imported as an
element.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                               44
Note for the transfer between A+W products:
By describing the individual sections, an unlimited number of different bars is generally feasible.
The limitation of the standard should be obeyed however:
-       up to 12 horizontal and 12 vertical bars.
-       up to 2 different horizontal Georgian bar articles, and
        2 different vertical Georgian bar articles
        (e.g. to depict different colours or width)
STEPPING Element
As for the spacer, a stepped record can also exist for Georgian bars. Prerequisite is that the
explicit spacer geometry function is active (MODUL_NEUESTUFEN and
MODUL_VERSIEGELUNGSTIEFE or ISO_RAHMEN_MODELL).
The shape geometry which is adopted for the Georgian bar pattern matches the reference
geometry in this case (see above „Steps: New step input“). The element „Valuation“ marks the
reliable geometry by an entry of 11.
The „STEPPING“ element of the bar shows values based on the step records for the superior
spacer; together with the shape sizes, these values describe the inside size of the spacer. It is
imported from ALCIB:
If special deductions were defined for the spacer: The sizes from table kstufparam; in contrast to
the spacer description, the spacer thickness will not be deducted here. The step sizes consist of
the defined spacer reductions and the defined steps (if applicable).
If no special reductions or steps have been defined, half of the spacer reduction defined for the
item will be adopted for every shape edge.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                          45
Note:
The spacer reduction in ALCIB (kpos.aham) always describes the inside edge of the spacer.
CUTBACK element
If the item includes Georgian bars, the same values as for the spacer's „CUTBACK“ section will be
adopted (see there) for this „CUTBACK“ section.
Several Georgian bar patterns
An ALCIB item may include two Georgian bar patterns in case of triple IG, if the Georgian bar
articles are allocated to certain spacers. OrderXML will describe two grid elements in this case.
They are imported as sub-elements of the defined spacer.
Georgian bar pattern as a main element
Where Georgian bar patterns are ordered internally (switch SPROSSENGITTER), it may happen
that grids are included in the item as main elements (in the receiving site's order). Such a grid
pattern is described by two elements in the OrderXML file. The grid article is the main element
and represents a type of spacer. The sub-element serves to describe the structure.
muntin bar type
The Georgian bar type is transferred in field „BarGrid -> TypeID“. The type numbers are fixed and
describe, together with the milling depth and the trim, the Georgian bar connection as well as the
continuous bar . This value is determined by means of the Georgian bar types known in ALCIB.
These will be converted.
We are now going to describe how the ALCIB Georgian bar types are changed into OrderXML
Georgian bar types and how the milling depth and the trim are calculated.
    •   ALCIB bar type 1 marks a double mitre at the junctions and matches OrderXML bar type 1.
        There is no continuous bar. The relevant milling depth (mitre) must be defined in ALCIB
        Georgian bar article master data. The trim will not be analysed; the program always uses
        0.
    •   ALCIB bar type 2 marks a continuous mitre. This means that there is a continuous bar.
        The milling depth is a fixed value, i.e. a quarter of the width of the continuous bar. The
        trim is always 0. There are three criteria for determining the continous bar:
        o    The bar direction with the smallest number of "auxiliary" bars.
        o    If the number of auxiliary bars is the same, the wider bar.
        o    If the bars have the same width, a standard will be applied which is defined by an
             ALCIB environment switch.
    If the continuous bar is the vertical one, this is OrderXML bar type 5.
    If the continuous bar is the horizontal one, this is OrderXML bar type 6.
    •   ALCIB bar type 3 marks a blunt connection. This means that there is a continuous bar
        without milling depth and trim (both will be adopted as 0 irrespective of the definition in
        master data). There are three criteria for defining the continuous bar:
        o    The bar direction with the smallest number of "auxiliary" bars.
        o    If the number of auxiliary bars is the same, the wider bar.
        o    If the bars have the same width, a standard will be applied which is defined by an
             ALCIB environment switch.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                            46
   If the continuous bar is the vertical one, this is OrderXML bar type 5.
   If the continuous bar is the horizontal one, this is OrderXML bar type 6.
   •   ALCIB bar type 4 is a cross with a blunt connection. The milling depth will always be 0. The
       trim for the corresponding Georgian bar article can be entered in ALCIB article master
       data. If the trim is 0 there, half the width of the crossing bar will be adopted.
       This type matches OrderXML type 2.
   •   ALCIB bar type 5 is a continuous mitre, albeit with a fixed milling depth. This means that
       there is a continuous bar. The trim is always 0. There are three criteria for defining the
       continuous bar:
       o    The bar direction with the smallest number of "auxiliary" bars.
       o    If the number of auxiliary bars is the same, the wider bar.
       o    If the bars have the same width, a standard will be applied which is defined by an
            ALCIB environment switch.
   If the continuous bar is the vertical one, this is OrderXML bar type 5.
   If the continuous bar is the horizontal one, this is OrderXML bar type 6.
   •   ALCIB bar type 10 is adopted as OrderXML bar type 7. All bars are continuous. If the
       milling depth or the trim are to be taken into account, the values must be entered in
       ALCIB article master data for the corresponding Georgian bar.
   •   ALCIB bar type 11 is a continuous mitre with variable milling depth. This means that there
       is a continuous bar. The milling depth is loaded from ALCIB article master data for the
       actual bar. The trim is always 0. There are three criteria for determining the continous
       bar:
       o    The bar direction with the smallest number of "auxiliary" bars.
       o    If the number of auxiliary bars is the same, the wider bar.
       o    If the bars have the same width, a standard will be applied which is defined by an
            ALCIB environment switch.
   If the continuous bar is the vertical one, this is OrderXML bar type 5.
   If the continuous bar is the horizontal one, this is OrderXML bar type 6.
   •   ALCIB bar type 10 is adopted as OrderXML bar type 7. All bars are continuous. If the
       milling depth or the trim are to be taken into account, the values must be entered in
       ALCIB article master data for the corresponding Georgian bar.
   •   ALCIB bar type 93 marks a double bar. Trim and milling depth can be defined in ALCIB
       article master data. The continuous bar is always the widest bar unless auxiliary bars have
       been defined for this bar. If the continuous bar is the vertical one, this matches ALCIM bar
       type 8.If the continuous bar is the horizontal one, this matches ALCIM bar type 9.
       If you are using ALCIM and want to transfer data to AWDesign please note that the
       display in AWDesign matches OrderXML bar types 5 and 6. The ALCIM bar types can be
       used to mark special patterns however.
The following marginal condition should be considered
   •   Information on the bar type and on the continuous bar are given by grid in OrderXML
       while ALCIB can describe this by section. Please note: The Georgian bar article number of
       the first horizontal bar is always used as a basis for data definition. Where comparisons




A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                            47
        are necessary (e.g. width of vertical bars and width of horizontal bars), the articles of the
        first horizontal and the first vertical bar will be used.
Continuation type for AWDesign
The Georgian bar continuation type is meant for the transfer to AWDesign. Based on this type, all
systems can identify the continuous bar and how it is determined in AWDesign. The continuation
type - in connection with the milling depth and the trim - describes the grid connection, i.e. the
way in which horizontal and vertical bars are assembled. This information is found in: <ORDER
ITEM - USER EXTENT - PRODUCT - PRODUCT_ELEMENTS - Item BarGrid – continuousType>. ALCIB
sets this value depending on the bar type (see above): Is transferred as the Georgian bar type
    •   1 is transferred as continuousType „none“ (no continuous bar).
    •   2 is transferred as continuousType „none“ (no continuous bar).
    •   3 is transferred as continuousType „vertical“ (the vertical bar continues).
    •   4 is transferred as continuousType „horizontal“ (the horizontal bar continues).
    •   5 is transferrd as continuousType „vertical“ (the vertical bar continues)
    •   6 is transferred as continuousType „horizontal“ (the horizontal bar continues).
    •   7 is transferred as continuousType „both“ (both bars are continuous).
    •   8 is transferred as continuousType „vertical“ (the vertical bar continues).
    •   9 is transferred as continuousType „horizontal“ (the horizontal bar continues).
    •   Exception: The bar has article type 235. This is a lead bar which is transferred as „lead“.

Element thickness

The thickness of an element is usually calculated from the total thickness of its sub-elements. The
thickness of the bottom element of the BOM is loaded from article master data (artikel.staerke).

Only if the thickness is still 0 after the elements have been summed up, the system loads the
individual thickness from article master data.
The IG spacer is an exception (article type 200/211) as the spacer is adopted as its thickness
(kpos.szr or for the second spacer, kposp.szr2). But even for the spacer, the thickness from article
master data is necessary: It is the width by which the outside size differs from the inside size (7
mm are assumed by default).

Number of sub-elements

The ALCIB BOM generally allows to add certain sub-elements like e.g. accessories several times
just by changing the quantity.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                            48
The total quantity may be relevant e.g. to determine how many units were ordered, have to be
taken from stock, etc. It can be calculated by multiplying the item quantity by the element
quantity.
The item quantity is found in field Amount in the A+W-specific item extensions.




The element quantity is found in field multiplier of the corresponding product.


Calculation is correct even for elements below an element the quantity of which has been raised.
If a sub-element with a quantity of 3 has another sub-element for which a quantity of 2 is defined,
the total quantity is calculated from the item quantity multiplied by 6. ‚6’ is entered in the
multiplier.



Supply types

Supply types are shown for every element type as well as for grid sections as the procurement
information. They generally match the supply types in the BOM (aufstrukt.bestellkz). The
following values are are transferred:
    •   0 if aufstrukt.bestellkz is 0, i.e. undefined. For the transfer to ALCIM this means that the
        ALCIM master data will be used.
    •   1 if the supply type is Production (aufstrukt.bestellkz is 6 or 3) and cutting (AWTyp 1700
        or 1790 or article type 505) is defined for the element.
    •   2 if the supply type is Stock Withdrawal (aufstrukt.bestellkz is 2 or 5).
    •   3 if the supply type is Production (aufstrukt.bestellkz is 6 or 3) and if the element is just
        processed. These elements usually have the same article type as their child element; they
        have no defining processing of their own but are solely created by the processing of a
        secondary element.
    •   7 if an element is part of the delivery (aufstrukt.bestellkz is 7 or 9).
    •   8, if an element is produced. aufstrukt.bestellkz is 6 or 3 and the element has a defining
        processing step (like toughening for toughened glass or IG /laminated glass assembly)
        which is not Cutting.
    •   9 if the element is ordered (aufstrukt.bestellkz is 4 (or 1)
The following EDI supply types can also be loaded:
    •   12 means P.O. before EDI and will be used if aufstrukt.bestellkz is 1 and a parent element
        is purchased.
    •   13 means 'production before EDI' and is used if aufstrukt.bestellkz is 3 and if a parent
        element is purchased.
    •   14 means Stock before EDI and will be used if the supply type is Stock Withdrawal
        (aufstrukt.bestellkz is 2) and a parent element is purchased.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                             49
    •   15 means Part of Delivery before EDI and is used if the supply type is Part of Delivery
        (aufstrukt.bestellkz is 9) and if a parent element is purchased.
    •   16 means Cutting before EDI and will be used if the supply type is Production
        (aufstrukt.bestellkz is 3), part of which is cut (AWTyp 1700 or 1790 or article type 505)
        while a parent element is purchased.
    •   17 means Processing before EDI and will be used if the supply type is Production
        (aufstrukt.bestellkz is 3), if the element is just processed, and a parent element is
        purchased. Processed elements usually have the same article type as their child element;
        they have no defining processing of their own but are solely created by the processing of
        a secondary element.
Not all of the "EDI" supply types on the ALCIB BOM are relevant. In case of incomplete BOM
transfer, they will be considered only as supply type "before EDI" if they are found on the BOM
level right below a purchased element. This also applies if META elements are used which usually
shall be ignored. If the complete BOM is transferred - as recommended for ALCIM - the entire
BOM tree below the purchased element will be checked for EDI supply types; the system will only
stop at elements on stock or included elements. "EDI" supply types that are not selected below a
purchased element will be adopted as standard supply type.
Especially for META elements, supply type "Production before EDI" (3) means that all direct sub-
elements and processing steps with supply type "before EDI" will be adopted.
If no "before EDI" supply types shall be considered in general, the ALCIB switch
ORDERXML_NODFUEPROCUREMENT can be enabled and set to ON.
Open items known in this logic: How should packing processing be handled in the BOM below
purchased elements? We should be grateful for feedback from the project team.
Laminated film cutting
Laminated film usually gets a processing step (cutting) in the ALCIB BOM. Normally, this does not
entail any further logic as for other glass, i.e. film is mostly cut from a roll and does not have to be
optimised, nor does it require stockplate definitions. This is why film the supply type of film -
unlike that of glass - is not set from "Production" to "Cutting" in ALCIB if it is to be cut, but
remains 'Production'. Changing the supply type to "Cutting" can be configured however.
The supply type of produced laminated film can be changed to 'cutting' in the following
conditions:
    •   Enable the ALCIB switch ORDERXML_FOLIENZUSCHNITTSBESCHAFFART and set it to 'ON'.
    •   The laminated film has to consist of film stocksize and processing 'cutting'.
Changing the supply type of film - especially if ALCIM is the receiving production system - makes
sense only if film can be optimised and the corresponding stockplates can be defined.

IG with more than three sheets

Quadruple IG can be handled from OrderXML service Version 3.6 and ALCIB 2011 upwards.
The
airspace details will be adopted for the spacer thickness. This is based on the sequence in which
the spacers are defined in the BOM. This means: AIR1 is used for the first spacer on the BOM,
AIR2 for the second spacer on the BOM, and AIR3 for the third spacer on the BOM.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                            50
The assembly position which is mandatory for IG units consisting of more than two sheets, defines
the actual sequence for the transfer (and can therefore principally differ from the BOM
sequence). It is also used for the correct allocation of Georgian bar patterns and sealants.

Transferring fire protection glass to ALCIM by OrderXML

Fire protection glass has an individual item type (160) in ALCIB, as do its fillings (177). The
following graphic shows an example structure.




A fire protection glass can be recorded as a header part and as a sub-part (e.g. an ISO).
Even if the article type is known only in ALCIB, transfer to ALCIM is possible without problems.
We recommend to define in ALCIM master data the glass article „Cast resin (9)“ as the article type
and to choose "Cast resin filling" (11) for the filling.
ALCIM also imports additional airspace information for fire protection glass (table pool_szr). This
permits to release this element separately, using a special batch type.
For fire protection glass, analog to the ISO framework, the table pool_szr
is filled. While some of the information shown in the tables pool_szr and pool_pos are redundant
for IG spacers (e.g. airspace), this adjustment will be prevented for fire protection glass fillings.
Also to be heeded is that the program logic of the import currently assumes that for BSG fillings
no sealings and no gas fillings can be defined. Should this nevertheless occur, additional program
adjustments are necessary.
The following information is imported from ALCIB into pool_szr for fire protection fillings (the
corresponding field in the OrderXML file is shown in brackets):
    •   lfd_nr Is a serial number for spacer articles in the current item. (a parts list can include
        more than one fire protection glass and the fire protection glass can be underneath an
        ISO).
    •   Biegertextnr     will not be filled for fire protection glass fillings
    •   gas_typ, gas_artnr, gas_name, gas_name_kurz:
        The program assumes that fire protection glass fillings cannot include gas. There will be
        no import
    •   rahmentyp (Item Spacer – typeID)         The article type (177) is imported as a distinction
        from IG spacers. Alternatively, the type can be determined by SP.
    •   rahmentyp_name (item spacer - typeDescription)
        The article name for the filling will be adopted from article master data (artikel.artbez1).
    •   rahmentyp_name_kurz (item spacer - shortTypeDescription)
        The short name for the filling will be adopted from article master data (artikel.kurzbez).



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                             51
    •   rahmenfarbe, rahmenfarbe_name, rahmenfarbe_name_kurz
        Will not be imported at present.
    •   versiegeltyp, versiegel_artnr, versiegel_name, versiegeltiefe, versiegel_name_kurz
        Import can be made correctly only if no sealing has been defined for the fire protection
        glass fillings.
    •   Rahmenstaerke (item spacer - width):
        The thickness of the filling is adopted from article master data (artikel.staerke).
Starting with OrderXML Service version 13.04.2605 (AWDesk #428315) the artikel.staerke is
interpreted as „Thickness of spacer“ and transferred to the OrderXML file into attribute
„thickness“ of element <SHAPE>.


New parameter for fire protection glass filling (AWDesk #428315)
Starting with OrderXML Service version 13.04.2605, additional parameters are transferred for FPG
fillings (atyp 177)
A FPG production of Vetrotech (SGG) requires the following three indications in production:
    •   Thickness of spacer (IZR) (sketch, green arrow)
    •   Width of spacer (TPSD) (sketch, red arrow)
    •   Cutback (ILAM/2) (sketch, blue arrow)




In order to be able to assign the parameters "Width of spacer" and "Cutback" to an article of atyp
177 in the AWE, a record must be created for the article in the "Mandatory dimensions" (table
musskenn).
In the OrderXML transfer, the new parameters are determined as follows and the OrderXML file is
written:
 Name                         AWE DB field            OrderXML element
 Spacer thickness (IZR)       artikel.staerke         Elements <SPACER>, attribute „thickness“
 Spacer width (TPSD)          musskenn.gv14           Elements <SPACER>, attribute „width“
 Cutback (ILAM/2)             muskenn.gv15            Element <CUTBACK>, attribute “value”



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                         52
                                                    Same value for each edge:
                                                    <CUTBACK edge="all"
                                                    value="<muskenn.gv15>" />




1.5.4. Determination of processing information
Allocating Processing Steps to Elements

Processing steps and the corresponding information are imported in a list as part of the element
information.




This means that the processing steps have to be allocated to the corresponding elements.
The way in which this allocation is made depends on the element's article type or on the A+W
processing type of the processing step.
The program always searches for the first (defining) processing step. The following processing
steps (subsequent processing) will be allocated to the same element.
The sequence is determined solely by the sequence in the BOM. If a different sequence is
required for production, this can only be determined by the production system.
Note:
This means that processing mode 1 has to set in ALCIM. In this mode, the import determines the
sequence based on its own master data.


For clarification, here is the BOM of a toughened sheet:




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                        53
Rules:
-       Cutting is the defining processing step for float glass.
-       Subsequent processing steps are:
        - Edges ground
        - Edges bevelled
-       Toughening is the defining processing step for a toughened sheet and is therefore
adopted as the first processing step for toughened glass.
        Actually, toughened glass is a special case. Processing steps on the same BOM level or
behind a defining processing step (like stamping) will generally be allocated to the same element
as the defining processing step. There is a special logic which only applies to toughened glass, see
chapter
        0 „Bearbeitungen unterhalb eines ESG“
Another example is laminated glass which can be cut or produced:




Depending on the supply type of the stock size, the first processing step loaded for laminated
glass number 99531167 is:
-        cutting (if the supply type is 'stock'), or
-        laminated glass production (if the supply type is 'production').
Only if the system is configured to consider the complete BOM (switch
ORDERXML_KOMPLETTESTUECKLISTE), both processing steps may be adopted (for a detailed
description of this special case please see 1.6.6 „Zusammbau- oder Zuschnitts-Bearbeitung“).
-         “Edges ground“ is adopted as the next processing step for element
 99531167.

-       Packing is a special case: It is moved one level upwards and is therefore adopted as a
process for the main element.
The above examples shall serve to explain how decisive the processing type is for the allocation of
processing steps to the element in question.
The example of an IG BOM shall show that the sequence in the BOM is decisive too:



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                         54
The edges of the IG unit shall be "roughly adjusted" after processing.
This means that the processing step must be added to the BOM after the "defining" processing
step, i.e. after IG production.
Adding this step before IG production is wrong. The processing would be allocated to one of the
sub-elements at random. Because this is edgework which is considered to be a subsequent
processing step. It will be allocated to the last element for which a defining processing step has
been found.
    •   The following processing article types are considered to be defining and are therfore
        usually applied as the first processing step for an element: 505 glass cutting, 703 wood
        cutting, 515 toughening, 516 pre-toughening, 518 laminated glass press, 519 laminated
        glass production, 521 fire protection glass production, 530 IG production, 532 spacer
        production, 534 Georgian bar construction
    •   The following processing article types are usually considered to be subsequent processing
        steps: 512 bending, 513 curving, 550 grinding, 551 mitres, 552 fluted bevelling,
        553 arrissing, 560 drilling, 561 counter-sunk holes, 565 rounded corners, 566 cut-off
        corner, 570 cut-out corner, 571 edge cut-out, 585 enamel, 586 etching, 587 sand
        blasting, 588 silk screening, 589 coating, 531 airspace filling, 700 heat soak.
    •   The following processing article types are considered to be subsequent processing steps
        but can be adopted as the first processing step where processed fixed sizes are used:
        520 glazing, 525 assembly, 545 packing.
    •   The following processing article types may affect additional elements/accessories in
        which case they are defining; otherwise they are subsequent processing steps for glass:
        535 basic assembly, 575 recessed grip, 580 ticket window, 590 enamel strip, 591 stamp,
        594 pressure compensation, 595 UV cover, 596 inside thread, 597 chamfers,
        598 moulding, 599 gluing, 540 other processing, 584 painting, 999 other
Allocation is even clearer if the processing step is allocated to an A+Wprocessing type .
    •   The following A+W processing types are considered as defining and are therefore usually
        applied as the first processing step to an element: 1500 toughening, 1510 pre-toughening,
        1530 laminated glass pre-compound, 1540 laminating, 1590 other thermal processing,
        1600 IG assembly, 1610 cast resin assembly, 1620 spacer filling, 1640 Georgian bar
        construction, 1680 fire protection glass assembly, 1700 cutting, 1790 other cutting.
    •   The following A+W processing types are considered to be subsequent processing steps:
        1000 arrissing, 1005 grinding, 1010 polishing, 1015 mitre, 1020 bevelling, 1025 edge
        stripping, 1030 sawing, 1090 other edgework, 1100 drilling, 1110 counter-sunk hole,
        1190 other drilling, 1200 coating, 1205 frosting, 1210 sand-blasting, 1215 colouring,
        1220 enamel, 1225 silk screening, 1230 fluted bevelling, 1235 bending, 1240 curving,
        1290 other surface treatment, 1300 cut-out corner, 1305 cut-off corner, 1310 rounded



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                          55
        corner, 1390 other corner treatment, 1400 edge cut-out, 1415 inside cut-out, 1420 NC
        processing, 1490 other geometrical processing, 1520 heat soak, 1630 airspace filling,
        1650 UV protection, 1660 pressure compensation, 1670 edge protection fitting, 1900 SN
        macro.
    •   The following A+W processing types may affect additional elements/accessories in which
        case they are defining; otherwise they are subsequent processing steps for glass:
        1245 alarm wire, 1250 stamp, 1255 logo, 1405 ticket window, 1410 recess grip.
    •   The following processing types are considered to be subsequent processing steps but can
        be used as first processing steps for processed cut sizes: 1800 packing, 1810 shipping,
        1820 assembly, 1830 glazing.
Note:
Using A+W processing types is recommended because this allows the clear distinction of defining
procesing steps and subsequent processing steps.

Defined processing steps for elements with a supply type other than production

If the entire BOM shall be adopted (switch ORDERXML_KOMPLETTESTUECKLISTE is active), even
the elements and processing steps below the BOM of the element to be ordered, included in the
delivery, or withdrawn from stock will be adopted.
This does not include the processing steps defined for these elements. An element taken from
stock does not have to be produced. The defined processing would just be irritating; the
production system will create the processing step 'stock withdrawal' if necessary. Further
processing steps will be adopted however to show that an element withdrawn from stock has
been drilled or coated.
If the supply type of an element is not 'production', the defined processing steps will be removed
when the complete BOM is adopted.
Processing steps below a toughened sheet
To transfer an order via OrderXML one has to define the processing steps applying to the
individual elements. For most articles of an ALCIB BOM, the allocation is clear provided that the
recommended BOM hierarchy - produced/cut glass below processed glass - is obeyed.
Only for toughened glass products which might be processed after toughening, this
recommendation did not exist yet. Even for this type, a BOM hierarchy of the shape 'produced
toughened below processed toughened' can be used. For example:
        1st level                      2nd level                      3rd level
        processed toughened glass      produced toughened glass
                                                                      cut float 110005
        10355555                       300005
                                       post-processing 199130         arrissing 399141
                                                                      Toughening 399150




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                           56
In this example, the allocation of processing steps is clear: Arrissing is applied to the float glass
while toughening (in connection with the appropriate article or processing type) is the defining
processing step for the produced toughened sheet; post-processing is applied to the produced
toughened glass.
This recommendation may not be applied to existing bills of material however. This is why a
special logic has been implemented for toughened glass. The example BOM looks like this:


        1st level       2nd level
        TG 350004       Cut float glass 110004
                        Arrissing 399130
                        Furnace
                        Additional processing step added to the BOM by hand 199130




This example clearly shows that edges of the cut float sheet shall be ground. Toughening (the
appropriate article or processing type provided) is the defining processing step for the toughened
sheet. Whether the additional processing step (edge adjustment) shall be applied to the
toughened sheet or to the float sheet, cannot be defined as easily.
In future, it is possible to define in ALCIB master data the processing steps to be added in the
BOM after toughening. Basically, the program assumes that a toughened sheet cannot be
processed further, and allocates the additional processing step to the float. If the processing step
has been marked in master data for being performed after the furnace, it will be allocated to the
toughened glass.
To be precise: The "Mark" in master data is taken into account for processing steps which are in
the BOM hierarchy on the same level as the furnace (article type 515 or 516, or processing type
1500 or 1510) and are located behind the furnace. If the same marked processing shall be applied
to the float glass - i.e. before toughening - it must be added to the BOM before the furnace.
For all other products (with defining processing steps other than the furnace), the following
processing steps should be added to the BOM one level higher - as recommended - i.e. below the
processed glass. Otherwise, the BOM sequence is decisive for single annealed products:



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                              57
Processing steps on the same level as the defining processing step will be allocated to the glass
below if they are positioned before the defining processing step; they will be applied to the
parent glass if they are positioned behind the defining processing step.
Marking the relevant processing steps
Processing steps are marked in a configurable field in article master data. Two steps are required:
Use menu Master data > Field configuration > Article field configuration to check if the
corresponding field has already been configured. The field name must include the term
"ProcPostThermal" (please obey capitalization, no blanks!). A possible name would be:
"Proc.afterFurn (ProcPostThermal)". Please make sure that there is no other field the name of
which contains the character string "ProcPostThermal".
Select the relevant processing step from article master data (menu Master data > Articles). Use F4
to go to the menu and select Configurable fields. Allocate 1 to the field the name of which
includes the term "ProcPostThermal".
This definition is only necessary for processing steps which - on the same BOM level as the
furnace - can be added after the furnace, and can be actually applied to a toughened glass, i.e.
after the furnace. The master data of other processing steps are not affected.
To cancel the mark for a processing step, reset the entry in the configurable field to '0'.
Please note that the relevant processing steps can also be marked via script. This is done in the
following way:
Check if the configurable field has been defined already:
This is done by "select count(*) from artcomfld where fldbez matches
'*ProcPostThermal*'".
The quantity returned must be 1. If it is 0, the field must be defined in the menu as described.
The entries <fldbez>, <fldnrz>, <fldpos> and <fldnr> of this definition are necessary for the
following Insert. This is determined by "select fldbez, fldnr, fldnrz, fldpos from
artcomfld where fldbez matches '*ProcPostThermal*'".
For relevant processing steps, the article number (<artnr>) is used to check if a definition exists:
"select count(*) from artprvfld where artnr=artnr and fldbez matches
'*ProcPostThermal*'"
If the result is 0, an insert can be made for the processing step, using the determined
values:"insert into artprvfld (artnr, fldnr, fldpos, fldnrz, fldtyp,
fldbez, longval, decval, charval, dateval) values (<artnr>, <fldnr>,
<fldpos>, <fldnrz>, 1, <fldbez>, 1, 0.0, '', '05.10.2012')"
If there is a record in table artprvfld however, an update is required: "update artprvfld set
longval=1 where artnr=<artnr> and fldbez matches '*ProcPostThermal*'".
ProcPostThermal processing below purchased toughened glass
The meaning of these processing steps used to be unclear if the toughened sheet was not
produced but purchased for example. The rule is now : Since the processing steps - from the
ALCIB user's point of view - lie below the ordered article, they are irrelevant for production and
will be purchased. OrderXML will ignore these special processing steps and will not transfer them
to a production system (like ALCIM).
Processing steps to be applied to a toughened sheet which has been ordered therefore require a
BOM hierarchy in which the ordered toughened sheet is secondary to the processed toughened
sheet.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                             58
Processing Reference

Every processing step has a processing reference by which it is identified. In the OrderXML file,
this is the information „reference“. It matches the tupel number in the ALCIB BOM.
The reference is mainly important for reports to ALCIB which refer to a certain processing step.
Together with the order number and item reference, the processing step can be clearly identified
in ALCIB.

A+W Processing Types

If processing steps have been allocated to A+W processing types, they can be described by fixed,
unique parameters. In OrderXML, the element „awProcessing“ is used for this purpose.
Depending on the valid parameters for the corresponding A+W processing type, this element can
be filled in different ways.




The wealth of possibilities would overload this chapter as well as the recording in the
documentation file if every parameter for the individual types would be described. The table
showing which parameter in ALCIB is represented by which piece of information can be found in
„Anhang: A+W-Bearbeitungstyp-Informationen“.

Numbering of Edges for Edgework

The edges to be processed are defined for the edgework. The edges are numbered for this
purpose. The numbering is generally anti-clockwise. E.g. for a rectangle:

                                               3


                                4                            2


Please note:                                1
To determine the edges to be processed, the edge vector in ALCIB must be legible. BYTE_VEKTOR
configuration is therefore prerequisite.

Supply types




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                           59
Supply types are listed as procurement information. They generally match the supply types in the
BOM (aufstrukt.bestellkz). The following values are are transferred:
    •   0 if the processing step is relevant for production (aufstrukt.bestellkz is 0, 6 or 3)
    •   1 if processing is purchased (aufstrukt.bestellkz is 4, 1, 7 or 9), i.e. has to be made by
        another company.
    •   2 if the processed element is to be taken from stock (aufstrukt.bestellkz is 2 or 5
The following EDI supply types can be imported:
    •   12 means P.O. before EDI and will be used if aufstrukt.bestellkz is 1 and the direct parent
        element is purchased.
    •   13 means Production before EDI and will be used if aufstrukt.bestellkz is 3 and the direct
        parent element is purchased.
Not all of the "EDI" supply types on the ALCIB BOM are relevant. In case of incomplete BOM
transfer, they will be considered only as supply type "before EDI" if they are found on the BOM
level right below a purchased element. This also applies if META elements are used which usually
shall be ignored. If the complete BOM is transferred - as recommended for ALCIM - the entire
BOM tree below the purchased element will be checked for EDI supply types; the system will only
stop at elements on stock or included elements. "EDI" supply types that are not selected below a
purchased element will be adopted as standard supply type.
Especially for META elements, supply type "Production before EDI" (3) means that all direct sub-
elements and processing steps with supply type "before EDI" will be adopted.
If no "before EDI" supply types shall be considered in general, the ALCIB switch
ORDERXML_NODFUEPROCUREMENT can be enabled and set to ON.
If ALCIM is the target system please note that ACLIM knows only supply types for elements. If a
supplier shall just do the processing, this can usually be handled by defining another glass level in
the ALCIB BOM and allocating the supply types 'P.O.' and 'Production before EDI' to these
elements.

Suppressing processing steps with supply type ‚none’

Basically, OrderXML adopts all processing steps from the ALCIB BOM. The receiving production
system usually decides which processing steps are relevant and which are not.
The system can be configured now so that processing steps explicitly set to supply type "non" in
the ALCIB BOM, will be suppressed in the OrderXML file.
Please note: Defining processing steps (like cutting, toughening or IG production) to be executed
in the ALCIB BOM below a purchased or stock article, do not have to be explicitly set to supply
type "none". They will be suppressed anyway.
To suppress processing steps of the supply type "none" in the OrderXML file, activate the switch
ORDERXML_IGNORIERE_BEARB_BESTELLKZ0 in ALCIB and set it to 'ON'.

Interlayer cutting as additional processing on LAMI

An interlayer cutting (atyp 752) can be interepreted in two different ways. If the interlayer cutting
is applied under a foil in the AWE BOM, this is the defining processing for the foil. If the interlayer
cutting is applied in the AWE BOM under a LAMI stock dimension, this is an additional processing



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                           60
with which during production of the LAMI , the protruding foil must be cut off again after the
LAMI assembly.

This additional processing "Cut off foil on the LAMI" must be assigned in the OrderXML transfer to
the LAMI fixed dimension during production of the LAMI.

It must be noted that the interlayer cutting must be created in the master data of the production
system with the correct article type (1792).

See also AWDesk #456476.


1.5.5. Customised information
As described above, the logic that defines which information is to be adopted is based on the
direct data import into ALCIM. Customised information could usually be determined and provided
by stored procedures (SP) there. There were also SPs for various texts.
Most SPs can also be used by the OrderXML interface under certain circumstances - if they are
needed at all asa standard information will be adopted for all SPs.
Text SPs are also availabale. As an alternative or completion, the OrderXML interface also has its
own mechanism for creating text.
The tool ALINFOTOXML can be used to define whether and which SPs shall be used and how text
has to be imported. This tool can be loaded from the Fix menu by which the programs ALCIB,
LAGER, ... are loaded as well.
Note:
This tool is meant for project engineers. Title, column information, and contents are therefore
shown in English so that it can still be operated when installed for a customer who does not speak
a universal language.
The tool can be loaded from the WINCIB menu. There it appears by the abbreviated name
„INFOTOXML“.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                        61
Stored Procedures

This is an example from the documentation file DokuInfosOrderXMLAlcib.txt:
        <ORDER ITEM - USER EXTENT - MainLineItemID=
                If SP exists and is usable cupmawpphauptpos(auftrnr, aufnr, 0, posnr, poskonr) is called,
                else item reference created from kpos.posnr and rack sequence: to pool_pos.h_pos>



As in this example, for every piece of information in OrderXML there is a standard logic defining
how it is determined from ALCIB data. For some bits of information, special stored procedures can
be defined alternatively to customise the information.
When switching from another interface to ALCIM please note that this interface offers the same
SPs as Direct Data Import. This shall make the change easier. It can be guaranteed that nearly the
same information can be transferred by the OrderXML interface as determined by the Direct Data
Import.
Standard information also help to minimise the project work for new installations.
Initially, the OrderXML service will always use the standard information. Even if there is an SP.
This allows to test the SP thoroughly before using it. When replacing the Direct Data Import
please note however that once the OrderXML interface has been introduced, PMS data will no
longer be available. SPs which were used there must therefore be checked as to whether they still
access PMS data; this may have to be amended.



A+W Software GmbH             EN-CONFIG-A+W EnterpriseProductionInterface.docx                              62
After that, the SP can be released. This is done by the tool ALINFOTOXML.
An entry is shown for every SP known to the OrderXML service. Please note that new entries can
only be made by development. These entries have to be made known to the OrderXML service by
development so that they can be taken into account.
SP entries are marked in the tool by „SP“ in column Type. Column Key shows the SP's number.
Entry "1" in column Set defines that the SP shall be executed by the OrderXML service. Enter „0“
or delete the „1“ if the SP shall not be loaded any more.
Note:
Only release the SP after it has been checked and tested. If must not include any access to PMS
tables.
The change of release of a SP by means of the tool ALINFOTOXML is activated by rebooting the
Windows service or becomes active automatically if the service starts the next cycle. The switch
„MaxNumOrders“ defines the number of orders after which the change is automtically activated.
Suggestion:
SPs are a useful way of quickly reacting to new customer requirements. Running SPs takes time
however. If a SP is therefore introduced to transfer information in a closed version which is not
available yet in the interface but is still generally valid, a short note to development would be
useful. Development can then check whether the information can be transferred as a default
value in the next version.
The following SPs can be released by the tool
All SPs listed below, in alphabetical order, can be released by the tool). A short description is
followed by the value that is adopted if the SP is not released (default), the transfer parameters,
and the required return values (in the defined sequence). The documentation file
DokuInfosOrderXMLAlcib.txt tells you where the returned information can be found in OrderXML.
    •   Cupmawpaauftxt:         Is loaded in a loop and can return one or two order-specific texts.

                All texts provided by the SP are listed in OrderXML.
        Default:         Can also be defined by this tool, see below.
        Transfer parameters: INTEGER = kauf.auftrnr (external order number)
                INTEGER = kauf.aufnr (internal order number)
        Return values: Per text:
                SMALLINT         = self-defined ID for the text type
                CHAR(80)         = Text to be imported
                CHAR(2)          = historical reason. Can consist of two blanks in a byte vector
        configuration
                INTEGER          = historical reasons. Always -1 in a byte vector configuration.
    •   cupmawpaktext1:        1. customer text, e.g. for informationen on the delivery note.
        Default:       Field exaufnr from table kauf.
        Transfer parameters: INTEGER = kauf.auftrnr (external order number)
                INTEGER = kauf.aufnr (internal order number)
        Return values: CHAR(32)         = Text to be imported
    •   cupmawpaktext2:        2. customer text, e.g. for information on the delivery note.
        Default:       Field exbez1 from table kauf.
        Transfer parameters: INTEGER = kauf.auftrnr (external order number)
                INTEGER = kauf.aufnr (internal order number)
        Return values: CHAR(32)        = Text to be imported



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                           63
   •   cupmawpaktext3         3 customer text, e.g. for information on the delivery note.
       Default:       Field exbez2 from table kauf.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
       Return values: CHAR(32)        = Text to be imported
   •   cupmawpakusprache: Customer language
       Default:          Fixed code depending on the information
               sprzu.alenvsprkz which is selected by kauf.sprkz:
               ger: if 1; ben: if 2,         fre: if 3, dut: if 4,
               swe: if 5, dan: if 6, nor: if 7,
               fin: if 8, spa: if 9, ita: if 10, pol: if 11,
               cze: if 12,        kor: if 13, eng: if 14, nor: if 15,
               jpn: if 16.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               SMALLINT = kauf.aufnr (internal order number)
               SMALLINT =
       Return values: CHAR(3)                = The SP can return the following language codes which
       are converted to the codes listed above (shown behind the code): GER (ger), GB (ben), F
       (fre),
                         NL (dut), SV (swe), DAN (dan), NOR (nor),
                         FIN (fin), SP (spa), I (ita), PL (pol), CZ (cze),
                         KOR (kor), USA (eng), PT (por), JP (jpn)
       .
   •   cupmawpasonderkz1 1. order-related special code. Numerical value for customised
       codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
       Return values: SMALLINT        = Customised code
   •   cupmawpasonderkz2 2. order-related special code. Numerical value for customised
       codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
       Return values: SMALLINT        = Customised code
   •   cupmawpauftyp           Order type or category
       Default:        depends on the fields _kaufart, schnell and eingang in table kauf: express,
       test, normal, reservation, call, stock, high priority, replacement. This text appears based
       on the Alenv language set in table xsprzu as the national language.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
       Return values: CHAR(10)           = Text entry for the category
   •   cupmawpbiekz Code (ID) for a spacer text.
       Default:      For the current spacer element, field rahmtxtnr from table artikel.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)



A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                          64
              SMALLINT = kpos.poskonr (BOM header number)
       Return values: SMALLINT     = Text code to be imported
   •   cupmawpbtext2          Additional processing name
       Default:       For the current processing article, field artbez2 from table artikel.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = immer 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
               SMALLINT = aufstrukt.tnr (Tupel number of processing)
       Return values: CHAR(80)        = Code to be imported
   •   cupmawpbtext3          Additional processing name
       Default:       For the current processing article, field kurzbez from table artikel.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = immer 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
               SMALLINT = aufstrukt.tnr (Tupel number of processing)
       Return values: CHAR(80)        = Code to be imported
   •   cupmawppauftxt           First SP for item-specific text
               Is loaded in a loop and can return one or more item-specific texts.
               All texts provided by the SP are listed in OrderXML.
       Default:         Can also be defined by this tool, see below.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (for historical reasons)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: Per text:
               SMALLINT         = self-defined ID for the text type
               CHAR(80)         = Text to be imported
               CHAR(2)          = historical reasons. Can consist always of two blanks in a byte
       vector configuration
               INTEGER          = historical reason. Always -1 in a byte vector configuration.
   •   Cupmawppbez3            Additional name for the header.
       Default:       artikel.artbez3
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: CHAR(30) = first information to be imported
   •   cupmawppextra          Supplementary information on the order item.
       Default:      -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = immer 0 (historic reason)



A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                           65
              SMALLINT = kpos.posnr (internal item number)
              SMALLINT = kpos.poskonr (BOM header number)
       Return values: CHAR(16) = first information to be imported
              CHAR(16) = second information to be imported
              CHAR(16) = third information to be imported
              CHAR(16) = fourth information to be imported
              CHAR(16) = fifth information to be imported
   •   cupmawppfrei73         Label code.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = immer 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: SMALLINT = first information to be imported
   •   cupmawpphauptpos Main item
       Default:        Is an item reference by default, in the shape of
               „2001“ - for: Internal item number 2 and first rack
               (item can be split to different racks).
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: INTEGER = Number of main item
   •   cupmawppkkommiss1 Reference text
       Default:       Information from field kommtxt in table komm; limited to the first 50
       characters.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = immer 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: CHAR(50) = reference text to be imported
   •   cupmawppkkommiss2 extended reference text
       Default:        If the information in field kommtxt in table komm exceeds 50 characters,
       the additional characters are imported here.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = immer 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: CHAR(50) = reference text to be imported
   •   cupmawpppmptxt           Second SP for item-specific text
               Is loaded in a loop and can return one or more item-specific texts.
               All texts provided by the SP are listed in OrderXML.
       Default:         Can also be defined by this tool, see below.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)



A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                      66
              INTEGER = kauf.aufnr (internal order number)
              SMALLINT = always 0 (historical reason)
              SMALLINT = kpos.posnr (internal item number)
              SMALLINT = kpos.poskonr (BOM header number)
       Rückgabewerte:        Per text:
              SMALLINT       = self-defined ID for the text type
              CHAR(80)       = Text to be imported.
   •   cupmawppsonderkz1 1. item-related special code. Numerical value for customised
       codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: SMALLINT        = code to be imported
   •   cupmawppsonderkz2 2. item-related special code. Numerical value for customised
       codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: SMALLINT        = code to be imported
   •   cupmawppsondertxt1 1. item-related special text. Text value for customised codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = immer 0 (historic reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: CHAR(32)        = special text to be imported
   •   cupmawppsondertxt2 2. item-related special text. Text value for customised codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = immer 0 (historic reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
       Return values: CHAR(32)        = special text to be imported
   •   cupmawppspectxt          Third SP for item-specific text
               Is loaded in a loop and can return one or more item-specific texts.
               All texts provided by the SP are listed in OrderXML.
       Default:         Can also be defined by this tool, see below.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reason)



A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                   67
              SMALLINT = kpos.posnr (internal item number)
              SMALLINT = kpos.poskonr (BOM header number)
       Rückgabewerte:       Per text:
              SMALLINT      = self-defined ID for the text type
              CHAR(80)      = Text to be imported.
   •   cupmawptauftxt            First SP for tupel-based text
                If loaded in a loop and can return one or more tupel-based text.
                All texts provided by the SP are listed in OrderXML.
       Default:          Can also be defined by this tool, see below.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
                INTEGER = kauf.aufnr (internal order number)
                SMALLINT = always 0 (historical reasons)
                SMALLINT = kpos.posnr (internal item number)
                SMALLINT = kpos.poskonr (BOM header number)
                SMALLINT = aufstrukt.tnr (tupel number of the imported element or processing
       article)
       Return values: Per text:
                SMALLINT         = self-defined ID for the text type
                CHAR(80)         = text to be imported
                CHAR(2)          = historical reasons. Can consist of two blanks in a byte vector
       configuration
                INTEGER          = historical reasons. Always -1 in a byte vector configuration.
   •   cupmawptbez2 Additional name for an imported BOM element
       Default:     For the current element, field artbez2 from table artikel.

       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
              INTEGER = kauf.aufnr (internal order number)
              SMALLINT = always 0 (historical reason)
              SMALLINT = kpos.posnr (internal item number)
              SMALLINT = kpos.poskonr (BOM header number)
              SMALLINT = aufstrukt.tnr (Tupel number of the element)
       Return values: CHAR(30)       = Name to be imported
   •   cupmawptdichttyp              By default, the sealing types are loaded from the sealant's article
       master data. Alternatively, the type can be determined by customer now.
       Default:            artikel.versieglungstyp (for the sealant)
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
                 INTEGER = kauf.aufnr (internal order number)
                 SMALLINT = kpos.posnr (internal item number)
                 SMALLINT = kpos.poskonr (BOM header number)
                 SMALLINT = aufstrukt.tnr (tupel number of spacer)
       Rückgabewerte:               SMALLINT         = numerical code for the spacer type.
       The SP is loaded for all airspace articles, i.e. IS spacers, cast resin and fire protection glass
       fillings. If its value shall not be analysed, the SP can return ‚-1’.
   •   cupmawptkurz Additional name for an imported BOM element
       Default:     For the current element, field kurzbez from table artikel.

       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
              INTEGER = kauf.aufnr (internal order number)
              SMALLINT = always 0 (historical reason)



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                             68
              SMALLINT = kpos.posnr (internal item number)
              SMALLINT = kpos.poskonr (BOM header number)
              SMALLINT = aufstrukt.tnr (Tupel number of the element)
       Return values: CHAR(30)       = Name to be imported
   •   cupmawptpmptxt            Second SP for tupel-based text
                Is loaded in a loop and can return one or more tupel-based texts.
                All texts provided by the SP are listed in OrderXML.
       Default:          Can also be defined by this tool, see below.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
                INTEGER = kauf.aufnr (internal order number)
                SMALLINT = always 0 (historical reasons)
                SMALLINT = kpos.posnr (internal item number)
                SMALLINT = kpos.poskonr (BOM header number)
                SMALLINT = aufstrukt.tnr (tupel number of the imported element or processing
       article)
       Return values: Per text:
                SMALLINT         = self-defined ID for the text type
                CHAR(80)         = text to be imported
   •   cupmawptrahmenfarb By default, spacer colours cannot be defined for the spacer itself
       because spacers already have size variants. The color can either be defined for an article
       of a special article type in the spacer BOM, or can be defined by customer.
       Default:            see description of the switch
                 PMQCIM_TYPRAHMENFARBTEXT
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
                 INTEGER = kauf.aufnr (internal order number)
                 SMALLINT = kpos.posnr (internal item number)
                 SMALLINT = kpos.poskonr (BOM header number)
                 SMALLINT = aufstrukt.tnr (Tupel number of the element)
       Return values: SMALLINT              = numeric code for the spacer colour.
       The SP is loaded for all airspace articles, i.e. IS spacers, cast resin and fire protection glass
       fillings. If its value shall not be analysed, the SP can return ‚-1’.
   •   cupmawptrahmentyp By default, the spacer types are loaded from article master data.
       For production, e.g. for bender control, a more detailed distinction or a different
       numbering of spacer types may be necessary. In this case, spacer types can be
       determined by customer now.
       Default:       artikel.rtyp
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
               SMALLINT = aufstrukt.tnr (tupel number of the element)
       Return values: SMALLINT         = numerical code for the spacer type.
   •   cupmawptsonderkz1 1. tupel-based special code for the currently imported BOM
       element. Numerical value for customised codes.
       Default:      -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historic reason)
               SMALLINT = kpos.posnr (internal item number)



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                             69
              SMALLINT = kpos.poskonr (BOM heder number)
              SMALLINT = aufstrukt.tnr (Tupel number of the element)
       Return values: SMALLINT       = code to be imported
   •   cupmawptsonderkz2 2. tupel-based special code for the currently imported BOM
       element. Numerical value for customised codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historic reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM heder number)
               SMALLINT = aufstrukt.tnr (Tupel number of the element)
       Return values: SMALLINT        = code to be imported
   •   cupmawptsonderkz3 3. tupel-based special code for the currently imported BOM
       element. Numerical value for customised codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historic reason)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM heder number)
               SMALLINT = aufstrukt.tnr (Tupel number of the element)
       Return values: SMALLINT        = code to be imported
   •   cupmawptsondertxt1 1. tupel-based special text for the currently imported BOM
       element. Text value for customised codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reasons)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
               SMALLINT = aufstrukt.tnr (tupel number of the element)
       Return values: CHAR(32)        = special text to be imported
   •   cupmawptsondertxt2 2. tupel-based special text for the currently imported BOM
       element. Text value for customised codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reasons)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
               SMALLINT = aufstrukt.tnr (tupel number of the element)
       Return values: CHAR(32)        = special text to be imported
   •   cupmawptsondertxt3 3. tupel-based special text for the currently imported BOM
       element. Text value for customised codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)



A+W Software GmbH      EN-CONFIG-A+W EnterpriseProductionInterface.docx                70
              SMALLINT = always 0 (historical reasons)
              SMALLINT = kpos.posnr (internal item number)
              SMALLINT = kpos.poskonr (BOM header number)
              SMALLINT = aufstrukt.tnr (tupel number of the element)
       Return values: CHAR(32)       = special text to be imported
   •   cupmawptsondertxt4 4. tupel-based special text for the currently imported BOM
       element. Text value for customised codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reasons)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
               SMALLINT = aufstrukt.tnr (tupel number of the element)
       Return values: CHAR(32)        = special text to be imported
   •   cupmawptsondertxt5 5. tupel-based special text for the currently imported BOM
       element. Text value for customised codes.
       Default:       -
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reasons)
               SMALLINT = kpos.posnr (internal item number)
               SMALLINT = kpos.poskonr (BOM header number)
               SMALLINT = aufstrukt.tnr (tupel number of the element)
       Return values: CHAR(32)        = special text to be imported
   •   cupmawptspectxt           Third SP for tupel-based text
                Is loaded in a loop and can return one or more tupel-based texts.
                All texts provided by the SP are listed in OrderXML.
       Default:          Can also be defined by this tool, see below.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
                INTEGER = kauf.aufnr (internal order number)
                SMALLINT = always 0 (historical reasons)
                SMALLINT = kpos.posnr (internal item number)
                SMALLINT = kpos.poskonr (BOM header number)
                SMALLINT = aufstrukt.tnr (tupel number of the imported element or processing
       article)
       Return values: Per text:
                SMALLINT         = self-defined ID for the text type
                CHAR(80)         = text to be imported
   •   cupmawpvtiefe Returns the sealing depth for a spacer.
               Sealing depth + spacer thickness define the cutback for spacers and Georgian
       bars.
       Default:         If MODUL_VERSIEGELUNGSTIEFE or
                ISO_RAHMEN_MODELL is set, the fields
               diff1-diff10 are imported from
               table kstufparam. Otherwise, the standard cutback is defined by field aham in
       table kpos, divided by 2.
       Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)



A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                       71
                SMALLINT = always 0 (historical reasons)
                SMALLINT = kpos.posnr (internal item number)
                SMALLINT = kpos.poskonr (BOM header number)
                SMALLINT = aufstrukt.tnr (tupel number of the imported element or processing
        article)
        Return values: DECIMAL= value for the sealing depth in millimetres.
Note for switching from Direct Data Import
Tupel-based SPs always receive the tupel number of the corresponding element or processing
step. This applies especially to the main element where 1 is transferred as the tupel number (not
0 as in former ALCIM interfaces).


The following SPs are available but are not shown in the tool
A special bender text for spacers can be determined. This function can be enabled by ALCIB
environment switch PMXTRAHMENSP. To determine the text by SP, the name of the SP must be
defined by the environment switch in this case. Please enable this switch only after checking and
testing the SP. The following parameters are valid for the SP
    •
        Transfer parameters: INTEGER = kauf.auftrnr (external order number)
               INTEGER = kauf.aufnr (internal order number)
               SMALLINT = always 0 (historical reason)
               SMALLINT = kpos.posnr (internal item number)
    •   Return values: INTEGER
                             A return value is expected here but the text
                             to be imported must be written by the SP
                             in table pmxtrahmen.
Unlike in Direct Data Import (ALCIM), the following SPs are no longer available
Cupmawpisdefbearb: How to allocate the individual processing steps of the BOM to the
corresponding elements is described in chapter 1.4.4 „Ermittlung von
Bearbeitungsinformationen“.
cupmawpprahmenkz: All values determined by the SP can be defined by master data or suitable
BOM structures, or by an element-based SP (there more as there can be two or three spacers in a
bill of materials).
cupmawppfrei61: The SP determined if text records existed for an item. This information can be
determined by the number of records in ORDER_ITEM - USER_DEFINED_EXTENSIONS -
CUSTOMER_REFERENCE.
cupmawptfrei19: The SP determined the element-based label code. This information - if necessary
- should only be defined by the production system; transfer via this interface is therefore not
planned at present.
cupmawppmenge: Was used to determine an alternative production quantity. If more or less
units are to be produced however, this should be defined by a suitable logic in ALCIB or in the
production system. Loading the SP in the interface causes inconsistencies between the two
systems and may result in incomprehensible quantities.
cupmawppbez2: Should be taken into account if the ALCIM interface is to be used. These SPs
could be used to determine names for the items. ALCIM uses this interface however to import the
corresponding information on the main element into item data (see cupmawptbez2).



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                         72
Texts

The previous chapter lists various SPs that can be used to determine text records for the interface.
A standard logic for text is also available. The SPs are just used for the sake of completeness in
this case.
The defined standard logic can be configured by the tool ALINFOTOXML . This tool shows all texts
which can be imported already by default. These are the records labelled Text in field Type.
Field Key now defines the text type. We distinguish order-based, item-based, and tupel-related
text. We also distinguish created text and text entered by hand. Text can also be allocated to
different forms.
Field Set shows a number for the text type. The interface transfers it as information <ADVICE –
key>. For example:
         <ADVICE typeID="Production" key="2033" text="LG process. 10mm“ number="1" />
This text type number serves for the grouping of text. It can e.g. be used in the production system
as a code if only certain text types shall appear on certain production lists.
Standard text is configured by this text type number, i.e. by means of the field Set. Enter ‚0’ (zero)
if the text shall not be adopted. Any entry over 0 means that this type of text shall be determined.

You can also enter a text type number other than the preset one. This allows to combine text
types. This may be useful for example if the distinction as to whether text shall be created
automatically or entered by hand is immaterial.
In connection with ALCIM we recommend to use text type numbers in the 2000 range because
there are no fixed numbers in this area; this section also includes the standard text numbers.
The text types that can be determined by the service by default are listed below together with a
short description. The name matches the name in the tool's key column.
All listed text types are loaded from table auftxt. A text can appear in the OrderXML file several
times if it is allocated to various forms and if several of these forms have been defined as transfer-
relevant.
Note:
To enable the service to recognise the allocation of forms and text, the form vector in table auftxt
must be available in legible form. BYTE_VEKTOR configuration is therefore mandatory.
Order-specific text
1.       Automatically created text
     •   1: Man. Cutting List, Order, generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Manual Cutting List. This means that the 7th
         flag of the form vector is set to 1, representing a bit value of 1. Field auftxt.generiert is
         not 0.
         If not customised already, this text is adopted with text type number 2050.
     •   512: Label       , Order, generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Label. This means that the 13th flag of the
         form vector is set to 1, representing a bit value of 512. Field auftxt.generiert is not 0.
         If not customised already, the text is adopted with text type number 2022.




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                              73
     •   1024: Work order       , Order, generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Work Order. This means that the 12th flag of
         the fom vector is set to 1, representing a bit value of 1024. Field auftxt.generiert is not 0.

         If not customised already, the text is adopted with text type number 2053.
     •   2048: Georgian bar doc., Order, generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Georgian Bar Paper. This means that the 11th
         flag of the form vector is set to 1, representing a bit value of 2048. Field auftxt.generiert is
         not 0.
         If not customised already, the text is adopted with text type number 2054.
     •   8192: Production      , Order, generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Production Paper. This means that the 9th flag
         of the form vector is set to 1, representing a bit value of 8192. Field auftxt.generiert is not
         0.
         If not customised already, this text is adopted with text type number 2055.
     •   4096: Purchase        , Order, generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form P.O. This means that the 10th flag of the form
         vector is set to 1, representing a bit value of 4096. Field auftxt.generiert is not 0.
         If not customised already, this text is adopted with text type number 2056.
2.       Manually entered text
     •   1: Man. Cutting List, Order, man.generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Manual Cutting List. This means that the 7th
         flag of the form vector is set to 1, representing a bit value of 1. Field auftxt.generiert is 0.

         If not customised already, the text is adopted with text type number 2040.
     •   512: Label        , Order, man.generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Label. This means that the 13th flag of the
         form vector is set to 1, representing a bit value of 512. Field auftxt.generiert is 0.
         By default, this text is adopted with text type number 2042.
     •   1024: Work order       , Order, man.generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Work Order. This means that the 12th flag of
         the form vector is set to 1, representing a bit value of 1024. Field auftxt.generiert is 0.
         If not customised already, the text is adopted with text type number 2043.
     •   2048: Georgian bar doc., Order, man.generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Georgian Bar Paper. This means that the 11th
         flag of the form vector is set to 1, representing a bit value of 2048. Field auftxt.generiert is
         0.
         If not customised already, the text is adopted with text type number 2044.




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                            74
     •   8192: Production      , Order, man.generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form Production Paper. This means that the 9th flag
         of the form vector is set to 1, representing a bit value of 8192. Field auftxt.generiert is 0.

         If not customised already, the text is adopted with text type number 2045.
     •   4096: Purchase        , Order, man.generated
         The text is found in table auftxt with the keys kauf.auftxt and drupos=1 or drupos=2.
         Moreover, it must be allocated to the form P.O. This means that the 10th flag of the form
         vector is set to 1, representing a bit value of 4096. Field auftxt.generiert is 0.
         If not customised already, the text is adopted with text type number 2046.
Additional, order-specific text can be determined by the SP cupmawpaauftxt (see above).
Item-specific text
1.       Created text
     •   1: Man. Cutting List, tnr=0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, they must be allocated to the form Manual Cutting List. This means that
         the 7th flag of the form vector is set to 1, representing a bit value of 1. Field
         auftxt.generiert is not 0.
         If not customised already, this text is adopted with text type number 2020.
     •   512: Label       , tnr=0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form Label. This means that the 13th flag of
         the form vector is set to 1, representing a bit value of 512. Field auftxt.generiert is not 0.
         If not customised already, the text is adopted with text type number 2022.
     •   1024: Work order       , tnr=0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form Work Order. This means that the 12th
         flag of the fom vector is set to 1, representing a bit value of 1024. Field auftxt.generiert is
         not 0.
         If not customised already, the text is adopted with text type number 2023.
     •   2048: Georgian bar doc., tnr=0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form Georgian Bar Paper. This means that
         the 11th flag of the form vector is set to 1, representing a bit value of 2048. Field
         auftxt.generiert is not 0.
         If not customised already, the text is adopted with text type number 2024.
     •   8192: Production      , tnr=0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form Production Paper. This means that the
         9th flag of the form vector is set to 1, representing a bit value of 8192. Field
         auftxt.generiert is not 0.
         If not customised already, this text is adopted with text type number 2025.
     •   4096: Purchase        , tnr=0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form P.O. This means that the 10th flag of



A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                           75
         the form vector is set to 1, representing a bit value of 4096. Field auftxt.generiert is not 0.

         If not customised already, this text is adopted with text type number 2026.
2.       Manually entered text
     •   1: Man. Cutting List, tnr=0, man.generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form Manual Cutting List. This means that
         the 7th flag of the form vector is set to 1, representing a bit value of 1. Field
         auftxt.generiert is 0.
         If not customised already, the text is adopted with text type number 2000.
     •   512: Label       , tnr=0, man.generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form Label. This means that the 13th flag of
         the form vector is set to 1, representing a bit value of 512. Field auftxt.generiert is 0.
         If not customised already, the text is adopted with text type number 2002.
     •   1024: Work order       , tnr=0, man.generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form Work Order. This means that the 12th
         flag of the form vector is set to 1, representing a bit value of 1024. Field auftxt.generiert is
         0.
         If not customised already, the text is adopted with text type number 2003.
     •   2048: Georgian bar doc., tnr=0, man.generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form Georgian Bar Paper. This means that
         the 11th flag of the form vector is set to 1, representing a bit value of 2048. Field
         auftxt.generiert is 0.
         If not customised already, the text is adopted with text type number 2004.
     •   8192: Production       , tnr=0, man.generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form Production Paper. This means that the
         9th flag of the form vector is set to 1, representing a bit value of 8192. Field
         auftxt.generiert is 0.
         If not customised already, the text is adopted with text type number 2005.
     •   4096: Purchase        , tnr=0, man.generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus
         tnr=0. Moreover, it must be allocated to the form P.O. This means that the 10th flag of
         the form vector is set to 1, representing a bit value of 4096. Field auftxt.generiert is 0.
         If not customised already, the text is adopted with text type number 2006.
Additional, item-related text can be determined by the SPs cupmawppauftxt, cupmawpppmptxt,
cupmawppspectxt.
As of AW Enterprise 5 Service Pack 1, the declaration of performance number is also copied as
item text. This is copied with text type number 6100.
Tupel-based text
1.       Created text




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                            76
     •   1: Man. Cutting List, tnr>0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
         tupel number of the current element. Moreover, it must be allocated to the form Manual
         Cutting List. This means that the 7th flag of the form vector is set to 1, representing a bit
         value of 1. Field auftxt.generiert is not 0.
         If not customised already, this text is adopted with text type number 2030.
     •   512: Label        , tnr>0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
         tupel number of the current element. Moreover, it must be allocated to the form Label.
         This means that the 13th flag of the form vector is set to 1, representing a bit value of
         512. Field auftxt.generiert is not 0.
         If not customised already, the text is adopted with text type number 2032.
     •   1024: Work order       , tnr>0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
         tupel number of the current element. Moreover, it must be allocated to the form Work
         Order. This means that the 12th flag of the fom vector is set to 1, representing a bit value
         of 1024. Field auftxt.generiert is not 0.
         If not customised already, the text is adopted with text type number 2033.
     •   2048: Georgian bar doc., tnr>0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
         tupel number of the current element. Moreover, it must be allocated to the form
         Georgian Bar Paper. This means that the 11th flag of the form vector is set to 1,
         representing a bit value of 2048. Field auftxt.generiert is not 0.
         If not customised already, the text is adopted with text type number 2034.
     •   8192: Production       , tnr>0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
         tupel number of the current element. Moreover, it must be allocated to the form
         Production Paper. This means that the 9th flag of the form vector is set to 1, representing
         a bit value of 8192. Field auftxt.generiert is not 0.
         If not customised already, this text is adopted with text type number 2035.
     •   4096: Purchase        , tnr>0, generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
         tupel number of the current element. Moreover, it must be allocated to the form P.O.
         This means that the 10th flag of the form vector is set to 1, representing a bit value of
         4096. Field auftxt.generiert is not 0.
         If not customised already, this text is adopted with text type number 2036.
2.       Manually entered text
     •   1: Man. Cutting List, tnr>0, man.generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
         tupel number of the current element. Moreover, it must be allocated to the form Manual
         Cutting List. This means that the 7th flag of the form vector is set to 1, representing a bit
         value of 1. Field auftxt.generiert is 0.
         If not customised already, the text is adopted with text type number 2010.
     •   512: Label       , tnr>0, man.generated
         The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
         tupel number of the current element. Moreover, it must be allocated to the form Label.
         This means that the 13th flag of the form vector is set to 1, representing a bit value of



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                          77
        512. Field auftxt.generiert is 0.
        If not customised already, the text is adopted with text type number 2012.
    •   1024: Work order       , tnr>0, man.generated
        The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
        tupel number of the current element. Moreover, it must be allocated to the form Work
        Order. This means that the 12th flag of the form vector is set to 1, representing a bit value
        of 1024. Field auftxt.generiert is 0.
        If not customised already, the text is adopted with text type number 2013.
    •   2048: Georgian bar doc., tnr>0, man.generated
        The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr as well as
        the tupel number of the current element. Moreover, it must be allocated to the form
        Georgian Bar Paper. This means that the 11th flag of the form vector is set to 1,
        representing a bit value of 2048. Field auftxt.generiert is 0.
        If not customised already, the text is adopted with text type number 2014.
    •   8192: Production       , tnr>0, man.generated
        The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
        tupel number of the current element. Moreover, it must be allocated to the form
        Production Paper. This means that the 9th flag of the form vector is set to 1, representing
        a bit value of 8192. Field auftxt.generiert is 0.
        If not customized already, the text is adopted with text type number 2015.
    •   4096: Purchase        , tnr>0, man.generated
        The text is found in table auftxt with the keys kpos.poskotxtnr and kpos.arttxtnr plus the
        tupel number of the current element. Moreover, it must be allocated to the form P.O.
        This means that the 10th flag of the form vector is set to 1, representing a bit value of
        4096. Field auftxt.generiert is 0.
        If not customised already, the text is adopted with text type number 2016.
Note:
The standard, tupel-based text is adopted for the elements which are relevant for import (e.g. not
for gas or sealants).
Exception:
For Georgian bars, just one element is imported representing the Georgian bar pattern. The text
for all Georgian bar articles provided in the BOM for this grid will be imported however.
Additional, tupel-based text can be determined by the SPs cupmawptauftxt, cupmawptpmptxt,
cupmawptspectxt.


1.5.6. ALCIB Environment switch
Chapter 1.3.5 „Aktivierung im ALCIB“ already explains that the ALCIB environment switches
ORDERXML, BYTE_VEKTOR and MODUL_KOSTENKALK are analysed for the process. The following
environment switches influence the information in an OrderXML file:
    •   ORDERXML_KOMPLETTESTUECKLISTE
        By default, the BOMis only broken down as fas as this is relevant for production. This
        means that the element's BOM will not be transferred if the element's supply type is
        Stock or Purchasing.
        If this switch is however active and ON, the elements and processing steps below an
        element with supply type Stock or Purchasing will be transferred as well. The adopted




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                         78
       supply types for the sub-elements will match those of the ALCIB BOM in this case.
       Especially for laminated glass this means: If the BOM includes both the process Cutting
       and Laminated glass production, both processing steps will be adopted provided that the
       laminated stocksize shall be produced (see 1.6.6 „Zusammbau- oder Zuschnitts-
       Bearbeitung“).
       Use of terms:
       This description mostly says „Complete BOM import“ if the switch is ON and active. If it is
       inactive, this is called „incomplete BOM“ for short.
       Recommendation for transferring data to ALCIM:
       We recommend to enable this switch for this purpose. For data import into ALCIM we
       also recommend to adopt the entire BOM. This applies especially to the case in which
       „before EDI" supply types can be imported and analysed as well as for the use of the
       function „change of supply type“ in ALCIM.
   •   ORDERXML_IGNORIERE_BEARB_BESTELLKZ0
        If the complete BOM is to be imported, all processing steps will be imported by default
       (except defining processing steps below purchased elements or elements on stock). If this
       switch is active and ON, certain processing steps can be suppressed by setting their
       processing type in the ALCIB BOM to ‚none’.
   •   ORDERXML_IGNORIERE_KPOSGEST

        If rack planning is used in an order, the items will be split by default: There will be a
       separate item in the OrderXML file for every item and rack, showing the rack number and
       the rack type. If this is not used, this switch can be enabled and set to ‚1’. Then, rack
       splitting is not taken into account in the OrderXML file and no rack number is transmitted.
       This switch is available with a patch version of the OrderXML service. Whether the
       customer's version already knows this switch can be checked by means of the version
       code at the bottom of the present OrderXML file: It has to be at least 12.1.3.
   •   ORDERXML_IGNORIERE_POS_BESCHAFFART0
       If this switch is ON and active, items with supply type ‚none’ will not be imported in an
       OrderXML file. They will still be taken into account for the counting of items.
   •   ORDERXML_VERSION
       The OrderXML structure depends on the version. If the receiving system uses an older
       version of this structure, this switch can be used to set the version number of the
       receiving system. Valid version numbers are: "4.0“, "4.1“, "4.2", "5.0". For details please
       refer to chapter 0 "OrderXML-Struktur-Versionierung“.
   •   PMCGHDICKETYP
       Apart from glass, the spacer articles like film and IG spacers will be adopted. These
       articles are used to determine the thickness of the assembled product. In case of cast
       resin, the system searches for an article with article type 340 by default. A PMS type can
       be defined alternatively: If an article is found in the BOM below a cast resin article which
       has been allocated this PMS type in its article master data, this article will be used as the
       spacer article.Here, the default is ptyp=340, too.
       Note: The available PMS types are still defined in PMS. Allocation is done in article master
       data.
   •   PMQCIM_TYPRAHMENFARBTEXT
       IG spacers cannot be allocated Colours because they come in different sizes. To specify
       the colour, an article can be added to the BOM of the spacer which is then allocated the
       colour. This article has to have a certain article type which can be defined by customer by



A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                           79
       means of this switch. (This should not be the spacer's article type however.)
       The first article of this article type in the spacer's BOM serves to specify the colour. The
       color allocated here is adopted as the color number. As the color name, the manually
       entered text in table poszu will be adopted. If this field is blank, the color name is adopted
       from the color code table.
       Alternatively, the spacer colour can be determined by SP.
   •   PMXTRAHMENSP
       A special Bender text can be imported for IG. This is done if the switch PMXTRAHMENSP is
       set to ‚ON’ and is active. The program will search for a text in table pmxtrahmen in this
       case. As a second value, the switch can get the name of a SP. This Sp must exist and must
       have been tested. It must insert the relevant bender text in table pmxtrahmen. The SP
       receives:
       INTEGER:        kauf.auftrnr
       INTEGER:        kauf.aufnr
       SMALLINT:       0 (historically grown parameter)
       SMALLINT:       kpos.posnr
       The expected value is
       INTEGER         but without further application.
   •   PMXAWPOOLSPROSSEN
       Georgian bar patterns can be described on segment level in OrderXML. For this purpose,
       the grid article is usually adopted as an element for which all Georgian bar construction
       information will be available.
       If the grid function is not used in ALCIB, the first Georgian bar article found in table
       kspross will be loaded instead.
       This switch can be used for grouping in this case. It defines that for all Georgian bar
       articles allocated to a certain PMS type, the same article shall be used as the Georgian bar
       element. If the first Georgian bar article in kspross is allocated to a PMS type and if this
       PMS type is defined in the switch's value list, the defined article number is imported as an
       element.
       Note: The available PMS types are still defined in PMS. Allocation is done in article master
       data.
   •   DURCHGSPROSSE
       This switch defines the continuous bar if this information cannot be gathered from the
       Georgian bar type and the bar widths. If the switch is active and ‚0’, the horizontal bar is
       considered to be continuous. Otherwise, the vertical bar is always considered to be
       continuous.
   •   SPROSSENGITTER
       This switch defines that ALCIB automatically adds a Georgian bar pattern article above
       Georgian bars. The Georgian bar pattern article type is 225 and has a sub-element in
       master data (no processing, preferably an element of the type 999).
       This function must be set for purchased Georgian bars.
   •   PMXPOOL_NOAWDFILE
       By default, the ALCIB table field kposp.privat_char is used to determine the AWDesign file
       name . If AWDesign is not used in connection with ALCIB however, this switch can be
       enabled and set to ‚ON’. The name of the AWDesign file will not be determined in this
       case; field <ORDER ITEM - USER EXTENT - PRODUCT - PRODUCT_ELEMENTS - Item BarGrid
       – reference> in the OrderXML file remains blank. The ALCIB table field kposp.privat_char
       can be used for other, customer-related purposes in this case.



A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                          80
   •   MODUL_VERSIEGELUNGSTIEFE
       This switch is only used in connection with the new step logic (MODUL_NEUESTUFEN)
       ausgewertet. If it is set, step records can be imported even for spacer elements. The
       outside dimensions of the spacer element are clearly defined by the geometry, minus the
       step reductions.
       The same applies (alternatively) if the switches MODUL_NEUESTUFEN and
       ISO_FRAME_MODELL are set.
   •   ISO_RAHMEN_MODELL
       This switch is only used in connection with the new step logic (MODUL_NEUESTUFEN)
       ausgewertet. If it is set, step records can be imported even for spacer elements. The
       outside dimensions of the spacer element are clearly defined by the geometry, minus the
       step reductions.
       The same applies (alternatively) if the switches MODUL_NEUESTUFEN and
       MODUL_VERSIEGELUNGSTIEFE are set.
   •   STUFENFORMEL
       This switch must be set if the new step logic is not in use. The first value of the switch
       defines the Step formula. Every glass which is allocated this formula in the BOM
       (aufstrukt.formnr) is considered to be stepped glass.
       If this switch is inactive although the new step logic is not used, a value of 110 is used as a
       "step formula".
   •   DATEI_REF_PFAD
       Orders and order items can be linked with documents. The document references are
       indicated in OrderXML, always complete with the path. The format for such a reference is:

       <DATEI_REF_PFAD>\<kauf.auftrnr>\<kpos.posnr>\<Dateiname> (posnr is 0 if the
       document is auftragsglobal. ).In <DATEI_REF_PFAD>\macro the SN macro files must be
       saved, that are used for the processing types macro (type 1900) and surface macro (type
       1910).
       In <DATEI_REF_PFAD>\motif the SN motif files must be saved, that are used for certain
       surface treatments (types 1200, 1205, 1210, 1215, 1220, and 1225).
   •   PMEHANDLE_GERADE_EP
       If this switch is inactive or if its value is 1, the program will take into account that the
       following BOM structure is reversed for even assembly positions. The sub-elements of
       such an element will be adopted in reverse order. This is standard behaviour as from
       Version 2012.
   •   PMEHANDLE_EP0
       This switch is used to define a fixed assembly position for glass and film layers if no
       assembly position is given in the BOM. Depending on whether this value is even or
       uneven, it will influence e.g. the coating position and the PMEHANDLE_GERADE_EP
       function.
       If the switch is inactive, the assembly position is derived from the parent article. If this has
       an even assembly position, the glass or the film layer is allocated the number 2.
       Otherwise, the assembly position is assumed to be 1.
   •   PMEKOPF_EP
       This switch defines whether the assembly position of the main element is relevant. If this
       switch is not set, the program assumes that the main element is always entered with an
       outside view. In this case, its BOM sub-tree will not be reversed.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                             81
   •   MODUL_DOPPELSCHICHT
       If the switch is ON and active, installation positions at lower levels can also be defined in a
       simple glass hierarchy. The OrderXML service evaluates these for the layers of structure
       and coatings as well as for the rotation of BOM trees and glass layers. The switch is
       evaluated from version ID 12.1.11
   •   KATALOGART
       The catalogue type is transferred by the OrderXML file so that the program knows what
       the shape of this shape number looks like. Valid entries are A+W, Bystronic, or Lisec. If
       this switch is not set, the program will use the A+W shape catalogue.
   •   MODUL_INTERNE_MANDANTENTRENNUNG
       The OrderXML service needs to know whether there is internal site separation because in
       this case,
       - site-specific settings and master data have to be determined based on the order's site
       number.
       - the OrderXML files have to be distributed by site (sub-directories with the order's site
       number)
       - if the site is changed, a cancellation file must be sent to the previous site.
   •   USER_ID        Analysis is already planned for possible, customised extensions. It is part
       of the OrderXML file (part of the version in section A+W-specific extensions of the order)
       and allows to determine the origin of the file.
   •   ORDERXML_NODFUEPROCUREMENT If this switch is active and ON, this means that
       OrderXML shall not take any EDI supply types into account. An element of a processing
       step below a purchased element cannot be produced beforehand or purchased elsewhere
       in this case.
   •   ORDERXML_FOLIENZUSCHNITTSBESCHAFFART If this switch is active and ON, the supply
       type of a laminated glass film shall be changed to „cutting“ if the supply type of the film in
       ALCIB is „Producion“ and if it scheduled for cutting (appropriate AW-Typ or Atyp).
       Especially if the production system is ALCIM, this is sensible only if the film layers are to
       be optimised, and if stockplates have been defined.
   •   ORDERXML_VERSIEGELUNGSDATEN Sealing data can be imported together with the
       airspace information, e.g. a name and a sealing type. The article in the ALCIB BOM
       representing these data can be defined by means of this switch.
       If it set and ‚1’, data for the sealant element (article type 240, element flag 1), which is
       found below the relevant META element, will be searched.
       If it is not set or shows another entry, the data for the META element itself (article type
       240, element flag 2 on the spacer's BOM level or below, and preferably with the same
       assembly position) will be searched.
   •   AWC_ANGEBOT_DEF_TERMINNo delivery date is required for quotations. In this case, the
       current date plus 14 days is transferred to A+W Capacity as the default date. The offset of
       14 days prevents a general date shift for quotations. If this value does not match, you can
       use this switch to specify a different value in days.


Recommendation:        The following switches should also be set for ALCIB order entry:
   •   ISO_RAHMEN_MODELL: ALCIB always creates a shape record for spacers. This serves to
       determine its width and height.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                             82
    •

        MODUL_NEUESTUFEN: With this setting, the step reductions can be adopted for the
        information of the actually stepped elements. Without this logic, the step reductions are
        always adopted for the main element while the stepped elements are only marked.


1.5.7. Item split
If the rack planning module is used in ALCIB, it can happen that an item is split onto several racks
(several entries for the item in table kposgest).
In this case, the item is split in the OrderXML file. This means that the item is transferred several
times: A separate transfer is made for every rack, not with the item quantity but with the quantity
scheduled for the rack.
The item reference shows that the item has been split.
Item reference
The item reference can be used as a unique item reference in ALCIB. It should always be stated in
reports that are made to ALCIB about the item. It can be found in the element „ReferenceID“.




The item reference is created as follows:
The first three digits are the internal ALCIB item number which is always unique (kpos.posnr).
The last three digits are a counter for the rack. Without rack planning, or if the item is loaded
completely onto one rack, the number is always „001“.
Example:
The item with internal item number 3 was distributed to the racks 261550 and 261551. This way,
the item is imported twice:

1. with item reference 003001
2. with item reference 003002.
For rack details please refer to the element Rack


Disable item split
If splitting is irrelevant for the transfer however and the reading system needs no rack
information, item splitting can be disabled. Enable the ALCIB switch
ORDERXML_IGNORIERE_KPOSGEST and set it to '1'. There will be just one record in the OrderXML
file for every order item; there will be no rack element.This setting is recommended in connection



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                          83
with AWProduction for ALCIB rack data which are not required. Scheduling will be faster because
the positions do not have to be scheduled several times.
This switch is available with a patch version of the OrderXML service. Whether the customer's
version already knows this switch can be checked by means of the version code at the bottom of
the present OrderXML file: It has to be at least 12.1.3.


1.5.8. Cancellation
This chapter describes the process in case of a cancellation due to
    •   Order cancellation
    •   Item cancellation
    •   Change of plant for an order

Order cancellation

When an order is cancelled in ALCIB, an OrderXML file is created. Its structure reflects the order
information available at the time of the cancellation. The fact that the whole order has been
cancelled is marked by the detail Ordering type for which the entry is „Cancel“. This information
is found in the A+W-specific extensions for the order:




Cancellation of order without previous transfer
If an order is cancelled which has not been transferred yet, the OrderXML service takes care of
this. The data noted in table ottranssav show whether it has been transferred yet. If there is no
entry in this table for this order, the order has not been transferred yet. No OrderXML file will be
created for the cancellation in this case.
The corresponding record in transfer table ottransfer is marked with status 471. This status is no
actual error status but serves to point out that OrderXML transfer had been planned for this order
but was eventually unnecessary.

Item cancellation

Cancelled items do not appear in the OrderXML file.
The clarity of the item references allows the reading program to compare them with existing data.
If the original data include an item with a reference ID which does no longer occur in the present
OrderXML, this item is assumed to have been cancelled.
The item reference is part of the A+W-specific extensions for the corresponding item:




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                         84
Change of plant for an order

In case of internal site separation , the allocated site can be changed in the ALCIB order header.
The OrderXML service recognises the change of plant based on the data in table ottranssav
because these show the plant which received the order last time.
If a change of plant is detected, two OrderXML files will be created:
    1. To the plant which received the order originally
       A cancellation of order is transferred in this case. This means, the information Ordering
       type for the order shows the entry "Cancel“.
    2. A new transfer is made to the present, i.e. new plant. This file has the same contents as
       the cancellation file, only the information Ordering type shows the entry „Produce“ for
       this order.


1.5.9. References in reports
The information of the OrderXML files also include references that can be used to retrieve items,
elements, or processing steps in ALCIB.
This information may be useful for the project team / service when it comes to run manual
searches or analyses.
They are most useful however for specifying report interfaces. The references must be available in
this case.
The information is:
Order number
All reports with an order reference must include the order number. It is found in field ORDER_ID
in the order header's order information.




The order number above matches the external order number in ALCIB.
Item reference




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                          85
Reports referring to a certain item must include the item reference in addition to the order
number. It is found in field ReferenceID in the A+W-specific extensions of the corresponding item.




The item reference consists of two values. The first three digits are the actually relevant ones
because the match the internal item number in ALCIB which is always clear. The last three digits
are a counter which show that an item has been split because it was loaded onto serveral racks.
Element reference
Reports referring to a certain element of an item BOM must show the element reference in
addition to the order number. It is found in field bomID for the corresponding product (element).




The item reference consists of two values.
    •   The first three digits are the internal (unique) item number in ALCIB .
    •   The next three digits are a counter and show that the item has been split and is to be
        loaded onto several racks.
    •   The last four digits are the tupel number, i.e. the element ID in the ALCIM BOM.
Processing reference
Reports on processing steps must include the order number, item reference, and processing
reference. The processing reference is found in field reference for the corresponding processing
step.




The processing reference matches the processing step's tupel number in the ALCIB BOM.


1.5.10.         OrderXML files for purchase orders
OrderXML files for purchase orders can be created as an integrated special solution.

Requirements

The entry in transfer table ottransfer is made after P.O. entry. It depends on the supplier. In the
supplier's partner master data, „OrderXML“ must be defined as the EDI type.



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                            86
The entry in the transfer table therfore does not depend on the switch ORDERXML.

Differences Compared with Orders/Quotations

Purchase orders are identified in the transfer tables by document type (field vorgang) 2.
The main changes in the OrderXML file only apply to the following information:
Internal customer number for purchase orders
In purchase orders, kauf.kunr gets the number of the supplier for which the P.O. is intended. This
information is not very useful for the supplier however. The customer which is internally used for
finding the relevant data is therefore determined for purchase orders based on
xhaus.kunr:
The site entering the P.O. is assumed to be the customer for this supplier. This is why the
customer number is selected by kauf.hausnr (=hnr) in table xhaus.
This field must therefore be maintained to be able to use this function.
If the customer number cannot be determined, all customer-relevant information is determined
by means of kauf.orgkunr.

An OrderXML file will be created in any case. The P.O. will remain in the transfer table for
information purposes, with error status 440. This status means that the customer data in the
OrderXML file need to be checked.
The customer number determined in this way influences the following details in the OrderXML
file:
ORDER - USER_DEFINED_EXTENSIONS - UDXAWORDERINFOS - CustomerInfos –
CustomerLanguage,
if the value is determined by SP. The SP receives the customer number. For orders and
quotations, this is always kauf.kunr and for purchase orders, the customer number which is
determined as descriebed above.
ORDER - ORDER_HEADER - ORDER_INFO - ORDER_PARTIES - BUYER_PARTY
The information below this node is determined for purchase orders from the partner master data
defined for the customer number in question. Also see paragraph „Buyer's address“.
ORDER - ORDER_HEADER - ORDER_INFO - ORDER_PARTIES - SHIPMENT_PARTIES -
DELIVERY_PARTY - PARTY – ADDRESS
Also see the paragraph on „Shipping address“.
Buyer's address (BUYER_PARTY)
The customer number which appears in field ORDER - ORDER_HEADER - ORDER_INFO -
ORDER_PARTIES - BUYER_PARTY – PARTY – PARTY_ID is the external customer number configured
for the supplier. In case of internal site separation, the external customer number is maintained
by site in a separate table called mpmdzu; otherwise directly in the supplier's partner master
data.
As for the address data, the program checks if a standard address has been defined (mp.stdadr) in
partner master data for the internal customer number (determined as described above): If so, the
corresponding address mastere data will be determined; otherwise, the information from partner
master data will be used.



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                       87
Shipping address (DELIVERY_PARTY)
For drop shipments, the address is determined from adress master data if kauf._ladrnr shows an
entry. This is done by means of the internal customer number as described above.
If no shipping address number is defined, the shipping address will match customer data
(BUYER_PARTY).
Supplier address (SUPPLIER_PARTY)
The supplier address is only filled for purchase orders. The supplier ID matches the supplier
number (kauf.kunr). The address information is taken from the „original“ fields of the document
(kauf.orgplz, kauf.orgort, ...).
Bill of materials (BOM)
The supply type of the main element of a purchase order is usually „P.O.“. For orders/quotations,
this supply type generally means that the BOM below is irrelevant for production. The supplier
however needs the BOM of the ordered element. This is why the whole BOM will always be
transferrred for purchase orders!
Information on purchased elements
This is the information below ORDER ITEM - USER EXTENT - PRODUCT - PURCHASE_INFO.

If an element's supply type is „P.O.“, this provides information on the supplier like his address but
also the article number the supplier uses for the ordered product (if defined in master data).
The same applies to purchase orders: Provided that the main element keeps the supply type
"P.O.“, this is information on the supplier the P.O. is directed to. The data for the main element
are determined by means of kauf.kunr.
File name
The name of the OrderXML file for purchase orders has the same structure as that of an order or
quotation (see chapter 0 „Dateiname“).
Purchase orders are identified by the number "2“ after the code "e“.
Example: Order900302i0e2t2008-06-12 12-08-52.xml
Storage directory
Below the directory defined for the OrderXML transfer, a "purchase" directory must be created.
All OrderXML files for purchase orders will be saved in this directory.


1.5.11.         OrderXML transfer just for production cost calculation
This transfer type is meant for transfer to ALCIM with ALCIM Capacity. It allows real-time
calculation of production costs even if the order is not released for production.
Prerequisite is that production cost calculation is active. The switch MODUL_KOSTENKALK must
be set to ‚1’ or ‚3’ for this purpose.
The process in ALCIB
When an order is entered in ALCIB, the OrderXML service is ordered first to create an OrderXML
file based on which the production system shall calculation the production costs.

The order is then processed by the ALCIB background processes. After that, the order can be



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                           88
released for production: This is either done automatically by the background processes or
manually by means of the ALCIB release pool.

This release actually instructs the OrderXML service to create the OrderXML file for order transfer.
Processing by the OrderXML service
The structure of the OrderXML file created for cost calculation matches that of the order transfer.
A code for the production system is set in field <ORDER - USER_DEFINED_EXTENSIONS -
UDXAWORDERINFOS - Ordering – type>. This tells the production system that the transfer was
made just for cost calculation purposes; it must prevent however that the order is released for
production.
If the OrderXML service fines the entry for cost calculation in the transfer table and if the entry for
the order transfer is already available at that point, only the file for the order transfer will be
created. The productions system should recalculate (update) the costs whenever an order is
transferred. This prevents that cost calculation is done unnecessarily often.

Transfer of quotations for production cost calculation (AWDesk #407684)

Quotation items can be entered in AWE without quantities in order to be able to offer a customer
alternative items.
Since cost determination in AWP for quotations with contained zero quantities runs on an error
("...Incomplete parts data: Missing quantity [1030][XDD10111,reason=404]"), version 6 sets zero
quantities in quotation items to calculation quantity 1 by the OrderXML service.


1.5.12.         Items with supply type "none" in the OrderXML interface
The system now offers a configuration option with the result that items with supply type 'none'
do not appear in OrderXML, and are therefore not transferred to the production system. This
option is useful for marking items which have informative or commercial character only by supply
type 'none'.
The items will not be transferred but this does not mean that they will not be considered for the
transfer. They will still be included in the item count (transfer in field LINE_ITEM_ID of the
OrderXML file). From an order consisting of three items in which the second item has got supply
type 'none', item 3 will be transferred marked 3; the item marked 2 would be missing.
If an order consists only of items with supply type 'none', no OrderXML will be created. The order
gets an error code and - if configured - a message will be issued with the code "OrderXML Error
458".
This function can be configured. If the supply type 'none' is not used in this way, the
corresponding items can still be transferred. They will be transferred with supply type '0' so that
the production system can decide how to handle these items.
Items with supply type 'none' can be suppressed by enabling the new switch
ORDERXML_IGNORIERE_POS_BESCHAFFART0 and setting it to 'ON'.
The switch will not be analysed if the OrderXML file is required for direct data import from PMS to
ALCIM for transmission to ShapingNesting, i.e. if the switch PMQCIMIN_SNTRANSFER has been
set; in this constellation, items must be identical in PMS and OrderXML.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                          89
Items with the supply type "none" will get no status. A late order change is always possible even if
all production-relevant items have been completed. In this case, it can be determined on a
customer-specific basis that no further transfer to the production system shall take place. Also see
chapter 0 „Übergabe verhindern“.


1.5.13.         Ordered glass
The ProcPostThermal processings (and generally the processings after the defining processing) are
only transferred in the OrderXML file since AWDesk #460675 when the parent part is ordered. It is
necessary to transfer these processings so that in the case of a turned ordering sheet, the
processings are also turned.
However, this change may have undesirable effects if customers work with bills of material where
a processed glass does not yet explicitly exist above a glass with defining processing. Processings
that take place after the defining processing are then assigned to the ordered glass in the
OrderXML file. In A+W Production, it then looks as if processing still has to take place after the
ordered glass has been delivered.
The correct way to prevent the undesired effect is to adjust the master BOMs. However, if it is not
possible to change the master BOMs, the effect can be prevented by setting the environment
variable ORDERXML_PROCPOSTDEF_LEVELDOWN=ON (site-specific). If the variable is active, for
an ordered parent part, processing that takes place after the defining processing is transferred in
the OrderXML file on the glass below the ordered glass (e.g. on the float below a tempered safety
glass).
It is important that a customer who uses this logic may under no circumstances subsequently
change the procurement type of the ordered glass to "Production" in A+W Production.
See also AWDesk #461345.


1.5.14.         End customer information
This development should ensure that particular information about the end customer or about the
distributors can be transferred to the production system of the production site.
This data is:
• Name of the end customer
• Delivery address of the end customer
• End customer reference (end customer's order or PO number)
• End customer's position reference
• Commission text
• End customer's requested date
• Delivery route in trade site
• Desired packaging type
• Desired delivery type
• Direct delivery flag
• Name and address of the distributor
• Order number of the distributor
• PO number of the distributor
The adjustment of the OrderXML is implemented in Version 5.5 using two stored procedures.It is
necessary to activate the two SPs with the 'INFOTOXML' tool. The set 7 described under 3. must
be defined as order header level.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                        90
SP cupmawpaktext1

This SP is responsible for the information that appears in the production database in the field
pool_auftrag.sondertext1. In the OrderXML this information is transferred in the
USER_DEFINED_EXTENSIONS .. .<OrderNotes><ADVICE number=1> area.
The string is composed of the following parts:
• Start value ‚t:‘
• The end customer's delivery date with a length of 10 characters, e.g.: '01/01/1899'
(kaufprvfld.dateval1 und setid = 7)
• ‚-‘
• Kauf.orgname with 19 characters.
• Kauf.exaufnr with 20 characters
cupmawpaktext2
This SP is responsible for the information that appears in the production database in the field
pool_auftrag.sondertext2. In the OrderXML this value is found under USER_DEFINED_EXTENSIONS
. .<OrderNotes><ADVICE number=2>.
The string is composed of the following parts:
• Start value type of delivery: ‚Trl‘ for direct delivery kauf.drkliefkz > 0 otherwise ‚Trf‘
• Order number of the distributor 6 characters
• ‚-‘
• Route to the end customer of the distributor 3 characters
• ‚-‘
• 14 empty spaces not specified
• ‚-‘
• Customer name of the branch office or customer name from distributor for EDI
• PO number of the distributor


#345567: Transfer production-relevant information OrderXML + AWP (Feature)
With the adjustments of this case, the previous SP logic from case #334558 is replaced. The ERP
data required in A+W Production is now transferred between the systems via special OrderXML
files.
ALENV ORDERXML_VERSION must have at least the value "5.4".
The current version of the A+W Enterprise 6 OrderXML Service must be installed.
In A+W Enterprise the configurable KAUF fields for setid = 7 must be created. These will later
contain the end customer data, among other things.
For details about the expansions of the OrderXML interface, the database expansion (AW
Production) and the fine planning properties, see the following document:
The environment variable ORDERXML_ENDCUSTOMER_DETAILS must be active.




1.6. Internal site separation
1.6.1. Company change in the order after transfer to AWP
If in an already-released order a company change is desired, then you can enter a new company
number via the menu or with <F5> from the "Input" field in the transaction header. If the




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                         91
transaction is already locked (local correction), a company change is no longer possible. After the
new company number has been taken over into the order header, the user can decide whether
the new supply types according to the stored master data should be pulled into the new
company. A new route is searched for and the order is re-calculated.
The company change always counts as production-relevant and if the transaction was already
released in Company 1, the release in the company is assumed as a "must." When saving, first a
query is sent to A+W Production whether a cancellation in Company 1 would still be possible. If
the cancellation query is accepted, then all other data in Company 1 is cancelled (dispatch, stock,
purchase orders) and the order is released in Company 2. If the cancellation is rejected, then the
order cannot be saved in the form. The user can contact employees in the production area and
then eliminate the possible blockage reasons on this side and make the change again. If this is not
possible, he must discard the change. We recommend executing the company change quickly and
not in connection with other changes since the lock from production can come at the time of the
change and then the changes must be discarded completely.
A company change in connection with cancellation to A+W Production is also logged in the order
status (kaufstat). If the purchase orders are thus also canceled. you can see this information in the
change log.

Export Service

In the config tool of the export service, several databases can now be configured. With internal
site separation, the DB configuration can be done subsite-precisely if needed. Polling interval and
the maximum number of transmission attempts are specified across DBs.
In the service, after expiration of the polling interval for all configured and active databases, it is
checked whether trigger records are present in the table EXPORTINFO. Existing records are
worked through. The databases are checked one after another, the sequence of the checking is
arbitrary.
With subsite-precise configuration of a DB connection, only the exportinfo records are processed
that contain the configured subsite in EXPORTINFO.HAUSNR.
Export Service: New interface "CANCELORDER"
Order cancellations are transferred to AWP using this interface.
The interface records in table EXPORTINFO are generated by the back end.
Records with the new interface are preferably processed by the export service. Attention! For
this, the polling interval in the config tool must be configured so that it is appropriately short.
The export services calls a PPS Webservice method, which executes the order cancellation in
AWP. The return value of the method indicates whether or not the order cancellation was
executed successfully in AWP:
    •   Return value > 0 indicates that the cancellation was executed successfully.
    •   The value -1 indicates that the action could not currently be executed due to content
        problems (e.g. OrderXML is being imported now).
    •   The value -2 indicates that the order was neither found in the database nor as OrderXML.
    •   The value -3 indicates that there are technical problems (e.g. DB connection problem,
        program error).




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                           92
Successfully processed records are transferred to the table EXPORTINFOOK, in the process the
long value from EXPORTINFO.IZEIT (insert-time) is transferred after EXPORTINFOOK.LONGWERT1,
so that records for the same order can be distinguished using the time stamp.
Records that encounter an error stop with status < 0 in EXPORTINFO. In EXPORTINFO.FEHLERTEXT
the error that occurred is described and the error code specified.
In the PPS Webservice, the new method for order cancellation is available starting with Version
13.04.1330.

OrderXML Service

In the config tool of the OrderXML Service, you can maintain a site number. Effective
immediately, it is also evaluated by the OrderXML service, so that only such transactions from the
OTTRANSFER table are read that fit the configured site number. If in the configuration the site
number was assigned the value 0, as previously, all data records will be processed.
The entries in the table OTTRANSSAV will serve only research purposes in the future. The previous
logic of sending a special OrderXML to the previous sites in case of a site change was deactivated
since it was causing problems.


1.7. A+W Processing Types
1.7.1. UV protection (awtyp 1650)
In AWE, a processing UV protection (awtyp 1650) may only be assigned to precisely one edge. In
the OrderXML file, this processing is also created for just one edge, for the OrderXML structure
permits the transfer of only one edge for the A+W processing type 1650. An edge vector cannot
be transferred here.
This creates a general problem with the OrderXML transfer of UV protection for shapes for which
the AWE edge quantity is smaller than the corresponding CAD segment quantity for the shape
(e.gg. shape 75 with 1 AWE edge but 8 CAD segments). With such a constellation, previously only
the UV protection for the first segment reached the OrderXML file.
With AWDesk #453699, a logic was built in that should prevent an incorrect production if in AWE
a processing UV protection was accidentally assigned to several edges. It is detected in the
OrderXML Service if a processing UV protection applies for several CAD segments simultaneously.
In this case, the OrderXML file creation is prevented. The consequence of this logic is that the
shape described above with deviations of edge and segment quantities can encounter an error in
the OrderXML Service if an AWE edge with UV protection is mapped to several CAD segments.
There is no quick solution for transferring the correct data in the OrderXML for this case.
Therefore, it was decided that in this special case, that for a shape on which an AWE edge with UV
protection is mapped to several CAD segments the OrderXML file will be written although there is
no complete information for the UV protection in the OrderXML file. Only the first segment is
transferred for the UV protection.
A corresponding error message is issued in the OrderXML Service log.
It is clear that with such an item there is an incorrect production if production is done based on
the data in the OrderXML file. The item must be corrected manually before production.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                           93
If the item is attached to a SN file attached in AWE, the SN file contains the correct information
about the UV protection.
See AWDesk #454284.



1.7.2. Configure/non-configured processing parameters
For the numeric processing parameters that are transferred in the OrderXML file, it must be
possible to distinguish whether or not an individual parameter is configured.
The parameter values (transaction data) are stored in the table poszu. Here, however, there is no
configured flag. Therefore, for the generation of the OrderXML file, there is a reliance on the
master data table artvermass. In artvermass, the type of configuration is stored for each
parameter of a processing (no/variable/fixed/mandatory):
    -   for the positioning dimensions poszu.mass1-4 in artvermass.getloc1-4
    -   for the positioning parameters poszu.dmess1-10 in artvermass.getval1-10
According to the configuration type, a "false" is transferred in the respective "isSpecified"
property of the element if the configuration type in artvermass is "no". In all other cases, "true" is
transferred.
This logic can cause problems if precisely between the entry of an order with A+W processing and
the transfer of the order to production (generation of the OrderXML file) the parameter
configuration for A+W processings present in the order in artvermass is changed from "no" to
"variable/fixed/mandatory" or from "variable/fixed/mandatory" to "no".
Since in A+W Enterprise there is currently no possibility to save the configuration type in the
transaction data, the logic will be retained this way. Previously, customers have not reported any
problems with this.
See also AWDesk #456954.


1.8. AWE item types
1.8.1. Other articles (atyp 999)
The atyp 999 is intended for price-relevant articles that should not reach production (or
purchasing). Articles with atyp 999 are not written to the OrderXML file.
See AWDesk #454469.


1.9. Extended Workbench (EWB)
By activating the environment variable MODUL_ORDERED_PROCESSING (ON), the logic of the
extended workbench (EWB) is switched on in AWE. The activation influences the generation of
the OrderXML BOM in the OrderXML service.
Meta elements with supply type "PO" are not transferred to the OrderXML file with active
extended workbench if there is an ordered processing below the meta element. (For general
treatment of meta elements, see chapter "Meta elements in the AWE BOM").



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                           94
An ordered accessory part (non-glass part) is not transferred in the OrderXML file with active
extended workbench if this accessory part is in the BOM under a meta-part and if an ordered
processing is present on the same BOM level.
The following item types are permissible for the meta parts:
- atypen that define processings (e.g. 589 "Coating", 540 "Foiling", 592 "Masking")
- atyp 270 "Edge protection" (meta for masking)
The following item types apply as accessory parts under metas:
- atyp 800 "Accessories"
- atyp 300 "Foils"
- atyp 320"Coating" if the superordinate meta part is atyp 589 "Coating"
For ordered accessory parts that are not transferred in the OrderXML file, for which, however,
there is an ordered processing on the same BOM level, a special logic is run through later with the
reporting of the scheduled order from AWP in the ERP Webservice; it ensures that PO records are
generated for AWE for ordered accessory parts. In particular here:
-the purchasing date of the ordered part is taken over without AWP reference from the ordered
processing on the same BOM level
-the quantity of the ordered part is taken over without AWP reference from the AWE item
(kpos.menge)
In the standard logic, ordered accessory parts (non-glass parts, item types see above) are
tranferred in the OrderXML file under a meta-part.
In contrast to the ordered or produced processings, which are assigned to the glass to be
processed in the OrderXML file, an ordered non-glass part is placed next to the glass to be
processed, i.e. assigned to the glass to which the glass to be processed is also assigned.


Notes about configurations in AWP
So that processing parameters for all processings are reported back (not just for processings of
ordered parts as in the default setting), the switch
ITEMS4ALCIM_SETTINGS/SUPPRESS_PROCESSING_PARAMETERS must be assigned the value 2.
CAUTION: If accessories (atyp 800) are ordered, the part type of the accessory item must be set to
0 (non-glass item) in AWP.
See also AWDesk #451780


1.10.           Interesting facts
This chapter is a collection of information. It should be completed by service and project teams to
provide answers to frequently asked questions.


1.10.1.         Error reports in the Windows service log
System.Web.Services.Protocols.SoapException

The exact wording is: System.Web.Services.Protocols.SoapException: Server was unable to
process request. ---> Albwir.Basis.Database.AWDatabaseException: Closing exception database
type: Informix ---> System.EntryPointNotFoundException: Unable to find an entry point named
'IFMX_CleanConnForPooling' in DLL 'iclit09b.dll'. [...]



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                          95
If this message appears at the start of the Windows service log file, a DLL is surely missing from
the GAC, or it is incorrect. The Informix driver must be installed in the described way so that the
correct DLL can be copied. This requires the following steps:
    1. When the Client-SDK is installed, the "Custom" installation should be chosen for safety's
       sake. When choosing the packages please make sure that the „Informix .NET driver“ is
       installed as well. If the Client-SDK has been installed already, the installation can be
       repeated via Windows system control  Software  Informix Client-SDK 
       "Amend/repair“. This means that the uninstallation/installation process is usually not
       required.
    2. Next, open two Windows Explorers (mandatory).
    3. In the first Windows Explorer, go to directory C:\Windows\Assembly (this is the so-called
       „GAC“ (Global Assembly Cache)).
    4. In the second Windows Explorer, go to directory C:\Program Files\IBM\Informix\Client-
       SDK\bin,
    5. Use Drag&Drop to move the file „IBM.Data.Informix.dll“ from the second Windows
       Explorer to the „GAC“ in the first Windows Explorer.
The recommended version for the Informix Client SDK is 3.50 TC9.


1.10.2.            No orders are processed
If the orders in table ottransfer are not processed although the OrderXML service has been
started, you should first check the service log. Set the log depth in the configuration file to at least
1 for this purpose (please only temporarily for this stage of the search as recording takes time).
The configuration file is found in the installation directory of the OrderXML service.
After changing the log depth, reboot the Windows service.
If the log provides no details, i.e. if it reports no error, the records in table ottransfer should be
checked again. If there are redundant records for the keys auftrnr, vorgang, and filltime,
processing is impossible. The service ID should be checked as well. Has this field been used to
reserve the order for another service which has not been started?


1.10.3.            List of form vectors
The following list refers to the form vectors in table auftxt in ALCIB. It shows which bits must be
set for the individual forms in a byte vector configuration.
This information can be useful if text shall be determined by SP from table auftxt. No matter
which SP is used: The SP must return only text which is actually relevant for the transfer. The SP
can decide this based on the relevant bits in the form vector.


         Form                                              Bit              Byte vector
         Manual cutting list / reminder                    7                 00000010000000
         Credit note                                       6                 00000100000000
         Invoice                                           5                 00001000000000
         Cancellation                                      4                 00010000000000



A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                              96
         Form                                              Bit              Byte vector
         Order                                             3                 00100000000000
         Quotation                                         2                 01000000000000
         Works order                                       12                00000000000100
         Bars                                              11                00000000001000
         Order                                             10                00000000010000
         Production papers                                 9                 00000000100000
         Delivery Note                                     8                 00000001000000



1.10.4.          Invalid special characters
The following special characters must not appear in text and names. This needs to be taken into
account for ALCIB master data and at order entry:
         Character                                       Can be represented by
         <                                               &lt;
         >                                               &gt;
         &                                               &amp;
         “                                               &quot;
         ’                                               &apos;
         Line break                                      &#xD;&#xA



1.10.5.          Manual transfer of orders
Orders should not be transferred manually by adding a record in table ottransfer.
This is principally possible and if the clarity of the keys auftrnr, vorgang, filltime is obeyed, the
records will even be processed. Correct transfer of an order includes much more however. It
provides the service with additional, necessary information.
This means that if orders are sometimes transferred manually and sometimes correctly after a
change of order, the information in the resulting OrderXML files will not always match.


1.10.6.          Processing step assembly or cutting
If the Whole BOM is Transferred

If the system is configured to import the complete BOM (switch
ORDERXML_KOMPLETTESTUECKLISTE), the import of processing steps for products which can be
assembled and cut afterwards, requires special attention.




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                             97
The above graphics show the BOM structure of a laminated sheet which can be both produced
and cut.
Import of the processing steps „Laminating“ and „Laminated cutting“ depends on the supply type
of the stocksize (in this case, article number 403210):
    •   If the supply type of this article is „Stock“, all elements of this article will be imported
        according to the setting. Import of the processing step „Laminating“ can cause problems
        in some of the target systems however. As the stocksize's supply type makes it clear that
        laminating is not required, this processing step will be filtered by the OrderXML service; it
        will not be included in the OrderXML file. „Laminated cutting“ is imported as the first
        processing step.
    •   If the stocksize's supply type is „Production“, „Laminating“ is imported as the first
        processing step for laminated glass. „Laminated cutting“ is imported as the second
        processing step. In this case it is up to the production system to decide whether the sheet
        shall be cut despite the production process.

If imported by ALCIM

If the laminated sheet described in this example is produced, both processing steps - „Laminating“
and „Laminated cutting“ - will be imported. If the sheet does not have to be cut because of the
production process, this processing step can be removed by means of the BOM configurator. The
following pictures show an example:




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                          98
If BOMs are Transferred up to the Stored or Purchased Elements

Even if the system is configured to import not the whole bill of material (switch
ORDERXML_KOMPLETTESTUECKLISTE is not set), import of the processing steps for products
which are assembled and cut afterwards, requires special attention.




A+W Software GmbH      EN-CONFIG-A+W EnterpriseProductionInterface.docx                  99
The above graphics show the BOM structure of a laminated sheet which can be both produced
and cut.
Import of the processing steps „Laminating“ and „Laminated cutting“ depends on the supply type
of the stocksize (in this case, article number 403210):
If the supply type of this article is Stock, the laminated sheet is only cut. Only the laminated glass
product with processing step "Laminated cutting“ is imported. The BOM below the stocksize is cut
off.
If the supply type of this articl is Production, the lamianted glass product is imported together
with the BOM below the stocksize. The only processing step to be imported for laminated glass is
laminating while laminated glass cutting will be ignored.


1.10.7.         If the database is inaccessible
A temporary loss of connection with the ALCIB database will be detected by the
OrderXML service; the database connection will be re-initialized before the next
order search.
Since every re-initialising of the database requires memory however, the re-initialising attempts
are limited now in case of a lengthy loss of connection:
    •   If database initialisation fails, the service will wait two minutes before attempting
        initialisation again.
    •   If initialisation fails five times in a row, the service is terminated and troubleshooting must
        be rebooted manually.
Automatic rebooting
If this error occurs, the service stops so that the service configuration can be used for rebooting
after an error:
Start the service manager and use the right mouse key to select the OrderXML service. A context
menu appears from which you select the menu item Properties.
On tab General in this window, the start type must be set to „Automatic“.
Now select the tab Restore.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                         100
Now define that the service shall be rebooted in case of an error, and the interval (in minutes).
Checkbox „Trigger actions in case of interruptions due to errors“ must be ticked.
Please note that the settings have to be made again after reinstallation.
If the connection cannot be established due to locked system tables
In special cases, the database may be accessible while the system tables are locked. This may be
the case if statistics are updated or if a backup is run. In this case, there is probably no error. Since
such a process might take longer, the time until the service is closed has been extended to 2 ½
hours. In the meantime, the program will try now and again to establish the connection with the
database. Even if all this fails, the program assumes that there is an error, and the service stops.


1.10.8.          Glass door systems and shape data
In connection with the new step recording, it is assumed that all parts of a parts list are based on
a reference geometry. Deviating geometries are completed with appropriate step deductions.
If the field refflag in the table kmodparam is set to '1' for the corresponding geometry, it is
possible to see that the new step recording is present.
Different for whole glass systems (item type 400). Here each part is described individually. The
geometries depend on one another. For this reason, the field refflag is not considered for this
type. The prerequisite is that a corresponding patch version (version identifier 12.1.13) of the
OrderXML service is installed. (#314985).


1.10.9.          Weight of main and sub parts
ATTENTION: Exchange articles will NOT be considered!




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                          101
In the standard configuration, the attribute "weight" is filled for each <PRODUCT> element in the
OrderXML file. This means that the weight is determined for each part and transferred to
"weight". If no weight can be determined, a 0 is transferred to "weight".
The weight of a header is calculated from the movement data (KPOS.GEWICHT / KPOS.MENGE).
For a sub part, the weight is calculated from the master data (ARTIKEL.GEW * surface (based on
the circumscribing rectangle)). This means that glass replacement in the sub part is not taken into
account for sub parts. The transferred weight of the sub part with the glass replacement does not
change in the transfer.
During import the weights are written to POOL_TEILE.GEWICHT_RECHTECK.
The attribute "WeightShape" for <PRODUCT> elements is currently never transferred to the
OrderXML file.
Adjustment AWDesk #422884:
For <PRODUCT> elements, the attribute "weight" will continue to be filled as previously. That
means for header parts, it contains the shape weight and for subparts, the weight of the
surrounding rectangle. If a weight = 0 is determined, the attribute is transferred nevertheless.
If the content OrderXML version >= 5.5.0002 (switch ORDERXML_VERSION = "5.5"), if necessary
the attributes "weightShape" and "weightRectangular" are transferred.
"weightShape" is only transferred for header parts and if their weight is > 0.
"weightRectangular" is only transferred for subparts and if their weight is > 0.

Weight calculation during import

In the OrderXML file, the attributes "weight" and/or "WeightShape" can be transferred per part.
The AWP interprets "weight" as an approximate weight (weight of the circumscribing rectangle)
and "WeightShape" as a weight for which the shape number of the part was taken into account.
If the weights are transferred in the OrderXML file, these have priority and the AWP does not
calculate anything itself (or it only calculates to check). However, if "WeightShape" has not been
transferred, then the AWP starts its own calculation. For assembled parts, the sum of the weights
of the subparts is selected here. For single glass, the surface (obtained from "SurfaceAreaShape"
in the OrderXML file or if not available from GetFrm32.dll) is multiplied by the thickness and
standard density of glass (2.5g/cm³).
The weights can then be found in the Alcim DB at the following location:
pool_teile.gewicht_rechteck (weight of the circumscribing rectangle)
pool_teile.gewicht_form (actual weight of the form)
Note: spacers, muntins, foils etc. are not charged. No distinction is made between glass articles.
All have the assumed density of 2.5g/cm³.




1.11.           Other documents
\\jupiter\DOKU_DocuWare\Interfaces\OrderXml\AusAlcib\2012 offers the following documents.
    1. DokuInfosOrderXMLAlcib.txt
       Describes for every filled-in OrderXML node how the information is gathered from ALCIB.



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                         102
        This is a genuine text file which can be opened by any editor. You should however choose
        an editor that does not add line feeds, no matter how long the lines are.

        This file can be reproduced on site any time. In the configuration file of the Windows
        service, set the trace level of the switch Albwir.Alcib.AlOrderXMLService to „Verbose“.
        We recommend to make sure that there is just one order for OrderXML creation and that
        this order includes just one item.
        The OrderXML log file which is created as a result now includes several lines marked by
        „Verbose“ all of which describe the OrderXML output.
    2. Inst_ALOrderXMLService_12_1.doc
       This document describes the elements to be installed and configured, and the sequence
       in which this is done. This is assumed to be the first installation. An update is not
       scheduled at that point. In this case, uninstall the service before installing and executing
       the new setup.
\\Jupiter\doku_docuware\Interfaces\OrderXml\Doc includes the document OrderXml_deu.doc
which handles the general OrderXML structure in detail.
Document
\\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity\Installation_Configuration\TU_090
327_InstConfigListAlcibAlcimOrderXML_129902.doc
serves as a system-wide overview of the settings required for the communication between ALCIB
and ALCIM AWCapacity.
\\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity\FAQ_Tips_Tricks\AlcibAlcimFAQ.do
c shall help to understand the general interaction of ALCIB – ALCIM and the search options.


1.12.           Annex: A+W processing Type Information
For processing steps allocated to an A+W processing type, the OrderXML file offers the
information awProcessing. Apart from type ID and quantity, this includes the catagory and the
relevant parameters according to the processing type.
For every processing tpye, the following table describes lists the category and processing
parameters maximally transferred, and the field in the ALCIB database from which the
information is loaded.
The imported processing quantity depends on the defined quantity unit and is calculated based
on the quantity and the sizes. It applies to every processed element.
In connection with edgework please note that the edges to be processed can be determined
correctly only if the BYTE_VEKTOR environment is used in ALCIB.
Reversal applies to the definitions in the processing vector (for edges and corners) and to the
corner used as a basis for positioning the processing step, but not to manually defined reference
corners for the surface treatment itself which must be entered in ALCIB as a fixed value.
The ALCIB processing vector which defines the edge to be processed will now be adapted to the
production settings (e.g. from ShapingNesting)
before the OrderXML transfer, depending on the processing (A+W processing type) and the
shape.
For clarification: A circle (shape 60) has no corners and therefore one continuous edge. The
processing step "masking" can be applied here only in four steps.
From the production point of view, a circle therefore has four edges. In this example, the



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                        103
processing step would be defined for one edge in ALCIB. The OrderXML file would however
transfer four edges to be processed.
For A+W processing types you can configure whether and which parameters can be defined.
Parameters which are irrelevant for a processing step are usually marked by a special "specified"
flag. Such a flag is however missing for the parameters <...-KEY> and <...COLORCODE> of surface
treatment. The fixed value „null“ shows in this case that the parameters for the relevant
processing step are missing.
The information in the following table are based on the second processing type catalog version
(11.05.2009) which is globally valid from program version 2011 onwards.
For various processing steps – like drilling and surface treatment – there are several options for
defining the position of the processing steps on the sheet. These processing steps are classified by
different dimensioning types for this purpose (called mtyp in the table below). The awProcessing
section in OrderXML is further divided into a Dimensioning section for positioning (depending on
the mtyp either CornerDim, EdgeDim or CornerEdgeDim) and a ProcessingArea section for
dimensioning the processing step itself. The table tries to explain where the individual parameters
can be found in the OrderXML file; parameters for which only the parameter name is shown are
found directly in awProcessing. The following picture shows an exmple for coating (processing
type 1200), with dimensioning type 1.




If the OrderXML file is meant to be transferred to ALCIM: There is a similarly structured table in
document
\\jupiter\DOKU_DocuWare\Interfaces\OrderXml\Bearbeitungstypen_nach_ALCIM\2012\Bearbeit
ungstypenOrderXMLNachALCIM.doc .
From SP 5.2 the new processing surface macro (1910) and additional motif parameters for surface
processings (1200, 1205, 1210, 1215, 1220, and 1225) are available. The OrderXML service can
consider these parameters from version 12.1.8. However, a transfer may only take place if the
reading program also has the corresponding version (e.g. A+W Production SP 5.2). If this is



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                       104
guaranteed, please set the switch ORDERXML_VERSION to the value "5.1". The new parameters
are then also listed in the OrderXML.
The current information about the A`W processing types is available in the document "DE-
Normierter-Bearbeitungskatalog".




A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                   105
2. AWP Connection
2.1. Overview
2.1.1. Motivation and goals of this development
Up to now, the ALCIB has been working closely with the PMS. This is taken over by capacity
planning and production management. In the future, ALCIM shall replace PMS.
This project helps to achieve better integration between ALCIB and ALCIM. Important points of
this integration are:
   •   Link with ALCIM capacity planning:
   •   Transfer of machine and personnel costs from ALCIM
   •   Order generation
   •   Simplification of the mechanism for reporting of completion reports from ALCIM to ALCIB.
   •   New rack feedback
   •   Display of ALCIB - shipping information in ALCIM


2.1.2. Components of the connection
The following section lists all components involved in the communication between ALCIB and
ALCIM.

ERP Webservice

The ERP web service is a central component of communication between ALCIB and ALCIM. He is
responsible for the following tasks.
   •   Creating the XML - data stream for writing OrderXML - files, which serve to transfer the
       order to the production (until version 2009).
   •   Provision of various functionalities which are called from ALCIM.
   •   Reporting goods receipts to the PPS web service (until 2009)

PPS-Webservice

The PPS web service provides methods to transfer information from ALCIB to ALCIM.

ALOrderXmlService

The ALOrderXMLService checks at regular intervals whether there are orders to be transferred to
production. In this case, an XML data stream is generated and written to an XML file.

AlcibExportService



A+W Software GmbH       EN-CONFIG-A+W EnterpriseProductionInterface.docx                      106
The AlcibExportService checks at regular intervals whether there are any incoming goods to be
reported to production. In this case, the information for this goods receipt is determined and
transferred to the PPS Web service.

Commonbase

The Commonbase provides the rights and switches for the ERP web service, the ALOrderXML
service and the ALGoodsReceiptService (until 2009, after that the configuration is done via ALCIB
environment switches).

RPC – Server

The RPC server is a background process controlled by the control server that provides the ERP
web service the ALCIB functionality.


2.1.3. Process description of the connection
The following sections describe the communication between ALCIB and ALCIM. The following
diagram shows the components involved in the communication between ALCIB and ALCIM.




Transfer of Orders to ALCIM




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                        107
First of all, an order must be entered in the ALCIB. If this is released for production, a note is made
in the "ottransfer" interface table and the order is blocked.
The OrderXML service regularly checks this table for new entries. In this case, an XML structure
with all production-relevant information for this order is generated. A file in OrderXML format is
then created and made available to the ALCIM import.
In addition to the standard transfer of orders to ALCIM, quotations and orders with the same
mechanism can also only be transferred for cost calculation.

Obtaining master data information via ERP web service

ALCIM requires some information such as calendar dates, warehouse numbers, cost centers or
even customer information from the ALCIB. For this purpose, the ERP web service provides
methods which are then called from ALCIM.

ALCIM Scheduling Orders

The OrderXML file generated by the OrderXML service is imported by the ALCIM import and
submitted to capacity planning for scheduling. During scheduling, capacity planning calls up
several methods of the ERP Web service to request customer handling times, possible delivery
dates for purchase parts and route information. If the order has been successfully scheduled in
ALCIM, the scheduling is then finally reported back to ALCIB via the ERP Web service. If necessary,
the delivery date is postponed in ALCIB, purchase orders are generated and costs are written back
to the order.
No matter whether the order was successfully scheduled or not, it is unlocked again in ALCIB at
the end of this process.

Reports

As production progresses in ALCIM, status feedback on production status and racks is generated.
These are bundled and reported back to the ALCIB.

Receiving message

Incoming goods in ALCIB are also reported to ALCIM. The interface table 'exportinfo' is filled
during receipt of goods. This interface table is polled by the'A+W ALCIB Export Service' (AWDesk
#178089), which forwards the information to the PPS web service.


2.2. Functions
This chapter describes the functions of important parts of the connection and explains
restrictions.


2.2.1. Postponement of delivery date
When the order is scheduled in ALCIM, the delivery date may be postponed, for example, due to
production bottlenecks or longer delivery times for purchased parts. If this is the case, the
following actions are performed in ALCIB:



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                         108
    •   Updating the order
    •   Note in the order changes ('kaufedit')
    •   Note in the order status ('kaufstat')
    •   Updating the shipping data
    •   System message 74 is sent.
    •   Logging in overview of delivery date change ('kaufltedit')

Starting with ALCIB version 2011 an additional comment can be received in this context. It should
be possible to enter the comment in A+W Production in the re-scheduling editor if the delivery
date is affected by re-scheduling. After booking in the ERP system (in table kaufltedit), it is
displayed in the overview of delivery date changes. The text will also be added to the memo that
e-mail users can send after delivery dates have been moved. If no comment is entered, a standard
text will will be booked (available in 2011 and 2012 from SP3 ).


2.2.2. Calculation of dates for the receipt of goods
During capacity planning, ALCIM asks ALCIB for each BOM element to be ordered whether the
BOM element can be available at the time calculated by capacity planning. For this purpose,
ALCIM transfers the calculated time to the ERP web service. The latter then calculates the earliest
possible delivery date. If this is before the date received from ALCIM, ALCIM can continue to work
with the requested delivery date in ALCIM. Otherwise, capacity planning receives the earliest
possible delivery date and must reschedule planning.
The calculation of the earliest possible delivery date for subparts in the ALCIB is based on today.
The delivery time is then determined according to the following hierarchy:
    1. Article-variant assignment (artfarbzu)
    2. Article-supplier assignment (artliefzu)
    3. Article master (artikel)
If an entry is found on one level, the lower levels are ignored.
For purchased header parts, the delivery time can be carried out manually in the order. The
function takes this time into account.
As of version 2011, the delivery time (for purchased header parts as well as for purchased
subparts) can alternatively be determined using a customer-specific SP .
This allows e.g. to define delivery times for special BOM structures or in case the ordered element
includes certain processing steps.
If no such a SP exists, the above mentioned time scheduling applies. This is also the case when the
SP requires this.
Delivery time calculation via SP overrides all other rules.
The program loads the SP with the following parameters:
procedure cu_pmartlieftage( auftrnr integer, aufnr integer, posnr smallint,poskonr smallint ,tnr
smallint ) returning smallint, smallint.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                       109
For ordered sub-elements, this is tnr the tupel number from table aufstrukt. The tnr for ordered
items (main items) is 0
The SP must return two SMALLINT values:
    •    The first value represents the delivery time for the P.O. in days (over or equal 0, maximum
         365 days).
    •    The second value must be 0 to define that the delivery time determined by the SP shall be
         used. If the second value is not 0, the standard scheduling routing will be used.
Please note: The same SP call is used as in the obsolete PMS scheduling function. In case of a
change you should make sure that the SP does not access PMS tables.
The delivery time determined is then added to the current date, taking the trading calendar into
account.
Example:
Today Thursday July 8, 2010, delivery time 4 days
         Result Wednesday July 14, 2010, as it is the weekend from July 10 to July 11 and
          the weekend is usually not one of the trading days.
The standard route of the supplier is then determined and the goods receipt date is moved to the
next tour day in the future. Finally, the supplier handling time (mp.hzeit or
AWC_MIN_HZEIT_LIEFERANT) is added. This time in operation after delivery is required in order
to make the goods available to production (unpacking, etc.). This is the earliest possible relevant
date for the production start, which is reported back via the ERP-WS method
GetItemProcurementDate.
AWP then schedules the order with this restriction and determines the date on which the goods
are really required for production.
During the later PO generation in CompleteScheduling, this date is then reported to AWE and a
goods receipt date (delivery date of the PO) is determined in that the handling time is deducted
again.


2.2.3. Order generation
After successful scheduling in ALCIM, P.O. proposals for all purchase parts of the BOM are
generated within the ERP web service. For this purpose, the supply type of the ALCIB BOM is
evaluated. The dimensions of the purchase parts are not taken from the order in the ALCIB, but
are returned to the ALCIB by the ALCIM to ensure that grinding allowances or similar are taken
into account in purchase order.
After successful scheduling of a changed order in ALCIM, the purchasing data need to be
updated.
For external purchases via the ALCIB order pool, this is possible as long as the previous
purchase suggestions are still in the pool and are not being processed: These are then
deleted and new entries are made for the new purchase elements.For internal and
automatically generated purchases, changes can still be made as long as the orders are
not yet released. Previously, when using the ALCIB-ALCIM link, the previous purchase
elements were always first cancelled and then new purchasing suggestions were made
for the current purchase elements. However, as new purchases are also always generated
and the P.O. numbers have changed, the behaviour has now been changed (Webservice


A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                       110
Build 12.0.1283 ). A cancellation will only take place for suppliers where no further
elements need to be purchased any more after the order change. A cancellation will also
take place with an internal site separation if the site number of the order changes.
Another cancellation reason has been implemented with case #339976. A cancellation is
also triggered when the transaction type changes (kpos.geschart <-> awc_bestproto).
Otherwise, ALCIM will only generate purchasing suggestions for the order purchasing
elements. In ALCIB, this means that for suppliers that have not been changed, the
purchases are only adapted. The P.O. numbers remain the same.
If an existing purchase order cannot be cancelled, the new scheduling or scheduling is rejected
and system message 73 is sent.
However, you can force scheduling in ALCIM that completely ignores purchase orders. The
existing orders remain unchanged and it must be ensured manually that the purchase orders are
correct and arrive on the correct date.
Simultaneous processing of an order in the AWE order pool and in the AWP load transfer
It can happen that an order is processed simultaneously in the AW Enterprise order pool and in
the AW Production load transfer.
In this case, the date of the original order suggestion cannot be changed, because otherwise the
processor in the AWE order pool is working with out-of-date data. In this context, there are now
two safety mechanisms:
In the course of the load transfer, a possible order date is queried by the ERP system. If the order
record is blocked via order pool or if an order already exists, the ERP then returns the original
order date. For the load transfer, if the date is after the follow-up processing, this can mean that
no load transfer is possible. Then no shifts on the work process for the incoming goods can be
determined.
However, it the date is earlier than the follow-up processing, a load transfer is possible. The new
dates are reported back to the ERP system.
The ERP system receives the message and checks whether the order date can still be shifted. If it
is determined that the original order record is still blocked, whether because it is being processed
in the order pool or has even already triggered an order, then the existing order record is not
changed. For this case, an e-mail notification can now be configured. The e-mail then informs
about the various dates and a decision can be made in the ERP system whether the date can be
shifted manually in the order pool.
The e-mail notification is configured using the switch PMEINBTERMINAENDMANR. The switch
must be active and the employee number of the inititiator of the mail must be defined with it.
This employee is then informed by default if an order date has changed, which could not be
written back into the order suggestion. Alternatively, using the mail ID 33, an alternative group of
recipients can be defined.
Insofar as an order suggestion is blocked only via the AWE order pool, only the order suggestion
itself cannot be updated (there is no additional entry in the tables bestwun and bestpool).
Additional order data such as changed model data or relevant processing parameters is then
adjusted. There is also an additional note in the table awc_bestproto: In the comment it is then
possible to tell that there was a block, that is, under some circumstances, the date may not match
the one in the production date. (Available in 2011 and 2012 versions from patchbuild version of
the ERP web service).
Expansion of the Bestwun lock logic with BEST_LOCK_TEST




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                        111
With the switch "BEST_LOCK_TEST," there is a check when loading and saving an order whether
there are locked records in bestwun/bestpool and this is also reported to the operator (with name
+ tel. of the employee). The changes can nevertheless be released because there can also be
production items in the order.
When saving, the free records in bestpool/bestwun are locked for the order with lockmanr= -100
(because -1 already exists) if
- it is a production-relevant change (starting with AWE5)
- and the operator transfer the changes to production.
After that, it is checked once again during the intauf run whether the release is still possible and
the records actually go to production. If not, then the lock -100 is removed again.
During the reporting via the CompleteScheduling in the ERP-WS, these records are deleted and
new Bestwun entries are written.
BEST_LOCK_TEST activates the reports for the correction.
Logic expansion via BEST_LOCK_TEST_SPERRE
BEST_LOCK_TEST_SPERRE activates an additional logic via the table awc_lock_bestwun.
If an order change was transferred to production and changes to POs arise from this, the ERP-WS
must update the records there with use of the PO pool. This must happen in timely fashion in
CompleteScheduling so that the scheduling in AWP can be completed. If, however, somebody is in
the PO pool and this record is locked with a Lockmanr, the ERP-WS cannot change this record. For
this reason, it writes cancellations to the table awc_lock_bestwun for the corresponding order
and new entries to awc_lock_bestwun without cancellation flag for all parts to be ordered after
change of the order.
If you are working with cost calculation, the background process intauf checks during the run with
still -10 whether there are records in awc_lock_bestwun for the corresponding order. If there are
such and the Bestpool lock has been released in the meantime, the cancellation records are
processed first and then the new entries are transferred.
If there were only cancellations, then only the old data to bestpool is deleted and no new data is
written to bestwun. The data is processed item by item and transferred. First via the KPOS. That
is, first all still existing items. After that, the remaining data in awc_lock_bestwun is analyzed. If
these are no longer present in KPOS, then the old data is deleted if it is free. IMPORTANT! During
the check of the existing item via kpos, communication takes place via kpos.lfdpos =
awc_lock_bestwun.kaposnr, kpos.lfdpos = bestwun.ksposnr, kpos.posnr = bestpool.orgposnr
statt. With the rest via awc_lock_bestwun.kaposnr = bestwun.kaposnr,
awc_lock_bestwun.kaposnr = bestpool.orglfdpos.
If the records in bestpool are still locked, then intauf resubmits the order itself with still -46 and
tries again later.
If the data was locked at the time of the takeover and was written to awc_lock_beswun. At the
time of the processing by intauf, however, POs for the order are already generated and there are
no "old" data in bestwun/bestpool. Here, the data is no longer taken over and deleted from
awc_lock_bestwun and the operator receives a system message (meldId= 1) "Check order"
Conclusion: with active cost calculation, the test for takeover of the data from awc_lock_bestwun
always finds still=-10 or still=-46.
If you are not working with cost calculation, the consequence is that the corresponding order no
longer runs through intauf with -10 and thus the logic described above cannot be triggered. To



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                           112
resolve this situation, today intauf checks with each start whether there are still records in
awc_lock_beswun and then initiates their processing. This has to be changed so that the ERP-WS
recognizes that you are not working with cost calculation and in this case places a record with still
-46 before intauf.
In addition, the employee who is in the PO pool and tries to trigger a PO for which a record exists
in awc_lock_bestwun, receives the message:
37335 : "The corrections for the purchase order proposals are already present. These will not be
taken over if you trigger the PO now."
Order cancellation (general)
With an attempt to cancel an order, there is a check whether it is still locked via PO pool. The
cancellation will be rejected on the spot if this is the case. The operator is also informed who has
locked the order at the moment. Only after the PO pool user releases it is cancellation possible
again.
Transfer to AWP despite ordered sub-parts
Order items 1-4 entered and transferred to AWP.
    •   Item 1 partially ordered!
This PO places the order NOT IN LOCAL CORRECTION!!!!
    •   Change to item 4 (free item).
Why shouldn't the data go to AWP here? The transfer to AWP is absolutely legitimate.
    •   Change to item 1 (partially ordered)
We do not distinguish the type of change!!! Since the order is not in local correction, the variable
KAUFUPDATE_BEI_BEST also plays no role. This variable was only created for the case that the
order is in local correction and thus completely locked. Thus the "local correction" is loosened if
the concern is exclusively POs as lock. Then the status per item was also evaluated. If, however,
the order is not in local correction, then it is a normal change that will also be passed along.
And to detect the status "ordered," the search is done with the order number in kaufstat
according to modus=301.
The ERP-WS checks during transfer to AWP whether there are existing POs. These will then no
longer be changed and the scheduling is done around these fixed PO dates.
Since there are no BOM-based locks and the system therefore cannot determine which BOM
elements can still be changed and which not, the operator must ensure by himself that he only
makes not YET PO-relevant changes to the item/BOM.
Dimensions of purchased spacers
Dimensions of the purchased parts are reported by AWP. This also applies to purchased spacers
and muntins. A correct calculation of dimensions require the new step entry in AWE and a
respective setting for ALCIM works.
Especially for spacers: The dimensions in AWP refer to the outside edge of the spacer. But AWE
needs the dimensions up to the inside edge of the spacer. Before a purchase order for spacers is
created, the Web Service calculates the spacer dimensions up to the inside edge. The calculation
is done both for shapes as well as for rectangular lites. (Available from version 2011 in a certain
patch version of ALRPC service and ERP webservice ).
See also AWDesk #256754 and #452453



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                       113
Order cancellation
If an order is cancelled in ALCIB, direct purchase orders via Intbest have to be cancelled as well as
data noted by the Webservice for P.O. creation has to be deleted. This will happen now already in
the background process intauf. Analyses can be made by means of the F-Test log in intauf. Min.
prerequisite: ALCIB 2011, Build number 2893 Rotation for purchasing
By default, the order is always with view of shift so that lites with coatings will be turned if
necessary. In A+W Enterprise, you can use the control for rotation for purchasing (EK_EP_DIREKT)
to disable this. If the switch is set, the order is placed as entered, with appropriate installation
position on the head part.
The turns refer to the shape dimensions and the processings applied.
In order to generate the purchase orders unturned, the EK_EP_DIREKT switch must be set in A+W
Enterprise.
In A+W Production the switch ALCIM_SHAPES/SN_CLOSE_MODE should be set to 0.
If, however, for certain reasons the switch SN_CLOSE_MODE must be set to 3 (or later 4),
attention must be paid that both switchesALCIM_SHAPE/SKETCHFLIPPINGVIEWS and
ITEMS4ALCIM_SETTINGS/VIEW_FOR_ORDERS_IN_SN are set to different SN views.
The evaluation of the switch EK_EP_DIREKT is possible from A+W Production 5.2 and from web
service build 3.6.2733




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                       114
Cost calculation
The personnel and machine costs are calculated exactly in the ALCIM and are returned to the
ALCIB after successful scheduling or rescheduling. In ALCIB, the cost calculation is updated by
deleting all existing personnel and machine costs (that were not created manually) from 'poskost'
and creating the new records.
For each BOM element transferred from A+W Production, the system checks whether machine
costs (MachineryCost) > 0 or personnel costs (LaborCost) > 0 exist. For each of these cost
specifications, if it is > 0, a cost rate is created in A+W Enterprise (table poskost). If no cost center
was transferred from AWP, the cost center in AWE remains empty for this cost record.


2.2.5. Stock forecast
After creating the work plan and scheduling via AWCapacity in ALCIM , stock forecasts can be
collected in ALCIB based on the results.
The BOM in ALCIB is searched for elements received from stock. Relevant are only those articles
for which the stock change code



    •   PMS,


    •   delivery note/PMS (only for BOM elements,) , or


    •   manual/PMS (only for BOM elements)

is defined.

These articles will be collected in the stock forecast table wlppms including order number, item
number, and tupel number. The forecast date (field a_datum) is adopted from the production
date determined by ALCIM for this element. If the element itself is not part of the ALCIM element
tree, the production date of the next parent element on the ALCIM element tree will be adopted.
The forecast quantity is calculated by means of the width, height, and - if applicable - thickness
depending on the quantity unit defined in ALICB article master data. Width and height match the
values in the ALCIM element tree (for the current element or for the next existing parent
element). The thickness is based on ALCIB article master data artikel.staerke): It is based on the
total thickness of the sub-elements. If the thickness has been defined for none of the sub-
elements in article master data, the thickness of the element itself is adopted from article master
data; if no thickness has been defined there either, the thickness of the next parent element will
be used. A special loss can be taken into account when calculating the quantity.
The quantity takes into account the item quantity (for BOM elements) and the entries in fields
Qty1 and Qty2 in the BOM tree.



The inventory number is usually determined by means of article master data. There are additional
configuration options.




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                          115
For main articles taken from stock, the stock variant comes directly from item data. A customised
solution can be enabled for BOM elements if required.
The booked colour versions match the entries in the ALCIB BOM.



If ALCIM reports rescheduling, the forecast date (a_datum) will be adapted. Prerequisite is that
the forecast status permits this (wlppms.status must be 0).
Availability and configuration options of this functionality are described in the appendix.

Function change history

Whether the last changes to the warehouse forecast function are already available in an
installation can be recognized in the ERP web service log in the future, provided a log depth of 4
(Verbose) has been set. In the first log message of each forecast booking, a type of version ID will
be displayed in the form:"<CompleteScheduling><Stock Forecast 3.6.2> ...". The following tables
briefly describe the changes for each version.
Changes to the stock forecast in version 2009
         Date          Process      Comment
                       Version
         2010-07-08    203868       Supply type for header parts is determined
                                    from item data (kpos) and not from BOM
                       3.5.2
                                    data (aufstrukt).




Changes to the stock forecast in version 2011
         Date          Process      Comment
         2010-07-08    203868       Supply type for header parts is determined
                                    from item data (kpos) and not from BOM
                       3.6.2
                                    data (aufstrukt).




Order cancellation
If an order is cancelled in ALCIB, storage forecast data must be deleted. This will happen now
already in the background process intauf. Analyses can be made by means of the F-Test log in
intauf. Min. prerequisite: ALCIB 2011, Build number 2893


2.2.6. Consideration of item splits when the successful scheduling is
    confirmed
When you confirm a successful scheduling, costs are booked, order proposals are generated, and
stock forecasts are determined. It is important that each item in ALCIB and within each item of
each part/processing is reported only once with the correct number of pieces. For this reason,
split items are combined again, depending on the type of split:
    •   Item split in OrderXML based on ALCIB rack planning: The items are combined again
        before being booked by the ERP web service. The item quantity is added and the average



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                       116
        is calculated for the processing costs. The smallest purchase order date is determined.
        The production date (e.g. relevant for stock forecasts) is determined as the smallest date
        for scheduling and the largest date for rescheduling.
    •   Item split during scheduling through capacity planning: An item record with multiplied
        parts/processings is confirmed from the scheduling. These are combined again before
        being booked by the ERP web service. The item quantity is added and the average is
        calculated for the processing costs. The largest is determined as the production date. If
        the measurements differ at all, the largest measurements are taken. The smallest
        purchase order date is determined. For the processing costs the average is calculated.
    •   Implicit processings: During scheduling, processings can be added implicitly (such as
        packing and sending). Then, these all have the same reference, namely that of the part.
        Since each reference may only occur once, these processings are already combined in the
        ALCIM import before report. The costs are totaled. Exception: If the Alenv
        SPLIT_POSKOST_COSTS is set, the costs of these processings are processed individually.


2.2.7. Status confirmations production
In principle, the production feedback from ALCIM to ALCIB can be divided into two categories. On
the one hand, there are the statuses without quantity information:
Error during scheduling (550)
Scheduled (551)
Roughly scheduled (552)
Scheduled in detail (553)
Released (554)
In production (555)
On the other hand, the statuses for which the number of pieces that has reached this status in
ALCIM is also confirmed as a snapshot:
    •   Produced (556)
    •   Ready for shipment (557)
    •   Delivered (558)
All status messages are sent with exact position. If a larger number of pieces is reported as ready
for dispatch than was previously reported as produced, the number of pieces produced is also set
to the number of pieces ready for dispatch. The same applies to a confirmation of a delivered
quantity that is higher than the quantity ready for dispatch received so far (see #197056).
Switches in the ALCIB can be used to control which of these ALCIM statuses triggers the ALCIB lock
status FIXED(300) and RELEASED(302).
The database tables for the production reports are still filled.
Overview of ALCIM and ALCIB status
The following table shows the statuses in ALCIM, the status updated in the ALCIB in the kposstat
table and describes the effects of the ALCIB switches using the example: AWC_FIXIERT_AB=552
and AWC_FREIGEGEBEN_AB=554.




A+W Software GmbH           EN-CONFIG-A+W EnterpriseProductionInterface.docx                     117
       Action                  Status   Status   Comment
                               ALCIM    ALCIB
       Scheduled               0        551      After scheduling, rescheduling or
                                                 change of supply type.
       Create bucket           10       551      The status is reduced if a batch has
                                                 already been created
       Create batch            100      552      If AWC_FIXIERT_AB =552, status 300
                                                 is also entered in kposstat. In the
                                                 order display in ALCIB, the item is
                                                 marked red, fixed and in local
                                                 correction. This status can be canceled
                                                 by batch resolution.
       Detailed                150      553
       scheduling     of   a
       batch
       Release batch           200      554      If AWC_FREIGEGEBEN_AB =554,
                                                 status 302 is also entered in kposstat.
                                                 The item is marked red in the order
                                                 display, as released and in local
                                                 correction. This status can no longer
                                                 be reversed by a batch resolution.
       Barcoding       -       700      556      ALCIM reports the total actual
       Completion report                         quantity. ALCIB books the status and
                                                 the difference quantity in kposstat: If
                                                 the first time 4 was reported and
                                                 ALCIM now reports 10, the system
                                                 books in kposstat quantity 6; 10
                                                 pieces are displayed in the ALCIB
                                                 order display as finished.
       Barcoding      -        800      557      Here, too, ALCIM reports the total
       Packed message                            actual quantity. ALCIB books the
                                                 status and the difference quantity in
                                                 kposstat




2.2.8. Status feedback racks
    The ALCIM only reports information regarding shipping racks back to the ALCIB.
    Depending on the configuration, these rack feedbacks are passed on to the normal
    rack system (GESTELL_BDE or MODUL_STAPELLOGIC) and/or to the Korean rack
    system (AWC_GESTZU_BUCHEN). The table 'bcbock' is always filled. It is assumed
    that the rack number received from ALCIM is a number. Alphanumeric rack
    numbers lead to errors in the ERP web service. The rack number may have a
    maximum of eight digits. For larger numbers, only the last eight digits are
    transferred to the ERP system.
    The label number is only imported completely if it has a maximum of nine digits. For
    larger numbers or an alphanumeric barcode, the last nine digits are written into the
    'bcbock'.
    The rack feedbacks are also snapshots. All lites are always returned to a rack.
    Booking to 'bcbock' means, all existing entries for the rack are deleted first and then
    the complete content of the rack is entered again.
    The following information is booked in bcbock:




A+W Software GmbH          EN-CONFIG-A+W EnterpriseProductionInterface.docx                118
     Quantity                            awbar_teile.menge
     Auftrnr                             awbar_teile.auftnr (similar to
                                         kauf.auftrnr)
     Bmnr                                awbar_stellen.maschinennr
     Date                                awbar_teile.letztebuchung
     Etinr                               awbar_teile.etikettnr
     Gnr                                 awbar_teile.gestell; (must be
                                         numeric!)
     Posnr                               pool_pos.pos_referenz (the first
                                         three digits, similar to kpos.posnr)
     Time                                awbar_teile.letztebuchung



Rack bookings status-dependent

    Action      Status     Status    Comment
                ALCIM      ALCIB -
                           ERPWS
    Entry       0          1         A rack receipt was booked.
                                     Booking of rack receipt to the rack warehouse
                                     (AWC_RACKSTOCK_REGPOINT_TYPE- ERPWS direct +
                                     alrpc table waeingestkopf + waeingestpos
                                     Booking BCBOCK - ERPWS directly

                                     Booking rack receipt (table GESTELL_BDE -
                                     MODUL_STAPELLOGIK) - ERPWS- alrpc

                                     Booking rack shipping (table gest/getzu
                                     AWC_GESTZU_BUCHEN) - ERPWS - alrpc - rserv
                                     status 21
    Packaging   800        2         Packing rack
                                     Booking BCBOCK - ERPWS directly
                                     Booking rack shipping (table gest/getzu
                                     AWC_GESTZU_BUCHEN) - ERPWS - alrpc - rserv
                                     Status 19 + 20
    Packed      900        3         The rack was packed
                                     Booking BCBOCK ERPWS directly
                                     Booking rack shipping (table gest/getzu
                                     AWC_GESTZU_BUCHEN) - ERPWS - alrpc - rserv
                                     Status 19 + 20
    Shippping   950        4         The rack was booked to shipping
                                     Booking BCBOCK ERPWS directly
                                     Booking rack receipt (table gestell GESTELL_BDE -
                                     MODUL_STAPELLOGIK)

                                     Booking rack shipping (table gest/getzu
                                     AWC_GESTZU_BUCHEN) - ERPWS - alrpc - rserv
                                     Status 19 + 20




A+W Software GmbH     EN-CONFIG-A+W EnterpriseProductionInterface.docx                   119
Logs:

Booking table gestell:

    • ERP-WS log
    • Ftest from alrpc

Booking table gest/gestzu:

    • ERP-WS log
    • Ftest from alrpc
    • Rserv log if necessary Ftest from rserv

Booking table bcbock

    • ERP-WS log



Changes/Extensions:

ALCIB offers a configuration option which prevents the booking of rack reports ALCIM sends via
ERP-Webservice. The switch AWC_IGNORIERE_GESTELLMELDUNG controls the booking of rack
reports. If the switch is ON and active, rack reports from ALCIM will be completely ignored. This
switch must be set if ALCIM cannot guarantee that only numerical rack barcodes are used. It can
also be set to prevent unnecessary bookings in table bcbock.
If the switch is ON and active, neither the table bcbock will be filled, nor will bookings be made
that are enabled by the switches GESTELL_BDE, MODUL_STAPELLOGIK, or
AWC_GESTZU_BUCHEN. (#229434)
In 2009 and 2011 versions, a current version of the ERP web service is required to take the switch
into account.
If you want to work with the rack-related shipping (Korean rack system), the
AWC_IGNORE_PACKINGMESSAGE variable must be set. Otherwise, the packed message from
AWP will already lead to a booking of lapooliststk and the later rack message can no longer report
the rack as packed and assign it to a route.
Booking to the table gestell:
If the status of the rack (receipt or removal) should not play any role, the switch
AWC_IGNORE_AWERACKSTATUS has to be enabled. Otherwise the system will check whether for
a removal message a receipt was previously booked for the rack or for a rack receipt whether
there was previously a removal. Otherwise, if this variable is not enabled, the messages will be
rejected.
For a rack removal, the customer reference is determined via the table bcbock. For a mixed rack,
there is an attempt to determine the oldest sheet booking on the rack. The rack is then removed
on the associated customer(order). For mixed racks, a mail about this will be sent.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                       120
Flow for rack bookings: (#459400/#459099)

The rack bookings from PDC readings are reported by A+W ERP Web Services via feedback servers. For a
detailed description, see the AWE configuration instructions.


2.2.9. Provision of cost centers
With the method AWCapacityGetCostCenters(), the ERP Web service provides a function for
determining the cost centers stored in A+W Enterprise. When the method is called, the system
selects the fields kostenst and bez from table kstelle and returns them.



2.2.10.   Treatment of orders with high priority (AWDesk
    #447496)
The treatment of orders with high priority (rush orders) in AWE during the transfer to the
OrderXML service (entry in the table ottransfer) has already been described in the preceding
chapters (to be found under the keyword "prioritization").
In order to continue the prioritization during scheduling, another logic has been added to the
OrderXML service. In the OrderXML service, the scheduling type of an order is evaluated. If it is a
rush order - schedule type = "rush" (kauf.abrufkz=2), the generated transfer file to AWP receives
the "highPrio" flag in the file name. The name thus ends in "highPrio.xml".
Files with the "highPrio" in the name are then processed preferentially in the sequence for import
(scheduling in AWP).


2.3. Data structure
To connect ALCIM capacity planning to ALCIB, some new tables were required, which are briefly
described in this chapter. More detailed information on these tables is available in the table
documentation "altab".


2.3.1. awc_bestproto
This table stores information about purchase orders generated by ALCIM capacity planning. These
are used to find and cancel the generated purchase orders in ALCIM during scheduling or
rescheduling.


2.3.2. awc_fertigmeldungen
The messages for the status PRODUCED, READY FOR SHIPMENT and DELIVERED are sent to the
ALCIB from ALCIM with quantity information. These quantities are snapshots. In ALCIB, however,
difference quantities are used internally. In order to calculate the required difference quantity
from the snapshots received, the quantities previously transferred from the ALCIM are stored in
this auxiliary table with item accuracy.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                         121
2.3.3. awc_modparams
The tables that are filled for P.O. generation ("intbest" or "bestwun") cannot transfer shape
parameters. However, since in ALCIM the shape dimensions (e.g. due to grinding surcharges) can
possibly be adjusted, these changed dimensions must also be taken into account when generating
the purchase order. This table is used to transfer these dimensions to "trm_ctrl".


2.4. Environment variables
2.4.1. AWC_ALCIM_ANBINDUNG
This variable activates the logic described in this document within the ALCIB. For example, this
adapts the flow through the background processes and enables functionalities specially
developed for the logic, such as the ALCIM production report within an HTML page.


2.4.2. AWC_ART_HZEIT (PMCHZEITART)
This variable determines the unit of measurement in which the handling time is stored in the
system:
        0 - No handling time is evaluated.
        1 - Handling time in days
        2 - Handling time in hours


2.4.3. AWC_MIN_HZEIT_KUNDE (PMEDASCHMINHZEITKUND)
It stores the minimum handling time. If this is greater than the handling time from the customer
master, the value of these environment variables is used for further calculations.


2.4.4. AWC_MIN_HZEIT_LIEFERANT (PMEDASCHMINHZEITKUND)
It stores the minimum handling time. If this is greater than the handling time from the supplier
master, the value of these environment variables is used for further calculations.


2.4.5. AWC_DEF_ROUTENABFAHRT (PMEDASCHROUTENABFAHRT)
This variable contains the default departure time in seconds of the day. If no departure time is
stored for the route, this variable is evaluated.


2.4.6. AWC_BESTELLEN_BIS (PMEHEUTEBZEIT)
This variable stores site-specifically in seconds of the day until which time the order can be
placed. If the variable is not set, it is assumed that orders can be placed until the end of the day.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                         122
2.4.7. AWC_FIXIERT_AB (similar to PMXCIMRMSTATI)
This variable defines from which AWCapacity status an item is considered fixed. If the status
specified here is reported for an item, the lock status FIXED (300) is also written. The default of
this variable is 552


2.4.8. AWC_FREIGEGEBEN_AB (similar to PMXCIMRMSTATI)
This variable defines from which AWCapacity status an item is considered released. If the status
specified here is reported for an item, the lock status RELEASED (302) is also written. The default
of this variable is 554; once this status has been set for a position, it is not reduced.


2.4.9. PMVERSANDSTEUER
With this switch only the packing message from AWP to the dispatch control is regulated. The
following settings can be applied:
ON or 1
AWP reports order items to Shipping as packed as soon as the item is ready. This also applies to
partially completed quantities.
Specifications 2 and 3 are no longer supported since the introduction of A+W Production.


2.4.10.         AWC_URL_PRODUKTIONSBERICHT
In this variable the URL of the detailed ALCIM production report is stored, so that it can be called
directly from the ALCIB at the click of a button. The URL must be entered here completely, only
without the final order number. The program then appends the order number dynamically.


2.4.11.         AWC_GESTZU_BUCHEN
If this environment variable is active, the table 'gestzu' is also booked for rack feedbacks from
ALCIM.


2.4.12.         AWC_GESTZU_BUCHEN_OHNE_VERPACKTMELDUNG
If the rack feedbacks are to be booked in rack-related shipping (AWC_GESTZU_BUCHEN) and are
configured from AWP Packing messages with status 800. Packaging messages can be booked
twice, since the assignment of the racks to a tour also causes a packaging message. This can be
prevented with these switches.


2.4.13.         AWC_IGNORE_PACKINGMESSAGE
If you work with rack-related shipping and the rack should be permanently assigned from AWP
rack reporting, this variable must be used to prevent a packing notification from the AWP from
being processed beforehand.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                          123
2.4.14.         AWC_IGNORE_AWERACKSTATUS
If this variable is active, the rack status in the AWE is ignored for PDC confirmations via the ERP-
WS. In other words, if, for example, an exit is sent twice in a row, the parking lot is transferred to
the second customer and the booking is not rejected.


2.4.15.         AWC_WAEIN_UEBERMITTLUNG
If this environment variable is active, the interface table 'exportinfo' is filled when a receipt of
goods with order reference is entered. The receipt of goods is then transferred to the ALCIM by
the A+W ALCIB Export Service (#178089).


2.4.16.         AWC_BUCHE_KPOSPROD
If this environment variable is active, the table 'kposprod' is additionally filled (#180809) for
produced feedback from the ALCIM.


2.4.17.         AWC_ALCIB_SERVER_NAME
This switch contains the name or IP address of the ALCIB server and is used by the ERP web
service. This switch was introduced during the expansion of the CommonBase(#191666).


2.4.18.         AWC_PORT_RPC_DIENST
This switch contains the port number of the RPC service and is used by the ERP web service. This
switch was introduced during the expansion of the CommonBase(#191666).


2.4.19.         AWC_PORT_CONTROL_SERVER
This switch contains the port number of the control server and is used by the ERP Web service.
This switch was introduced during the expansion of the CommonBase(#191666).


2.4.20.         AWC_IGNORIERE_GESTELLMELDUNG
The switch controls the booking of rack reports. If the switch is ON and active, rack reports from
ALCIM will be completely ignored. This switch must be set if ALCIM cannot guarantee that only
numerical rack barcodes are used. It can also be set to prevent unnecessary bookings in table
bcbock.
If the switch is ON and active, neither the table bcbock will be filled, nor will bookings be made
that are enabled by the switches GESTELL_BDE, MODUL_STAPELLOGIK, or
AWC_GESTZU_BUCHEN. (#229434)


2.4.21.         GESTELL_BDE
Book completion reports from the barcoding to the rack management. Table gestell, gestellz,
bugest…



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                          124
2.4.22.         AWC_RACKSTOCK_REGPOINT_TYPE
This variable is used to define the registration point type for which the stock addition is booked
for a stock filling order in the rack warehouse.
For this purpose, the registration point number must be entered in the registration points in A+W
Production as ERP machine.


2.4.23.         AWC_NACHBEST_MANR
As of version 12.1, the functionality of the remake order can be activated. If an ALCIB employee is
to be informed by mail about parts to be reordered, this variable must be activated. As value, the
number of an employee must be stored, who then counts as initiator of the mail or as mail
recipient if nothing else is defined in the ALCIB mail system for the mail-ID 43.


2.4.24.         PMEINBTERMINAENDMANR
If order dates are affected by a re-scheduling in AWProduction that can no longer be changed in
AWEnterprise (block in the purchase order pool or purchase order released), then a mail
notification can be configured. The switch must be active and the employee number of the
inititiator of the mail must be defined with it. This employee is then informed by default if an
order date has changed, which could not be written back into the order suggestion. Alternatively,
using the mail ID 33, an alternative group of recipients can be defined. (required in 2011 and 2012
patch version of ERPWebservice ).


2.4.25.         PMEZKBESTELLT
If the variable is active, cutting corrections from table awc_modparams are taken over for
purchased glasses from trm_ctrl during purchase order generation. Table awc_modprams is filled
during feedback from AWP with the data determined in AWP (for example, due to grinding
allowances) . Table awc_modparams is filled regardless of whether the variable is set or not.


2.4.26.         SPLIT_POSKOST_COSTS
Automatically generated operations, such as packing and shipping, are no longer cumulated on
the corresponding part, but are returned by ALCIM as independent parts of the BOM and written
to poskost.


2.4.27.         BEST_LOCK_TEST
The variable activates check when obtaining or saving the order correction, whether the order
was being obtained for PO generation (bestool-, bestwun-, intbest-lock) Only until AWE5. Starting
with Version 6.0, there is always a check.




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                        125
2.4.28.         BEST_LOCK_TEST_SPERRE
Activates the logic that mistaken writing of the data in bestwun because the data is being
processed in the pool is backed up in a lock table and written again by intauf (intauf -46) to the
table at a later time.


2.4.29.         KAUFUPDATE_BEI_BEST
A released PO sets the order to the state of LOCAL CORRECTION. Thus an order change can no
longer be transferred to purchasing. (ON+WAEIN even if GR is already generated) If this variable is
active, then despite LOCAL CORRECTION, the changed order can be transferred again to the PMS
if the user responds to the subsequent security query appropriately. This order change is no
longer communciated to purchasing. The POs thus remain unchanged.


2.5. Switch in ALCIM
Starting with ALCIM version 2011 SP1, all switches in this context can also be set in ALCIM. This is
recommended from AW Production 5. In the following, first the switches for the functioning of
the logic are described, but then also the switches which are also important in the interaction
ALCIB-ALCIM.
All switches can be set via the ALCIM configuration dialog (menu item Master Data >
Configuration).


2.5.1. Switch for loading OrderXML files.
Some switches are station specific. In this case, you must make the settings for the station on
which scheduling is running.
ALCIM -> Import (Items4Alcim) -> <StationID> -> Settings -> Import Interface:
Set the switch to '1', so that OrderXML files are read
ALCIM -> Import (Items4Alcim) -> <StationID> -> Settings -> Archive Path
In the directory path specified here, the OrderXML files that were successfully imported are
saved.
ALCIM -> Data import (Items4Alcim) -> <StationsID> -> Settings -> Problem path
OrderXML files that have not yet been successfully imported are saved in the directory specified
here. More detailed information can then be found in the ALCIM post-processing.
ALCIM -> Data import (Items4Alcim) -> <StationsID> -> Settings -> Import path
The new OrderXML files should be read from this directory path. This is the directory where the
OrderXML service writes the OrderXML files.
ALCIM -> Import (Items4Alcim) -> (global) -> Customer Settings -> Processing Sequence
The value must be set to '1'. The processing sequence on a part can only be determined by the
master data in ALCIM.
ALCIM -> Import (Items4Alcim) ->(global and station-specific) -> ALCIB Communication




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                        126
The parameters in this area are not evaluated in this context. They were only relevant for direct
data import from PMS.
ALCIM -> General -> (global) -> Settings -> BOM Mode
Has to be set to 1. Spacers and muntins must be imported as producible parts according to ALCIM.
ALCIM -> General -> (global) -> Settings -> Complete BOMs:
Has to be set to 1. All parts and processings must be known in ALCIM, for example for turning
processings under purchase parts or the change in the supply type of laminated glass products.


2.5.2. Switches without Common base
Starting with versions 2011, CommonBase has been gradually removed from the programs. In AW
Production 5, the Common Base is already only needed for the rights management in ALCIM. But
even then it is recommended to set the earlier CommmonBase switches directly in ALCIM.

In ALCIM 2011 the expansion of CommonBase was not yet complete. It is recommended to set
the switches in both CommonBase and ALCIM.
Most switches can be set both global and station-specific (unless otherwise specified). Please note
that if you set a switch to station-specific, all switches must be set to station-specific.
ALCIM -> General -> Settings -> Use CommonBase
This switch can only be set globally.
It can be activated when a CommonBase is in use. It is mainly used for user rights.
ALCIM -> General -> Settings -> Use CommonBase also for Settings
This switch can only be set globally.
It is considered active by default if the "Use CommonBase" switch is active.
It can then be explicitly set to '0' so that all settings for capacity planning, ERP web service
communication and so on can be made in ALCIM. In this case, the CommonBase is actually
considered to be pure rights management.
ALCIM -> General -> Feedbacks -> Erp Feedback
This switch can only be set globally.
It must be set to'1' so that the feedback to ALCIB is sent via the ERP web service instead of via
STSL files.
ALCIM -> General -> ERP System Settings -> URL:
Enter the URL of the ERP Web service here. It begins with " http://... ".
ALCIM -> General -> ERP System Settings -> Timeout:
Timeout of the ERP web service.
ALCIM -> General -> ERP System Settings -> Version:
Determines which Web service methods are called. In ALCIM version 2009, 2011 to AWProduction
5 the value '35' must be set in connection with ALCIB. As of AWProduction 5.1 the value '37' is still
available above which performance improvements can be activated.
ALCIM -> General -> ERP System Settings -> Database Server:
Name of ALCIB database server.



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                          127
ALCIM -> General -> ERP System Settings -> Database Name:
Name of ALCIB database
ALCIM -> General -> ERP System Settings -> Database User:
Name of a user on the ALCIB database.
ALCIM -> General -> ERP System Settings -> Database Password:
Password of the specified user on the ALCIB database.
ALCIM -> General -> ERP System Settings -> ERP System:
Select "ALCIB" from the predefined selection.
ALCIM -> General -> ERP System Settings -> Database Type:
Select "Informix" from the predefined selection.
ALCIM -> General -> ERP System Settings -> Database locale:
Database locale value, such as "en_US.CP1252".
ALCIM -> General -> ERP System Settings -> Client locale
Client locale of the ALCIB database, such as "en_US.CP1252".
ALCIM -> General -> ERP System Settings -> Site Number:
For internal site separation in ALCIB (MODUL_INTERNE_MANDANTENTRENTRENNUNG), the
number of the site for which ALCIM is responsible must be entered here. The setting is used in
ALCIB to address the correct ALRPC process and evaluate the correct switches. However, even
without site separation, the correct site number must be entered here, namely the number as it
also appears in the order (database field kauf.hausnr).


2.5.3. Additional ALCIM switches for ALCIB-ALCIM communication
The following parameters should also be checked and set when setting up ALCIB-ALCIM
communication. They influence the data that is reported to ALCIB (for example, for purchase
order parts).
ALCIM -> General -> Shape Catalogs -> Mode to Close SN Files
This parameter affects the turning of SN views. The setting '4' is recommended here, which causes
ALCIMWorks to turn the view. Otherwise the turning will take place at a later time, which may
cost time. This parameter is related to parameter ALCIM -> General -> Shape Catalogs ->
Shaping/Nesting Drawings.
ALCIM -> General -> Shape Catalogs -> SN Views to be Turned
Several views can be specified here. However, it is important that the SN view specified for
turning purchase order parts is also specified. See Switch ALCIM > Data Import (Items4Alcim) >
<StationID> > Settings > Purchased Parts View in SN
ALCIM -> General -> Shape Catalogs -> Use New Shape Recognition
Should always be set to '1'.
ALCIM -> General -> Shape Catalogs -> Resolve Shape Geometries
Useful values are '2' or '3'. '3' should be set if the resolved geometries shall also be saved (with
bearb_nr=1000); this is always useful for ALCIB.



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                             128
ALCIM -> General -> Shape Catalogs -> Geometry Resolution
Always set to '1'.
ALCIM -> General -> Shape Catalogs -> Use Cache for SN
Must be set to '0'.
ALCIM -> General -> Shape Catalogs -> Create Raw Geometry for P.O. Parts
Only if this parameter is set to '1', order parts with the correct geometries can be ordered.
ALCIM -> General -> Shape Catalogs -> Turn Shaping & Nesting Drawings:
If the parameter ALCIM -> General -> Model catalogs -> Mode for closing SN files is set to '4', this
parameter must be set to '1' or '2'. This is the prerequisite that ordered parts are reported back to
ALCIB with turned model number if required.
ALCIM -> General -> Shape Catalogs -> Consistency Check BOM and Drawing:
The setting '2' is recommended. The prerequisite for this is the consistent use of the A+W
processing type catalog, which should also be the standard.
ALCIM -> General -> Shape Catalogs -> Spacer - Geometry Calculation
This parameter should be set to '1', especially when working with the new shape entry in ALCIM.
This causes the calculation of the spacer and muntin geometries, which can then be taken into
account in the ALCIB for order generation or stock forecast.
ALCIM -> Roughly Scheduling -> Shaping & Nesting -> Datafile Path
The specified directory should be accessible to all programs: ALCIB, ALCIM and SN.
ALCIM -> Import (Items4Alcim) -> Settings -> Create SN Files
Should be enabled if the shape number for ordered parts needs to be mirrored if required. Please
note that the continuous use of the A+W machining type catalog for machining is a prerequisite
for this.
SN files are only created if no file has yet been created in ALCIB.
ALCIM -> Import (Items4Alcim) -> Customer Settings -> Edge Shift Module
Should always be set to '2'.
ALCIM -> Import (Items4Alcim) -> Customer Settings -> Processing Sequence
The value must be set to '1'.
ALCIM -> Import (Items4Alcim) -> <StationID> -> Settings > P.O. View in SN
Enter the name of the SN view in which the order part is to be turned to the correct edge. This
view must also be included in the definition for parameter ALCIM -> General -> Shape catalogs ->
SN Views to be turned.
ALCIM -> Import (Items4Alcim) -> <StationID> -> Settings > Report Processed Parameters ...
Only if this switch is set to '1', the processing parameters for processings under purchase parts are
also reported back to ALCIB. This is necessary for processings that are assigned to an A+W
processing type and that lie below a purchase order part whose shape number has been mirrored.
ALCIM -> Import (Items4Alcim) -> <StationID> -> Customer Settings > Ignore Error in Size
Correction




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                       129
Must be set to '0', otherwise it could happen that purchase order parts are confirmed without
dimension correction.


2.6. System messages
2.6.1. Status 73 - Scheduling or rescheduling failed

2.6.2. Status 74 - Postponement of delivery date

2.6.3. Status 43 - A broken product contains purchase order parts
    which have to be reordered



2.7. Logging
        2.7.1.   Report (CompleteScheduling) about the ERP
            Webservice
The reporting of a scheduled order is done with a call to the CompleteScheduling method of the
ERP Webservice by AWP. Reported are especially ordered parts and their current dimensions and
parameters.
The logging of the report is done in the ERP Webservice log ("%PROGRAMDATA%\A+W\log").
In addition, the storage of the report object can be configured for research purposes. The report
object includes all data reported by AWP for an order in the xml structure.
The activation of the report object is done with the env variable AWC_ERPDOC_FILE. It is
recommended that you activate the variable with the value "201". For activation with the value
"201," for each order the current report object for the last 24 hours can be found in the directory
"%PROGRAMDATA%\A+W\A+W ERP Web Service" under the name
"compsc_<auftrnr>_YYYY_MM_dd_HH_mm_ss.xml".


2.8. Appendix
2.8.1. Stock forecast in version 2009 and configuration options
The logic for the stock forecast booking, described above in chapter "Funktionalität;
Lagerprognose" is available in ALCIB Version 2011 as a standard. Whether or not a booking will
be made, can be defined by means of the stock change code in article master data.

It has to be specially enabled in Version 2009. Prerequisite are the latest build numberes of ERP
Webservice and of the ALCIB background process alrpc. Prerequisite are the latest build
numberes of ERP Webservice and of the ALCIB background process alrpc. The table awc_wlppms



A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx                       130
must exist. This table contains temporary data for the alrpc background process which makes the
booking in table wlppms. To install this table later, please use the script from the UNIX
development servers (see case 171284):
Updating the stock forecast date in case of rescheduling is a new feature. Otherwise, the data for
stock forecast are determined in the same as as by the former PMS. Quantity calculation does not
permit to analyse BOM formulas. A special loss can be defined via switch PMLAGERVERLUST. If
this switch is active and set to 1, the material loss defined in article master data (artikel.mverlust)
will be applied. If the switch is active and set to 2, a correction factor (artikel.kverlust) will be
applied.
The stock variant for BOM elements (wlppms.s_bitnr) is 0 by default. It can be individually
calculated via SP cu_pmewlagbitnr. The SP has to return the variant number as a SMALLINT value.
It receives eleven parameters:
INTEGER          external order number (kauf.auftrnr)
SMALLINT         internal item number (kpos.posnr)
SMALLINT         tupel number of the stock part (aufstrukt.tnr)
SMALLINT         article number of the stock part (aufstrukt.artnr)
DECIMAL         Width of the stock part (as in ALCIM pool_teile.breite to the part itself or to the
next existing parent part)
DECIMAL         Height of the bearing part (as in ALCIM pool_teile.hoehe to the part itself or to
the next existing parent part)
DECIMAL         Thickness of the stock part (see external description for determination)
INTEGER         Article number of the header part (kpos.artnr)
DECIMAL         Width of header part (kpos.laenge)
DECIMAL         Height of header part (kpos.breite)
DECIMAL         Thickness of the header part (see external description for determination)


2.8.2. Generation of remake purchase orders
The AV remake function in ALCIM allows generation of a new production item with reference to
the original order item for a remake. This item can then be planned separately. If such an item
includes purchased parts, it may be necessary to re-order these.
In this context, in AWEnterprise and AWProduction 5.1 is now a new function available that
allows you to inform the ERP system about parts that must be re-ordered. The function must be
configured appropriately.
If the function is enabled, during the generation of the remake item, the appropriate purchased
parts are marked accordingly. Depending on how the function has been enabled, a remake item
that includes purchased elements can be scheduled right away, or the item is assigned to the next
P.O. pool so that it may be necessary to wait for the elements to arrive before the item can be
scheduled.
In both cases, the purchased parts of the remake items are then visible in the purchased parts
view of the ALCIM rough planning. The context menu for the purchased part view has been
expanded to include the Remake purchase orders submenu. This submenu offers you two
operating possibilities:



A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                          131
Trigger
With this menu option, the ERP system is informed that for the purchased parts selected in the
view, orders must be triggered. Goods receipts that are then reported by the ERP system can be
booked for this item. Insofar as the function with order pot is enabled, the item is first release for
planning when all parts have been received. However, as for the original item, it is possible to
move the item into the pool using the appropriate function in the purchased parts view and to
plan it before goods receipt.
Do not trigger
With this menu option, you decide whether the purchased part is still available and does not have
to be re-ordered. Insofar as the function with order pot is enabled, the item is moved
automatically from the order pot to the pool and it can be planned.
For both functions it is ensured that they are only executed for purchased parts for remake items
(even if the selection may include parts for other items) and that a purchase order cannot be
triggered twice for a part. For security, the parts for which the functions are executed and the
parts for which execution is not possible are listed again on a dialog. Via this dialog, you can then
confirm or cancel the execution.
       If the selection includes several of the same purchased parts (if there are several remake
items for the same order item), then these parts are combined and the information of the ERP
system is done with the appropriate quantity.
Note: For a part for which the "Do not trigger" was selected, a re-order can still be triggered after
the fact if this item is not yet planned. For this, move the relevant item into the order pot so that
it is visible once again in the purchased parts view. Here, the Trigger function can be executed as
described.
In ALCIB, if the Trigger function was selected, there is a check from which supplier the purchased
part was last ordered and whether the purchase order was triggered directly or via the order
pool. The procedure for the part to be re-ordered works exactly the same way. The order date is
the date on which the Trigger function was selected. Insofar as configured, a mail is also sent that
informs about the parts to be re-ordered. This is especially useful when using the order pool so
that the re-order can be triggered promptly.
Re-orders are treated like normal purchase orders in ALCIB, for which goods receipts can also be
recorded. These goods receipts are forwarded as usual to ALCIM and noted there.
Activation in ALCIM
The function is activated via a switch on the ALCIM configuration dialog (menu option Master
Data > Configuration). It can be found globally under ALCIM > Rough planning > Settings >
Remake orders. It has the following setting possibilities:
    0. The function is not active.
    1. The function is active. During the generation of the remake item, the purchased parts are
       marked accordingly. The item is then visible in the order pool, where the decision can be
       made whether or not a re-order is necessary, and also in the rough planning view for
       planning,
    2. The function is active. During the generation of the remake item, the purchased parts are
       marked accordingly and the item is assigned to the order pot. The item is only visible in
       the purchase parts view, where the decision can be made whether or not a re-order is
       necessary. Planning of the item is only possible when all goods receipts have been
       reported or if the item was moved via the purchased parts view into the pool.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                         132
If the function should already be used with AW-Production 5.1, you must make sure that the
necessary database extension has been made. The script
awupdate_alcim_#208786_2_510_2_510.xml is available for this. It extends the table
pool_bestellteile to include the fields nachbestoffen and nachbesttodo. Here it is noted whether a
decision must still be made or what decision has been made.
Activation in ALCIB
Here it is recommended that you activate the switch AWC_NACHBEST_MANR. The switch
activates that a mail is sent that informs about parts to be re-ordered. As value, the number of an
employee must be stored, who then counts as initiator of the mail or as mail recipient if nothing
else is defined in the ALCIB mail system for the mail-ID 43.
If the function should already be available with AW-Enterprise 5.1, a database change is required.
For this, execute the script that is available on the development computers under
develop\alcib\12\1\de\install\xsql\12\1\1\120101004_awc_bestproto.sql (unless it has already
been executed with the standard update to SP1).
Participating processes
The following processes participate in the flow of this function and if necessary must be restarted
after the function has been activated:
    •   Alcim-Booking: If a remake item is generated via the remake dialog, the booking creates
        the new function and marks the affected purchased parts.
    •   ALCIM rough planning:The new menu option and the functionality for triggering the re-
        orders are then available here. In the table field pool_bestellteile.nachbestoffen there is a
        note about whether a decision was made; in table field pool_bestellteile.nachbesttodo
        which one.
        Note: It is recommended that you make a view available in the purchased parts view that
        filters only the entries with pool_bestellteile.nachbestoffen=1 . Then only the purchased
        parts can be seen for which no decision has been made.
    •   ERP-Webservice:It forwards the "Trigger" function to ALCIB and makes the appropriate
        entries for the internal order triggering or for the order pool. Insofar as configured via the
        ALCIB switch AWC_NACHBEST_MANR, the information mail is sent. That a re-order was
        necessary is noted in the table awc_bestproto, here with the identifier bruch=1.
    •   ALCIB-Exportservice and PPS-Webservice:They are responsible for the booking of the
        goods receipts.
Requirements
All participating processes must be present in the latest version and if necessary restarted in case
of new configuration.
The function is available in connection with the ALCIB-ALCIM coupling and the reporting via ERP
Webservice.
Remake orders can only be generated for purchased parts in remake items that were created via
the AV remake dialog. This applies only for such remake items that were created after activation
of the function. In already-existing remake items, the necessary marking is missing.




A+W Software GmbH         EN-CONFIG-A+W EnterpriseProductionInterface.docx                        133
2.8.3. Workflow of background processes
The following diagrams exist:


      \\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity\AngeboteWorkflow.vsd
      \\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity\AufträgeWorkflow.vs
        d




A+W Software GmbH        EN-CONFIG-A+W EnterpriseProductionInterface.docx            134

