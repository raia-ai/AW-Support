---
title: "EN-INST-AW_Planning_Stock"
source: "EN-INST-AW_Planning_Stock.pdf"
tags: ["A+W Planning Stock", "Software Installation", "Installation Instructions", "Technical Documentation", "Glass and Windows Software", "System Configuration", "Uninstallation", "A+W Infrastructure", "Job Service", "Stock Service"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides installation, configuration, update, and uninstallation instructions for the A+W Planning Stock software, a component of the A+W software suite for glass and windows manufacturing."
long_description: "This technical guide details the complete lifecycle management for the A+W Planning Stock software. It is intended for system planners and administrators responsible for deploying and maintaining the application. The document begins with an overview of the installation process, outlining prerequisites such as the A+W Infrastructure ProcessServer and IIS Version 8. It specifies system requirements for a reference device, including processor, RAM, and operating system, and provides an estimated installation time of 30 minutes. The guide walks through the installation procedure using the A+W_SetupLauncher, detailing the necessary components to install, including Planning Stock Services, Planning Web, and Job Services. It covers post-installation configuration, specifically how to set up the A+W Production database connection within the A+W Infrastructure. The document also provides instructions for verifying a successful installation by accessing the web interface and checking services in the Service Locator Administration. Furthermore, it includes a comprehensive section on uninstalling the software, with a recommended order for removing dependent components and a manual cleanup process for Windows services if they are not removed automatically. Finally, the guide addresses the update process, noting that automatic updates are not possible and manual uninstallation may be required. It highlights key checks and troubleshooting steps for updates, such as verifying service registration and database connections."
---

# Installation Instructions: A+W Planning Stock

**Software for Glass and Windows**

---

---
### Change history:

| Date        | Edited by | Remarks          | Version |
| :---------- | :-------- | :--------------- | :------ |
| 2018.11.21  | AKU       | Original version | 1.0     |

---

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## Content

- **Installation Instructions**
- **A+W Planning Stock**

### 1. New Installation
- **1.1 Overview and the basics**
- **1.2 Time requirement**
  - 1.2.1 Installation time for the software
- **1.3 Requirements**
  - 1.3.1 Network
  - 1.3.2 Software
- **1.4 Procedure**
- **1.5 Settings**
- **1.6 Result of the installation**
- **1.7 Uninstalling**
  - 1.7.1 Checking the uninstallation

### 2. Updates
- **2.1 Time requirement**
- **2.2 Procedure**
  - 2.2.1 The job service does not start

---

## 1. New Installation

The following installation instructions assume that there is no previous version installed. The set-up and additional configuration possibilities are described in the start-up documentation.

### 1.1 Overview and the basics

The following list provides and overview of the work that must be done during installation:
- Installation of the Planning Stock Service
- Installation of the Job Service (dependency)
- Installation of the Planning Web

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data: 30 minutes.

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
- **Processor:** Intel Core i7 870
- **RAM:** 16 GB
- **Other:** Windows 8

For an initial or new installation, an installation time of 10 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

### 1.3 Requirements

Prerequisite is an **A+W Infrastructure ProcessServer** in the customer environment.

#### 1.3.1 Network

The URL for the Stock function is:
```
http://<servername>/Planning.web/Stock
http://<servername>/CIM.web/SmartTerminalBooking
```

#### 1.3.2 Software

An IIS (at least Version 8) must be installed and activated on the server.

### 1.4 Procedure

In the A+W_SetupLauncher, the following points must be installed including their dependencies:
- A+W Planning Stock Services
- A+W Planning Web
- A+W Planning Job Services

After the installation has been completed, the page must be called up in the browser again so that the database tables are created.

To do this, go to the link: `http://<servername>/Planning.web/`

The initial execution can take a moment.

### 1.5 Settings

Since Version 6, the **A+W Planning Job Service** and the **A+W Planning Stock Service** use switches to find the A+W Production database. These must be set in the **A+W Infrastructure**. If the configuration is not correct, the services cannot be started in the IceGrid.

> **System Switch Management: Database Connection**
> The following settings for the A+W Production database connection must be configured in the A+W Infrastructure UI.
>
> - **Database Connection:** SqlServer
> - **Host Name:** QM-DBSRV
> - **Instance:** TSESQL2016EXP
> - **Database:** alcimdb_v6_b1
> - **Data Source Name (DSN):** alcimdb_v6_b1
> - **Windows Authentication:** OFF
> - **User:** alcimdb
> - **Password:** [hidden]
> - **Expert:** OFF

