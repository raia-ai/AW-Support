---
description: "EN-FUNC-AW_Info_Terminal"
---


# A+W Functional Specifications
# A+W Info Terminal

**A+W - Software for Glass**

---

---
## 1. Contents

1.  **Contents**
2.  **Notes on this Document**
    1.  Trademarks
    2.  Copyrights
    3.  Exclusion of liability
3.  **Performance Description**
    1.  Data
    2.  Description
    3.  Requirements
    4.  List of functions
    5.  Limitations
    6.  Notes
4.  **Contact Address**

---

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2017, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to perform changes to software data, structure and interfaces as part of program extensions without prior notice. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This also includes possibly necessary long-term costs and expenses for amending and extending subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220095 |
| **Module** | A+W Info Terminal |
| **Brief description** | Information Terminal for Production |
| **Available** | Starting with A+W Production v6 |

### 3.2. Description

A+W Info Terminal handles the display of production-relevant information for individual sheets, orders or batches. In addition to pure display on a screen, with A+W Info Terminal it is possible to output reports or labels on a printer that can be selected.

Because A+W Info Terminal is only a tool for supplying information, there is no possibility here to make bookings for plant data collection or to generate machine code for activation.

### 3.3. Requirements

The prerequisite for the use of A+W Info Terminal is A+W Production with set up operating data collection. The formation of production batches with A+W Production is not necessary. The booking service A+W Production Booking and the PPS Web Service must be installed.

### 3.4. List of functions

For selection of the sheets, various search parameters can be entered. Typically, the order and item number are entered here. This can be done via manual input or entry using a locally-connected scanner. Available as additional search parameters are the batch number, physical rack or the exact sheet bar code.

In addition to the existing search parameters, the hit quantity can be restricted with a part filter. This way, it is possible to concentrate the search on end products or to focus specifically on the subparts of the main product.

Available to the user are a multitude of display elements for providing information. These include: the document link, an editing overview, special item information, a CAD drawing, defined production texts, and much more. For a better overview, it is possible to zoom in on the CAD drawing or it can be displayed on a separate monitor. Using a selection box, it is possible to switch between different CAD views.

From the menu bar, it is possible to select reports or labels and select a printer. The individual reports or labels are not included in the scope of delivery of A+W Info Terminal and must be specified and purchased separately.

A+W Info Terminal can display order information both for large series (see A+W Serial Manager) as well as for classic individual sheet orders.

### 3.5. Limitations

A+W Info Terminal is intended for a full HD screen resolution (1920 x 1080).

If A+W Info Terminal is running on a terminal server, there are limitations for the use of USB scanners. Ideally, you should use serial scanners here.

### 3.6. Notes
*(No notes provided in the document)*

---

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com
Internet: http://www.a-w.com/
