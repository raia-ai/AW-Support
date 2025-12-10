---
title: "EN-INST-AW_Production"
source: "EN-INST-AW_Production.pdf"
tags: ["A+W Production", "installation guide", "software setup", "glass industry", "windows manufacturing", "database configuration", "licensing", "troubleshooting"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical manual providing step-by-step installation and configuration instructions for the A+W Production 6 software, designed for the glass and windows industry. It covers system prerequisites, setup procedures, component selection, licensing, and troubleshooting."
long_description: "This document is the official installation guide for A+W Production 6, a specialized software solution for glass and windows manufacturing. It is intended for consultants and system administrators responsible for deploying the software. The guide begins by outlining the necessary prerequisites, including hardware, network, software (Windows 7/Server 2008 R2), database (Informix/SQL Server 2008), and directory permissions. The core of the document details the installation process using the A+W SetupLauncher, covering component selection, module-based configuration dialogs for settings like exchange directories and database connections, and service user setup. It provides a structured sequence for installing various packages like the Process Server and Terminal Server. A significant portion is dedicated to the configuration of A+W ProductionComServer, protocolling, and various parameters from the production database. The guide also covers the multi-step licensing process for the A+W Production Terminal, explaining the roles of the PPS Webservice, AWSOA service, and LicenseClient. A detailed troubleshooting section offers guidance on resolving common licensing issues, including how to use tools like the Service Locator Administration and Protocolling Config Tool to diagnose problems. Finally, it provides technical tips, such as how to manually edit the machine.config file when uninstalling the Informix driver."
---

# Installation Instructions A+W Production 6

---
## Change history:

| Date | Edited by | Comments | Version |
| :--- | :--- | :--- | :--- |
| 08/2012 | Jens Schmidt | Release | 1.0 |
| 2014-07-07 | D.Langsdorf | Revision for SP5.4 | 1.1 |
| 2016-12-27 | M. Schmidt | Revision for v6.2 + PT Licensing | 1.2 |

The installation instructions guide the consultant through the installation and the configuration process of the cited software. Please proceed in the following order:

1.  Check the installation requirements.
2.  Collect the necessary data, additional programs, drivers, etc.
3.  Consider or calculate the time required.

## Content

*   **1 Overview and Basics**
    *   1.1 Prerequisites
        *   1.1.1 Hardware
        *   1.1.2 Network
        *   1.1.3 Software
        *   1.1.4 Database
        *   1.1.5 Exchange directory
        *   1.1.6 Documentation and manuals
*   **2 Installation**
    *   2.1 Procedure
    *   2.2 Installation of A+W SetupLauncher
    *   2.3 Component selection
    *   2.4 Module-based dialogs
        *   2.4.1 Exchange directory
        *   2.4.2 Database connection parameters
        *   2.4.3 Enter the service users
        *   2.4.4 Infrastructure Collector Service
    *   2.5 Configuration
        *   2.5.1 A+W ProductionComServer
        *   2.5.2 Exchange directory
        *   2.5.3 Protocolling configuration
        *   2.5.4 Database connection parameters
        *   2.5.5 Parameter from the production database
        *   2.5.6 Plan Editor settings
*   **3 Licensing**
    *   3.1 Production Terminal
        *   3.1.1 Problem handling
*   **4 Tips and tricks**
    *   4.1 Uninstalling the Informix driver

## 1 Overview and Basics

### 1.1 Prerequisites

#### 1.1.1 Hardware
No special requirements.

#### 1.1.2 Network
A+W Production 6 requires at least a 10 Mbit Ethernet (10Base2 / IEEE 802.3a, 10Base-T / IEEE 802.3i ) network, better Fast Ethernet or Gigabit Ethernet. Please make sure that the client terminals can access the database.

#### 1.1.3 Software
For A+W Production 6, Microsoft Windows 7 is the minimum requirement. For the process server and terminal server, Windows Server 2008 R2 is required.

Please also remember to install all other available service packs for the framework and the operating system. We recommend to always keep the server up to date with the Microsoft Update Service.

The .NET Framework 3.5 SP1 is installed by A+W SetupLauncher. This installation takes about 30 minutes! If possible, please install .NET Framework in advance (or have it installed).

#### 1.1.4 Database
Informix or Microsoft SQL Server 2008 is required as the database system.

#### 1.1.5 Exchange directory
A+W Production 6 requires an exchange directory (also known as Trans or drive P:). This directory must be set up prior to installation. Please make sure that the necessary rights are available for this directory. All A+W Production users have to have full access to this directory. These rights must be granted regarding safety and regarding the release.

*(Images display the Windows properties dialog for a shared folder named 'Trans'. The first image shows the 'Security' tab where permissions for 'Everyone' are set to 'Full control'. The second image shows the 'Sharing' tab, where 'Share Permissions' for 'Everyone' are also set to 'Full control', including 'Change' and 'Read'.)*

#### 1.1.6 Documentation and manuals
The setup also includes the existing manuals in German and in English. They are located in the exchange directory in sub-folder User_Manuals.

## 2 Installation
The setup for A+W Production 6 is available from `\\jupiter\SW_Install\v6`.

### 2.1 Procedure
1.  Please check the requirements
2.  Please make sure that you belong to the local group of administrators.
3.  Start Setup.exe.

### 2.2 Installation of A+W SetupLauncher
A+W SetupLauncher is the central installation and update tool of A+W Software GmbH. After starting "SetupStartes.exe", the following warning may be issued which has to be acknowledged by using the button "Install".

*Fig. 1: Installation of the Setup Launcher*
*(Image shows a User Account Control (UAC) prompt asking for permission to allow a program from an unknown publisher (setup.exe) to make changes to the computer.)*

While the A+W SetupLauncher is installed, .NET Framework 3.5 and Microsoft Windows Installer 3.1 may be installed as well if necessary. When this installation is finished, the program opens and the actual software to be installed can be selected.

- A splash screen appears. Press [Next] to proceed.
- Dialog **Diskset Selection** opens.

*Fig. 2: SetupLauncher – Diskset dialog*
*(Image shows the A+W SetupLauncher window with the "Choose or create your installation diskset" screen. It lists available disksets like "A+W Production Process Server" and "A+W Production Terminal Server".)*

Select the version to be installed. This version is just a preselection of set-up components which can be changed during the installation process.

The shown sequence of packages should match the installation sequence. This means, if several packages are necessary on one server, the individual packages should be installed in the sequence displayed in the A+W Setup Launcher.

These components are listed in section "Component selection".

A dialog opens in which the directories have to be entered:

*Fig. 3: SetupLauncher – Select the installation directory*
*(Image shows the A+W SetupLauncher "Setup Locations" screen. Fields are present for "Diskset Folder", "Installation Drive", and "Hotfix Path".)*

Enter the path for the A+W Diskset in **Diskset Folder**.
(e.g. `\\jupiter\SW_Install\v6\Diskset`)
Enter a hard disk under **Installation drive** and the additional directory structure is provided by the installation.

The A+W Setup Launcher features „Auto Update" and „FTP Download" are described in detail in A+W Setup Launcher Dokumentation.

- Press [Next] to proceed.
- The following dialog shows the already installed A+W components. Press [Next] to proceed.
- A dialog opens to select the installed components.

*Fig. 4: Setup-Launcher – Component selection*
*(Image shows the "Component Selection" screen in SetupLauncher. A tree view lists various A+W products, with "A+W Production 6" and its sub-components expanded and selected.)*

- Press [Next] to proceed.
- Maybe, further configuration dialogs appear.
- Then, a dialog appears with the respective languages for A+W Production, which will be updated in the Text-Table of the Production database.

*Fig. 5: SetupLauncher – Language update*
*(Image shows the "Texte-Language-Setup" screen, allowing the user to select which languages to install from the Texte-Table, with checkboxes for languages like English, German, French, etc.)*

- After this step further configuration dialogs follow.
- The following dialog allows to select the required action:

*Fig. 6: SetupLauncher - Starting the installation*
*(Image shows the final step before installation, offering radio buttons for actions: "Install software", "Install software and save setup configuration to an XML file", "Only save setup configuration to an XML file", and "Manage Hotfixes".)*

**Install Software**: Installs the selected packages without saving the parameters entered.

**Install Software and save setup configuration to a xml file**: Installs the selected packages and saves the defined parameters in a diskset file for further installations. This diskset can be selected from the Diskset Selection Control dialog afterwards.

**Only save setup configuration to an Xml file**: This means that just a diskset file will be created. No software will be installed. This option serves for preparation purposes only.

**Manage Hotfixes**: This means that the hotfix management is started.

Select "Install Software and save setup configuration to a xml file" and press [Next].

- The following dialog lists the individual components to be installed and configured. Installation of the individual components will start automatically.

*Fig. 7: SetupLauncher - Progress display*
*(Image shows the installation progress screen, listing each component, its version, and status columns for Installation, Hotfix, and Configuration.)*

### 2.3 Component selection
2 default disksets in SetupLauncher are available for A+W Production; they define which components are to be installed.

**Note:** Please make sure that the A+W Infrastructure Services (for Logging, Tracing, etc.) especially A+W Infrastructure Service Locater is installed.
Make sure that only one instance of the Service Locator exists in the customer network.

**A+W Production Process Server** – Installation of process server
**A+W Production Terminal Server** - Installation of terminal server or workstation

### 2.4 Module-based dialogs

#### 2.4.1 Exchange directory
*Fig. 7: SetupLauncher - Exchange directory*
*(Image shows the "Production Settings" dialog within the installer, with fields for "Server Directory" (showing a UNC path `\\ALFAKALCIM2012S\Trans\`) and "Server Volume" (showing `P:`).)*

**Server Directory:** Path where A+W Production finds the exchange directory. Please enter the UNC path for the directory you have set up in step 1.5.
**Server Volume:** The preset P: should not be changed because it cannot be guaranteed that all scripts read the value from the registry.

#### 2.4.2 Database connection parameters
*Fig. 8: SetupLauncher - Connection parameters SQL Server*
*(Image shows the "ALCIM Database Connection Parameters" dialog, configured for SQL Server. Fields include Hostname, ALCIM Database, Database User Name, and Password.)*

Please choose the database system and enter the connection parameters.
Alternative: Informix-Database system

*Fig. 9: SetupLauncher - Connection parameters Informix*
*(Image shows the "ALCIM Database Connection Parameters" dialog, configured for Informix. Fields include Hostname, Informix Server Name, Service Name / Port, DB Locale, and Client Locale.)*

#### 2.4.3 Enter the service users
*Fig. 10: SetupLauncher - Service users*
*(Image shows the "ALCIM Service User" dialog, prompting for a User and Password to run the ALCIM services.)*

This dialog can be used to select a user for whom the services are executed. SetupLauncher may want to know whether the user shall have the right to log in as a service. **Please enter Yes to confirm this**.

#### 2.4.4 Infrastructure Collector Service
*Fig. 11: SetupLauncher – Collector Service*
*(Image shows the "Infrastructure Configuration" dialog for "Service Locator Settings". It prompts for the Host and Port (defaulting to 12000) of the service locator.)*

This inquiry is only shown when no infrastructure services have been installed on this computer yet. As a host, enter the computer on which the infrastructure services and thus the service locator have been installed. Enter 12000 as the port. It should only be changed if it is already occupied in the system. This change must then be executed company-wide.

### 2.5 Configuration

#### 2.5.1 A+W ProductionComServer
Define the user account that is in control of the A+W ProductionComServer execution. Start the program 'Component Services' for this purpose (Control Panel/Administration). Select the entry A+W ProductionComServer under DCOM configuration.

*(Image shows the Windows 'Component Services' console, with 'AlcimComServer' highlighted in the DCOM Config list.)*

Select the function "Properties" in the context menu. Select the "Identity" tab in the dialog.

Enter a user with rights in the network, i.e. belongs to a domain. The user must have the right to change Block.ind or Block.zip.

Ensure that for the user account that is used by A+W ProductionComServer:

*   the Brieve-32 bit driver has been installed (only applies if Block.ind is used).
*   the right has been granted to change the file `block.ind` or `block.zip`.

The path to the block database is defined in the file block.pth. If the path includes a drive letter, the drive letter must be connected with the network directory.

*(Image shows the 'AlcimComServer Properties' dialog, specifically the 'Identity' tab, where "This user" is selected, with fields for User and Password.)*

#### 2.5.2 Exchange directory
*Fig.: A+W Production Config - General System Settings*
*(Image shows the "A+W Production Config" tool with fields for Server Directory, Server Volume, User Directory Template, and checkboxes for Terminalserver Mode, Log File Mode, and Don't map Server Directory.)*

**Server Directory:** Path where A+W Production finds the exchange directory. Please enter the UNC path for the directory you have set up in step 1.5.

**Server Volume:** The preset P: should not be changed because it cannot be guaranteed that all scripts read the value from the registry.

**User Directory Template:** Location to save user settings and temporary files

**Override User Directory:** Activates the deviating user directory

**Terminal server mode:** Set to terminal server; cannot be changed and must be activated on workstation. It activates Windows-compliant work by writing into the Program Files directory.

**Log File Mode:** This settings determines whether the tracing for calculating geometries is active only in case of errors (0: default) or always (1: default). The logging is always the same, this settings only determines the trigger. This function is required for tracing so called "Incorrect Cutting Sizes" in order to understand how the calculation was made.

**Don't map Server Directory:** Drive P is not mapped

#### 2.5.3 Protocolling configuration
*Fig.: Log Configuration*
*(Image shows the "Log Configuration" dialog. It allows setting Trace Level and Log Level (e.g., Debug, Info) for different categories like 'AlcimDetailedScheduling' and 'AlcimMasterData', either globally or per user.)*

Tracing and logging behavior for the application and all its integrated components can be set. This is possible globally or per user.

#### 2.5.4 Database connection parameters
*Fig.: A+W Production Config - Database Settings*
*(Image shows the "Database Settings" screen in the A+W Production Config tool. It prompts for DBMS Type, Server instance, User, Password, and Database. A "Test Connection" button is available.)*

This dialog serves to configure the database connection of A+W Production to its production database.

Please choose the database system and enter the connection parameters. The connection can be checked by means of the **Test Connection** button.

#### 2.5.5 Parameter from the production database
Settings from the production database that must be reset when a system is transferred can be changed now.

*Fig.: A+W Production Config - Database Parameter Settings*
*(Image shows the "Database Parameter Settings" screen. It includes sections for "A+W Production Service User", "Shape Catalog", and "A+W PPS Web Service URL".)*

**A+W Production Service User:** User for whom the services run.

**Shape Catalog:** Shape catalog for the system.

**A+W PPS Webservice:** The URL where the PPS web service can be reached.

*Fig.: Database Parameter Settings - A+W ERP WebService*
*(Image shows settings for the A+W ERP WebService, including various ERP parameters like `ERP_DATABASESERVER`, `ERP_DATABASENAME`, and `ERP_WEBSERVICEURL`.)*

**A+W ERP WebService:** Parameter to address the ERP web services.

*Fig.: Configure the BLOCK.PTH files*
*(Image shows a screen to configure paths to `BLOCK.IND` and `BLOCK.ZIP` files, allowing replacement and scanning of paths.)*

Settings for the Block.ind access

*Fig.: License settings*
*(Image shows the "License settings" screen. A default configuration can be set, and specific license types can be assigned per Station ID.)*

Setting for the licenses to be queried for certain modes of A+W Production.
Unless a different setting per station has been selected, the default configuration applies globally for all stations. The corresponding license is subsequently allocated on the license server.

#### 2.5.6 Plan Editor settings
Subsequently, set the settings of the Plan Editor.

*Fig.: A+W Plan Editor Config*
*(Image shows the Plan Editor configuration screen, first asking to set the program language.)*

Here, the language of the Plan Editor is defined.

*Fig.: A+W Plan Editor Config*
*(Image shows the next step, asking for the path to the BLOCK file, e.g., `\\ALFAKALCIM2012sp4\Trans\SN\BLOCK.Zip`.)*

Path to Block.ind with shape 99 parameters.

*Fig.: A+W Plan Editor Config*
*(Image shows the final step for the Plan Editor config, which is the selection of the Shape catalog.)*

Selection of Shape catalog for Plan Editor.

## 3 Licensing

### 3.1 Production Terminal
Licensing of A+W Production Terminal is made in several steps and starts while opening the respective version. The following components are part of the licensing:

*   A+W Production Terminal
*   A+W PPS Webservice
*   A+W AWSOA Infrastructure License (AWSOA-Service)
*   A+W LicenseClient

If a Production Terminal is started, then after selection of the mode to be started and the user, a license query is started via the PPS Webservice. If after an update it is executed for the first time or if initially a license is queried, the PPS Webservice calls an internal component that asks the AWSOA service for the license in question. The AWSOA service logs and initiates the query to the A+W LicenseClient, which grants or refuses the license.

If the AWSOA service cannot be reached later (error, etc.), then an internal cache mechanism in the component of the PPS Webservice ensures that the Production Terminal will still temporarily have access to a valid license. This prevents production shutdowns. The temporary use is indicated to the user for the fastest possible elimination.

Summarized again in brief below:
1.  Start of the Production Terminal
2.  Query of the license via the PPS Webservice
3.  Forwarding of the query to the AWSOA service
4.  Granting/refusal of the license by A+W LicenseClient

While the Production Terminal is running, the license will be confirmed every 5 minutes with a "hold." This serves only the purpose of logging (for query of the license usage duration). On exiting, the license is also "released" again with a corresponding method. However, the current Production Terminal license it not a limited volume license, so that both of these last steps currently serve only the purpose of evaluation.

With respect to the evaluation, it must be mentioned that within the AWSOA service, a Web interface can be called up, which displays the license queries of all A+W programs in "compressed" form. Warning: this is not a real-time display!

*Fig.: View of the license data*
*(Image shows a web interface for infrastructure license monitoring. It displays a table of license usage data, with columns for Module Name, Version, Date, Number of Calls, Usage, and Workstation.)*

This display shows the license data (duration, module, version, etc.) and the respective duration of usage. You must note that current license queries are only displayed after "compression" (once a day) and thus there is a brief offset.

Furthermore, "parallel use" is also visible, which displays the respective parallel use of individual modules.

*Fig.: Parallel use*
*(Image shows the "Parallel Use" tab of the license monitoring web interface, with a table detailing the maximum parallel usage for each module on a specific date.)*

These displays should serve sales and planning to get an overview of the customer's licenses and modules. Thus it is possible to point out bottlenecks to the customer and to enable him to adjust his licensing in timely fashion.

### 3.1.1 Problem handling
The following section will explain important steps to take if the Production Terminal does not start because it cannot get a license.

1.  Are all participating components installed and available?
    a. In particular: can the PPS service be reached and can the A+W LicenseClient reach the appropriate license server?
2.  Is the appropriate AWSOA service running?
3.  Is the appropriate Production Terminal license installed on the license server and can it be reached?

Usually checking into these questions helps clarify licensing problems.

Point 1 is each to check with the set PPS Webservice URL and the A+W LicenseClient Config Tool.

Point 2 can best be checked with the "Service Locator Administration" tool. This can be found in the A+W Start menu folder under "Config tools."

*Fig.: Initial view of the opened tool*
*(Image shows the 'IceGrid Admin' tool, which is initially empty and displays "Working Offline".)*

First you must connect to the respective "IceGrid registry," under which all A+W AWSOA services run and can be reached.

The following steps describe how to add the connection:
1.  Click the "Log into an IceGrid Registry" button in the top left. The following window opens:
    *Fig.: Saved Connections - IceGrid Admin*
    *(Image shows the 'Saved Connections' dialog with options to create a 'New Connection', 'Edit', 'Set As Default', etc.)*

2.  Here, first the connection must be created once with "New Connection."

    *   **2.1. Direct Connection**
        *(Image shows the 'New Connection' wizard, asking to choose between a 'Direct Connection' and a 'Routed Connection'.)*
    *   **2.2. Master Registry**
        *(Image shows the next step, a checkbox to "Connect to a Master Registry".)*
    *   **2.3. Manuel Endpoint**
        *(Image shows a list of 'Discovered Endpoints' and a field to enter a 'Manual Endpoint'.)*
    *   **2.4. Hostname and port number**
        *(Image shows a choice between providing 'A hostname and a port number' or 'An endpoint string'.)*
    *   **2.5. Localhost, 12000 and TCP**
        *(Image shows fields to enter the Hostname ('localhost'), Port number ('12000'), and Protocol ('TCP').)*
    *   **2.6. Username und password (both are arbitrary, but not empty)**
        *(Image shows fields for Username and Password.)*
    *   **2.7. Finish**

After these steps, you should see the following view:

*Fig.: Connection to AWRegistry*
*(Image shows the 'IceGrid Admin' tool now connected to the 'AWRegistry (Master)'. The left pane shows a tree of deployed services like QM-AWBAWP60-CIM, -Infrastructure, etc.)*

Links are now listed for all installed AWSOA services. For successful licensing, the following service should be installed and started:

*Fig.: Infrastructure-License-001*
*(Image shows the 'IceGrid Admin' tool with the 'QM-AWBAWP60-Infrastructure-License-001' service selected. The right pane displays its properties, including State ('Active'), Path to Executable, and other configuration details.)*

#### 3.1.1.1 Execution of the AWSOA service
If the AWSOA service "{Computername}-Infrastructure-License-{ClientId}" is not started (you can see if something is started if there is an icon with a green arrow), then it can be started with a right-click on "Start" on the context menu.

Here you can see that the start of the service also starts all dependent components and services.

Usually, there are errors here: The service cannot be started. Here, a view of the error output of the service to be started can help:

*Fig.: Starting a service*
*(Image shows the context menu after right-clicking a service in IceGrid Admin, with the 'Start' option available.)*

Now a window opens on which the start process is logged and errors are displayed accordingly:

*Fig.: Server stderr - IceGrid Admin*
*(Image shows a log output window from IceGrid Admin, displaying warnings and service observer messages related to the service startup.)*

If the display does not show the complete list of errors, you can use "Edit > Preferences" to increase the internal display of the characters and lines:

*Fig.: Preferences - IceGrid Admin*
*(Image shows the 'Preferences' dialog for IceGrid Admin, which allows adjusting buffer sizes like 'Max lines in buffer' and 'Max characters in buffer'.)*

If you make adjustments here, then close the output and open it again (only then are the settings applied).

The error messages logged can indicate missing components (usually after a flawed update) or occupied or locked ports.

#### 3.1.1.2 Logging and tracing of the AWSOA services
If the license service runs successfully, however, then the next thing you should do is increase the tracing to find a possible cause.

For this, you should first start the "A+W Protocolling Config Tool" in which all AWSOA services can be configured appropriately:

*Fig.: A+W Protocolling Config*
*(Image shows the 'A+W Protocolling Config' tool. A dropdown menu for 'Service' is displayed.)*

Here, select "Infrastructure License" in the combo box and click "Protocol."
On the dialog that appears, select the category "InfrastructureLicense" under "AWSOA Infrastructure" and set the trace level for error tracing to "Debug."

Then you stop and start the license service in the Service Locator Administration and try again to query a license by starting the Production Terminal. Now there should be at least one entry with the appropriate category in the trace file for the service; it describes possible causes.

If you cannot find any error here, you can also check whether the correct Production Terminal license was installed – via A+W License Monitor – and whether the license server can also be reached. There is an appropriate connection test in the config tool of the license server. This test checks the connection to the license server if it is on another computer on the network. If the license server is running on the local computer, you can check with the display of the local services (e.g. in the Task Manager) whether the license server has been started. With the "SafeNet Aladdin Control Center (HASP Tool)" from the Config Tools folder, you can check whether the dongle is connected correctly to the computer (for more information about this, see the installation instructions for the license server, section 1.8).

## 4 Tips and tricks

### 4.1 Uninstalling the Informix driver
During the installation of the Infomix driver an assembly redirect is entered into the machine.config.

For this purpose, the key is
`<runtime />`
replaced with
```xml
<runtime>
  <assemblyBinding xmlns="urn:schemas-microsoft-com:asm.v1">
    <dependentAssembly xmlns="urn:schemas-microsoft-com:asm.v1">
      <assemblyIdentity name="IBM.Data.Informix" publicKeyToken="7c307b91aa13d208" />
      <bindingRedirect oldVersion="1.0.0.0-3.0.3000.2" newVersion="3.0.0.2" />
    </dependentAssembly>
  </assemblyBinding>
</runtime>
```

Machine.config is located at two locations:
*   C:\Windows\Microsoft.NET\Framework\v2.0.50727\CONFIG
*   C:\Windows\Microsoft.NET\Framework\v4.0.30319\Config

When you uninstall the Informix driver, you must reset these entries manually! This is not necessary when an update is executed!
