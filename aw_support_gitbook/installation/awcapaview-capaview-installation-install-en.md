---
title: "EN-INST-AW_CapaView"
source: "EN-INST-AW_CapaView.pdf"
tags: ["A+W", "CapaView", "Installation", "Software", "Glass", "Windows", "Setup", "Configuration", "Technical Guide"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides installation instructions for the A+W CapaView software, a solution for the glass and windows industry. It covers system requirements, installation procedures, configuration settings, and uninstallation steps."
long_description: "This is a comprehensive installation guide for A+W CapaView, a software product by A+W designed for the glass and windows industry. The document begins with a change history, detailing versions from 1.0 to 1.3. It outlines the necessary steps for a new installation, assuming no prior version exists. Key sections include system requirements (network and software), time estimations for installation, and a detailed procedural walkthrough. The guide specifies that an A+W Infrastructure ProcessServer and IIS Version 8 are prerequisites. It details the components to be selected in the A+W SetupLauncher, such as 'A+W Planning 6 Web' and 'A+W Planning 6 Job Services'. It also provides guidance on post-installation database configuration, troubleshooting steps if CapaView doesn't appear, and the process for uninstalling the software via the Windows 'Programs and Features' utility."
---

# Installation Instructions A+W CapaView

---
## Change history:

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2015-02-19 | AKU | Original version | 1.0 |
| 2016-07-05 | MME | Corrections | 1.1 |
| 2016-07-21 | DLA | Reworking | 1.2 |
| 2018-12-12 | DLA | Multi-site | 1.3 |

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1. Check the installation requirements.
2. Compile the required data, additional programs, drivers, etc.
3. Note or determine the time required.

## 1. New installation

The following installation instructions assume that there is no previous version installed. The set-up and additional configuration possibilities are described in the start-up documentation.

### 1.1 Overview and the basics

The following list provides and overview of the work that must be done during installation:
- Installation of the A+W CapaView

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
- Processor: Intel Core i7 870
- RAM: 16 GB
- Other: Windows 8

For an initial or new installation, an installation time of 10 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

#### 1.2.2 Conversion Time for Data Set
*(No content provided for this section in the document.)*

### 1.3 Requirements

Prerequisite is an A+W Infrastructure ProcessServer in the customer environment.

#### 1.3.1 Network

The URL for reaching the CapaView is
`http://<servername>/planning.web/capaview`

Please use the following address in an A+W Production multi-site environment:
`http://<servername>/planning.web/<SiteID Number>/capaview`

#### 1.3.2 Software

An IIS (at least Version 8) must be installed and activated on the server.

The client needs a new browser (e.g. Internet Explorer 10, Chrome 35) with activated JavaScript and CSS.

### 1.4 Procedure

In the A+W SetupLauncher, the following points must be installed including their dependencies.

- A+W Planning 6 Web
- A+W Planning 6 Job Services

*(A screenshot shows the 'A+W SetupLauncher' component selection window. The items 'A+W Planning 6 Job Services' and 'A+W Planning 6 Web' are highlighted as required for installation, along with their dependencies.)*

After the installation has been completed, the page must be called up in the browser again so that the database tables are created.

To do this, go to the link: `http://servername/planning.web/capaview`

The initial execution can take a moment.

### 1.5 Incompatibilities

None known thus far.

### 1.6 Directory structure

None to heed thus far.

### 1.7 Settings

Since Version 6, the **A+W Planning Job Service** uses switches to find the A+W Production database. These must be set in the A+W Infrastructure. If the configuration is not correct, the **A+W Planning Job Service** cannot be started in the IceGrid.

*(A screenshot displays the configuration interface for A+W services, specifically showing the 'A+W Production' database connection settings. Fields for Database, Host Name, Instance, Database, and authentication credentials (User/Password) are visible.)*

### 1.8 Result of the installation

With a call of the `http://servername/planning.web/capaview` page, the CapaView appears.

If the CapaView should not be displayed, then you should check using the Service Locator Administrator (IceGrid Admin) whether the services are registered and started.

The log files for the service are here: `%ProgramData%\A+W\Log`

### 1.9 Uninstalling

To uninstall the A+W CapaView, the installed programs must be uninstalled using the standard Windows function "Programs and Features."

*(A screenshot of the Windows 'Programs and Features' control panel lists various installed A+W software components. 'A+W Planning 6 Web' and 'A+W Planning 6 Job Services' are highlighted in the list, demonstrating where to find them for uninstallation.)*

It is recommended that of the dependencies, you first uninstall A+W Planning Web, then A+W Planning Job Services.
