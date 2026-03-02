---
description: "EN-INST-AW_Enterprise_FinAc_Service"
---


# Installation Instructions: A+W Enterprise 6 FinAc Service

**Software for Glass and Windows**

## Change History

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 16.04.22 | MP | New creation | 1.0 |
| 16.10.04 | SVH | Addition | 1.1 |
| 16.12.13 | MP | AutoUpdate | 1.2 |
| 17.03.21 | SVH | Additions/changes AWDesk #379226 | |
| 18.11.23 | SVH | Additions AWDesk #425206 | |
| 2021-12-16 | SVH | Addition [AW-84955], modifications | |
| 2022-06-13 | SVH | Additions to Intrastat | |

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

## Content

*   **1. Installation of the A+W Enterprise 6 FinAc Service**
    *   1.1 Overview and the basics
    *   1.2 Time requirement
        *   1.2.1 Installation time for the software
    *   1.3 Requirements
        *   1.3.1 Windows Server Version
        *   1.3.2 Network
        *   1.3.3 Software
    *   1.4 Procedure
    *   1.5 Customer-specific configurations
        *   1.5.1 Open Amounts Import Settings
        *   1.5.2 Ongoing Orders Export Settings
        *   1.5.3 Customer-specific settings (account information)
        *   1.5.4 Stock Movements Export Settings
    *   1.6 Incompatibilities
    *   1.7 Directory structure
    *   1.8 Result of the installation
    *   1.9 Configuration
    *   1.10 Tips and tricks
        *   1.10.1 AutoUpdate
        *   1.10.2 Known errors and workarounds
    *   1.11 Uninstalling

## 1. Installation of the A+W Enterprise 6 FinAc Service

The following installation instructions assume that there is no previous version installed.

The update of an earlier release version of the A+W Enterprise 6 FinAc Service is performed exactly as a new installation.

The update of an earlier version of the FinAc Service, e.g. A+W Enterprise FinAc Service to A+W Enterprise 6 FinAc Service is not possible. There should always only be one version of the FinAc Service installed.

This document describes only the installation and configuration of A+W Enterprise 6 FinAc Services. In case of questions about the installation or configuration of dependent set-ups/disk sets, please see the installation instructions for these products.

### 1.1 Overview and the basics

The following list provides and overview of the work that must be done during installation:

*   Installation and configuration of the Informix driver via `setnet32.exe`.
*   Creation of the necessary set-ups/disk sets:
    *   A+W Enterprise 6 FinAc Service
    *   A+W Infrastructure 6 Collector Services
    *   A+W Infrastructure 6 Middleware
    *   Java 7 Update 51
    *   A+W Setup Launcher
*   Installation of the FinAc Service and dependent disksets with the Setup Launcher.
*   Configuration of the FinAc Service with the Config Tool.

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:

*   **Processor**: 3000 Mhz
*   **RAM**: 4 GB
*   **Other**: /

For an initial or new installation, an installation time of 5 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

### 1.3 Requirements

#### 1.3.1 Windows Server Version

Supported operating systems:
*   Windows 2008 Server R2 32/64bit.
*   Windows 2012 Server R2 32/64bit.

#### 1.3.2 Network

For the installation itself, no network access is necessary. For the operation of the service, there must be a connection to the A+W Enterprise DB Server and the company network. The service user used must have sufficient access rights also to network resources used.

#### 1.3.3 Software

It is assumed that the following disk sets were already installed and configured BEFORE the installation of the A+W Enterprise 6 FinAc Service disk set.
*   Informix Client SDK 3.5 TC9 (or newer)
*   Microsoft .NET Framework 4.5.1 SDK

### 1.4 Procedure

For the installation, please proceed in the following sequence:

1.  Use `setnet32.exe` to configure the database server and hosts. This assumes that an IBM Informix Client SDK was installed (see software requirements).
2.  Installation of the A+W Enterprise 6 FinAc Service with the Setup Launcher.
    On the Component Selection dialog on the A+W Enterprise node, select the "A+W Enterprise 6 FinAc Service" module. This automatically selects all dependent set-ups.

    **A+W SetupLauncher - Component Selection**

    *   A+W Business
    *   A+W Common
    *   **A+W Enterprise**
        *   A+W Enterprise 6 B2B Service
        *   A+W Enterprise 6 BMECat Import
        *   A+W Enterprise 6 CAD Service
        *   A+W Enterprise 6 Export Service
        *   [x] **A+W Enterprise 6 FinAc Service**
        *   A+W Enterprise 6 Frontend
        *   A+W Enterprise 6 OrderXML Service
        *   A+W Enterprise 6 Print Service
        *   A+W Enterprise 6 Web
    *   A+W Production
    *   External Software

    > **Details for A+W Enterprise 6 FinAc Service:**
    > Interface for financial account systems. Install on: Process Server.
    > Version: 13.0.3795.0
    > Folder: `\\jupiter\SW_Develop\v13.0\Diskset\A+W Enterprise 6 FinAc Service`

3.  After the successful installation, the FinAc Service is configured with the Config Tool.

### Configuration with the Config Tool

#### Common Settings

This section covers the general settings for the service.

*   **Polling Interval (Minutes)**: Time interval in minutes in which the FinAcService checks the transfer table `fibutransfer`.
    *   "Rush" transfer records (status -1) will be processed at the next polling time.
    *   "Normal" records (status 0) will be processed only at the "Start time".
    *   "Urgent" records can only be generated by calling a corresponding script in the individual programs. The update urgent scripts are made available by A+W.
    *   Default value: 15 minutes. Maximum: 1440 minutes (= once a day).
*   **FinAc Interface**: Various FinAc Interface types are available. The correct setting is determined customer individually after consultation with Development. (Example: `eGecko_1_0_001`)
*   **Transfer Type**:
    *   **No Transfer**: No data transfer. The XML files generated remain in the directory that was specified in the XML Export Path field. The files are also not deleted if the 'Delete XML files' option was not set.
    *   **Copy to network path**: Activates the transfer of XML files within a company network. Additional settings are necessary. See File Transfer Settings.
    *   **FTP upload**: Activates the transfer of XML files on an FTP server. Additional settings are necessary. See FTP Settings.
    *   Default value: No Transfer.
*   **Intrastat Interface**: Various Intrastat Interface types are available. The correct setting is determined customer-specifically after consultation with Development. (Example: `Intrastat_6.3.1_DE_001`)
*   **Lock Limit (records)**: A record limit can be specified, starting from which the table `intrastat` is locked exclusively for the Intrastat processing. The limit only applies if the "Exclusive Table Lock" checkbox in the "Site Properties" is activated. (Example: `1000`)

##### Protocol Button

With the Protocol button, you can reach the Protocol Configuration dialog. This automatically selects all dependent set-ups. On the first tab, the trace categories for the frontend are configured; on the following tabs, the tracing of dependent modules and programs can be activated if necessary.

The following trace levels are distinguished:
*   Fatal
*   Error
*   Warning
*   Info
*   Debug

If, for example, the Info level is active, trace messages of the type Error and Warning will also be written into the tracing file.

The tracing file is always in the directory `%ProgramData%\A+W\Log`. The file name consists of the service name, the current date and the process number and ends with `.awtrc`.

The A+W Enterprise FinAc Service currently uses no log protocol.

#### Document Export Settings

On this dialog, the settings for the FinAc document export are made.

*   **Export Documents**: Check box that activates the document export.
*   **Use Site Folders**: Check box that activates company-specific subdirectories.
*   **Start Time (hh:mm)**: Start time of the regular FINAC transfer. At this time, all data records of the table `fibutransfer` are processed, which are in the table with status 0 (or -1). The specification of the time is done in 24-hour format. (Example: `00:00`)
*   **Rerun Interval (h)**: Specification of the repetition interval in hours and how many times the run should be repeated.
*   **Export Root Path**: File path in which all XML files generated are stored before they are transferred by the transfer logic. If "Use Site Folders" is active, the files are stored in company-specific subdirectories. (Example: `C:\Temp`)

#### Intrastat Export Settings

On this dialog, the settings for the Intrastat document export are made.

*   **Export Intrastat**: Checkbox that activates the Intrastat export.
*   **Use Site Folders**: Check box that activates company-specific subdirectories.
*   **Export Root Path**: File path in which all XML files generated are stored before they are transferred by the transfer logic. If "Use Site Folders" is active, the files are stored in company-specific subdirectories.
*   **Clean Up Time (days)**: All back-up records for the table `intrastatok` are removed from the table as soon as they are older than the time period specified here in days. (Example: `100`)
*   **Daily Export**:
    *   **Daily Export Checkbox**: Activates the daily export.
    *   **Daily Issue Checkbox**: Activates the daily checking of Intrastat data available for export.
    *   **Start Time (hh:mm)**: Start time of the daily Intrastat-xml file generation. At this time, all data records of the table `intrastat` are processed, which are in the table with status 0 (or -1). The time is specified in 24-hour format.
    *   **Rerun Interval (h)**: Specification of the repetition interval in hours and how many times the run should be repeated.
*   **Monthly (Closed Months Only) Export**:
    *   **Monthly Export Checkbox**: Activates the monthly export.
    *   **Start Day (d)**: Day of the month on which the monthly Intrastat-xml file generation should start.
    *   **Start Time (hh:mm)**: Start time of the monthly Intrastat-xml file generation. At this time, all data records of the table `intrastat` are processed, which have a status of 0 (or -1). The time is specified in 24-hour format.

#### Database Settings

On this dialog, all database-precise settings are configured, starting with the database itself. You can manage configurations using the following buttons:
*   **New**: Create a new configuration.
*   **Edit**: Edit an existing configuration.
*   **Delete**: Delete an existing configuration.
*   **De-/Activate**: Activate or deactivate the selected configuration.
*   **Copy**: Copy an existing configuration.

##### Site Properties

With the `New` or `Edit` buttons or with a double-click on a row in the table, you reach the Site Properties dialog. Here, all database-dependent settings can be made.

*   **Site Settings**
    *   **Active Connection**: Checkbox to activate the DB connection.
    *   **AWE Site**: The site number of the AWE site. See `xhaus.hnr`. (Example: `140`)
*   **FinAc Interface Settings**
    *   **FinAc Site**: The FinAc site number assigned to this site. (Example: `901`)
    *   **FinAc Interface**: The designation of the FinAc interface. (Example: `eGecko`)
    *   **FinAc Interface Version**: The client-specific version of the FinAc interface. (Example: `eGecko_1_0_001`)
*   **Intrastat Interface Settings**
    *   **Intrastat Export**: Checkbox to activate the Intrastat export.
    *   **Test**: Checkbox to run Intrastat export in test mode.
    *   **Exclusive Table Lock**: Activates the exclusive locking of the table `intrastat` during processing. Applies only starting from the Lock Limit.
    *   **Lock Limit (records)**: Specifies the lower limit. Starting with this number of records, the table `intrastat` is locked exclusively. The value is taken from "Common Settings" but can be adjusted DB-specifically here.
    *   **Intrastat Interface Version**: The client-specific version of the Intrastat interface.
*   **Database Settings**
    *   **Server Name**: The database server. Via the combo box, all DB servers entered in `setnet32` can be selected.
    *   **User**: A user name that has access to the database.
    *   **Password/Confirm Password**: The password for the user.
    *   **Database Name**: If Server Name, User, and Password are valid, this combo box contains all available database names.
    *   **Client Locale / DB Locale**: The appropriate locale settings. The combo boxes contain most common values, but manual entry is possible.
    *   **SQL Explain**: Checkbox to activate the database log.
*   **DB Functions**
    *   **Start Setnet32**: Button to start the `setnet32.exe` program to configure database servers/hosts.
    *   **Check Alenv**: Checks the A+W Enterprise environment variables for this service and views the current database configuration.
    *   **Test Connection**: Button to check the current database configuration values. A success message ("Database Connection established") or an error message is displayed.

#### Subsite Settings

On this dialog, all subsites of a multisite system can be entered. The subsites can optionally be entered in the "Database Settings." The difference is that in the "Database Settings" for each subsite, the DB connection must be entered. In the "Subsite Settings," the DB connection is referenced via the entry in "AWE Main Site." Therefore, there must only be an entry in "Database Settings" for the main site.

*   **Active Site**: This checkbox marks whether the specified subsite is active. Active subsites are processed by the FinAc service, inactive ones are not.
*   **AWE Main Site**: Number of the main site via which the DB connection is referenced.
*   **AWE Subsite**: Number of the subsite.
*   **FinAc Site**: Number of the FINAC sites assigned to the subsites.

#### File Transfer Settings

If in the **Transfer Type** switch the point `Copy to network path` was selected, the File Transfer Settings dialog appears.
*   **Base Path**: The path where defined directories will be created and XML files will be copied. The path must be reachable from the server on which the FinAc Service is installed. Write permissions have to be set up for the Service user.

#### FTP Settings

If in the **Transfer Type** switch the point `FTP upload` has been selected, the dialog FTP Settings appears. There are fields here to establish a connection to an existing FTP server.

*   **FTP Server**: The address of the FTP server without the specification "ftp://".
*   **FTP User**: The login name of the FTP user.
*   **FTP Password + Confirm Password**: The password of the FTP user.
*   **FTP Base Path**: The defined directories are created below the base path; the XML files are copied to these. Write permissions have to be set up for the FTP user.
*   **Max. Attempts**: The maximum number of attempts to upload a file to the FTP server before the process is terminated. Default value: 1. Maximum: 100.

#### Maintenance Settings

The maintenance functions of the FinAc Service are configured in the Maintenance Settings dialog.

*   **Archive Transfer Data**: It can be set as to whether processed records of the table `fibutransfer` should be deleted or whether they should remain in the table for research purposes.
    *   Default value: Move transfer data to `ok*`-table.
*   **Clean Up Time (days)**: All successfully processed records of the `fibutransfer` table are removed from the table as soon as they are older than the time interval set here.
    *   Default value: 90 days. Maximum: 360 days.
*   **Delete XML Files**: You can also select for generated XML files whether they are deleted after successful transfer or whether they should remain. If the transfer type "No transfer" was selected, the XML files are not deleted automatically.
    *   Default value: Delete XML files after successful transfer.

#### Windows Service Configuration

The service users are stored on the Windows Service Configuration dialog. These are Windows users who are used to access external objects such as network paths, etc. This user must have the appropriate rights.

*   **Domain/User/Password**:
    *   With the **Pick user...** button, it is possible to select a domain user.
    *   If no network domain is available (e.g., on a PC), use `.` for the domain.
    *   If no user is available, the service can also run under "LocalSystem" in case of emergency. This is the default services user in a Windows system. Leave the field empty to use "LocalSystem".
*   **Parallel Services**:
    *   **No. of Extra Services**: Set up the quantity of additional parallel services here in order to increase the processing speed. For this function, the computer on which the FinAc Service is running must have appropriate hardware (e.g. multi-core processor).

With a click on `Next`, the component registration for SN is executed. The Windows component manager is opened and then closed again. For this reason, it is recommended that you always let the Config Tool run through to the end.

4.  Now the A+W Enterprise 6 FinAc Service is ready and it writes a log into the directory named above.
5.  Setting of A+W Enterprise environment variables.

### 1.5 Customer-specific configurations

The information whether the respective functionality is available for the customer FinAc interface can be found in the customer-specific interface description.

#### 1.5.1 Open Amounts Import Settings

*   **Import Open Amounts**: check box, which activates the import of the open items.
*   **Start Time (hh:mm)**: First daily start time of the import. The specification of the time is done in 24-hour format.
*   **Rerun Interval (h)**: Specification of the repetition interval in hours and how many times run should be repeated.
*   **Import Root Path**: File path in which the import files should be searched for.

#### 1.5.2 Ongoing Orders Export Settings

*   **Export Ongoing Orders**: Check box that activates the export of the open orders.
*   **Start Time (hh:mm)**: First daily start time of the export. The specification of the time is done in 24-hour format.
*   **Rerun Interval (h)**: Specification of the repetition interval in hours and how many times run should be repeated.
*   **Export Root Path**: File path in which all export files generated are stored. The files are stored in company-specific subdirectories.

#### 1.5.3 Customer-specific settings (account information)

*   **Basis Account**
*   **Department Account**

#### 1.5.4 Stock Movements Export Settings

*   **Export Stock Movem.**: Checkbox that activates the export of the incoming and outgoing stock transactions.
*   **Start Time (hh:mm)**: First daily start time of the export. The specification of the time is done in 24-hour format.
*   **Rerun Interval (h)**: Specification of the repetition interval in hours and how many times run should be repeated.
*   **Export Root Path**: File path in which all export files generated are stored.

### 1.6 Incompatibilities

No incompatibilities are known.

### 1.7 Directory structure

(No specific directory structure is detailed in this section.)

### 1.8 Result of the installation

If the service could be started, the installation was successful. Otherwise, the trace log is available for determining possible problems.

### 1.9 Configuration

For additional configurations, please see the FinAc Service documentation.

### 1.10 Tips and tricks

#### 1.10.1 AutoUpdate

In order to be able to install the service via AutoUpdate, the setup must have been installed successfully at least once with the Setup Launcher and configured with the ConfigTool.

#### 1.10.2 Known errors and workarounds

(No known errors or workarounds are listed.)

### 1.11 Uninstalling

You can uninstall the program as usual via **Control Panel -> Programs and Functions**.

> **Programs and Features Dialog**
>
> Möchten Sie A+W Enterprise 6 FinAc Service wirklich deinstallieren?
> (Do you really want to uninstall A+W Enterprise 6 FinAc Service?)
> [ ] Diesen Dialog nicht mehr anzeigen (Do not show this dialog again)
>
> [ Ja ] [ Nein ]

**Note**: The config file is not deleted automatically. For a final uninstallation, the program directory of the A+W Enterprise 6 FinAc Service must be deleted manually.