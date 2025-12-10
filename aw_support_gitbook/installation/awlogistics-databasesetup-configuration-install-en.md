---
title: "EN-INST-AW_Logistics_Optimizer"
source: "EN-INST-AW_Logistics_Optimizer.pdf"
tags: ["A+W Logistics Optimizer", "Installation Guide", "Software", "Database Setup", "Configuration", "ERP Integration", "SQL Server", "ODBC", "Licensing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides comprehensive installation and configuration instructions for the A+W Logistics Optimizer software. It covers database setup, ODBC source creation, software installation via the SetupLauncher, and post-installation database updates. The guide also details configuration for integration with A+W Business 5/6, software licensing, and necessary Internet Explorer security settings."
long_description: "This is an official installation manual for the A+W Logistics Optimizer, a software solution for glass and windows logistics. The document is intended for planners and technical personnel responsible for deploying the software. It begins with a change history, tracking versions from 1.0 to 13.4.0. The core of the manual is divided into two main sections: Installation and Configuration. The Installation section provides step-by-step guidance on preparing the system, starting with database creation in SQL Server by restoring a backup file (OTR.BAK). It then covers creating a 32-bit ODBC system data source and running the main installation from the A+W SetupLauncher. A crucial post-installation step is updating the database using the OTR DB Updater tool. The Configuration section details how to integrate the Logistics Optimizer with other A+W products. For A+W Business 5, it explains how to create custom formulas and buttons to launch the optimizer. For A+W Business 6, it notes the shift to using the A+W Commercial Logistic Service. The guide also covers setting up database connections within the optimizer, licensing the application (including how to obtain a temporary license), and configuring Internet Explorer's Trusted Sites to ensure map functionality."
---

# Installation Instructions: A+W Logistics Optimizer

**Software for Glass and Windows**

---
## Change history:

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2013-10-01 | PK | Original version | 1.0 |
| 2014-01-10 | DLA | New Version | 1.1 |
| 2014-09-02 | JL | New Functions | 1.1.1 |
| 2015-02-05 | JL | New Version | 1.2 |
| 2016-02-26 | D.Langsdorf | Database directory | 13.0.0 |
| 2016-04-06 | B. Michel | Last change Version 6 | 13.0.1 |
| 2016-07-27 | DLA | DB update and adjustments | 13.1.0 |
| 2017-12-15 | DLA | DBUpdate tool on DB server | 13.4.0 |

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

## Table of Contents

*   **1 Installation**
    *   1.1 Database
        *   1.1.1 Database Creation
    *   1.2 Create ODBC Source
    *   1.3 SetupLauncher
        *   1.3.1 Database Update
*   **2 Configuration**
    *   2.1 A+W Business 5 + Pro
    *   2.2 A+W Logistics Optimizer database connection
    *   2.3 ERP interface
    *   2.4 Licensing the A+W Logistics Optimizer
    *   2.5 Internet Explorer
        *   2.5.1 Compatibility with Internet Explorer 10

## 1. Installation

The following installation instructions assume that there is no previous version installed. Setup and additional configuration options are described in the Configuration Documentation.

### 1.1 Database

Before starting installation, a database has to be created for the Logistic Optimizer in SQLServer.

#### 1.1.1 Database Creation

The Restore function in the SQLServer Management Studio has to be used for creating the database. The backup file OTR.BAK has to be restored.

This is located in the following folder:
`...\Diskset\A+W Logistics Optimizer\DB\OTR.BAK`

> **Note:** The screenshot shows the "Restore Database" (Datenbank wiederherstellen) dialog in SQL Server Management Studio.
> *   **Destination Database (In Datenbank):** OTR
> *   **Source (Quelle):** From device (Von Medium) is selected, pointing to the `OTR.BAK` file.
> *   The backup set to restore is "OTR-Full Database Backup".

Another way to create the database is to do it manually and then to execute each of the files in the `[.\Scripts\SYSDAM.OTR_*.SQL]` folder. These create the database. The scripts are located at:
`...\Diskset\A+W Logistics Optimizer\DB\Scripts`

### 1.2 Create ODBC Source

A 32-bit system ODBC Source has to be created on the OTR database so that reports can also be printed from the OTR. For this purpose, use the ODBC Administrator under:
`"C:\Windows\SysWOW64\odbcad32.exe"`

The name of the ODBC connection has to be **"OTRcr"**.

Follow these steps in the "Create a New Data Source to SQL Server" wizard:
1.  **Name:** `OTRcr`
2.  **Description:** `A+W Logistic Optimizer`
3.  **Server:** Enter your SQL Server instance (e.g., `localhost\awmssqlsvr`).
4.  Select "With SQL Server authentication using a login ID and password entered by the user."
5.  Enter the appropriate Login ID (e.g., `alcimdb`) and Password.
6.  Check the box for "Change the default database to:" and select `OTR` from the dropdown list.
7.  Click `Next` and then `Finish`.

### 1.3 SetupLauncher

A+W Logistics Optimizer is contained in the A+W Setup Launcher. The launcher will show the currently installed components and the versions available in the setup package.

The following dialogs appear during the installation process:
1.  **Welcome Screen:** The wizard starts. Click `Next`.
2.  **Destination Folder:** Choose the installation folder. The default is `C:\Program Files (x86)\ORB OTR\`. Click `Next`.
3.  **Ready to Install:** Click `Install` to begin the installation.
4.  **Installing:** A progress bar shows the status.
5.  **Completed:** The installation finishes. Click `Finish`.
6.  **Setup Successful:** A confirmation dialog appears. Click `Close`.

After installation, A+W Logistics Optimizer must be found under **Programs and Features** in the Control Panel.

#### 1.3.1 Database Update

After the installation or after an update, the database must be brought up-to-date. The **OTR DB Updater** is used for this purpose. This tool can be found in the installation directory: `Ort.DbInstaller.EXE`.

> **Warning:** OTR DB Updater must run on a server on which a SQLServer or its components are installed, since the tool uses these. Either install OTR completely on a DB server or copy the OTR directory from a ProcessServer to the DB Server.

In the OTR DB Updater tool:
1.  Enter the **Server Name**, **Database User name**, **Password**, and **Database Name** (OTR).
2.  For **Scripts path**, select the sub-directory "Databases" within the OTR installation folder (e.g., `C:\Program Files (x86)\A+W\OTR\Database`).
3.  Click **Test database** to verify the connection.
4.  If the test is successful and updates are pending, click **Update**.
5.  The log will show the progress and confirm when the database is up-to-date.

## 2. Configuration

> From A+W Business 6 on, the OTR is connected over the A+W Commercial Logistic Service. Therefore, point 2.1 is not necessary any longer, since OTR is not directly connected to the ERP database anymore. You must read the service's Installation Manual thoroughly, in order to completely commission the integration. The integration in A+W Business 6 is not part of this Installation Manual.

### 2.1 A+W Business 5 + Pro

Using customizing, an additional button has to be integrated so that the OTR software can be called from AWB5. To do this, you have to create 2 formulas. One formula describes the button (BUTTON OTR) while the other one describes the function that is assigned to the button (EXECUTE OTR).

To do this, you open "Masterdata/Company/Formulas" in AWB and insert the 2 new formulas.

1.  **Formula 1 (Button Definition)**
    *   **Number:** `20000`
    *   **Description:** `BUTTON OTR`
    *   **Content:**
        ```sql
        !** BOTON OTR ;
        **************
        udf_CreateButton('OTR', 'OTR.bmp', 20001);
        ```

2.  **Formula 2 (Execution Logic)**
    *   **Number:** `20001`
    *   **Description:** `EXECUTE OTR`
    *   **Content:**
        ```sql
        !** EXEC OTR;
        SET g_nUdv[1]=0;
        SET g_nUdv[2]=0;
        SET g_sUdv[3]='"C:\\Program Files (x86)\\A+W\\ALFAK 2012\\OTR_APP\\Ort.App.exe" ' || dfsMITARB_ID || ' ' || dfsNV_NAME;
        SET g_nUdv[2]=SalLoadAppAndWaitForProcessing(g_sUdv[3], 1, g_nUdv[1]);
        SET g_sUdv[1]=SalNumberToStrX(g_nUdv[1], 0);
        ```
    
    *   The formula numbers (here 20000 and 20001) should stay as these values. If existing formulas have already been assigned these numbers, other values can be used. Here, it must be ensured that the reference made in the first formula to the second formula (20001), is entered correctly.
    *   Additionally, it must be ensured that the path to the OTR software (`Ort.App.exe`) that is included in the 2nd formula is also entered correctly.

Then the button has to be integrated in such a way that it appears when called by the Number Manager. To do this, you open the Number Manager under "Documents/Order/NM order".

By right-clicking on the upper window bar of the Number Manager, you open a context menu. Select "Customizing Buttons erstellen" (Create Customizing Buttons). In the formula search dialog that appears, select formula `20000 BUTTON OTR`.

Following a restart of A+W Business, the new "OTR" button should now be visible in the Menu Bar once the Number Manager is opened.

### 2.2 A+W Logistics Optimizer database connection

The OTR database and if necessary the OTR archive database have to be entered the first time the A+W Logistics Optimizer is executed. This is done via the **Configuration -> Database** menu.

*   **OTR Connection Tab:** Enter the Data Source, Initial Catalog (`otr`), User ID, and Password for the main OTR database.
*   **OTR Archive Connection Tab:** (If applicable) Enter connection details for the archive database.
*   **ERP Connection Tab:** If A+W Business 5 is used, the connection to the ERP database must be configured additionally. Check "Use SQL Connection ERP System" and enter the Data Source, Initial Catalog (e.g., `AUW50`), User ID, and Password.

> **Please note:** These settings have to be made for each Windows user. From version 6, the tab "ERP Connection" is no longer configured.

### 2.3 ERP interface

From A+W Business 6, the switch **AW_ERP_INTERFACE** must be set in A+W Logistics Optimizer, so that OTR communicates with the A+W Commercial Logistic Service.

Go to **Configuration -> Parameters**. Find the parameter `AW_ERP_INTERFACE` and set its value to `Yes`. After that, the program must be restarted.

### 2.4 Licensing the A+W Logistics Optimizer

If you see the message "Invalid map service license" in the A+W Logistics Optimizer status line, you need to acquire a license. The installed system has a temporary license that is valid for 5 days.

To get a new license:
1.  Click on the **Start** Tab → **About OTR**.
2.  In the "About OTR" dialog, click the **[Temporal license]** button.
3.  A "Request license data" form will appear. Complete the following fields:
    *   **Customer:** Name of the customer.
    *   **License Name:** Name or description where OTR is installed.
    *   **Company Consultancy:** (e.g., A+W)
    *   **Consultant Name:** Your name.
    *   **Comment:** (e.g., AWDesk ticket number)
4.  Click **[OK]**. This creates a temporary license that is valid for 5 days.

When the license has been successfully issued, the "About OTR" dialog will display a license key and the [Temporal license] button will be replaced with a [License Information] button.

If you have a problem with the online license creation, please send an e-mail to **jordi.luque@a-w.com**.

### 2.5 Internet Explorer

Internet Explorer 10 or higher must be installed to be able to work with the A+W Logistics Optimizer. There are security issues with Internet Explorer in some instances. After installing the map license, you may need to adjust security settings.

Enter the following URLs in the Internet Explorer Security Settings as **Trusted Sites**:
*   `https://otrservice.onerbox.com`
*   `https://js.cit.api.here.com`
*   `https://1.base.maps.api.here.com`
*   `about:security_Ort.App.exe`

> It is absolutely imperative that the URL `"about:security_Ort.App.exe"` is included and that the checkbox **"Require server verification (https:) for all sites in this zone"** is deactivated for the Trusted Sites zone.

The following messages can appear when calling the maps through Nokia Maps if the settings are incorrect.
