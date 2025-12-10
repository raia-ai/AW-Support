---
description: "EN-INST-AW_IOT"
---


# Installation Instructions A+W IOT Platform (Base Actiware)

**Software for Glass and Windows**

---
## Change history

| Date | Edited by | Comments | Version |
| :--- | :--- | :--- | :--- |
| 2019-01-09 | OSO | Original Version | 0.1 |
| 2019-01-30 | OSO | Screenshot added | 0.2 |

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## 1 New installation

The following installation instructions assume that there is no previous version installed. The set-up and additional configuration possibilities are described in the start-up documentation.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:
*   Install the Gateway Service

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
*   Processor: Intel Core i7 870
*   RAM: 16 GB
*   Other: Windows 8

For an initial or new installation, an installation time of 10 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

### 1.3 Requirements (Which?)

#### 1.3.1 Network

The URL for reaching the Infrastructure configuration:
`http://servername/infrastructure.web`

#### 1.3.2 Software

#### 1.3.3 Database

### 1.4 Procedure

In the A+W SetupLauncher, the following points must be installed including their dependencies.
*   A+W Corporate Gateway Service

For this, just select the A+W ? diskset in the SetupLauncher.

***

**[Image: Screenshot of the A+W SetupLauncher interface titled "Choose or create your installation diskset". It shows a list of "Available Disksets" on the left and a list of "Products" on the right. In the "Products" list, "A+W Corporate Gateway Service" is highlighted, indicating it should be selected for installation.]**

***

After the installation has been completed, the page can be called up in the browser again so that the database tables are created.

Please enter the following URL: `http://servername/infrastructure.web`

The initial execution can take a moment.

After the page is displayed, the parameters for configuration can be entered:

***

**[Image: Screenshot of a menu with the options "Gateway", "Gateway Verbindungseinstellungen", and "Reporting". The "Gateway Verbindungseinstellungen" option is highlighted.]**

***

### 1.5 Incompatibilities

None known thus far.

### 1.6 Directory structure

None to heed thus far.

### 1.7 Settings

#### 1.7.1 Database

TBD

### 1.8 Result of the installation

On the first start of the browser, the Infrastructure start page appears.

The setting for the Gateway Service can be made under configuration.

***

**[Image: Screenshot of the A+W Infrastructure web interface. The main page shows a background image of a glass ceiling and a menu on the right with options: Database, Configuration, License, Log, Trace, Basic data, and Workflow. The "Configuration" option is highlighted.]**

***

Enter the parameters for configuration in Gateway.

***

**[Image: Screenshot of the Infrastructure configuration page, specifically the "System switch management" section. It shows a long, collapsible list of configuration categories. The "Gateway" category is expanded, and the sub-item "Gateway Connection Settings" is highlighted with a red box.]**

***

The following parameters must be entered:

***

**[Image: Screenshot of the "Gateway Connection Settings" form. It contains fields for "Use Secure Protocol (https)", "Server Name", "Port", "Update Path", "Login User", and "Login Password". A red box highlights these input fields.]**

### 1.9 Tips and Tricks

#### 1.9.1 FAQS

#### 1.9.2 Known errors and workarounds

### 1.10 Uninstalling

Necessary?
