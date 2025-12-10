---
description: "EN-INST-A+W Enterprise BMECat Import"
---


# Installation Instructions: A+W Enterprise 6 BMECat Import

---
## Change History

| Date      | Edited by | Remarks        | Version |
| :-------- | :-------- | :------------- | :------ |
| 16.04.22  | MP        | New creation   | 1.0     |
| 16.12.13  | MP        | AutoUpdate     | 1.1     |

## Introduction

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1. Check the installation requirements.
2. Compile the required data, additional programs, drivers, etc.
3. Note or determine the time required.

---

## 1. Installation of the A+W Enterprise 6 BMECat Import

The following installation instructions assume that there is no previous version installed.

An update of an earlier release version of the A+W Enterprise 6 BMECat Import is executed precisely like a new installation.

An update of an earlier version of the BMECat Import, e.g. from ALCIB 2011 BMECat Import to A+W Enterprise 6 BMECat Import is not possible. Only one version of the BMECat Import should be installed.

This document describes only the installation and configuration of the A+W Enterprise 6 BMECat Import. In case of questions about the installation or configuration of dependent set-ups/disk sets, please see the installation instructions for these products.

### 1.1 Overview and the Basics

The following list provides an overview of the work that must be done during installation:

- Installation and configuration of the Informix driver via `setnet32.exe`.
- Creation of the necessary set-ups/disk sets:
  - A+W Enterprise 6 BMECat Import
  - A+W Infrastructure 6 Collector Services
  - A+W Infrastructure 6 Middleware
  - Java 7 Update 51
  - A+W Setup Launcher
- Installation of the BMECat Import and the dependent disk sets with the Setup Launcher.
- Configuration of the BMECat Import with the ConfigTool.

### 1.2 Time Requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation Time for the Software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:

- **Processor:** 3000 Mhz
- **RAM:** 4 GB
- **Other:** /

For an initial or new installation, an installation time of 5 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

### 1.3 Requirements

#### 1.3.1 Windows Server Version

Supported operating systems:

- Windows 7, 8, 8.1 32/64bit
- Windows 2008 Server R2 32/64bit
- Windows 2012 Server R2 32/64bit

#### 1.3.2 Network

For the installation itself, no network access is necessary.

For the operation of the service, there must be a connection to the A+W Enterprise DB Server and the company network.

#### 1.3.3 Software

It is assumed that the following disk sets were already installed and configured BEFORE the installation of the A+W Enterprise 6 BMECat Import disk set.

- Informix Client SDK 3.5 TC9 (or newer)
- Microsoft .NET Framework 4.5.1 SDK

### 1.4 Installation and Configuration Procedure

For the installation, please proceed in the following sequence:

#### 1. Configure Database and Hosts

Use `setnet32.exe` to configure the database server and hosts. This assumes that an IBM Informix Client SDK was installed (see software requirements).

#### 2. Install with Setup Launcher

Installation of the A+W Enterprise 6 BMECat Import with the Setup Launcher.

On the **Component Selection** dialog on the A+W Enterprise node, select the "A+W Enterprise 6 BMECat Import" module. This automatically selects all dependent set-ups.

**Component Details:**
- **Name:** A+W Enterprise 6 BMECat Import
- **Description:** Loads article data from DORMA Web Service.
- **Install on:** Process Server, Terminal Server, Client Computer
- **Version:** 13.0.2526.0

#### 3. Configure with the Config Tool

After the successful installation, the BMECat Import is configured with the Config Tool.

##### Database Settings

In the **A+W Enterprise 6 BMECat Configuration** window, configure the following database settings:

- **Server Name**: The database server is entered here. Via the combo box, all DB servers entered in the `setnet32` can be selected.
- **User Name**: A user name that has access to the database must be entered.
- **Password / Confirm Password**: Enter the user's password.
- **Database Name**: If the fields Server Name, User Name, and Password are filled with valid values, this combo box already contains all available database names of the database server.
- **Client Locale / Database Locale**: The appropriate locale settings are entered here (e.g., `en_US.CP1252`). The combo boxes already contain most values used. If it is necessary to enter deviating values, this is also possible manually.
- **Start Setnet32 Button**: It is possible to start the `setnet32.exe` program directly; with it, database server/hosts can be set up.
- **Test Connection Button**: Allows you to check the current values of the database configuration. If a database connection can be established with these values, you will see a "Database Connection established" message; otherwise, an error message.

##### Protocol Configuration

With the **Protocol** button, you can reach the **Protocol Configuration** dialog. This automatically selects all dependent set-ups. On the first tab, the trace categories for the frontend are configured; on the following tabs, the tracing of dependent modules and programs can be activated if necessary.

- **Trace Levels**: The following trace levels are distinguished:
  - Fatal
  - Error
  - Warning
  - Info
  - Debug
- **Functionality**: If, for example, the Info level is active, trace messages of the type Error and Warning will also be written into the tracing file.
- **Log File Location**: The tracing file is always in the directory `%ProgramData%\A+W\Log`. The file name consists of the service name, the current date, and the process number and ends with `.awtrc`.

The A+W Enterprise BMECat Import currently uses no log protocol.

#### 4. Set A+W Enterprise Environment Variables
(This step is mentioned but not detailed in the document.)

---

## Post-Installation Information

### 1.5 Incompatibilities

No incompatibilities are known.

### 1.6 Directory Structure

(The document does not specify the directory structure.)

### 1.7 Result of the Installation

If the service could be started, the installation was successful. Otherwise, the trace log is available for determining possible problems.

### 1.8 Additional Configuration

For additional configurations, please see the BMECat Import documentation.

### 1.9 Tips and Tricks

#### 1.9.1 AutoUpdate

In order to be able to install the program via AutoUpdate, the setup must have been installed successfully at least once with the Setup Launcher and configured with the ConfigTool.

#### 1.9.2 Known Errors and Workarounds

(The document does not list any known errors or workarounds.)

### 1.10 Uninstalling

You can uninstall the program as usual via Control Panel -> Programs and Functions.

A confirmation dialog will appear:
> **Programme und Features**
>
> Möchten Sie A+W Enterprise 6 BMECat Import wirklich deinstallieren? (Do you really want to uninstall A+W Enterprise 6 BMECat Import?)
>
> [ ] Diesen Dialog nicht mehr anzeigen
>
> [ Ja ] [ Nein ]

**Note:** The config file is not deleted automatically. For a final uninstallation, the program directory of the A+W Enterprise 6 BMECat Import must be deleted manually.
