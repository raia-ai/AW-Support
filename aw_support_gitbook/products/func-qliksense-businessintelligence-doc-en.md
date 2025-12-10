---
title: "A+W Analytics for A+W Clarity - Functional Description"
source: "EN-FUNC-AW_Analytics.pdf"
tags: ["A+W Analytics", "QLIK Sense", "Business Intelligence", "Software for Glass", "Functional Description", "Data Visualization", "A+W Clarity", "ERP", "A+W Business", "A+W Production"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a functional description of A+W Analytics for A+W Clarity, a business intelligence (BI) solution powered by QLIK Sense®. It outlines the software's capabilities, requirements, and data visualization features for the glass industry."
long_description: "This functional description details the 'A+W Analytics for A+W Clarity' module, a web-based, self-service business intelligence (BI) tool developed by A+W Software GmbH. Powered by QLIK Sense®, the solution enables the visualization of data from A+W Clarity products (A+W Production and A+W Business) across multiple locations. The document covers the necessary requirements for implementation, including a QLIK Sense® server and appropriate database licenses. It explains the 'data loading architecture,' which processes data from live and archive databases into compressed QVD files for analysis. A significant portion of the document is dedicated to describing the standard visualizations provided, such as sales statistics, stock forecasts, work-in-process tracking, breakage analysis, production statistics, workload planning, waste statistics, and delivery reliability. It also discusses restrictions, noting its current compatibility with A+W Business and A+W Production, and outlines the process for custom adjustments and extensions."
---

# A+W Analytics for A+W Clarity powered by QLIK Sense®
---
## A+W Functional Description

A+W - Software for Glass

---

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2017, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This also includes possibly necessary long-term costs and expenses for amending and extending subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Clarity |
| **Module number** | 261001 |
| **Module** | A+W Analytics powered by QLIK® |
| **Brief description** | A+W Analytics powered by QLIK® is a fully web-based “self-service" BI tool. |
| **Available** | A+W Clarity v6, Q2.2017 |

### 3.2. Description

A+W Analytics is a BI solution for A+W Clarity, which enables the visualization of A+W Clarity data across locations and Web-based with state-of-the-art technologies from QLIK Sense®.

### 3.3. Requirements

#### 3.3.1. QLIK Sense®
The requirement for start-up is a QLIK Sense® server (www.qlik.com) with the rights and technical possibilities to access A+W databases. At a company with several locations, an A+W Analytics package per location and a QLIK Sense® server for the whole company are required.

#### 3.3.2. Database license
QLIK Sense® draws data from various A+W databases saved on different database servers. A database license for the QLIK Sense® server is required for each connected database server according to the license provisions of the database supplier in question.

A database license for each QLIK Sense® user is also required according to the license provisions of the database supplier in question. If the user also uses the A+W product in question, he should already have an appropriate database license.

#### 3.3.3. Data basis
A complete data basis is required for meaningful visualizations. For breakage statistics, precise breakage bookings are required, or for a WIP (Work in Process) evaluation, the costs must be maintained correctly in the master data and PDC bookings in production must be made completely.

#### 3.3.4. Maps
If you want to display your customers' data on maps, GEO coordinates are required. This information is not a component of A+W Analytics, however it can be added via a prepared Excel list. The maintenance of the list is the responsibility of the customer.

*[Image: Map of the northeastern United States showing customer locations plotted by net amount.]*

### 3.4. A+W Analytics - data loading architecture

The core of A+W Analytics is the "data loading architecture." With it, the data is loaded and compressed from the live and archive databases of the A+W Clarity products (A+W Production and A+W Business) for all connected sites.

The result is several QLIK data files (QVD files) with the compressed A+W Clarity data; these are required for visualizations. The field descriptions of the compressed data are in English, documentation of the data is included in an individual visualization APP. Information about the basis of the compressed data – the A+W databases can be taken from the A+W database documentation.

### 3.5. A+W Analytics - visualizations

A+W Analytics includes a package of standard visualizations when it is purchased. Insofar as the data is on hand and maintained at the purchaser/customer according to the requirements (for example, PDC data for breakage statistics), the standard evaluations are fully functional and can be copied and adjusted according to individual needs. Furthermore, the creation of completely individual QLIK Sense® visualizations is possible.

The standard visualizations included in the package with the purchase of A+W Analytics are available in English and German. Translations into additional languages are an additional service and are possible on request.

#### 3.5.1. Sales statistics by customer and supplier
The visualization shows the sales and costs of all orders, quotations, complaints, and credits from A+W Business. All sales are listed by fiscal year, customer, and supplier. There is a direct comparison of the current fiscal year with the last one.
An analysis of the existing quotations and a distinction between invoiced and not invoiced orders is possible.

*[Image: A collection of dashboards showing various sales statistics charts including bar charts, line graphs, and pie charts.]*

#### 3.5.2. Sales statistics by end product and all products
This visualization includes not just the orders, but all items and their BOMs from A+W Business. This enables an evaluation of the products on the item level and even on the BOM level. In this visualization it is possible, for example, to analyze particular processings on particular kinds of glass. Since the questions asked in this area are very individual, this visualization serves as a basis on which the individual visualizations can be constructed.

#### 3.5.3. Stock forecast
This visualization shows the current stock on hand and the current development for the next days from A+W Business.

*[Image: A dashboard showing stock forecast data, including bar charts and line graphs for current and forecasted stock levels.]*

#### 3.5.4. Work in process
This visualization includes the current value of production, divided by registration points, from the A+W Production data. Here it is necessary to maintain the master data in the A+W Clarity systems, which is possible starting with Version 6; in addition, production must be controlled by PDC bookings.

*[Image: A chart showing the value of work in process per registration point.]*

#### 3.5.5. Breakage statistics
This visualization includes all breaks reported by A+W Production, broken down by reasons and registration points. If the master data allow, in addition to the number, the times and costs of the breaks are also listed.

*[Image: A dashboard with bar charts and key performance indicators related to breakage statistics.]*

#### 3.5.6. Production statistics
This visualization displays the products produced with A+W Production. The data includes all processings that are defined via an A+W standard processing type. The visualization enables the display of information about individual areas and processings, such as drillings, edge processings, and IG production. Since the questions asked can be very individual, this evaluation serves as the basis for creating targeted evaluations.

*[Image: A dashboard with bar charts, pie charts, and key metrics related to overall production statistics.]*

#### 3.5.7. Workload
The visualization displays the current workload without A+W Capacity in A+W Production. The basis is the production date of the batch. The visualization includes a general overview and a detailed view tailored to IG production. This visualization can be used as basis for the requirements of the production in question if the planning is organized solely via the dates of the batches.

*[Image: A dashboard displaying workload statistics through various charts and graphs.]*

#### 3.5.8. Batch overview
This visualization displays all batches booked via A+W Production. It is possible to filter the associated orders by the batch number or by order number of the associated batches.

#### 3.5.9. Waste statistics
This visualization displays the waste determined by A+W Production and A+W Realtime Optimizer.

*[Image: A dashboard showing waste statistics with percentages and area measurements in a grid format.]*

#### 3.5.10. Workload capacity planning
In process

#### 3.5.11. Customer requirements, credit limit, budget
This visualization displays the customer's requirements as compared to the credit limit and sales. Prerequisite for using this visualization completely:
- Customer requirements must be transmitted from a financial bookkeeping system to A+W Business
- Customer's budget in A+W Business defined via a classifier

*[Image: A dashboard with various charts comparing customer requirements, credit limits, and budgets.]*

#### 3.5.12. Delivery reliability
Visualization compares planned and actual delivery date for orders and purchase orders. The number and value of orders and purchase orders are displayed.

The actual delivery date has to be booked by means of appropriate functions in ERP system and the scheduled delivery dates must not be changed after entry (please consider rules for entry in A+W Business).

*[Image: A dashboard showing delivery reliability metrics, including KPIs for delays and a map visualization.]*

### 3.6. Restrictions

#### 3.6.1. A+W Clarity Modules
A+W Analytics currently relies on A+W Business and A+W Production. An incorporation into A+W Enterprise and A+W Business Pro has not yet been achieved.

#### 3.6.2. QLIK Sense® Server
To use A+W Analytics, you will need a Qlik Sense ® Server. It is not a component of A+W Analytics and has to be purchased separately.

#### 3.6.3. Services
In order to not adversely affect the performance of the productive application or maintenance tasks when reading in the data, it is recommended that you coordinate the data procurement appropriately.

With use of SQL Base database in A+W Clarity products, it must be noted that SQLBase also locks the data records during reading. Thus, under SQLBase, the data procurement must be done outside of productive times.

### 3.7. Notes

**Adjustments**

If additional data from A+W Clarity databases is required, it is possible to expand the "data loading architecture" individually for a fee.

Individual adaptations of A+W Analytics visualizations and the creation of completely new evaluations are possible for a fee.

The effort required for these extensions depends on the complexity of the requirement and is offered in the course of the implementation.

---

## 4. Contact Address

**A+W Software GmbH**

Siemensstraße 3
35463 Fernwald
Germany

**Tel.** +49 641 96620-0

**E-mail:** info@a-w.com
**Internet:** http://www.a-w.com/
