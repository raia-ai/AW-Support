---
description: "EN-INST-AW_Enterprise_B2B_Service"
---


# Installation Instructions: A+W Enterprise 6 B2B Service

---
## Change History

| Date       | Edited by | Remarks                                           | Version |
|------------|-----------|---------------------------------------------------|---------|
| 2016-04-22 | MP        | New creation                                      | 1.0     |
| 2016-09-29 | SVH       | Addition                                          | 1.1     |
| 2016-12-13 | MP        | AutoUpdate                                        | 1.2     |
| 2017-05-04 | MP        | Multi database configuration                      | 1.3     |
| 2017-05-10 | SVH       | Configuration of openTRANS export                 |         |
| 2018-06-06 | SVH       | Configuration Hornbach export / Mail dispatch     |         |
| 2020-05-12 | SVH       | Configuration A+W EDI Export (AWDesk #422752)     |         |
| 2023-09-01 | SVH       | Maintenance Settings                              |         |
| 2024-06-25 | SVH       | [AW-111997] – e-invoicing                         |         |

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## 1. Installation of A+W Enterprise 6 B2B Service

The following installation instructions assume that there is no previous version installed.

An update of an earlier release version of the A+W Enterprise 6 B2B Service is executed precisely like a new installation.

An update of an earlier version of the B2B Service, e.g. from ALCIB 2011 B2B Service to A+W Enterprise 6 B2B Service is not possible. Only one version of the B2B Service should be installed.

This document describes only the installation and configuration of the A+W Enterprise 6 B2B Service. In case of questions about the installation or configuration of dependent set-ups/disk sets, please see the installation instructions for these products.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:

-   Installation and configuration of the Informix driver via `setnet32.exe`
-   Creation of the necessary set-ups/disk sets
    -   A+W Enterprise 6 B2B Service
    -   A+W Infrastructure 6 Collector Services
    -   A+W Infrastructure 6 Middleware
    -   Java 7 Update 51
    -   A+W Setup Launcher
-   Installation of the B2B Service and the dependent disk sets with the Setup Launcher
-   Configuration of the B2B Service with the Config Tool

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
-   Processor: 3000 Mhz
-   RAM: 4 GB
-   Other: /

For an initial or new installation, an installation time of 5 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

### 1.3 Requirements

#### 1.3.1 Windows Server Version

Supported operating systems:
-   Windows 2008 Server R2 32/64bit.
-   Windows 2012 Server R2 32/64bit.

#### 1.3.2 Network

For the installation itself, no network access is necessary.
For the operation of the service, there must be a connection to the A+W Enterprise DB Server and the company network.

#### 1.3.3 Software

It is assumed that the following disk sets were already installed and configured BEFORE the installation of the A+W Enterprise 6 B2B Service disk set.

-   Informix Client SDK 3.5 TC9 (or newer)
-   Microsoft .NET Framework 4.5.1 SDK

For the operation of the A+W Enterprise 6 B2B Service, access to an installed A+W ERP Web Service 6 is required. This must absolutely be installed on the same computer as the B2B Service.

-   A+W ERP Web Service 6

### 1.4 Procedure

For the installation, please proceed in the following sequence:

1.  Use `setnet32.exe` to configure the database server and hosts. This assumes that an IBM Informix Client SDK was installed (see software requirements).
2.  Installation of the A+W Enterprise 6 B2B Service with the Setup Launcher.
    On the **Component Selection** dialog on the A+W Enterprise node, select the "A+W Enterprise 6 B2B Service" module. This automatically selects all dependent set-ups.
    
    *(Image of A+W SetupLauncher Component Selection dialog, showing "A+W Enterprise 6 B2B Service" selected.)*

3.  After the successful installation, the B2B Service is configured with the Config Tool.

---

## 2. Configuration with the Config Tool

### 2.1 Common Settings

This is the first dialog in the configuration process.

*(Image of A+W Enterprise 6 B2B Service Configuration - Common Settings dialog)*

#### 2.1.1 Polling Interval

In the **Polling Interval (Seconds)** field, set the number of seconds that the service waits before it checks the `ottransfer` transfer table again for new data records. The default value is 60 seconds.

#### 2.1.2 Internal Invoice/Dispatch Transfer

If this checkbox is active, the B2B Service processes `ottransfer` entries with interface = `INVOIC` or `DELIVE`. (This handles the logic of internal calculation, and creation of INVOICE and DISPATCHNOTIFICATION documents in AW extended openTRANS format).

#### 2.1.3 Dorma Orders

If this checkbox is active, the B2B service processes `ottransfer` entries with interface = `INVOIC` (for Dorma P.O.).

#### 2.1.4 openTRANS Document Export

If this checkbox is active, the B2B Service processes the `ottransfer` entries with = `OTDOC` (user-specific export of openTRANS documents).

#### 2.1.5 A+W EDI Export (P.O. export)

If this checkbox is active, the B2B Service processes `ottransfer` entries with interface = `EDIEXP` (A+W standard export).

#### 2.1.6 Export of E-Invoice

If this checkbox is active, the B2B Service processes `ottransfer` entries with interface = `E-INV` (export of electronic invoices).

#### 2.1.7 Protocol-Button

With the **Protocol** button, you can open the **Protocol Configuration** dialog. This automatically selects all dependent set-ups. On the first tab, the trace categories for the frontend are configured; on the following tabs, the tracing of dependent modules and programs can be activated if necessary.

*(Image of Protocol Configuration dialog)*

The following trace levels are distinguished:
-   Fatal
-   Error
-   Warning
-   Info
-   Debug

If, for example, the **Info** level is active, trace messages of the type **Error** and **Warning** will also be written into the tracing file.

The tracing file is always in the directory `%ProgramData%\A+W\Log`. The file name consists of the service name, the current date, and the process number, and ends with `.awtrc`.

The A+W Enterprise B2B Service currently uses no log protocol.

### 2.2 ERP Webservice Settings

This dialog only opens if at least one of the **Internal Invoice/Dispatch Transfer** or **Dorma Orders** checkboxes were activated in the Common Settings.

*(Image of ERP Webservice Settings dialog)*

#### 2.2.1 ERP Web Service URL

Enter the URL for the ERP Web Service.

#### 2.2.2 Export Path

Enter the Root path in which the exported openTRANS xml files are saved. The internal logic completes the directory `<site number>` and `<customer number>` in the path specified here.

The exported file is saved with the name: `openTRANS_<process type>_<site number>_<customer number>_<process number>_<process sub-number>.xml`

**Example:**
If the file export path `D:\openTRANS` is entered in the Config tool, the created openTRANS invoice file of invoice 776655 for customer 1234 in site 10 is saved in:
`D:\openTRANS\10\1234\openTRANS_INVOICE_10_1234_776655_0.xml`

If errors occur during the creation of the export file, the records remain in the table `ottransfer` with an error flag. The A+W Enterprise B2B Service currently uses no log protocol. If for some reason the file generation for a transaction is started again even though a file has already been generated, the existing file is overwritten by the newly-generated one.

### 2.3 Cantor Export – openTRANS 2.1 Settings

This dialog only opens if the **openTRANS Document Export** checkbox was activated in the Common Settings.

*(Image of Cantor Export - openTRANS 2.1 Settings dialog)*

#### 2.3.1 Active

The checkbox enables the export.

#### 2.3.2 Export Root Path

Enter here the basic path in which the export files are saved. Below this basic path, the B2B Service automatically creates sub-directories for site numbers and customer numbers in which the export files are saved.

### 2.4 Hornbach export – openTRANS 2.1 settings

This dialog only opens if the **openTRANS Document Export** checkbox was activated in the Common Settings.

*(Image of Hornbach Export - openTRANS 2.1 Settings dialog)*

#### 2.4.1 Active

The checkbox enables the export.

#### 2.4.2 Export Root Path

Enter here the basic path in which the export files are saved. Below this basic path, the B2B Service automatically creates sub-directories for site numbers and customer numbers in which the export files are saved.

### 2.5 A+W EDI Export Settings

This dialog only opens if the **A+W EDI Export** checkbox was activated in the Common Settings.

*(Image of A+W EDI Export Settings dialog)*

#### 2.5.1 Active

The checkbox enables the export.

#### 2.5.2 Export Root Path

Enter here the basic path in which the export files are saved. Below this basic path, the B2B Service automatically creates sub-directories for site numbers and supplier numbers in which the export files are saved.

This configuration can be overridden by a supplier-specific configuration in A+W Enterprise. For a detailed description of overriding, see the configuration document "A+W Enterprise EDI."

### 2.6 E-Invoice Export Settings

This dialog only opens if the **E-Invoice Export** checkbox was activated in the Common Settings.

*(Image of E-Invoice Export Settings dialog)*

#### 2.6.1 Active

The checkbox enables the export.

#### 2.6.2 Export Root Path

Enter here the basic path in which the export files are saved. The path is only used if the export files were generated manually. For a detailed description, see the B2B Service configuration instructions.

### 2.7 Database settings

On this dialog, all database-precise settings are configured, starting with the database itself.

*(Image of Database Settings list view dialog)*

-   With the **New** button, you can create a new configuration.
-   With the **Edit** button, you can edit an existing configuration.
-   With the **Copy** button, you can copy an existing configuration.
-   With the **Delete** button, you can delete an existing configuration.

#### 2.7.1 Site Properties

With the **New** or **Edit** buttons or with a double-click on a row in the table, you reach the **Site Properties** dialog. Here, all database-dependent settings can be made.

*(Image of Database Settings (Site Properties) dialog)*

-   **Site Settings**
    -   **Active Connection**: Check to enable this database connection.
    -   **AWE Site**: The site number.
-   **Database Settings**
    -   **Server Name**: The database server is entered in the Server Name field. Via the combo box, all DB servers entered in the `setnet32` can be selected.
    -   **User Name** and **Password**: Enter database credentials.
    -   **Database Name**: If the fields **Server Name**, **User Name**, and **Password** are filled with valid values, the **Database Name** combo box already contains all available database names of the database server.
    -   **Client Locale** and **DB Locale**: The appropriate locale settings are entered here. The combo boxes already contain most used values. If it is necessary to enter deviating values, this is also possible manually.
-   **DB Functions**
    -   **Start Setnet32**: It is possible to start the `setnet32.exe` program directly; with it, database server/hosts can be set up.
    -   **Check Alenv**: With Check Alenv you can check the A+W Enterprise environment variables for this service and view the current database configuration. This dialog is for checking purposes only. The settings of the Alenv variables are made in A+W Enterprise.
    -   **Test Connection**: Allows you to check the current values of the database configuration. If a database connection can be established with these values, you will see a "Database Connection established" message; otherwise, an error message is shown.

### 2.8 Maintenance Settings

On the **Maintenance Settings** dialog, it is configured when successfully processed transfer records from the archive table and incorrect records from the transfer table are deleted.

*(Image of Maintenance Settings dialog)*

-   **Clean Up Time Success (Days)**: number of days after which successfully processed records are deleted from the table `ottransferok`.
-   **Clean Up Time Error (Days)**: number of days after which records that encountered an error are deleted from the table `ottransfer`.

### 2.9 E-Mail Settings

Use the **E-Mail Settings** dialog to configure whether and to which recipients error messages can be sent via email.

*(Image of E-Mail Settings dialog)*

-   **SMTP Server**: The name of the SMTP server
-   **Port**: (optional) deviating SMTP port
-   **From**: Email address of the sender
-   **To**: Email address of the recipient. Several recipient addresses can be specified separated by semicolons.
-   **CC**: Email address of the CC recipient. Several recipient addresses can be specified separated by semicolons.
-   **Encoding**: Coding of E-mail. Default: `utf-8`.
-   **Enable SSL**: Activate SSL encryption (Y/N)
-   **Authentication**: Activate authentication (Y/N)
    -   **Account**: Domain account for the authentication
    -   **Password**: Password
    -   **Confirm password**: Confirmation of the password

### 2.10 Service Configuration

The service users are stored on the **Windows Service Configuration** dialog. These are Windows users who are used to access external objects such as network paths, etc. This user must have the appropriate rights.

*(Image of Windows Service Configuration dialog)*

-   With the **Pick user...** button, it is possible to select a domain user.
-   If no network domain is available (e.g., the service was installed on a PC), the value `.` can be entered in the **Domain** field.
-   If no user is available, the service can also run under "LocalSystem" in case of emergency. This is the default services user in a Windows system.

---

## 3. Post-Installation

4.  Now the A+W Enterprise 6 B2B Service is ready and it writes a log into the directory named above (`%ProgramData%\A+W\Log`).
5.  Setting of A+W Enterprise environment variables.

### 3.1 Incompatibilities

No incompatibilities are known.

### 3.2 Directory structure

(This section is not detailed in the document.)

### 3.3 Result of the installation

If the service could be started, the installation was successful. Otherwise, the trace log is available for determining possible problems.

### 3.4 Configuration

For additional configurations, please see the B2B Service documentation.

### 3.5 Tips and tricks

#### 3.5.1 AutoUpdate

In order to be able to install the service via AutoUpdate, the setup must have been installed successfully at least once with the Setup Launcher and configured with the ConfigTool.

#### 3.5.2 Known errors and workarounds

(This section is not detailed in the document.)

### 3.6 Uninstalling

You can uninstall the program as usual via **Control Panel -> Programs and Functions**.

*(Image of German uninstall prompt: "Möchten Sie A+W Enterprise 6 B2B Service wirklich deinstallieren?" - Do you really want to uninstall A+W Enterprise 6 B2B Service?)*

> **Note:** The config file is not deleted automatically. For a final uninstallation, the program directory of the A+W Enterprise B2B Service must be deleted manually.
