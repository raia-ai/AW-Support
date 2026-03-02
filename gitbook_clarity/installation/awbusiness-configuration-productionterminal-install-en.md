---
description: "EN-INST-AW_Business_Production_Terminal_EL"
---


# Installation and Configuration Documentation: A+W Business Production Terminal (EL)

---
## Change history:

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2017-11-16 | MST | Original version | 0.1 |
| 2017-12-01 | PK | Corrections | 0.2 |
| 2018-06-25 | MST | Driver version Chapter Set-up 4.1.2 and function 5.2.3 | 0.3 |
| 2018-08-31 | MST | Release August 2018 6.1: Barcode and checksum 6.1.1, BOM tree with additional capacity planning parts 6.1.2, Read barcode 6.1.3 | 0.4 |
| 2019-03-12 | MST | Release March 2019 6.2: Short keys, Parameter settings, Delete block file entries | 0.5 |
| 2019-09-12 | MST | September Release 2019 Fehler! Verweisquelle konnte nicht gefunden werden. Setup provides all dependencies | 0.6 |
| 2020-04-22 | DNI | Barcoding - unique label identification per glass 6.4 | 0.7 |

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

## 1. Overview

The following description assumes that no version was previously installed and therefore that this is a new installation.

-   Follow this description exactly
-   Use the setups and configuration programs offered
-   Do not use programs such as XCOPY or REGEDIT. Please only use programs that the setup offers.

The following list offers an overview of which steps must be run through during and after the installation:

-   Requirements: Chapter 2
-   Installation: Chapter 3
-   Configuration: Chapter 4

## 2. Requirements

The following prerequisites must be implemented before installation.

### 2.1 Other program documents

The following documents offer a detailed description of steps that must be performed beforehand. You can find these documents on the Intranet > Online service Area > Documentation > Internal Documentation.

#### 2.1.1 Installation instructions A+W Business Pro

The installation instructions for A+W Business Pro are here:
`\\Jupiter\SW_Install\v6\InstallationDocumentation\EN-INST-A+W Business Pro.pdf`

#### 2.1.2 Configuration instructions A+W Business

The old instructions are here:
`\\jupiter\doku_docuware\ALFAK2000\!General\Installation_Configuration\DE-Installationshinweise.pdf`

The current instructions are found here:
`\\Jupiter\SW_Install\v6\ConfigurationDocumentation\DE-CONFIG-A+W Business.pdf`

#### 2.1.3 Configuration instruction License Server

The current instructions are found here:
`\\Jupiter\SW_Install\2012\InstallationDocumentation\EN-INST-A+W License Server.pdf`

#### 2.1.4 Configuration instruction License Client

The current instructions are found here:
`\\Jupiter\SW_Install\2012\InstallationDocumentation\EN-INST-A+W License Client.pdf`

#### 2.1.5 Configuration instruction A+W CAD Designer (Shape)

The current instructions are found here:
`\\Jupiter\SW_Install\V6\InstallationDocumentation\EN-INST-A+W CAD Designer Shapes.pdf`

#### 2.1.6 Configuration instructions machines, bender output

The current instructions are found here:
`\\Jupiter\SW_Install\v6\ConfigurationDocumentation\EN-CONFIG-A+W Production MachineControl.pdf`

### 2.2 System environment

The operating system should support at least .Net 4.5.2 (Windows 7 SP1, Windows 8, Windows 8.1, Windows Server 2008 SP2, Windows Server 2008 R2 SP1, Windows Server 2012 and Windows Server 2012 R2 and higher). The latest Windows updates should be imported. If the system has to be updated before installation, it must be restarted before installation.

### 2.3 Database Server

A+W Business Production Terminal uses the existing A+W Business Pro database. Among other things, this means that only the SQL Server database system is supported. For more information, please read the A+W Business Pro installation instructions (chapter `Fehler! Verweisquelle konnte nicht gefunden werden.` / `Error! Reference source not found.`).

### 2.4 .Net Framework 4.5

The .Net Framework 4.5 is required and will be installed by the Setup Launcher. Before installation, please check the required rights for the installation.

### 2.5 License Server

The license server must be installed. Please read the appropriate instructions (chapter 3.1.2).

## 3. Installation

You need administrator rights for the installation and configuration.

### 3.1 Minimal program versions

#### 3.1.1 A+W CAD Designer (Shapes)

The following program and build versions are required:
-   AWSNLive.ocx: 13.4.389
-   SN.exe: 13.4.322

#### 3.1.2 A+W Business database scripts

You need at least the following database scripts:
-   20171124a
-   20171026a
-   20170922a

It is recommended that you bring the A+W Business Pro database up to date.

#### 3.1.3 A+W Production Manager

You need at least version 13.4.885.0

#### 3.1.4 A+W Business Module

The A+W Business Time Management is absolutely necessary.

### 3.2 Setup Starter

Start the Setup Starter from your installation disk set. First the required .Net framework is installed if it is not yet on the PC.

### 3.3 Installation with the Setup Launcher

#### 3.3.1 Welcome Screen

First you see the welcome screen of the Setup Launcher.

