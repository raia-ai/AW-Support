---
title: "EN-FUNC-AW_Business_Pro"
source: "EN-FUNC-AW_Business_Pro.pdf"
tags: ["A+W", "Business Pro", "ERP", "Glass Industry", "Software", "Functional Description", "Production Planning", "Optimization", "Machine Control"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A functional description of A+W Business Pro 6, an integrated ERP/PPS solution for small and medium-sized businesses in the glass processing and production planning sector. It outlines supported and unsupported features across organization, optimization, machine control, and integration with other A+W modules."
long_description: "This document provides a detailed functional description of A+W Business Pro 6, a specialized ERP and Production Planning System (PPS) designed for the glass industry. It targets small and medium-sized companies, offering a comprehensive solution for managing quotations, orders, production planning, and other business areas like warehouse and dispatch. The document outlines the software's capabilities, particularly focusing on the production area (master data and production manager). It details supported features and limitations in key areas such as organizational setup (lot types, rack systems), optimization modes (waste and sequence optimization), and machine control. A significant portion is dedicated to explaining how A+W Business Pro 6 couples with other A+W products like the Realtime Optimizer, Business Capacity Planning, and Business BDE (barcoding), specifying the functionalities that are supported and those that are not. The document serves as a technical specification to clarify the software's scope and distinguish it from other A+W solutions and market alternatives."
---

# A+W Functional Description: A+W Business Pro 6

A+W - Software for Glass

---
## 1. Content

1.  **Content**
2.  **Notes on this Document**
    *   2.1. Trademarks
    *   2.2. Copyrights
    *   2.3. Disclaimer of liability
3.  **Product Presentation**
    *   3.1. Notes
        *   3.1.1. A+W Business Pro in connection with A+W Realtime Optimizer
        *   3.1.2. A+W Business Pro in connection with A+W Production Terminal (EL)
4.  **Features in the Organization Area**
5.  **Features in Optimization**
6.  **Coupling / expansion with other A+W products / modules**
    *   6.1. Production software
    *   6.2. A+W Business Capacity Planning
    *   6.3. A+W Business stock connection
7.  **Features of Machine Control**
8.  **Contact Address**

## 2. Notes on this Document

This documentation and the software described in it are only licensed and may only be used and copied pursuant to this license. The contents of the documentation are for information purposes only and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation may also be registered trademarks or other industrial property rights held by third parties. Copyrights of third parties must be complied with.

### 2.2. Copyrights

© 2015, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Disclaimer of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Product Presentation

A+W Business Pro is an integrated ERP PPS solution for small and medium-sized businesses in the sector of order processing and production planning.

The business solution from A+W not only makes it possible to enter quotations, orders, credit notes, complaints and delivery notes as well as to manage orders and inquiries, but also facilitates controlling of other company areas (e.g. warehouse, purchasing, dispatch, etc.).

The integrated production solution offers comprehensive technical support for the processing and planning of orders and quotations. Thanks to the intelligent wizard function, the process of batch formation, optimization, on through to production release can be completed with a mouse-click.

The user has the option to switch to the so-called "expert" mode at any time, where he/she can manually and explicitly directly influence the individual planning and optimization steps, and consequently the result.

The target group for A+W Business Pro are small and medium-sized companies that mainly organize their production manually and by means of production documents.

A+W Business Pro should be regarded as independent of earlier A+W products. In particular, A+W Business Pro is not an upgrade product from earlier production solutions (such as ALFERT or XOPT2000). Thus there is also no guarantee that all functional characteristics of earlier products are available in this product. Required features that are not listed in these technical specifications must be clarified on request.

In this document only the services and functional characteristics of the production area (master data and production manager) are specified in order to distinguish them from other A+W products and other production solutions available on the market.

### 3.1. Notes

#### 3.1.1. A+W Business Pro in connection with A+W Realtime Optimizer

If A+W Business Pro is used together with the A+W Realtime Optimizer, the waste statistics refer only to plan values. All manual changes or changes due to the influence of the A+W Realtime Optimizer are not considered here. If an A+W Realtime Optimizer standalone is used, the actual consumption data can be drawn from the A+W Realtime Optimizer database.

#### 3.1.2. A+W Business Pro in connection with A+W Production Terminal (EL)

If A+W Business Pro is used together with the A+W Production Terminal (EL), the Partial Delivery functionality is not available since rack bookings are not supported.

The same applies for the Reject Handling for Purchased Orders functionality (item number 210015). In this environment, the required service is not available.

## 4. Features in the Organization Area

| Supported features / processes | Features / processes that are not supported |
| :--- | :--- |
| **Predefined lot types** <br> - 100 = single glass, processed single glass <br> - 200 = LAMI <br> - 300 = IG | **Lot types that cannot be defined as desired** <br> - Predefined lot types cannot be changed. <br> - New or additional lot types cannot be defined. |
| **Predefined rack organization systems** <br> - The system is delivered with two predefined rack organization systems: A racks and IG harp racks <br> - Within these two standard organization systems, the following production / organization types are shown: processed single glass, IG, LAMI production | |
| **Self-defined rack organization systems** <br> - It is possible to set up and manage organization systems that were defined by yourself, provided that the predefined parameters and framework conditions that are specified here are met (e.g. lot types) <br> - Multi-level production organization systems can be mapped <br> - A rack and harp rack organization systems are supported. Mixed types are also possible | |
| **Predefined parking mode (stack mode)** <br> - The system supports / includes the stack mode Production with split groups <br> *You can read more about the stack mode that is described here in the Manual on the Process of Detailed Scheduling.* | **No changes / supplements to the stack mode** <br> - Other stack modes, such as unit, glass or Vabgla are not supported <br> - In case of frame-break (new generation when the maximum load is reached), groups cannot be kept together <br> - Changes to the stack modes or split modes are not possible |
| **Self-defined rack numbers** <br> - The number area for racks or rack groups can be defined in the master data as desired | |
| **Consecutive rack numbers** <br> - With reaching of the maximum load of a storage space, the system automatically generates a new storage space with a new logical number | **No permanent reset of the rack numbers** <br> - A reset of the rack numbers is only done with reaching of the self-defined number limit |
| **Predefined rough and detailed scheduling views** <br> - The system offers predefined rough scheduling and detailed scheduling views <br> - In rough scheduling, you can create your own filter structures with predefined columns and save these user-dependently | **Rough and detailed scheduling views that cannot be defined as desired** <br> - It is not possible to show or configure additional information (e.g. additional new columns or filters) <br> - Customizing is not possible |
| **No splitting of order items in detailed scheduling** <br> - The A+W Business Pro detailed scheduling does not support the splitting of order items | |
| **Output of production papers and bar codes** <br> - The system supports the manual organization of production processes by means of predefined production papers and bar codes <br> - The format and layout of production papers and bar codes that are already integrated in the system can be adjusted (Crystal Reports) | |
| **Creation of self-defined reports** <br> - The system enables the creation of self-defined queries and reports in accordance with the database description A+W Business (CR) | **No integration of self-defined / additionally defined production papers in the printing process** <br> - It is not possible to define new additional production papers and integrate those into the standard process flow |
| **Predefined criteria for rack organization systems** <br> - A+W Business includes a set of pre-defined formula elements (variables and operators) that are used to define filter criteria for sorting and grouping in the sector of rack organization systems | **No support of self-defined formulas** <br> - You cannot define new variables or operators yourself and add them to the system <br> - An option for formula-based criteria / filter definition (SQL) has not been provided for |
| **Item split in the AWB Capacity Planning** <br> - Is supported since V6 and thus split items can be scheduled in the Production Manager. | |

## 5. Features in Optimization

| Supported features / processes | Features / processes that are not supported |
| :--- | :--- |
| **Supported waste and sequence optimization modes** <br> - Sequence optimization XOPTS 6.2 (strict sequence) <br> - Sequence optimization XOPTS 6.1 (keep customers together) <br> - Sequence optimization XOPTS 5.2 (standard) <br> - Sequence optimization XOPTS 5.1 (IGU on harp racks or many A-racks) <br> - XOPT (chaotic optimization) <br> - Implicit setting of the optimization mode via the grouping and sorting parameters <br> *You can read more about the optimization modes that are described here in the Manual on the Process of Detailed Scheduling.* | **No explicit selection of the optimization modes** <br> - Setting of the optimization mode not explicitly possible; rather, it is executed while controlled by the system via setting of the grouping and sorting parameters |
| **Synchronous optimization** <br> - For the optimization process, the system takes into account the dependencies of the pane and the counter pane for IG and LAMI for the sequential orientation of the optimization (dependent on the selected organization type and set grouping and sorting keys) | **No dynamic optimization** <br> - A+W Business Pro does not include or support dynamic optimization modes <br> - Extensions such as A+W Dynopt or A+W Dynopt Compact cannot be connected to the system |
| **Optimization of quotations and/or reservation orders** <br> - Quotations or reservation orders entered in the ERP area can be optimized in the production manager for calculational purposes. The results are saved as PDF in the quotation. | **Optimization of quotations and/or reservation orders** <br> - Except for the PDF, no data is saved. <br> - Costs determined are not written back. <br> - There is no reservation of stock lites |
| **Decoat** <br> We write the decoating widths for the shape into the Opt2 files if: <br> - We are using the A+W catalog <br> - The shape does not have any circular arc segments <br> - Decoating is possible on the machine and the decoating width is greater than or equal to the minimum on the machine. <br> - For individual sheets or LSG, the processing edge decoating (1025) from the A+W processing catalog is heeded and evaluated accordingly. | |
| **Manual insertion of additional lites (fillers)** <br> - Fillers can be added manually in the A+W Planeditor (after optimization has been performed and stored) <br> - Entry of pane parameters possible: Height, width, model number, rack number | **No automatic filler dimensions** <br> - The system does not generate any fillers automatically in the course of optimization |
| **No bar codes or production papers for manually added panes** <br> - Bar codes are not generated for manually inserted panes. <br> - Manually inserted panes are not taken into account / shown on production documents | |
| **Graphic display of shapes in the quick display** <br> - The quick display (detail view in the process of optimization) cannot display any shape geometries graphically. <br> Displayed instead are the circumscribed rectangles. This is the preview that can be generated more quickly | **No modification of optimization results** <br> - The optimization results (sectional views) cannot be manually edited in A+W Planeditor <br> - Any changes that may become necessary must be carried out as changes to optimization parameters (model trims, Orga, ...) during the optimization process – prior to saving the optimization |
| **Optimization of shapes** <br> - During the optimization process, A+W Business Pro takes the model parameters that are stored in the system and in the order into account | |
| **Integration of A+W Shape Opt** <br> - If the extension A+W Shape Opt has been activated, 2 model geometries are combined at a time during the optimization process | |
| **Graphic display of shapes in printouts and in A+W Planeditor** <br> - The system shows shapes correctly in A+W Planeditor (after saving the optimization results) and on printouts (shop papers) | |
| **Display of the most important information on printouts and displays** <br> - The quick display provides the following information: dimensions, cutting dimensions, storage space no., breakage sequence <br> - Printouts and the A+W Planeditor provided the following additional information: shape image | **No editing of the graphic display in the A+W Planeditor and the quick display** <br> - The information displayed in the quick display (detail view) and in the A+W Planeditor cannot be changed or expanded. Thus, for example, no order numbers or item numbers can be displayed. |
| **Free shapes for IGU or LSG** <br> - The processing of free shapes (shape 99) is supported for insulated glass and/or LSG glass | |
| **Surcharges for edge processings (rectangle, default shape)** <br> - For dimension-changing edge processings such as grinding, the surcharges can be managed in Business Pro. These surcharges are added for rectangles and default shapes to the cutting contour. | **Surcharges for edge processings (free shape [F99])** <br> - For free shapes, surcharges are not added automatically to the geometry. The user must create the contour as it should be cut. <br> The exception to this are drilling hole markings in the cutting code. The shapes are written here as F99 to the block file and the edge surcharges are calculated in advance. |
| **Number of stock plates** <br> - The number of stock plates and/or residual sheets per optimization can be 10 or 30. | |
| **Breakage** <br> - Breakage can be reported in the Production Manager (starting with V6). With the broken sheets, the user can form a breakage run and then plan in detail, optimize, and produce as usual. | |
| **Marking drilling holes** <br> - The drilling holes can be scored on the cutting table. <br> - Normal drilling holes and stepped drilling holes are heeded. | |
| **Offer optimization** <br> - In addition to orders, quotations can also be planned. The quotation mode is only possible in standard mode. The quotation mode runs precisely like the order mode (detailed planning, optimization, and report output). For quotations, the user can change stock plate dimensions in the optimization and the purchase price of the stock plate (price per m²) and thus influence the optimization result. The results are 3 reports (no cutting code) that depict the following: <br>   - Optimization result with optimization parameters. <br>   - Cross-sections <br>   - List of the stock plates <br> The reports are attached to the quotation. | |
| **Switchable tolerances for cuts in the optimization in A+W Business Pro** <br> - In A+W Business Pro it is now possible that the optimization ignores the minimum and maximum distances from XX and YY cuts if otherwise no result can be achieved. This applies for these tolerances: <br>   - Tolerance for min. dist.X-X <br>   - Tolerance for min. dist.Y-Y <br>   - Tolerance for max. dist. X-X <br>   - Tolerance for max. dist. Y-Y | |

## 6. Coupling / expansion with other A+W products / modules

### 6.1. Production software

| Supported features / processes | Features / processes that are not supported |
| :--- | :--- |
| **Coupling / data transfer to A+W Realtime Optimizer** <br> - It is possible to transfer the optimized sectional views to A+W Realtime Optimizer in order to monitor and control cutting to size online there | **No coupling to external production software or display systems** <br> - It is not possible to connect A+W Business Pro to production software or display / monitoring systems of external software producers <br> **No coupling to A+W Production** <br> - A+W Business Pro cannot be connected to A+W Production <br> **No coupling to / transfer of data to A+W Production Terminal** <br> - It is not possible to transfer data for the graphical display of production steps to the A+W Production Terminal <br> **No feedback / data feedback from A+W Realtime Optimizer** <br> - Feedback from A+W Realtime Optimizer is not analyzed in A+W Business Pro <br> - Feedback from A+W Realtime Optimizer is not analyzed in A+W Business capacity planning (in the coupling A+W Business Pro – A+W Business capacity planning - A+W Realtime Optimizer) |
| **Connection of A+W Business BDE (barcoding)** <br> - The system supports data transfer to and from A+W Business BDE (barcoding) | **Barcoding bookings only specific to the item** <br> - A+W Business BDE can only make bookings specific to the item <br> - A precise booking of lites or parts is not possible |
| **Incorporation of AWB Barcode Scanner** <br> - With the AWB Barcode Scanner (starting with V6), breakage or defects on the sheet can be reported. The Production Manager can access the reported sheets on the breakage dialog and the user can form a breakage lot with these and additional broken sheets. | **A+W Realtime Optimizer stock plate quantity 30** <br> - For the cutting process and the existing optimization modes, only optimizations with a maximum of 10 different stock plate sizes or residual sheet sizes are possible. The option 30 stock plates per optimization is not supported. |

### 6.2. A+W Business Capacity Planning

| Supported features / processes | Features / processes that are not supported |
| :--- | :--- |
| **Coupling with A+W Business Capacity Planning** <br> - The standard delivery version of A+W Business Pro already includes the functions of the machine classification (integrated in the capacity planning module) <br> - In order to use the capacity planning functions (shifts, transition periods, standard times, etc.), it is possible / necessary to expand the system with a full A+W Business capacity planning program (additional license) | **Excess quantities** <br> - No excess quantities possible, neither production-technically nor order-technically <br> **Undersupply** <br> - No undersupply possible, neither production-technically nor order-technically |
| **Item split in the AWB Capacity Planning** <br> - Is supported since V6 and thus split items can be scheduled in the Production Manager. | |

### 6.3. A+W Business stock connection

| Supported features / processes | Features / processes that are not supported |
| :--- | :--- |
| **Use of residual plates from the stock location for residual plates** <br> - The system offers the option to create and manage a stock for residual plates <br> - Residual plates that have been manually added to the booking can be used for the optimization <br> - Residual sheets can only be added manually to the residual stock <br> - Residual sheets are calculated and removed after the stock plates in the residual stock. | |
| **Use of stock sizes for the "best result"** <br> - The optimization essentially uses the stock lites that provide the "best result" with respect to costs and yield <br> - If it is mandatory that a residue plate is used despite worse waste or worse costs, the use of the residue plate can be manually controlled by means of the priority | **Booking out a quantity of stock not possible with A+W Realtime Optimizer** <br> - Since A+W Business Pro already provides an option for manually booking quantities out of stock within the scope of the optimization, it is not possible / allowed to carry out automatic or manual booking of quantities out of stock using A+W Realtime Optimizer <br> - The option to book quantities out of stock must be deactivated in the settings of A+W Realtime Optimizer |

## 7. Features of Machine Control

| Supported features / processes | Features / processes that are not supported |
| :--- | :--- |
| **Control of standard machines** <br> - The system offers data transfer and control of cutting tables, IG lines and spacer benders <br> - Here, only commercially available standard machines are supported <br> - Please contact A+W Sales in advance of the project (during the quotation phase) to see whether the machine type you are using is supported. | |

## 8. Contact Address

**A+W Software GmbH**  
Siemensstraße 3  
35463 Fernwald  
Germany

**Tel:** +49 641 96620-0  
**E-mail:** info@a-w.com  
**Internet:** http://www.a-w.com/
