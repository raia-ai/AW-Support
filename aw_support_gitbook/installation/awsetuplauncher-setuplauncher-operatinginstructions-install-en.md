---
description: "EN-INST-AW_SetupLauncher"
---


# Operating instructions: A+W Setup Launcher

**Software for Glass and Windows**

---
## Change history:

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2008-01-06 | André Münch | Original version | 1.0.1000 |
| 2009-12-15 | André Münch | Auto Update | 1.0.1001 |
| 2010-01-05 | André Münch | Installation Directory | 1.0.1002 |
| 2010-05-28 | André Münch | Prerequisites amended | 1.0.1003 |
| 2011-07-21 | André Münch | Client AutoUpdate (1.7) added | 1.0.1004 |
| 2013-07-22 | André Münch | Inclusion of the 2012 server preparation | 1.0.1005 |
| 2013-10-08 | Jens Schmidt | Unsupervised installation | 1.0.1006 |
| 2017-01-24 | Jens Schmidt | Version 6.2 | 13.2 |
| 2017-12-01 | Jens Schmidt | RDSH role (3.1.1) | 13.5 |

## Content

- **1 New installation**
  - 1.1 Installation directory
  - 1.2 Overview and basics
  - 1.3 Definition of Terms
  - 1.4 Time Required
    - 1.4.1 Installation time for the software
    - 1.4.2 Conversion Time for Data Set
  - 1.5 Requirements
    - 1.5.1 Hardware
    - 1.5.2 Dongle
    - 1.5.3 Network
    - 1.5.4 Software
    - 1.5.5 Service user/Administrator rights
  - 1.6 Procedure
  - 1.7 AutoUpdate
    - 1.7.1 General Information
    - 1.7.2 Set-up
    - 1.7.3 Release
  - 1.8 Incompatibilities
  - 1.9 Diskset Directory Structure
  - 1.10 Manual settings
  - 1.11 Command line option and automatic mode
    - 1.11.1 Unsupervised initial installation
  - 1.12 Result of the installation
  - 1.13 Installation alternatives
  - 1.14 Patches
  - 1.15 Uninstalling
- **2 Update**
  - 2.1 Procedure
- **3 Preparing a Windows Server 2012 for A+W Software**
  - 3.1 ATTENTION!!!
  - 3.2 The Server Manager
    - 3.2.1 Roles
    - 3.2.2 Role services
    - 3.2.3 Features
    - 3.2.4 Server manager operation
  - 3.3 Adding Roles and Features
    - 3.3.1 Server roles
    - 3.3.2 Features
    - 3.3.3 Role services of the application server (Application Server)
    - 3.3.4 Web server role services
    - 3.3.5 Role services for the Remote Desktop Services
    - 3.3.6 Conclusion of the configuration
  - 3.4 Script-supported setup of the required Windows Features

## 1. New installation

The following installation instructions assume that there is no previous version installed.

### 1.1 Installation Directory

The following rules apply to the customer's installation directory:

- To create the installation directory, you can copy the entire release `\\jupiter\SW_INSTALL\v6` for a complete installation, and save it on the customer's system in a directory called `Software\A+W`. The Software directory should be configured as a release, all users should have reading rights.
- If just A+W Production or A+W Business shall be installed, you can use the two scripts `\\jupiter\SW_INSTALL\GetAWProduction6Complete.cmd` or `\\jupiter\SW_INSTALL\GetAWB6Complete.cmd` to create a local copy of the installation directory, and copy it to the customer's system.
- To speed up the installation, the customer can be provided beforehand with a directory which includes .NET Framework 4.5 and Service Pack 1 plus Windows Installer 3.1. These can be installed by the customer on the system before the actual installation. This directory can be created by means of the script `\\jupiter\SW_INSTALL\GetRequirements.cmd` in order to be passed on to the customer.

### 1.2 Overview and the basics

The following list provides an overview of the work that must be done during installation:
- Check all requirements (for Windows 2012 Server please stick to chapter 3)
- Installation of the Setup Launcher
- Run the Setup Launcher to install A+W software

### 1.3 Definition of Terms

**Diskset**: A diskset is the set of software packages to be installed, including their parameters.

### 1.4 Time Required

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.4.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
- **Processor:** Intel Pentium 4, 2.7 GHz, 1 GByte RAM
- **Storage space:** Approx. 10 MB of hard disk space is required
- **Miscellaneous**

For an initial or new installation, an installation time of 2 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

#### 1.4.2 Conversion Time for Data Set

None.

### 1.5 Requirements

#### 1.5.1 Hardware

None.

#### 1.5.2 Dongle

No dongle required.

#### 1.5.3 Network

When the A+W setup packages are available in the network, the directory must be released and the user of the Setup Launcher must be able to access it.

#### 1.5.4 Software

- .Net Framework 4.5 (will be downloaded and installed if it has not been installed already, and if there is a connection with the Internet or a Windows Update Server).
- The use of the automatic update via FTP requires Internet connection and access to the FTP Server.

#### 1.5.5 Service user/Administrator rights

Use of the Setup Launcher requires local administrator rights.

### 1.6 Procedure

1.  **Installing the Setup Launcher:**
    Execute `SetupStarter.exe` in the CD's main directory. After installation, the Setup Launcher will start automatically. Press "Next" to proceed.

    