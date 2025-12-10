---
title: "EN-INST-AW_SLT"
source: "EN-INST-AW_SLT.pdf"
tags: ["A+W SLT", "Installation Guide", "Software Installation", "Firebird", "Network Mode", "Uninstallation", "Glass and Windows Software", "A+W Software"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides detailed installation instructions for the A+W SLT software, a tool for calculating technical values for glass and windows. It covers new installations, system requirements, setup procedures, configuration, and uninstallation steps."
long_description: "This is a comprehensive installation guide for the A+W SLT software, developed by A+W for the glass and windows industry. The document is intended for planners and system administrators responsible for deploying the software. It details the entire installation process, assuming no prior version is installed. Key topics include system requirements (hardware, network, and supported operating systems like Windows XP, 7, 8, Server 2008 R2, and 2012 R2), time estimates for installation, and a step-by-step procedural walkthrough. The guide covers both single workstation and network mode installations, explaining the necessary steps for sharing directories and installing the A+W SLT Network Driver for client access. It also describes the integrated installation of the Firebird 2.1 database. Post-installation configuration, such as licensing, user creation, and customer-specific settings, is also explained. Finally, the document provides instructions for completely uninstalling A+W SLT, Firebird, and the associated FBDriver from the system."
---

# Installation Instructions A+W SLT

---
## Change history:

| Date      | Edited by | Remarks                             | Version |
|-----------|-----------|-------------------------------------|---------|
| 13.11.07  | MP        | Original version                    | 0.9     |
| 15.06.17  | MP        | Information regarding Windows environment | 1.0     |
| 16.04.25  | MP        | Update                              | 1.1     |

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## Content

*   **Installation Instructions**
*   **A+W SLT**
*   **1 New Installation of the Version**
    *   1.1 Overview and the basics
    *   1.2 Time requirement
        *   1.2.1 Installation time for the software
    *   1.3 Requirements
        *   1.3.1 Hardware
        *   1.3.2 Network
        *   1.3.3 Software
    *   1.4 Procedure
    *   1.5 Settings
        *   1.5.1 Licensing
        *   1.5.2 Creating a New User
        *   1.5.3 Customer-specific configuration
    *   1.6 Result of the installation
    *   1.7 Installation alternatives
        *   1.7.1 Network Mode
    *   1.8 Uninstalling
        *   1.8.1 A+W SLT Uninstallation
        *   1.8.2 Firebird Uninstallation
        *   1.8.3 FBDriver Uninstallation

---

## 1. New Installation of the Version

The following installation instructions assume that there is no previous version installed.

The update of an earlier release version of the A+W SLT is performed exactly as a new installation.

A+W SLT can be operated in two modes, single workstation and network mode. These installation instructions describe both modes. For the network mode, the A+W SLT Network Driver is required. The differences between network and single workstation can be found in the chapter Installation alternatives (1.7.1).

A Firebird 2.1 database is installed with A+W SLT. Its setup is integrated in the A+W SLT setup.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:
-   Creation of the necessary set-ups
    -   A+W SLT
    -   If necessary, an A+W SLT network driver
-   Installation with the Setup Launcher
-   Licensing of the A+W SLT
-   User set up in A+W SLT
-   Release of program directory (network mode)

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
-   Processor: 3000 Mhz
-   RAM: 4 GB
-   Other: /

For an initial or new installation, an installation time of 20 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

### 1.3 Requirements

#### 1.3.1 Hardware
Up-to-date Windows computer or server.

#### 1.3.2 Network
For the installation itself, no network access is necessary.

To operate the A+W SLT in network mode, there has to be a connection to the A+W SLT main installation and the company network.

> **IMPORTANT!** The server on which A+W SLT is installed, must be in the same Windows domain in which the A+W Enterprise Frontend is installed. The server must be listed in the list of trusted computers.

#### 1.3.3 Software
Supported operating systems:
-   Windows XP
-   Windows 7
-   Windows 8
-   Windows Server 2008 R2
-   Windows Server 2012 R2

### 1.4 Procedure

For the installation, please proceed in the following sequence:

1.  **Installation of A+W SLT with the Setup Launcher**
    On the **Component Selection** dialog on the **External Software** node, select the **A+W SLT** module. Currently, there are no depending Setups.

2.  **Configuration of A+W SLT during setup**
    To proceed with installation, enable the checkbox "Ich habe die Lizenzvereinbarung gelesen und akzeptiere die Bedingungen" (I read the license agreement and accept the conditions).

3.  **Select Setup Type**
    When selecting the **A+W SLT Poweruser**, a desktop icon is created on the desktop. This is not the case for **A+W SLT Standardusers**. After selecting an option, click "Weiter" (Next).

4.  **Begin Installation**
    Confirm the following dialogs with "Proceed" until installation starts. No other settings are required.

5.  **Firebird Database Installation**
    The installation of the Firebird database starts automatically. In the License agreement dialog, select "Ich akzeptiere die Vereinbarung" (I accept the agreement). Confirm the following dialogs with "Proceed". No other configurations are required.

6.  **Complete Installation**
    After a successful installation of A+W SLT, a dialog will appear confirming completion. You can choose to start the application immediately.

### 1.5 Settings

#### 1.5.1 Licensing
Licensing is carried out under "Init Passwort". The license is ordered via the Contract department of A+W Software GmbH from Sommer Informatik GmbH.

#### 1.5.2 Creating a New User
The employees who are going to use A+W SLT have to be set up in A+W SLT.

Start A+W SLT and click the menu option "Bearbeiter" (User). Confirm login with "OK". No password is required.

In the next dialog, you will see an overview of employees that have been previously entered. On the right side, there are three icons to add new users and to edit or delete existing ones.

It is important that the A+W Enterprise login name is entered in the "Name" field, so that A+W Enterprise and A+W SLT can communicate with one another. When adding a new user, fill in the required fields (Kürzel, Vorname, Name).

#### 1.5.3 Customer-specific configuration
You can find the instructions for customer-specific configuration in the release notes for construction products regulations Part 2.

### 1.6 Result of the installation
The program files were unpacked under `C:\Program Files (x86)\Sommer Informatik GmbH\A+W SLT`.

An icon was stored on the desktop with which you can start A+W SLT.

### 1.7 Installation alternatives

#### 1.7.1 Network Mode
To access the A+W SLT program (A+WSLT.exe) the program directory `C:\Program Files (x86)\Sommer Informatik GmbH\A+W SLT` has to be released on the server.

1.  Select the program directory, right-click and select the item "Erweiterte Freigabe..." (Advanced Sharing...).
2.  In the properties dialog, click "Erweiterte Freigabe..." (Advanced Sharing...) again.
3.  In the next dialog, check "Diesen Ordner freigeben" (Share this folder). Set the share name (e.g., `AWSLT`, remove any blanks). Click on "Berechtigungen" (Permissions).
4.  In the authorizations ["Berechtigungen"], assign full access to the directory to the user "Jeder" (Everyone). Check "Vollzugriff" (Full control) under "Zulassen" (Allow).
5.  The A+W SLT Network Driver (FBTreiber) has to be installed on all client PCs that are to have access to the central A+W SLT. For this, please refer to the respective installation instructions.

### 1.8 Uninstalling
To uninstall the software, go to the Control Panel under "Programs and Features", select the entries "A+W SLT", "FBTreiber" and "Firebird" and execute the "Uninstall" option for each.

#### 1.8.1 A+W SLT Uninstallation
When the InstallAware wizard starts, select the "Deinstallieren" (Uninstall) option and click "Weiter" (Next). Proceed through the wizard to complete the uninstallation.

#### 1.8.2 Firebird Uninstallation
Confirm the prompt asking if you are sure you want to remove Firebird.

If prompted about removing a shared file (`Firebird2Control.cpl`), select the option "Ja, für Alle" (Yes to All).

#### 1.8.3 FBDriver Uninstallation
Confirm the prompt asking if you really want to uninstall FBTreiber by clicking "Ja" (Yes).

