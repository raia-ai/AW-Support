---
description: "EN-INST-AW_Enterprise_Frontend"
---


# Installation Instructions: A+W Enterprise 6 Frontend

---
## Change history:

| Date      | Edited by | Remarks                  | Version |
| :-------- | :-------- | :----------------------- | :------ |
| 16.04.18  | MP        | Creation                 | 1.0     |
| 16.05.31  | MP        | SSH proxy                | 1.1     |
| 16.12.13  | MP        | AutoUpdate               | 1.2     |
| 21.02.20  | TSC       | Adjustments to WiX setup | 1.3     |

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1. Check the installation requirements.
2. Compile the required data, additional programs, drivers, etc.
3. Note or determine the time required.

---

## 1. Installation of the A+W Enterprise 6 Frontend

The following installation instructions assume that there is no previous version installed.

An update of an earlier release version of the A+W Enterprise 6 Frontend is executed precisely like a new installation.

An update of an earlier version of the Frontend, e.g. from ALCIB 2011 Frontend to A+W Enterprise 6 Frontend is not possible. These versions can be operated in parallel on a computer.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:
- Creation of the necessary set-ups
  - A+W CAD Designer (Bars)
  - A+W CAD Designer (Shapes)
  - A+W Infrastructure 6 Collector Services
  - A+W Infrastructure 6 Middleware
  - A+W Enterprise 6 Frontend
  - A+W Setup Launcher
- Execute Setup Launcher and thus install the Frontend disk set.

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
- Processor: 3000 Mhz
- RAM: 4 GB
- Other: /

For an initial or new installation, an installation time of 15 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

#### 1.2.2 Conversion Time for Data Set

No data is converted.

### 1.3 Requirements

#### 1.3.1 Hardware

- 1200 MHz or higher processor.
- 512 MB or more main RAM.
- 250 MB or more hard disk.
- Network card.

#### 1.3.2 Network

For installation itself, no connection to a network is required. For the operation of A+W Enterprise 6 Frontend, however, a network connection to the A+W Enterprise Application Server must be established.

If a firewall is installed, then the ports 5000 to 5050 and 512 must be opened.
It is recommended that you deactivate the Windows firewall. The Windows firewall can cause problems with some server operating systems. If the server operating system is LINUX, the firewall must be deactivated on the client PCs.

#### 1.3.3 Software

Supported operating systems:
- Windows 7, 8, 8.1 32/64-bit
- Windows 2008 Server R2 32/64-bit
- Windows 2012 Server R2 32/64-bit

The desktop must be set to at least 16-bit color depth.

### 1.4 Procedure

For the installation, please proceed in the following sequence:

1. The user who would like to install the A+W Enterprise 6 Frontend must have administrator rights.
2. Installation of the A+W Enterprise 6 Frontend with the Setup Launcher.
   On the Component Selection dialog on the A+W Enterprise node, select the "A+W Enterprise 6 Frontend" module. This automatically selects all dependent set-ups.
3. All running sessions of the A+W Enterprise 6 front end must be closed so that an installation or update is possible. If this is not the case, the error 1224 will occur during installation.

