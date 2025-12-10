---
description: "A+W Business - External Site Capability and Replication"
---


# A+W Functional Description: A+W Business - External Site Capability and Replication

---
## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The greatest care was used in compiling the texts and figures. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights
© 2017, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Without the prior written permission of A+W Software GmbH, the documentation may not be transmitted electronically, by recording or in any other form.

### 2.3. Exclusion of liability
A+W Software GmbH assumes no liability for data errors that rely on basic principles of the standard functions made available by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All adjustments, expansions, database queries, reports, analyses, and interface expansions that were created individually for our customers and/or machines and software partners as well as all costs and efforts associated with these were borne by the client (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary in order to ensure that the adjustments/expansions commissioned that were undertaken/developed for a version will also work perfectly and be used in the subsequent version.

## 3. Performance Description

### 3.1. Data

| | |
|---|---|
| **Product** | A+W Business |
| **Module number** | 210003 / 230003 Master Data Replicator |
| **Module** | External site capability and replication |
| **Brief description** | Possibility to use separate databases for the mapping of several operations and copy of the master data from a master to one or more slave databases |
| **Available** | In all A+W Business und A+W Business Pro versions |

### 3.2. Description
The external site management includes the possibility to use separate databases to map several operations/business units/profit centers of a corporate group on a central server system.

Central master data management is done using master data replication for customers, items, prices, product groups, conditions, and particular system parameter settings from the company table from a master database to the databases for the individual sites.

Orders between the sites of the individual separate databases are made by Purchasing via EDI communication.

For the group statistics, there is a combination of the statistics of all company units through import of the slave statistics into the master database via ASCII interface.

### 3.3. Requirements
The following modules are required for the EDI communication:
- EDI Export - Module 12
- EDI Import - Module 11
- Item referencing – Module 116
- Import of standard shapes – Module 117

The following modules are required for the group statistics:
- Sales statistics - Module 15
- Super statistics – Module 16

During the configuration, work is required for the:
- Creation of the databases according to customer requirements
- Setup of the replication according to customer requirements
- Setup of the group statistics according to customer requirements
- Setup of the EDI transfer according to customer requirements

### 3.4. List of functions
- **Several databases for autonomous company units**
- **Central master data maintenance in a central database (master database)**
- **Replication**
  Through master data replication of customers, items, prices, product groups, conditions, and/or particular system parameter settings, this centrally-maintained master data is synchronized with the other databases (slave databases).

  Replication thus serves to transmit the data from the main company of a corporate group to its branch offices/branches. For this, it is necessary to create the necessary data structures in all databases in which the changed or new data of the main company should be saved. By means of replication, the data will be distributed from headquarters to all sites, to be added or updated. In order to be able to collect the data that has been created anew or changed in the database of the main company, the so-called triggers must be installed there. Triggers are database processes that can respond to events such as Insert or an update.

  In the main company's database, all branch offices must be created to which these selected data records should be replicated. In the branch offices, all data fields in the management program for products, customers/suppliers/partners, and company parameters are initially deactivated. In order to be able to maintain individual data that differs from the central office, so-called local fields are defined. This makes sense, for example, for the route in the customer master data. The definition of this local data is done in the management program for replication. With activated replication, the management dialogs for the products, customers, and company parameters are in a position to detect which fields contain local data and which do not. Accordingly, fields that are not local can no longer be edited by the user.

  In order to select data records in the receiving branch office and edit them, there is the locking identifier "replicated" in QBE mode. The data marked this way in the system is only available if the editor has viewed and edited the data and then set the locking identifier to "not locked."

  In the receiving branch offices, it is important that nothing more be changed in the existing catalog data since a replication may otherwise no longer take place correctly. To guarantee this, the rights must be created appropriately for all users. Rights should be allocated in such a way that new data can be created, but existing data cannot be changed.

  The replication creates the data based on so-called Jobs. In these jobs, it is specified which tables of the main company should participate in the replication. Tables can also be explicitly excluded from the replication. The tables that are deactivated manually are never transferred by the replication.

  In order to be able to replicate data for the branch offices, in the main company an automatic task for the ALFAK Interface Service must be created. The function called in this formula carries out an export of the replication data. The data will be saved in the directory defined for the subsidiary in replication management. In each branch office, an automatic task for the ALFAK Interface Service must also be created in which the appropriate import formula is attached. This formula reads in all import files for this branch office (from the directory specified in the replication management) and creates a receipt for each of these files.

  This completes the replication cycle. The result must be emailed and also appears on the ALFAK Service Monitor.

- **The following functionalities for internal site capability are also available**
  - Storage of PP area-dependent procurement types per product and customer
  - Assignment of the employees to AV areas, possible delimitation of the organizational units
  - Mapping of a multi-step production through internal procurement in the organizational areas (only in connection with Purchasing)
  - Automatic order exchange between sites and AV areas using automatically-generated internal orders with individual price calculation according to adjustable conditions
  - Calculation of the base glass consumption per organizational unit in a particular time frame or by number manager. The accounting is done on the basis of the total consumption per product, separated by shapes.
  - Definable transfer to the financial accounting per site in various FinAc systems or various sites within a FinAc system

- **Group statistics**
  - Combination of the statistics of all company units through import of the slave statistics into the master database via ASCII interface
  - Data transmission of the ASCII file via DFÜ, router or e-mail
  - Statistics functions analogous to sales statistics
  - In addition, the sales statistics can be evaluated on the company or unit level

- **Order between the sites of the individual databases via EDI communication**
  - Prerequisite: The individual company units must be defined among one another as customer and/or supplier
  - Export of orders per database/site in a pre-defined data format incl. all technical product descriptions, prices, and conditions
  - Import of customer orders per database/site using standardized interface
  - File transfer via DFÜ, router or e-mail
  - Reference tables for items and/or BOM combinations of the individual database
  - Grille and shape detection
  - Conversion of DXF files into the internal S&N format
  - Calculation of the products based on stored customer conditions
  - Determination of the material primary costs.

### 3.5. Limitations
If the master data of the master database and the branch office databases are already different, then the replication is no longer in a position to combine these. It makes sense to create the databases for the branch offices from the master database.

The schema for all participating databases must always match exactly.

It is important that the base number ranges of the main company and the branch offices do not overlap. This would mean that data that is maintained in the branch offices would be overwritten by the replication.

No data can be deleted by the replication. For customers/suppliers and products, however, there can be a shutdown. For price conditions, there is no possibility for deletion. Here, the validity date can be used to deactivate a condition.

User guidance for the local fields in the branch offices is only supported graphically in the management programs for customers, suppliers, partners, items, and company parameters.

## 4. Contact Address
**A+W Software GmbH**  
Siemensstraße 3  
35463 Fernwald  
Germany

**Tel:** +49 641 96620-0  
**E-mail:** info@a-w.com  
**Internet:** http://www.a-w.com/

---
*A+W - Software for Glass*
