---
title: "EN-INST-AW_License_Server"
source: "EN-INST-AW_License_Server.pdf"
tags: ["A+W", "License Server", "Installation", "Software", "Windows", "Setup", "Configuration", "Sentinel", "AnywhereUSB", "Technical Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides detailed installation instructions for the A+W License Server, Version 5 SP4. It covers system requirements, installation procedures, configuration settings, and troubleshooting steps for both new installations and updates. The guide is intended for system planners and administrators responsible for setting up and maintaining the A+W software environment."
long_description: "This is a comprehensive installation manual for the A+W License Server. The document begins by outlining the change history and a general overview of the installation process. It details the specific system requirements, including hardware (such as the mandatory A+W dongle and optional AnywhereUSB devices), network configurations (fixed IP, open TCP ports), and software prerequisites (Windows Server versions, .NET Framework 3.5). The core of the manual is a step-by-step guide for a new installation of Version 5 SP4 using the A+W SetupLauncher. This includes selecting the correct modules, configuring infrastructure services, importing the license file, and setting up optional email notifications for server events. The guide also covers the installation and configuration of the AnywhereUSB driver for virtualized environments. Post-installation topics include checking the installation result, understanding the directory structure, and configuring protocol settings. The manual concludes with instructions for updating and uninstalling the license server, and an appendix on using the License Service Monitor tool to check license status and usage."
---

# Installation Instructions: A+W License Server

---
## Change history:

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2014-07-22 | J. Makowka | Original version | 1.0 |
| 2022-12-08 | B. Hanewinkel | System requirements | 1.1 |

The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:

1. Check the installation requirements.
2. Compile the required data, additional programs, drivers, etc.
3. Note or determine the time required.

## 1. New Installation of Version 5 SP4

The following installation instructions assume that there is no previous version installed.

### 1.1 Overview and the basics

To install the license server, you must have local administrator rights for the machine on which the server should be installed.

The following list provides and overview of the work that must be done during installation:
> Installation of license server using the Setup Launcher. Usually the license server is installed in conjunction with other A+W server components.

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
- Processor: Intel Xeon E5520, 2.67 GHz
- RAM: 4 GB

For an initial or new installation, an installation time of 5 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated. When combined with the installation of other A+W software, the time required for installing the clients' licence is negligible.

#### 1.2.2 Conversion time for data stock

Data is not converted. Therefore no time is required for this purpose.

### 1.3 Requirements

#### 1.3.1 Hardware

The license server can only be operated with an A+W dongle. The dongles are registered to the respective customer. They receive the dongles and related license files (see 1.3.4) from the colleagues in the Sales Support department.

The dongle must be plugged into one of the USB interfaces of the machine on which the license server should be installed. If the license server is installed in a virtual environment, the dongle must be available using the suitable tools. Professional virtualization solutions (VMWare, Hyper-V) do not allow hardware to be put on the virtualization servers and mirrored in the virtual machines. A+W recommends **AnywhereUSB von Digi** for the provision of dongles in such environments. This solution has been tested with the license server and is also used in Pohlheim for the house-wide license server. Other options are associated with a higher risk. If the customer uses AnywhereUSB, then he should also install the driver software. The A+W diskset contains a package with the AnywhereUSB driver software, which you can also install yourself if necessary. Please note that in that case you need to determine the IP address of the AnywhereUSB box, this should be ready to hand prior to the installation.

A+W recommends that the machine onto which the license server is installed, and the network hardware that maintains the connection to this server, and possibly the AnywhereUSB box, are operated with an uninterruptible power supply. If these components are lost due to a local power failure, it will result in the loss of the license, and this may lead to significant operational faults.

#### 1.3.2 Network

The server on which the license server is installed must have a fixed IP address. The DNS entry of the server must be correct and must be reliable enough in order to easily cancel it.

The license clients use TCP ports 1572 and 1570 to communicate with the license server. These ports must be opened in the firewall of the machine.

AnywhereUSB (or another USB-over-IP solution) requires a stable network connection between the AnywhereUSB box and the license server.

#### 1.3.3 Software

The license server can be installed on the Windows server systems 2008 R2 or higher. For Windows 10 and Windows 11 there is a limited release: The license server can be used as a local license server for components that also run on the same desktop system.

The license server requires the Microsoft NET Framework 3.5. Please note that the Windows feature .NET Framework 3.5 must be activated on server systems prior to installation. On the Windows server 2012 and 2012 R2, you require the Windows installation medium for this purpose since the installation files for this feature are not installed together with the Windows installation. During installation on these systems, please refer to the corresponding documentation or have the feature activated by a competent IT employee of the customer.

If the customer uses AnywhereUSB, it is best if he installs the driver software for this product in advance and configures the connection to the AnywhereUSB box. You can also do this yourself during the installation. Please note that you will need to have the IP address of the AnywhereUSB box handy for this purpose.

#### 1.3.4 License file

To grant a license, the license server requires a license file with information about the licenses that were purchased by the customer. This license file can be obtained on request (dongle@a-w.de) from the colleagues in the Sales Support department. The license file is created by the colleagues on the basis of the existing system certificates and existing OCs. Please contact the colleagues with sufficient time before the installation in order to obtain the required license file.

#### 1.3.5 Email access

The license server does not have a direct way of displaying information if operations are disrupted. While the corresponding messages are written into the log, the log is rarely viewed on a regular basis, meaning that malfunctions are often only noticed when the licenses can no longer be obtained. Therefore the license server has the option of sending emails in the case of extraordinary operating conditions, so that measures can be taken before licensing is interrupted.

Therefore it is important that you clarify with the customer prior to installation that an email address that the license server can use to send messages will be created. Obtain the access data (mail server, email address, log-in required?, possibly user name, password), and keep it to hand during the installation. Also get the customer to give you the email address of the customer's employee to whom messages from the license server should be sent.

Advise the customer that the program "Albwir.CB.LicenseServices.exe" may have to be registered on the installation machine as an exception in the virus scanner software, so that the system is able to send emails.

### 1.4 Procedure

For the installation, please proceed in the following sequence:

1.  Start the installation of the SetupLauncher from your diskset. Usually, you will only do this once and then install all required A+W packages.
    *(Fig. 1: Start SetupLauncher installation)*

2.  Confirm the administrator rights for the installation.
    *(Fig. 2: Confirm the administrator rights)*

3.  You may receive additional safety information and queries depending on the operating system of the machine and the configuration of the computer. Always confirm with "Continue", "OK", etc.

4.  Wait until SetupLauncher has been installed.
    *(Fig. 3: Example of an installation progress box)*

5.  Click "Next" in the welcome dialog of SetupLauncher.
    *(Figure 4: Welcome dialogue of SetupLauncher)*

6.  This installation description shows you how to install the license server separately from other A+W products. You can also add the license server during the installation of a standard disk .set. In order to do this, simply select the items described below. Create a new diskset. Select "Create new disk set" and click "Next".
    *(Figure 5: Create new diskset)*

7.  In the SetupLauncher, you can now set up the installation plate and hotfix source, execute an FTP download or configure the auto update. This may be important if you are installing the license server together with other A+W products. Please read the documentation for the products that you are installing. If you are only installing the license server, you can leave the dialogue by clicking "Next".
    *(Figure 6: SetupLauncher - System settings)*

8.  The next dialogue shows the installed A+W software. Since this is a new installation, only the SetupLauncher is listed. Exit the dialog using "Next."
    *(Figure 7: Installed A+W software)*

9.  Select the following modules for the installation of the license server:
    -   Under **A+W Common**: "A+W Infrastructure 5 Collector Services", "A+W Infrastructure 5 Middleware", "A+W LicenseServices" and "A+W License Services Monitor"
    -   Under **External Software**: "A+W Sentinel HASP Runtime"
    Add "A+W AnywhereUSB/5 Gen 2" under "External Software" if (and only if) the customer uses AnywhereUSB and has not yet installed the driver software.
    *(Figure 8: License server module)*

10. You are now in the entry dialogue for the infrastructure configuration. Under "Host," enter the name of the server on which the network-wide service locator runs. Please read the installation instructions for the infrastructure services for further information.
    *(Figure 9: Infrastructure configuration)*

11. The SetupLauncher has now collected all required data. Leave the preset selection "Install software and save setup configuration to an XML file" and click "Next."
    *(Figure 10: Start installation)*

12. Now you have to assign a name that will be used to save the disk set for later reference. You can use e.g. "LicenseServer".
    *(Fig. 11: Save diskset)*

13. The following steps are only required if you wish to install the AnywhereUSB driver. If the dongle is plugged directly into the machine or the AnywhereUSB driver software has already been installed, you can skip these steps and continue with step 21.
    Please note that you have approximately two minutes for the installation and configuration of the AnywhereUSB drivers. After that, the SetupLauncher automatically continues with the installation of the next components. If you are not sure that this will be enough time for the installation and configuration, it is recommended that the AnywhereUSB driver software is installed in a separate SetupLauncher session before the actual license server installation. You can also abort the SetupLauncher session by clicking the "End" button.
    Click "Setup" to start the setup for the AnywhereUSB driver software.
    *(Figure 12: Start AnywhereUSB setup)*

14. You will see a command prompt window with information regarding the AnywhereUSB installation. Wait until the window closes.
    *(Figure 13: AnywhereUSB installation)*

15. The AnywhereUSB configuration tool starts automatically. Usually the existing AnywhereUSB boxes will be shown on the left side. But if the selected box is located in another Subnet, it will not be displayed in the list. If the selected box is shown on the list, please continue with step 20. If you cannot see the selected box, click the menu item "Edit" and then "Discovery List".
    *(Figure 14: AnywhereUSB configuration (box could not be found))*

16. In the entry field, enter the IP address of the AnywhereUSB box and click "Add". The address will be shown in the "Discovery Address List". Now click "Close".
    *(Figure 15: Publish AnywhereUSB box)*

17. Now click the "View" menu item in the "AnywhereUSB Remote Hub Configuration Utility" and click "Refresh". This displays the selected AnywhereUSB box. Click "Connect". Close the dialogue when the AnywhereUSB box is displayed as connected (in bold).
    *(Figure 16: ConnectAnywhereUSB box)*

18. Wait while the modules are being installed. You may see additional information and progress boxes during that time.
    *(Figure 17: Installation progress)*

19. This begins the configuration portion of the SetupLauncher session. The configuration tools frequently open up behind the SetupLauncher window. In that case, click on an area in the configuration tool that does not contain any active elements to move the tool into the foreground.
    *(Figure 18: Move configuration tool into the foreground)*

20. You must enter a license file if this is the first time that you are installing the license server on a machine. You have received this license file together with the dongle from the colleagues at Sales Support. If required, Sales Support can also activate Weak Mode in the license file for a limited time.¹ If that is the case, you must also activate Weak Mode by checking "Enable weak mode" so that this mode is actually active. To enter the license file, click on the Browse symbol after the "License file" input field.
    *(Figure 19: License server basic settings)*

    > ¹ **Weak mode** means that for a limited time period, the license server will not pay attention to the number of purchased licenses for certain modules. This mode is used to ensure operability during complex installations without always having to change the license. The license server automatically deactivates Weak Mode after the time period which was defined by Sales Support. Weak Mode allows you to acquire licenses above and beyond those purchased, as well as licenses that were not purchased at all. Weak Mode cannot be activated for A+W Business. While Weak Mode is activated, the system enters a report regarding the licenses not covered by the existing license into the log on a daily basis. If email delivery has been configured, the report is also emailed to the employee who has been entered as the email recipient.

21. Navigate to and select the license file, and then click "Open".
    *(Figure 20: Select license file)*

22. The selected license file is now displayed in the "License file" field. Click "Next" to continue.
    *(Figure 21: License file selected)*

23. Now place a check mark at "Enable mail notifications". Enter the name or IP address of the SMTP server in the field "Mail host [...]", the sender email address in field "Sender address [...]" and the email recipient in the field "Recipients [...]". Separate multiple recipients with semicolons (;). The machine name is already entered in the "Subject prefix" field. The contents of this field precede the email subject line. This makes it possible to allocate emails to the sending license server based on the subject, if one employee is responsible for multiple license servers. If the email server does not require a login, you can now send a test email to the recipients using the "Send test mail" button. Click on "Next" to complete the installation.
    *(Figure 22: email configuration (login not required))*
    If the email server requires a login, place a check mark by "Host requires login". Additional input fields will be shown. Enter the user name in the "User name" field. Use the syntax "<domain>\<user>" when logging into a Windows domain. Enter the password in the "Password" field and enter it again in the "Repeat password" field.

24. The existing version of the configuration tool cannot send test emails if the mail server requires a login. Therefore the "Send test mail" is hidden and a corresponding notification is provided. The license server itself can send out emails even if a login is required. The data that you enter will be saved for the license server, so that emails can subsequently be sent out. Click on "Next" to complete the installation.
    *(Figure 23: Email configuration (login required))*

25. This completes the configuration portion of the SetupLauncher session. Click "Finish" to return to the SetupLauncher.
    *(Figure 24: Configuration completed)*

26. The license server is now restarted in the background. Wait until you see the completion report for the installation, and confirm with "OK".
    *(Figure 25: Completion report)*

27. Terminate the SetupLauncher by clicking "End".
    *(Figure 26: Terminate SetupLauncher)*

### 1.5 Incompatibilities

No incompatibilities are known. The license server uses ports 1570 and 1572, hence they are not available for other software components. If this results in a conflict, you should move the conflicting software to another machine. If such a conflict cannot be solved, please contact the Development department to clarify additional options.

### 1.6 Directory structure

-   The license server saves imported license files in the sub-folder "License/Updates" of its installation folder. The "Feedback" folder contains dump files. The Development department will explicitly ask you for these files if they are required for fault analysis purposes. The "Succeeded" folder contains the successfully imported license files. The name of the sub-folder indicates the date and time at which the license file was imported. License files that could not be imported can be found in the "Failed" folder.
-   The license server uses standard protocolling. The protocol settings are configured with the configuration tool.

### 1.7 Settings

All of the settings for the license server must be applied with the "A+W License Services Config Tool". This tool can be found in the A+W start menu under "Config Tools". The settings that can be applied have already been described in the section on the installation procedure. You can also edit the protocol settings.

#### 1.7.1 Protocol settings

The "A+W License Services Config Tool" has a "Protocol" button, and is therefore distinct from the version that you see during a SetupLauncher session. Click on this button to start the protocol configuration.
*(Figure 27: Start protocol configuration)*

The "License Server" tab contains the settings for the license server functions. Please note that the license server only writes trace messages. Therefore the settings for log messages are irrelevant.
*(Figure 28: License server trace configuration)*

| Category | Description |
| :--- | :--- |
| **AWCHasp** | Entries that relate directly to the communication with the connected dongle |
| **AWCLicenseLegacyObject** | Entries that relate to the provision and function of interfaces for license clients before the 2009 version |
| **AWCLicenseServer** | Entries that relate to the operation of the license server's Windows service and general processes in the license server |
| **AWCLicenseWatcher** | Entries that relate to the monitoring service for the license server |
| **AWCLicensing** | Entries that relate to the direct granting of a license |

The "Basis" tab contains the protocol settings for the Basis libraries used by the license server.
*(Figure 29: Protocol settings for Basis components)*

| Category | Description |
| :--- | :--- |
| **AlbwirBasis** | Entries that relate to general functions in Albwir.Basis, other Basis libraries and entries from program components that do not use their own protocol categories. |
| **[...]** | Entries regarding detailed functions of the Basis libraries. Please change the setting for these categories only if you have been asked to do so by a developer. These categories can quickly lead to very large logs and a significant reduction in disk space. |

### 1.8 Result of the installation

The ability to access the license server from the network must be tested to verify the result of the installation. This can be done e.g. by starting an A+W program on a connected client.

If you are having problems, you can check the connection with the dongle by starting the "SafeNet Aladdin Control Center (HASP Tool)" from the A+W start menu under "Config Tools".

Click on "Sentinel Keys" on the left side of the navigation bar, and examine the view.
*(Figure 30: Check dongle)*

The A+W dongle for the license server is the dongle that is shown with the values "Local" in the "Location" column, and "81178" in the "Vendor" column. If you cannot see such an entry, it means that the connection to the dongle is not working and you must first ensure that the dongle is known to the system.

It might be difficult to identify the correct dongle if several dongles have been plugged into the PC (e.g. if you want to plug it into another PC). You can make the dongle flash by activating the "Blink on" button, so that the correct dongle can now be easily identified.

### 1.9 Configuration

No other configurations are required.

### 1.10 Installation alternatives

There are no available alternative installations.

### 1.11 Uninstalling

You can delete the license server using the "Programs" item in the control panel. If you only want to uninstall the license server, *select/uninstall* the programs "A+W License Services", "A+W LicenseServices Monitor", "A+W Sentinel HASP Run-time" and - if applicable - "A+W AnywhereUSB/5 Gen 2" (in that order).
*(Figure 31: Uninstalling options)*

If you want to delete the entire A+W software, you must also uninstall the programs "A+W Infrastructure 5 Collector Services", A+W Infrastructure 5 Middleware" and "A+W SetupLauncher" (in that order). Please note that these components are also required by other A+W programs. Uninstall the components marked with green arrows only if there is no other A+W software on the machine.

## 2. License server update

The procedure that is used to update the license server is very similar to that followed during the installation process.

The yellow icon in front of the relevant component will tell you if there is an available update for the SafeNet Dongle drivers or the AnywhereUSB drivers. It is recommended that you install the updates on systems as of Windows Server 2008. You should not install the components with Windows servers 2003 R2. You can deselect the components if the check marks were set automatically, and confirm the corresponding warning notification.

The license file must not be indicated during the update installation if there is no new license file. The license server will retain the old license file unless a new one is indicated. All configuration settings that may have been applied along with the configuration tool will also be maintained.

## 3. Appendix

### 3.1 License server monitoring

Tools that can be used to e.g. read out and check a license file are available for the license server environment

#### 3.1.1 License service monitor

The license service monitor provides detailed information on how many licenses are currently assigned for which modules.

On first start-up, the license service monitor will try to establish a connection to the license service. In this context, the connection settings that have been set for the entire computer will be used. If the license service can be reached, the assigned licenses will be queried and displayed in the license service monitor. If the service cannot be reached using the computer-wide settings, then the license service monitor will display the "Server Settings" dialogue.
*(Figure 32: Lizence service monitor - Settings)*

The license service to be queried must first be set up in this dialogue. One of three communication types can be selected using the Connection selection menu:
-   **WCF-Communication via Pipe.** This connection type is preferred if the license service is used by the local computer (as of 2009 version).
-   **WCF-Communication via TCP.** This connection type also only works with license servers as of version 2009. But this concerns the license service on an uninstalled computer.
-   **.Net Remoting.** This connection type should be avoided, since it is designed for older license services (up to 2009 version). Version 2009 or higher has to use one of the first two options.

This pop-up window can be activated with the menu item "Actions → Set server" or the ALT+R hotkey.

Usually this only requires you to enter the host name or IP address of the server on which the license service is operated. If the port or the name under which the license service is contracted must be changed, you must first check "allow modification" after the corresponding entry. The entry can now be modified.

The license information from the license service can be triggered through the menu "Actions → Refresh data" or the F5 hotkey after setting the service parameters. The Explorer view that contains the license information is displayed. The branches of a view tree can be opened by clicking on the "+" symbols. (Opened branches can be closed again by clicking on the "-" symbol.)
*(Figure 1: A+W license service monitor)*

Since the licence service monitor shows the licences defined in the licence server no matter whether one of them is being used at present, it has to check this information with the licence server before displaying it. This involves the transfer of a fairly large amount of data (depending on the size of the license file). Only the assignment of licenses will be changed. Only values for licenses will change. The licence service monitor therefore calls for the licence information in certain intervals (currently every 10 min).

The menu item „Refresh licenses“ in menu „Actions“ (Ctrl+F5) calls again for the entire licence information. Therefore, if you want to review the new license situation after a license update, you have to retrieve the new data from the license service using the shortcut Ctrl+F5. Starting with the 2009 version, the tool offers the option of activating a timer. In this case the program will retrieve the license data from the server at regular intervals. The pop-up window for this setting can be displayed using the hotkeys Alt+P or the "Actions → Preferences" menu. In addition, you can also use this area to define how the modules should be sorted in the Explorer view. Users can select from two options: sorting by module name or sorting by module ID.
*(Figure: 2 A+W license server monitor - Preferences)*

The 2009 license service provides additional information: the assembly versions of the server and a list of loaded assemblies. Now the information can be released with the license service monitor (as of 2009 version). The assembly versions are displayed using the "Actions → Server Information" menu or the Alt+I hotkey.
*(Figure: 3 A+W license server monitor - Assembly versions)*

The dialogue with the loaded assemblies can be displayed using the "Actions → Server Details" menu. The information is saved in a CSV file using the Export button.
*(Figure: 4 A+W license service monitor - Loaded assemblies)*

#### Meaning of Icons in the Tree Structure

| Icon | Description |
| :--- | :--- |
| (Overview) | **Overview of licenses.** |
| (Group) | **Corporate group.** The entry after the colon indicates the name of the group of companies. |
| (Client) | **Client.** The entry after the colon indicates the name of the client. |
| (Workstation) | **Work station.** Logical work station name for licensing. If fixed licences are allocated, this is the „workstation name“ defined by F&A when creating the license. This name is not necessarily identical to the computer name. The "[Default]" entry lists all floating licenses. |
| (Application) | **Application.** The name of the application - if known - is shown after the colon; ex. capacity planning. The application ID is added in round brackets. |
| (Edition) | **Edition.** Edition of application (e.g. "Evolution"). |
| (Version) | **Version.** The number of the licensed version is displayed after the colon. |
| (Business Area) | **Business area.** Corresponds with the classification criterion in the CommonBase ("Business Area"). |
| (Module) | **Module.** In the case of modules for which licenses have been currently assigned, the number of assigned licenses as a proportion of the number of existing licenses is shown in square brackets before the entry. E.g.: <4/250> means that 4 out of 250 available licenses have been assigned. "Session" refers to session-based licensing², while "Instance" refers to instance-based licensing². "Licenses" shows the total number of available licenses. |
| (Options) | **Options.** This item lists the options that are available for the license (if applicable). |
| (Sessions) | **Active sessions.** This item lists the sessions that used at least one of the existing licenses at the time of the query. The items that are listed are the name of the machine ("Machine name="), the session ID ("session="), the user name ("user=") and the number of requested licenses ("allocated="). |

> ² In the case of "session-based" licensing, any number of instances of a module only use one license, if they are started in a joint session. In the case of "instance-based" licensing, each started instance of a module uses a license, even if several of them are running in the same session.
> ³ On the aforementioned systems the session ID will be 0 if they are console sessions.

To save the present state of occupied licences and display the saved data, Version 2009 includes export and import functions. These functions are found in menu "File". The entry **Export** can be used to export the licence data and the occupied licences. The same is achieved by means of the hotkey Ctrl+S. Dialogue "Save" appears from which you can select the target directory for the XML file. These data can be displayed on another computer as well as on the same one by means of the import function. Just click on the hotkey Ctrl+O or menu "File -> View exported File".
*(Figure 33: License server monitor - Explorer view with imported data)*

#### Background Color Meanings

The background colors in the tree structure provide information about the use of the license. The following colors may be used:
-   **White**: No license is in use if an entry in the tree structure is highlighted in white.
-   **Light green**: If an entry in the tree structure is highlighted in light green, less than 90% of the available licenses are in use.
-   **Light yellow**: If an entry in the tree structure is highlighted in light yellow, more than 90% of available licenses are in use or only one additional license is available.
-   **Light salmon color**: If an entry in the tree structure is highlighted in a light salmon color, all licenses have been used up. If the entry is followed by a date in square brackets, then the license has expired for this application.
-   **Bright purple**: If an entry in the tree structure is highlighted in bright purple, more than the allowed number of licenses are in use. That may be the case if Weak Mode has been activated.

The status line at the bottom of the view displays information about the current connection. This information includes the host name or IP address, the port number of the connection, the service name, information whether a connection exists ("connected") and information whether the connection is working properly ("healthy").
