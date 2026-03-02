---
description: "EN-INST-AW_Plan_Editor"
---


# Installation Instructions: A+W Plan Editor

**Software for Glass and Windows**

---
## Change history:

| Date | Edited by | Comments | Version |
| :--- | :--- | :--- | :--- |
| 2014-07-23 | Michael Hartmann | Release 5.4 | 5.4 |

---

## Contents

*   **1 Overview and Basics**
    *   1.1 Requirements
        *   1.1.1 Hardware
        *   1.1.2 Network
        *   1.1.3 Software
        *   1.1.4 Database
*   **2 Installation**
    *   2.1 Directory Structure
    *   2.2 Settings
        *   2.2.1 A+W Plan Editor ConfigTool
        *   2.2.2 Parameters
        *   2.2.3 Registry
    *   2.3 Installation Result
    *   2.4 Alternative Installations
    *   2.5 Patches
    *   2.6 Uninstalling

---

## 1. Overview and Basics

### 1.1 Requirements

#### 1.1.1 Hardware
No special requirements.

#### 1.1.2 Network
A+W Plan Editor does not require a network.

#### 1.1.3 Software
For A+W Plan Editor, Microsoft Windows 7 is the minimum requirement. If it is to be run on a terminal server, Windows Server 2008 R2 is required.

Please also remember to install all other available service packs for the framework and the operating system. We recommend to always keep the server up to date with the Microsoft Update Service.

The .NET Framework 3.5 SP1 is installed by A+W SetupLauncher. This installation takes about 30 minutes! If possible, please install .NET Framework in advance (or have it installed).

#### 1.1.4 Database
If you want to manually create patterns with A+W Plan Editor, certain master data (article and parameters) must be maintained in a database. The Microsoft Access 97 database that is required for this purpose is automatically installed by the setup.

---

## 2. Installation

Subsequently, please proceed in the following order during installation:

1.  Start the A+W Setup Launcher. Subsequently, the following splash screen opens:
    > **Welcome to the A+W SetupLauncher**
    > The wizard will help you to install ALBAT+WIRSAM software to your computer or your network.

2.  After you have confirmed the dialog by clicking "Next", the following new dialog opens for the selection of the diskset. Select "Create new diskset":
    > **Choose or create your installation diskset**
    > In the "Available Disksets" list, find and select the option "Create new diskset...".

3.  This is followed by a dialog in which the source and target directory can be entered:
    > **Setup Locations**
    > - **Source Directory**: [e.g., `\\jupiter\sw_install\2012\Diskset`]
    > - **Target Directory**: [e.g., `C:\Program Files (x86)`]
    > - **Operation System**: [e.g., `Windows 7 Enterprise 64 Bit Service Pack 1`]
    > - **Log Directory**: [e.g., `C:\Program Files (x86)\A+W\Installation Log`]

4.  Setup-Launcher now lists all components installed so far:
    > **Installed Components**
    > This screen shows a list of products already installed on the system, including their installed version, setup version, and last installation date.

5.  In the next dialog, select A+W Plan Editor from the components to be installed:
    > **Component Selection**
    > From the component tree, navigate to `A+W Production` and check the box for **A+W Plan Editor 5**.

6.  Now the software is being installed. The next screen confirms readiness:
    > **Setup has gathered all required data and is now ready to start the installation**
    > You can choose to:
    > - Install software
    > - Install software and save setup configuration to an XML file
    > - Only save setup configuration to an XML file

7.  The program has been successfully installed.

---

### 2.1 Directory Structure
By default, A+W Plan Editor is installed in folder `"C:\Programme\A+W\Techsoft\Planedit"`.

### 2.2 Settings

#### 2.2.1 A+W Plan Editor ConfigTool
In A+W Plan Editor Config Tool you can set the settings for protocolling. For this purpose, click on the Protocol button in the first dialog of the A+W Plan Editor Config Tool. The following dialog opens where you can set the protocolling settings:

> **Log Configuration**
> This dialog allows you to configure trace and log settings globally or per user.
>
> A+W Plan Editor only uses tracing, therefore the values in the "Trace Level" column must be set correspondingly.

In addition, you can use A+W Plan Editor Config Tool to select the language that should be used for the program interface:

> **A+W Plan Editor Config**
> - **Program Language**: Select the desired language (e.g., German) from the dropdown menu.

In the next dialog, which opens when you click "Next" in the first dialog of the A+W Plan Editor Config Tool, you can configure the path for the BLOCK file (in which the existing free shapes are saved). Usually, the correct path is already defined here after the installation.

> **A+W Plan Editor Config**
> - **Select path of BLOCK file**: The path is typically `C:\ProgramData\A+W\Techsoft\Xopt Planedit Shared\BLOCK`.

By clicking on the "Next" button, you will reach the last dialog of the A+W Plan Editor Config Tool in which you can configure the shape catalog that should be used by the program. Here, the correct value is also usually already defined.

> **A+W Plan Editor Config**
> - **Select Shape Catalog**: The appropriate catalog (e.g., A+W) should be pre-selected.

#### 2.2.2 Parameters
All program settings are saved in the registry. In order to configure any of these values, you must start the Settings Editor which has been installed by the setup in the program directory of A+W Plan Editor.

#### 2.2.3 Registry
(See 2.2.2 Parameters)

### 2.3 Installation Result
In the start menu under A+W, select the A+W Plan Editor shortcut and start the program.

### 2.4 Alternative Installations
Unknown.

### 2.5 Patches

| Designation | Description | Precondition |
| :--- | :--- | :--- |
| | | |

### 2.6 Uninstalling
To uninstall the software, select menu item "Software" in the Control Panel. Now A+W Plan Editor can be uninstalled in here.
