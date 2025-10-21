title: "EN-FUNC-AW_Defect_Optimizer"
source: "EN-FUNC-AW_Defect_Optimizer.pdf"
tags: ["A+W", "Defect Optimizer", "Software for Glass", "Production Optimization", "Cutting Plan", "Realtime Optimizer", "Viprotron", "Glass Manufacturing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Functional description for the A+W Defect Optimizer, a software module for glass production. It details how the software identifies, visualizes, and optimizes cutting plans to avoid defects on glass stock dimensions, thereby reducing waste and improving process efficiency."
long_description: "This document provides a detailed functional description of the A+W Defect Optimizer, a module designed to work with A+W Production and A+W Realtime Optimizer 5.4 or later. The optimizer processes defect data from scanners (e.g., Viprotron) to improve glass cutting yields. It operates in two stages: a 'Pure display functionality' mode that visualizes defects on the cutting pattern without altering it, and a 'Complete defect optimization' mode that actively restructures the cutting plan. The complete optimization uses degrees of freedom like shifting lites and residuals to move planned cuts away from detected defects. The document outlines the module's data, presentation, system requirements (including the A+W Realtime Optimizer module), a list of functions, and its limitations. It also includes standard legal notices regarding trademarks, copyrights, and liability."
---

# A+W Functional Description
# A+W Defect Optimizer

---

## 1. Content

1.  **Content**
2.  **Notes on this Document**
    1.  Trademarks
    2.  Copyrights
    3.  Exclusion of liability
3.  **Performance Description**
    1.  Data
    2.  Presentation
    3.  Requirements
    4.  List of Functions
        1.  Pure display functionality
        2.  Complete defect optimization
    5.  Limitations
4.  **Contact Address**

---

## 2. Notes on this Document

This documentation and the software described in it are only licensed and may only be used and copied pursuant to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation may also be registered trademarks or other industrial property rights held by third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2015, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This also includes possibly necessary long-term costs and expenses for amending and extending subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220033 |
| **Module** | A+W Defect Optimizer |
| **Brief description** | Defect optimization Restructuring of an optimization result for a stock dimension for avoidance of defects on individual cutting lites or display of defects of the stock dimension |
| **Available** | Starting with A+W Realtime Optimizer 5.4 |

### 3.2. Presentation

The A+W Defect Optimizer exists in two different stages of expansion.
1.  The pure display functionality receives the defects and visualizes these in the XTV
2.  The complete defect optimization receives the defects, restructures the stock dimension, and visualizes these in the XTV

In addition to the lower consumption of glass due to the avoidance of defects, which cause a lite to have to be recut, the main advantage is that the lites affected by defects can be identified very early in the process.

### 3.3. Requirements

-   A+W Realtime Optimizer (Module number 220016)
-   Transfer of the defects of a stock dimension (Viprotron scanner or SGG TCP-IP)
-   Configuration of the A+W Realtime Optimizer for defect optimization
-   In case of active restructuring, after any restructuring done, there may be no manipulation of the results (e.g. XOPTMULT, etc.)
-   For the complete defect optimization incl. restructuring, either the requesting of stock dimensions must be uncoupled from the cutting plan transmission or it must be possible to replace an already-transmitted cutting plan (system-specifically).

### 3.4. List of Functions

#### 3.4.1. Pure display functionality

The stock dimension is requested via cutting code transmission. For the transmission of the tapeline from the stock in the direction of cutting, the existing defects are reported, e.g. by a Viprotron scanner to the A+W Realtime Optimizer. It receives the defects and stores these in the database. There is no restructuring of the pattern. If there is a residual plate stock, the defects that are still on the residual sheet are stored in the database in order to display these during use of the residual plate. This is necessary since for such residual plates there is no new reporting of information about existing defects. The A+W Realtime Optimizer transmits the information about the defects (e.g. position, size, etc.) to the XTV. If the pattern is displayed on the XTV, the defects are visualized there and the cutter can check these defects explicitly and report the affected lites broken if necessary.

#### 3.4.2. Complete defect optimization

The stock dimension is either requested via loader file or via manual request if a subsequent exchange of a cutting code is not possible or via cutting code transmission. For the transmission of the tapeline from the stock in the direction of cutting, the existing defects are reported, e.g. by a Viprotron scanner to the A+W Realtime Optimizer. The information received is stored in the database. The A+W Realtime Optimizer transmits the defect information and order item-related limit values for the visible area and the edge area in the form of a .cvs file, the Opt2 files, and the information about which plate is affected to the XoptReorg module and starts it. XoptReorg restructures the pattern and uses the specified degree of freedom of the pattern for this. The degrees of freedom include shifting residuals, breaking up residuals, shifting lites, and exchanging lites as long as the sequence restriction permits this. The goal of the restructuring is to avoid defects, whereby different limit values are heeded for visible areas and hidden areas (e.g. insulated edge lamination). If avoidance is not possible, there is an attempt to minimize the resulting waste (that is, to place unavoidable defects on as small a lite as possible). The pattern resulting from the restructuring is written to the Opt2Out (note: only for this pattern. The other patterns are unaffected). Statistical information and the lites still affected by defects are added to the .csv file. In case of a defect, XoptReorg reports an error or in case of successful restructuring the Opt2 files as results and returns the completed .csv file to the A+W Realtime Optimizer. The A+W Realtime Optimizer saves this information in the database. Subsequently, the cutting plan is re-generated and transmitted to cutting or replaced. In case of an error, the previous cutting plan is transmitted or no replacement is called up. All information with respect to the defects, the still-affected lites, and the changed pattern are transmitted by the A+W Realtime Optimizer to the XTV. The XTV displays the restructured pattern and also visualizes the defects on the plate there. All lites still affected by defects are pre-marked with a yellow cross as breakage proposal in the XTV. The cutter must check the affected lites and confirm the breakage marking or take it away.

For rectangular lites that become insulated glass, defects that are in the area around the spacer are ignored since on the window they will be covered by the frame.

### 3.5. Limitations

-   For temporal and organizational reasons, there is no new optimization of the pattern. Without an uncoupling of the cutting code and the requesting of a stock dimension, no complete defect optimization with automatic feeding can be done.
-   It is not checked whether there is a defect on a non-critical area of the primitive. This could be a defect in the remaining area of shapes or parts that are irrelevant due to a surface processing. The exception is only the area mentioned above of defects in the area around the spacer for rectangles.

---

## 4. Contact Address

**A+W Software GmbH**

Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com
Internet: http://www.a-w.com/
