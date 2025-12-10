---
description: "EN-FUNC-AW_Gantry_Interface"
---


# A+W Functional Description
# A+W Gantry Interface

---

---
## 1. Content

1.  **Content**
2.  **Notes on this Document**
    *   2.1. Trademarks
    *   2.2. Copyrights
    *   2.3. Exclusion of liability
3.  **Performance Description**
    *   3.1. Data
    *   3.2. Description
    *   3.3. Requirements
    *   3.4. List of functions
    *   3.5. Restrictions
    *   3.6. Notes
4.  **Contact Address**

---

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2021, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This also includes possibly necessary long-term costs and expenses for amending and extending subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Enterprise / A+W Business / A+W Business Pro |
| **Module number** | 200034 / 210034 / 230034 |
| **Module** | A+W Gantry Interface |
| **Brief description** | Module for synchronizing third-party storage (Bystronic/Hegla/Lisec) |
| **Available** | Starting with A+W Enterprise v5, A+W Business + Pro v5 |

### 3.2. Description

The A+W Gantry Interface is an interface for the synchronization of the stock of the A+W ERP stock systems with the Hegla, Bystronic and Lisec stock systems. Using the A+W Gantry Interface results in a more precise inventory synchronized with the physical inventories in the ERP glass stocks.

### 3.3. Requirements

This expansion is only available in connection with A+W Enterprise, A+W Business or A+W Business Pro and the appropriate stock interface from Hegla, Bystronic and Lisec.

**Gantry connection**

| Third-party stock interface | A+W ERP Stock Service | A+W Enterprise | A+W Business |
| :--- | :--- | :--- | :--- |
| Bystronic stock interface Version 3.2 or higher | Version 6 or higher | Version 6 or higher | Version 6 or higher |
| Hegla stock interface Version at least 2.1.0.0 or higher | Version 6 or higher | Version 6 or higher | Version 6 or higher |
| Hegla stock interface Version 2.2.0.0 or higher | Version 6 or higher | Version 6 or higher | Version 6 or higher |
| Lisec stock interface Versions 02.00.000 and 2.71 or higher | Version 6 or higher | Version 6 or higher | Version 6 or higher |

The A+W Gantry Interface must be licensed. Different licenses are required for the coupling of the different third-party stock systems.

### 3.4. List of functions

1.  **Integrated incoming goods**
    Only after recording of the incoming goods in the ERP system can the goods be stored in the portal stock. This functionality is optional.

2.  **Integrated outgoing goods**
    If there is a removal from third-party stock, the booking is reported online to the connected ERP system and the goods are removed from the corresponding ERP stock.

3.  **Automatic inventory/stock comparison**
    The stocks of the ERP stock systems can be synchronized automatically with the stocks of the third-party stock systems. The third-party stock system is always the leading system. Synchronization is done once every 24 hours. The time of the daily synchronization can be configured.
    -> Manual inventory of the ERP stock is no longer required.

4.  **Complex connection**
    The A+W Gantry Interface can connect several external stocks and even different external stock systems in an installation.

5.  **Separate ERP cover sheet stock**
    In the ERP system, the cover sheets are kept in a special stock.

6.  **Broken sheet treatment**
    Broken sheets will be removed from the ERP stock.

| | **Hegla 2.2** | | **Bystronic 3.2** | | **Lisec 02.00.000 and 2.71** | |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| | **AWB⁽¹⁾** | **AWE⁽²⁾** | **AWB⁽¹⁾** | **AWE⁽²⁾** | **AWB⁽¹⁾** | **AWE⁽²⁾** |
| **on 1.** | ✓ | ✓ | | x | | x |
| **on 2.** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| **On 3.** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| **On 4.** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| **On 5.** | ✓ | ✓ | x | x | ✓ | ✓ |
| **On 6.** | ✓ | ✓ | x | x | ✓ | ✓ |

**AWB⁽¹⁾:** A+W Business
**AWE⁽²⁾:** A+W Enterprise

### 3.5. Restrictions

*   Bookings and incoming goods are only recorded based on the incoming goods in the ERP system or inventory differences during automatic inventory.
*   In the course of permanent stock-keeping, no unplanned removals from stock are processed.
*   Outward bookings for items that are not present in A+W Enterprise Stock will be rejected, as are bookings that would cause negative inventories.
*   The predictive data in A+W Enterprise is not corrected with the outward booking since it is not known which items have been cut with the sheet. Correction of the predictive data is done as previously, using the planned cutting date.
*   The keeping of a separate ERP cover sheet stock is only possible with a Hegla or Lisec connection. With a Bystronic connection, this functionality is not available.
*   The removal of broken sheets from the ERP stock is only possible with a Hegla or Lisec connection. With a Bystronic connection, this functionality is not available.

### 3.6. Notes

The optional functionality *Integrated incoming goods* is the prerequisite for an exact value stock-keeping. If this functionality is not configured, attention must be paid that the incoming goods are recorded promptly in the ERP. Interim inventory changes, especially incoming bookings by the automatic inventory, cause an imprecise value stock booking.

---

## 4. Contact Address

A+W Software GmbH<br>
Siemensstraße 3<br>
35463 Fernwald<br>
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com<br>
Internet: http://www.a-w.com/
