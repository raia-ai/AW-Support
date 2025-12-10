---
description: "EN-CONFIG-AW_Enterprise_Production_Interface"
---


# A+W Configuration Instructions
# A+W Enterprise 6 Production Interface
**english**

**- -INTERNAL-**

**A+W - Software for Glass**

---
## Change history
| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2013-03-14 | PG | #314985: Ignore kmodparam.refflag for whole glass systems. New section „Ganzglasanlagen und Modelldaten" | 2012.1_13 |
| Bearbei | PG | #288831: Evaluation of AWC_ANGEBOT_DEF_TERMIN to determine the default date for quotations without appointment specification. | 2012.1_12 |
| 2013-11-15 | PG | #278789: If switch MODUL_DOPPELSCHICHT is active, all installation positions at lower levels are evaluated in a simple glass hierarchy. | 2012.1_11 |
| 2013-11-05 | PG | #292040: New section <ORDER - USER_DEFINED_EXTENSIONS - UDXAWORDERINFOS - ERP_INFOS> | 2012.1_10 |
| 2013-08-22 | PG | #267331: DB field name macroname is now file name. DATEI_REF_PFAD replaces also SN_MAKRO_BASISPFAD and SN_MOTIV_BASISPFAD | 2012.1_9 |
| 2013-08-01 | PG | #280668: Treatment of sting fields, that are NULL. Patch 5.2 #201980: New processing type 1910 surface macro. #267331: Additional motif parameter for surface processings 1200, 1205, 1210, 1215, 1220, 1225. Patch 5.2 #201980: New processing type 1910 surface macro. #267331: Additional motif parameter for surface processings 1200, 1205, 1210, 1215, 1220, 1225 | 2012.1_8 |
| 2013-07-09 | PG | Due to #281878: Explicit spacer geometries (steps/back cuts) can also be transferred if variable ISO_RAHMEN_MODELL is set (not only for MODUL_VERSIEGELUNGSTIEFE) | 2012.1_7 |
| 2013-05-23 | PG | Due to #274633: SP cuxmltransfer can prevent that an order is transferred (see chapter 0 „Übergabe verhindern"). Due to #289718: For processings with <...PROCESSING - side> is filled with the layer information | 2012.1_6 |
| 2013-04-10 | PG | Due to #276862 Correction 1.8 „Anhang: A+W-Bearbeitungstyp-Informationen": Processing parameter A/B for corner processings exchanged. | 2012.1_5 |
| 2013-03-22 | PG | Declaration of performance number was transferred as item text (due to AWDesk 274142) | 2012.1_4 |
| 2013-03-05 | PG | Disable item split extended in chapter 1.4.7 „Positionssplit" (due to AWDesk 275242) | 2012.1_3 |
| 2013-02-26 | PG | 0 „XSD-konforme OrderXML-Dateien" (due to AWDesk 251817) | 2012.1_2 |
| 2012-11-30 | PG | Notes regarding processing type 1900 (due to AWDesk 264532) | 2012.1_1 |
| 2012-10-25 | PG | Original edition for version 2012.1 (AWDesk 199448) | 2012.1 |
| 2017-11-01 | SVH | Internal client separation | 6 |
| 2017-01-15 | RS | Change of site allocation in the order | |
| 2018-05-14 | SVH | Weight of main and sub parts | |
| 2018-05-16 | RS | Feedback chapter extended | |
| 2018-05-17 | RS | Status allocation rack feedbacks | |
| 2018-05-23 | SVH | Cost centers / Cost calculation | |
| 2018-06-04 | RS | PMVERSANDSTEUER and AWC_GESTZU_BUCHEN_OHNE_VERPACKTMELDUNG | |
| 2019-06-17 | SVH | Adjustments to the extended workbench (AWDesk #438718) | |
| 2019-07-22 | SVH | New adjustments to the extended workbench (AWDesk #438718) | |
| 2019-08-26 | SVH | Description AWC_ERPDOC_FILE | |
| 2019-10-02 | SVH | Adjustments to the extended workbench (AWDesk #451780) | |
| 2019-11-21 | SVH | UV protection (awtyp 1650) (AWDesk #454284) | |
| 2019-11-28 | SVH | Other articles (atyp 999) (AWDesk #454469) | |
| 2020-04-03 | SVH | Addition to meta elements with extended workbench | |
| 2020-05-06 | RS | Bestewun lock logic + UPDATE_KAUF_BEI_BEST added | |
| 2020-07-20 | RS | AWC_IGNORE_AWERACKSTATUS added | |
| 24.07.202 | RS | Flow for rack bookings: (#459400) | |
| 2020-09-21 | SVH | Distinction of configured and non-configured processing parameters (AWDesk #456954) | |
| 2021-11-26 | SVH | Restructuring of the section "Customized information" | |
| 2022-02-09 | SVH | Addition in the "Weight of main and sub parts" section | |
| 2022-07-20 | SVH | System diagram | |
| 2022-11-02 | SVH | Adjustment of the chapter division "Elements information" and "Processing information" each have their own subchapter (level 2). | |
| 2022-11-10 | RS | Reservation resolution with XTV report | |
| 2023-05-05 | SVH | Cost calculation + reservation - [AW-126899] | |
| 2023-09-13 | SVH | [AW-142005] - Logical and physical machine in the cost calculation | |
| 2023-10-17 | SVH | [AW-159250] – Logic ORDERXML_PROCPOSTDEF_LEVELDOWN_MODE | |
| 2024-07-22 | SVH | Docu ORDERXML_POSTPROCTHERMAL_ON_TVG | |

# 1. System diagram

**Systemarchitektur A+W Enterprise - A+W Production**
In diesem Schaubild sind die an der A+W Enterprise-A+W Production-Integration beteiligten Prozesse sowie deren Interaktionen aufgelistet.

*A diagram shows the system architecture for A+W Enterprise and A+W Production. On the left is "A+W Enterprise - Entwicklung" with a database and several processes (ALRPC Dienst, A+W Enterprise OrderXML, A+W Enterprise Export). On the right is "A+W Production - Entwicklung" with its own database and processes (A+W Production, A+W ALCIM Items4ALCIM, A+W ALCIM Booking Engine). The two systems communicate through a central "Import - Verzeichnis" and two web services (ERP Webservice and PPS Webservice). Data flows between components like OrderXML files, scheduling commands (CompleteScheduling), and status updates (SetOrderStatus).*

Further system/process diagrams can be found in
\\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity

# 2. Transfer to OrderXML

## 2.1. General Information
This document describes the general process of creating OrderXML files based on ALCIB information. This document requires knowledge of the internal processes and data structures in ALCIB (A+W Enterprise 5). This document is therefore meant only for project engineers, not for customers.

OrderXML files are used to transfer order/quotation data to other systems by means of a defined interface. This version (available on the basis of A+W Enterprise 5 (ALCIB 2012.1)) allows to transfer the order and quotation data to a production system, e.g. ALCIM.

The transfer to ALCIM necessitates ALCIM-Capacity. This replaces PMS and the direct data import into ALCIM completely.
This is the basis for information which will be found in the OrderXML files and also for the information gathered by means of direct data import. All data are directly loaded from A+W Enterprise 5 (ALCIB), not from PMS.
This document also handle the subject of data gathering.

**Terminology**: OrderXML files can be created for orders as well as for quotations if configured accordingly. To simplify matters, we are going to use only the term 'orders' while meaning both orders and quotations. We will draw your attention to any distinctions should they be necessary.

Creating OrderXML files for purchase orders is a special feature however which shall be dealt with in a separate chapter.

### 2.1.1. Amendments compared to the previous version
This chapter briefly lists the main amendments as compared with the previous version, 2011 (3.6).

- The A+W Enterprise 5 OrderXML service is based on ALCIB database version 2012.1.
- The service's configuration tool automatically makes the necessary Informix Setnet entries. The ODBC data source is set up at the same time.
- If a patch is installed within this version, a previous uninstallation of the service is no longer necessary; provided the service is installed via the A+W-Setuplauncher.
- AW processing type 1900 (SN macro) can be imported
- The switch **PMEHANDLE_GERADE_EP** is assumed to be active by default so that the BOM below an element with an even assembly position will be transferred in reverse sequence.
- **ORDERXML_VERSION="5.0"** indicates that ALCIM can validate the OrderXML file; it is XSD compliant. Requires current ALCIM and current OrderXML service (ID 12.1.2).
- The item split based on the kposgest data can be switched off using the switch **ORDERXML_IGNORIERE_KPOSGEST** (from version ID 12.1.3).
- The AW processing type 1910 (SN surface macro) can be used, provided ALCIM and ALCIB are from service pack 5.2 (from version ID 12.1.8, switch ORDERXML_VERSION must be set to "5.1").
- Transfer of SN motif parameters for processing types 1220, 1205, 1210, 1215, 1220, and 1225, provided ALCIM and ALCIB are from service pack 5.2 (from version ID 12.1.8, switch **ORDERXML_VERSION** must be set to "5.1").
- Section `<ORDER - USER_DEFINED_EXTENSIONS - UDXAWORDERINFOS - ERP_INFOS>` will now be filled. This means for the transfer to ALCIM, that a user and an entry date are transferred to ALCIM (available as of version ID 12.1.10).
- Up to now, the current date was transferred for quotations without an appointment specification. To avoid a general shift in A+W Capacity, today's date plus 14 days will be transferred in the future. Switch **AWC_ANGEBOT_DEF_TERMIN** can be used to define a different number of days (available from version ID 12.1.12).

### Information on Version Changes
If the ALCIB version is 2012.1, the OrderXML service should be updated as well in order to use all new functions. If this is impossible for internal reasons, OrderXML service version 2011 can still be used but new functions may be missing. On the other hand, the OrderXML service version 2012.1 **cannot** be used in connection with a lower ALCIB version because of the changed structures in ALCIB which are completely supported by the OrderXML service.

### 2.1.2. Information about previous versions of A+W Enterprise OrderXML 6
The documentation for the versions before A+W Enterprise OrderXML 6 (for example, version 2011/4.5) can be found here: `\\jupiter\Doku DocuWare\Interfaces\OrderXml\AusAlcib`

## 2.2. Process Overview

*A simple diagram shows the general process. An "ALCIB Datenbank" (database process) sends data to the "ALCIB OrderXML" (Windows service). This service generates an "OrderXML" file and places it in an "Ausgabeverzeichnis" (output directory).*

### 2.2.1. In ALCIB
After an order or quotation is changed in ALCIB, a record with the order number is written in transfer table **ottransfer**.
The table is a mere transfer table. This means the entries just say that an OrderXML has to be created for a certain order number.

### 2.2.2. Windows Service
On a Windows PC, the service A+W Enterprise 5 OrderXML must be started. This service takes over the control.

- It checks if there is an order ready to be processed. If so, information is loaded from the ALCIB tables and compiled in OrderXML format.
- The Windows service saves this information in an OrderXML file.
- Successfully processed, the order record is deleted from the transfer table or, in case of an error, the record is marked by an error status.

This process is repeated as long as there are orders to be processed. If no order left to be processed, the Windows service switches to waiting mode. After a - configurable - wait, the service checks again whether there are orders to be processed.

The OrderXML service directly imports from the ALCIB database. For reasons of performance, it should therefore be installed on the server of the ALCIB database. Please also note that the OrderXML service needs writing rights to write the files. Access rights to the target directory must not be switched off by the Firewall.

### 2.2.3. Details

#### Transfer Tables
So far, just one transfer table has been mentioned. Actually, there have to be three tables which have to be filled to guarantee the running of the process. These are:

- **Ottransfer**: This is the actual transfer table which defines the orders for which OrderXML files have to be created.
- **Ottranssav**: Serves for internal control of order cancellations. An order cancellation does not have to be transferred for instance if the order had not been transferred. In connection with internal site separation, the program notes the number of the site that was the last to receive the order.
- **Ottranszus**: ALCIB can provide the OrderXML service with additional information.

The following sub-chapters describe the tables in detail.

#### Transfer table ottransfer
The table **ottransfer** is a global transfer table which is now also used for the OrderXML functions. An entry in this table informs the OrderXML service of the orders for which a OrderXML files shall be written.

If this is successful, the record is deleted from the table. In case of an error, the record gets an error status.

The table consists of the following fields:

- **Ordno**: Number of the quotation or order
- **Document**:
    - 5 if the document is an order
    - 4 if it is a quotation
- **Interface**: Defines the interface for which this entry is meant. Orders for the OrderXML interface are marked by the text, 'ORDXML'.
- **Control flag**: Processing status:
    - **0**: ready for processing
    - **1**: being processed
    - **400**: Data completely read, Windows service to create the file
    
    **Statuses over 400 indicate an error:**
    - **401**: Error while selecting from table kauf
    - **402**: Error while selecting from table kpos
    - **403**: Error while selecting from table kposp
    - **404**: Error while selecting from table kposgest
    - **405**: Error while selecting from table aufstrukt
    - **406**: Error while selecting from table kspross
    - **407**: Error while selecting from table poszu
    - **408**: Error while selecting from table kmodparam
    - **409**: Error while selecting from table kstufparam
    - **410**: Error while selecting from table ksprpar
    - **411**: Error while selecting from table kaufref
    - **412**: Error while selecting from table ktechw
    - **413**: Error while selecting from table ottranssav
    - **414**: Error while selecting from table ottranszus
    - **433**: Error while selecting from table alsysinfo
    - **434**: Error while selecting from table modelle
    - **435**: Error while selecting from table xfarbe
    - **436**: Error while selecting from table xxfarbe
    - **437**: Error while selecting from table artvermass
    - **438**: Error while selecting from table xsprzu
    - **439**: Error while selecting from table route
    - **440**: Information status: For purchase orders, the "customer number" must be specially determined. If this does not work, the OrderXML file will still be created. The customer information has to be checked though.
    - **458**: Can only happen if items with supply type 'none' shall not be transferred. For orders which include only items with supply type 'none', no OrderXML file will be created. The order will be marked by this number.
    - **459**: Error while compiling the item data
    - **460**: Program error while compiling the data for the node ORDERType and following.
    - **461**: Program error while compiling the data for the node ORDER_INFO and following.
    - **462**: Program error while compiling the data for the node ORDER_ITEM_LIST and following.
    - **463**: No items found to be transferred.
    - **464**: Program error while compiling the data for the node ORDER_ITEM and following (e.g. wrong supply type (included) for the main article).
    - **465**: Program error while compiling the BOM data (e.g. wrong data in aufstrukt; tnr > 999).
    - **466**: BOM of an item is blank
    - **467**: Program error while compiling the data for elements
    - **468**: No elements found in the BOM
    - **469**: Program error while compiling the data for processing steps
    - **470**: Invalid supply type
    - **471**: Cancellation information not transferred because there has been no transfer before. This status serves for information only and is actually no error.
    - **472**: The array that shall take the BOM data, the relevant elements, and their processing steps, is too small. This program error must be passed on to development.
    - **496**: Transfer completed, but the note in ottranssav could not be made.
    - **497**: OrderXML service failed to serialize the compiled data for file creation.
    - **498**: Windows service could not write the reported data in a file (possible reason: disk full).
    - **499**: Updating the control flag failed.

- **Filltime**: Time stamp which shows when ALCIB has submitted the order for processing.
- **Serno**: Orders are generally processed in Filltime sequence. This field can be used to influence this sequence. An entry with a higher Serno has priority over an entry with a lower Serno. AWE prioritizes by default: Rush orders have top priority, and standard orders have priority over orders which are only transferred for cost calculation purposes. These rules can be customized however by means of the SP cu_orderxmlpriori (see chapter "Activation in ALCIB").
- **Serviceid**: In case of redundant systems (there are several computers with OrderXML service), a service uses its unique ID to reserves the order it has been processing. Simultaneously running services realize that they must not process this order. The "unique ID" for an OrderXML system can be configured in the Windows service configuration file. The entry in the transfer table can also be made directly with a configurable ID (see chapter "Parallel OrderXML Systems").

**Error status in the control flag?**
If the field steuerflag has a status of over 400, this denotes an error. For detailed analysis, the trace level of the OrderXML service (switches **Albwir.Alcib.AlOrderXMLService** and **Albwir.Alcib.Basis**) must be raised, and the Windows service must be rebooted. The order in question has to be resubmitted by setting steuerflag is set to 0 for the order by manual update to table **ottransfer**. If the order status after repeated processing is again over 400, it is possible to search for "error" entries in the OrderXML service.

#### Transfer table ottranssav
By means of table **ottranszus** ALCIB can provide the service with additional information for which the service would have to be provided with complex definition mechanisms otherwise. These are e.g. the width and height of the surrounding rectangle for shape records for which the shape files would be required. Extensions are possible. The table is structured as follows:

- **Ordno**: Number of the quotation or order
- **Document**: 5 if the document is an order, 4 if it is a quotation
- **Posnr**: Item number. Depending on the type or the contents of the record, this information can show the internal item number or the BOM header number.
- **Eno**: If information on a certain element or a certain processing step is listed, this field shows the tupel number of the article in the BOM.
- **Typ**: Tells the OrderXML service the type of data used for this record. Currently valid:
    - **1**: = Shape data
    - **2**: = Informs the OrderXML service that this order is transferred only for cost calculation. The entry will be deleted once the order has been released (see chapter "OrderXML transfer just for production cost calculation").
    - **3**: For purchased elements for which no supplier was entered in the order, the standard supplier is determined and noted here. Downstream programs (Capacity, P.O. creation) can easily access this.
    - **4**: = scheduling
    - **128**: = cost calculation + reservation - [AW-126899], description in special chapter
- **Serno**: Several records may have to be transferred for one piece of information. In this case, this field defines the sequence in which the OrderXML service must read the data.
- **Shpno**: Shape number
- **Width**: Width
- **Height**: Height
- **Edges**: Number of edges of the present shape that can be processed.
- **Date**: Preparation for the transfer of special dates. E.g. earliest purchase date or similar.
- **Filler**: For extensions.

#### One Service per site (independent DBs, sites)
The term **sites** is chosen on purpose because a distinction has to be made here between internal clients and external clients.

With **internal site separation**, all sites are in the same ALCIB database. For the service, this is **a** site. The OrderXML files are saved in separate sub-directories in this case, based on the order's site number. No additional configuration is required.

**Several sites** are different ALCIB databases. A separate OrderXML service (installed on different computers) is required per site.

#### Several Orders at Once
So far, the description assumed that the process is executed by order. This is the standard. The process can be configured so that the service gathers the information for several orders at once. The advantage of this configuration is that the service can remember data for determining several orders.

Please note that lots of data have to be kept in the memory for this function. If more memory is used than is available, this will result in an error. Also, it will take longer until the first OrderXML file is available because all information has to be gathered before the files for the relevant orders can be written.

The number of orders to be gathered can thus be configured. The number should be matched to the customer's requirements.

> **Note**: The configuration that a certain number of orders has to be gathered at the same time is of course not mandatory; the system does not wait until this requirement is met. If less orders are available, the available ones are processed and the system correctly realizes that there are no more orders at present.

#### Cancelled orders
OrderXML files are also written for cancelled orders. But only if this is necessary, i.e. if the order had already been transferred. This is detected based on the data in table **ottranssav**. If this table shows a line for the order, this means that it has been transferred and the cancellation must be transferred as well.

After cancellation, the record is deleted from table ottranssav.

#### Change of site in connection with internal site separation
If ALCIB uses internal site separation, it needs to be checked if the site which is to produce the order has been changed since the last transfer. In table **ottranssav**, the OrderXML service does not only note whether an order has been transferred, but also the receiving site.

Before every transfer, the noted site number is compared with the current site number in the order. If this has changed, two OrderXML files are written: The first one is used to cancel the order at the original site and the second is the actual file for the transfer to the right production site.

Relevant for determining this is the field **hausnr** in table **kauf**.

> **Note**: This is an internal process during which the OrderXML service notes the progress in the transfer tables. This is why the data in the transfer tables must not be manipulated as long as the order is being processed (discernible by ottransfer.steuerflag>0 and <401).

#### Parallel OrderXML Systems
OrderXML files in ALCIB can be written by several OrderXML services at once. This option can be used:
- **For fail safety**: If one of the computers on which an OrderXML service is installed fails, further OrderXML files will be written by a second, redundant system.
- **Load distribution for big sites**: If the data volume is very large, the systems share the task of creating OrderXML files; orders are sooner available in the production system.

The following requirements must be met:
- For every OrderXML service there must be a separate computer on which the Windows service is installed.
- OrderXML files should be saved by all OrderXML services in the same directory to guarantee the transfer sequence to the target system.
- Every OrderXML service must be allocated a **unique service ID** by means of appropriate configuration.

The unique service ID permits to reserve orders in the transfer table for a certain OrderXML system. As long as an order is processed by one OrderXML service, it cannot be accessed by any other OrderXML service.

With regard to fail safety please note: If one OrderXML service fails during the write process, it may happen that the current order remains locked. In this case, a manual update of the **serviceid** in transfer table **ottransfer** to 0 is required (for all entries for this order).

#### Definition of the reading service
The system can be configured so that even ALCIB - which presents the order - decides which OrderXML service is going to process the order. This can be useful if the distribution of load shall be influenced. Configuration is made by creating the SP **cu_orderxmlservid**. This SP receives two parameters:
- **INTEGER**: Order number (kauf.auftrnr)
- **SMALLINT**: Document type (kauf.vorgang)

It has to return a **SMALLINT** value. The value returned by the SP must be the ServiceID allocated to the relevant OrderXML service.

#### If an error occurs while the OrderXML file is created
If an error occurs while an OrderXML file is created, this is noted with a code in field **steuerflag** in table **ottransfer**. A notification can be sent by email as well. If the OrderXML file interface is used in connection with ALCIM Capacity (if **AWC_ALCIM_ANBINDUNG** is set), an error status is also noted in ALCIB for the document in question.

To dispatch an email telling the user that the OrderXML file could not be created, please enable the following switches in ALCIB:
- **ORDERXML_MESSAGEMANR**: Define a user number to be treated as the initiator of the message.
- **AWC_ALCIB_SERVER_NAME**: The ALRPC background process in ALCIB is ordered to dispatch the message. To address it, enter the name of the server on which the ALRPC process is run.
- **AWC_PORT_CONTROL_SERVER**: The ALRPC background process in ALCIB is ordered to dispatch the message. This switch needs the socket port number of CTRL_SERVER.
- **AWC_PORT_RPC_DIENST**: The ALRPC background process in ALCIB is ordered to dispatch this message. This switch needs the socket port number of ALRPC.

#### OrderXML service waiting for order lock
After transfer to production from ALCIB, the OrderXML service will wait for the number server lock to be removed before creating a new OrderXML file. This is standard behavior but can be switched off.

The following switches must be active and set to enable the waiting for the number server lock:
- **AWC_ALCIB_SERVER_NAME**: Name of the computer on which the ALCIB background processes are run.
- **AWC_PORT_NR_SERVER**: Port number of the number server.

To switch off the wait, activate the switch **ORDERXML_SPERRMODUS** and set it to '1'.

## 2.3. Installation and configuration
The elements to be installed for this interface are described in detail in a separate document `\\Jupiter\doku docuware\Interfaces\OrderXml\AusAlcib\2012\Inst_ALOrderXMLService 12 1.doc`. These are:
- Installation of this service.
- Fill in the configuration file for this service.

### 2.3.1. Configuring the process
Installation includes a configuration file which can be edited by hand or with a configuration tool. The database settings are made in the second dialog of the OrderXML service:

*(Screenshot of "A+W Enterprise 5 OrderXML Service Configuration" dialog for database settings)*

In the configuration file, the switches have the following names:
- **DB/Server**: Defines the name of the database server.
- **Db/Host**: The name of the database host is required for Informix Setnet settings.
- **Db/Service**: The port number for database communication.
- **DB/Database**: Defines the name of the ALCIB database.
- **DB/User**: Defines the name of a database user.
- **DB/Password**: Defines the password of the current database user. Must be encoded by the configuration tool.
- **DB/ClientLocale** and **DB/DBLocale**: Requires input of the Client and Database Locale. The format is e.g. „en_US.CP1252 ".
- **Db/DSN**: A name for an ODBC data source; the name can be selected at random.

The first dialogue of the configuration tool defines where the OrderXML files shall be saved.

*(Screenshot of "A+W Enterprise 5 OrderXML Service Configuration" dialog for service settings)*

- **OrderXML/ExportFilepath**: The directory into which the Windows service is to write the OrderXML files. In case of **internal site separation**, sub-directories are expected in this directory, matching the site number (hnr) of the corresponding sites.

#### Further Settings for the Windows Service
The following settings in the Windows service configuration file can be used to influence the process.
- **MaxNumOrders**: Defines the number of orders that shall be processed at once.
- **OrderXMLEncoding**: Defines the Encoding by which the OrderXML files shall be created. The standard setting will produce the OrderXML file in UTF8 format.
- **PollingIntervall**: Defines the waiting time before the service checks for new orders.
- **ServicelD**: A unique ID for redundant services. If there is one OrderXML system, the setting '0' is correct.

### 2.3.2. Fileless transfer via AWSOA Planning Import Service
With the latest version of the OrderXML services (status as of May 2021), it is possible in the configuration program to set the transfer to the Planning Import Service so that it is fileless. This can be set in the configuration program instead of the output path. If you select the "AWSOA Planning Import Services" option, you have to select a Planning Import Service. With this mode, no more file is required. However, the "files" processed are stored in the "Archive" or "Problem" folder with the extension ".stream".

### 2.3.3. Starting the process
After installation and configuration, the A+W Enterprise 5 OrderXML service can be started. This is done in the Windows start menu: `Settings > System control > Administration > Services`. It may be necessary to change the start type to 'Automatic'.

### 2.3.4. Updating to a higher version
To install a new version please stick to the following sequence:
- Uninstall the service in `System control > Programs and functions`. The configuration file will be kept.
- Install the new diskset for the SetupLauncher and install the ALCIB-OrderXML service using the SetupLauncher.
- SetupLauncher automatically starts the configuration tool. The configuration file of the previous version can be used as an input template. It should not be copied from the earlier versions 2.0, 2009 or 2011.
- Now delete the installation path of the old version.
If only a patch update is required, it is not necessary to uninstall the existing service.

### 2.3.5. Tracing
Recording can be switched on after the setup, to check the setup or search for errors. The entire process is noted in the OrderXML service's log file.

> **Note**: Tracing is useful for searching and should also be used especially in the set-up phase. Recording should however be switched off during operation. Tracing is quite time-consuming.

#### Switches for the Windows Service Tracing
Tracing is set in the third dialogue of the configuration tool.

*(Screenshot of the "A+W Enterprise 5 OrderXML Service Configuration" trace settings dialog)*

The settings can be found in the configuration file `AWAlcibOrderXMLService.exe.config`.
- **AWTrace/Path**: Defines the directory in which the trace file shall be written.
- **AWTrace/Filename**: Defines the name of the trace file.
- **AWTrace/MaxSize**: Determines the maximum size of the trace file.
- **AWTrace/FileMode**: Specifies what will happen when the log file has reached the maximum size (backup or timestamp).

Section `<switches>` of the configuration file determines the log depth, separately for:
- **Albwir.Basis**: Basic functions like database communication.
- **Albwir.Alcib.AlOrderXMLService**: The search for orders, selection and compiling of data, and the writing of the OrderXML file.
- **Albwir.Alcib.Basis**: The ALCIB bill of material is changed into a hierarchy that can be handled by OrderXML.

The OrderXML log itself can be used to create Documentation on where certain information from ALCIB can be found in OrderXML. The trace level of the switch **Albwir.Alcib.AlOrderXMLService** must be set to 4 for this purpose.

### 2.3.6. Activation in ALCIB
The OrderXML interface can be enabled from ALCIB 2008.2 upwards. To enable the process in ALCIB please set the following ALCIB-ALENV switch:
- **ORDERXML**: Defines that a case is submitted to the service for processing after input. The first parameter defines the version; an unequal entry means that only orders shall be transferred while an even input means that both orders and quotations shall be transferred. Currently valid entries: 1, 2.

The following switches are mandatory for the process:
- **MODUL_KOSTENKALK**: This variable must be '2' only if the transfer is not made to ALCIM by Alcim Capacity. Entries '1' or '2' in connection with ALCIM-Capacity permit a preliminary transfer just for production cost calculation.
- **BYTE_VEKTOR**: Necessary for determining the relevant edge for edgework, and the right forms for text.
- **SPROSSENGITTER**: Please use the muntin function in ALCIB for ordering muntins.
- **MODUL_NEUE_STUFEN**: The new step logic should be active.
- **ISO_RAHMEN_MODELL**: If a spacer record is available, the correct spacer width and height to be transferred can be determined.

ALCIB prioritizes rush orders over standard orders, and standard orders over those for cost calculation only. This can be customized with the SP **cu_orderxmlpriori**.

#### SP cu_orderxmlpriori
This SP receives four parameters:
- **INTEGER**: Order number (kauf.auftrnr)
- **SMALLINT**: Code for the document type (5=Order, 4=Quotation, 2=P.O.)
- **SMALLINT**: message type (0=Order transfer, 1=Order cancellation, etc.)
- **SMALLINT**: 1 if it is a rush order, 0 otherwise

The SP must return a **SMALLINT** value, which is transferred to **ottransfer.lfdnr**. The higher the value, the higher the document priority.

#### Preventing Transfer
In certain circumstances it may be necessary to prevent the transfer of orders. The transfer can be prevented by order using the SP **cuxmltransfer**. This SP receives two parameters:
- **INTEGER**: Order number (kauf.auftrnr)
- **SMALLINT**: Code for the document type (5=Order, 4=Quotation, 2=P.O.)

It has to return a **SMALLINT**. It should return '1' by default for transfer. If the SP returns '0', no file will be created. This logic is available in OrderXML service version 12.1.6 or higher.

### 2.3.7. Technical data
The described OrderXML function is based on the following versions:
- A+W Enterprise 5 (ALCIB 2012.1)
- A+W Enterprise 5 OrderXML-Service 2012 (12.1)
- ALCIB-Data 12.0
- ALCIB-Basis 12.0
- Edi-Order-Data 12.0

The service writes the data by „InvariantCulture". This is why they do not depend on the computer locale.

## 2.4. Environment variables

### 2.4.1. ORDERXML_NOSTOCKPLATES
With activation, all stockplate items (atyp >= 180 and < 190) in the OrderXML transfer are filtered out of the BOM and not transferred to production. See AWDesk #448684.

### 2.4.2. ORDERXML_PROCPOSTDEF_LEVELDOWN
Site reference: order. If active, for an ordered parent part, processing that takes place after the defining processing is transferred in the OrderXML file on the glass below the ordered glass. See AWDesk #461345

### 2.4.3. ORDERXML_PROCPOSTDEF_LEVELDOWN_MODE
Site reference: order. If this is active with a value > 0 and the variable **ORDERXML_PROCPOSTDEF_LEVELDOWN** is also active, similar logic applies.
- **Value "1"**: A ProcPostThermal processing on the only TG below the ordered part is transferred if there are several kinds of glass below the ordered part. [AW-159250]

### 2.4.4. ORDERXML_ENDCUSTOMER_DETAILS
Client reference: no. If this variable has the value ON, the optional node EndCustomerOrderDetails is also written. Prerequisite is that the connected sites have common MP master data. For details, see #345567.

### 2.4.5. ORDERXML_POSTPROCTHERMAL_ON_TVG
For the changed behavior, the switch "ORDERXML_POSTPROCTHERMAL_ON_TVG" must be activated to prevent stamps on tempered glass from being transferred to the float glass. See AWDesk #460528, #459758, and PF [AW-83155].

## 2.5. General information in the OrderXML
`\\Jupiter\doku_docuware\Interfaces\OrderXml\AusAlcib\2012\DokuInfosOrderXMLAlcib.txt` is a text file which describes how every piece of information filled in by the Windows service in OrderXML is determined in ALCIB.

This chapter offers information on:
- Where are the OrderXML files written
- What is necessary to write the data correctly
- How the data are gathered.
- How can the written information be influenced (SPs, text attachments)
- Which ALCIB Alenv switches are analyzed for compiling the OrderXML information.

### 2.5.1. How to read the documentation text file
An excerpt from `DokuInfosOrderXMLAlcib.txt`:
```
<ORDER ITEM - USER EXTENT - MainLineItemID=
If SP exists and is usable cupmawpphauptpos(auftrnr, aufnr, 0, posnr, poskonr) is called,
else item reference created from kpos.posnr and rack sequence: to pool_pos.h_pos>
```
- `<ORDER ITEM - USER EXTENT – MainLineItemID:` is the node in the OrderXML file.
- `If SP ...rack sequence:` Describes how the information is gathered, either by SP or directly from ALCIB data.
- `: to pool_pos.h_pos>:` A hint on where to find the information in ALCIM if the OrderXML file is imported.

### 2.5.2. OrderXML files
OrderXML files are created by order. This means that there is one file per order, and this file includes information on all relevant items.

#### Directory
The directory in which the files are to be saved must be defined in the Windows service configuration file. For internal site separation, further directories have to be created below the configured directory. The names of the directories match the corresponding site numbers (like kauf.hausnr).

#### File name
The names of the OrderXML files follow a defined pattern. An example: `Order237715i0e5t2010-12-12 17-35-24.xml`.
Since PF [AW-70328], the desired delivery date is added to each file name.
Example: `order123i0e5t2021-05-17 10:02:20w2021-06-01.xml`

The name consists of the following elements:
- **Order**: Fixed string.
- **237715**: Unique order number.
- **i**: Separator for item number.
- **0**: The item number is always 0 because orders are always saved completely.
- **e**: Separator for document type.
- **5**: Document type (5=order, 4=quotation).
- **t**: Separator for time stamp.
- **2010-12-12 17-35-24**: Time stamp of information compilation.
- **w**: Separator for delivery date. [AW-70328]
- **2021-06-01**: Delivery date. [AW-70328]
- **[.highPrio]**: facultative: flag for "high priority". (#447496)
- **.xml**: Fixed suffix.

#### Versioning
There are two version numbers: OrderXML structure version and Version contents.

**OrderXML structure version** appears in the header of the OrderXML file, e.g. `version="4.2.0001"`.
- **Main version (4)**: Changes when the structure is completely revised.
- **Sub-version (2)**: Changes after new information is added.
- **Patch version (0001)**: Changes with every extension.

In the switch **ORDERXML_VERSION**, only the main and sub-version are entered (e.g. "4.0").
- **4.0**: First version.
- **4.1**: Includes processing types 1960 and 1970.
- **5.0**: ALCIM synchronizes the file with XSD before importing.
- **5.1**: Includes surface macro (1910) and motif parameters for surface processings.

**Version contents** is a version number at the end of the OrderXML file, e.g., `version="025-04-05-01(12.1.1)"`. It can be used to check if a new service needs to be installed for a new requirement.

#### Structure of Contents
Order information in an OrderXML file can be split into four sections:
- **Order header**: Details like order number, input information, and delivery dates.
- **List of items**: List of all order items.
- **Order summary**: Shows the number of items.
- **A+W-specific extensions**: Includes order-related text and document links.

For every item, the **List of items** offers:
- Information on the item article
- A+W-specific extensions

The A+W-specific extensions for an item include:
- Information on the item, especially the item reference ID.
- **Production list**: A list of relevant elements (glass, foil, spacers, etc.).
- Customer reference
- Reference texts

For every product (element) on the product list, the following are available:
- Information on the element (especially bomID)
- List of sub-products
- Product elements (glass, foil, spacers, etc.)
- Geometries
- Processing list
- List of tupel-specific text

#### XSD-compliant OrderXML files
Starting with a patch version, ALCIM is able to validate OrderXML files before import. To use this feature, set the ALCIB **ORDERXML_VERSION** control to "5.0".

### 2.5.3. ALCIB Environmentswitch
The following environment switches influence the information in an OrderXML file:
- **ORDERXML_KOMPLETTESTUECKLISTE**: By default, the BOM is only broken down as far as relevant for production. If ON, the entire BOM is transferred. **Recommendation for ALCIM: Set to "ON"**.
- **ORDERXML_IGNORIERE_BEARB_BESTELLKZO**: If ON, certain processing steps can be suppressed by setting their processing type in the ALCIB BOM to 'none'.
- **ORDERXML_IGNORIERE_KPOSGEST**: If rack planning is used, items are split by default. If set to '1', rack splitting is not taken into account.
- **ORDERXML_IGNORIERE_POS_BESCHAFFARTO**: If ON, items with supply type 'none' will not be imported.
- **ORDERXML_VERSION**: Sets the version number of the receiving system. Valid: "4.0", "4.1", "4.2", "5.0".
- **PMCGHDICKETYP**: Defines article types for spacers (foil, IG spacers, cast resin) to determine thickness.
- **PMQCIM_TYPRAHMENFARBTEXT**: Defines an article type to specify IG spacer colour.
- **PMXTRAHMENSP**: Allows a special Bender text to be imported for IG.
- **PMXAWPOOLSPROSSEN**: Used for grouping muntin articles.
- **DURCHGSPROSSE**: Defines the continuous muntin if this information cannot be gathered from the muntin type.
- **SPROSSENGITTER**: Defines that ALCIB automatically adds a muntin pattern article above muntins.
- **PMXPOOL_NOAWDFILE**: If ON, prevents the AWDesign file name from being determined.
- **MODUL_VERSIEGELUNGSTIEFE** / **ISO_RAHMEN_MODELL**: Used with new step logic to import step records for spacer elements.
- **STUFENFORMEL**: Must be set if the new step logic is not in use. Defines the step formula.
- **DATEI_REF_PFAD**: Links orders/items with documents (e.g., SN macro files).
- **PMEHANDLE_GERADE_EP**: Reverses the BOM structure for even assembly positions. Standard behavior from Version 2012.
- **PMEHANDLE_EPO**: Defines a fixed assembly position for glass and foil layers.
- **PMEKOPF_EP**: Defines whether the assembly position of the main element is relevant.
- **MODUL_DOPPELSCHICHT**: If ON, installation positions at lower levels can also be defined in a simple glass hierarchy.
- **KATALOGART**: Transfers the catalogue type (A+W, Bystronic, Lisec) for shape numbers.
- **MODUL_INTERNE_MANDANTENTRENNUNG**: Informs the service about internal site separation.
- **USER_ID**: For customized extensions.
- **ORDERXML_NODFUEPROCUREMENT**: If ON, no EDI supply types are taken into account.
- **ORDERXML_FOLIENZUSCHNITTSBESCHAFFART**: If ON, changes the supply type of laminated glass foil to "cutting".
- **ORDERXML_VERSIEGELUNGSDATEN**: Allows importing sealing data with airspace information.
- **AWC_ANGEBOT_DEF_TERMIN**: Defines a default date offset for quotations without a specified date.

**Recommendation**: The following switches should also be set for ALCIB order entry:
- **ISO_RAHMEN_MODELL**: ALCIB always creates a shape record for spacers. This serves to determine its width and height.
- **MODUL_NEUESTUFEN**: With this setting, the step reductions can be adopted for the information of the actually stepped elements.

### 2.5.4. Item split
If rack planning is used in ALCIB, an item can be split onto several racks. The item is transferred several times, once for each rack. The item reference (ReferenceID) shows that the item has been split.
- The first three digits are the internal ALCIB item number (kpos.posnr).
- The last three digits are a counter for the rack.

#### Disable item split
If splitting is irrelevant, it can be disabled with the ALCIB switch **ORDERXML_IGNORIERE_KPOSGEST** set to '1'. This is available from version 12.1.3.

### 2.5.5. Cancellation
- **Order cancellation**: An OrderXML file is created. The `Ordering type` is set to "Cancel". If the order was not previously transferred (checked in table **ottranssav**), no cancellation file is created.
- **Item cancellation**: Cancelled items do not appear in the OrderXML file. The reading program must compare reference IDs to detect cancellations.
- **Change of plant for an order**: If a plant change is detected, two OrderXML files are created: one to cancel the order at the original plant, and a new one to transfer it to the new plant.

### 2.5.6. References in reports
- **Order number**: Found in field **ORDER_ID** in the order header.
- **Item reference**: Found in field **ReferenceID** in the A+W-specific extensions of the item.
- **Element reference**: Found in field **bomID** for the corresponding product (element).
- **Processing Reference**: Found in field **reference** for the corresponding processing step.

### 2.5.7. OrderXML files for purchase orders
This is an integrated special solution.
- **Differences**: P.O.s are identified by document type 2. The internal customer number is determined from **xhaus.kunr**. The Buyer's address and other party details are handled differently. The entire BOM is always transferred.
- **File name and Storage**: Similar structure to orders, but identified by "e2". Stored in a "purchase" sub-directory.

### 2.5.8. OrderXML transfer just for production cost calculation
This transfer type is meant for transfer to ALCIM with ALCIM Capacity. It allows real-time calculation of production costs even if the order is not released for production. The switch **MODUL_KOSTENKALK** must be set to '1' or '3'.

### 2.5.9. Items with supply type "none" in the OrderXML interface
The switch **ORDERXML_IGNORIERE_POS_BESCHAFFARTO** can be enabled and set to 'ON' to suppress items with supply type 'none' from being transferred.

### 2.5.10. End customer information
This development allows transferring particular information about the end customer or distributors. It is implemented using two stored procedures: **SP cupmawpaktext1** and **cupmawpaktext2**. The environment variable **ORDERXML_ENDCUSTOMER_DETAILS** must be active.

### 2.5.11. Automatic creation of rack groups and additional parameters for PMO
AWP permits the automatic creation of rack groups defined by formulas. PMO commands are defined in the ERP system and transferred via OrderXML. Keywords like `#CIMGROUP`, `#PMOGROUP`, `#PMOSET`, `#STRATEGY`, etc., are analyzed. This functionality requires detailed configuration in master data and formulas.

#### 2.5.11.1. Changing the PMO command via SP
As of version 13.4.11794, the PMO command transferred in OrderXML can be adapted via a stored procedure `cu_getpmocommand`.

## 2.6. Elements information in OrderXML

### 2.6.1. Import-Relevant Element Types
The following element types will be imported:
- **Sheets**: Cut sizes (article types 100-179, and 200). Stocksizes are generally ignored.
- **Laminated glass foil**: Article type 176. Only foil elements are imported.
- **IG spacers**: Article type 210 or 211.
- **Cast resin**: Spacer for cast resin products, usually article type 340.
- **Muntins**: One element is imported for the muntin pattern.
- **Wood**: Article type 701 is handled like glass.
- **Other elements/accessories**: Various types like edge protection, foil, glass bricks, accessories, etc. are recognized.
- Gas (260) and sealants (240) are not imported as separate elements but as information with spacers.

### 2.6.2. Meta elements in the AWE BOM
Meta elements (marked by element flag 2) are meant to unite processing steps or depict pricing structures. They are generally ignored if their supply type is "Production". Special logic applies for ordered META elements or when EDI supply types are used.

### 2.6.3. Element Reference / BOM ID
Each element is identified by "bomID". The reading program uses this to determine the BOM hierarchy. The reference is structured as:
- First three digits: internal item number (kpos.posnr)
- Next three digits: serial number for the item (counter for rack splits)
- Last four digits: tupel number, a unique number in the ALCIB BOM.

### 2.6.4. Step information
We recommend enabling the new step input method in ALCIB (switch **MODUL_NEUESTUFEN**).
- **Old step input**: Step parameters are adopted in the "STEPPING" element of the main element.
- **New Input of Steps**: The same geometry is adopted for all sheets. The reference glass is marked by "3" in the "Valuation" element. For stepped sheets, a "STEPPING" element contains the actual step reductions. For shapes with radii (e.g., circles), the single step entered in ALCIB is extended to the multiple steps required for production. A detailed table maps ALCIB shape numbers to the number of steps and the corresponding database fields.

### 2.6.5. Spacer
A step record can exist for spacers if the explicit spacer geometry function is active (**MODUL_NEUESTUFEN** and **MODUL_VERSIEGELUNGSTIEFE** or **ISO_RAHMEN_MODELL**). The "Valuation" element identifies the reliable spacer geometry by 10.
- **CUTBACK element**: Describes the spacer cutback.
- **Width and height**: The switch **ISO_RAHMEN_MODELL** should be set in ALCIB to import correct widths and heights.
- **Gas**: Considered part of the spacer information. The gas article should be located below the spacer in the ALCIB BOM.
- **Sealant**: Also part of the spacer information. The sealant article should be located below the spacer in the BOM for clear allocation, especially in triple IG. Sealing type and color can be determined by SPs.

### 2.6.6. Muntins
If an item includes muntins, an element record describing the pattern is loaded. The structure is arranged by horizontal and vertical sections. Using the grid function in ALCIB is recommended. The muntin continuation type (e.g., continuous, double mitre, blunt connection) is transferred and depends on the ALCIB muntin type and other parameters.

### 2.6.7. Element thickness
The thickness of an element is usually calculated from the total thickness of its sub-elements. The IG spacer is an exception.

### 2.6.8. Number of sub-elements
The ALCIB BOM allows adding sub-elements multiple times by changing the quantity. The total quantity is calculated by multiplying the item quantity by the element quantity (`multiplier`).

### 2.6.9. Supply types
Supply types are shown for every element. They generally match the supply types in the BOM (aufstrukt.bestellkz). Various standard (Production, Stock, P.O.) and EDI-specific supply types (P.O. before EDI, Production before EDI) are transferred.

### 2.6.10. Laminated foil cutting
The supply type of produced laminated foil can be changed to 'cutting' if the switch **ORDERXML_FOLIENZUSCHNITTSBESCHAFFART** is set to 'ON' and the foil has a stocksize and 'cutting' processing.

### 2.6.11. IG with more than three sheets
Quadruple IG can be handled from OrderXML service Version 3.6 and ALCIB 2011 upwards. Airspace details are adopted based on the sequence of spacers in the BOM.

### 2.6.12. Fire protection glass
Fire protection glass (item type 160) and its fillings (177) are handled. ALCIM imports additional airspace information for these fillings. Specific parameters for Vetrotech (SGG) production, like spacer thickness, width, and cutback, can be transferred.

## 2.7. Ordered glass and processings after the definining processing
The ProcPostThermal processings are only transferred in the OrderXML file when the parent part is ordered. This can have undesirable effects if master BOMs are not structured correctly. The environment variable **ORDERXML_PROCPOSTDEF_LEVELDOWN=ON** can prevent this by transferring the processing to the glass below the ordered glass. The variable **ORDERXML_PROCPOSTDEF_LEVELDOWN_MODE** provides more nuanced control.

## 2.8. Processing information in OrderXML

### 2.8.1. Allocating Processing Steps to Elements
Processing steps are imported as a list within the element information. The allocation depends on the element's article type or the A+W processing type. The program searches for the first (defining) processing step (e.g., cutting, toughening) and allocates subsequent steps to the same element. The sequence is determined by the BOM.

### 2.8.2. Defined processing steps for elements with a supply type other than production
If the complete BOM is adopted, elements and processing steps for non-production items (ordered, stock) are also transferred. However, the *defined* processing steps for these elements are removed.

### 2.8.3. Processing steps below a toughened sheet
A special logic is implemented for toughened glass. A processing step can be marked in master data as "ProcPostThermal" (to be performed after the furnace). This determines if it's allocated to the float glass (before furnace) or the toughened glass (after furnace).

### 2.8.4. Marking the relevant ProcPostThermal processing steps
The marking is done via a configurable field in the article master data. A field name containing "ProcPostThermal" must be configured and set to '1' for the relevant processing step articles.

### 2.8.5. Processing reference
Every processing step has a processing reference ("reference") which matches the tupel number in the ALCIB BOM, allowing clear identification.

### 2.8.6. A+W Processing Types
If processing steps are allocated to A+W processing types, they are described by fixed, unique parameters in the `awProcessing` element. This allows for a much richer, structured description of the processing.

### 2.8.7. Numbering of Edges for Edgework
Edges are numbered anti-clockwise for edgework definitions. For example, for a rectangle, edge 1 is the bottom, 2 is the right, 3 is the top, and 4 is the left.

### 2.8.8. Supply types
Supply types for processings match those in the BOM (aufstrukt.bestellkz). '0' for production, '1' for purchased, '2' for stock. EDI supply types are also supported.

### 2.8.9. Suppressing processing steps with supply type 'none'
The switch **ORDERXML_IGNORIERE_BEARB_BESTELLKZO** can be activated in ALCIB to suppress the transfer of processing steps that have their supply type explicitly set to 'none'.

### 2.8.1. Interlayer cutting as additional processing on LAMI
An interlayer cutting (atyp 752) can be interpreted as a defining processing for a foil or as an additional processing on a LAMI stock dimension to cut off protruding foil.

### 2.8.2. Customer's own label number from EDI order overwrites own label number
The environment variable **ORDERXML_BDE_BARCODE** (ON/OFF) controls whether the label number from `kposzusatz.barcode_char` is transferred to A+W Production.

### 2.8.3. Location-spanning PDC
This enables the transfer of a label number to individual sites, each with its own production system. The environment variable **ORDERXML_VERSION** must be at least "5.4" and **ORDERXML_BDE_BARCODE** must be "ON".

## 2.9. Customized information in OrderXML

### 2.9.1. Configuration of SPs and texts
In A+W Enterprise Version 6, the configuration dialog for Stored Procedures (SPs) and texts is called from the system menu: `CTRL+F4 > System configuration > Production transfer`. This dialog allows activating/deactivating SPs and texts for the OrderXML interface.

### 2.9.2. Stored Procedures
For many pieces of information in OrderXML, a standard logic exists, but special SPs can be defined to customize the information. A long list of available SPs is provided, covering order texts, special codes, processing names, document links, spacer types, sealant types, and more. Each SP entry details its purpose, default behavior, transfer parameters, and expected return values.

### 2.9.3. Texts
A standard logic for text transfer is also available, configurable via the same dialog. Texts can be order-based, item-based, or tupel-related. They can be created automatically or entered by hand. The configuration depends on the form vector in the `auftxt` table. A comprehensive list of text types and their conditions for transfer is provided.

## 2.10. Internal client separation

### 2.10.1. Company change in the order after transfer to AWP
If a company change is desired for a released order, a new company number can be entered. The system queries A+W Production if a cancellation is possible. If accepted, the order is cancelled in the old company and re-released in the new one. This process is logged in the order status. The Export Service handles the cancellation transfer to AWP. The OrderXML Service handles site changes, deactivating the old logic of sending a special OrderXML to the previous site.

## 2.11. A+W Processing Types

### 2.11.1. UV protection (awtyp 1650)
In AWE, a UV protection processing can only be assigned to one edge. If this single AWE edge is mapped to multiple CAD segments, the OrderXML file will be written, but only the first segment's UV protection is transferred, and an error is logged.

### 2.11.2. Configure/non-configured processing parameters
For numeric processing parameters, the OrderXML file distinguishes between configured and non-configured parameters. This is determined by checking the parameter configuration in the `artvermass` master data table.

## 2.12. AWE item types

### 2.12.1. Other articles (atyp 999)
Articles with `atyp 999` are intended for price-relevant items that should not reach production or purchasing. They are not written to the OrderXML file.

## 2.13. Extended Workbench (EWB)
Activating the environment variable **MODUL_ORDERED_PROCESSING (ON)** switches on the extended workbench logic in AWE. This influences the OrderXML BOM generation, for example, by not transferring meta elements with supply type "PO" if there is an ordered processing below them.

## 2.14. DB switch - Status feedback / rack feedback when switching to a new ERP database (e.g. multisite system)
A logic in the ERP web service allows status feedback to be reported to either an old or a new ERP system during a conversion phase. The logic is enabled by the environment variable **AWC_DBSWITCH ="ON"**. The table **AWC_DBSWITCH** is checked to determine the correct database connection based on the order number range.

## 2.15. Interesting facts

### 2.15.1. Error reports in the Windows service log
An error like `System.EntryPointNotFoundException: Unable to find an entry point named 'IFMX_CleanConnForPooling' in DLL 'iclit09b.dll'` indicates a missing or incorrect Informix driver DLL in the GAC. The Informix Client SDK must be installed or repaired correctly.

### 2.15.2. No orders are processed
If orders in `ottransfer` are not processed, check the service log. If no errors are reported, check for redundant records in the table or an incorrect `serviceid`.

### 2.15.3. List of form vectors
A table lists the bit values for various forms (Manual cutting list, Credit note, Order, etc.) within the byte vector configuration in the `auftxt` table.

### 2.15.4. Invalid special characters
The characters `<`, `>`, `&`, `"`, `'` are invalid in text and names and must be represented by their XML entities (`&lt;`, `&gt;`, etc.).

### 2.15.5. Manual transfer of orders
Orders should not be transferred manually by adding a record to `ottransfer`, as this bypasses the transfer of necessary additional information.

### 2.15.6. Processing step assembly or cutting
The import of "Laminating" and "Laminated cutting" processing steps depends on the supply type of the stocksize in the BOM. A BOM configurator in ALCIM can be used to remove the "cutting" step if it's not needed for a produced laminated sheet.

### 2.15.7. If the database is inaccessible
The OrderXML service will attempt to re-initialize the database connection. After five consecutive failures, the service will terminate. It can be configured for automatic reboot.

### 2.15.8. Glass door systems and shape data
For whole glass systems (item type 400), each part is described individually. The `refflag` in `kmodparam` is not considered for this type.

### 2.15.9. Weight of main and sub parts
To address incorrect weight calculations, the OrderXML file can now transfer two unique attributes, `weightShape` and `weightRectangular`, to distinguish between the actual shape weight and the weight of the circumscribing rectangle. This requires `ORDERXML_VERSION` >= "5.5".

### 2.15.10. Ordering types and their significance
A list of ordering types used in the AWE environment is provided, such as Produce, ChangeProduce, Cancel, Offer, Calculation, etc.

## 2.16. Other documents
The document `\\jupiter\DOKU_DocuWare\Interfaces\OrderXml\AusAlcib\2012\Dokulnfos OrderXMLAlcib.txt` describes how information is gathered from ALCIB for each OrderXML node. Other related documents for installation and general structure are also referenced.

## 2.17. Annex: A+W processing Type Information
For processing steps allocated to an A+W processing type, the OrderXML file includes the `awProcessing` element, which contains the category and relevant parameters. A detailed table (not fully included, but referenced) describes the parameters for each processing type and their corresponding fields in the ALCIB database. Correct edge determination requires the **BYTE_VEKTOR** environment.

# 3. AWP Connection

## 3.1. Overview

### 3.1.1. Motivation and goals of this development
This project helps to achieve better integration between ALCIB and ALCIM, replacing the older PMS system. Key points include:
- Link with ALCIM capacity planning
- Transfer of machine and personnel costs from ALCIM
- Order generation
- Simplified completion reports from ALCIM to ALCIB
- New rack feedback
- Display of ALCIB - shipping information in ALCIM

### 3.1.2. Components of the connection
- **ERP Webservice**: Central component for communication, creating the OrderXML data stream and providing various functions called by ALCIM.
- **PPS-Webservice**: Provides methods to transfer information from ALCIB to ALCIM.
- **ALOrderXmlService**: Checks for orders to be transferred and generates the OrderXML file.
- **AlcibExportService**: Handles reporting of incoming goods.
- **Commonbase**: Provides rights and switches (legacy).
- **RPC - Server**: Background process providing ALCIB functionality to the ERP web service.

### 3.1.3. Process description of the connection
An order is entered in ALCIB and released, creating an entry in the `ottransfer` table. The OrderXML service creates an OrderXML file, which is imported by ALCIM for scheduling. During scheduling, ALCIM calls the ERP web service for master data. After successful scheduling, the result is reported back to ALCIB, which may postpone the delivery date, generate purchase orders, and write back costs. Production status and rack feedback are also reported back to ALCIB.

## 3.2. Functions

### 3.2.1. Postponement of delivery date
If ALCIM postpones a delivery date, the order is updated in ALCIB, changes are noted in `kaufedit` and `kaufstat`, and system message 74 is sent.

### 3.2.2. Calculation of dates for the receipt of goods
During capacity planning, ALCIM asks ALCIB for the earliest possible delivery date for each purchased BOM element. The calculation in ALCIB is based on a hierarchy (article-variant, article-supplier, article master) or can be determined by a customer-specific SP `cu_pmartlieftage`.

### 3.2.3. Order generation
After successful scheduling in ALCIM, P.O. proposals are generated via the ERP web service. For changed orders, existing purchase orders are adapted rather than cancelled and re-created, unless the supplier changes. Logic is in place to manage simultaneous processing in the AWE order pool and AWP load transfer, with email notifications for date conflicts.

#### Locking Logic and Order Updates
- **BEST_LOCK_TEST**: (AWE 5 and earlier) A switch to check for locked records in `bestwun`/`bestpool` when saving an order.
- **BEST_LOCK_TEST_SPERRE**: Activates additional logic using `awc_lock_bestwun` to handle PO changes more gracefully, especially with cost calculation.
- **KAUFUPDATE_BEI_BEST**: If active, allows a changed order to be transferred to PMS despite a LOCAL CORRECTION lock, if the user confirms.

### 3.2.4. Cost calculation - General
Personnel and machine costs are calculated in AWP and returned to AWE. For each cost specification > 0, a cost rate is created in the `poskost` table in AWE.

### 3.2.5. Cost calculation - logical and physical machines
The AWP transfers machine and personnel costs in cost elements, specifying a physical and a logical machine. The IDs and descriptions are stored in `pmsbm` (physical) and `pmspsbm` (logical) tables in AWE.

### 3.2.6. Stock forecast
After scheduling in ALCIM, stock forecasts can be collected in the ALCIB table `wlppms` for elements received from stock. The forecast quantity is calculated based on dimensions and quantity units.

#### Inventory Check
- Via the switch **AWC_CHECK_STOCK**, an inventory check can be configured for scheduling. If stock is insufficient, the order is placed in a "reporting problems" state in A+W Production and gets an "error during scheduling" status in A+W Enterprise.

### 3.2.1. Stock removal - reporting of stock plates (XTV)
The ERP WebService function `SetStockplateBooking` handles stock removal reports from AWP. It checks if the stockplate exists, performs a booking via alrpc, and records the withdrawal in the `pmyoptlm` table to prevent double booking.

### 3.2.2. Resolving reservations in the warehouse forecast for XTV feedbacks
For XTV feedback, the corresponding reservations in the stock forecast (`wlppms`) are resolved. For production completion reports, reservations are also resolved by adjusting the booked quantity and status.

### 3.2.3. Consideration of item splits when the successful scheduling is confirmed
Split items (from rack planning or capacity planning) are combined again before booking costs and forecasts in AWE to ensure each item is reported only once with the correct total quantity.

### 3.2.4. Status confirmations production
Production feedback from ALCIM to ALCIB can be statuses without quantity (Scheduled, Released, etc.) or with quantity (Produced, Ready for shipment, Delivered). Switches in ALCIB (**AWC_FIXIERT_AB**, **AWC_FREIGEGEBEN_AB**) control which ALCIM status triggers a lock in AWE. A table provides an overview of the status flow.

### 3.2.5. Status feedback racks
ALCIM reports information on shipping racks to ALCIB via the `SetRackInfo` method. The feedback is a snapshot of the rack's contents. The data is temporarily stored in `ERP_GEST_MELDUNG` in AWP and then booked into `bcbock` in AWE. The bookings can be made status-dependent (Entry, Packaging, Packed, Shipping).

### 3.2.6. Provision of cost centers
The `AWCapacityGetCostCenters()` method in the ERP Web service provides cost centers stored in A+W Enterprise to AWP.

### 3.2.7. Treatment of orders with high priority (AWDesk #447496)
Rush orders in AWE result in a transfer file to AWP with a "highPrio" flag in the filename, ensuring they are processed preferentially in AWP.

### 3.2.8. AWP transfer cost calculation + reservation - [AW-126899]
The transfer type 128 in `ottranszus` triggers a reservation in AWP in addition to a cost calculation. If the marginal income check in AWE is positive, the order is released in AWP via the Export Service and a PPS Webservice call, bypassing a second OrderXML transfer.

### 3.2.9. Forced errors
It is possible to generate artificial scheduling errors for testing by using specific article names in the BOM (e.g., "Capa Error Order").

### 3.2.10. Transfer of purchase information to AWP
This happens with appropriate configuration after a renewed transfer of an order to AWP by the rserv.

### 3.2.11. Reporting of an element exchange
For companies with multiple IG lines, an existing spacer in the AWE BOM can be replaced by another via a stored procedure (`cu_getspacerarticle`) upon reporting from production.

## 3.3. Data structure
- **awc_bestproto**: Stores information about purchase orders generated by ALCIM capacity planning.
- **awc_fertigmeldungen**: Auxiliary table to store previously received quantities for calculating difference quantities from snapshots.
- **awc_modparams**: Transfers changed shape dimensions for P.O. generation.

## 3.4. Feedback object from AWP
The storage of the report object from AWP during CompleteScheduling can be configured via the env variable **AWC_ERPDOC_FILE** for research purposes.

## 3.5. Environment variables
- **AWC_ALCIM_ANBINDUNG**: Activates the main logic for ALCIB-ALCIM integration.
- **AWC_ART_HZEIT (PMCHZEITART)**: Determines the unit for handling time (days or hours).
- **AWC_MIN_HZEIT_KUNDE (PMEDASCHMINHZEITKUND)**: Minimum customer handling time.
- **AWC_MIN_HZEIT_LIEFERANT (PMEDASCHMINHZEITKUND)**: Minimum supplier handling time.
- **AWC_DEF_ROUTENABFAHRT (PMEDASCHROUTENABFAHRT)**: Default route departure time.
- **AWC_BESTELLEN_BIS (PMEHEUTEBZEIT)**: Site-specific order placement deadline.
- **AWC_FIXIERT_AB**: AWCapacity status from which an item is considered fixed.
- **AWC_FREIGEGEBEN_AB**: AWCapacity status from which an item is considered released.
- **PMVERSANDSTEUER**: Regulates packing messages to dispatch control.
- **AWC_URL_PRODUKTIONSBERICHT**: URL of the detailed ALCIM production report.
- **AWC_GESTZU_BUCHEN**: If active, books rack feedbacks to table `gestzu`.
- **AWC_GESTZU_BUCHEN_OHNE_VERPACKTMELDUNG**: Prevents double booking of packing messages.
- **AWC_IGNORE_PACKINGMESSAGE**: Prevents processing of a packing notification from AWP.
- **AWC_IGNORE_AWERACKSTATUS**: Ignores the rack status in AWE for PDC confirmations.
- **AWC_WAEIN_UEBERMITTLUNG**: If active, fills `exportinfo` table for goods receipts.
- **AWC_BUCHE_KPOSPROD**: If active, additionally fills `kposprod` table for produced feedback.
- **AWC_ALCIB_SERVER_NAME**: Name/IP of the ALCIB server.
- **AWC_PORT_RPC_DIENST**: Port number of the RPC service.
- **AWC_PORT_CONTROL_SERVER**: Port number of the control server.
- **AWC_IGNORIERE_GESTELLMELDUNG**: Controls booking of rack reports.
- **GESTELL_BDE**: Book completion reports to rack management.
- **AWC_RACKSTOCK_REGPOINT_TYPE**: Defines registration point type for stock additions.
- **AWC_NACHBEST_MANR**: Employee number for remake order mail notifications.
- **PMEINBTERMINAENDMANR**: Employee number for mail notifications on PO date changes.
- **PMEZKBESTELLT**: If active, takes cutting corrections from `awc_modparams` for purchased glass.
- **SPLIT_POSKOST_COSTS**: Splits costs for automatically generated operations.
- **BEST_LOCK_TEST**: Activates check for order correction locks (until AWE5).
- **BEST_LOCK_TEST_SPERRE**: Activates additional locking logic via `awc_lock_bestwun`.
- **KAUFUPDATE_BEI_BEST**: Allows order change transfer despite LOCAL CORRECTION lock.

## 3.6. Switches in AWP (formerly ALCIM)

### 3.6.1. Switch for loading OrderXML files.
These station-specific switches configure the import interface in ALCIM:
- **Import Interface**: Set to '1' to read OrderXML files.
- **Archive Path**: Directory for successfully imported files.
- **Problem path**: Directory for files that failed to import.
- **Import path**: Directory where the OrderXML service writes the files.
- **Processing Sequence**: Must be '1'.
- **Complete BOMs**: Must be '1'.

### 3.6.2. Switches without Common base
With the removal of CommonBase, many settings are now configured directly in ALCIM.
- **Use CommonBase**: Set to '0' to make all settings in ALCIM.
- **Erp Feedback**: Set to '1' to send feedback via ERP web service.
- **URL, Timeout, Version**: For the ERP Web service connection.
- **Database Server, Name, User, Password, etc.**: For the ALCIB database connection.
- **Site Number**: For internal site separation.

### 3.6.3. Additional AWP switches for AWE-AWP communication
These switches in ALCIM's Shape Catalogs influence data reported back to AWE.
- **Mode to Close SN Files**: Recommended '4'.
- **SN Views to be Turned**: Must include the view used for purchased parts.
- **Create Raw Geometry for P.O. Parts**: Set to '1'.
- **Spacer - Geometry Calculation**: Set to '1'.

### 3.6.4. PF tickets with AWP configuration problem
- **[AW-113462]**: Problem with mirroring of lites ordered. Solution: set AWP switch "Reporting of the processed processing parameters" to "2".

## 3.7. System messages
- **3.7.1. Status 73 - Scheduling or rescheduling failed**
- **3.7.2. Status 74 - Postponement of delivery date**
- **3.7.3. Status 43 - A broken product contains purchase order parts which have to be reordered**

## 3.8. Logging

### 3.8.1. Report (CompleteScheduling) about the ERP Webservice
Logging is done in the ERP Webservice log (`%PROGRAMDATA%\A+W\log`). The report object can also be stored for research.

## 3.9. Troubleshooting

### 3.9.1. Grinding allowance missing in the PO feedback
An update to AWP may be needed. See PF [AW-146391] + [AW-163528].

### 3.9.2. During scheduling, references are not found
"For the order item [x/y], the processing with the reference [z] was not found in the SN file...". This error occurs if the SN file references are incorrect. The import checks for corresponding references for all relevant processings. AWP configuration for "ERP reporting" must be set to 2.

### 3.9.3. Shape change for purchased part
A shape change for a purchased shaped glass can be prevented with a switch in the SN: `PreferInitialShapeNumber = 1`.

### 3.9.4. Crash of the OrderXML Service
Flawed BOMs (e.g., corrupted muntin with tnr=0) can cause an endless loop and memory overflow. Install the latest hotfix. See PF [AW-200146].

### 3.9.5. ProcPostThermal processings in der OrderXML transfer on the wrong lite
Set the env variable **ORDERXML_POSTPROCTHERMAL_ON_TVG**.

### 3.9.6. Order too large for current ERP Webservice configuration
An error like "Maximum request length exceeded" or "The operation has timed out" means the order/report object is too large. Adjust `maxRequestLength` and `executionTimeout` in the IIS or web.config for the ERP Webservice.

## 3.10. Appendix

### 3.10.1. Stock forecast in version 2009 and configuration options
The logic for stock forecast booking is standard in ALCIB 2011. In Version 2009, it requires special enablement, including the creation of table `awc_wlppms`. The stock variant can be calculated via SP `cu_pmewlagbitnr`.

### 3.10.2. Generation of remake purchase orders
The AV remake function in ALCIM can generate a new production item. A function in AWE and AWP 5.1 allows informing the ERP system about parts that must be re-ordered. In ALCIM's rough planning, a context menu for purchased parts allows to "Trigger" a re-order or "Do not trigger". This is activated via a switch in ALCIM and requires the AWC_NACHBEST_MANR switch in ALCIB for mail notifications.

### 3.10.3. Workflow of background processes
Diagrams exist for workflow:
- `\\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity\AngeboteWorkflow.vsd`
- `\\jupiter\DOKU_DocuWare\Interfaces\AlcibAlcimAWCapacity\AufträgeWorkflow.vsd`
