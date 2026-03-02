---
description: "EN-INST-AW_Business"
---


# Installation Instructions A+W Business 6

---
## Change history:

| Date | Edited by | Remarks |
| :--- | :--- | :--- |
| 2012-01-13 | André Münch | Original version |
| 2014-03-25 | Alexander Weil | Cl adjustment |
| 2014-07-09 | André Münch | Adjustment SP4 |
| 2015-01-12 | André Münch | Adjustment of SQL Server authentication (1.7.4) |
| 2015-01-12 | Sebastian Weil | Adjustment of eDocPrinter installation |
| 2015-07-17 | Dirk langsdorf | Addition of hosts and group guidelines |
| 2015-12-01 | André Münch | Version 6 |
| 2017-11-01 | André Münch | Automatic installation Unify TD 6.1 EMP |
| 2021-03-16 | D. Langsdorf | Determine .Net Framework versions |

This document enables the competent reader to install the described software. You should generally stick to this procedure:

1. Check the installation requirements.
2. Compile the required data, additional programs, drivers, etc.
3. Heed or determine the time required.

## Content

- **Installation Instructions**
- **A+W Business 6**
- **1 New installation of Version A+W Business 6**
    - 1.1 Overview and the basics
        - 1.1.1 Mixed installation A+W Business 6 with old production software
    - 1.2 Time requirement
        - 1.2.1 Installation time for the software
        - 1.2.2 Conversion Time for Data Set
    - 1.3 Requirements
        - 1.3.1 Hardware
        - 1.3.2 Network
        - 1.3.3 Operating system
    - 1.4 Procedure
    - 1.5 Incompatibilities
    - 1.6 Directory structure
    - 1.7 Settings
        - 1.7.1 Edition for the license query
        - 1.7.2 Customer-Specific Configuration
        - 1.7.3 Settings in the SQL.INI
        - 1.7.4 SQL Server authentication
    - 1.8 Result of the installation
    - 1.9 Tips and tricks
        - 1.9.1 FAQS
        - 1.9.2 Known errors and workarounds
        - 1.9.3 SQL Server performance problems on login
        - 1.9.4 SQL Server performance through DNS server
    - 1.10 Uninstalling
- **2 Update to version A+W Business 6**
    - 2.1 Overview
    - 2.2 Time requirement
        - 2.2.1 Installation time for the software
        - 2.2.2 Conversion Time for Data Set
    - 2.3 Requirements
    - 2.4 Procedure
    - 2.5 Incompatibilities
    - 2.6 Directory structure
    - 2.7 Settings
        - 2.7.1 Parameters
        - 2.7.2 Customer-Specific Configuration
        - 2.7.3 Registry
    - 2.8 Result of the installation
    - 2.9 Alternative Installations
    - 2.10 Patches
    - 2.11 Tips and tricks
    - 2.12 Uninstalling

## 1 New installation of Version A+W Business 6
The following installation instructions assume that there is no previous version installed. The set-up and configuration are described in the configuration instructions.

### 1.1 Overview and the basics
The following list provides an overview of the work that must be done during installation:
- Installation of .Net Runtime 3.5
- Installation of all components via the SetupLauncher
- database client Unify SQL Base 11.6 or Microsoft SQL Server 2012 R2 Native Client. Installation of both clients is possible.

The .Net Runtime 4.8 must be installed, it is deployed by the Setup Launcher.
[https://docs.microsoft.com/de-de/dotnet/framework/migration-guide/how-to-determine-which-versions-are-installed](https://docs.microsoft.com/de-de/dotnet/framework/migration-guide/how-to-determine-which-versions-are-installed)
This link explains which frameworks are installed.

#### 1.1.1 Mixed installation A+W Business 6 with old production software
Essentially it applies that for the installation of A+W Business 6, the 6 components of CAD Designer must also always be installed.
This means that for mixed installation (e.g. including A+W Production 5 or ALCIM 2011), the latest main installation defines the elements to be used.
This is essentially no problem since the components are always upward compatible.
Here you must heed that the same CAD version is used in the entire operation since an older CAD version cannot process files from a newer version.
Only this way can you ensure that the SN files from A+W Business 6 can also be read in A+W Production 6.

### 1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data: the first or new installation of A+W Business 6 and the accompanying software installed by the setup takes approx. 60 minutes per workstation.

#### 1.2.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
- Prozessor: Intel Core i7 8770 @2,93GHz

For an initial or new installation, an installation time of 60 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated. If the .NET Framework 3.5 is already installed with Service Pack 1, the installation will take much less time.

#### 1.2.2 Conversion Time for Data Set
The duration of the database update on the server depends on the size of the database, the size and number of archive databases, and the hardware equipment of the server. Therefore, it can vary significantly.
For the migration, all data records in the source database must be read in and stored in the target database. This is done using normal SQL commands. The porting of a 815 MB database on a virtual PC with 2.4 GHz requires approximately 15 minutes. A data migration with switched-on Unicode option on the same system requires approximately 20 minutes. From this, a factor of approximately 25% arises with respect to a non-Unicode to Unicode porting. However, this applies only for the server; no conversion is required on the clients.

### 1.3 Requirements
The .NET Framework 3.5 must be installed, this is not done through the setup.
There must be a server available for the A+W license management on which the A+W License Server is installed and configured for the customer. Therefore, during the A+W Business installation, only the License Server Client is installed. For more information about the installation and set-up of the license server, please see the appropriate installation instructions.
In addition, the A+W Infrastructure Services must be accessible.
If A+W Business 6 and A+W Production 6 are installed on one computer, then the terminal server mode of A+W Production 6 and CAD must be activated. SNLive can only work together with A+W Business 6 in this mode.

#### 1.3.1 Hardware
For the hardware prerequisites for an A+W Business 6, please see the relevant specifications.

#### 1.3.2 Network
Network access must be present In addition, the following paths on the server must be enabled and connected as network drives on the clients:
- the directory in which the A+W Business 6 Setup is located
- the program directory where A+Business 6 is installed
- the folder for the report files

#### 1.3.3 Operating system
For approved operating systems, please see the release matrix.

### 1.4 Procedure
For the installation, please proceed in the following sequence; this is also specified by the Setup assistant:

1.  Copy the complete contents of the setup CD to a directory on the server. Do not delete this directory after the installation since any updates are installed from this directory. The directory should not be in the Programs folder. It is recommended that you set up a Software/A+W on a separate drive and store the installation packages in the subdirectory 6. The A+W directory should then be set up as release. In the SetupLauncher, this drive should be used via a UNC path.

2.  Start the "SetupStarter.exe" in this directory. This setup installs the Albat+Wirsam SetupLauncher for the current user. The user should have administrator rights. After the installation, the SetupLauncher starts automatically. For operation of the SetupLauncher, please see the appropriate document. Knowledge of the operation is assumed as a precondition.

3.  For an A+W Business 5 Client installation, the diskset "A+W Business Terminal Server" should be selected in the SetupLauncher.

4.  For an A+W Business 5 Server installation, the diskset "A+W Process Server" should be selected in the SetupLauncher.

5.  **Selection of the maxx PDFMAILER version**
    For the maxx PDFMAILER, there are a German and English version available in the SetupLauncher. Only one of these versions can be installed.
    > [Screenshot: maxx PDF Mailer selection in Albat+Wirsam Setup Launcher, with options for "English Version" and "German Version".]

6.  **Settings for the A+W Business 6 setup**
    For A+W Business 6, no further settings are required. If several languages are installed together with the A+W Business 6 Server module, the language of the links on the Start menu must be selected for the script management and the database migration.

7.  **Installation of maxx PDFMAILER**
    This installation of the maxx PDFMAILER is done with an external setup, which allows free configuration. The settings should look as follows:
    > [Screenshot 1: maxx PDFMAILER Setup - Registration. The user is prompted to enter Name, Organization, and License. The "Install as Promotion" checkbox is checked.]
    > [Screenshot 2: maxx PDFMAILER Setup - Features Selection. The recommended selection is "PDFMAILER XML STANDARD and PDFMAILER XML PROMOTION".]

8.  **Installation eDocPrinter (alternative to maxx PDFMAILER)**
    During the setup, no special settings must be made. Generally the standard edition (see screen shot) should always be installed. The registration runs via the Devices and Printer menu of the Windows Control Panel.
    > [Screenshot: maxx PDFMAILER Setup - Configuration. Shows the Destination Folder and Printer name settings. The printer name is set to "maxx PDFMAILER".]
    
    In the previous screen shot, you can already see the dialog for configuring the printer settings. Important here is the Links tab. On this tab, you must activate the options marked in red on the following screen shot.
    
    > [Screenshot: eDocPrinter PDF Pro Printing Preferences - Links Tab. The following options are checked:]
    > - `Automatische URL-Konvertierung in PDF-Links` (Automatic URL conversion in PDF links)
    > - `Aktiviere Erkennung lokaler Dateilinks und Konvertierung in PDF-Links` (Activate detection of local file links and conversion in PDF links)
    > - `Aktiviere die Erkennung von 'PDF-Kommandos'` (Activate detection of 'PDF commands')
    > - `Start und Ende Markierung: %%EmailSubject: Betreffzeile ist hier%%` (Start and End marker)
    > - `Entferne Textlinien, die mit einem Kommando-Tag beginnen` (Remove text lines that begin with a command tag)

    In order to be able to use the functionality of the eDocPrinter, A+W Business Reports must be adjusted. An example of this is the reworked version of the report for declarations of performance: `\\hausi\AWDCaseDoc\328\328277\dop.qrp`
    The eDocPrinter can be defined as PDF printer per user after successful installation in the employee management of A+W Business.

9.  **Installation Unify SQLBase 11.6**
    For the installation of SQLBase, you must distinguish between two different modes. For the installation of the drivers in order to configure a connection to a database server, no license is required. For the installation of a database server, you need a product media key from Unify for the SQLBase 11.6.
    For the installation of the A+W Business 6 Demo database, a local database server must be installed or already be installed. The most important installation dialogs are displayed below, what what you must pay attention to on each:
    - As setup type, select the "Custom" method during installation of the SQLBase.
    > [Screenshot: Unify SQLBase 11.6 Setup Type selection, with "Custom" selected.]
    
    - For the installation of a database client, it is sufficient to install the components "SQLBase 32bit Client" and "SQLBase 32-bit Drivers."
    > [Screenshot: Unify SQLBase 11.6 Select Features, showing only "SQLBase 32bit Client" and its sub-components checked.]
    
    - For the installation of a database server, all components should be activated.
    > [Screenshot: Unify SQLBase 11.6 Select Features, showing "SQLBase Server" and all other components checked.]
    
    - (Server installation) For the installation of a database server, you must have a product media code. The database server must have a name.
    > [Screenshot: Unify SQLBase 11.6 Product Media Code entry screen.]
    
    - Next you must select the directory in which the files for SQLBase 11.6 should be installed.
    > [Screenshot: Unify SQLBase 11.6 Choose Destination Location, with default path `C:\Program Files\Unify\SQLBase116\`.]
    
    - (Server installation) If SQLBase is running on a computer on which other interactive programs are running, the "server priority" should be set to "normal"; otherwise this setting should be on "high."
    > [Screenshot: UNIFY SQLBase Advanced Server Options, with Server Priority set to "High (Dedicated Server)".]
    
    - (Server installation) The last setting before the installation is the selection of the directory in which the databases are located.
    > [Screenshot: Unify SQLBase 11.6 Choose Destination Location for database files, with default path `C:\ProgramData\Unify\SQLBase116`.]
    
    - After the installation, you must only ensure that the SQLBase installation is added to the path variables. A correct functioning is only guaranteed with this entry.
    > [Screenshot: Question dialog asking "Add SQLBase to the windows PATH (recommended)?".]
    
    After the installation, be sure to check whether the path exists!

10. **Configuration of SQLBase client/server**
    The first step of configuration is the setting of the database connection. On this dialog under SQLBase -> TCP/IP, you must set the database where the database is located.
    > [Screenshot: Unify Connectivity Administrator showing the tree view to configure a TCP/IP connection to the ALFAK database.]

11. **Configuration of A+W Business 6**
    The second step of the configuration is the setting of the A+W Business 6 settings. With the help of the configuration dialog, the following settings can be made:
    - I. The path for the A+W Business 6 installation is entered in the system path variables.
    - II. The file types for the A+W openTrans documents (electronic order confirmation, invoices and delivery notes) are set so that they start the import program automatically with a double-click on the files.
    - III. The settings for the logging are made. On the first dialog, you can completely deactivate the logging for the components A+W Business, GetFrm, and SNLive.
    - IV. The description of the "Use SQL Server Authentication" switch is found in Chapter 1.7.4.
    
    > [Screenshot 1: A+W Business 5 Configuration showing the "Settings for all users" tab. Option "Use SQL Server Authentication" is visible.]
    > [Screenshot 2: A+W Business 5 Configuration showing the "Log Configuration" tab with settings for Trace Level and Log Level for various components.]
    
    On the second page of the configuration program, you can make the setting for the A+W Business 6 Trace.

12. After the installation, the EMPs for Unify SQLBase may need to be installed. It is in the installation directory (e.g. `\\jupiter\SW_INSTALL\2012\Diskset\Unify SQLBase 11.6`). Only the last EMP must be installed. With the release of a new service pack for this modules, the EMPs must be removed again before the ServicePack can be imported.

> **In this case, Development recommends a complete uninstallation and reinstallation since under some circumstances during an update, it is possible that not all components are replaced.**

### 1.5 Incompatibilities
No incompatibilities are known.

### 1.6 Directory structure
The user does not have to create anything.
The setup must be copied from the CD before the installation to an approved directory on the server.
The program creates the directory structure of A+W Business 6 in the selected target directory (default: in the Program directory in the Business 6 subfolder).

### 1.7 Settings

#### 1.7.1 Edition for the license query
The edition that should be installed on the customer system must now be set with the help of the script management. The set edition is saved in the database and later used by A+W Business in order to request the license from the license server. If the set edition does not correspond to the license file of the license server, then it is not possible to start A+W Business.
> [Screenshot: Script management tool showing an "Edition" dropdown set to "Standard".]

#### 1.7.2 Customer-Specific Configuration
If the customer uses a product identifier (CEKAL classification or quality identifier), then this must be set in the company data. In earlier versions, this was determined by two entries in the license file. The license check is still done, however, the handling via the switches in the company master data is easier.
> [Screenshot: Company data settings screen showing the "Produktkennzeichnung" (Product Identification) section with "Aktive Kennzeichnung CEKAL-Klassifizierung" selected.]

#### 1.7.3 Settings in the SQL.INI
After the installation of SQLBase 11.6, the following entry in the section [dbntsrv] must be checked in SQL.INI:
`usecmcache=0`
With this entry, "Corrupt index" errors in the database are prevented.

#### 1.7.4 SQL Server authentication
Starting with version 12.5, SQL Server authentication is available as an alternative to Windows authentication for SQL Server. So that this works, you must take the following steps:

1.  The user must be created on the SQL Server. You can choose the password freely. The user must receive the required rights for the database via his rights or a separate assignment to the database.
2.  In the A+W Business Config Tool, the SQL Server authentication can be activated and the user and password stored. This setting applies for the current computer.
3.  The same setting is used for those services that are used on this computer. Special configuration is no longer necessary.
4.  The ALFAKUSER application role is not used in this case.

### 1.8 Result of the installation
If A+W Business 6 can be started and the database connection works, an order should be entered and the shape or processing view tested using the shaping nesting. If this all works perfectly, the installation was successful.

### 1.9 Tips and tricks

#### 1.9.1 FAQS

1.  **If I display muntins in the ALFAK muntin entry starting with version 2009, I do not see an AWDesign picture. The screen remains white. What can I do?**
    - For visualization, AWDesign needs a current version (at least October 2007) of the GETFRM32.DLL. How many GETFRM32.DLLs are on the computer? The latest version should always be first in the system path.
    - Is AWDesign registered as a COM object? Example: with `C:\Program Files\A+W\Techsoft\AWDeisng\awd20.exe / regserver`, it is possible to register after the fact.
    - Is the XOPTFRM environment variable in the system variables correct (Start-->Settings-->Control Panel-->System-->Expanded-->System Variables)? Is the path that is entered there reachable? Default value is: `C:\PROGRA~1\A_W~1\Techsoft\SHAPES\FRM` (in 8-bit form)
    - With a call of the muntin sketch (entry or print), there is a message box from AWDesign with the message "Creation of file INDEX.TAB not possible." You must check whether the Windows user has full access to the following path (installation directory AWDesign) : `"C:\Programs\A+W\Techsoft\AWDesign\AWDESIGN\MACRO"`. If this is the case, the following must be entered in awd20.ini (in the installation directory of AWDesign):
        ```ini
        [AWDESIGN]
        MacroFileLocation=$USER$\AWDesign\Macro
        ```

2.  **For the output of the forms on the gotomaxx PDF-mailer, the mail client always opens and the mail address of the recipient is missing, although a mail address was entered in the document.**
    The PDF mailer reads the control commands only starting with a particular distance from the upper paper edge. Therefore, in the ReportBuilder using the "Report-Format-Report" menu element on the "Page Layout" tab, the page margin top must be set to at least 0.7.

3.  **How can I register all COM objects after the fact?**
    Starting with version 2009, the file "RegisterCom.exe" with which all objects are registered exists in the `\Config\` folder.

#### 1.9.2 Known errors and workarounds
For the installation of the license client, you must pay attention that all user have write access to the cryptography folder `%appdata%\Microsoft\Crypto\RSA` (e.g. C:\Documents and settings\All users\Application data\microsoft\crypto). This can be achieved if the user "every" is given full rights to this folder.

#### 1.9.3 SQL Server performance problems on login
If the login to the SQL Server takes a long time, this problem can be eliminated with a change of group guidelines. Call of the group guidelines and deactivation of the multicast name resolution.
> [Screenshot: Local Group Policy Editor.]
> The setting to change is located at: `Computer Configuration` -> `Administrative Templates` -> `Network` -> `DNS Client`.
> The policy is "Turn off multicast name resolution". It should be set to `Enabled` to resolve the performance issue. The screenshot shows it as "Disabled".

#### 1.9.4 SQL Server performance through DNS server
In the file `hosts`, enter the computer names of all participating servers. Thus the DNS name resolution is worked around. If this should be the problem on the network. However, this measure should only be temporary until the problems have been eliminated. However, it can be useful in order to prove that the software is not the problem.

### 1.10 Uninstalling
In order to uninstall the software, in the Control Panel - Software, you must just select the "A+W Business 5" entry and click "Remove"; this starts the uninstallation.
You only have to uninstall during an update to a new version, otherwise this is not necessary.

## 2 Update to version A+W Business 6
The following installation description only describes the points that differ from the full installation described above and that must be heeded for an update.

### 2.1 Overview
(No specific details provided, refers to new installation)

### 2.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 2.2.1 Installation time for the software
Based on the version [n-1], the program can be installed on the reference device in approx. x minutes.

#### 2.2.2 Conversion Time for Data Set
The installation time for the different computers depends on the computer type, storage space, and configuration. The conversion time specified was determined using a reference device with the following characteristics:
- Processor:
- RAM:
- Miscellaneous

For the required data conversion, a time of approx. 30 minutes plus 1-2 minutes per GB must be calculated (depending on computer performance).

### 2.3 Requirements
See new installation.

### 2.4 Procedure
1. First the new version A+W Business 5 should be installed.
2. After successful start-up of A+W Business 5, the preceding version should be uninstalled.

### 2.5 Incompatibilities
See new installation.

### 2.6 Directory structure
See new installation.

### 2.7 Settings
The existing settings are taken over unchanged. You may only have to adapt the new switches.

#### 2.7.1 Parameters
See new installation.

#### 2.7.2 Customer-Specific Configuration
See new installation.

#### 2.7.3 Registry
See new installation.

### 2.8 Result of the installation
See new installation.

### 2.9 Alternative Installations
None.

### 2.10 Patches
(No specific details provided)

### 2.11 Tips and tricks
See new installation.

### 2.12 Uninstalling
See new installation.
