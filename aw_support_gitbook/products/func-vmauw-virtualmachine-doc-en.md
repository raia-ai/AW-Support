---
title: "VMAUW Functional Description"
source: "EN-FUNC-VMAUW.pdf"
tags: ["VMAUW", "A+W", "Virtual Machine", "Software", "Functional Description", "Internal Product", "Glass Software", "A+W Clarity"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a functional description of VMAUW, an internal virtual machine (VM) product from A+W. The VM is designed for A+W employees to facilitate presentations, training, and support by providing a pre-configured environment running current A+W Clarity products."
long_description: "This functional description details the VMAUW product, a virtual machine developed by A+W for internal use only. The primary purpose of VMAUW is to provide a standardized, ready-to-run environment for A+W employees to conduct presentations, training sessions, and handle support cases. The VM comes pre-loaded with a suite of A+W Clarity products, including A+W Business, A+W Enterprise, A+W Production, and various optimizers and design tools. The document outlines the technical specifications and prerequisites for running the VM, such as minimum RAM, required VMWare software, and licensing access. It also details the list of functions, included A+W products, system and application language support, and limitations, particularly regarding unit conversions and language localization. Furthermore, the document clarifies the process for requesting additional content or languages and outlines the responsibilities of MarketSolutions and other departments in maintaining and updating the standard VMAUW image."
---

# A+W Functional Description: VMAUW

---
## 2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The greatest care was used in compiling the texts and figures. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights
© 2016, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Without the prior written permission of A+W Software GmbH, the documentation may not be transmitted electronically, by recording or in any other form.

### 2.3. Exclusion of liability
A+W Software GmbH assumes no liability for data errors that rely on basic principles of the standard functions made available by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All adjustments, expansions, database queries, reports, analyses, and interface expansions that were created individually for our customers and/or machines and software partners as well as all costs and efforts associated with these were borne by the client (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary in order to ensure that the adjustments/expansions commissioned that were undertaken/developed for a version will also work perfectly and be used in the subsequent version.

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | VMAUW |
| **Article number** | None, VMAUW is an internal product |
| **Module** | Virtual machine |
| **Brief description** | VM for presentations, training, support |
| **Available** | Starting with v6 – older versions upon request |

### 3.2. Description
VMAUW is a virtual machine that runs current products from A+W Clarity. Its purpose is to aid in quickly establishing a running environment for presentations, training or support cases.
The current version of this VM can be downloaded here. A document on operation, changing languages, activation of the local license server, etc. can be found here.

### 3.3. Prerequisites
- Min. 4 GB RAM
- For the use of A+W Enterprise, at least an additional 3 GB RAM is needed in order to run the backend LINUX VM (VMAUWX).
- Licensed VMWare player 6.04 or VMWare workstation 1
- Access to a license server or an own A+W dongle.
- Users must be employed by A+W. The VM may not be given to customers or persons who are not employees of A+W!

### 3.4. List of functions

#### 3.4.1. General
The VMAUW is provided by Market Solutions and is created on the basis of basic databases maintained by Market Solutions. It contains one of the most recently released A+W Clarity versions. Subsequent hotfixes or patches may have to be installed independently.

#### 3.4.2. A+W products
VMAUW contains the following A+W Clarity products:
- A+W Business
- A+W Business Pro
- A+W Enterprise
- A+W Production (in combination with A+W Business and A+W Enterprise)
- A+W Production Monitor
- A+W Realtime Optimizer
- A+W Dashboard
- A+W CAD Designer
- A+W iQuote (in combination with A+W Business)
- A+W Logistics Optimizer (in combination with A+W Business)
- A+W License Server (deactivated in the standard version)

**System language**
In Windows systems, a user is available in the languages German, English, Spanish and French. Depending on the logged in user, the system (Windows and keyboard) switches to the respective language.

**Languages of the application**
A+W products are also rendered in the language of the registered user, if they support German, English, Spanish or French.
The language of external programs, such as MS SQL Server Management Studio, is generally English (if available); otherwise German.

**A+W Enterprise**
The databases for A+W Enterprise are available without and partially with internal client separation. This has not been fully implemented; if necessary this can be requested by means of a described requirement from Market Solutions.
The master data is available in German and for simple articles also in English. The articles in the master data are metric.

**A+W Business**
In the database, capacitive scheduling is active as a workflow. A document on deactivation can be found here.
The master data in the database consists of a mixture of German and English; it is currently not possible to switch languages. A corresponding project has been initiated and should make it possible in the future to switch master data from one language to another in the database.
The articles in the master data are metric.

**A+W Production**
The A+W Production database has been optimized for the communication with A+W Enterprise and A+W Business. There is a function with which you can switch to the other ERP system (see instructions); it is not possible to connect both ERP systems in parallel.
The basic master data is available in German, English, French and Spanish. Master data that cannot be localized in the database (e.g. names for machines or entry locations) can be switched by means of a function (see instructions) and can therefore not be run in parallel.
Article master data is transferred from the ERP system; the article master is transferred by means of system data alignment in collaboration with A+W Business.
The articles are displayed in metric measurement units.

### 3.5. Limitations

**A+W Production**
It is possible to switch A+W Production to inches (see instructions). However, in doing so, only the measurements contained in the database are converted to inch. This means:
- The article name does not change → a FLOAT 3mm will continue to be FLOAT 3mm (and not inch) in the name.
- The corresponding measurements cannot be precisely converted for the market for US customers → 3mm FLOAT here corresponds to 1/8 inch in the USA, which would result in a converted metric measurement of 3.125mm.

### 3.6. Notes

**Further content**
If additional content with regard to master data, sample orders or processes is desired, this can be directly sent via the AWDesk (Deleg. To AUW) or the MarketSolutions Helpdesk (in the intranet under "Service/MarketSolutions/Helpdesk"). MarketSolutions checks whether these additional requirements can be integrated into the standard version. In doing so, market relevance as well as compatibility with existing functions must be taken into account.

**Further languages**
If the A+W application supports the language, the applications A+W Production and A+W Business can be switched. For A+W Business, the corresponding language version also has to be installed. A+W Enterprise must be set up separately.
To create a Windows profile for the new language, this language can be installed in the VM if it is supported by Microsoft.
If you want to see the master data (articles, machines, etc.) of our products in the new language, they have to be translated. Here, the following expenses and restrictions must be observed:

**A+W Business**
The project "AWB translation tool" must be completed for it to be technically possible to translate the database into another language. A table is output with all texts, which can, if necessary, be translated into another language by our translation department. The translated article master data can then be transferred to A+W Production by means of article master data alignment.

**A+W Production**
In A+W Production it is possible to add a Western European language. To do so, Market Solutions will give lists of the required text to a translator. These are in Excel and do not correspond to any translation format. This applies to the following master data:
- Views and filters in rough scheduling
- Processing types
- Production data collection entry locations and statuses
- MZO machines

As A+W Production does not have a UNICODE database, non-Western European languages (such as Russian or languages of the Far and Middle East) cannot simply be added. For this, an independent database must be provided for this language on the VMAUW.
A user-dependent switch on such a database is only technically possible once the new multi-site function in A+W Production is complete and has been integrated by Market Solutions. This results in permanent extra work for Market Solutions, as with each new release, the databases for these languages have to be converted from our basic databases and made available.

**A+W Enterprise**
Extensions in A+W Enterprise are technically possible, if necessary, the work involved has to be determined and resources made available. Loosely speaking, the current master data has to be extracted from A+W Enterprise, given to the translation department and then imported again.

**Responsibilities**
The VMAUW can be used by every A+W employee - as it is. Customer-specific requirements and new patches, etc. are entered by the users themselves in their local copy. The responsibilities listed in the following refer to the standard VMAUW:

| No. | What | Who | Prerequisite |
| :-- | :--- | :--- | :--- |
| 1 | Provision of VMAUW | MarketSolutions | Takes place continuously after each new release |
| 2 | Notification of change requests (functions, master data, etc.) | Everyone | AWDesk case, positive review by MarketSolutions |
| 3 | Incorporation of new functions | MarketSolutions | AWDesk case from no. 2 |
| 4 | Additional language in operating system | MarketSolutions | Project and AWDesk case |
| 5 | Release of new language versions of A+W products | R&D | See release matrix |
| 6 | Installation of new language versions | MarketSolutions | Project and AWDesk case |
| 7 | Translation of scripts in order to convert master data in A+W Production | Doc. | MarketSolutions provides language Excel |
| 8 | Installation of new language packages from no. 7 | MarketSolutions | AWDesk case, positive review by MarketSolutions |

> **PLEASE NOTE:** MarketSolutions only maintains a standard database. If it is not possible to integrate new requirements in this database, an additional database must be created. The maintenance of this database however is the responsibility of the person using it (e.g.: USA database).

## 4. Contact Address
A+W Software GmbH  
Am Pfahlgraben 4 - 10  
35415 Pohlheim  
Germany

Tel. +49 6404 2051-0  
Fax. +49 6404 2051 877

E-mail: zentrale@a-w.com  
Internet: http://www.a-w.com/

---
*A+W - Software for Glass*
