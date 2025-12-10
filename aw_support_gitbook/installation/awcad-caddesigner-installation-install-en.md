---
description: "EN-INST-AW_CAD_Designer_Shapes"
---


# Installation Instructions: A+W CAD Designer 6 (Shapes)

**Software for Glass and Windows**

---
## Change history:

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 11/2012 | Bernd Hanewinkel | Version 2012 | 1.0 |
| 05/2014 | Bernd Hanewinkel | Cl adjustment | 1.1 |
| 07/2014 | Bernd Hanewinkel | Screen adjustment | 1.2 |
| 09/2016 | Bernd Hanewinkel | Adjustments Version 6 | 1.3 |
| 12/2022 | Bernd Hanewinkel | Adaptation system requirements | 1.4 |

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## Content

*   **Installation Instructions**
    *   **A+W CAD Designer 6 (Shapes)**
*   **1. Overview and the basics**
    *   1.1 Requirements
        *   1.1.1 Hardware
        *   1.1.2 Network
        *   1.1.3 Software
        *   1.1.4 Database
*   **2. Installation**
    *   2.1 Configuration
        *   2.1.1 SetUp settings
        *   2.1.2 Global settings
        *   2.1.3 User settings
        *   2.1.4 services
        *   2.1.5 Overview
        *   2.1.6 Update Files
        *   2.1.7 Finish

---

## 1. Overview and the basics

### 1.1 Requirements

#### 1.1.1 Hardware
No special requirements.

#### 1.1.2 Network
A+W CAD Designer 6 requires at least a 10 Mbit Ethernet (10Base2 / IEEE 802.3a, 10Base-T / IEEE 802.3i) network, better Fast Ethernet or Gigabit Ethernet.

#### 1.1.3 Software
For A+W CAD Designer (Shapes), installation on Windows 10 or Windows 11 is recommended. If it is to be run on a terminal server, Windows Server 2008 R2 or higher is required.

Reinstallation on older systems is not supported. Windows systems for which Microsoft support has expired may have limited support.

Please also remember to install all other available service packs for the framework and the operating system. We recommend to always keep the server up to date with the Microsoft Update Service.

#### 1.1.4 Database
No database required.

---

## 2. Installation

The setup for A+W CAD Designer 6 is available from `\\jupiter\SW_Install\v6`.

In connection with A+W Production /A+W Business /A+W Enterprise, A+W CAD Designer (Shapes) will be installed automatically. For details on these installations please refer to the corresponding installation instructions. A+W CAD Designer is part of the program group A+W Common. The ticked box in front of A+W Common means that elements from the A+W Common section will be installed as well.

**Fig.: 1 Setup-Launcher - Component selection**

The component selection window shows a tree of available A+W software components. The following components are listed under "A+W Common":
- A+W AWUpdate ToolDatabase
- A+W Basic Data 6 Services
- A+W CAD 6 Services
- A+W CAD 6 Web
- A+W CAD Designer (Bars)
- A+W CAD Designer (Bars) Interface Service
- A+W CAD Designer (Shapes)
- A+W CAD Designer (Shapes) Picture Service
- A+W CIM 6 Services
- A+W CIM 6 Web
- A+W Commercial 6 Document Services
- A+W Commercial 6 Logistic Services
- A+W CommonBase Configuration
- A+W CommonBase Database Updates v6
- A+W CommonBase Services
- A+W Corporate 6 Cockpit Services
- A+W Corporate 6 KPI Services
- A+W Corporate 6 Web
- A+W Discovery
- A+W ERP Stock Service 6
- A+W ERP Web Service 6
- A+W Infrastructure 6 Collector Services
- A+W Infrastructure 6 Middleware
- A+W Infrastructure 6 Service Locator
- A+W Infrastructure 6 Services
- A+W Infrastructure 6 Web
- A+W Infrastructure 6 Workflow Studio
- A+W iQuote 6 Services
- A+W iQuote 6 Web
- A+W LicenseClient
- A+W LicenseServices
- A+W LicenseServices Monitor
- A+W Planning 6 Automation Services
- A+W Planning 6 DataProvider Services

---

### 2.1 Configuration
After installation, the configuration tool for A+W CAD Designer is started.

#### 2.1.1 SetUp settings
In the first dialog, the user has to decide if the configuration shall be based on default settings or on the existing settings.
- For a new installation, choose **Start from default values** then move on with **Next**.
- To start from the current configuration, directly choose **Next**.
- To keep the current configuration and make no changes, choose **Close**.

If **Start from default values** is selected, the existing configuration will be lost!

The system does not decide automatically here. This is due to the fact that configuration settings will be kept even if the system is uninstalled then installed again. You can therefore keep settings although the installation is officially a new one.

The standard settings will be determined based on the installed programs.

If you use **Next** to move through the following menus you will always get an executable system. This is perfectly sufficient in the A+W Enterprise/Business environment.

**Close** aborts the configuration without further changes and is therefore the right choice for an update. **Next** will bring you to further settings.

#### 2.1.2 Global settings
The following menu serves to select a couple of global settings. The screenshot shows the default setting for the fields with A+W Production installed. SN is configured in the SN Server Directory, in this case in the sub-directory SN of the Alcim Server Directory, i.e. in `trans\SN`. The user-specific configuration is based on the ALCIM Station ID. The SN catalog for standard shapes is found in `\trans\SN\Catalog`.

If A+W Production has not been installed, the directory `%ProgramData%\A+W\Techsoft\SN` is chosen as the default location for the configuration, i.e. usually `C:\ProgramData\A+W\Techsoft\SN`. This is not the installation directory (`c:\Program Files (x86)\A+W\Techsoft\SN`)! The installation directory usually offers only limited access rights which make a change of configuration difficult and quite error-prone.

The settings for the SN Server Directory is the main switch in the AW Enterprise/ AWBusiness environment. A central configuration can be set up here by means of network release.

Via the **protocol** button, the trace and log level can be set.

##### Log Configuration
The Log Configuration window allows setting the following:
- **Scope**: Global or User
- **Retention Days**: e.g., 14
- **Combined Trace/Log setting**: e.g., Error, Info
- **Category-specific levels**:
    - **Category**: CAD
    - **Trace Level**: Error
    - **Log Level**: Info

#### 2.1.3 User settings
The next dialog shows the settings for the current user. During installation this is usually an administrator, i.e. none of the future users so that his menu is just meant for information. If `Use ALCIM Station ID` has been selected in the first menu, the field `User Station ID` is grey and cannot be changed. Otherwise, you can enter a (SN) Station ID for the current user. This way, a user-specific CAD Designer configuration can be defined in A+W Business/A+W Enterprise.

#### 2.1.4 services
The next dialog configures the users for which A+W CAD Designer runs as a service. The user for scheduling should be entered here (if scheduling shall be started on this computer). A user should be added by means of the button **Add user**. All necessary system settings will be made now so that the processes can be run in the background.

When you proceed to the next menu, the settings will be saved in the Registry. Up to that point you can use **Close** to abort the configuration; the system will remain unchanged.

#### 2.1.5 Overview
The menu **Overview** shows a list of settings. At the bottom, the entry in category Registry shows that the switches have been set successfully.

**Meaning of the paths:**

-   **SN Installation Directory:** Installation directory. This is where SN.exe is found. (e.g., `C:\Program Files (x86)\A+W\Techsoft\SN\`)
-   **SN User Directory:** This is the directory in which SN is executed. This is the standard path in which SN searches first for data without an absolute path. This is where (in the production environment) the files `Block.PTH` and `opt2txt.dat` should exist. (e.g., `C:\Users\bhanewinkel\AppData\Roaming\A+W\TECHSOFT\SN`)
-   **SN.INI Path:** The path for SN.INI. (e.g., `\\ALFAK\ALCIM2012S\Trans\SN\SN.INI`)
-   **User Data Directory:** The specific user data are stored here. The configuration tool shows the path for the user who has started the configuration tool. For the SetUps this is the installing user. In connection with ALCIM, this path is created by the Station ID. This is where additional data can be stored which are copied to the user directory when `SN.exe` is started. Supplements for `SN.ini` can also be stored here which override the switches in the standard `Sn.ini`. Example: a SN.ini which only includes the lines:
    ```ini
    [Customer]
    Machines = BZ1
    ```
    The machine PC1 is enabled for this user; all other machines are disabled. Still, all machines can be listed in the central SN.ini to permit a central configuration.
-   **DefaultData:** Data stored here will be copied to `%APPDATA%\Techsoft\SN` for all users. (e.g., `\\ALFAK\ALCIM2012S\Trans\SN\User\Default`)
-   **SN ServerDirectory:** Central configuration directory for SN. (e.g., `\\ALFAK\ALCIM2012S\Trans\SN`)
-   **Block.pth Path:** There are two entries for `BLOCK.PTH`. The first defines the contents of the file `BLOCK.PTH`, i.e. the path for the block file. The second shows where the `BLOCK.PTH` can be found.

The configuration tool can even be started without administrator rights. In this case, only this menu appears, showing a list of settings.

#### 2.1.6 Update Files
Next, the configuration tool copies data from the installation section to the configuration section (e.g. `Sn.ini`). In case of an update, there can be already data there. The tool offers a list of all files with conflicts in that case. This will be e.g. `SN.ini` if it does not match the standard SN.ini. These files will not be overwritten automatically unless the user ticks them on the list.

The "Update files in SNServerDir" dialog shows files that are new or changed in the current installation and differ from the files in the `SNServerDir`. You must choose which files to copy. If files in the `SNServerDir` have been manually adjusted (e.g., a standard shape file), you may need to add those changes manually to the new files.

#### 2.1.7 Finish
The configuration of the service is now finished. The final screen confirms "SN configuration is finished" and shows the path for the LOG file.
