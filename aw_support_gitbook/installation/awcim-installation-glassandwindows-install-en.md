---
title: "EN-INST-AW_CIM"
source: "EN-INST-AW_CIM.pdf"
tags: ["A+W CIM", "Installation", "Software", "Glass and Windows", "Technical Documentation", "Setup", "Uninstallation", "Updates", "Configuration"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides installation, configuration, uninstallation, and update instructions for the A+W CIM software, which is part of the A+W software suite for glass and windows manufacturing."
long_description: "This document serves as a comprehensive guide for system planners and administrators tasked with deploying the A+W CIM (Computer Integrated Manufacturing) software. It outlines the step-by-step procedures for a new installation, including prerequisites, time requirements, and initial configuration. The guide details the necessary components to be installed, such as CIM Services, CIM Web, and Planning Job Services. It also covers post-installation procedures, including database table creation and service settings within the A+W Infrastructure. The document provides instructions for using key functions like BarcodeReading and Smart Terminal, with examples of URL structures for both standard and MultiSite environments. Additionally, it contains detailed uninstallation instructions, covering both the standard process through 'Programs and Features' and a manual command-line procedure for removing residual services. Finally, a dedicated section on updates explains the process and potential need for manual uninstallation due to version changes, along with troubleshooting steps for services that fail to start."
---

# Installation Instructions: A+W CIM

---
## Change history

| Date       | Edited by | Remarks                     | Version |
| :--------- | :-------- | :-------------------------- | :------ |
| 2016-07-05 | MME       | Original version            | 1.0     |
| 2016-07-21 | DLA       | Reworking                   | 1.1     |
| 2018-05-03 | DLA       | MultiSite and SmartTerminal | 1.2     |

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

# A+W CIM

## 1. New installation

The following installation instructions assume that there is no previous version installed. The set-up and additional configuration possibilities are described in the start-up documentation.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:

-   Installation of the CIM Barcoding Service
-   Installation of the Job Service (dependency)
-   Installation of the CIM Web

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data: 30 minutes.

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:

-   **Processor:** Intel Core i7 870
-   **RAM:** 16 GB
-   **Other:** Windows 8

For an initial or new installation, an installation time of 10 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

### 1.3 Prerequisites

A prerequisite is an A+W Infrastructure ProcessServer in the customer environment.

#### 1.3.1 Network

The URL for the CIM function is:
`http://servername/CIM.web/BarcodeReading`
`http://servername/CIM.web/SmartTerminalBooking`

#### 1.3.2 Software

An IIS (at least Version 8) must be installed and activated on the server.

### 1.4 Procedure

In the A+W SetupLauncher, the following points must be installed including their dependencies:

-   A+W CIM Services
-   A+W CIM Web
-   A+W Planning Job Services

After the installation has been completed, the page must be called up in the browser again so that the database tables are created.

To do this, go to the link: `http://<servername>/CIM.web/`

The initial execution can take a moment.

### 1.5 Settings

Since Version 6, the A+W Planning Job Service and the A+W CIM Barcoding Service use switches to find the A+W Production database. These must be set in the A+W Infrastructure. If the configuration is not correct, the services cannot be started in the IceGrid.

> **System Switch Management Configuration:**
> The settings for the database connection are configured under `Infrastructure -> Database -> A+W Production -> Datenbank Verbindung`.
> Key fields include:
> -   **Host Name:** e.g., `QM-DBSRV`
> -   **Instance:** e.g., `TSESQL2016EXP`
> -   **Database:** e.g., `alcimdb_v6_b1`
> -   **User:** e.g., `alcimdb`

### 1.6 Result of the installation

The services are addressed via browser (e.g., IE) in domain CIM.WEB. If the page is not displayed in the browser, then you must check in the Service Locator Administration (IceGrid Admin) whether the ICE services are registered and can be started.

The log files for the service are here: `%ProgramData%\A+W\Log\`

### Function BarcodeReading

This for-fee function serves as a scanner function on a Windows CE scanner, but can also be used from any browser.
`http://servername/CIM.web/BarcodeReading`

**In a MultiSite environment:**
`http://servername/CIM.web/SiteID/BarcodeReading`

Use the following addition (address) to add a StationID that is used to distinguish the different scanners during booking.
`?stationid=ID`

**Example:** `http://MyCimServer/CIM.web/BarcodeReading?stationid=5`

If you would like to know whether the A+W CIM Barcoding Service is working, you can click the upper bar code icon in order to enter a bar code manually, for example "600000000", which typically depicts the "logged off" user.

### Function Smart Terminal

This for-fee function offers an easy possibility to make bookings via browser by entering the barcodes.
`http://servername/CIM.web/SmartTerminalBooking`

**In a MultiSite environment:**
`http://servername/CIM.web/SiteID/SmartTerminalBooking`

### 1.7 Uninstalling

To uninstall the A+W CIM Service, the installed programs must be uninstalled using the standard Windows function "Programs and Features."

> **Uninstallation Order:**
> It is recommended that of the dependencies, you first uninstall A+W CIM Web, then A+W CIM Services, and then the A+W Planning Job Service.

#### 1.7.1 Checking the uninstallation

Open "Services" and check whether the following Windows services were removed:
-   A+W CIM 6 Services
-   A+W Planning Job Service

If the services are still present, you can remove them using the command line.

1.  Open the command line as administrator.
2.  Open the Properties of the service that was not uninstalled.
    > In the service's properties window, go to the `General` tab.
3.  Copy the "Service name" to the clipboard (e.g., `icegridnode.AWRegistry.VM-AKU-VS2013-CIM`).
4.  Close the Property window.
5.  Enter the following on the command line: `sc delete <service name>`

Check whether the services were removed from the "Service Locator Administration."

---

## 2. Updates

The following installation description only describes the points that differ from the full installation described above and that must be heeded for an update.

An automatic update of the services is not possible since the procedures, precisely those for installation, have changed between the versions. A manual uninstallation of the services may be unavoidable under some circumstances.

### 2.1 Time requirement

15-30 minutes.

### 2.2 Procedure

If the Barcode Scanner interface is not displayed or if it is not possible to enter a bar code, then you must check in the Service Locator Administration (IceGrid Admin) whether the services are registered and started (see [Result of the installation](#16-result-of-the-installation)).

**Required services:**
-   A+W Planning Job Service
-   A+W CIM Barcoding Service

Starting with Version 6.0, the CIM Service also requires the Job Service as a dependency.

#### 2.2.1 The job service does not start

For the Job Service, the A+W Production database connection must be stored in the infrastructure. Otherwise, the service will not start (see [Settings](#15-settings)).

#### 2.2.2 The CIM Barcoding Service does not start

Starting with Version 6, the CIM Service also requires the Job Service. First check whether this can be started.

If this is the case, you must uninstall and then reinstall the service (see also [Uninstalling](#17-uninstalling)).
