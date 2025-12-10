---
title: "EN-FUNC-AW_Windows_CE_Scanner_Client"
source: "EN-FUNC-AW_Windows_CE_Scanner_Client.pdf"
tags: ["A+W Software", "Windows CE", "Scanner Client", "CIM Barcoding", "Functional Description", "Software for Glass", "Production Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a functional description for the A+W Windows CE Scanner Client, a web-based scanner application for production bookings. It details the software's purpose, requirements, functions, and limitations."
long_description: "This document provides a comprehensive functional overview of the A+W Windows CE Scanner Client, identified as module number 872505. The client is a web-based application designed for use with A+W Production v6 and later, facilitating production bookings via handheld scanners. The description outlines the system's advantages, such as hardware independence (requiring only a WLAN connection and Internet Explorer 6), ease of configuration, offline data storage capabilities, and direct error reporting. It specifies the necessary software and hardware requirements, including the A+W Infrastructure Process Server components and minimum specifications for Windows CE scanners (CE 6.0, IE 6.0, 240x320 display, WiFi). The document details the user interface, explains the meaning of various icons and display fields for booking results, and illustrates correct and incorrect booking sequences. It also lists hardware devices the client has been tested on (Datalogic, Motorola) and notes software limitations, such as a recommendation of a maximum of 50 offline scans and incompatibility of breakage bookings with the A+W Serial Manager."
---

# A+W Functional Description: A+W Windows CE Scanner Client

**A+W - Software for Glass**

---

---
## 1. Content

**1. Content**
- 2. Notes on this Document
- 3. Performance Description
- 4. Contact Address

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Disclaimer of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 872505 |
| **Module** | CIM Barcoding Client |
| **Brief description** | Web-based scanner application for bookings in production |
| **Available** | Starting with A+W Production v6 |

### 3.2. Description

The CIM-Barcoding Client is a Web-based scanner application. The application supported by A+W Production offers the following advantages:

- The application works regardless of the scanner hardware
- All you need is a WLAN connection and Internet-Explorer 6 on the scanner
- Easy configuration: Only a shortcut is required on the desktop, no software must be installed on the scanner
- Also saves the data in Offline mode
- Direct reporting in case of booking errors

### 3.3. Requirements

#### 3.3.1. Software

In order to be able to work with the CIM-Barcoding Client, the following infrastructure setups must be installed anywhere in the network (normally the process server). The "A+W Infrastructure Process Server" contains these setups.

- A+W Infrastructure 6 Collector Services
- A+W Infrastructure 6 Middleware
- A+W Infrastructure 6 Service Locator
- A+W Infrastructure 6 Services
- A+W Infrastructure 6 Web
- A+W Infrastructure 6 Workflow Studio

In addition, the following setups must be installed to run the scanner software (usually also on the process server):

- A+W Infrastructure 6 Collector Services
- A+W Infrastructure 6 Middleware
- A+W CIM 6 Barcoding Services
- A+W CIM 6 Web
- A+W Planning 6 Job Services

#### 3.3.2. Hardware (Scanner)

The Windows CE scanners used must fulfill at least the following minimum requirements:

- Windows CE 6.0
- Internet Explorer 6.0
- Display: 240 x 320 pixels
- WiFi-capable

### 3.4. List of functions

The interface of the CIM-Barcoding Client presents itself as follows on the scanner:

The fields above the dotted line display the booking results, the fields below display the last scanned bar code information.

| Symbol | Description |
| :--- | :--- |
| **0 1 1** | - **Black field:** number of non-processed bookings (of AlcimBooking) <br> - **Green field:** number of successfully processed bookings <br> - **Red field:** number of incorrect bookings |
| 