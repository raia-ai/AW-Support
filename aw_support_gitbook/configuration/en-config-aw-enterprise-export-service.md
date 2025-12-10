---
title: "EN CONFIG A+W Enterprise Export Service"
category: "configuration"
product: "A+W Enterprise Export Service"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W Enterprise Export Service"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration   A+W Enterprise Export Service                                                                            english        A+W Software GmbH                                           - -INTERNAL-                        EN-CONFIG-A+W Enterprise Export Service.docx    1 Change history             Date          Author                  Remarks                              Version                                                 Copy of DE-           2017-05-08    SVH"
source_file: "EN-CONFIG-A+W Enterprise Export Service.pdf"
---


# EN CONFIG A+W Enterprise Export Service

         Configuration


A+W Enterprise Export Service




                                                                       english




   A+W Software GmbH                                           - -INTERNAL-
                       EN-CONFIG-A+W Enterprise Export Service.docx    1
Change history


          Date          Author                  Remarks                              Version
                                                Copy of DE-
          2017-05-08    SVH                     TU_AlcibExportService_2012.doc,      1.0
                                                modified
          2019-02-18    SVH                     P.O. modes
          2023-05-04    SVH                     Logging
          2023-05-04    SVH                     [AW-126899] - Production release
          2023-07-27    SVH                     [AW-149830] – Clean-up logic
          2024-01-31    SVH                     Troubleshooting chapter




Content

1.   Introduction                                                                           4
2.   Procedure                                                                              5
     2.1. From A+W Enterprise                                                               5
     2.2. Windows Service                                                                   5
     2.3. General functionality                                                             6
     2.4. Logging                                                                           6
     2.5. Details                                                                           6
          2.5.1. Transfer table                                                             6
          2.5.2. Internal client separation in AWP                                          8
          2.5.3. Paralleluse of ‚A+W Enterprise 5 Export Service ‘                          8
          2.5.4. Multi site capability (AWDesk #363300)                                     8
          2.5.5. Cleanup logic                                                              9
3.   Interfaces                                                                            10
     3.1. WAEINALCIM                                                                       10
          3.1.1. Activation in A+W Enterprise                                              10
          3.1.2. A+W Enterprise Export Service – settings                                  10
          3.1.3. Functions                                                                 11
     3.2. ERFSTELLENALCIM                                                                  11
          3.2.1. Multi site logic (adjustment AWDesk #344831)                              11
     3.3. GESTWAEINALCIM                                                                   12
          3.3.1. Activation in A+W Enterprise                                              12
          3.3.2. A+W Enterprise Export Service – settings                                  12
          3.3.3. Change in the incoming goods interface with AWDesk #369553/374014         12
     3.4. BESTINFOALCIM                                                                    13
          3.4.1. Activation in AWE                                                         14
     3.5. CANCELORDER                                                                      14
          3.5.1. Functions                                                                 14
          3.5.2. Limitations                                                               15


A+W Software GmbH           EN-CONFIG-A+W Enterprise Export Service.docx                        2
     3.6. PRODRELEASE                                                     15
          3.6.1. Functions                                                15
     3.7. Customer-specific interfaces                                    15
          3.7.1. ECOMCUST                                                 16
          3.7.2. ECOMSTAT                                                 16
4.   Troubleshooting                                                      17
     4.1. Export Service hangs                                            17
     4.2. Incompletely processed records in the table exportinfo          17
     4.3. Lock problems with DB accesses                                  17
     4.4. Error during export of rack receipt of goods                    17




A+W Software GmbH          EN-CONFIG-A+W Enterprise Export Service.docx        3
1. Introduction
   Web services cannot be directly addressed from A+W Enterprise. Since A+W are using Web
   services at many points for program-wide communication, we have implemented a solution
   that allows to pass on events and data from A+W Enterprise to other program's Web services.




A+W Software GmbH         EN-CONFIG-A+W Enterprise Export Service.docx                       4
2. Procedure
The database offers a new interface table filled by A+W Enterprise should transfer events occur.
Moreover, a new Windows service („A+W Enterprise 5 Export Service“) has been implemented for
polling this interface table. If a corresponding entry is found, the service selects the necessary
information from the database and passes it on to the appropriate Web services.




2.1. From A+W Enterprise
When an event occurs in A+W Enterprise which shall be passed on to a Web service, the interface
table ‚exportinfo‘ is filled.


2.2. Windows Service
The service A+W Enterprise Export Service must be started on a Windows PC. It will control the
process
    •   Using the information from its configuration file, it logs into the A+W Enterprise database.
    •   It reads the first record from the interface table ‚exportinfo‘ and checks the interface.
    •   If necessary, further information has to be selected from the database for this interface.
    •   The information is passed on to the target Web service.
    •   The record is deleted from the interface table ‚exportinfo‘ and archived in table
        ‚exportinfook‘.
This process is repeated until there are no records left in table ‘exportinfo‘. When the table is
empty, the Windows service switches to waiting mode. After a waiting time defined in the
configuration file (default: 18 seconds), the interface table is checked again for information to be
transferred. If an error occurs during the transfer, transfer is attempted again until it is successful,
or until the maximum number of transfer attempts (default: 10 attempts) has been reached.


A+W Software GmbH            EN-CONFIG-A+W Enterprise Export Service.docx                              5
2.3. General functionality
The trigger record in the table exportinfo is generated programatically by the call of the function:
        short exportinfoins_* ()
in the back end.
The current insert time stamp is transferred as "izeit".
Records with CANCELORDER interface are preferably processed by the export service. The polling
interval must be configured so that it is appropriately short.
Depending on the interface, the export service calls a PPS Webservice method or, in the case of
eCommerce, an ERP Webservice method, and receives a return value that indicates whether or
not the call was processed successfully.
Successfully processed records are transferred to the table EXPORTINFOOK, in the process the
long value from EXPORTINFO.IZEIT (insert-time) is transferred after EXPORTINFOOK.LONGWERT1,
so that records for the same order can be distinguished using the time stamp.
Records that encounter an error stop with status < 0 in exportinfo. The error code from the return
value of the Webservice method is stored as error code in the field exportinfo.fehlertext.




2.4. Logging
After expiry of the pollint time, the export service checks the interface table exportinfo for
records that are waiting for processing. If there are no records for processing, the next polling
interval is waited, etc.
If the table exportinfo contains no new records, the export service writes a message into the
export service log every 5 minutes in order to show that it is working. The log message says "Still
alive, but nothing to do."




2.5. Details
          Transfer table
Transfer table exportinfo

When the event which is to be transferred occurs, the table exportinfo is filled by A+W Enterprise,
and is processed by the Window service.
If this is successful, the record is deleted from the table. In case of an error, the record gets an
error status.
The table consists of the following fields:
            Field          Data Type          Description
            Name


A+W Software GmbH            EN-CONFIG-A+W Enterprise Export Service.docx                              6
            Interface     char(20)       Defines the information to be transferred:
                                         WAEINALCIM – goods received to A+W Production
            Izeit         Long           Time when the record was saved. Serves to define the
                                         processing sequence.
            status        smallint       1 – being processed
                                         0 – to be transferred
                                         <0 – error code:
                                          Error status           Description
                                                            -1 General error

                                                            -2 Error when selecting the purchase orders
                                                               for a BOM element of the order
                                                            -3 Error when selecting supplier information
                                                            -4 Error when loading the PPS Web service
                                                            -5 Error when selecting rack receipt
                                                               information
            fehlertext    char(100)      If status <0 error report
            fzeit         Long           If status <0 time of the failed transfer attempt
            versuche      smallint       Total number of transfer attempts
            haus          smallint       Street address
            auftrnr       integer        Document number
            vorgang       smallint       Document type
            subnr         smallint       Sub-number of the document
            shortwert1    smallint       Field for additional parameter
            shortwert2    smallint       Field for additional parameter
            shortwert3    smallint       Field for additional parameter
            longwert1     Long           Field for additional parameter
            longwert2     Long           Field for additional parameter
            longwert3     Long           Field for additional parameter
            charwert1     char(30)       Field for additional parameter


Transfer table exportinfook

Records successfully transferred by A+W Enterprise 5 Export Service will be saved in table
exportinfook for further investigation.
The table contains the fields:



A+W Software GmbH            EN-CONFIG-A+W Enterprise Export Service.docx                          7
             Field Name        Data Type      Description
             schnittstelle     char(20)       Defines the information to be transferred: See
                                              „exportinfo.schnittstelle“.
             uezeit            long           Time of the successful transfer.
             Haus              smallint       Street address
             auftrnr           integer        Document number
             vorgang           smallint       Document type
             Subnr             smallint       Sub-number of the document
             shortwert1        smallint       Field for additional parameter
             shortwert2        smallint       Field for additional parameter
             shortwert3        smallint       Field for additional parameter
             longwert1         long           Field for additional parameter
             longwert2         long           Field for additional parameter
             longwert3         long           Field for additional parameter
             charwert1         char(30)       Field for additional parameter


          Internal client separation in AWP
One Windows service can execute the transfer for several internal AWP clients. The necessary
client-specific AWE environment variables (e.g. „AWC_URL_PPS_WEBSERVICE“ for interface
„WAEINALCIM“) have to be maintained per client for this purpose.


          Paralleluse of ‚A+W Enterprise 5 Export Service ‘
It is currently impossible to run several Windows services at the same time. This extension will be
realized upon request.


          Multi site capability (AWDesk #363300)
From version v6 on, several databases can be configured in the config tool of the export service.
With internal client separation, the DB configuration can be done subclient-precisely if needed.
Polling interval and the maximum number of transmission attempts are specified across DBs.
In the service, after expiration of the polling interval for all configured and active databases, it is
checked whether trigger records are present in the table EXPORTINFO. Existing records are
worked through. The databases are checked one after another, the sequence of the checking is
arbitrary.
With subsite-precise configuration of a DB connection, only the exportinfo records are processed
that contain the configured subsite in EXPORTINFO.HAUSNR.




A+W Software GmbH            EN-CONFIG-A+W Enterprise Export Service.docx                                 8
         Cleanup logic
Previously the AWE Export Service was missing the logic for cleanup of the tables exportinfo and
exportinfook.
Since the PO transfer to AWP is configured for most customers, over time, many transfer records
are created and as many records in the ok table.
With the Config tool, it is possible to store the number of days for which the records with error
status in the transfer table exportinfo or successfully processed records in the archive table
exportinfook should be kept. If the period has elapsed, the records are deleted.
The default retention time for successfully processed records in the table exportinfook is 100
days. The value from exportinfook.uezeit is used as reference time.
The default retention time for faulty records in the table exportinfo is 200 days. The value from
exportinfo.fzeit is used as reference time.
A configuration of "0" days is possible in the Config tool, but it is intercepted by the program. In
this case, the records are deleted after 365 days.
It is not recommended that you set the retention time for faulty records to a value < 30 (days).
The records may be required for any error research.
See PF [AW-149830].




A+W Software GmbH            EN-CONFIG-A+W Enterprise Export Service.docx                              9
3. Interfaces
Follows a list of already implemented interfaces.


3.1. WAEINALCIM
This interface reports goods received in A+W Enterprise via PPS-Webservice to A+W Production.
This function is part of the new A+W Enterprise-A+W Production link (AWDesk #129902). Not only
the data of newly entered goods received will be transferred but amendments and cancellations
will be passed on to A+W Production as well.
Here's the figure:




         Activation in A+W Enterprise
This interface is enabled in A+W Enterprise by means of the environment variable
„AWC_WAEIN_UEBERMITTLUNG“. If it is set, every receipt of goods will result in an entry in the
interface table Exportinfo.


         A+W Enterprise Export Service – settings
The A+W Enterprise Export Service requires the URL of the PPS Webservice to pass on the
information. These are loaded from the environment variable „AWC_URL_PPS_WEBSERVICE“.


A+W Software GmbH           EN-CONFIG-A+W Enterprise Export Service.docx                         10
         Functions
As soon as a change is made to the PO and saved, a corresponding record is written to the table
exportinfo.
Caution: Changing the PO quantity of a PO with order reference is not suppressed in A+W
Enterprise. A change of the PO quantity creates a record in the table exportinfo, and thus for
further processing by the export service and forwarding to the PPS Webservice.
The changed PO quantity is not processed further in the PPS Webservice, however. There is NO
adjustment of the PO quantity in A+W Production. PO quantities in AWP can only be adjusted
with a new OrderXML transfer of the order.




3.2. ERFSTELLENALCIM
This interface does not serve to transfer information to external systems but selects the
registration points defined in A+W Production and saves them in A+W Enterprise table
“awc_alcimerfstellen“. The registration points are required for entering rack-related receipt of
goods (#144075).
To address this interface, enter a record - including the above interface name and the required
client number - in the interface table. This can be done just once or, in order to keep the A+W
Production and A+W Enterprise data consistent, in regular intervals, e.g. by means of an CRON
job.
The SQL is:
insert into exportinfo(schnittstelle,haus) values ('ERFSTELLENALCIM',<MANDANT>)

The registration points are selected via PPS Webservice. This is why the environment variable
„AWC_URL_PPS_WEBSERVICE“ must be set for this interface.
The environment variable AWC_ALCIMERFSTELLEN_TYP can be used to limit the registration
points to be transferred.


         Multi site logic (adjustment AWDesk #344831)
The insert is: insert into exportinfo(schnittstelle,haus, shortwert1) values ('ERFSTELLENALCIM',<
SITE >, <SITE-FLAG>)
The determination of the registration points can be limited in the registration point types. The
limitation is placed via the env variable AWC_ALCIMERFSTELLEN_TYP. The type entries in the env
variables must be numeric and separated with commas.
SITE specifies the env variables AWC_URL_PPS_WEBSERVICE and AWC_ALCIMERFSTELLEN_TYP.
They can be defined company-specifically, so that it is possible via various PPS Webservices to
determine registration points from different production systems for different registration points.
SITE also supplies the HAUSNR, which is written to AWC_ALCIMERFSTELLEN if the determination
of the registration points should be made precisely for the company (see SITE-FLAG).



A+W Software GmbH           EN-CONFIG-A+W Enterprise Export Service.docx                            11
SITE FLAG = 1 indicates that all registration points determined company-specifically should be
written to AWC_ALCIMERFSTELLEN.
The table AWC_ALCIMERFSTELLEN has been expanded by field HAUSNR.
If SITE FLAG != 1 the company number is filled with 0 (single-site logic).
If the export service does not receive any registration points from PPS, the current entries in the
table AWC_ALCIMERFSTELLEN remain untouched.
If the PPS Webservice provides at least one registration point, the content of
AWC_ALCIMERFSTELLEN is deleted completely and the new data record(s) are inserted.


3.3. GESTWAEINALCIM
Similar to the interface described in chapter 3.1, this interface transfers goods received to A+W
Production. While the interface described in chapter 3.1 transfers goods received which are
entered automatically or by hand, this interface transfers rack-related goods received (#144075).
Here, the information on the quantity received for a BOM element of a certain order is completed
by the rack and registration point on which the sheets can be found.


         Activation in A+W Enterprise
This interface is enabled in A+W Enterprise by means of the environment variable
„AWC_WAEIN_UEBERMITTLUNG“. If it has been set, booking of rack-related goods received will
result in an entry in the interface table “exportinfo“.


         A+W Enterprise Export Service – settings
The A+W Enterprise Export Service requires the URL of the PPS Webservice to pass on the
information. These are loaded from the environment variable „AWC_URL_PPS_WEBSERVICE“.


       Change in the incoming goods interface with AWDesk
     #369553/374014
         Available      AWE Export           ERP                 PPS               AWP
         in version     Service              Webservice          Webservice
         5.5            A+W                  from 2016-06-       from 2016-06-     from 2016-
                        Enterprise           21                  21                06-21
                        v12.5 setup
                        12.5.1286
         6.0            A+W                  from 2016-06-       from 2016-06-     from 2016-
                        Enterprise           21                  21                06-21
                        v13.0 setup,
                        from, 2016-06-
                        21



A+W Software GmbH            EN-CONFIG-A+W Enterprise Export Service.docx                         12
         from           always               always             always              always
         update 6.1


For the transfer of order and incoming goods information for remakes from AWE to AWP, there
was the problem that the AWP production item could no longer be assigned unambiguously to an
order/IG information from AWE.
With the current version, the AWP production item is transmitted to the ERP Webservice when
triggering a remake order. Then the export service transfer the production item for order and IG
information back to the PPS Webservice, which means that the assignment can be made
unambiguously in AWP.
The logic was realized through the provision of a new PPS Webservice method:
RefreshPurchaseInfoExt()
And a new ERP Webservice method: TriggerPurchaseExt()
Within AWE, the production item is guided through in the DB field "plfdpos" from the order
generation to the order to the IG.
bestwun.plfdpos -> bestpool.lfdpos -> intbest.plfdpos -> bpos.plfdpos
CAUTION:
In rack-related incoming goods, previously no Ext method was made available in the PPS
Webservice (it then had to be called RefreshPurchaseInfoRackExt()) in order to be able to transfer
the production item there.
In the Export Service, the data is already ready for transfer, so that the effort to implement the
transfer is low (approx. 2 h).


3.4. BESTINFOALCIM
Transfer of purchase information, see AWDesk #318644
The purchase order information for an order was previously only reported to A+W Production
with the first incoming goods.
From now on, each update of the order is forwarded to the production system.
Updated data will be transferred:
    •   after the purchase order generation
    •   after a change of a purchase order
    •   according to Avision / confirmation of the purchase order date
    •   after cancellation of the purchase order
    •   after renewed import of an order with the status processing of the status 551 in rserv.
        The record is only described for MODUL_PROD_SPAETE_AENDERUNGEN.


The mode of P.O. information is transferred in field exportinfo.shortwert1. Possible values:
 Mode            Description



A+W Software GmbH           EN-CONFIG-A+W Enterprise Export Service.docx                             13
 0                 Purchase order generation
 1                 Change P.O.
 2                 Purchase order release
 3                 Reset P.O.
 4                 Cance P.O.



          Activation in AWE
This interface is enabled in AWE by means of the environment variable
„AWC_BEST_UEBERMITTLUNG“.


3.5. CANCELORDER
Transfer of an order cancellation to AWP, see AWDesk #363300
Activation of this logic is not necessary.


          Functions
The trigger record in the table exportinfo is generated programatically by the call of the function:
short exportinfoins_cancelorder(long auftrnr, short vorgang, short subnr, short haus, long izeit)
in the back end.
The current insert time stamp is transferred as "izeit".
Records with the new interface are preferably processed by the export service (caution!) The
polling interval must be configured so that it is appropriately short.
The Export Service calls the new PPS Webservice method "OrderDeleteEx2(int orderno, bool
deleteOrderXML)" and receives a return value that indicates whether or not the order
cancellation was executed successfully in AWP:
     •   Return value > 0 indicates that the cancellation was executed successfully.
     •   The value -1 indicates that the action could not currently be executed due to content
         problems (e.g. OrderXML is being imported now).
     •   The value -2 indicates that the order was neither found in the database nor as OrderXML.
     •   The value -3 indicates that there are technical problems (e.g. DB connection problem,
         program error).
Successfully processed records are transferred to the exportinfook table, in the process the long
value from exportinfo.izeit (insert-time) is transferred to exportinfook.longwert1, so that records
for the same order can be distinguished using the time stamp.
Records that encounter an error stop with status < 0 in exportinfo. The error code from the return
value of the method is stored as error code of the method OrderDeleteEx2() in the field
exportinfo.fehlertext.


A+W Software GmbH               EN-CONFIG-A+W Enterprise Export Service.docx                        14
          Limitations
The new PPS Webservice method OrderDeleteEx2() is available in the PPS Webservice starting
with version 13.04.1330. If the Export Service determines that the PPS Webservice is not
sufficiently current, an exception is thrown. The record to be processed then remains with
status=1 in the table exportinfo.




3.6. PRODRELEASE
Transfer of the production release for an order to AWP after the order was previously transferred
to AWP via the OrderXML interface with type "Cost calculation + reservation".
See PF [AW-126899].
No activation of the logic is required.


          Functions
The trigger record in the table exportinfo is generated programatically by the call of the function:
         short exportinfoins_prodrelease(long auftrnr, short vorgang, short subnr, short haus, long
izeit)
in the back end.
The export service calls the new PPS Webservice method "int PublishTemporaryOrder(int auftnr)"
and gets a return value that indicates whether or not the production release was successful in
AWP (shifting from temporary order pot (12800) into the pool):
    •    Return value > 0: release successful.
    •    Value -1: The database connection to the AWP database could not be established right
         now.
    •    Value -2: The order is currently locked in AWP. This should be impossible for an 12800
         order, but it is checked for the sake of completeness.
    •    Value -3: Another exception occurred. For more precise info about problems, see the
         PPSWebservice trace file.




3.7. Customer-specific interfaces
With AWDesk #368340, an eCommerce interface is implemented (at customer request). For
description and configuration of the interface, see \\jupiter\Doku_DocuWare\ALCIB-
PMS\EXPORTSERVICE\User_Manuals\SGGS-eCommerceMyGlassolutionsEnterpriseInterface-
SGGPARIS-368340.docx




A+W Software GmbH            EN-CONFIG-A+W Enterprise Export Service.docx                         15
       ECOMCUST
See AWDesk #368340


       ECOMSTAT
See AWDesk #368340




A+W Software GmbH    EN-CONFIG-A+W Enterprise Export Service.docx   16
4. Troubleshooting
4.1. Export Service hangs
Eliminated with build Version 13.04.8527 (QR 22/06):
In case of a database error, starting now the transaction is reset, since previously there was a lock
in particular scenarios that could only be eliminated with a restart of the service.
See [AW-64518].




4.2. Incompletely processed records in the table
   exportinfo
Eliminated with build version 13.04.9190 (05/23):
In the Export Service, there could be lock problems, the consequence of which was that records
with unclear processing status lay in the table exportinfo.
See [AW-143284].




4.3. Lock problems with DB accesses
Eliminated with build version 13.04.9272 (06/23):
In the Export Service, there were previously lock problems with various database accesses. Thanks
to a basic reworking of the Export Service, this problem should no longer occur.
See [AW-144637].




4.4. Error during export of rack receipt of goods
Error message from the PPS Webservice can be found in the log of the AWE Export Service:
…
Exception occured while calling PPS-Webservice: System.Web.Services.Protocols.SoapException:
Server was unable to process request. --->
Albwir.Basis.Database.AWDatabaseRowNotFoundException: Could not find any data in DB.
ParaNames (@auftnr, @posref, @upos, @teilenr); ParaValues (…); SQLCommand: select distinct
awbar_teile.etikettnr, awbar_teile.pos from pool_bestellteile, awbar_teile, awbar_bearbeit,
bearbeitstamm where pool_bestellteile.auftnr = awbar_teile.auftnr and pool_bestellteile.pos =
awbar_teile.pos and pool_bestellteile.u_pos = awbar_teile.u_pos and pool_bestellteile.teile_nr
>= awbar_teile.teilenr_min and pool_bestellteile.teile_nr <= awbar_teile.teilenr_max and
awbar_teile.etikettnr = awbar_bearbeit.etikettnr and awbar_bearbeit.art_nr =


A+W Software GmbH           EN-CONFIG-A+W Enterprise Export Service.docx                           17
bearbeitstamm.artnr and bearbeitstamm.typ in (…) and pool_bestellteile.auftnr = @auftnr and
pool_bestellteile.posref = @posref and pool_bestellteile.u_pos = @upos and
pool_bestellteile.teile_nr = @teilenr and awbar_bearbeit.fertig = 0 and awbar_teile.bruch_flag =
0 and awbar_teile.etikettnr not in (select distinct unitbc from awbar_booking where status = 0
and station = 'PPS_WEB' and unitbc > 0) order by awbar_teile.pos asc, awbar_teile.etikettnr asc
at Albwir.Alcim.DataService.DataService.RefreshPurchaseInfoRack(String rack, Int32 esnr, Int32
lagerplatz, PurchaseInfo[] purchaseInfos)
…
Solution:
With the statement (see error message), all available labels are searched for in AWP that belong
to the order, item, and part. Available are all labels whose goods receipt is not yet booked. If the
goods receipt was already booked with a ToolTV, the labels are no longer available. Then
"awbar_bearbeit.fertig = 0" is the condition due to which no data can be found.
See PF [AW-203046].




A+W Software GmbH           EN-CONFIG-A+W Enterprise Export Service.docx                           18

