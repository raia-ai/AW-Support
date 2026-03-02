---
description: "US-FUNC-AW_Business_Pro"
---


# A+W Functional Specification
---
## A+W Business Pro 6

A+W - Software for Glass

---

## 1. Notes about this Document
This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The greatest care was used in compiling the texts and figures. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 1.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 1.2. Copyrights
© 2015, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Without the prior written permission of A+W Software GmbH, the documentation may not be transmitted electronically, by recording or in any other form.

### 1.3. Exclusion of liability
A+W Software GmbH assumes no liability for data errors that rely on basic principles of the standard functions made available by Microsoft, Unix or other software and hardware suppliers.

A+W reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All adjustments, expansions, database queries, reports, analyses, and interface expansions that were created individually for our customers and/or machines and software partners as well as all costs and efforts associated with these were borne by the client (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary in order to ensure that the adjustments/expansions commissioned that were undertaken/developed for a version will also work perfectly and be used in the subsequent version.

---

## 2. Table of Contents
- **Notes about this Document**
  - Trademarks
  - Copyrights
  - Exclusion of liability
- **Description of the product**
- **Characteristics in the Organization Area**
- **Features in the Optimization**
- **Coupling/Expansion with other A+W Products/Modules**
  - Production Software
  - A+W Business Capacity Planning
  - A+W Business Stock Connection
- **Machine Activation Features**
- **Functionality A+W Business Pro and A+W Business Pro (EL)**
- **Contact Address**

---

## 3. Description of the product
A+W Business Pro is an integrated ERP-PPS solution for small and medium-sized companies for use in order processing and production planning.

The A+W commercial solution enables not just the entry of quotations, orders, credits, complaints, delivery notes, and the management of purchase orders and inquiries, but also the control of other company areas (e.g. stock, purchasing, dispatch, etc.).

The integrated production solution offers comprehensive technical support for the processing and planning of orders and quotations. Thanks to the intelligent wizard function, the process of batch formation, optimization, on through to production release can be completed with a mouse-click.

The user can switch to "expert mode" at any time and can influence individual planning and optimization steps manually and explicitly there and thus change the result.

The target group of A+W Business Pro is small and medium-sized companies who organize their production mostly manually and using production papers.

A+W Business Pro should be regarded as independent of earlier A+W products. In particular, A+W Business Pro is not an upgrade product from earlier production solutions (such as ALFERT or XOPT2000). Thus there is also no guarantee that all functional characteristics of earlier products are available in this product. Required features that are not listed in these technical specifications must be clarified on request.

In this document, only the services and characteristics of the production area (master data and production manager) are specified in order to delimit them as compared to other A+W products and other production solutions available on the market.

---

## 4. Characteristics in the Organization Area

| Supported features/processes | Non-supported features/processes |
| :--- | :--- |
| **Pre-defined lot types** | **Lot types cannot be defined freely** |
| - 100 = simple glass, processed simple glass | - Pre-defined lot types cannot be changed. |
| - 200 = LSG | - No new or additional lot types can be defined. |
| - 300 = IGU | |
| **Pre-defined storage space organizations** | |
| - The system is delivered with two predefined storage space organizations: A-rack and IGU harp racks | |
| - Within these two standard orgas, the following production/organization forms are mapped: processed simple glass, IGU, LSG production | |
| **Self-defined storage space organizations** | |
| - The set-up and management of self-defined organizations is possible - with adherence to the pre-defined parameters and basic conditions mentioned here (lot types, for example) | |
| - Multi-level production organizations can be mapped | |
| - A-rack and harp rack organizations are supported. Mixed forms are also possible | |
| **Pre-defined storage mode (stacking mode)** | **No changes/additions to stacking mode** |
| - The system supports/includes the stacking mode production with split groups | - Other stacking modes, such as unit, glass or Vabgla, are not supported |
| For details about the stacking mode described here, please consult the manual about detailed scheduling. | - In case of frame-break (new generation when the maximum load is reached), groups cannot be kept together |
| | - Change to stacking modes and split modes are not possible |
| | For details about the stacking modes described here, please consult the manual about detailed scheduling. |
| **Self-defined rack numbers** | |
| - The number ranges for storage spaces and storage space groups can be defined freely in the master data | |
| **Sequential rack numbers** | **No permanent reset of the rack numbers** |
| - With reaching of the maximum load of a storage space, the system automatically generates a new storage space with a new logical number | - A reset of the rack numbers is only done with reaching of the self-defined number limit |
| **Pre-defined rough scheduling and detailed scheduling views** | **No splitting of order items in the detailed scheduling** |
| - The system offers pre-defined rough scheduling and detailed scheduling views | - The A+W Business Pro detailed scheduling does not support the splitting of order items |
| - In the rough scheduling area, it is possible using pre-defined columns to create individual filter structures and to save them depending on the user | **No freely-definable rough and detailed planning views** |
| | - No additional information can be displayed or configured (for example additional, new columns or filters) |
| | - Customizing is not possible |
| **Output of production papers and bar codes** | **No incorporation of self-defined/additional production papers in the printing process** |
| - The system supports the manual organization of production processes using pre-defined production papers and bar codes | - It is not possible to define additional production papers and to incorporate these in the standard process flow |
| - Production papers and bar codes already integrated into the system can be adjusted in format and layout (Crystal Reports) | |
| **Creation of self-defined reports** | |
| - The system permits the creation of self-defined queries and reports according to the A+W Business (CR) database description | |
| **Pre-defined criteria for storage space organization** | **No support of self-defined formulas** |
| - A+W Business receives a set of pre-defined formula building blocks (variables and operators) in order to define filter criteria for sorting and groupings in the area of storage space organization | - It is not possible to define new variables or operators yourself and add them to the system |
| | - There is no possibility for form-based criteria/filter definition (SQL) provided |
| **Item split in the AWB Capacity Planning** | |
| - Is supported since V6 and thus split items can be scheduled in the Production Manager. | |

---

## 5. Features in the Optimization

| Supported features/processes | Non-supported features/processes |
| :--- | :--- |
| **Supported yield and sequence optimization modes** | **No explicit selection of the optimization modes** |
| - Sequence optimization XOPTS 6.2 (strict sequence) | - Setting of the optimization mode not explicitly possible; instead, controlled by the system via setting of the grouping and sorting parameters |
| - Sequence optimization XOPTS 6.1 (keep customers together) | |
| - Sequence optimization XOPTS 5.2 (standard) | |
| - Sequence optimization XOPTS 5.1 (IGU on harp racks or many A-racks) | |
| - XOPT (chaotic optimization) | |
| - Setting of the optimization mode implicitly, via the grouping and sorting parameters | |
| For details about the optimization modes described here, please consult the manual about detailed scheduling. | |
| **Synchronous optimization** | **No dynamic optimization** |
| - In the optimization, the system considers the dependencies of sheet and countersheet for IGU and LSG in the sequence orientation of the optimization (depending on the organizational form selected and the grouping and sorting keys set) | - A+W Business Pro does not include or support a dynamic optimization mode |
| | - Expansions such as A+W Dynopt and A+W Dynopt Compact cannot be coupled to the system |
| **Optimization of quotations and/or reservation orders** | **Optimization of quotations and/or reservation orders** |
| - Quotations or reservation orders entered in the ERP area can be optimized in the production manger for calculation purposes. The results are saved as PDF in the quotation. | - Except for the PDF, no data is saved. |
| | - Costs determined are not written back. |
| | - There is no reservation of stock plates |
| **Decoating** | |
| - We write the decoating widths for the shape into the Opt2 files if: | |
|   - We are using the A+W catalog | |
|   - The shape does not have any circular arc segments | |
|   - Decoating is possible on the machine and the decoating width is greater than or equal to the minimum on the machine. | |
| - For individual sheets or LSG, the processing edge decoating (1D25) from the A+W processing catalog is heeded and evaluated accordingly. | |
| **Manual insertion of additional sheets (fillers)** | **No automatic filler dimensions** |
| - Fillers can be added manually in the A+W Planeditor (after optimization has been performed and stored) | - The system does not generate any fillers automatically in the course of optimization |
| - Entry of sheet parameters possible: height, width, shape number, storage space number | **No bar codes or production papers for manually-added sheets** |
| | - No bar codes are generated for manually-added sheets. |
| | - Manually-added sheets are not considered/displayed on production papers. |
| **Graphic display of shapes in the quick display** | **No modification of the optimization results** |
| - The quick display (detail view in the process of optimization) cannot display any shape geometries graphically. | - The optimization results (cutting patterns) cannot be edited manually in the A+W Planeditor |
| Displayed instead are the circumscribed rectangles. This is the preview that can be generated more quickly | - If changes are necessary, then changes must be made to optimization parameters (shape break edges, orga, etc.) in the process of optimization - before saving the optimization |
| **Optimizing shapes** | |
| - In the optimization, A+W Business Pro considers the shape parameters stored in the system and the order | |
| **Integration of A+W Shape Opt** | |
| - If the add-on A+W Shape Opt should be activated, then 2 shape geometries apiece are combined in the optimization | |
| **Graphic display of shapes on printout and in the A+W Planeditor** | **No editing of the graphic display in the A+W Planeditor and the quick display** |
| - In A+W Planeditor (after saving the optimization results) and on printouts (work sheets), the system displays shapes correctly | - The information displayed in the quick display (detail view) and in the A+W Planeditor cannot be changed or expanded. Thus, for example, no order numbers or item numbers can be displayed. |
| **Display of the most important information on printouts and displays** | |
| - The quick display provides the following information: dimensions, cutting dimensions, storage space no., breakage sequence | |
| - Printouts and the A+W Planeditor also provide the following information: shape image | |
| **Free shapes for IGU or LSG** | **Surcharges for edge processings (free shape [F99])** |
| - The processing of free shapes (shape 99) is supported for insulated glass and/or LSG glass | - For free shapes, surcharges are not added automatically to the geometry. The user must create the contour as it should be cut. |
| **Surcharges for edge processings (rectangle, default shape)** | The exception to this are drilling hole markings in the cutting code. The shapes are written here as F99 to the block file and the edge surcharges are calculated in advance. |
| - For dimension-changing edge processings such as grinding, the surcharges can be managed in Business Pro. For rectangles and default shapes, these surcharges are added to the cutting contour. | |
| **Number of stock plates** | |
| - The number of stock plates and/or residual sheets per optimization can be 10 or 30. | |
| **Breakage** | |
| - Breakage can be reported in the Production Manager (starting with V6). With the broken sheets, the user can form a breakage run and then plan in detail, optimize, and produce as usual. | |
| **Marking drilling holes** | |
| - The drilling holes can be scored on the cutting table. | |
| - Normal drilling holes and stepped drilling holes are heeded. | |
| **Offer optimization** | |
| - In addition to orders, quotations can also be planned. The quotation mode is only possible in standard mode. The quotation mode runs precisely like the order mode (detailed planning, optimization, and report output). For quotations, the user can change stock plate dimensions in the optimization and the purchase price of the stock plate (price per m²) and thus influence the optimization result. The results are 3 reports (no cutting code) that depict the following: | |
|   - Optimization result with optimization parameters. | |
|   - Cross-sections | |
|   - List of the stock plates | |
| The reports are attached to the quotation. | |
| **Switchable tolerances for cuts in the optimization in A+W Business Pro** | |
| - In A+W Business Pro it is now possible that the optimization ignores the minimum and maximum distances from XX and YY cuts if otherwise no result can be achieved. This applies for these tolerances: | |
|   - Tolerance for min. abs. X-X | |
|   - Tolerance for min. abs. Y-Y | |
|   - Tolerance for max. abs. X-X | |
|   - Tolerance for max. abs. Y-Y | |

---

## 6. Coupling/Expansion with other A+W Products/Modules

### 6.1. Production Software

| Supported features/processes | Non-supported features/processes |
| :--- | :--- |
| | **No coupling to external production software or display systems** |
| | - It is not possible to couple A+W Business Pro to external software producers' production software or display/monitoring systems |
| | **No coupling to A+W Production** |
| | - A+W Business Pro cannot be coupled to A+W Production |
| | **No coupling to/transfer of data to A+W Production Terminal** |
| | - A data transfer for the graphic display of production steps on A+W Production Terminal is not possible |
| **Coupling/data transfer to A+W Realtime Optimizer** | **No feedback/data reporting from A+W Realtime Optimizer** |
| - It is possible to transfer the optimized cutting patterns to the A+W Realtime Optimizer in order to monitor and control the cutting online there | - Reports from A+W Realtime Optimizer are not evaluated in A+W Business Pro |
| | - Reports from the A+W Realtime Optimizer are not evaluated in the A+W Business Capacity Planning (in the coupling A+W Business Pro - A+W Business Capacity Planning - A+W Realtime Optimizer) |
| **Connection to A+W Business PDC** | **PDC bookings only to the item** |
| - The system supports the data transfer to and from A+W Business PDC | - The A+W Business PDC can only book to the item |
| | - A precise booking of sheets or parts is not possible |
| **Incorporation of AWB Barcode Scanner** | **A+W Realtime Optimizer stock plate quantity 30** |
| - With the AWB Barcode Scanner (starting with V6), breakage or defects on the sheet can be reported. The Production Manager can access the reported sheets on the breakage dialog and the user can form a breakage lot with these and additional broken sheets. | - For the cutting process and the existing optimization modes, only optimizations with a maximum of 10 different stock plate sizes or residual sheet sizes are possible. The option 30 stock plates per optimization is not supported. |

### 6.2. A+W Business Capacity Planning

| Supported features/processes | Non-supported features/processes |
| :--- | :--- |
| **Coupling to A+W Business Capacity Planning** | **Over-quantities** |
| - The standard delivery version of A+W Business Pro already includes the functions for machine assignment (which are integrated into the capacity planning module) | - No over-quantities possible, neither production-technically nor order-technically |
| - For the use of the capacity planning functions (shifts, transition times, default times, etc.) it is possible/necessary to expand the system with a complete A+W Business Capacity Planning (additional license) | **Shortage** |
| | - No shortage possible, neither production-technically nor order-technically |
| **Item split in the AWB Capacity Planning** | |
| - Is supported since V6 and thus split items can be scheduled in the Production Manager. | |

### 6.3. A+W Business Stock Connection

| Supported features/processes | Non-supported features/processes |
| :--- | :--- |
| **Use of residual sheets from the residual sheet stock** | |
| - The system offers the possibility for creating and managing a residual sheet stock | |
| - Manually-added residual sheets can be used in the optimization | |
| - Residual sheets can only be added manually to the residual stock | |
| - Residual sheets are calculated and removed after the stock plates in the residual stock. | |
| **Use of stock sheets for the "best result"** | **No stock removals with the A+W Realtime Optimizer** |
| - The optimization essentially uses the stock sheets that provide the "best result" with respect to costs and yield | - Since A+W Business Pro already offers the possibility for manual stock removal in the course of optimization, it is not possible/permissible to make automatic or manual stock removal bookings with the A+W Realtime Optimizer |
| - If a residual sheet should absolutely be used despite poorer yield or costs, then the use of the residual sheet can be controlled manually via the priority | - The possibility for stock removal must be deactivated in the settings of the A+W Realtime Optimizer |

---

## 7. Machine Activation Features

| Supported features/processes | Non-supported features/processes |
| :--- | :--- |
| **Activation of standard machines** | |
| - The system offers data transfer to and the activation of cutting tables, IGU lines, and frame benders | |
| - Here, only commonly-available machines are supported | |
| - Please contact A+W Sales in advance of the project (during the quotation phase) to see whether the machine type you are using is supported. | |

---

## 8. Functionality A+W Business Pro and A+W Business Pro (EL)

| Functionality | A+W Business Pro | A+W Business Pro (EL) |
| :--- | :---: | :---: |
| **Company Areas** | | |
| Purchasing | ✓ | ✓ |
| Sales | ✓ | ✓ |
| Production | ✓ | x |
| Stock | ✓ | x² |
| Dispatch | ✓ | ✓ |
| **Organization** | | |
| Pre-defined lot types | ✓ | ✓ |
| Pre-defined storage space organizations | ✓ | ✓ |
| Self-defined storage space organizations | ✓ | ✓ |
| Pre-defined storage mode (stacking mode) | ✓ | ✓ |
| Self-defined rack numbers | ✓ | ✓ |
| Sequential rack numbers | ✓ | ✓ |
| Pre-defined rough scheduling and detailed scheduling views | ✓ | ✓ |
| Output of production papers and bar codes | ✓ | ✓ |
| Creation of self-defined reports | ✓ | ✓ |
| Pre-defined criteria for storage space organization | ✓ | ✓ |
| Item split in the AWB Capacity Planning | ✓ | x |
| Technical order entry | ✓ | ✓ |
| **Optimization** | | |
| Supported yield and sequence optimization modes | ✓ | ✓ |
| Synchronous optimization | ✓ | ✓ |
| Optimization of quotations and/or reservation orders | ✓ | x |
| Decoating | ✓ | ✓ |
| Manual insertion of additional sheets (fillers) | ✓ | ✓ |
| Graphic display of shapes in the quick display | ✓ | ✓ |
| Optimizing shapes | ✓ | ✓ |
| Integration of A+W Shape Opt | ✓ | x |
| Graphic display of shapes on printout and in the A+W PlanEditor | ✓ | ✓ |
| Display of the most important information on printouts and displays | ✓ | ✓ |
| Free shapes for IGU or LSG | ✓ | ✓ |
| Surcharges for edge processings (rectangle, default shape) | ✓ | ✓ |
| Number of stock plates | ✓ | ✓ |
| Breakage | ✓ | ✓ |
| Marking drilling holes | ✓ | ✓ |
| Offer optimization | ✓ | x |
| **Expansion with other A+W Products / Modules** | | |
| Coupling/data transfer to A+W Realtime Optimizer | ✓ | x |
| Connection A+W Business EDI | ✓ | ✓¹ |
| A+W CAD Designer | ✓ | x² |
| **A+W Capacity Planning** | ✓ | x |
| **A+W Business Stock Connection** | ✓ | x¹ |
| **Activation of Standard Machines** | | |
| Cutting Tables | ✓ | ✓ |
| IG Lines | ✓ | x |
| Spacer Benders | ✓ | x |

### Legend:
| Symbol | Meaning |
| :---: | :--- |
| ✓ | Included |
| ✓¹ | Included in US Version |
| x | Not available |
| x¹ | Optionally available |
| x² | Optionally available for US Version |

---

## 9. Contact Address
**A+W Software GmbH**  
Am Pfahlgraben 4 - 10  
35415 Pohlheim  
Germany

Tel. +49 6404 2051 0  
Fax. +49 6404 2051 877

E-Mail: zentrale@a-w.com  
Internet: http://www.a-w.com/
