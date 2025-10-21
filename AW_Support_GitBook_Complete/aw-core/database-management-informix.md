---
title: "EN-INST-AW_Customizing_Manager"
source: "EN-INST-AW_Customizing_Manager.pdf"
tags: ["Installation Guide", "A+W Customizing Manager", "Software Configuration", "Database Management", "Informix", "DB2", "Customizing", "Software Deployment", "Version Control"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "An installation and user guide for the A+W Customizing Manager, a tool for managing and deploying software customizations like reports, scripts, and configuration files across multiple sites and environments."
long_description: "This document serves as a comprehensive installation and operations manual for the A+W Customizing Manager. It is intended for technically competent users responsible for installing the software and managing application customizations. The guide begins with prerequisites, detailing the necessary installation of the IBM.DB2 Driver Package and subsequent manual configuration of Windows Registry keys and GAC assemblies. The core installation process is covered, from using the A+W Setup Launcher to the initial database connection and setup, which currently supports INFORMIX. The guide then transitions to configuration, explaining how to set trace levels and define master data such as sites, environments (Live/Test), and path categories. A major section provides a step-by-step walkthrough of the tool's workflow, demonstrating how to create and manage 'Objects' (customization files). This includes adding new files, versioning them through 'test', 'release', and 'archived' states, and managing their metadata. The final part of the workflow covers the 'Publish' functionality, which allows users to simulate and then execute the deployment of these objects to their designated target environments. The document concludes with specific technical instructions for configuring Informix and DB2 databases to listen for the DRDA protocol, a necessary step for database connectivity."
---

# Installation Instructions: A+W Customizing Manager

**Software for Glass and Windows**

### Change history:
| Date | Edited by | Remarks |
|---|---|---|
| 2018-09 | DLA | First draft |
| 2018-10 | DLA | Second draft |

This document enables the competent reader to install the described software. You should generally stick to this procedure:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## Content
- **Installation Instructions A+W Customizing Manger**: 1
- **1 Introduction**: 3
- **2 Prerequisites**: 4
- **3 Installation**: 5
  - 3.1 First start: 5
  - 3.2 Configuration: 6
    - 3.2.1 Restrictions: 6
  - 3.3 Registries: 7
- **4 How it works**: 8
  - 4.1 Configure Master Data: 8
  - 4.2 Configure Objects: 11
  - 4.3 Publish Objects: 16
- **5 DB2 and Informix**: 19

---

## 1. Introduction

The A+W Customizing Manager supports the management of customizing, like Reports, scripts, configuration files, for a customer. It will be helpful for a company who handles the management by himself, e.g. a company who creates their own reports. The size of the company doesn't matter, but A+W Customizing Manager supports the handling of customizing in different sites.

The A+W Customizing Manager has to run once on a central place in the company. The tool is not made for multi-user work and has no right system. The user who is allowed to login at the A+W Customizing Manager database has access to all functions and objects stored in the application.

The A+W Customizing Manager has its own database, currently only INFORMIX. The database user login will be the user of this tool. This user is also used in the history protocol. So if you have different users which work with the A+W Customizing Manager (not in parallel!), use different database logins to see in history who has done what.

The tool is running on Windows OS.

## 2. Prerequisites

Install the IBM.DB2 Driver Package on the system before starting the A+W Customizing Manager setup. Currently we deliver the Version 11.1.3fp3 (`v11.1.3fp3_nt32_dsdriver_ALL_LANG`) as an extra package in the diskset.

If there is already an IBM.Data.Informix Driver installed on that system, you need to do some steps manually. Only then the IBM.DB2 Driver will fully work.

-   After the installation of the driver package, check (and add when missing) the Registry for the key:
    `HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\IBM\DB2\InstalledCopies`
    -> `"11.1.3030.DEF.4"="IBMDBCL1"`
    The value of the key must match your “InstalledCopies” DB2 Name.

-   Check the GAC Folder `C:\Windows\Microsoft.NET\assembly\GAC_32`. There should be two folders present (DLLs installed):
    -   `IBM.Data.DB2`
    -   `IBM.Data.DB2.Entity`

If they are not present, then you add them with an administrative Command Prompt and the `gacutil` tool.

Normally it could be found in one of these folders:
-   `C:\Program Files (x86)\Microsoft SDKs\Windows\v7.0A\Bin`
-   `C:\Program Files (x86)\Microsoft SDKs\Windows\v8.1A\bin\NETFX 4.5.1 Tools`

Or copy it from our Tools folder:
-   `\\jupiter\SW_install\Tools -> NETFX 4.7.2 Tools`

Run the following commands:
```bash
gacutil /i "C:\Program Files (x86)\IBM\IBM DATA SERVER DRIVER\bin\netf40\IBM.Data.DB2.dll"

gacutil /i "C:\Program Files (x86)\IBM\IBM DATA SERVER DRIVER\bin\netf40\IBM.Data.DB2.Entity.dll"
```
The commands should return "Assembly successfully added to the cache".

## 3. Installation

The A+W Customizing Manager is installed via the A+W Setup Launcher, under the section Common. Install the tool on a central server or PC.

This central Server or PC needs network access to the different servers of the different sites where files should be exchanged. For further versions, database access and corresponding database drivers to different environments are also needed.

To create the database, use the following command:
`CREATE DATABASE {db name} IN {DBSPACE name} WITH BUFFERED LOG;`

> **Important:** Don't forget to put this database into the backup jobs!

### 3.1 First start

After starting the application, the database login information must be entered.

**Login Fields:**
-   **Database Type**: Informix
-   **Database Server**: e.g., `10.1.31.153:9088`
-   **Database Name**: e.g., `customizing_manager`
-   **User**: e.g., `alcimdb`
-   **Password**: *[Enter password]*
-   **Database Locale**: `Client Locale=en_US.UTF8; Database Locale=en_US.UTF8`
-   **Database Owner**: e.g., `alcimdb`

If the database connection works, the application checks its database version and updates the table structure if needed. For this reason, the database user must have the right to change the database structure.

If you want to work with different users (not at the same time, as the tool isn't made for multi-user access), you need different database logins. The last login will be stored for each Windows user.

### 3.2 Configuration

Open the tab **Configuration**.

The settings for trace level, entity framework trace level, and language are stored for each Windows user and PC/server. To apply the changes, the application must be restarted.
-   **Trace Level**: Represents the application logs that are saved in the logging file.
-   **Entity Framework Trace Level**: Represents the level on which the scripts executed by entity framework will be logged by the logging mechanism.

The settings in the list on the right side are global parameters which are stored in the database.

-   **Object Output path**: The base path which is suggested if an object should be exported into a file.

The database owner represents the user that is responsible for creating the structure of the database. All the tables must be accessed using this user as schema. The database owner is set as default with the user that logged in for the first time in the application, but it can be modified manually after that from the configuration tab.

#### 3.2.1 Restrictions

When creating SQL objects (stored procedure, function, or view) the object name needs to be the same as the SQL object in the database. For example, an object for the stored procedure “cu_sealingtype" needs to be named “cu_sealingtype”.

The reason is the customizing manager uses this name when checking if the object exists in the target database(s) already. It will also use this name when dropping a database object before creating it.

If no owner is defined in the script, the owner defined in Master Data for the target database will be used. If no owner is defined in Master Data for the target database, the user logged into the A+W Customizing Manager is used.

### 3.3 Registries

All A+W Customizing manager registries can be found in:
`HKEY_CURRENT_USER\Software\A+W\AUW\CustomizingManager`

The registries are split into 4 subdirectories: `Database`, `DatabaseOwner`, `Language`, and `Trace`.

-   **Database folder**: You can find all the information needed to log in to the application (login to the Customizing Manager database). The password is encrypted and can be decrypted only from the same device on which it was stored in the registry.
-   **Database Owner folder**: You can find the database owner set in the login screen, which represents the schema on which all the tables are created. In Informix, the schema corresponds with the user that created the tables.
-   **Language folder**: You can find the value representing the default language in the application. It can be changed in the Configuration tab.
-   **Trace folder**: You can find all the settings about the trace level set in the application. It contains a trace level for the application, a trace level for the ORM (the mechanism responsible for connecting to the database), and a trace level for the view.

## 4. How it works

This chapter describes how A+W Customizing Manager works by an example.

### 4.1 Configure Master Data

In the **Master Data** tab, you configure Sites and their Environments. An Environment is allocated to one of our A+W products: A+W Business, A+W Enterprise, or A+W Production. For each environment, the user must define whether it is a Live or Test Environment.

Parameters can be set for each environment, which are UNC paths to different categories of files: Reports, Scripts, and Configuration or database. The Windows user must have access to this UNC path. This is a base path; subfolders can be defined later during object configuration.

**Example Setup:**

1.  Open the **Master Data** Tab and click **Site new** to enter a new Site, e.g., "A+W Germany" with Site ID 1.
2.  With the new site selected, click **Environment new** to add a new A+W Production live Environment named “Production Germany”.
3.  Set the **Product** to "A+W Business" and check the **Live Environment** box.
4.  With the new environment selected, click **Path new** to add a new Path Category. For example, select "Configuration" and define the UNC Path (e.g., `C:\ProgramData\A+W`).
5.  Repeat these steps to add a Test Environment “Production Germany Test” and a second Site “A+W France” with a Test and Live Environment.
6.  For every environment, you can also add a database connection by selecting the environment and clicking **Database connection new**. You will need to enter the connection string data for that specific database.

### 4.2 Configure Objects

In the **Objects** tab, all objects (files) to be managed by the A+W Customizing Manager are handled. Currently, an object is a file from one of the existing categories like Report, Configuration, or Script. In the future, database objects like Functions and Stored Procedures will also be handled.

**Example: Adding a Report Object**

1.  In the **Objects** tab, click **New** in the "Object" group to add a new object. A file open dialog will appear.
2.  Navigate to the folder where the report is stored and select the file (e.g., `IG_ProductionList.rpt`).

**Configure the new object:**

1.  **Set Product**: "A+W Production".
2.  **Set Category**: "Report".
3.  **Filename**: This is pre-filled from the selected file. Change it if the filename in the target environments is different.
4.  **Sub Folder**: If the file is stored in a subfolder at the target location, enter the subfolder name here.
5.  **Description**: Add a description for the object for management purposes within the tool.
6.  **File Info**: Add information for the loaded file. This is preset with the filename but can be changed. This is used to manage different versions of an object's file.
7.  **Assign Sites**: In the "Assigned Sites" panel, move the sites where this object exists (e.g., A+W Germany, A+W France) from "Available Sites" to "Assigned Sites". The object will be assigned to all “A+W Production” environments in the selected sites.

The new object has one file, which is marked as a **test file** (indicated by a file symbol with a gear). If the object is published, this file will be published to the “A+W Production” test environments of the assigned sites.

**File Versioning and Management:**

-   **Release a Test File**: To use a file in live environments, select the test file in the "File List" and click **Release Test File**. The file is copied, and its symbol changes to a green checkmark.
-   **Add a New Test File**: To add a new version or draft of a file, click **New Test File**. Select the new file. The existing test file is automatically moved to "archived". The new test file gets its own information and version, which can be edited.
-   **Copy as Test File**: A selected archive or release file can be copied to become the current test file by clicking **Copy into Test File**. If this happens, the actual test file will be moved into the archive.
-   **Delete a File**: Select a file in the "File List" and click **Delete File**.
-   **Edit File Info**: Select a file and click **Edit File** to change its information.
-   **Export a File**: Select a file and click **Export File** to save its content to your local file system.

> **Note**: If you try to add a new test file or release a test file and the source and target files have the same content, the action will be blocked, and a message will be displayed.
> The last column in the file list shows a file symbol indicating if the file has content. An empty file symbol means an empty file was loaded.

### 4.3 Publish Objects

The **Publication** tab is used to copy new versions of test or live files to the target sites.

**Publishing Workflow:**

1.  **Select Scope**:
    -   Select the environment type (Live or Test).
    -   Select the product (A+W Production, A+W Business, A+W Enterprise).
    -   Select the category type (Report, Configuration, Script).

2.  **Select Items to Publish**:
    -   Two lists will appear: one with all possible Environments and one with all allocated Objects matching the selected scope.
    -   By default, all records in both lists are checked. You can uncheck any environment or object you do not want to include in the publication.
    -   Objects marked in grey are not allocated to all environments in the list. Objects in black are allocated to all of them.
    -   You can filter the object list by Filename, Sub Folder, and Description.

3.  **Check Publication**:
    -   Once you have selected the environments and objects, click **Check**.
    -   The A+W Customizing Manager simulates the publication and displays the results in the "Result" list below. This will show potential warnings, such as "File doesn't exist in target directory."
    -   If an object cannot be published because an environment doesn't have the specified category configured, it will be skipped.

4.  **Execute Publication**:
    -   If the result list has no errors, you can proceed.
    -   Enter a **Publication Description** (e.g., "Publication of Purchase Order 23").
    -   Click **Execution**.
    -   The files are copied to the target environments.
    -   If a target file already exists but is not tracked as a version within the Customizing Manager, it will be backed up as an archive before being overwritten.
    -   The Customizing Manager will not overwrite a target file if the publishing file has the same content.
    -   A message will appear when the task is finished, showing how many files succeeded, failed, or were skipped.

5.  **Export Results**: The results of the publication can be exported to a CSV file using the **Export to CSV** button.

## 5. DB2 and Informix

You, or the customer's IT, need to define a listener for the DRDA protocol. This is done through corresponding entries in the following files:

-   **`$INFORMIXDIR/etc/$ONCONFIG`**:
    ```
    DBSERVERALIASES [<other_aliases>,]<drda_ifxserver>
    ```

-   **`$INFORMIXSQLHOSTS`**:
    ```
    <drda_ifxserver> drsoctcp *<server_hostname> <drda_service>
    ```

-   **`/etc/services`**:
    ```
    <drda_service> <drda_portnum>/tcp
    ```

The database instance needs to be restarted to activate the newly configured listener.
