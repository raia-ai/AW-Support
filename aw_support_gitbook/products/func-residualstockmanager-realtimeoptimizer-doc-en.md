---
title: "EN-FUNC-AW_Residual_Stock_Manager"
source: "EN-FUNC-AW_Residual_Stock_Manager.pdf"
tags: ["A+W", "Residual Stock Manager", "Glass Software", "Realtime Optimizer", "Stock Management", "Functional Description", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A functional description of the A+W Residual Stock Manager module. This document outlines the module's purpose, which is to enable the reuse of residual glass plates in upcoming cutting batches. It covers the module's data, requirements, functions, and limitations, explaining how it integrates with the A+W Realtime Optimizer to improve material yield."
long_description: "This document provides a detailed functional description of the A+W Residual Stock Manager, a software module designed for the glass processing industry. The module's primary function is to manage and reuse residual glass plates, thereby optimizing material usage and reducing waste. It integrates with the A+W Realtime Optimizer and can be accessed via a web interface, allowing users to save, process, and track residual plates without direct machine assistance. The documentation outlines the technical requirements, including compatibility with the MCStockMasterControl interface used by third-party storage systems like Hegla or Bystronic. It details the core functionalities, such as manually creating and editing residual plates, changing their dimensions or storage locations, and selecting specific plates for optimization in cutting batches. The document also highlights current limitations, for instance, that scheduling is only for end pieces of a stock plate and that full stock plate management requires additional logic. The guide is intended for users and system administrators to understand the module's capabilities and integration points within the A+W software ecosystem."
---

# A+W Functional Description: A+W Residual Stock Manager

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
    *   3.5. Limitations
    *   3.6. Notes
4.  **Contact Address**

---

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation might also be registered trademarks or other property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2019, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation must be copied, completely or in part, saved, or transferred only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions that have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| **Product** | A+W Realtime Optimizer (220016), A+W Realtime stand-alone (220903) |
| :--- | :--- |
| **Module number** | 220079 / 230079 |
| **Module** | A+W Residual Stock Manager |
| **Brief description** | Module for reuse of residual plates in upcoming cut batches |
| **Available** | Starting with A+W Production v6 |

### 3.2. Description

With the A+W Residual Stock Manager, you can save and process residual plates without machine assistance. For this purpose there is a web interface that can be opened from anywhere via a browser. The stored residual plates are then automatically available in the A+W Realtime Optimizer for further processing.

### 3.3. Requirements

It must be guaranteed that the stock serves supports the interface (MCStockMasterControl) used by the A+W Realtime Optimizer. This interface already provides communication to third-party storage systems such as Hegla or Bystronic.

### 3.4. List of functions

*   The cutting dialog shows in which manual slot a residual lite is to be stored or from which it is to be removed.
*   You can create residual plates manually, defining the glass type, glass thickness, storage location/warehouse location, and dimensions of the residual plate.
*   You can change the dimensions of a created residual plate.
*   You can change the storage location of a created residual plate.
*   You can change the glass type and thickness of a created residual plate.
*   In the course of table optimization in the A+W Realtime Optimizer, you can select individual residual plates that can be used for the optimization.

