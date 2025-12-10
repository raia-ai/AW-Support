---
title: "EN-FUNC-AW_Gestellpool_Europe_Connector"
source: "EN-FUNC-AW_Gestellpool_Europe_Connector.pdf"
tags: ["A+W Software", "Gestellpool Europe Connector", "Logistics Optimizer", "Functional Description", "Glass Software", "CSV Import", "Rack Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a functional description of the A+W Gestellpool Europe Connector. It details the interface for importing rack pick-up information via a CSV file into the A+W Logistics Optimizer, outlining prerequisites, functions, and data specifications."
long_description: "This is a functional description for the A+W Gestellpool Europe Connector, an interface module designed to integrate Gestellpool Europe with the A+W Logistics Optimizer. The document explains how the connector facilitates the import of rack data, specifically information about racks ready for pick-up, from Gestellpool Europe into the A+W system. The import is handled via a CSV file. The guide covers the product details, prerequisites for use (requiring Gestellpool Europe and one of the A+W logistics modules like Smart Delivery or Logistics Optimizer), and a step-by-step list of functions, including how to access the import feature. It provides a detailed breakdown of the CSV file structure and the 'GPE rack header' data fields, specifying which are used. It also outlines the process after import, such as geolocating pick-up addresses and planning them into routes. The document concludes with restrictions, noting the lack of a web service and the need for manual checks on packaging dimensions, along with contact information for A+W Software GmbH."
---

# A+W Functional Description: Gestellpool Europe Connector

**A+W - Software for Glass**

---

---
## 1. Contents

1.  **Contents**
2.  **Notes on this document**
    *   2.1. Trademarks
    *   2.2. Copyrights
    *   2.3. Exclusion of liability
3.  **Performance Description**
    *   3.1. Data
    *   3.2. Description
    *   3.3. Prerequisites
    *   3.4. List of functions
        *   3.4.1. Interface description
        *   3.4.2. GPE rack header
    *   3.5. Restrictions
    *   3.6. Notes
4.  **Contact Address**

---

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation can also be registered trademarks or other property rights of third parties. Third-party copyrights must therefore be observed.

### 2.2. Copyrights

© 2022, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions that have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions that have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | Gestellpool Europe Connector |
| **Article no.** | 262030 |
| **Module** | A+W Logistics Optimizer - Gestellpool Europe Connector |
| **Brief description** | Interface for the import of information (CSV file) for racks that are ready for pick-up |
| **Available** | QR2210 |

### 3.2. Description

The Gestellpool Europe Connector is an interface between Gestellpool Europe and the A+W Logistics Optimizer. With this interface, racks from the Gestellpool Europe ready for pick-up can be imported via CSV file into the A+W Logistics Optimizer.

### 3.3. Prerequisites

Prerequisite is the use of Gestellpool Europe and one of the modules:
- A+W Smart Delivery
- A+W Smart Delivery Maps
- A+W Logistics Optimizer

### 3.4. List of functions

From the A+W Logistics Optimizer, click the `Pack...` button...

*Image of the A+W Logistics Optimizer interface, showing a map on the left and a grid of packaging data on the right. A button labeled "Import GPE" is highlighted.*

... to reach the Import GPE button. This button is only available if the license for the Gestellpool Europe Connector is in use.

*Image of the "Data Import" window. The "Packaging: GestellPool" option is selected. A file path is shown for a CSV file. Below, a preview of the CSV data is displayed in a grid, showing columns like "A-Gestell mittel", "Abholbereit", etc.*

After execution of the import, the A+W Logistics Optimizer writes the pick-up address into a geolocation (address, latitude and longitude), which is assigned to a real map.

If a geolocation is not found or if more than one is found, the packing action is marked as geolocation error so that it can be geolocalized by the user.

After the import, these packing actions can be planned into a route --> Route planner > Packing tab.

*Image of the A+W Logistics Optimizer interface after import. The map shows various locations marked with packaging icons. The data grid lists imported racks with a "Collected" status and details like barcode, customer name, and geolocation data.*

### 3.4.1. Interface description

**GPE - CSV file example**

The CSV file contains the following header fields:
`Group;plant;number;reference;product;status;description;last comment;last movement;last movement by;GPE customer number;customer name;customer number;delivery address;reporting date;supplier group;supplier plant;delivery date;in hand;outgoing goods route;outgoing goods route stop;contact on-site;pick-up location;pick-up route;pick-up route stop;barcode number;packaging ID`

**Example Data Rows:**
```csv
002;160;203000047;10279848;A-rack medium;ready for pick-up;A-rack medium;beds 1;20.03.2022 10:41:17;marvin_gortmann;K38750;Duinkerke Glasservice BV;1515050;Steenoven 6 , 3911 TR, Rhenen;03.03.2022 10:38:00;002;150;20.03.2022 10:41:17;45;19;5;;Steenoven 6, 3911 TR, Rhenen;;;002160203000047;2
002;160;203000242;218864;A-rack medium;ready for pick-up;A-rack medium;;25.03.2022 14:01:27;KY-621;K30121;Tietjen Holz-Kunststoff-;800313;Huchtinger Straáe 18, 28197, Bremen;08.03.2022 10:13:00;002;160;25.03.2022 14:01:27;14;706;;;Huchtinger Straáe 18, 28197, Bremen;;;002160203000242;2
002;160;203000352;2215520;A-rack medium;ready for pick-up;A-rack medium;;24.03.2022 00:00:00;NO_USER;K14713;Fenster 2000;2215520;Georg-Leppien-Str. 21, 21337, Lüneburg;25.08.2019 00:00:00;002;160;24.03.2019 00:00:00;63;;;;Georg-Leppien-Str. 21, 21337, Lüneburg;;;002160203000352;2
```

### 3.4.2. GPE rack header

Type "GPE"

| Spalte -DE (German) | Index | Description | Example Value | Format |
| :--- | :--- | :--- | :--- | :--- |
| Gruppe | 0 | Group | Not in use | --- |
| Werk | 1 | Plant | Not in use | --- |
| Nummer | 2 | Packaging Id | 203000047 | Integer |
| Referenz | 3 | Reference | Not in use | --- |
| Produkt | 4 | Packaging Type Name | A-Gestell mittel | String |
| Status | 5 | Status | Not in use | --- |
| Beschreibung | 6 | Packaging Description | A-Gestell mittel | String |
| Letzte Bemerkung | 7 | Last remark | Not in use | --- |
| Letzte Bewegung | 8 | last movement | Not in use | --- |
| Letzte Bewegung durch | 9 | Last move through | Not in use | --- |
| GPE-Kundennummer | 10 | GPE customer number | Not in use | --- |
| Kundenname | 11 | Customer Name | A+W Software GmbH | String |
| Kundennummer | 12 | Customer number | 1515050 | Integer |
| Lieferadresse | 13 | Shipping address | Not in use | --- |
| Freimeldedatum | 14 | Release date | Not in use | --- |
| Lieferant-Gruppe | 15 | Supplier group | Not in use | --- |
| Lieferant-Werk | 16 | Supplier factory | Not in use | --- |
| Lieferdatum | 17 | Delivery date (Pick up date) | 20.03.2022 10:41:17 | Date (yyyy-MM-dd) |
| Im Besitz | 18 | In possession | Not in use | --- |
| Warenausgang-Tour | 19 | Goods issue tour | Not in use | --- |
| Warenausgang-Tourstopp | 20 | Goods issue tour stop | Not in use | --- |
| Kontakt vor Ort | 21 | Contact on site | Not in use | --- |
| Abholort | 22 | Pickup location | Steenoven 6, 3911 TR, Rhenen | --- |
| Abholung-Tour | 23 | Pickup tour | Not in use | --- |
| Abholung-Tourstopp | 24 | Pick up tour stop | Not in use | --- |
| Barcodenummer | 25 | Barcode number | 002160203000047 | String |
| Packmittel ID | 26 | Packaging Type Id | 2 | Integer |

### 3.5. Restrictions

A CSV file is used for the transport of the information. No Web service!

The Gestellpool Europe Connector does not provide any information about the packaging type such as width, height, depth, etc., so that after the first import of a new packaging type, the Gestellpool Europe interface automatically initializes the packaging type, but this must absolutely be checked by the user since otherwise the freight optimization does not have the corresponding dimensions in order to optimize the cargo space of the truck.

### 3.6. Notes

(No specific notes are listed in this section of the document.)

---

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0
E-mail: info@a-w.com
Internet: http://www.a-w.com/
