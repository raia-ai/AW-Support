---
title: "EN-INST-AW_License_Client"
source: "EN-INST-AW_License_Client.pdf"
tags: ["A+W", "License Client", "Installation", "Configuration", "Software", "Windows", "SetupLauncher", "Technical Documentation", "System Requirements"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides comprehensive installation and configuration instructions for the A+W License Client software. It covers system requirements, step-by-step procedures using the SetupLauncher, and detailed expert settings for both machine-wide and user-specific configurations."
long_description: "This is an official installation guide for the A+W License Client, a critical component of the A+W software suite designed for the glass and windows manufacturing industry. The document provides detailed instructions for system planners and administrators to perform a new installation of Version 5 SP4. It begins by outlining prerequisites, such as local administrator rights and network connectivity to an A+W license server. The core of the document is a step-by-step walkthrough of the installation process using the A+W SetupLauncher, guiding the user from starting the installer and selecting the correct software modules to configuring the connection to the license server. It includes screenshots of each dialog box in the installation wizard. The guide also covers important post-installation topics, including how to configure protocol and logging settings, how to uninstall the client via the Windows Control Panel, and how to perform an update. A detailed appendix is provided for experts and special users, offering in-depth explanations of advanced configuration options. This includes the 'ConfigTool' for both computer-wide (machine) and user-specific settings, which is essential for environments like terminal servers. The appendix thoroughly documents various connection types (PIPE, TCP, .net-Remoting) and legacy support, complete with tables that explain each configuration parameter, its possible values, and its function."
---

# Installation Instructions: A+W License Client

**Software for Glass and Windows**

---
## Change history:

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2014-07-18 | J. Makowka | Original version | 1.0 |
| 2022-12-08 | B. Hanewinkel | System requirements | 1.1 |

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1. Check the installation requirements.
2. Compile the required data, additional programs, drivers, etc.
3. Note or determine the time required.

---

## Content

### Installation Instructions
- A+W License Client

### 1. New Installation of Version 5 SP4
- **1.1 Overview and the basics**
- **1.2 Time requirement**
  - 1.2.1 Installation time for the software
  - 1.2.2 Conversion time for data stock
- **1.3 Requirements**
  - 1.3.1 Hardware
  - 1.3.2 Network
  - 1.3.3 Software
- **1.4 Procedure**
- **1.5 Incompatibilities**
- **1.6 Directory structure**
- **1.7 Settings**
  - 1.7.1 Protocol Settings
- **1.8 Result of the installation**
- **1.9 Configuration**
- **1.10 Alternative Installations**
- **1.11 Uninstalling**

### 2. Update License Client

### 3. Appendix
- **3.1 Configuration Settings for Experts and Special Users**
  - 3.1.1 ConfigTool for Computer-Wide Settings (License Client Machine Settings Config Tool)
  - 3.1.2 User-Specific Configuration (License Client User Settings Config Tool)

### 4. Table of Figures

---

## 1. New Installation of Version 5 SP4

The following installation instructions assume that there is no previous version installed.

### 1.1 Overview and the basics

For the installation of the license client you must have local administrator rights on the machine on which the client shall be installed.
The following list provides an overview of the work that must be done during installation:

> Installation of the license client with the Setup Launcher. Normally, you install the license client together with other A+W products.

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
- Processor: Intel Xeon E5520, 2.67 GHz
- RAM: 4 GB

For an initial or new installation, an installation time of 2 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated. When combined with the installation of other A+W software, the time required for installing the clients' licence is negligible.

#### 1.2.2 Conversion time for data stock

Data is not converted. Therefore no time is required for this purpose.

### 1.3 Requirements

#### 1.3.1 Hardware
There are no additional hardware requirements.

#### 1.3.2 Network
If the license server is located on a different machine, a stable network connection to this machine must exist.

#### 1.3.3 Software
An A+W license server must exist, run and be available in the network. This condition is met even if an A+W license server is installed on the same machine on which the license client is supposed to be installed or if the A+W license server is installed on the machine during the course of the same SetupLauncher session.

For the license client, installation on Windows 10 or Windows 11 is recommended. If it is to be run on a terminal server, Windows Server 2008 R2 or higher is required.
Reinstallation on older systems is not supported. Windows systems for which Microsoft support has expired may have limited support.

### 1.4 Procedure

For the installation, please proceed in the following sequence:

1.  Start the installation of the SetupLauncher from your diskset. Usually, you will only do this once and then install all required A+W packages.

    **Fig. 1: Start SetupLauncher installation**
    > The image shows a Windows Explorer window displaying the contents of an installation folder named '2012.4'. The 'SetupStarter.exe' application is highlighted, indicating it's the file to be executed to begin the installation.

2.  Confirm the administrator rights for the installation.

    **Fig. 2: Confirm the administrator rights**
    > The image displays a 'Open File - Security Warning' dialog box. It warns that the publisher of 'SetupStarter.exe' cannot be verified and asks for confirmation to run the file. The 'Run' button is the expected action.

3.  You may receive additional safety information and queries depending on the operating system of the machine and the configuration of the computer. Always confirm with "Continue", "OK", etc.

4.  Wait until SetupLauncher has been installed.

    **Fig. 3: Example of an installation progress box**
    > This image shows the 'A+W SetupLauncher - InstallShield Wizard' progress box. It indicates that the setup is preparing the wizard and configuring the Windows Installer.

5.  Click "Next" in the welcome dialog of SetupLauncher.

    **Fig. 4: Welcome dialog of SetupLauncher**
    > The image displays the initial welcome screen of the A+W SetupLauncher wizard. An arrow points to the 'Next' button to proceed.

6.  The license client is included in the standard disksets that SetupLauncher offers for the installation. Usually, you select one of these disksets, e.g. "A+W Business Pro." You can also select one of the other standard disksets or create your own diskset. The approach depends on the A+W product you intend to install.

    **Fig. 5: Select diskset**
    > The image shows the 'Choose or create your installation diskset' screen in the SetupLauncher. A list of 'Available Disksets' is shown, with several options like 'A+W Business Pro' highlighted with a red bracket, indicating that one of these should be selected.

7.  In the SetupLauncher, you can now set up the installation plate and hotfix source, execute an FTP download or configure the auto update. For this purpose, please read the documentation on the product you are installing. Unless the corresponding documentation includes different instructions, you can leave the preset default values unchanged and exit the dialog by selecting "Next." You can also execute the auto update configuration later.

    **Figure 6: SetupLauncher - System settings**
    > This image shows the 'Setup Locations' screen. It displays default paths for the 'Diskset Folder', 'Installation Drive', and 'Hotfix Path'. An arrow points to the 'Next' button.

8.  The next dialogue shows the installed A+W software. Since this is a new installation, only the SetupLauncher is listed. Exit the dialog using "Next."

    **Figure 7: Installed A+W software**
    > The image displays the 'Installed Components' screen, which lists software already installed by the launcher. In this case, only 'A+W SetupLauncher' is listed. An arrow points to the 'Next' button.

9.  In the following dialog, you can select the software that is to be installed. For standard disksets the license client modules are already preselected. The actual module is "A+W License Client." The modules "A+W Infrastructure 5 Collector Services" and "A+W Infrastructure 5 Middleware" are additionally required so that the protocols of the license client can be provided centrally. These modules are also preselected. If you install the license client in a different context, you may need to make these selections yourself. After selecting, exit the dialog using "Next."

    **Fig. 8: Modules of the license client**
    > The image shows the 'Component Selection' screen. A list of available software modules is displayed. Red circles highlight 'A+W Infrastructure 5 Collector Services', 'A+W Infrastructure 5 Middleware', and 'A+W LicenseClient', indicating these are the required components to be selected for installation.

10. Depending on the product you are installing, you may now need to fill out one or several entry dialogs. Please look up these dialogs in the installation instructions for the product you are installing. Lastly, the entry dialog for the infrastructure configuration opens. Under "Host," enter the name of the server on which the network-wide service locator runs. Please read the installation instructions for the infrastructure services for further information.

    **Figure 9: Infrastructure configuration**
    > This image shows the 'Infrastructure Configuration' dialog. It requires the 'Host' name and 'Port' for the Service Locator. The host field is populated with a placeholder 'INFRASTRUCTURE.DOMAIN.INTRA'. An arrow points to the 'Next' button.

11. The SetupLauncher has now collected all required data. Leave the preset selection "Install software and save setup configuration to an XML file" and click "Next."

    **Figure 10: Start installation**
    > The image shows the final screen before installation begins. The radio button 'Install software and save setup configuration to an XML file' is selected, and an arrow points to the 'Next' button.

12. Now you have to enter a name under which the diskset is saved for later references.

    **Fig. 11: Save diskset**
    > The image shows a 'Save As' dialog box. The user is prompted to enter a 'File name' for the diskset configuration. The example name is 'Thisinstallation' and the 'Save' button is highlighted.

13. Now the installation of the modules starts. During the installation, the Setup Launcher displays the installation progress. You may also see various progress displays and notes. Wait until the configuration part of the SetupLauncher session starts.

    **Figure 12: Installation progress**
    > This image shows the 'Installing...' screen, which displays a table of products being installed. The status of each component (e.g., 'OK', 'Installing', 'Ready to install') is shown.

14. The configuration tool for the license client is called up in the configuration section of the SetupLauncher session. On server systems, it is possible that the tool opens behind the SetupLauncher dialog. If this is the case, click on an area of the configuration tool that does not include any buttons, in order to get the tool to the front.

    **Fig. 13: Activate config tool**
    > This image shows the 'Configuring...' screen of the SetupLauncher. A separate configuration window is partially visible behind it. A red arrow indicates that the user should click on the background configuration tool to bring it to the foreground.

15. In the configuration tool, you must select the license server to which the license client should connect. If a license server is running on the machine on which you are installing the license client, the selection option "The license service is running on this machine" is available and preselected. Normally, this is not the case; then this selection option is not available and instead the option "The license server is running on another machine" is preselected. If this selection has been made, you must always enter the name or the IP address of the machine on which the license server is running into the field "Host name or IP address." You can have the connection to other machines checked by clicking on the "Test" button.

    **Note:** In order to successfully complete the configuration, it is required that the license client can communicate with the specified license server.

    Click "Next" to open the next dialog.

    **Fig. 14: Select license server**
    > The image shows the 'License Client Configuration' tool. The option 'The license service is running on another machine' is selected. The user needs to enter the 'Host name or IP address' of the license server, with a placeholder 'LICENSESERVER.DOMAIN.INTRA' shown.

16. The configuration tool obtains data from the license server now. During this process you will see a message.

    **Fig. 15: Obtaining data from the license server**
    > A small message box is shown, indicating that the 'License Service is still starting and refreshing its license data'. A progress bar is visible at the bottom.

17. Now you must confirm or enter the settings for the workstation. Usually, the top three selection options are deactivated since there are no selection options available in the license. If a selection option has been enabled, make sure you make the correct selection for the workstation. You can also change the selection later by selecting the "License Client Machine Settings Config Tool" from the A+W program selection. Click the "Next" button to show the results.

    **Fig. 16: Workstation settings**
    > The image displays the 'License Settings' screen in the configuration tool. It shows dropdowns for 'Company group', 'Site', and 'Workstation (LS)'. The values are pre-filled (e.g., 'Standard', 'TS-12R2-FULL'). An arrow points to the 'Weiter' (Next) button.

18. You will see the configuration results in the bottom section. Click the "Next" button to complete the configuration.

    **Fig. 17: Configuration results**
    > The 'Finished Configuring License Client' screen is shown. The results section at the bottom confirms 'Licenses info Read Success' and 'Base settings Save Success'. An arrow points to the 'Weiter' (Next) button.

19. Now the configuration of the license client within the scope of the SetupLauncher session is completed. Click on the "Finish" button to exit the configuration tool and continue with the configuration tools of other components, if applicable. Please look up the installation instructions for the remaining modules to be installed in order to obtain information about the processes and entries.

    **Fig. 18: Completing the installation**
    > The 'Configuration finished' screen is shown, with the same success messages as the previous step. A red arrow points to the 'Finish' button.

20. As soon as all required configurations have been set, you will see the completion notification of the installation. Please wait until you see this notification. SetupLauncher may still be running operations in the background even if it seems in the foreground as if the installation is finished.

    **Fig. 19: Installation end**
    > A small dialog box titled 'Installation complete' is displayed with the message 'The installation is finished'. An arrow points to the 'OK' button.

21. After installation has been completed, close the Setup Launcher using the "End" button.

    **Figure 20: Terminate SetupLauncher**
    > The final screen of the SetupLauncher, 'Installation finished!', is shown. It provides a summary of all installed components and their status. An arrow points to the 'End' button.

## 1.5 Incompatibilities
No incompatibilities are known.

## 1.6 Directory structure
The program does not use any data on the hard disk. The protocols are stored at the usual location (`%PROGRAMDATA%\A+W\Log`).

## 1.7 Settings
All settings shall be made with one of the configuration tools for the license client. There is the "License Client Machine Settings Config Tool" for machine-wide settings and the "License Client User Settings Config Tool" for user-specific settings. The latter is only important in exceptional cases and is usually not used.

In addition to the basic configuration that has been made during the installation, only the protocolling configuration is of general interest. The configuration tools additionally offer a number of advanced configuration settings. These settings are described in the attachment.

### 1.7.1 Protocol Settings
There are two sections in the license client for which the protocol settings can be set at different locations. On a client machine there is a license proxy service. The protocol settings for this proxy service can be set with the "License Client Machine Settings Config Tool."

Every program that is subject to license includes a component for communicating with the license proxy. This component does not have its own protocol category. It uses the category "AlbwirBasis" to write entries. You can set this category in the "Basis" tab of the protocol configuration of the configuration tool for the program in question.

#### 1.7.1.1 Protocol settings of the license proxy service
The protocol settings for the license proxy service can be changed with the "License Client Machine Settings Config Tool." You can start this tool from the folder "Config Tools" in the A+W start window. You have to have administrator rights to use this tool.

The configuration tool differs from the variant that you see during the installation with the SetupLauncher by the two buttons "Expert Settings" and "Protocol" on the first page. The settings that can be made using the button "Expert Settings" are described in the attachment. Click on the "Protocol" button to change the protocol settings. Click on [Protocol] to change the protocol settings.

**Fig. 21: License Client Machine Settings Config Tool**
> This image shows the main window of the 'License Client Configuration (Machine Global Settings)' tool. An arrow points to the 'Protocol' button, distinguishing it from the installation wizard version.

The settings on the "LicenseProxy" tab relate to the areas of the license proxy.

**Fig. 22: License proxy settings**
> This image displays the 'Protocol Configuration' dialog with the 'License Proxy' tab selected. It shows a list of categories (e.g., `AWCLicenseCache`, `AWCLicenseClient`) and their configurable 'Trace Level' and 'Log Level'.

| Category | Description |
| :--- | :--- |
| **AWCCacheLicensing** | Entries that relate to licensing from the license cache on the client side. |
| **AWCLicenseCache** | Entries that relate to the operation of the license cache on the client side (e.g. activation, deactivation, mode switching). |
| **AWCLicenseClient** | Entries that relate to the communication with connected clients. |
| **AWCLicenseProxy** | Entries that relate to the operation of the license proxy (e.g. communication errors with the license server, notifications from the Windows service). |
| **AWCLicenseWatcher** | Entries of the Watcher service that monitors the license proxy. |
| **AWCLicensing** | Entries that relate to the communicated licensing (license server or license cache). |

On the "Basis" tab, you will see the protocol settings for the basis libraries.

**Fig. 23: Settings for the basis libraries**
> This image shows the 'Protocol Configuration' dialog with the 'Basis' tab selected. It lists categories related to base libraries like `AlbwirBasis`, `AWBinding`, etc., and their logging levels.

| Category | Description |
| :--- | :--- |
| **AlbwirBasis** | Entries resulting from functions of the Albwir.Basis and other basis libraries. Many base functions, e.g. standardized database functions use this protocol category to write entries. |
| **[...]** | Special protocol categories of certain functions. Please leave the settings for these categories under Trace Level at "Error" until you are requested by a developer to change them. Changes to these protocol categories can result in log occurrences in the range of gigabytes within very short periods of time. |

After you have carried out the requested changes, click the "OK" button to save the changes. Exit the configuration tool by clicking "Next" until you can exit the tool using "Finish." This will trigger a restart of the license proxy so that the new settings take effect. Please note that it is useless to enter user-specific settings for the protocol level. The license proxy is a Windows service that runs under a separate service user. Therefore, user-specific settings do not take effect.

## 1.8 Result of the installation
The installation has been carried out correctly if you see the text "Success" in the two result lines of the dialog shown in Chapter 1.4, item 18.

## 1.9 Configuration
No further configurations are required.

## 1.10 Alternative Installations
Support is available for the communication procedure of older programs subject to license. Read the attachment for details.

## 1.11 Uninstalling
You can uninstall the license client by using the Windows Control Panel. Uninstalling is basically only necessary if the A+W software is to be deleted from a machine.

**Fig. 24: Uninstall license client**
> The image shows the 'Programs and Features' window in the Windows Control Panel. A list of installed programs is displayed, and a red arrow points to 'A+W LicenseClient', indicating it can be uninstalled from here.

---

## 2. Update License Client
The update of the license client does not differ from a new installation. The previously set values are preset in the configuration tool in the configuration section of the SetupLauncher session and do not need to be reentered.

---

## 3. Appendix

### 3.1 Configuration Settings for Experts and Special Users

#### 3.1.1 ConfigTool for Computer-Wide Settings (License Client Machine Settings Config Tool)

**Fig. 25: License client configuration - basic configuration, computer-wide**
> The image shows the main screen of the 'License Client Configuration (Machine Global Settings)' tool.

| Key | Value | Description |
| :--- | :--- | :--- |
| **The license service is running on this machine.** | • Not selected (workstations)<br>• Selected (process server) | The license service runs on the same computer on which the license client is running. The settings are then made by the Config Tool so that they are optimized for this case. |
| **The license service is running on another machine.** | • Selected (workstations)<br>• Not selected (process server) | The license service and license client do not run on the same computer. In this case, the computer on which the license service runs must be entered in the field "Host name or IP address." |
| **Host name or IP address** | Name of the computer with the license service | The name or the IP address of the computer on which the license service runs. |
| **Test** | (Button) | With this button you can check the connection to the license service if the option "The license service is running on another machine" has been selected. |
| **Caution: personal settings for this user are overriding the global machine settings** | Visible or hidden | If this note is visible, it means that there are user-specific settings that overwrite the computer-wide settings for the logged-on user. You can check and edit such user-specific settings with the "License Client User Settings Config Tool" (see 3.1.2). This note is a link which shows a detailed note when you click on it (Figure 26). |
| **Expert settings** | (Button) | Open the advanced dialogs for the expert settings with this button (see Figure 28 et seq.). Please note that you can make any setting in the expert dialogs – even settings that will result in an inoperable system. Therefore, you should normally avoid using the expert dialogs. You should only use these dialogs if you have been asked to do so by an employee of A+W Service or a developer. |

**Fig. 26: License client configuration - note regarding user-specific settings**
> This dialog provides more details if the Config Tool has recognized that there are user-specific settings that overwrite the computer-wide settings for the logged-on user. It is just for information purposes.

**Fig. 27: License client configuration - workstation settings**
> This image shows the second page of the configuration tool, where 'Company group', 'Site', and 'Workstation (LS)' can be set.

| Key | Value | Description |
| :--- | :--- | :--- |
| **Company group** | STANDARD | Company group under which the licenses will be searched for. The company group is the highest hierarchy level where licenses are granted. You can only change this field if more than one company group has been configured in the license file of the specified license service. Default value: `Standard`. |
| **SITE** | STANDARD | Client under which the licenses will be searched for. You can only change this field if more than one client has been configured in the license file of the specified license service. Default value: `Standard`. |
| **Workstation (LS)** | Name of the workstation | Workstation under which the licenses will be searched for. The workstation is the lowest hierarchy level where licenses can be granted. You can only change this field if the license file of the specified license service includes at least one named workstation. Then you can select one of the named workstations in the license file and the computer name. If you select the computer name, the licenses will be taken from the stock of the "floating licenses." Default value: Name of computer. |

**Expert Settings Dialogs**
> **Please only use this dialog if you are absolutely sure that you know what you are doing!**
> There are different variations of this dialog for the different connection types ("Connection"). The other variations are shown and explained in the images below.

**Fig. 28: License client configuration - expert settings, named pipe**
> This image shows the 'License Client Machine Configuration (Expert Settings)' dialog. The connection type is set to 'WCF Connection to Service via PIPE (Version 2009 and Later)'.

| Key | Value | Description |
| :--- | :--- | :--- |
| **Connection** | WCF Connection to Service via PIPE (From Version 2009) | Connection type for the connection to the license server. *WCF Connection to Service via PIPE (from Version 2009)* means that the connection is established via so-called "named pipes." This connection type can only be reliably established on a local computer by means of a license service. Therefore, the computer cannot be specified if you select this connection type ("Host name/IP"). |
| **Allow modification** | Not selected | This checkbox allows you to edit the input field in front of it. This way, settings that are usually not changed are protected against unintentional changes. Default value: not selected. |
| **Pipe name** | Glaston/SW/LicensePipe | Name of the named pipe used for the connection. This name must be the same as the one that has been configured for the license service. Default value: `Glaston/SW/LicensePipe`. |
| **Provide legacy client interface** | Selected | Determines whether the connection method for applications that was valid until Version 2008 is supported. Default value: selected. |
| **Port no.** | 1571 | Port that is used for the connection method for applications that was valid until Version 2008. Default value: 1571. |
| **Copy global settings**| (Button) | You can only see this button if the settings in the dialog do not match the settings that were valid prior to the dialog being opened. If you can see this button, you can use it to readopt the settings in the dialog that were valid prior to the dialog being opened. As a result, changes that you have made in the dialog will be lost. |

**Fig. 29: License client configuration - expert settings, WCF/TCP**
> This image shows the 'Expert Settings' dialog configured for 'WCF Connection to Service via TCP (Version 2009 and Later)'.

| Key | Value | Description |
| :--- | :--- | :--- |
| **Connection** | WCF connection to service via TCP (from Version 2009) | Connection type for the connection to the license server. *WCF connection to service via TCP (from Version 2009)* means that the connection is established via TCP/IP and WCF. |
| **Allow modification** | Not selected | This checkbox allows you to edit the input field in front of it. Default value: not selected. |
| **Host name/IP** | Name of the computer on which the license service is running | DNS name or IP address of the computer on which the license service is running. |
| **Port no. (top section)**| 1572 | Port number via which the connection to the license service is established. This port must be open for the TCP protocol in the firewall of the computer on which the license service is running. Default value: 1572. |
| **Service name** | Glaston/SW/License | Name of the TCP service that is addressed via the connection. This name must be the same as the one that has been configured for the license service. Default value: `Glaston/SW/License`. |
| **Provide legacy client interface** | Selected | Determines whether the connection method for applications that was valid until Version 2008 is supported. Default value: selected. |
| **Port no. (bottom section)** | 1571 | Port that is used for the connection method for applications that was valid until Version 2008. Default value: 1571. |
| **Copy global settings**| (Button) | You can only see this button if the settings in the dialog do not match the settings that were valid prior to the dialog being opened. Use it to readopt the prior settings. |

**Fig. 30: License client configuration - expert settings, .net-Remoting**
> This image shows the 'Expert Settings' dialog configured for 'Legacy (Remoting) Connection to Service (Pre Version 2009)'.

| Key | Value | Description |
| :--- | :--- | :--- |
| **Connection** | Legacy (Remoting) Connection to Service (Pre Version 2009) | Connection type for the connection to the license server. *Legacy (Remoting) Connection to Service (pre version 2009)* means that the connection is established via TCP/IP and .net-Remoting. This connection type must be set if the addressed license service is a version before 2009. |
| **Allow modification** | Not selected | This checkbox allows you to edit the input field in front of it. Default value: not selected. |
| **Host name/IP** | Name of the computer on which the license service is running | DNS name or IP address of the computer on which the license service is running. |
| **Port no. (top section)**| 1570 | Port number via which the connection to the license service is established. This port must be open for the TCP protocol in the firewall of the computer on which the license service is running. Default value: 1570. |
| **Service name** | AWLicenseServices.rem | Name of the TCP service that is addressed via the connection. This name must be the same as the one that has been configured for the license service. Default value: `AWLicenseServices.rem`. |
| **Provide legacy client interface** | Selected | Determines whether the connection method for applications that was valid until Version 2008 is supported. Default value: selected. |
| **Port no. (bottom section)** | 1571 | Port that is used for the connection method for applications that was valid until Version 2008. Default value: 1571. |
| **Copy global settings**| (Button) | You can only see this button if the settings in the dialog do not match the settings that were valid prior to the dialog being opened. Use it to readopt the prior settings. |

#### 3.1.2 User-Specific Configuration (License Client User Settings Config Tool)

This Config Tool is used to define and edit user-specific settings for the license client. User-specific settings allow the logged-on user to use settings different from the computer-wide settings. For example, this is required on a terminal server if a user should receive his licenses from a separate license stock while the other users obtain them from the stock of floating licenses.

If there are no settings available yet, you cannot directly change the fields Company group, Site und Workstation (LS). First of all, you must create a copy of the computer-wide settings for the logged-on user, using the button Copy global settings. Subsequently, you can change the settings.

**Fig. 31: License client configuration - basic settings, user-specific**
> The image shows the 'License Client Configuration User Settings' tool, with fields for License Service, Company group, Site, and Workstation. Buttons for 'Copy Global Settings', 'Remove Settings', and 'Expert Settings' are visible.

| Key | Value | Description |
| :--- | :--- | :--- |
| **Company group** | STANDARD | Company group under which the licenses will be searched for. You can only change this field if more than one company group has been configured in the license file. Default value: `Standard`. |
| **SITE** | STANDARD | Client under which the licenses will be searched for. You can only change this field if more than one client has been configured in the license file. Default value: `Standard`. |
| **Workstation (LS)** | Name of the workstation | Workstation under which the licenses will be searched for. You can only change this field if the license file includes at least one named workstation. If you select the computer name, licenses are taken from the "floating licenses" stock. Default value: Name of computer. |
| **Copy global settings**| (Button) | Use this button to copy the computer-wide settings into the user-specific settings. You have to do this if no user-specific settings are available yet and you want to define them. |
| **Remove settings** | (Button) | Use this button to remove all user-specific settings. After removal, the computer-wide settings apply for the logged-on user. |
| **Expert settings** | (Button) | Use this button to open the dialog for the expert settings (Figure 32 et seq.). This allows you to set advanced configurations, including a different license service. **Note:** Incorrect settings may prevent the user from obtaining licenses. Only use this if you are absolutely sure what you are doing. |

**User-Specific Expert Settings Dialogs**
> **Please only use this dialog if you are absolutely sure that you know what you are doing!**
> There are different variations of the dialog below depending on the set connection type (Connection). The variations are individually described in this section.

**Fig. 32: License client configuration - connection configuration, same as computer, user-specific**
> This image shows the 'License Client Configuration User Settings (Expert Settings)' dialog where the 'Connection' is set to 'Use Machine Connection Settings'.

| Key | Value | Description |
| :--- | :--- | :--- |
| **Connection** | Use Machine Connection Settings | The computer-wide settings for the connection to the license service are used. This setting represents the most frequent case, as usually only a deviating workstation is specified per user. This ensures the user does not encounter connection problems if computer-wide settings are changed. |
| **Copy global settings**| (Button) | Appears if current settings deviate from previously valid ones. Use this to revert changes made in the dialog. |

> **Please avoid selecting settings in this dialog that are identical to the computer-wide settings. Later changes to the computer-wide settings would then not have an effect on the logged-on user. If you want to use the computer-wide settings for connecting to the license service, please set Connection to "Use Machine Connection Settings."**

**Fig. 33: License client configuration - connection configuration, pipe, user-specific**
> The expert settings dialog configured for a user-specific 'WCF Connection to Service via PIPE'.

| Key | Value | Description |
| :--- | :--- | :--- |
| **Connection** | WCF connection to service via PIPE (from Version 2009) | The connection is established via TCP/IP and WCF. |
| **Allow modification** | Not selected | This checkbox allows you to edit the input field. Default value: not selected. |
| **Pipe name** | Glaston/SW/LicensePipe | Name of the named pipe for the connection, must match the license service configuration. Default value: `Glaston/SW/LicensePipe`. |
| **Copy global settings**| (Button) | Appears if settings deviate from previously valid ones. Use to revert changes. |

**Fig. 34: License client configuration – connection settings, WCF via TCP, user-specific**
> The expert settings dialog configured for a user-specific 'WCF Connection to Service via TCP'.

| Key | Value | Description |
| :--- | :--- | :--- |
| **Connection** | WCF connection to service via TCP (from Version 2009) | The connection is established via TCP/IP and WCF. |
| **Allow modification** | Not selected | Allows editing the input field. Default value: not selected. |
| **Host name/IP** | Name of the computer on which the license service is running | DNS name or IP address of the computer with the license service. |
| **Port no.** | 1572 | Port number for the license service connection, which must be open in the firewall. Default value: 1572. |
| **Service name** | Glaston/SW/License | Name of the TCP service, must match the license service configuration. Default value: `Glaston/SW/License`. |

**Fig. 35: License client configuration - connection configuration, .net-Remoting, user-specific**
> The expert settings dialog configured for a user-specific 'Legacy (Remoting) Connection to Service'.

| Key | Value | Description |
| :--- | :--- | :--- |
| **Connection** | Legacy (Remoting) Connection to Service (Pre Version 2009) | The connection is established via TCP/IP and .net-Remoting. Must be used if the license service is a version before 2009. |
| **Allow modification** | Not selected | Allows editing the input field. Default value: not selected. |
| **Host name/IP** | Name of the computer on which the license service is running | DNS name or IP address of the computer with the license service. |
| **Port no.** | 1570 | Port number for the license service connection, which must be open in the firewall. Default value: 1570. |
| **Service name** | AWLicenseServices.rem | Name of the TCP service, must match the license service configuration. Default value: `AWLicenseServices.rem`. |

---

## 4. Table of Figures
- Fig. 1: Start SetupLauncher installation (Page 4)
- Fig. 2: Confirm the administrator rights (Page 5)
- Fig. 3: Example of an installation progress box (Page 5)
- Fig. 4: Welcome dialog of SetupLauncher (Page 6)
- Fig. 5: Select diskset (Page 6)
- Figure 6: SetupLauncher - System settings (Page 7)
- Figure 7: Installed A+W software (Page 7)
- Fig. 8: Modules of the license client (Page 8)
- Figure 9: Infrastructure configuration (Page 9)
- Figure 10: Start installation (Page 10)
- Fig. 11: Save diskset (Page 10)
- Figure 12: Installation progress (Page 11)
- Fig. 13: Activate config tool (Page 12)
- Fig. 14: Select license server (Page 13)
- Fig. 15: Obtaining data from the license server (Page 13)
- Fig. 16: Workstation settings (Page 14)
- Fig. 17: Configuration results (Page 15)
- Fig. 18: Completing the installation (Page 16)
- Fig. 19: Installation end (Page 16)
- Figure 20: Terminate SetupLauncher (Page 17)
- Fig. 21: License Client Machine Settings Config Tool (Page 19)
- Fig. 22: License proxy settings (Page 19)
- Fig. 23: Settings for the basis libraries (Page 20)
- Fig. 24: Uninstall license client (Page 21)
- Fig. 25: License client configuration - basic configuration, computer-wide (Page 23)
- Fig. 26: License client configuration – note regarding user-specific settings (Page 25)
- Fig. 27: License client configuration - workstation settings (Page 26)
- Fig. 28: License client configuration – expert settings, named pipe (Page 27)
- Fig. 29: License client configuration – expert settings, WCF/TCP (Page 28)
- Fig. 30: License client configuration - expert settings, .net-Remoting (Page 30)
- Fig. 31: License client configuration - basic settings, user-specific (Page 32)
- Fig. 32: License client configuration – connection configuration, same as computer, user-specific (Page 33)
- Fig. 33: License client configuration – connection configuration, pipe, user-specific (Page 34)
- Fig. 34: License client configuration – connection settings, WCF via TCP, user-specific (Page 35)
- Fig. 35: License client configuration - connection configuration, .net-Remoting, user-specific (Page 36)
