---
title: "A+W Smart Terminal Functional Description"
source: "EN-FUNC-AW_Smart_Terminal.pdf"
tags: ["A+W Smart Terminal", "Functional Description", "Software for Glass", "Production Booking", "Web-based Interface", "CIM", "SOA", "A+W Production"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A functional description of the A+W Smart Terminal, a web-based interface for making simple production bookings. It details the product's purpose, requirements, functions, and limitations for use with A+W Production software."
long_description: "This document provides a comprehensive functional description of the A+W Smart Terminal, a software module for A+W Production v6 and later. The A+W Smart Terminal is a web-based interface designed to simplify production booking processes, such as assigning frames to registration points or sheets to racks. It can be operated on mobile devices like tablets. The document outlines the product's data, provides a detailed description of its functionality, and lists the necessary technical requirements, including SOA infrastructure, CIM Barcoding Service, CIM Web, and the Production Booking Engine. It also includes a detailed list of available booking functions with corresponding symbols, explains limitations like the need for manual data entry, and provides notes on device compatibility. Legal information, including trademarks, copyrights, and a disclaimer of liability, is also included, along with contact information for A+W Software GmbH."
---

# A+W Smart Terminal Functional Description

**A+W - Software for Glass**

---

---
## Notes on this Document

This documentation and the software described in it are only licensed and may only be used and copied pursuant to this license. The contents of the documentation are for information purposes only and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation may also be registered trademarks or other industrial property rights held by third parties. Copyrights of third parties must be complied with.

### 2.2. Copyrights

© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Disclaimer of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to perform changes to software data, structure and interfaces as part of program extensions without prior notice. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This also includes possibly necessary long-term costs and expenses for amending and extending subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220090 |
| **Module** | A+W Smart Terminal |
| **Brief description** | Web-based interface for bookings in production |
| **Available** | Starting with A+W Production v6 |

### 3.2. Description

The A+W Smart Terminal is a Web-based interface and allows the user to make simple bookings: frame to a registration point or sheet on rack. Here it is possible to search through the existing frame/registration points/states. After entry of the first character, you can select from a menu. The A+W Smart Terminal can be operated on a suitable mobile device.

> **UI Overview:** The user interface displays three counters at the top for non-processed, successful, and incorrect bookings. Below this, it shows the logged-in user. The main section contains several icons representing different booking functions. Underneath the icons are input fields for barcode and quantity, followed by a "Book" and a "Delete Fields" button.

### 3.3. Requirements

The A+W Smart Terminal requires the following components:

-   SOA infrastructure service
-   CIM Barcoding Service
-   CIM Web
-   Production Booking Engine / Service
-   Current browser with activated Javascript and cookies

### 3.4. List of functions

The following bookings are possible and must be selected accordingly:

| Symbol (Description) | Description |
| :--- | :--- |
| Icon of a barcode pointing to a rack | Unit to rack |
| Icon of a barcode pointing to a computer terminal | Unit to registration point |
| Icon of a rack pointing to a computer terminal | Rack to registration point |
| Icon of a traffic light pointing to a computer terminal | Status to registration point |
| Icon of a traffic light pointing to a barcode | Status to unit |
| Icon of a traffic light pointing to a rack | Status to rack |

After selecting the booking type, the corresponding data are entered in the respective fields and booking is made.

The three fields in the top section of the dialog show the booking results:

-   **Black field:** number of non-processed bookings (of AlcimBooking)
-   **Green field:** number of successfully processed bookings
-   **Red field:** number of incorrect bookings

### 3.5. Limitations

Data must be entered here manually and can NOT be scanned.
A+W Smart Terminal does NOT support the A+W Serial Manager!

### 3.6. Notes

The minimum resolution for mobile devices (tablets) is 385 x 420 pixels. Smartphones are not suitable for this application.

## 4. Contact Address

**A+W Software GmbH**

Siemensstraße 3
35463 Fernwald
Germany

**Tel.** +49 641 96620-0
**E-mail:** info@a-w.com
**Internet:** http://www.a-w.com/
