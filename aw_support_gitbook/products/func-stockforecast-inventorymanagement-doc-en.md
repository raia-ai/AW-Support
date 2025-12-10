---
title: "EN-FUNC-AW_Clarity_Experience_Stock_Forecast"
source: "EN-FUNC-AW_Clarity_Experience_Stock_Forecast.pdf"
tags: ["A+W Clarity Experience", "Stock Forecast", "Inventory Management", "Software Functional Description", "ERP", "Glass Industry", "A+W Enterprise", "Inventory Control"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a functional description for the A+W Clarity Experience - Stock Forecast module. It details the module's purpose, features, prerequisites, and restrictions for optimizing inventory control and reducing operating costs in the glass industry."
long_description: "This functional description provides a comprehensive overview of the A+W Clarity Experience - Stock Forecast module, identified by article numbers 200041 and 200042. The module is an extension for the A+W Enterprise ERP system, designed to help businesses monitor stock inventories, forecast future trends, optimize inventory management, and ultimately reduce operational costs. The document outlines the module's core functionality, which includes displaying stock-critical items, visualizing future stock development by considering backorders, expected receipts, and consumptions. It details the system prerequisites, such as the required A+W Enterprise version, AWSOA-Infrastructure, and correctly maintained warehouse master data. A full list of functions is provided, covering features like stock history visualization, advanced filtering options, drill-down capabilities, and data export to CSV. The document also clearly states the module's limitations and restrictions, such as variable loading times and specific handling for multisite installations."
---

# A+W Functional Description: A+W Clarity Experience - Stock Forecast

**A+W - Software for Glass**

---
## 1. Content

*   **2. Notes on this Document**
    *   2.1. Trademarks
    *   2.2. Copyrights
    *   2.3. Exclusion of liability
*   **3. Performance Description**
    *   3.1. Data
    *   3.2. Description
    *   3.3. Prerequisites
    *   3.4. List of functions
    *   3.5. Restrictions
    *   3.6. Notes
*   **4. Contact Address**

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation might also be registered trademarks or other property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2023 A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions that have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance Description

### 3.1. Data

| **Produkt** | **A+W Clarity Experience** |
| :--- | :--- |
| **Artikelnummer** | 200041, 200042 |
| **Modul** | A+W Clarity Experience - Stock Forecast |
| **Kurzbeschreibung** | It is a module to monitor the inventories of stocked items and forecast future inventory trends. The aim is to optimize inventory control and, in this context, to reduce operating costs. |
| **Verfügbar** | QR[2306] |

### 3.2. Description

The module displays stock-critical items in a simple way and enables an overview of the future stock development. Backorders, initial stock, expected goods receipts, expected consumptions are taken into account and the final stock at the end of the selected point in time is displayed. In addition, a graphical visualization of the inventory development is provided. The module offers three standard indicators or filters to display items that are "Out of stock", "Under minimum" or "Under alarm stock". This also makes it easy to see temporary stock shortages within the time period. The user can monitor and control stock levels in an intuitive way. This results in the possibility to avoid overstocks and shortages in the warehouse and to ensure availabilities for customer orders.

### 3.3. Prerequisites

*   A+W Enterprise 6 (single oder multisite) – QR2302
*   AWSOA-Infrastructur / ICE-Configuration / LINUX 7
*   Warehouse master data is correctly maintained (stock change indicator, no incorrect postings, standard warehouse defined, etc.)
*   Close open purchase orders and orders (wlppms.b_status) that were not closed correctly (e.g. order from 2 years ago without goods receipt)
*   Recommendation: Computer monitor (>= 27 Inches)

The A+W side PS effort depends on the data quality of the customer. With correctly maintained master data, an installation and short introduction is necessary. In addition, the environment variables for the module are to be set up with the customer in this context. The module offers the possibility of the announcement of customer-individual data (3 fields), for which a Stored Procedure is to be written. If this is done by A+W, then there is further PS effort here. A master data optimization and/or training is to be offered separately.

### 3.4. List of functions

*   Display of the stock history of selected items
*   Visualization of stock history of selected article (incl. minimum and alarm stock)
*   General filter options by time period, warehouse, project, article number, purchasing department, article type, order number (multiple selection)
*   Display of relevant item data such as initial stock, backlog, open/alert orders, final stock, replenishment time, average consumption
*   Drill-down of article data to (dimension) variant level
*   Three standard metrics to view and filter items that are "Out of Stock", "Below Minimum" or "Below Alarm Stock".
*   Opening of detailed stock history. Grouping by day, week and month
*   Display of orders (order and item level), backorders and purchase requisitions
*   Displaying orders (order and item level) and backorders
*   Hiding and showing of fields
*   Change of field order and size
*   Definition of three private fields (data is filled by customer-specific SP)
*   Grouping of fields and filtering by field values
*   Export of the respectively displayed table data to *.csv

### 3.5. Restriktions

*   Depending on the number of items and filters, the module loading time may vary
*   Inventory history does not show historical values
*   No stock forecast on dimension variant level
*   For articles with size and color variants, only the "variable variant" may exist
*   The filter by warehouse number allows inventory forecasting according to the warehouse related item inventories. The other filter fields have an effect on the selection of articles (cross-stock inventory forecast)
*   In multisite installations, only the warehouse data of the login house for the logged-in employee is displayed at any time

### 3.6. Notes

*(This section is empty in the original document.)*

## 4. Contact Address

**A+W Software GmbH**  
Siemensstraße 3  
35463 Fernwald  
Germany

**Tel.** +49 641 96620-0

**E-Mail:** info@a-w.com  
**Internet:** http://www.a-w.com/
