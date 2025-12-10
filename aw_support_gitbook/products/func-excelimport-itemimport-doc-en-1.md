---
title: "EN-FUNC-AW_Enterprise_Excel_Import"
source: "EN-FUNC-AW_Enterprise_Excel_Import.pdf"
tags: ["A+W Enterprise", "Excel Import", "Item Import", "Software for Glass", "ERP", "Functional Description", "200018"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A functional description for the A+W Enterprise module 'Excel import of items' (Article no. 200018). This document outlines the module's capability to import order line items from a Microsoft Excel clipboard into the A+W Enterprise system. It details the process, requirements, functions, and limitations of the import feature."
long_description: "This document provides a detailed functional description of the 'Excel import of items' module for the A+W Enterprise software, specifically for versions starting with v6 QR 04/19. The module, identified by article number 200018, is designed to streamline order entry by allowing users to import line items directly from an MS Excel clipboard. The description covers two main takeover types: importing item dimensions for a pre-defined article and importing a complete order with article numbers. It outlines the step-by-step process, from copying data in Excel to mapping columns and transferring items into the order, including automatic price calculation and restriction checks. The document also specifies the system requirements (A+W Enterprise core module), lists the key functions such as data transfer and editing, and details important restrictions like the maximum number of lines (900), columns (10), and specific data fields that can be imported. Legal notices regarding copyrights, trademarks, and liability are also included, along with contact information for A+W Software GmbH."
---

# A+W Functional Description: A+W Enterprise - Excel import of items

---
## 1. Contents

1.  **Contents**
2.  **Notes on this Document**
    - 2.1. Trademarks
    - 2.2. Copyrights
    - 2.3. Exclusion of liability
3.  **Performance description**
    - 3.1. Data
    - 3.2. Description
    - 3.3. Requirements
    - 3.4. List of functions
    - 3.5. Restrictions
    - 3.6. Notes
4.  **Contact Address**

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2021, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions that have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance description

### 3.1. Data

| Product | A+W Enterprise |
| :--- | :--- |
| **Article no.** | 200018 |
| **Module** | Excel Line Item Import |
| **Brief description** | Import of line items from the MS Excel clipboard |
| **Available** | Starting with A+W Enterprise v6 QR 04/19 |

### 3.2. Description

The Excel Line Item Import module enables the import of order items that are transferred by the customer as Excel file.

There are 2 types of takeover supported:
- Takeover of item dimensions for an article defined in the A+W Enterprise order entry.
- Takeover of a complete order with reference to articles or customer article numbers. That is, in addition to the dimensions, the article numbers are also included in the Excel file.

The takeover is accomplished in the following steps:
- Marking of the data to be taken over in Excel and copying to the clipboard
- Assignment of the columns to the fields of the item
The Excel format used by the customer can be saved and reused for the next import. A renewed assignment of the columns to the field of the item is thus no longer necessary
- Takeover of the data on the import dialog
- If necessary, there can be an addition to/manipulation of the data transferred
- Takeover of the items in the order

Analogous to the manual input of the items, prices are calculated and restrictions and dates checked. If conflicts arise during the takeover of the items, the corresponding items are marked for reprocessing (Infostatus).

### 3.3. Requirements

- A+W Enterprise (core module)

### 3.4. List of functions

- Transfer of the data from the clipboard to a screen table
- Editing and selection of the data to be imported on the Import dialog
- Generation of the new items in the current document including price calculation and restriction check.

> **Image: Fremddaten - Import Dialog**
> The image displays the "Fremddaten - Import" (External Data - Import) dialog window within the A+W software. It shows a table grid with data ready to be imported.
> - **Columns:** LfdPos, Ku.Pos, Artikel, Ku.Artikel, Kommis., Menge, Breite, Höhe, SZR, SZR2, Pos 1:19, J/N.
> - **Data:** The table contains 19 rows, each representing a line item. All items share the same `Artikel` number (500055). The `Menge` (Quantity) is 1 for all items, while `Breite` (Width) and `Höhe` (Height) vary for each line. A checkbox at the end of each row (`J/N`) is checked, indicating the item is selected for import.
> - **Buttons:** At the bottom, there are buttons for `Import`, `Zuordnung` (Assignment), `Test`, `Übernehmen` (Apply), `Löschen` (Delete), and `Abbrechen` (Cancel).

### 3.5. Restrictions

- **Maximum 900 lines:**
  If the clipboard contains more than 900 lines, the import is terminated after 900 lines.
- **Maximum 80 characters column width:**
  If a field contains more than 80 characters, the content is shortened accordingly.
- **Maximum 10 columns**
- **Empty lines are skipped**
- **The import is restricted to the following fields:**
  - Customer item
  - Sequential item
  - Article number (A+W Enterprise - article)
  - Customer article
  - Quantity
  - Width
  - Height
  - AIR
  - AIR2
  - Reference
- **The data is expected in the metric system.**

### 3.6. Notes

*(This section is intentionally blank in the source document.)*

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-Mail: info@a-w.com
Internet: http://www.a-w.com/
