---
title: "EN-INST-AW_Dashboard"
source: "EN-INST-AW_Dashboard.pdf"
tags: ["A+W Dashboard", "Installation Guide", "Software Configuration", "Database Setup", "System Requirements", "Software Update", "Technical Documentation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides comprehensive installation instructions for the A+W Dashboard software, a tool for the glass and windows industry. It covers new installations, updates from previous versions, and initial configuration."
long_description: "This installation manual is a technical guide for planners and administrators responsible for deploying the A+W Dashboard software. The document is divided into two primary sections: a new installation and an update from versions 5.4/5.5. The 'New Installation' section details prerequisites, including server and client software requirements (IIS, browsers), database configuration (especially for A+W Production data), and network settings. It provides a step-by-step procedure for using the A+W SetupLauncher, creating database tables, importing standard forms, and setting up GUIDs for registration points. The 'Update' section addresses the specific steps needed to upgrade from older versions, highlighting changes in dependencies like the A+W Planning Job Service and the replacement of the A+W Corporate KPI Service. It includes procedures for uninstalling old services, checking the uninstallation, and converting data namespaces via SQL scripts to ensure compatibility. The guide also offers troubleshooting tips, such as purging browser cache and manually removing services."
---

# Installation Instructions A+W Dashboard

---
## Change history

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2014-05-26 | AKU | Original version | 1.0 |
| 2015-02-24 | AKU | Reworking for Version 5.5 | 2.0 |
| 2016-07-05 | MME | Reworking for Version 6.0 | 2.1 |
| 2016-07-21 | DLA | Reworking | 2.2 |
| 2016-11-28 | ΜΜΕ | Reworking | 2.3 |
| 2017-05-24 | ΜΜΕ | Section 1.4 - Default views in P:\Views | 2.4 |
| 2007-09-11 | DLA | Adaption section 1.4 | 2.5 |

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

## Content

*   **Installation Instructions**
    *   **A+W Dashboard**
*   **1 New installation**
    *   1.1 Overview and the basics
    *   1.2 Time requirement
        *   1.2.1 Installation time for the software
        *   1.2.2 Conversion Time for Data Set
    *   1.3 Requirements
        *   13.1 Network
        *   1.3.2 Software
        *   1.3.3 Database
    *   1.4 Procedure
    *   1.5 Incompatibilities
    *   1.6 Directory structure
    *   1.7 Settings
        *   1.7.1 Database
    *   1.8 Result of the installation
    *   1.9 Tips and Tricks
        *   1.9.1 FAQs
        *   1.9.2 Known errors and workarounds
    *   1.10 Uninstalling
*   **2 Update from Version 5.4/5.5**
    *   2.1 Time requirement
    *   2.2 Procedure
    *   2.3 Uninstalling the old services
        *   2.3.1 Checking the uninstallation
    *   2.4 Converting data from Version 5.4
        *   2.4.1 Note regarding table names

## 1. New installation

The following installation instructions assume that there is no previous version installed. The set-up and additional configuration possibilities are described in the start-up documentation.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:
- Installation of the dashboard
- One-time execution of the dashboard
- Importing of the standard forms
- Adjustment of the GUID for the registration points to be displayed

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
- **Processor**: Intel Core i7 870
- **RAM**: 16 GB
- **Other**: Windows 8

For an initial or new installation, an installation time of 10 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

#### 1.2.2 Conversion Time for Data Set

Time for the conversion of existing data must be expected.

The importing of the data takes a certain amount of time. Furthermore, the registration points must already have a particular GUID so that the controls can display the data for the registration points.

An additional 30 to 60 minutes should be planned in.

### 1.3 Requirements

Prerequisite is an **A+W Infrastructure ProcessServer** in the customer environment.

In order to be able to display the PDC data, **A+W Production PDC** must be installed and used actively.

#### 1.3.1 Network

The URL for reaching the dashboard is `http://servername/corporate.web`

#### 1.3.2 Software

An IIS (at least Version 8) must be installed and activated on the server.

The client needs a new browser (e.g. Internet Explorer 10, Chrome 35) with activated JavaScript and CSS.

#### 1.3.3 Database

If A+W Dashboard should display booking data from A+W Production, then up to Version 6, the A+W Production database must absolutely be used as database for the A+W infrastructure.

Starting with Version 6 this is no longer necessary; for this, the database connection to the A+W Production database must absolutely be configured in the infrastructure. This is done in the System Configuration settings for A+W Production, where you define the `Host Name`, `Database`, `User`, and `Password`.

### 1.4 Procedure

In the A+W SetupLauncher, the following points must be installed including their dependencies.
- A+W Corporate Web
- A+W Corporate Dashboard Services

If booking data from A+W Production should be displayed, then the following services must also be installed.
- A+W CIM Services
- A+W Planning Job Service

For this, just select the **A+W Corporate ProcessServer** diskset in the Setup Launcher.

After the installation has been completed, the page must be called up in the browser again so that the database tables are created.

To do this, go to the link: `http://servername/corporate.web/Monitor`

The initial execution can take a moment.

After the page has been displayed, the standard forms can be imported into the database. Starting with version 6.4 these are copied to `P:\Views\AUW_DashboardViews.txt` via A+W Production SharedFolder disk set.

### 1.5 Incompatibilities

None known thus far.

### 1.6 Directory structure

None to heed thus far.

### 1.7 Settings

#### 1.7.1 Database

In order to be able to use the standard form for the PDC display, the registration points and status must be compared using the following SQL:

**SQLServer:**
```sql
SELECT '00000000-0000-4000-0000-000' + esbc, Guid, * FROM awbar_stellen;
SELECT '00000000-0000-4000-0000-000' + zustandbc, Guid, * FROM awbar_zustand;

UPDATE awbar_stellen SET Guid = '00000000-0000-4000-0000-000' + esbc;
UPDATE awbar_zustand SET Guid = '00000000-0000-4000-0000-000' + zustandbc;
```

**Informix:**
```sql
SELECT '00000000-0000-4000-0000-000' || esbc, Guid, * FROM awbar_stellen;
SELECT '00000000-0000-4000-0000-000' || zustandbc, Guid, * FROM awbar_zustand;

UPDATE awbar_stellen SET Guid = '00000000-0000-4000-0000-000' || esbc;
UPDATE awbar_zustand SET Guid = '00000000-0000-4000-0000-000' || zustandbc;
```

### 1.8 Result of the installation

On the first start of the browser, an empty space appears.

After the standard forms have been imported and the GUIDs of the registration points adjusted, the created forms should be visible. The dashboard will show controls for status and performance of various machines and machine groups.

If the A+W Dashboard should not be displayed, then you should check using the Service Locator Administrator (IceGrid Admin) whether the services are registered and started.

The log files for the service are here: `%ProgramData%\A+W\Log`

### 1.9 Tips and Tricks

#### 1.9.1 FAQs
*(No FAQs listed in the document.)*

#### 1.9.2 Known errors and workarounds

If the data is not displayed correctly or if changes in the views are not visible, then you should first purge the browser cache.

To do this, just press "F12" to open developer tools and press the "Delete browser cache..." button. Alternatively, you can use "Ctrl + R."

### 1.10 Uninstalling

To uninstall the dashboard, the installed programs must be uninstalled using the standard Windows function "Programs and Features."

It is recommended that of the dependencies, you first uninstall A+W Corporate Web, then A+W Corporate Dashboard Services, and finally A+W CIM Services.

## 2. Update from Version 5.4/5.5

The following installation description only describes the points that differ from the full installation described above and that must be heeded for an update.

An automatic update of the services is not possible since the procedures, precisely those for installation, have changed between the versions. A manual uninstallation of the services may be unavoidable under some circumstances.

### 2.1 Time requirement

15-30 minutes.

### 2.2 Procedure

Starting with Version 6.0, the **A+W Planning Job Service** is also required as an indirect dependency. In addition, the `A+W Corporate Service` was replaced by **A+W Corporate Dahsboard Service**. The `A+W Corporate KPI Service` does not exist any longer.

For an update from Version 5.4, an uninstallation of the services before the new installation is mandatory; in addition, the data must be converted due to structural changes.

Starting with Version 5.5, an update can work; in case of problems, install the services here too. In any case, the **A+W_Corporate_KPI Service** must be de-installed.

After the update, the database connection to the A+W Production database must be configured in the infrastructure; otherwise, the A+W Planning Job Service will not start.

If the A+W Dashboard should not be displayed, then you should check using the Service Locator Administrator (IceGrid Admin) whether the services are registered and started. In case of errors, uninstall the services and install them from scratch.

The log files for the service are here: `%ProgramData%\A+W\Log`

### 2.3 Uninstalling the old services

After the uninstallation, the machine should be rebooted.

Open "Programs and features" and select the following programs for uninstallation one after another:
- A+W Corporate 5 Web
- A+W Corporate 5 Services
- And/or A+W Corporate Dashboard Services
- And/or A+W Corporate KPI Services
- A+W CIM 5 Services

#### 2.3.1 Checking the uninstallation

Open the Windows services (Services) and check whether the following services were removed:
- A+W CIM 5 Barcoding
- A+W Corporate 5
- And/or A+W Corporate Dashboard Services
- And/or A+W Corporate KPI Services

If the services are still present, you must remove them using the command line.
1.  Open the command line as administrator.
2.  Open the Properties of the service that was not uninstalled.
3.  Copy the "Service name" from the General tab to the clipboard (e.g., `icegridnode.AWRegistry.VM-AKU-VS2013-CIM`).
4.  Close the Property window.
5.  Enter the following on the command line: `sc delete <service name>`

Check whether the services were removed from the IceGrid:
1.  Open the "Service Locator Administration" (IceGrid Admin) and log in.
2.  If the service nodes "localhost-CIM" and "localhost-Corporate" are still present, remove them using "Tools -> Application -> Remove from registry".

### 2.4 Converting data from Version 5.4

Namespaces have changed from Version 5.4 to Version 5.5. These are saved serially in the table.

In order to convert the data to SQL server, use the following SQL:
```sql
UPDATE cockpit_pages SET
namephrases=replace(namephrases, 'AWSOA.Core.Client.Data.CultureTextItem, AWSOA.Core.Communication', 'AWSOA.Core.Contracts.Data.CultureTextItem, AWSOA.Core.Contracts'),
descriptionphrases=replace(descriptionphrases, 'AWSOA.Core.Client.Data.CultureTextItem, AWSOA.Core.Communication', 'AWSOA.Core.Contracts.Data.CultureTextItem, AWSOA.Core.Contracts');

UPDATE cockpit_controls SET
namephrases=replace(namephrases, 'AWSOA.Core.Client.Data.CultureTextItem, AWSOA.Core.Communication', 'AWSOA.Core.Contracts.Data.CultureTextItem, AWSOA.Core.Contracts'),
descriptionphrases=replace(descriptionphrases, 'AWSOA.Core.Client.Data.CultureTextItem, AWSOA.Core.Communication', 'AWSOA.Core.Contracts.Data.CultureTextItem, AWSOA.Core.Contracts');
```

> **If this does not happen, no Dashboard will be displayed!**

#### 2.4.1 Note regarding table names

From version 6 update 2 on, the tables are called `dashboard_***`

