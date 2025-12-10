---
title: "EN-CONFIG-AW_ERP_Stock_Service"
source: "EN-CONFIG-AW_ERP_Stock_Service.pdf"
tags: ["A+W", "ERP", "Stock Service", "Configuration", "Bystronic", "Hegla", "Lisec", "Inventory Management", "Software"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Configuration instructions for the A+W ERP Stock Service module. This document details how to set up and manage the reconciliation of third-party stock systems (Bystronic, Hegla, Lisec) with A+W ERP stocks (A+W Business and A+W Enterprise). It covers general installation, system-specific configurations, master data setup, and operational logic for inventory management."
long_description: "This is a comprehensive internal configuration guide for the A+W ERP Stock Service, a module designed to synchronize inventory data between A+W's ERP systems (A+W Business and A+W Enterprise) and external, third-party stock management systems, specifically those from Bystronic, Hegla, and Lisec. The document provides detailed step-by-step instructions for installation, configuration, and operation. It outlines the architectural differences in communication protocols for each third-party system, explaining the 1:n relationship for Bystronic and the 1:1 relationship for Hegla and Lisec. Key topics include setting up environment variables, configuring the Config Tool, managing master data (such as third-party item numbers and stock market partners), and the specific logic for goods receipt (GR) and purchase order (PO) processing. The guide also covers advanced features like cyclical stock reconciliation, special treatment of cover sheets and broken glass, and handling of various booking types. It concludes with extensive troubleshooting sections and FAQs to address common issues, error messages, and operational questions, making it an essential resource for technical staff responsible for implementing and maintaining the A+W ERP Stock Service."
---

# A+W Configuration Instructions: A+W ERP Stock Service

**-INTERNAL-**

**A+W - Software for Glass**

---
## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2013-06-25 | SVH | Original version | 1.0 |
| 2015-09-21 | SVH | Adjustment (AWDesk #338820) | 1.1 |
| 2017-03-15 | SVH | Chapters were re-arranged | |
| 2018-03-16 | SVH | Lisec Interface (AWDesk #391319) | |
| 2018-03-20 | SVH | AWE XTV feedback | |
| 2018-06-04 | SVH | AWE XTV feedback | |
| 2018-08-16 | SVH | Error during establishment of connection to the Hegla server Configuration of the cover sheet stock | |
| 2019-04-02 | SVH | Addition to the documentation (#443136) | |
| 2019-05-13 | SVH | Addition of problem handling (#443136) | |
| 2019-08-26 | SVH | Addition to the documentation (#443136) -> a Hegla server counts as one stock | |
| 2019-09-04 | SVH | Addition WL_KEINE_NEGATIVEN_BESTAENDE (#443136) | |
| 2019-12-04 | SVH | STOCK_HEGLA_IGNORE_THICKNESS (#453768) | |
| 2022-04-06 | SVH | PO logic (only AWE and only in connection with Hegla stock) [AW-76610] | |
| 2022-12-08 | SVH | Notes about the documentation, reference to other documents | |
| 2023-01-24 | SVH | In the Bystronic particularities, the documentation of the WL_PORT_COSTUNIT* variables was removed since this document was incorrect. The variables were not valid. | |
| 2023-02-02 | SVH | Information about the Lisec stock system | |
| 2023-02-08 | SVH | Differentiation of the "ERP Stock Service" | |
| 2023-03-22 | SVH | [AW-135791] – Lisec connection | |
| 2023-06-26 | SVH | [AW-147994] - Expansion of the docu for PO logic | |
| 2023-07-20 | SVH | [AW-147159] – Lisec-connection - Info email | |
| 2023-09-12 | SVH | [AW-157440] - Socket communication | |
| 2023-12-06 | SVH | [AW-161492] – Hegla – time stamp of the last booking | |
| 2024-01-15 | SVH | Additions: "inventory type", " No valid variant ID found", E-Mail, Panorama, order logic - open POs | |
| 2024-01-26 | SVH | [AW-143894] – Activation/deactivation of the cyclical reconciliation | |
| 2024-03-05 | SVH | [AW-171618] – AWB - Comparison with use of imperial dimensions in AWB | |
| 2024-04-23 | SVH | Overview of used Hegla telegrams | |
| 2024-05-29 | SVH | [AW-192587] – AWE – Booking and comparison for discontinued articles allowed. | |
| 2024-07-04 | SVH | [AW-198448] - No external inventory for ERP item announced | |
| 2024-07-19 | SVH | [AW-198448] – Lisec - treatment of glass types with inventory "0" | |
| 2024-07-23 | SVH | [AW-199683] - treatment of PO items without third-party product code | |
| 2024-07-25 | SVH | [AW-199683] – treatment of incorrect details in the "OrderListReference" in the "OrderListEntryBooked" telegram | |
| 2025-02-18 | SVH | [AW-217449] – Verification of the connection to the external stock | |
| 2025-06-10 | SVH | [AW-230073] – Goods receipt in the ERP system - change in the logic | |

## 1. General information
A+W ERP Stock Service is a module for reconciling a third-party stock with an A+W ERP stock. Possible third-party stocks are currently Bystronic, Hegla, and Lisec stocks.

Via the corresponding configuration in the Config Tool of the ERP Stock Service, the link is established between the third-party stock and ERP stock.

Because the communication of the third-party stocks with the ERP Stock Service relies on different transfer protocols depending on the manufacturer, the configuration in the Config Tool must be done a little differently:

- In the Bystronic system, the stock numbers of the connected ERP stocks are known. Each transfer protocol of the Bystronic server includes the ERP stock number for which the protocol is sent; therefore, one Bystronic server can be linked to several ERP stocks.
- In the Hegla system, the stock number of the connected ERP stock is not known. As a result, transfer protocols of the Hegla server do not include any ERP stock number; therefore, a Hegla server can only be linked to precisely one ERP stock.
- In the Lisec system, the stock number of the connected ERP stock is not known. As a result, transfer protocols of the Lisec server do not include any ERP stock number; therefore, a Lisec server can only be linked to precisely one ERP stock.

Here, the assignment information is presented again in the form of a table:

| System | Assignment Third-party server - ERP stock | Remark |
| :--- | :--- | :--- |
| Bystronic connection | 1 : n | ERP stock numbers known in the Bystronic server |
| Hegla connection | 1 : 1 | ERP stock number unknown in the Hegla server. Exception: GR stock logic, see special description, Chapter 6 |
| Lisec connection | 1 : 1 | ERP stock number unknown in the Lisec server. |

### 1.1. Differentiation
The A+W ERP Stock Service may not be confused with other A+W programs that also have the term "Stock Service" in their names.

- **A+W Planning Stock Service**
  More precisely: A+W Production Planning Stock Service
  This service is used in the production environment. With this service, the Residual Stock Manager (manual residual lite management) and Remaster (automatic residual management - Remaster is a Hegla brand name), data about residual lites is called up from the SOA database.

- **A+W Commercial Stock Business Service**
  More precisely: A+W Commercial Business Smart Companion Stock Service
  This service is only used by A+W Business.

- **(Linux) Stock Service**
  More precisely: Linux Enterprise Stock Service
  This service is only used by A+W Enterprise. It provides the data for the Smart Companion and the CX stock forecast.

### 1.2. Availability
The Stock Service 5 can be operated with the ERP programs ALCIB 2011 and A+W Enterprise 5.
Starting with Version 6, the Stock Service can also be made available for A+W Business.

### 1.3. Benefits
Ideally, the Stock Service results in a more precise inventory in the ERP glass stocks.

With the previous outward booking methods, the glass stocks (for belt dimensions) are subject to a certain imprecision in the ERP systems. The previous outward booking methods are:

- Automatic outward booking for delivery note creation
- Automatic outward booking for completion reports from production
- Automatic outward booking based on prediction data
- Automatic outward booking for XTV report
- Manual outward booking

All outward booking processes have limitations with respect to the Stock Service.

1.  **Automatic outward booking for delivery note creation:**
    a. The quantities to be booked are calculated from the dimensions of the delivery note items (with cutting and correction factors, only approximate values are possible). In order to consider that only complete stock dimensions can be withdrawn from physical stock, in the ERP stock, a variable variant is used for the booking. (in practice, however, it has become clear that the complexity of the logic sooner scares customers off.)
    b. Breakage is not considered.
    c. If there is a long period between production and delivery of an order, there can be a similarly large time difference between the actual removal from physical stock and the outward booking of the corresponding inventory from the ERP stock.
    d. No automatic stock reconciliation can be performed during which the inventory in the ERP stock is reconciled with the inventories in the physical stock.
    e. No support of stock management due to lacking interplay with the stock prediction.

2.  **Automatic outward booking for completion reports from production:**
    a. The quantities to be booked are calculated from the dimensions of the glass to be produced (with cutting and correction factors, only approximate values are possible). In order to consider that only complete stock dimensions can be withdrawn from physical stock, in the ERP stock, a variable variant is used for the booking. (in practice, however, it has become clear that the complexity of the logic sooner scares customers off.)
    b. Breakage is not considered (or is there a switch for this?)
    c. No automatic stock reconciliation can be performed during which the inventory in the ERP stock is reconciled with the inventories in the physical stock.

3.  **Automatic outward booking based on prediction data:**
    a. The quantities to be booked are calculated from the dimensions of the order items (with cutting and correction factors, only approximate values are possible). In order to consider that only complete stock dimensions can be withdrawn from physical stock, in the ERP stock, a variable variant is used for the booking. (in practice, however, it has become clear that the complexity of the logic sooner scares customers off.)
    b. For large orders that are produced across a longer period, there is imprecision in the outward booking if for the order items no item split is executed or if there is no rescheduling.
    c. The outward booking is done in a nightly routine and considers only the preliminary production date and not the actual cutting date.
    d. No automatic stock reconciliation can be performed during which the inventory in the ERP stock is reconciled with the inventories in the physical stock.

4.  **Automatic outward booking for XTV report:**
    a. No automatic stock reconciliation can be performed during which the inventory in the ERP stock is reconciled with the inventories in the physical stock.
    b. No support of stock management due to lacking interplay with the stock prediction.
    c. A manual removal for hand cutting or trade is not considered.

5.  **Manual outward booking:**
    a. There is no timely booking, generally booking is done once a day.
    b. Error due to incorrect entries are possible, either directly during the entry of the booking record or at the cutting tables, where lists with item numbers and quantities must be kept.
    c. No automatic stock reconciliation can be performed during which the inventory in the ERP stock is reconciled with the inventories in the physical stock.

With the use of the Stock Service:

- Timely outward booking is guaranteed (the booking is done precisely at the moment at which the lite is removed from the physical stock)
- Following from this, the precision of the inventory data in the ERP stock is increased
- Following from this, an effective materials management (material flow, order generation) is supported
- The stock management provides more accurate values at all times than all other outward booking methods

In the Stock Service, a daily stock reconciliation can be configured, which ensures that all differences in the inventories that can occur due to careless GR booking are eliminated. The inventories of the ERP stock are thus compared to the inventories of the physical stock. Leading here is the physical stock.

If the customer was previously forced to execute a stock inventory at short intervals (once a month) in order to determine the inventories and update them, this interval can now be extended and thus the amount of work reduced.

For customers with a long inventory interval (e.g. once a year), the Stock Service automatically produces much greater security in the inventory of the ERP stock.

The Stock Service can be configured very flexibly depending on customer needs. It is multi-site capable, it can connect several external stocks and even different external stock systems (Hegla and Bystronic).

**Notes:**

- In order to maintain precision of the average prices in the ERP stock, it is important that the customer books inward goods in the ERP in timely fashion. Unbooked inward goods in the ERP stock mean that the unbooked quantities are corrected with the daily stock reconciliation, whereby the inward booking is done at the current average price.

**Special notes for A+W Enterprise:**

- **Stock forecast:**
  The forecast data for a portal stock is adjusted using a current stock booker (version >= 13.04.0634) and activation of XTV feedback for the portal stock.
  For XTV feedback, in this configuration, the prediction data is adjusted by the ERP Webservice in cooperation with the alrpc service.
  See chapter "XTV feedback."
  If a stock booker < Version 13.04.0634 is used, the adjustment of the forecast data for a portal stock CANNOT be done by the XTV feedback.
  The XTV feedback for the portal stock has to be deactivated in any case. An adjustment of the forecast data has to be built in via customizing.

### 1.4. Documentation
#### 1.4.1. Start-up with A+W Business
The general configuration/functionality is described in this document.
The AWB-specific configuration/functionality is **not** described in this document.
Consult the general A+W Business configuration documentation for additional information.
For the configuration of the ERP Stock Service in the Config Tool, please consult the associated installation instructions.

#### 1.4.2. Start-up with A+W Enterprise
The general and AWE-specific configuration/functionality is described in this document.
For the configuration of the ERP Stock Service in the Config Tool, please consult the associated installation instructions.

## 2. General Installation
There is a special installation instruction available at:
`\\jupiter\SW_Install\<version>\InstallationDocumentation`

It is available in SetupLauncher when the complete SW_Install directory is delivered for installation.

### 2.1. Operating Systems
The Stock Service is approved for the server systems:
- Windows Server 2008 R2
- Windows Server 2012
- Windows Server 2012 R2

### 2.2. Execution of the Config Tool
See installation instructions.

### 2.3. Licensing
The installation of a LicenseClient on the server on which the Stock Service is running is necessary.
The Stock Service can only be operated with a valid license. A separate license must be available for each third-party stock type.

| Third-party stock type | License module |
| :--- | :--- |
| Bystronic | App=2300; BA=1; ED=2300; Ver=2012; Modul=1 |
| Hegla | App=2300; BA=1; ED=2300; Ver=2012; Modul=2 |
| Lisec | App=2300; BA=1; ED=2300; Ver=2012; Modul=3 |

## 3. Installation with A+W Enterprise
### 3.1. Bystronic connection with ALCIB 2011
**Attention:** The following steps are only necessary in ALCIB Version 2011!

#### 3.1.1. Installation of ALCIB stock
1.  Install a current wlager binfile (buildnr > 776).
2.  Bring the database up to the correct status. Execute the SQL script from the installation directory of the ALCIB Version 2013 `"xsql/12/1/0/120100008_wlraum_sql"` or execute the following update statement:
    `"ALTER TABLE wlraum ADD (welnr INTEGER DEFAULT 0);"`
3.  Add files to the stock area. The files must be retrieved from the appropriate language version ALCIB 2011. The following files must be installed:
    a. $PRG/lager/mfo/wlraump.mfo
    b. $PRG/lager/pan/wlraump.pan (language-dependent)
    c. $PRG/lager/sel/wlraum_welnr.sel (language-dependent)
    d. fx_texte/messages (language-dependent, date > 12.10.2011)
4.  Create the ALCIB environment variable WL_PORTALLAGER and activate it with "ON".

## 4. General Configuration
### 4.1. Multi-site systems
As far as we know, there is (as of 03/29/22) no multi-site installation where several ERP multi-site sites "talk" to stocks with third-party stock connection. The multi-site capability of the ERP Stock Service is not guaranteed in such an installation.

### 4.2. Socket communication
Communication between a third-party stock and the ERP Stock Service takes place via a socket connection.

The socket interface used by the ERP Stock Service (Panorama interface) accesses the port range of the free dynamic ports on the customer system.
Thus, it is the customer's responsibility to determine which ports are available to the ERP Stock Service for communication by configuring the dynamic port range.

**Caution:** It is also the customer's responsibility to ensure that the ports of the dynamic port range are not blocked even in the firewalls and the routers that are located between ERP Stock Service and the third-party stock server.

**Note:** In the configuration with a Hegla warehouse, in addition to the IP address of the Hegla server, a port number (by default "10010") is also stored for communication. This combination of IP and port is used by the socket interface to define the remote target system; beyond that, the port number stored here has no meaning.
The port for the local system is still taken from the dynamic port range during communication.

netstat example (on the client computer / computer of the ERP Stock Service):
`TCP 192.168.11.22:49876 192.168.33.44:10010 SYN_GESENDET`
- the port „49876“ comes from the dynamic port range
- the port „10010“ comes from the configuration of the Hegla connection in the ERP Stock Service

See also PF [AW-157440].

### 4.3. Cyclical stock reconciliation (deactivation)
The cyclical stock reconciliation is a core component of external stock incorporation.
Since in individual cases it can nevertheless be necessary not to conduct this reconciliation cyclically, it is possible via the Config Tool to deactivate the functionality.
The deactivation is done separately for each external stock type (Hegla, Lisec, Bystronic). Within a stock type, the setting applies for all connected stocks.
See PF [AW-143894].

### 4.4. Special Features of Hegla Connection
#### 4.4.1. Configuration of the DB settings in the Config Tool
The configuration is described completely in the installation document. Here, an excerpt of this is reproduced, which is required for the PO logic. (The detailed description of the PO logic is also found in the separate chapter "Function description with A+W Enterprise".)

- **Checkbox „Use AWSOA"**: Using the AWE purchaseservice
- **AWSOA Login Name**: User for the use of the AWE purchaseservice, the stored name must exist in the AWE employee master as login name (mitarb.loginname)
- **AWSOA Multisite ID**: Client number of the purchaseservice in case of a multisite installation, the client numbers available for selection are displayed in the drop-down menu of the field.
- **Date Range Into Past (days)**: The number of days to search for open purchase orders in the past, starting from the current date, is entered.
- **Date Range Into Future (days)**: The number of days to search for open purchase orders in the future, starting from the current date, is entered.

#### 4.4.2. Configure the Hegla Connection in the Config Tool
- **Stock ID**: Per "Hegla communication," only one stock ID can be stored. That is, for each AWE portal stock, a separate "Hegla communication" must be created. From the point of view of the ERP system, a Hegla server represents precisely one Hegla stock. It can be connected/synchronized with precisely one ERP stock in the configuration. The configuration of several ERP stocks with one and the same Hegla servers by generating several entries in the connections that only differ in the Client ID (but address the same Hegla server, with the same IP and the same port), is NOT permissible.

- **Cover Sheet Stock ID**: By specifying a cover sheet stock (stock number > 0), it is possible to configure a connected cover sheet stock for a portal stock. The defined stock number specifies the cover sheet stock. For stock number > 0 the developed special logic (AWDesk #371602) for cover sheet applies. All cover sheets are booked to the cover sheet stocks indicated here.
  **CAUTION:** Each portal stock must be assigned a separate (exclusive!) cover sheet stock. It is not possible that several portal stocks can share one cover sheet stock. If two portal stocks were assigned to the same cover sheet stock, during the cyclical stock reconciliation, incorrect inventories would arise.

- **Stock MP**: Via a special stock market partner, the item numbers of the Hegla stock items are mapped to the ERP item numbers. In different "Hegla communication" entries, the same stock market partner can be used.

- **Interface Version**: Hegla interface versions 2.1.0.0 or higher are supported.
  - If the customer has an interface subversion 2.1.x.y, „2.1.0.0" must be selected in configuration.
  - The GR stock logic can only be activated with an interface version 2.2.0.0 or higher.
  - If the customer has an interface subversion 2.2.x.y, „2.2.0.0" must be selected in configuration.
  - The stock logic can only be activated with an interface version 2.3.0.0 or higher.
  - If the customer has an interface version 2.3 or higher, „2.3.0.0" must be selected in configuration.

- **Port number**: Information from Hegla (Mr. Ridder, 2013-08-21): The port number, via which the stock server communicates on the server system, is 10010 by default and should be the same for all connected stocks. For more information on ports, see also the separate chapter "Socket communication".

- **Client ID**: Information from Hegla (Mr. Ridder, 2013-08-21): With the client ID, it is communicated to the Hegla server which client is connecting to it. Even if several "Hegla communication" records exist, the same client ID is entered in each one since from the point of view of the Hegla server, the same client (ERP Stock Service) always connects. The configuration of several ERP stocks with one and the same Hegla servers by generating several entries in the connections that only differ in the Client ID (but address the same Hegla server, with the same IP and the same port), is NOT permissible. Generally, the client ID "1" can be used.

- **Measurement**: Measurement unit during communication, presently just in "mm".

- **Ignore Broken Glass**: Normally, this checkbox should not be checked. The treatment of breakage in Stock Service was corrected with AWDesk #371602. Broken glass will be taken over into the ERP inventory during the cyclical reconciliation. The inventory will be reduced if a breakage booking is reported from the Hegla stock. But if for some reason a customer cannot work with the corrected logic, check the checkbox and the Stock Service will handle breakage as before the correction. Broken glass will be ignored both during the cyclical reconciliation as well as during the breakage reports.

- **Allow Inward Stock Booking**: The "Allow inward stock booking" checkbox must be enabled if the PO logic or GR stock logic is used. If the checkbox is not enabled, the bookings that are sent by the third-party stock with the telegram "OrderListEntryBooked" are rejected by the ERP Stock Service.

### 4.5. Special Features of Lisec Connection
#### 4.5.1. Configure the Lisec Connection in Config Tool
**Interface Version**
Configuration instructions.

| Lisec interface version of the Lisec server | Lisec version to be configured in the A+W ERP Stock Service Config tool | Remark |
| :--- | :--- | :--- |
| 2.71 or higher (in this version nomenclature) | 2.71 | "2.71" is the oldest of the versions listed here |
| 02.00.000 to 02.00.006 | 02.00.000 | Current versions use the notation "02.00.000" or "02.x.y" |
| 02.00.007 or higher | 02.00.007 | see above |

See also PF [AW-135791] and [AW-220804].

**Client Name**
The entered "Client Name" is an agreement on the name between the Lisec system and the ERP Stock Service. The name can be selected at will, but must be known to the Lisec system.
Via the name, it is ensured in the Lisec system that only telegrams are sent to the client that are suited for it.
See also PF [AW-135791].

**Port number**
Lisec must provide the port number to be used.

**Measurement**
Measurement unit during communication, presently just in "mm."

**Cover Sheet Stock ID**
See chapter "Configuring the Hegla Connection in Config Tool"

## 5. Configuration with A+W Enterprise
### 5.1. Environment variables
#### 5.1.1. WL_PORTALLAGER
In Version ALCIB 2011 (4.5), the env variable WL_PORTALLAGER must be activated so that the portal stock logic is activated. The variable is only present in Version 2011. It serves as protection, since for the use of the portal stock logic, the dialog for storage space management (wlraum) must be adjusted.
Starting with Version AWE 5 (12.1) the logic is no longer clipped via WL_PORTALLAGER.

#### 5.1.2. AWC_ALCIB_SERVER_NAME
The variable must contain the name of the AWE (Unix/Linux) server.

#### 5.1.3. AWC_PORT_CONTROL_SERVER
In the variables, it must be stored on which port the Stock Service can communicate with the AWE background processes.

#### 5.1.4. WL_KEINE_NEGATIVEN_BESTAENDE
This variable must be set in order to prevent bookings from external stock from creating negative stock in the ERP stock.
If the variables are set, stock bookings that would lead to negative stock are rejected by the stock booker and only processed after the next incoming booking.

#### 5.1.5. STOCK_HEGLA_IGNORE_THICKNESS
If the variable is active, the thickness of the Hegla article is not taken into account when searching for the mapped article in the AWE stock. Mapping can only work if there are no thickness variations in the Hegla system for article numbers.
The logic only works if an AWE stock is linked to a Hegla stock. For a link with A+W Business or for other third-party stocks (Bystronic, Lisec), the logic is not made available. (AWDesk #453768)
With AWDesk #461784, with the "Ignore Thickness" checkbox in the Config Tool, it is possible to not consider the glass thicknesses for article mapping in the Hegla stock connection. If the checkbox is activated, the logic applies both in the connection with A+W Enterprise as well as with A+W Business.
For the connection to A+W Enterprise, there is no hierarchy in the configuration. If either the variable STOCK_HEGLA_IGNORE_THICKNESS or in the Config Tool the "Ignore Thickness" checkbox is activated, the glass thicknesses are not considered during article mapping.

### 5.2. Configuration of the Stock Booker
In order to specify the message recipient for system messages from the stock booker, the AWE environment variable WL_MELD_EMPF must be activated. If the variable is not active, the system messages are sent to the respective recorder of the stock booking. In the case of the Stock Service, the recorder of bookings is always the user ID -1 (system). Messages go to the e-mail address stored in the employee master data.

### 5.3. Master Data
#### 5.3.1. Third-party stock market partner
Via the Master data > Market partner dialog, a special market partner of the type "Other" must be created, which represents the stock connection to a particular third-party stock (Bystronic, Hegla, or Lisec). Via this market partner, the third-party item numbers are assigned in the stock connection below.

#### 5.3.2. Third-party item numbers
Via the Master data > Articles > F4 > Market partner details dialog, the third-party item numbers of the connected stock must be assigned to the appropriate AWE article numbers. As market partner, the previously-created third-party market partner is entered.

**CAUTION:**
Several entries for which different external article codes are assigned to one and the same AWE article number are not permissible.
The determination of the external article code would then not be unambiguous when creating the "OrderList"!

**Hegla stock incorporation**
Attention: doubled third-party item numbers for a third-party stock market partner (in artkuzu) are permissible. Since the third-party article is defined by the combined key (item code, thickness of the glass, height of the glass, width of the glass), an item code in artkuzu can be assigned to several AWE article numbers.

**Bystronic stock incorporation**
No thickness information about the lites is transferred by Bystronic. Here, a Bystronic item number must be assigned to precisely one AWE item number.

#### 5.3.3. Article Caching
Article/variant master data from AWE is cached in the Stock Service. After a change in the AWE variant data, therefore, the Stock Service must be restarted so that the changes take effect.

#### 5.3.4. Glass thicknesses
**Hegla stock incorporation**
Since for the assignment of the Hegla article number to the AWE item number the glass thickness transmitted by Hegla is part of the key, the glass thicknesses must be maintained correctly in AWE (artikel.staerke), that is, they must match the Hegla glass thicknesses.

#### 5.3.5. Determination of the AWE variant number
For the determination of the AWE variant number using width and height, the stored procedure wlgetbitnur is called within the Stock Service. It determines the variant number (artvarzu.bitnr/xxvar.bitnr) in the standard version delivered by A+W using the dimensions transmitted taking into consideration a Delta range.

The ERP Stock Service and the A+W Enterprise Stock Booker interpret the return value of the SP wlgetbitnr in the same way: a variant counts as determined if the return value of the SP > 0. The return value corresponds to the variant number in A+W Enterprise.
Return values <=0 mean that no variant was found.

With PF [AW-135791] the logic for determining the AWE dimensional variant was adapted so that in addition to the exchanged dimensions of width and height, an appropriate variant is searched for if no variant with the original values could be found. This logic is not included in the SP wlgetbitnr, but in the logic called up in the ERP Stock Service.
The logic was generally adjusted and affects all stock connections (Hegla, Lisec, and Bystronic).

Whether the same logic exists in AWB is not known at this point.

**Digression: Description of the logic in the standard version of the SP wlgetbitnr delivered by A+W**
The return value of the SP is a numeric value.
A positive return value (>0) corresponds to the variant number determined in A+W Enterprise.
A return value <=0 means that no variant was found.

In the standard version of the SP wlgetbitnr, first there is a search for a variant with a dimension Delta of 20 mm. If with this dimension Delta a variant is found, then this variant number will be returned.
If no variant is found, the Delta is increased to 200 mm and then searched for again. If a variant with the increased Delta is found, the variant number is delivered back as a negative value.
If no variant is found with the larger Delta, the value "0" is returned.

It is no longer possible to trace where the logic in wlgetbitnr that searches with the increased Delta for a variant and in case of a hit returns the negative variant number comes from (status as of 08/24/2024).
Important is that both the AWE Stock Booker and the ERP Stock Service ignore this negative variant number and interpret any return value <=0 as "Variant not found".

The SP wlgetbitnr can be adjusted on the customer system according to the customer's wishes at any time. Attention must only be paid that only positive return values count as variant numbers found.

#### 5.3.6. Portal stocks
The third-party stock-connected AWE stocks must be marked as portal stock in the master data.
When creating a portal stock on the stock dialog Master data > Room, the stock type "normal" must be specified for the stock and the toggle value "portal stock" selected in the field interface.
The specification of an IG stock may only take place if the user would like to work with the GR stock logic of the Bystronic stock connection. For inward goods for a portal stock, the entry of an GR stock causes automatic steering of the inward goods to the IG stock entered.

**Configuration of GR stocks**
In order to set up an interface stock on the stock room management dialog (STOCK > Master data > Room), proceed as follows:
1. Set up a corresponding inward goods stock for the interface stock to be created. A inward goods stock must be created as shelf stock. A GR stock will be assigned an interface stock in a 1:1 assignment. This means that precisely one GR stock belongs to an interface stock. The GR stock cannot be assigned to a second interface stock.
2. Now define the interface stock. In the GR stock field of the interface stock, the stock number of the corresponding IG stock must be specified.

**Prevention of the automatic booking of prediction data**
The marking of a stock as portal stock (interface: "portal stock") prevents the automatic outward booking from stock based on the prediction data (wlppms table) within the nightly stock routine.

#### 5.3.7. Cover sheet stocks
The configuration of a cover sheet stock that differs from a portal stock can only be done in the Hegla stock connection. In AWE, the cover sheet stock is created as "normal stock."
Each portal stock must be assigned a separate (exclusive!) cover sheet stock. If two portal stocks were assigned to the same cover sheet stock, during the cyclical stock reconciliation, incorrect inventories would arise.

#### 5.3.8. Inventory change marker
The inventory change marker has to be set to "AWP" for the stock articles kept in the portal stock; this creates the forecast data using the calculated production date.
**Attention:** if the inventory change marker is set to "Delivery note/AWP," there can be doubled bookings in the forecast data.

### 5.4. XTV feedback
With use of the Stock Service, previously the XTV reporting had to be deactivated since otherwise removals from coupled stocks were made twice. As a result, the adjustment of the forecast data coupled to it was also deactivated. This was changed with AWDesk #289178.
The XTV reporting - and thus the adjustment of the forecast data can now - with use of a current stock booker (starting with build 13.04.0634) be used together with the Stock Service - for the stock booker now checks the stock properties for removals with status 68 (PMS_ABGANG_EXT). If the stock from which the removal should be made is a portal stock (WLRAUM.INTERFACE = 2), no stock removal is made. In this case, the stock in question is a synchronized third-party stock that is removed by the Stock Service. A corresponding entry in the stock booker log documents that this removal is suppressed. The record is then deleted from the table wlh.
There is also a chapter on this topic in the "Enterprise Production Interface" configuration instructions.

### 5.5. Special features of Hegla connection
#### 5.5.1. PO logic (Hegla goods receipts based on the AWE POs)
With a connected Hegla stock, the PO logic can be activated.
Here, the goods receipts are generated based on the open POs that exist in AWE. The logic is described in detail in the special chapter "Function description with A+W Enterprise".

### 5.6. Special features of Bystronic connection
#### 5.6.1. Master Data
For the ByStore communication, it is necessary that all ALCIB tape measure and cover sheet articles that should be booked into the ByStore interface stock be mapped to the appropriate ByStore material number. The ByStore material number must be stored in the article master data in the private fields (artikel.private_long1).

## 6. General Function Description
### 6.1. Logging
The Stock Service protocol can be found in `%PROGRAMDATA%\A+W\Log`.

### 6.2. Sending e-mails
The Stock Service sends e-mails in order to inform about errors that have occurred. The sending of an e-mail is recorded with a log entry in the Stock Service log (text "Send E-mail...", TraceLevel "Info").
If no e-mail is received by the recipient although the sending is noted in the log and no error has occurred, it must be checked whether the firewall is blocking the sending.

### 6.3. GR stock logic
#### 6.3.1. General
The GR stock logic was previously available in the Bystronic and Hegla stock connection. It was conceived in order to prevent removals from the third-party stock being reported to the ERP system by the Stock Service before the inward goods were booked in the ERP system. The removal of lites from non-booked goods receipts results in incorrect inventories and incorrect average prices.

In the respective third-party systems there is a logic that allows the removals for a goods receipt only once the inward goods have been confirmed in the ERP stock. The query of the confirmation starts with the third-party system.

The use of the GR stock logic is recommended in order to prevent incorrect inventories and incorrect average prices. However, many customers decide against the logic nevertheless since they feel restricted in the way they work by the forced confirmation of the ERP goods receipt.

#### 6.3.2. Configuration
The GR stock logic can only be used if, on the one hand, a GR stock is specified in the stock master data for a portal stock configured in AWE and, on the other hand, the third-party stock system has the appropriate logic to query the incoming goods.
Furthermore, the "Allow inward stock booking" checkbox must be enabled in the Config Tool if the GR warehouse logic is used. If the checkbox is not enabled, the bookings that are sent by the third-party stock with reference to the GR stock are rejected by the ERP Stock Service.

#### 6.3.3. Process
For the GR stock logic, for each goods receipt for a connected portal stock from a third-party stock system, first the AWE incoming goods booking must be queried and confirmed before the goods receipt stocks in AWE are finally booked to the portal stock.

The query for transferring the goods receipt stocks is initiated from the third-party stock system. The query of the third-party system always refers to a stock order placed in AWE.

The flow of the handling of the goods receipt is designed as follows: upon the recording of the PO in AWE, the goods are delivered sometime. The delivery note is compared to the PO. The included cover sheets for the stacks are added to the PO after the fact. In case the purchase order is already in local correction, this change however is only commercially relevant. While it is transferred into the goods receipt, it cannot be transferred into the stock anymore due to the status of the purchase order (local correction).

For the subsequent inward goods booking for the PO in AWE, the stock stored is analyzed for the PO item. If the stock is an interface stock (interface = "portal stock"), the inward goods are booked to the corresponding goods receipt stock (GR stock). The respective slot number is composed of the order number and sub-number in the form "BBBBBBBB/SSS".
Here missing cover sheets can be booked manually via a slot inward booking into the respective slot.

An automatic correction of cover sheets takes places through the nightly stock reconciliation.

After the goods receipt has been booked in the AWE GR stock, only then is it transferred to the corresponding portal stock if the third-party stock system has queried the goods receipt via the Stock Service and confirmed it.

### 6.4. Special treatment of cover sheets
The logic for special treatment of cover sheets (booking of the cover sheets to a separate cover sheet stock) was previously only available in the Hegla stock connection.

In the ERP stock, cover sheets cannot be distinguished from normal lites. There is no marking that identifies a cover sheet. For distinction, the lites can only be booked into different stocks in the ERP system. A separate stock is configured for cover sheets.

The advantage of a cover sheet stock that deviates from the portal stock is thus that in the ERP system the inventory of the portal stock is not falsified by cover sheets since under some circumstances cover sheets may not even be available to production (e.g. due to low glass quality).

Each portal stock must be assigned a separate (exclusive!) cover sheet stock. If two portal stocks were assigned to the same cover sheet stock, during the cyclical stock reconciliation, incorrect inventories would arise.

The flow for booking cover sheets is described in more detail in Chapter Special treatment of cover sheets (AWDesk #371602).

### 6.5. Cyclical stock reconciliation
The cyclical stock reconciliation ensures that the inventory of the ERP stock is synchronized with the inventory of the third-party stock at least once a day. Here the third-party stock is the leading stock. Ideally, the cyclical reconciliation determines that the inventories of both stocks are identical. If this is not the case, the inventories of the ERP stock are reconciled with additions or removals of the individual variants of the inventories in the third-party stock. All bookings are made using the respective current average price.

#### 6.5.1. Behavior in case of non-processed records in the booking queue (wlh)
Before the stock reconciliation, the Stock Service checks whether there are records in front of the stock booker for the current stock to be reconciled.
For non-processed records, the stock reconciliation waits for the processing. For security, in this case the stock booker is started by the service.
If after 5 minutes there are still non-processed records in front of the stock booker, the reconciliation is not performed for the complete current stock. Here it plays no role which articles are affected by the non-processed records.
If an e-mail recipient is configured in the config tool, an appropriate notice is sent to him via e-mail.
See also #330257

#### 6.5.2. Treatment of negative stocks (see also #364470, #344044)
There is no special treatment for negative stocks in the ERP stock.
If, for example, for a variant in the ERP stock the stock is -20 and the corresponding article in the external stock indicates an inventory of 30, then the amount after the stock reconciliation will be 30.

#### 6.5.3. ERP variants without external correspondence – "No external inventory for ERP item announced"
During the cyclical reconciliation, the Stock Service queries the inventories of the connected third-party stock. If no inventory is reported by the third-party system for an article that is kept in the ERP stock (that is, no data record for this article is transmitted), the Stock Service cannot decide whether the missing message for the inventory means that the inventory is 0 or whether there was an error during the transmission. Therefore, in this case, the inventory is NOT changed in the ERP system in this case.

In the log, a message with the following content is output: "No external inventory was transmitted for the article variant X. The inventory of this variant in the ERP system will not be changed."
An info is sent as e-mail in which the recipient is asked to check the master and transaction data in the ERP stock.

**Message text in the original (English):**
> "No external inventory for ERP item announced (...): WARNING: No external inventory has been announced for ERP item ID ..., variant ID ..., stock ..., actual amount .... The amount won't be changed automatically. Please review master data and stock data."

#### 6.5.4. Error handling
If during the stock reconciliation for an article an error occurs (e.g. no corresponding ERP article data is found), the reconciliation for this article is skipped and continued with the next article.

Errors that cause a cancellation of the entire stock reconciliation are:

- Non-processed records in the booking queue during cyclical stock reconciliation => the stock reconciliation is not executed.
  Changed with #330257, for non-processed records, the stock reconciliation waits for the processing (but 5 minutes at most)
- Error records in the booking queue during cyclical stock reconciliation => the stock reconciliation is not executed.

### 6.6. Restrictions
#### 6.6.1. XTV coupling
With use of the Stock Service, it must be ensured that for the corresponding cutting tables, the XTV coupling to this stock is deactivated, if the system works with stock booker version < 13.04.0634. With use of a stock booker from version 13.04.0634 on, the XTV coupling can be deactivated.
See chapter "XTV feedback."

#### 6.6.2. Cyclical stock reconciliation
At the time of the stock reconciliation, all inward goods in the ERP stock and stock accesses in the third-party stock must be matched to one another. If this is not the case, the deviating quantities are booked as inventory difference, this has effects on the prices in the ERP stock.

#### 6.6.3. Inventory of portal stocks
With an external stock connection, it is essentially assumed that the external stock is the leading stock (during cyclic reconciliation, the inventories in the ERP system are corrected based on the data of the external stock).
The keeping of an inventory on the ERP side does not make sense for portal stocks. The nightly stock reconciliation therefore does not check whether the stock for which the reconciliation is executed is in inventory or not.

#### 6.6.4. Variable variants
Variable variants can't be booked with this interface.

### 6.7. Error handling
Essentially for an error that has occurred, an e-mail is sent to the recipient stored in the configuration.
Known errors are:
- No item mapping possible => The current booking is not executed.
- Non-processed records in the booking queue during cyclical stock reconciliation => the stock reconciliation is not executed.
- Error records in the booking queue during cyclical stock reconciliation => the stock reconciliation is not executed.

### 6.8. License query
Upon starting, the Stock Service checks whether for the configured stock connections there is a valid license.
If the license check fails, no communication about the configured stock is established, however the service continues to run since another licensed connection could be present.
An info e-mail is sent about the licensing problem.
Since the license check is not automatically repeated by the Stock Service, the service must be restarted in order to perform another license check.

### 6.9. Special features of Bystronic connection
#### 6.9.1. IG stock logic
**#337007**
Previously invalid slot numbers (order number = 0) were not included.
With this process, a check is built in. If the order number = 0, the IG booking is not executed. A corresponding note is in the Stock Service log, no e-mail is sent.

#### 6.9.2. OrderListRequest/OrderList/BookData telegram
After the inward goods in AWE, all bookings that relate to this deliver will be initiated by Bystronic. Bystronic first sends the telegram "OrderListRequest" with the number of the AWE interface stock in order to query the inward goods for the stock. The Stock Service responds to this with the "OrderList" telegram, which contains the inventories in the corresponding IG stock. If an error occurs during the query of the IG stock in the Stock Service or if the "OrderList" cannot be created because there are unbooked records for the IG stock in front of the stock booker, an empty "OrderList" telegram is sent back to Bystronic. The error is logged by the Stock Service (log file, see installation instructions) and the employee configured in the Stock Service receives the error message via e-mail.

On the Bystronic page, there is now a reconciliation of the "OrderList" telegram with the goods delivered. If a deviation is determined (incorrect cover sheet), it is possible to correct the inventory in the ERP stock in the GR stock. The slot assignment for the new cover sheet must absolutely be adhered to. Then, Bystronic must send another "OrderListRequest" telegram in order to receive the updated "OrderList."

After the successful reconciliation of the "OrderList" telegram with the goods delivered, Bystronic initiates the inward booking into the interface stock by sending the "BookData" telegram. The Stock Service executes the appropriate outward bookings from the IG stock and inward bookings to the interface stock. The booking price for the inward booking of a variant into the interface stock is determined from the average price of the variant in the IG stock. No response telegram is sent. Errors that occur are logged by the Stock Service and sent via e-mail.

#### 6.9.3. UnBookData telegram
Bystronic can then initiate outward bookings from the interface stock with the "UnBookData" telegram. The outward booking types AUTO (production/cutting) and BREAK (break) are processed. Both types equally cause an outward booking in the ERP stock. No response telegram is sent. Errors that occur are logged by the Stock Service and sent via e-mail.

#### 6.9.4. Cyclical stock reconciliation
In a 24-hour rhythm, the Stock Service initiates a stock reconciliation of all interface stocks configured in AWE. The service sends an "InventoryRequest" telegram for a stock to be reconciled and receives a "StoreInventory" telegram as response, which contains the inventory of the corresponding Bystronic stock. The Stock Service reconciles the inventories of the variants and adjusts the stock of the AWE stock to the inventory of the Bystronic stock with inward or outward booking orders. A stock reconciliation is not executed if there are flawed booking records in front of the stock booker for the interface stock to be reconciled.

#### 6.9.5. Restrictions
**Batch tracing**
Batch tracing is not implemented. During the stock inward booking via interface, Bystronic transmits a batch number, however this is not transmitted to the ERP system by the Stock Service.

**Thickness specifications**
No glass thicknesses are transmitted by the Bystronic interface, as a result, these can also not be considered for the data matching in the ERP system. This means that items that are distinguished only by their thickness always have different material numbers in the Bystronic system.

**No special treatment of cover sheets and breakage**
With AWDesk #371602 the special treatment of cover sheets was implemented for Hegla connection.
The analysis of Bystronic interface shows that the treatment of cover sheets and breakage can NOT be supplied within the process by the Bystronic interface. The main reason is, that no information regarding glass type (cover sheet/breakage/normal) was sent in the telegram of cyclic stock reconciliation.

### 6.10. Particularities of the Hegla stock connection
#### 6.10.1. IG stock logic
IG stock logic can only be used with a Hegla interface version 2.2.0.0 or higher.

#### 6.10.2. Booking the goods receipt
**OrderListRequest/OrderListRequestResult/OrderListEntryBooked Telegramm (AWDesk #338820)**
After the inward goods in AWE, all bookings that relate to this delivery will be initiated by Hegla. Hegla first sends the telegram "OrderListRequest" with the number of the AWE interface stock in order to query the inward goods for the stock. The Stock Service responds to this with the "OrderListRequestResult" telegram, which contains the inventories in the corresponding GR stock. If an error occurs during the query of the IG stock in the Stock Service or if the "OrderList" cannot be created because there are unbooked records for the IG stock in front of the stock booker, an empty "OrderList" telegram is sent back to Hegla. The error is logged by the Stock Service (log file, see installation instructions) and the employee configured in the Stock Service receives the error message via e-mail.

On the Hegla page, there is now a reconciliation of the "OrderListRequestResult" telegram with the goods delivered. If a deviation is determined (incorrect cover sheet), it is possible to correct the inventory in the GR stock in the AWE stock. The slot assignment for the new cover sheet must absolutely be adhered to. Then, Hegla must send another "OrderListRequest" telegram in order to receive the updated "OrderList."

After the successful reconciliation of the "OrderListRequestResult" telegram with the goods delivered, Hegla initiates the inward booking into the interface stock by sending the "OrderListEntryBooked" telegram. The Stock Service executes the appropriate outward bookings from the IG stock and inward bookings to the interface stock. The booking price for the inward booking of a variant into the interface stock is determined from the average price of the variant in the IG stock. No response telegram is sent. Errors that occur are logged by the Stock Service and sent via e-mail.

**OrderListReference**
The "OrderListRequestResult” telegram contains in particular the “OrderListReference".
In the GR stock logic, the reference consists of:
- Slot number
- Article number
- Variant number
- In format `<Slot number>/< Article number>/< Variant number>`

Example: Slot 224455/1, Article number 100004, Variant number 23
=> OrderListReference “224455/1/100004/23"

The OrderListReference is sent back by Hegla using the “OrderListEntryBooked" telegram to refer to the respective element of the “OrderListRequestResult".

#### 6.10.3. Booking types (Hegla InventoryType)
The Stock Service currently only books the following booking types (inventory changes) reported active by the Hegla stock:
1 - Manual inward booking (only to cover sheet stock)
3 - External booking out of stock
4 - Automatic booking out of stock
7- Breakage (if "Ignore Broken Glass" is configured)

This means that with the current Stock Service, NO inward bookings initiated by the Hegla stock into the ERP stock are possible. Correction bookings (Inventory Type 2) are also currently not processed.

**Removals**
*Logic adjustment with build 13.04.9880*
Previously, for the processing of the InventoryChange telegram, the "Destination position" (target position) was not evaluated.
This problem is now solved.
If an InventoryChange telegram is sent by the Hegla interface, now first the "Destination position" is checked.
InventoryChange telegrams with a destination position <= 1000 are not processed further since these are not removals from the stock.
Destination positions <= 1000 are stock locations within the stock. For cutting tables, destination positions > 1000 are provided.
Only the destination positions > 1000 are now processed further as stock removals.

#### 6.10.4. Re-booking previously unbooked stock removals
When starting the Stock Service and after successful establishment of socket communication with the Hegla server, there is a query of all bookings executed by the sending of the GetInventoryChange telegram. All bookings are requested that have been executed in the Hegla stock since the last booking transmitted.

When the ERP Stock Service receives the GetInventoryChangeResult telegram, it checks the validity of the time stamp of each booking (see chapter "Time stamp of the last booking made").

Only records with valid time stamp are forwarded to the ERP system for booking. After a successful booking, the time stamp for the query of the booking made is updated.

#### 6.10.5. Time stamp of the last booking made
In the ERP system, the time stamp of the last booking made ("footprint") is saved for a portal stock.

Each booking report from the Hegla stock is compared to the saved time stamp. The currently reported booking in the ERP system is only made if the time stamp of the current booking is greater than the saved reference time stamp. Each booking must be more recent than the last booking made.
This logic exists to prevent out-of-date booking messages from creating new bookings in the ERP system.

The complete time stamp set consists of:
- Portal stock number (stock_id)
- ID of the source item (Hegla) of the booked lite (key1)
- ID of the destination item (Hegla) of the booked lite (key2)
- Time stamp as string (key3)

In A+W Enterprise, the time stamp table is called "wlportalsync".
In A+W Business, the time stamp table is called "SYSADM.LG_LASTBOOKED".

For a Hegla connection, the following logic also exists:
If the ERP Stock Service is started, there is a check whether there are "passed-over bookings" that must be rebooked.
For this logic, in the ERP Stock Service, there are log entries with the keyword "WorkMissedInventoryChanges()". In the ERP system, the time stamp of the last booking made is determined. Then in the Hegla stock, all bookings are queried whose time stamp is greater than the last booking made in the ERP system. If the Hegla stock reports bookings for this query, these are rebooked in the ERP system.
If in the ERP system no time stamp of the last booking made can be determined, the rebooking logic is exited without further actions.
In the log, you will find the message "HeglaSyncSingle.WorkMissedInventoryChanges(): No booking foot print existing => exit.".

**Remark:**
The time stamp in the ERP system is saved as string. The format of the string is specified regardless of culture ("CultureInfo.InvariantCulture"): "MM/dd/yyyy hh:mm:ss".
The formatting has nothing to do with the transfer in the interface telegram.
Sample time stamp string: " 12/05/2023 08:39:27".

#### 6.10.6. Special treatment of cover sheets (AWDesk #371602)
If a cover sheet stock was entered in the Config Tool for Hegla connection, the cover sheets will be booked to this special cover sheet stock.
**Caution:** A cover sheet stock may only be entered if it is different from the interface stock.

Cover sheets are marked as such on the racks in the Hegla stock. For a lite to be booked, it can be determined using the rack on which the sheet is located, and using the position of the lite on the rack, whether or not it is a cover sheet.

Configuration without GR stock means that the ERP stock's inventory is updated by booking telegrams and the cyclic reconciliation and then all bookings of cover sheets are made from the corresponding cover sheet stock.

Configuration with GR stock and in the PO logic [AW-76610] means, when receipt of goods is confirmed (OrderListRequestEntryBooked) the cover sheets are booked for a short period to the portal stock and rebooked immediately from the portal stock based on a booking telegram (InventoryChangeEvent) to the cover sheet stock. Following, all bookings of cover sheets - as in configuration without GR stock - from cover sheet stock.

**Restrictions**
If in the Hegla stock an existing cover sheet is rebooked, that is, it goes from type "cover sheet" to type "normal sheet," this information is not known immediately in the ERP system. Only with the next cyclical reconciliation is the sheet booked into the portal stock instead of the cover sheet stock.

#### 6.10.7. Treatment of broken glass (AWDesk #371602)
With Hegla connection, the "Ignore Broken Glass" checkbox can be enabled or disabled in the Config Tool.
If the "Ignore Broken Glass" checkbox is disabled, broken lites that are reported by external stock with an InventoryChangeEvent are removed from the ERP stock.
During the cyclical comparison, the broken lites are also booked in the ERP system.
If the "Ignore Broken Glass" checkbox is enabled, broken lites from external stock are NOT booked in the ERP system.

#### 6.10.8. Handling of residual plates
At the moment (status as of 07/25/2024), in the InventoryChangeEvent, the type "Restblatt" is not recognized and there can therefore be no special treatment.
If the dimensions of a residual lite fit a variant, the lite is booked.
It can be that with PF [AW-176670] special treatment of the residual lites will be implemented.
In the interface description of Hegla, the telegrams GetInventoryChangeResult, InventoryChangeEvent, GetRackLoadingResult, GetStockInventoryResult all receive the parameter "Type". The information whether the lite is a residual lite is in "Type".

**6.45 Type**

| Type | Unsigned Long |
| :--- | :--- |
| Description | Describes the stack type on the rack: <br> 0: normal glass <br> 1: Cover sheet <br> 2: Cardboard <br> 3: Broken glass <br> 4: Remnant |

Currently, however, precisely the information that this is a residual lite is not transferred to the ERP Stock Service by the A+W interface ("Panorama").

```csharp
namespace Albwir.Alcim.Machines.MachineControl;

public enum HeglaStockType
{
    Undefined = -1,
    NormalGlass,
    CoverSheet,
    Carton,
    BrokenGlass
}
```

#### 6.10.9. Treatment of glass thicknesses (AWDesk #461784)
By activating the "Ignore Thickness" checkbox in the Config Tool, the thickness of the Hegla article is not considered in the Hegla stock connection when searching for the mapped article in the ERP stock. Mapping can only work if there are no thickness variations in the Hegla system for article numbers.
The logic only works if an ERP stock is linked to a Hegla stock. For other third-party stocks (Bystronic, Lisec), the logic is not made available.
For the AWE connection, the same configuration option also exists via the environment variable STOCK_HEGLA_IGNORE_THICKNESS (AWDesk # 453768). This type of configuration was made available when it was not yet known that the same logic was also required in the AWB connection. It is recommended that the configuration is preferably done via the Config Tool.

#### 6.10.10. Checking the connection to the Hegla server (AWDesk #459484, PF [AW-41702])
When starting the Stock Service, the socket connection to the Hegla server is established. The Stock Service functions as a client. At the time of the cyclical reconciliation, it is checked whether there is still a connection to the Hegla server. If not, there is an attempt to establish a connection.
In addition, it is checked every 30 minutes whether there is still a connection to the Hegla server. If it is determined that the connection has been interrupted, there will be another attempt to make a connection.
The cyclical check should prevent that the connection remains permanently interrupted after a reboot of the Hegla server, and as a result that no bookings may be made in the ERP stock.

#### 6.10.11. PO logic [AW-76610]
Instead of the GR stock logic, the PO logic can be configured in connection with A+W Enterprise. This logic is only available if on the ERP side an A+W Enterprise is configured and a Hegla stock is connected. A precise description of the logic is in section 7.

#### 6.10.12. Restrictions
**General**
- Only dimension variants, but no color variants are considered.
- All referenced ERP items must keep dimension variants.
- Each Hegla stock will be synchronized with precisely one ERP stock. Here, a Hegla server is regarded as a Hegla stock.

**Configuration of the communication in the Config Tool**
From the point of view of the ERP system, a Hegla server represents precisely one Hegla stock. It can be connected/synchronized with precisely one ERP stock in the configuration.
The configuration of several ERP stocks with one and the same Hegla servers by generating several entries in the connections that only differ in the Client ID (but address the same Hegla server, with the same IP and the same port), is NOT permissible.

**Socket communication**
All time stamps are requested by the Stock Service from the Hegla server in the format. "dd.mm.yyyy hh:nn:ss" - that is, to the second.

**Batch tracing**
Since in the current Hegla interface no information about the batch is transmitted, no batches are considered within the Stock Service.

**Limitations of the reconciliation**
In the course of permanent stock-keeping, only outward bookings are processed. Inward bookings take place on the basis of the inward goods in the ERP stock (only thus can a value stock-keeping be guaranteed and a meaningful stock log arise). The inward booking of the inward goods in the ERP stock must be done in timely fashion, in particular before an outward booking can take place via the Hegla stock. The inward booking of the inward goods in the ERP stock must be done in timely fashion.

Bookings from the Hegla stock for items not present in the ERP stock are rejected.

Bookings that would cause negative stocks are rejected by the stock booker if the env variable WL_KEINE_NEGATIVEN_BESTAENDE is active. They remain as booking records with error flag in the booking table wlh.

Re-bookings within the Hegla stock have no meaning for ERP stock.

**Problems due to the decoupling of the commercial inward goods in the ERP stock from the inward goods in the Hegla stock**
In the long run, the stock connection only functions smoothly if the inward goods in the ERP stock is executed in timely fashion with respect to the inward goods in the Hegla stock. If the commercial IG is delayed, in the course of the day there can be a stock shortfall, so that the booking records get stuck with the error status before the ERP booking process (if the env variable WL_KEINE_NEGATIVEN_BESTAENDE is active). In this case, no nightly stock reconciliation is executed.
If the shortfall in the commercial stock is corrected easily with a forced stock reconciliation, there is an incorrect determination of the prices in the ERP stock. The solution is always the commercial IG booking.

**Handling of broken glass in inward stock booking**
In GR stock logic Hegla announces the amount of broken glass in the telegram "OrderListEntryBooked". But the broken glass is ignored by the Stock Service and thus is not considered in the booking. All lites, whether broken are not, are booked in.
Example: Hegla announces AMOUNT=10 and AMOUNT-BROKEN=3, which means that 3 of 10 booked glass lites are broken. The booking in AWE is 10 lites. The information about the broken glass is dismissed.

**Problems in case of deviation of the clocks on the Hegla server and the ERP Stock Service process server**
Both servers have to run synchronously so that the checking of the time stamp of a booking transmitted by the Hegla server works correctly in the ERP Stock Service.
See also PF-Ticket [AW-58648].

#### 6.10.13. Overview of used telegrams
Here is an overview of the Hegla telegrams that are used in the communication with the ERP Stock Service.
The socket communication with the Hegla stock is done via the A+W Panorama interface that is integrated into the ERP Stock Service. The A+W Panorama interface is supported by the "Techsoft" department. For detailed information about implementation of the Hegla telegrams, please consult the responsible Techsoft developer.
The telegrams are described in the Hegla interface documentation "Warehouse Management System Interface 2.3.0.0_Rev2 -gb".
The completeness of the list is not guaranteed.

| Telegram name | Use in the ERP Stock Service |
| :--- | :--- |
| GetRacks | Cyclical reconciliation, racks |
| GetRacksResult | |
| GetRackLoading | Cyclical reconciliation, rack loading |
| GetRackLoadingResult | |
| GetInventoryChange | Request for bookings lost after connect with the Hegla server |
| GetInventoryChangeResult | |
| InventoryChangeEvent | Report of a removal |
| OrderListRequest | Request of the open POs or goods receipt |
| OrderListRequestResult | |
| OrderListEntryBooked | Report of the goods receipt by Hegla |
| OrderListEntryBookedResult | |
| OrderListUserEvent | Report triggers a complete or partial good receipt (only PO logic) |

### 6.11. Particularities of the Lisec stock connection
The Lisec connection contains cyclical stock reconciliation and the transfer of bookings (AWDesk #391319).
The determination of the type of glass (normal glass/cover sheet/residual sheet) is done via the master data of the last cyclical reconciliation. Changes to the master data therefore only affect bookings after the next cyclical reconciliation.

Relevant tickets for booking are:
- AWDesk #457700
- PF [AW-63663]
- PF [AW-107751]

The GR stock logic is not implemented.

#### 6.11.1. Functional characteristics
With the cyclical comparison, the entire inventory is queried by Lisec [GET_GLASS_STOCK].
For the inventory report by Lisec, the type of the glass (normal glass/cover sheet/residual lite) is also communicated for each lite. This glass type is cached in the ERP Stock Service and used for all following bookings. If in the Lisec system the type of glass has been changed in the meantime, this change will only be noticed and become effective with the next cyclical comparison.
By stopping and then re-starting the ERP Stock Service, the updating of the cached glass types (independently of the cyclical comparison) can be forced.

**User interface version older than 02.00.007**
With the Lisec interface version older than 02.00.007, bookings were processed via the inventory change telegram (actions types "PUT_DOWN" and "REMOVE").

**Changes with Lisec interface version 02.00.007**
With the Lisec interface version 02.00.007, removal bookings from the Lisec stock are processed exclusively by the stock movement telegram (FROM_STOCK_ELEMENT - TO_STOCK_ELEMENT).
So that the logic takes, the Lisec interface version "02.00.007" must be selected in the Config tool of the ERP Stock Service.

A glass is booked out of the stock if the element [TO_STOCK_ELEMENT] contains a value that is in the number range 1010020001 to 1010029999.
This number range is reserved for the lines according to the Lisec interface description. If a glass goes to the line, it counts as booked out of the stock.
Since via the stock movement telegram residual lites also go to the line, for the Lisec connection the notification e-mail is suppressed, which is actually sent if an ERP variant for a removal booking message cannot be sent.
It is assumed that this is a residual lite if no variant can be found. Residual lites are not booked.
See also PF [AW-135791] and [AW-220804].

#### 6.11.2. Special treatment of cover sheets
If a cover sheet stock was entered in the Config Tool for the Lisec connection, the cover sheets will be booked at cyclical stock reconciliation to this special cover sheet stock.

#### 6.11.3. Handling of residual plates
Residual lites in the Lisec stock are not considered during the inventory updating (cyclical synchronization and stock movement) in the ERP stock.
See also "Info e-mail" chapter.

#### 6.11.4. Treatment of broken glass
The handling of rejects was never discussed explicitly in the context of the interface. Right now (as of 10/04/2023), it is not known with which telegram the removal booking of rejects is reported by the Lisec stock.
If the rejects are reported by the stock movement telegram (starting with Lisec interface version 02.00.007) or the inventory change telegram (action types "PUT_DOWN" and "REMOVE")(Lisec interface version older than 02.00.08) by the Lisec stock, they are booked in the ERP system so that it is not known that this is a reject.
If the rejects are reported by another telegram or another action type, they are not booked in the ERP system.

#### 6.11.5. Info e-mail
For a Lisec connection, there is the special feature that for lites reported for removal booking, it cannot be detected whether they are stock dimensions or residual lites. For each removal booking, there is a search in the ERP system for an appropriate variant.

For residual lites, there should be no removal booking in the ERP system according to the interface description. Since for a Lisec residual lite generally no ERP variant is found, the removal booking is omitted. Normally, the ERP Stock Service sends an info e-mail if no appropriate variant can be found in the ERP system for a removal booking message. In the case of the Lisec connection, this e-mail is suppressed since otherwise incorrect info e-mails would be sent constantly for residual lites in ongoing operation.
However, the side-effect of the suppressed e-mails is that there is no information via e-mail about variant data that is actually missing. The message about a missing variant is always in the log of the ERP Stock Service, however.
See PF [AW-147159] + [AW-135791].

Within the stock comparison, there is still information about lacking variants via e-mail.
See PF [AW-195424].

#### 6.11.6. Restrictions
**General**
- Only dimension variants, but no color variants are considered.
- All referenced ERP items must keep dimension variants.
- Each Lisec stock will be synchronized with precisely one ERP stock. Here, a Lisec server is regarded as a Lisec stock.

**Problems due to the decoupling of the commercial inward goods in the ERP stock from the inward goods in the Lisec stock**
In the long run, the stock connection only functions smoothly if the inward goods in the ERP stock is executed in timely fashion with respect to the inward goods in the Lisec stock. If the commercial GR is delayed, the correction is made with the next cyclical stock reconciliation, whereby there can be an incorrect determination of the prices in the ERP stock. The solution is always the commercial IG booking.

#### 6.11.7. Information about the Lisec stock system
The Lisec version numbers follow the notation "02.00.000" or "02.x.y" (new crane system). ("2.71" is an older version (old crane system).)
Between the crane systems, there are, among other things, mechanical differences.
For the current crane generation, V02.00.007 is required (status as of 02/02/2023).
With a converter, the old V2.71 can be used, however not all functions can be used with it.

A crane system recognizes 2 modes:
1. Glass stock for Lisec and glass info from third-party system
2. Glass stock with third-party system and start location from third-party system

In the documentation for V2.71, both modes are described.
With the conversion to the new crane system, the documentation was split. Each mode is described in an individual document.
See also PF [AW-135791].

## 7. Function description with A+W Enterprise
### 7.1. Process diagram
To understand the process, use the process diagram. Had initially been created and optimized for Bystronic interface.

