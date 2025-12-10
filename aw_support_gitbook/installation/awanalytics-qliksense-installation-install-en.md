---
description: "EN-INST-AW_Analytics"
---


# Installation Instructions: A+W Analytics powered by QLIK Sense®

---
## Change history

| Date | Author | Comments | Version |
| :--- | :--- | :--- | :--- |
| 2018-04-03 | DLA | Initial version and release | 1.0 |

## 1 New installation
A+W Analytics copies the basic package of our BI solution based on QLIK Sense® to the central QLIK Sense® Server.

### 1.1 Overview and the basics
The following list provides an overview of the work that must be done during installation:
- QLIK Sense® Server must be installed and configured on a dedicated server
- Installation A+W Analytics
- Installation of database drivers
- Configuration of database drivers (see configuration instructions)
- Configuration of A+W Analytics in QLIK Sense® Server (see configuration instructions)

### 1.2 Requirements
Installation is done on the central QLIK Sense® Server. This server is a dedicated server on which no other A+W applications are running.

#### 1.2.1 Hardware
Note system requirements if the QLIK Sense® Server should be put on by A+W.
[http://www.qlik.com/us/products/qlik-sense/system-requirements](http://www.qlik.com/us/products/qlik-sense/system-requirements)

#### 1.2.2 Network
QLIK Sense® communicates via various ports; it may be necessary to release these in the firewalls.
[http://help.qlik.com/en-US/sense/3.2/Subsystems/PlanningQlikSenseDeployments/Content/Server/Server-Deployment-Ports.htm](http://help.qlik.com/en-US/sense/3.2/Subsystems/PlanningQlikSenseDeployments/Content/Server/Server-Deployment-Ports.htm)

#### 1.2.3 License
The QLIK Sense® license must be activated. If this is not possible via the Internet since the QLIK Sense® Server has no access, the key can be generated manually with the following service: [http://lef1.qliktech.com/manuallef](http://lef1.qliktech.com/manuallef)

The license key is ordered from the dealer from whom the QLIK Sense® license was purchased.

If the license was ordered via A+W, this is a QLIK Sense® OEM license. With this, it is only permitted to evaluate data from A+W databases.

#### 1.2.4 Software
ODBC drivers (SQLServer, INFORMIX) are required in order to be able to load A+W Analytics data from the A+W databases.

### 1.3 Procedure
Via the A+W SetupLauncher, the A+W Analytics diskset and the required ODBC database drivers are installed on the central QLIK Sense® Server. After the installation, the configuration begins with the help of the configuration instructions.

### 1.4 Incompatibilities
A+W Enterprise is not yet supported. A+W products whose databases should be integrated must be at least Version 6. SQLBase databases are supported with restrictions.

### 1.5 Directory structure
The data is copied into a configurable directory on the server. There, a `QLIKDATA` subdirectory is created.

In this directory, various subdirectories are created, some of the data from these subdirectories must be loaded into the QLIK Sense® Server after the installation; for more details, see the configuration instructions.

> **A+W SetupLauncher Process:**
> The `A+W SetupLauncher` will display an "A+W Analytics Settings" window. You must enter the "Parent Directory for QLIK Data" (e.g., C:\). This action creates a `QLIKDATA` folder in the specified parent directory with the following sub-folder structure:
> - `Apps`
> - `Excel`
> - `Extensions`
> - `PNG`
> - `Scripts`

### 1.6 Configuration
Configuration is the larger part and must be done manually. Automation is not possible since QLIK Sense® does not support it. For more details, see the configuration instructions.

Configuration of the environment is done in the Excel file `.\Excel\CU_Config.xlsx`. This file is not overwritten during an update. All other files can be overwritten and thus any changes to these files are forbidden.

## 2 Update
An update copies new and updated existing files. Files are overwritten during an update with the exception of the configuration file `.\Excel\CU_Config.xlsx`.

### 2.1 Configuration
With a new version, new switches or even tables for the configuration file `CU_Config.xlsx` can come along. These are not entered automatically in it. Here, the new template `CU_Config_Template.xlsx` must be checked and new data transferred to `CU_Config.xlsx` if necessary.
