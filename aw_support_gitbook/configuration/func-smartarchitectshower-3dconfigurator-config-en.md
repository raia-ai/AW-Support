---
description: "A+W Smart Architect Shower Functional Description"
---


# A+W Functional Description: A+W Smart Architect Shower

[Image: A hand placing the final piece into a jigsaw puzzle, overlaid with architectural and digital graphics, symbolizing a complete software solution.]

**A+W - Software for Glass**

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

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2023, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied, in whole or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions that have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Smart Architect Shower |
| **Article Number** | 264106 |
| **Module** | A+W Smart Architect Shower |
| **Brief description** | Integration of a 3D shower door configurator with dimensional corrections, glass processing, hardware parts and other fittings (such as sealing profiles, stabilizing strips, etc.) in A+W Enterprise (still under development) / A+W Business |
| **Available** | for pilot installation |

### 3.2. Description

This module includes the shower configuration and its integration into the order and quotation entry of A+W Business or A+W Enterprise by an import of the glasses, their machining and hardware parts, so that in one order/quotation different product types (shower, IGU, LG, TG ...) can be mixed.

### 3.3. Requirements

This tool requires:

**For the design / configuration:**
*   A+W Business or A+W Enterprise
*   A+W CAD Designer

**For machine control:**
*   A+W Business Pro or A+W Production
*   Machine connector

The shower configurator is installed on a system provided by the customer, which meets the following requirements:
*   Windows 10 / Windows Server 2016 and later
*   IIS enabled
*   SQL Server
*   Docker Engine executable
*   Stable internet connection (25 Mbit/s or higher)
*   At least 100 GB of free hard disk space
*   At least 8 GB usable RAM memory
*   At least 2 x 2.6 GHz processor
*   Access via RDP for maintenance purposes

### 3.4. List of functions

The module makes it possible to open the shower configurator via a button in the order and quotation entry (item level) and configure a shower in the new 3D Designer configurator. In doing so, the dimensions for the glass components, their machining and the hardware parts with technical restrictions and rules are automatically deducted to simplify the input and reduce errors and time.

The price calculation is performed by the A+W system (A+W Business or A+W Enterprise). The price calculation must be started by the user himself. In case of incorrect calculation (e.g. due to missing master data / prices), the system will issue a corresponding message.

The configured shower will be automatically imported into A+W Business or A+W Enterprise in different items (one item per glass or fitting part) when closing the shower configurator. A 3D image of the shower to be printed will also be available in A+W Business or A+W Enterprise.

Each configured shower is linked to the order/quotation and its items in the A+W ERP system via an internal ID, which makes it possible to reopen the shower in the configuration directly from A+W Business / A+W Enterprise and make changes if necessary.

The imported items are complete with bill of materials, so that a machine control can be created as usual in the A+W production software, which in turn saves time and errors and increases product quality.

The shower configurator uses DXF files for the macros of the fittings.

**Existing functionalities:**
*   Change model shape
*   PDF Download
*   DXF Download
*   Shower installation situations: niche, corner, U-shower, bath tops
*   Own validation rules
*   Gap dimensions input, min & max range (glass)
*   Activate and deactivate shower tray
*   Multilingual (default translation) language (DE, EN-UK, EN-US, ES)
*   Multilingual (own translation / no default language)

**Existing, but faulty:**
*   3D room design (standard colors, standard floors, ...)
*   3D room design (definition of own colors, floors, walls)
*   3D room - upload image

**Currently not available functionalities:**
*   Replace individual fittings
*   Separate individual glass treatments
*   Shower installation situations: Walk-in, 5-corner shower, round, on bathtub, special installation situations (created by customer)
*   Automatic beveled edge (bottom / top) over the whole installation situation
*   second unit of measurement (INCH & CM)

### 3.5. Restrictions

At this stage, the Showers Configurator is only connected to the local A+W Business / A+W Enterprise. There is no integration with A+W iQuote and not accessible via the public Internet.

Items from a configuration cannot be edited subsequently in the A+W system. These are locked for the user. All adjustments must be made in the configurator.

The 3D area can only be used if the A+W Business / A+W Enterprise server contains a sufficiently powerful graphics card.

The 3D area in the configurator is deactivated when the configurator is delivered. Can be activated after consultation. This can lead to performance problems if the graphics power is too weak.

### 3.6. Notes

The macros required for the fittings are not part of the configurator. These must be created by the customer.

---

## 4. Contact Address

**A+W Software GmbH**

Siemensstraße 3  
35463 Fernwald  
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com  
Internet: http://www.a-w.com/
