---
description: "EN-INST-AW Business Production Manager 4"
---


---
## 7 Uninstalling
Use the OS control panel to uninstall the software.

## 8 A+W iCut

### 8.1 Prerequisite

#### 8.1.1 Software
A Windows 10 or Server 2019 installation is the prerequisite for the installation of A+W iCut.

**Creating a diskset**
The installation diskset can be generated with the batch `GetAWiCutComplete.cmd`; this way, all A+W modules are available for a successful installation.

> **File Directory Example:**
> ```
> Netzwerk jupiter SW_Install
> ├── 2009
> ├── 2011
> ├── 2012
> ├── Hotfix
> ├── Tools
> ├── v6
> ├── CopyUpdates.cmd
> ├── GetALCIB2009Frontend.cmd
> ├── GetALCIB2011Frontend.cmd
> ├── GetALCIM2009Complete.cmd
> ├── GetALCIM2011Complete.cmd
> ├── GetAWB6Complete.cmd
> ├── GetAWE5Frontend.cmd
> ├── GetAWE6Frontend.cmd
> ├── GetAWiCutComplete.cmd  <--
> ├── GetAWProduction5Complete.cmd
> ├── GetAWProduction6Complete.cmd
> ├── GetClaritySuiteFrontend.cmd
> └── GetRequirements2009.cmd
> ```

**The Microsoft .NET Framework 3.5 has to be installed !!!**
```
Dism /online /enable-feature/featurename:NetFx3 /All /Source:D:\sources\sxs /LimitAccess
```
The directory `D:\sources\sxs` has to be adjusted to suit the Windows installation medium.

The Windows network search and file release have to be activated; otherwise no release drive P: can be attached.

> **Advanced sharing settings**
>
> Under the `Domain (current profile)` section, ensure the following options are selected:
> - **Network discovery**: `Turn on network discovery`
> - **File and printer sharing**: `Turn on file and printer sharing`

#### 8.1.2 Modules of the license server
The following modules play a role for A+W iCut; these have to be released in the Edition Startup on the license server. The production modules have to be enabled in the standard edition.

| Module | Application | Edition | Name | Price list no. | Add-on module |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | ALFAK(300) | Startup | Basic module A+W Business | 235001 | No |
| 143 | ALFAK(300) | Startup | Basic module Production Manager | 235001 | No |
| 11 | ALFAK(300) | Startup | EDI Import | 240011 | Yes |
| 156 | ALFAK(300) | Startup | Excel Import | 240018 | Yes |
| 140 | ALFAK(300) | Startup | Barcode Manager (EL) | 240101 | Yes |
| 52 | Planedit | Standard | Planedit | | No |
| 1 | XOPT-Opti | Standard | XOPT-Opti | | No |
| 2 | XOPT | Default | XOPT | | No |
| 4 | XOPTS | Default | XOPT/S | | No |
| 1 | XOPTS SHAPENESTER | Default | A+W Shape Optimizer | 240115 | Yes |
| ? | | | Machine driver | | |

## 8.2 Installation SQLServer Express and the database
Please perform the installation with the SQLServer 2019 Express or newer.

> **SQL Server Installation Center**
>
> 1. On the `Installation` tab, select:
>    - `New SQL Server stand-alone installation or add features to an existing installation`
>
> **Instance Configuration**
>
> 2. Select a `Default instance`.

Install the SQL Server as mixed mode installation and give the current user the administration rights via the SQL Server.

> **Database Engine Configuration**
>
> 1. On the `Server Configuration` tab, set the Authentication Mode to:
>    - `Mixed Mode (SQL Server authentication and Windows authentication)`
> 2. Specify the password for the SQL Server system administrator (sa) account.
> 3. Add the current user as a SQL Server administrator by clicking `Add Current User`.

Now install the SQL Server management tool; the call causes a download of the installation package.

> **SQL Server Installation Center**
>
> 1. On the `Installation` tab, select:
>    - `Install SQL Server Management Tools`
> 2. Do the download and execute the EXE.

> **Management Studio (SSMS) Download**
>
> 1. From the Microsoft download page, click the link to `Download SQL Server Management Studio (SSMS)`.
> 2. Run the downloaded `SSMS-Setup-ENU.exe` file.

Now you can log onto the SQL Server, either via the Windows login or the "sa" authentication.

> **Connect to Server**
>
> - **Server type**: Database Engine
> - **Authentication**: Windows Authentication (or SQL Server Authentication with user `sa`)

Please install the databases for your selected language for A+W iCut.

> **Restore Database**
>
> 1. In SQL Server Management Studio, right-click on `Databases` and select `Restore Database...`.
> 2. In the `Source` section, select `Device` and browse to the backup file location.
> 3. Select the appropriate language backup file (e.g., `ICUT_ENG.bak`).
> 4. Click `OK` to restore the database.

Thus the SQL Server installation is completed and the database for A+W iCut is present.

## 8.3 Installation of the software with the A+W Setup Launcher

### 8.3.1 Creating the fingerprint for the soft lock
Download the SoftlockPreparePackage.zip and unzip it.
`\\jupiter.a-w.intra\Doku DocuWare\AWEnterprise\LicenseServer\!General\FAQ Tips Tricks\Softlock`

Start a command shell as administrator and execute the file "StartPrepare.cmd."

If there are problems, perhaps you need a newer version of the "Sentinel HASP installer." You can download this from the manufacturer.
`https://www.sentinelcloud.com/minisites/SRM/Downloads.aspx?s=&c=all&p=Sentinel+HASP&o=all&t=all&l=all`

The `haspdinst.exe` has to be stored in the "SoftlockPreparePackage\Driver" subdirectory.

During the installation, the fingerprint file of the computer can be generated. Using this, the license for this computer can be issued.

> **A+W Softlock Tool Fingerprint Collection**
>
> This tool assists in creating an exchange file with the machine information needed to create a new A+W Soft Lock.
> - Fill in the `Customer`, `Your name`, `Site`, and `Your company` fields.
> - Select a destination folder for the exchange file (e.g., `my desktop`).
> - The tool will generate a `.awfp` file (e.g., `icuttest-a-w.intra-200707-0936.awfp`).

### 8.3.2 Installing the Setup Launcher and license server
If you have received your license file, we can begin with the installation of the Setup Launcher and the license server. Execute the `SetupStarter.Exe`.

1.  In the `A+W SetupLauncher`, select the diskset:
    - `A+W License Server`
2.  Click `Next`.

This places the following components on your computer.

> **Component Selection**
>
> The following components will be installed:
> - `A+W LicenseServices`
> - `A+W LicenseServices Monitor`
> - `A+W Distribution for Gemalto Sentinel Runtime`
> - `Microsoft OLE DB Driver for SQL Server`

Please enter the license file in the configuration of the license server.

> **A+W License Server Base Configuration**
>
> 1.  Check the box `Import new license file`.
> 2.  Browse to and select your received license file.
> 3.  Click `Next`.

## 8.4 Installation of A+W iCut software
Start the A+W Setup Launcher again.

1.  In the `A+W SetupLauncher`, choose the installation diskset:
    - `A+W iCut`
2.  Click `Next`.

The following modules are installed by the defined diskset:

> **Component Selection**
>
> The installer will select a predefined set of components, including:
> - A+W Business 6 (Basis, Production Manager, and language packs)
> - A+W Common (CAD Designer, LicenseClient, etc.)
> - A+W Production (Plan Editor 6, Shared Folders)
> - External Software (Gemalto Sentinel Runtime, OLE DB Driver, etc.)

> **A+W Business 6 Setup**
>
> - **COM Credentials for Service Backends**: Specify a Windows user account (e.g., `icut`) under which the Business Com Object will run.

Here, the specification is made of the user under whom the COM parts are running. This can be the user who uses iCut or another user with appropriate rights (login authorization).

> **License Client Configuration**
>
> - **License Service**: Select `The license service is running on this machine`.

The license server is running on the PC; for a server installation, this could also be another machine.

> **A+W Business 6 Configuration**
>
> - **SQL Server database connection**: Select `OLE DB Provider (recommended)`.

Here, the recommended OLEDB Provider should be selected; it is also selected in the diskset.

The user has to be specified for the Exchange Windows Service; he receives the "Windows Service Logon" authorization.

> **AWSOA Service User**
>
> - **User**: Specify the user to run the AWSOA Services (e.g., `ICUTTEST\icut`).

The Windows Service is installed and started. It executes the workflow. In the Windows Services list, you will see `A+W Commercial 6 Exchange Windows Service` running with a Startup Type of `Automatic`.

## 8.5 iCut activation in script management
The activation is done in the script management by setting the edition to "iCut."

> **ICUT60 Tool**
>
> 1.  Open the ICUT60 tool.
> 2.  In the `Edition` dropdown, select `iCut`.
> 3.  The tool will then process the necessary scripts.

On the next start of A+W iCut, the license of the edition "Startup" is queried and the license file must be ordered accordingly. It is important that at least the module 1 and 143 in the "Startup" edition are released. All other modules are limited by the program or are additional modules (see also 8.1.2).

The display of the license in the license manager looks like this:
> **A+W License Monitor**
>
> The monitor will show the active licenses for the workstation. Key applications include:
> - **Application: ALFAK (300)**
>   - Edition: Start-up
>   - Module: 1 ALFAK 2000 Basisversion Verkauf
>   - Module: 11 Connect II (Datenimport...)
>   - Module: 140 Barcodeloesung
>   - Module: 143 Business Pro

## 8.6 MDI window and the main menu
In A+W iCut there are two user groups, the standard users and the XTV users. The standard users (operators) work in the office and can, for example, edit products, enter orders, approve batches for the production manager, etc. The XTV users, by contrast, work on the cutting table. In the Production Manager, there is an XTV mode and in this mode, users can only display optimization (cutting plan) and remove stockplates. For this reason, depending on the group to which a user belongs, the main menu in A+W Business is displayed accordingly.

The other tool dialogs such as the "Last used" – tool are not available in A+W iCut. Furthermore, some functions are deactivated in the edition.

## 8.7 Master Data

### 8.7.1 Customers
In the customer management, only the fields for the definition of the address are available. All others are deactivated, just like the functions that you can call from the menu.

### 8.7.2 User rights
In the management of the user rights, only the programs are displayed that are available in this edition. Adding new rights also only works for the selected programs.

### 8.7.3 Number ranges
In the number ranges, you can specify ranges for orders and S+N file numbers. No other areas can be edited. Furthermore, you can define the ranges only for the standard scheduling range `<n.e.>`.

### 8.7.4 Product Management
In product management, only existing products can be changed, the tabs 3 and 12 were deactivated, there are no prices and also no technical parameters (service description).

For the following product groups, a new creation of products is permitted:
- "001 - Single glass” / “011 - Single glass"
- "002 - TG" / "018 - TG”
- "003 - LG" / "020 - LG”

## 8.8 Documents

### 8.8.1 Number manager
In the number manager, you can only copy or overwrite a number manager. Furthermore, you can make a status change and display the currently selected document. The scale drawing can no longer be called from the number manager in this edition.

### 8.8.2 Document entry
It's only possible to enter orders. Furthermore, the total tab is deactivated and there is no price calculation in the item entry. But for the history, status change, and selection of the number manager, all functions are deactivated. Only the first tab of the header entry is active.

In the item entry, it is not possible to select the columns in the table. You can only enter edge processings, steps, and shapes. The creation of texts is also possible. If the item entry is ended, the program changes back to header entry.

In the item entry remain only 1=item, 2=BOM, 3=shapes and processings, and 8=texts active. Only edges, steps are allowed as processings.

### 8.8.3 Form printing
The form printing can be started from the main menu or as direct printing from order entry and be done from the number manager. It is only an order confirmation and a production paper can be printed. The printouts are generated via Gupta Reports. Crystal Reports is not supported.

### 8.8.4 Archive transfer
In the transfer to the archives, it is only possible for the user to delete orders from A+W Business and to remove flows from the production manager via defined workflow task.
No archive databases are required for A+W iCut.

### 8.8.5 Exchange Service
The Exchange Service and the infrastructure are not installed. The A+W Commercial 6 Exchange Windows Service takes their place.
This Windows service executes the workflow tasks defined in A+W Business, such as the archiving of production manager batches.

For this, a formula (`Company` > `Formulas`) that calls the function `udf_TransferEndOfDayProdManager()` has to be defined at the start.
```vb
! *************************************************************************************
! ** Removes jobs and optimizations from Production Manager tables (PROD_*) **
! *************************************************************************************
udf_TransferEndOfDayProdManager();
```
Then you change to the Customizing program (`Company` > `Customizing`) and create a new workflow task with this formula. Now you have to specify how and when this task should be executed.

> **Autom. Process Execution**
>
> - **Workflow Task**: 1 - Archiving jobs
> - **Execution**: Cyclic
> - **Sequence**: e.g., `00:05` (every 5 minutes)

As already mentioned, the execution will be taken over by the Exchange Windows Service. And on the tab `5. Monitor`, you can verify the result of the execution.

#### 8.8.5.1 Config Tool
In order to specify the Trace Level for the Exchange Windows Service, you have to use the A+W Commercial 6 Exchange Windows Service Config Tool.
Here you select the Commercial Exchange Service and click Protocol. Then you can define the trace and log level.

### 8.8.6 Data back-up
This has to be done by the planning via script.
