---
description: "A+W Defect Optimizer - Brief Description"
---



title: "EN-AWDefect_Optimizer_Short_Description"
source: "EN-AWDefect_Optimizer_Short_Description.pdf"
tags: ["A+W", "Defect Optimizer", "Glass Manufacturing", "Software", "Quality Control", "Optimization", "Viprotron", "Hegla", "Realtime Optimizer"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a brief description of the A+W Defect Optimizer software. It outlines the software's purpose, which is to identify and optimize cutting patterns for glass sheets to avoid defects. The guide covers the requirements for deployment, the benefits of intelligent defect optimization, and the step-by-step procedure for its use in a production environment, including integration with quality scanners and cutting systems."
long_description: "This is a user guide and brief description for the A+W Defect Optimizer, a software solution designed for the glass, windows, and doors industry. The document begins with editorial notes, copyright information, and display conventions. The core of the document is a tutorial that explains the functionality and benefits of the software. The A+W Defect Optimizer works by integrating with quality scanners (e.g., from Viprotron) and online cutting control stations (A+W Realtime Optimizer) to detect defects on jumbo stock sheets *before* cutting. It then re-optimizes the cutting pattern in real-time to avoid these defects, thereby reducing waste, saving costs, and increasing production quality and delivery reliability. The tutorial details the entire procedure, from sending the initial cutting code to the final, re-optimized cutting pattern that accounts for detected defects. It also explains concepts like defect classes and how the system handles different types of faults. The document is intended for end-users of the software."
---

# A+W Defect Optimizer - Brief Description

## Editorial

### Revision overview of the documentation
| Date | Version |
|---|---|
| 10-2014 | Original version. |

### Notes
This document is intended only for end users of A+W Defect Optimizer.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The content of the documentation serves only as information and can be changed without prior notice at any time.

The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The descriptions in this document are based on the full program level of A+W Defect Optimizer.

### Copyrights
© 2014, A+W Software GmbH, all rights, including the right of reprint, production of copies and translation, are reserved.

The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. This documentation may not be transmitted, neither electronically, nor mechanically, nor by recording or in any other way, without the prior written permission from A+W Software GmbH.

### Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### Display conventions
Individual elements of the sentences are displayed in a special form. The meanings are:

| Convention | Description |
|---|---|
| *Italics* | marks character strings describing the software elements, e.g. the *Buckets dialog*. |
| **Bold** | marks character strings to be entered via keyboard, e.g.: **Enter 5**. |
| > | The "bread crumb trail" marks the path that you can use to open a dialog, e.g. *Master data > Prices > IG Prices*. |
| [] | Square brackets mark the buttons in the dialog, e. g. [OK] to save the data. |
| < > | Pointed brackets refer to keys or shortcuts on the keyboard, e. g.: <F1> is used to open the online help. |

### Contact
**A+W Software GmbH**  
Siemensstr. 3  
D-35463 Fernwald  
Deutschland

**Tel.:** +49 641 96620 0  
**E-Mail:** info@a-w.com  
**Web:** http://www.a-w.com

## Content

- **Tutorial** A-7
- **A+W Defect Optimizer introduces itself** A-9
- **Intelligent defect optimization** A-10
  - Your benefits A-10
- **Procedure** A-11
  - Detection of defective areas A-11
  - Processing of defective areas A-13
  - The online analysis A-14

## Tutorial

This section provides information on the following subjects:
- ⇨ A+W Defect Optimizer introduces itself
- ⇨ Intelligent defect optimization
- ⇨ Procedure

### A+W Defect Optimizer introduces itself
Statistically speaking, every second jumbo stock sheet is defective. At the same time, inclusions and defects on stock plates and residual plates are often only noticed very (or too) late - for example, during quality control before/after the IG assembly or, in the worst case scenario, at the customer.

In these cases, you have already incurred considerable costs for the production (and shipping) of the stock sheet. And now you are making another investment to produce another stock sheet and (where applicable) resend it to the customer.

Why not identify defects prior to cutting and take them into account during the optimization process?

#### Requirements for using A+W Defect Optimizer
In order to deploy A+W Defect Optimizer in your company, the following requirements must be met:
- A+W Realtime Optimizer (online cutting control station) version 12.3 and up must be available and installed.
- An inspection system that reliably reports the corresponding data when the stock plate runs through the machine (e.g. quality scanner by Viproton).

### Intelligent defect optimization
The stock plates are scanned in conjunction with a quality scanner, e.g. from Viprotron, and any faults or defects are detected and displayed. The earlier defects are detected during the process, the lower the incurred costs.

Defects are taken into account during optimization for the restructuring of the sectional image. If there are any orders that are to be considered, then those will of course be taken into account.
Defects in residual plates are also stored, and can thus be reused later without additional inspections.

If defects cannot be avoided through the optimization process (e.g. number and size of stock sheets on pattern), the optimization process tries to use smaller and thus cheaper glass panes for the defects.

Glass that is positioned on defects is automatically reported as breakage and is recut.

#### Your benefits ...
... from using A+W Defect Optimizer in summary:
- Increase in quality through defect avoidance
- Significant cost reduction due to early detection of defective areas prior to the cutting process and restructuring of the optimization process (using A+W Realtime Optimizer and quality scanner, e.g. Viprotron)
- Avoiding processing of already-defective stock sheets
- Selecting suitable suppliers through quality controls
- Increase in delivery reliability

### Procedure
In the following, you will find an overview of the procedure. For our example, we are using the following components:
- Compact loader from Hegla
- Automatic cutting system from Hegla (Optimax)
- Jumbo Controller from Viprotron
- A+W Realtime Optimizer
- A+W Defect Optimizer

#### Detection of defective areas
During the first step, the cutting codes that have been determined by the optimization process are sent to the cutting table.

**Fig. A-1:** Cutting code is sent to the cutting table

Subsequently, the cutting table sends the corresponding request for stock plates.

**Fig. A-2:** Stock plates are requested

The first stock plate is loaded and runs through the Jumbo Controller.

**Fig. A-3:** Detection of defective areas

The Jumbo Controller detects the defective areas and reports the corresponding coordinates to the A+W Defect Optimizer.

**Fig. A-4**

Based on the reported data, the A+W Realtime Optimizer creates the new cutting code and transmits it to the cutting table.

#### Processing of defective areas
Defective areas are displayed as follows:

**Fig. 2:** Defective areas in the cutting pattern

After another optimization process executed by A+W Defect Optimizer, the cutting pattern now looks as follows:

**Fig. 3:** New cutting pattern

> **Red circles around the defective areas**
> The red circles are only intended to show the defective areas; they are not available at the time of the run!

#### The online analysis
The A+W Defect Optimizer analyzes the inspection data for each individual stock plate during the transport and alignment of the plate on the cutting table.

**Fig. 4:** Defective areas

The system automatically detects the stock sheets that are affected and marks them in accordance with the trimming drawing display:

**Fig. 5:** Breakout Display

#### Defect classes
The defects are classified by size and type into two classes. One class includes the defects that are located on the stock sheet edge. These defects are tolerated and the stock sheet is not marked as breakage.
The other defects are in the visible area of a stock sheet. Those are reported as breakage.

The limits of these classes are determined in coordination with the customers.

> **Using breakage**
> If a stock sheet that has been marked as breakage can still be used (e. g. the defect was removed by cleaning), you can mark them with one click as OK!

