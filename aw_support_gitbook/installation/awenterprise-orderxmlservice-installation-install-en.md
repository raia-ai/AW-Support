---
description: "EN-INST-AW_Enterprise_OrderXML_Service"
---


# Installation Instructions: A+W Enterprise 6 OrderXML Service

---
## Change history:

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 16.04.19 | MP | New creation | 1.0 |
| 16.12.13 | MP | AutoUpdate | 1.1 |
| 17.11.28 | MP | Client number | 1.2 |

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## 1. Installation of the A+W Enterprise 6 OrderXML Service

The following installation instructions assume that there is no previous version installed.

An update of an earlier release version of the A+W Enterprise 6 OrderXML Service is executed precisely like a new installation.

An update of an earlier version of the OrderXML Service, e.g. from ALCIB 2011 OrderXML Service to A+W Enterprise 6 OrderXML Service is not possible. Only one version of the OrderXML Service should be installed.

This document describes only the installation and configuration of the A+W Enterprise 6 OrderXML Service. In case of questions about the installation or configuration of dependent set-ups/disk sets, please see the installation instructions for these products.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:

-   Installation and configuration of the Informix driver via setnet32.exe
-   Creation of the necessary set-ups/disk sets
    -   A+W Enterprise 6 OrderXML Service
    -   A+W Infrastructure 6 Collector Services
    -   A+W Infrastructure 6 Middleware
    -   Java 7 Update 51
    -   A+W Setup Launcher
-   Installation of the OrderXML Service and the dependent disk sets with the Setup Launcher
-   Configuration of the OrderXML Service with the Config Tool

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:

-   Processor: 3000 Mhz
-   RAM: 4 GB
-   Other: /

For an initial or new installation, an installation time of 15 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

### 1.3 Requirements

#### 1.3.1 Windows Server Version

Supported operating systems:

*   Windows 2008 Server R2 32/64bit
*   Windows 2012 Server R2 32/64bit

#### 1.3.2 Network

For the installation itself, no network access is necessary.

For the operation of the service, there must be a connection to the A+W Enterprise DB Server and, depending on the configuration, to the company network.

#### 1.3.3 Software

It is assumed that the following disk sets were already installed and configured BEFORE the installation of the A+W Enterprise 6 OrderXML Service disk set.

*   Informix Client SDK 3.5 TC9 (or newer)
*   Microsoft .NET Framework 4.5.1 SDK

### 1.4 Procedure

For the installation, please proceed in the following sequence:

1.  Use `setnet32.exe` to configure the database server and hosts. This assumes that an IBM Informix Client SDK was installed (see software requirements).

2.  Installation of the A+W Enterprise 6 OrderXML Service with the Setup Launcher.
    On the **Component Selection** dialog on the A+W Enterprise node, select the "A+W Enterprise 6 OrderXML Service" module. This automatically selects all dependent set-ups.

    