---
title: "A+W iCut (EL) Functional Description"
source: "EN-FUNC-AW_iCut.pdf"
tags: ["A+W iCut", "Glass Software", "Cutting Optimization", "Functional Description", "A+W Software", "EL Version", "Manual Cutting", "Software for Glass"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Functional description of A+W iCut (EL), an integrated optimization and cutting software designed for small glass companies. It covers features for order entry, optimization, stock management, and control of cutting tables."
long_description: "This document provides a detailed functional description of A+W iCut (EL), a software solution by A+W Software GmbH. A+W iCut (EL) is a 2-station system designed for small companies that manage their glass cutting processes manually. It facilitates order entry for various glass types (insulated, LAMI, TG, single glass), optimization of cutting plans, and control of standard cutting tables. The software includes features for managing stock, handling residual plates, and calculating cutting dimensions for standard shapes. It offers two working modes: a standard mode for quick processing and an expert mode for detailed control over optimization. The document outlines the system's core functions, requirements (Windows 10/Server 2019, .NET Framework 3.5), optional enhancements like the A+W Barcode Manager, and notable limitations, such as the lack of support for advanced processing, price calculation, or integration with external production systems. It also lists modules that are not compatible with A+W iCut (EL)."
---

# A+W iCut (EL)

---
## Contents
1.  [Contents](#contents)
2.  [Notes on this document](#notes-on-this-document)
    -   [Trademarks](#trademarks)
    -   [Copyrights](#copyrights)
    -   [Exclusion of liability](#exclusion-of-liability)
3.  [Performance Description](#performance-description)
    -   [Data](#data)
    -   [Description](#description)
    -   [Requirements](#requirements)
    -   [List of functions](#list-of-functions)
    -   [Optional enhancements of the basic module](#optional-enhancements-of-the-basic-module)
    -   [Limitations](#limitations)
    -   [Notes](#notes)
4.  [Contact Address](#contact-address)

## Notes on this document
This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### Copyrights
© 2020, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of A+W Software GmbH.

### Exclusion of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions that have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## Performance Description

### Data
| | |
| :--- | :--- |
| **Product** | A+W iCut (EL) |
| **Module number** | 235001, 235002 |
| **Module** | A+W iCut (EL) |
| **Brief description** | Integrated optimization and cutting software for small companies |
| **Available** | July 2020 |

### Description
A+W iCut (EL) is a 2-station system (in the office and at the cutting table) for order entry, optimization, and cutting control. The target group for A+W iCut (EL) is small companies that organize their cutting primarily manually and using production documents. A+W iCut (EL) allows the input of orders without price calculation for insulated glass, LAMI, TG, and single glass including edge processings and standard shapes. The system manages the optimization and cutting. In addition, A+W iCut (EL) allows stock management and residual plate control.

The optimization can be done both in chaotic and in sorted mode. Broken sheets can be re-optimized manually. The printing of labels and visualization of cutting plans can be done on the cutting table.

A+W iCut (EL) offers 2 working modes:
-   **Standard mode:** in this mode, the optimization process and production release are done with a mouse-click.
-   **Expert mode:** this mode allows control of the individual planning and optimization steps and thus also the optimization result.

### Requirements
-   Windows 10 or Server 2019
-   Microsoft.NET Framework 3.5

### List of functions
A+W iCut (EL) supports the following functions and processes:
-   **Order entry**
    -   Entry of IG, LAMI, TG, and single sheets
    -   Entry of edge processings (for calculation of the correct cutting dimensions)
    -   Entry of standard shapes from the A+W shape catalog
    -   Calculation of the total order price based on manually input item prices
    -   DXF import for the order entry with shape 99
-   **Stock**
    -   Manual stock receipt bookings (no purchasing module)
    -   Automatic stock removals by the optimization
-   **Optimization/use of residual plates**
    -   The system offers the opportunity to create and maintain a stock for residual plates
    -   Residual plates can be added manually to the residual plate stock
    -   The optimization primarily uses the stock sheets that provide the "best result" with regard to costs and yield, and only then the residual plates
    -   If the use of a residual plate is desired despite poorer yield or costs, this can be controlled manually (priority)
-   **Control of standard cutting tables**
    -   The system offers the data transfer and control of cutting tables
    -   Only commonly used standard cutting tables are supported. Please contact A+W Sales before the project (during the quotation phase) in order to ensure that the machine type you are using is supported.
    -   Edge stripping for IG is supported

### Optional enhancements of the basic module
-   **A+W Barcode Manager (EL)**
    A+W iCut (EL) supports data exchange with the A+W Barcode Manager (EL). You can use this module to report breaks and defects and then to optimize.
    -   230101 A+W Barcode Manager (EL) - Basic license
    -   230102 A+W Barcode Manager (EL) - Concurrent user license
    -   230105 A+W Barcode Manager (EL) - Glass Remake Manager
-   **235002** A+W iCut (EL) Concurrent user license (additional user)
-   **230018** Excel Line Item Import
-   **230011** EDI-Import and Export (only the import is supported, not the export)
-   **230115** A+W Shape Optimizer

### Limitations
The following functions and processes are not supported by the order entry:
-   No additional processings such as drilled holes, surface processings, glass edge cuts, cut-outs, etc. are supported.
-   No FinAc connection is possible.
-   Price calculation and cost calculation are not supported.
-   No purchasing is supported.
-   No quotations can be entered.
-   No customer master data is supported. Only the customer address can be entered.
-   No statistics functions.

The following functions and processes are in the **organization area** and are not supported in the optimization:
-   **No coupling to external production software or display systems**
    It is not possible to connect A+W iCut (EL) to production software or display or external software providers' monitoring systems.
-   **No coupling to A+W Production modules**
    -   It is not possible to transmit data for the graphic display of production steps to A+W Production Terminal or A+W Production sTerminal (EL).
    -   It is not possible to transmit the optimized cutting patterns to the A+W Realtime Optimizer.

The A+W Business Barcode Manager (EL) can only make product and main process-specific bookings. A booking of sub-parts is not possible.

A+W iCut (EL) does **not** support the following modules:
-   200100 A+W iQuote (G)
-   262001 – 262010 A+W Logistics Optimizer
-   261001 A+W Analytics
-   264101 – 264103 A+W Smart Companion
-   200004 - 220931 A+W CAD Designer
-   210006 / 230006 A+W Rack Manager
-   210034 / 230034 A+W Gantry Interface
-   210009 / 230009 Document Management Connector
-   210010 A,B / 230010 A, B Fittings Catalog Connector
-   230013 A+W Production Terminal (EL)
-   230035 Document Transfer in openTRANS Format 2.1
-   230103 / 230104 A+W Capacity Planner (EL)
-   230120 Extended Optimizer
-   230080 – 230083 A+W Realtime Optimizer
-   230015 Delivery Check I
-   230121 Quote Optimization
-   230035 Door Order Entry: Fitting and Processings

### Notes
A+W iCut (EL) must be regarded independently of earlier A+W products. In particular, A+W iCut (EL) is not an upgrade product from earlier production solutions (such as ALFERT or XOPT2000, for example). Thus it cannot be guaranteed that all function characteristics of earlier products are available in this product.

A+W iCut (EL) allows an upgrade to a A+W Business PRO with the same master data.

Project work (configuration, training, reports and labels, ...) by A+W requires approx. 5-7 man-days.

## Contact Address
**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0
E-mail: info@a-w.com
Internet: http://www.a-w.com/
