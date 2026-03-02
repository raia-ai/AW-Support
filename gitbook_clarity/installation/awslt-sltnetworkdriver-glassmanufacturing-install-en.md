---
description: "EN-INST-AW_SLT_Network_Driver"
---


# Installation Instructions: A+W SLT Network Driver

---
## Change history:

| Date      | Edited by | Remarks          | Version |
| :-------- | :-------- | :--------------- | :------ |
| 13.11.11  | MP        | Original version | 0.9     |
| 16.04.25  | MP        | Update           | 1.0     |

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## 1 New installation

The following installation instructions assume that there is no previous version installed.

The update of an earlier release version of the A+W SLT Network Driver is performed exactly as a new installation.

The installation of the A+W SLT Network Driver is only necessary if A+W SLT runs in the so-called network mode.

The real name of the A+W SLT Network Driver is FBTreiber and stands for FireBird driver.

### 1.1 Overview and the basics

The following list provides and overview of the work that must be done during installation:
- Creation of the necessary set-ups
  - A+W SLT Network Driver
- Installation with the Setup Launcher

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
- Processor: 3000 Mhz
- RAM: 4 GB
- Other: /

For an initial or new installation, an installation time of 5 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

### 1.3 Requirements

#### 1.3.1 Hardware

Up-to-date Windows computer.

#### 1.3.2 Network

For the installation itself, no network access is necessary.
To operate the A+W SLT, there has to be a connection to the A+W SLT main installation and the company network.

#### 1.3.3 Software

- A+W SLT in network mode

### 1.4 Procedure

For the installation, please proceed in the following sequence:

1.  **Installation of A+W SLT Network Driver with the Setup Launcher**

    On the **Component Selection** dialog on the **External Software** node, select the A+W SLT module. Currently, there are no depending Setups.

    [Image: A+W SetupLauncher showing the Component Selection screen. Under the 'External Software' tree, 'A+W SLT Network Driver' is checked. The description pane reads: "The A+W SLT Network Driver is needed to connect to a remote A+W SLT Installation. Install on: terminal server, client computer. Version: 1.0.0.0..."]

2.  **Execute Setup**

    No configuration is necessary. Confirm all dialogs with "Proceed".

### 1.5 Result of the installation

The program files were unpacked under `C:\Program Files (x86)\Sommer Informatik GmbH\FBTreiber`.

### 1.6 Uninstalling

To uninstall the software, go to the Control Panel under "Programs and Features", select the entry "FBTreiber" and execute the option "Uninstall".

[Image: Windows 7 Control Panel, "Programs and Features" view. The list of installed programs is visible, and the entry "FBTreiber" from publisher "Sommer Informatik GmbH" is highlighted.]

[Image: A confirmation dialog box in German titled "Programme und Funktionen". The text asks "Möchten Sie FBTreiber wirklich deinstallieren?" (Do you really want to uninstall FBTreiber?), with "Ja" (Yes) and "Nein" (No) buttons.]
