---
description: "EN-INST-AW_Infrastructure_BasicData"
---


# Installation Instructions: Infrastructure and Basic Data Services

---
## Change history:

| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2014-06-05 | D. Langsdorf | Release version | 12.4.0 |
| 2014-06-10 | D. Langsdorf | Preparation of Informix | 12.4.1 |
| 2014-07-09 | D. Langsdorf | Adjustment for Informix | 12.4.2 |
| 2014-09-16 | D. Holzapfel | Requirements for domain user removed | 12.4.3 |
| 2014-10-17 | D. Holzapfel | User input entered | 12.4.4 |
| 2016-02-17 | D. Holzapfel | Update of installation instruction | 13.0 |
| 2016-02-29 | J. Schmidt | Worflow Designer | 13.0.1 |
| 2017-10-25 | D. Langwald | Adjustment v6.4 and expansion part INFORMIX | 13.4.0 |
| 2017-12-06 | D. Langwald | Note INFORMIX Client Version | 13.4.1 |
| 2022-06-22 | A. Weil | Workflow Dialog Infrastructure.Web Multisite | 13.4.2 |

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## Content

*   **Installation Instructions... 1**
*   **Infrastructure and Basic Data Services... 1**
    *   **1 New installation of version... 3**
        *   1.1 Overview and the basics... 3
        *   1.2 Time requirement... 3
        *   1.3 Requirements... 3
        *   1.4 Installation of server components... 8
        *   1.5 Installation of client components... 10
        *   1.6 Call of the application... 11
        *   1.7 Setting up access to the Service Locator... 12
        *   1.8 Incompatibilities... 15
        *   1.9 Directory structure... 16
        *   1.10 A+W Infrastructure Workflow Designer... 16
        *   1.11 Infrastructure.Web – Workflow Management Dialog... 16
    *   **2 Tips and tricks /FAQs... 19**
        *   2.1 The service/node is not displayed in the Service Locator, is red, has yellow?... 19
        *   2.2 Application no longer starts "No switches were loaded for client xxx."... 19
        *   2.3 Check of the accessibility of the standard ports (if necessary, from DMZ)... 20
        *   2.4 Service Locator Administration is not displayed... 20
        *   2.5 CorelceStorm cannot be reached... 21
    *   **3 Uninstalling... 23**

---

## 1. New installation of version

The following installation instructions assume that there is no previous version installed.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:
- Installation .Net Framework 4.5
- Installation Internet Information Service IIS >=8
- Installation of the database client software
- Creation of the database if no inventory database is used
- Installation of the software with the Setup Launcher

### 1.2 Time requirement

The time requirement will be approx. 30 minutes for the creation of the prerequisites and the actual installation. There is no conversion of data stocks.

### 1.3 Requirements

#### 1.3.1 Hardware

Computer with Windows Server operating system Windows Server 2008R2 or higher are approved. In emergency situations and workstation installations will support the installation starting with Windows 7. The latest service packs and operating systems from Microsoft must always be installed.

#### 1.3.2 Network

ICE services communicate via the ports **12000-12007**, which have to be opened in the network. The installation opens these in the Windows firewall of its own accord. If other firewall programs are used, then the ports must be opened manually there.

To download the SQL database scripts via FTP, a connection has to be established to the A+W FTP Service (port 25). Without this connection it is not possible to download the SQL scripts and the locally installed SQL scripts must be used. The connection is configured in the auto update of the Setup Launcher.

#### 1.3.3 Installation account

For the installation, a user with administration rights must be used. If there is a MUI/Language pack installation on the Windows system, for this user the installation language of the system must be set as primary language since otherwise the internal users will not be recognized correctly during the installation of the ICE services (Could not retrieve Security ID for NT-AUTORITÄT\SYSTEM: No mapping between account names and security IDs was carried out.).

*[Image: Screenshot of Windows language options showing how to set a display language as the primary language.]*

### 1.3.4 Software

#### 1.3.4.1 Manual Installation

For configuration of the Windows Server, we recommend that you use our pre-prepared installation scripts: `\\jupiter\SW_Install\Tools\InstallationsSkripts\`

e.g. the script `Install_WindowsServer2016.cmd` if you are using Windows Server 2016.

*[Image: Command prompt window running a PowerShell script to enable Windows optional features, followed by a prompt to restart the computer.]*

##### 1.3.4.1.1 .Net Framework 4.5

The framework is installed automatically by the Setup Launcher.

##### 1.3.4.1.2 Internet Information Service

The IIS (Version 8 or higher) must be installed.

If the .Net Framework 4.5 was installed prior to the IIS, it may occur that the required Asp.Net 4.0 AppPools cannot be created correctly. Please check this in IIS management under the application pools. Normally, this is not necessary.

*[Image: IIS Manager window showing the 'Edit Application Pool' dialog. The '.NET CLR version' is set to 'v4.0.30319'.]*

If this is the case, and .NET Framework Version is not on v4.0.30319, an administrative command line could be used to generate the respective App Pools.
`C:\Windows\Microsoft.NET\Framework\v4.0.30319> aspnet_regiis.exe -i`

If a Windows Server OS is used, the Server Management Tool has to be used.

In the Windows features, the following marked functions must be activated for the IIS. The activation of the WebSocket protocol is optional. With activated WebSockets, the communication between the browser (>= IE10) and ASP.net is executed at the level of the modern and fast WebSocket. Otherwise, less effective methods are reverted to.

*[Image: Windows Server 'Add Roles and Features Wizard' showing required IIS components. The following items under 'Application Development' are checked:]*
- .NET Extensibility 4.5
- ASP
- ASP.NET 4.5
- ISAPI Extensions
- ISAPI Filters
- WebSocket Protocol

#### 1.3.4.2 Windows Server operating system

If the user directly requests the web interface on a Windows Server operating system, the "Internet Explorer Advanced Security Configuration" has to be disabled.

*[Image: Server Manager window showing the 'Internet Explorer Enhanced Security Configuration' dialog. Both options for Administrators and Users are set to 'Off'.]*

### 1.3.5 Databases and clients

The released 32-bit version database clients for INFORMIX, SQLServer, and Oracle are supported (A+W does not support 64-bit database drivers).

It is recommended that you use your own database for AWSOA components. It is possible to integrate this into an existing A+W database, but since some of the AWSOA data is site-spanning, this could cause confusion. We recommend an individual database with the name AWSOA. This database must be created and a database user must be configured for administrative access to the database. The data structure is created by the applications independently if required.

Do not forget to incorporate the AWSOA database into the database back-up and maintenance concept.

If the system is used as an extension for A+W Business on SQLBase for the trace/log mechanism, the necessary databases cannot be integrated in just any SQLBase database. To obtain the log analysis, an SQLServer Express 2012 installation can be performed to install the Sandpiper components.

#### 1.3.5.1 Preparation of SQLServer

Here, only the native client must be installed; there is no need for configuration of the client software. Access can be tested with a file with the extension .udl; these can be created on the desktop and access to the SQL Server tested.

#### 1.3.5.2 Preparation of Informix

> The INFORMIX Client 3.50 is not supported, it causes problems. Please use the client released by A+W with this version, at least version 4.10 TC9X2.

Informix does not support Guids. Since, however, in stock databases a GUID column is also created in existing tables. A function `makeguid` must be installed in Informix. For this, the following steps must be executed before the installation of the infrastructure services:

1.  Create an empty database `AWSOA` and assign administrative rights to a user:
    ```sql
    CREATE DATABASE awsoa IN <DBSpace e.g. alcimsvr> WITH BUFFERED LOG;
    GRANT dba TO "<user e.g. alcimdb>";
    ```

2.  On the database server, copy the file `GUID.BLD` into the directory `"%INFORMIXDIR%\extend\Guid"` or `"c:\Program Files\IBM Informix Software Bundle\extend\Guid"`. The subdirectory `Guid` has to be created.

    The file is a component of the middleware infrastructure and is in the directory `"%PROGRAMFILES%\A+W\Sandpiper1\InfrastructureMiddleware\Informix\x86"`, for 32-bit Informix, or `„%PROGRAMFILES%\A+W\Sandpiper1\InfrastructureMiddleware\Informix\x64“`, for 64 Bit Informix or in directory: `\\jupiter\SW_Install\Tools\InformixGuid`

3.  The file `GUID.BLD` must have set the write-protect attribute.

4.  Define function `MAKEGUID` on AWSOA and on `ALCIMDB` database. The function is in the file `GUID.SQL` in addition to the `GUID.BLD` file.
    ```sql
    CREATE FUNCTION makeguid()
    RETURNING lvarchar
    WITH(VARIANT, PARALLELIZABLE)
    EXTERNAL NAME "$INFORMIXDIR/extend/guid/guid.bld(makeguid)"
    LANGUAGE C;
    ```

5.  After the installation of the function, it should be tested once manually. For a successful test, the call must return a GUID.
    ```sql
    EXECUTE FUNCTION makeguid();
    ```

For database access to Informix, an ODBC connection must be created. This DSN name is used in the Config Tool infrastructure. For this, the INFORMIX client must be configured via SETNET32. If the database is on the same INFORMIX server as the A+W Production database, you can leave the configuration of SETNET32 to A+W Production. During the installation and infrastructure configuration, simply cancel, and after installation of A+W Production, start the infrastructure ConfigTool manually and do the configuration.

#### 1.3.5.3 Preparation of Oracle

For Oracle, the Oracle client has to be installed as well as an ODBC system DSN.

### 1.4 Installation of server components

For the installation, please proceed in the following sequence:

Start the Setup Launcher and select the pre-defined diskset „A+W_Infrastructure Process Server“. An autoupdate installation should be the standard installation method for the infrastructure services. Please read the installation instructions for the Setup Launcher. Check the diskset directory, the installation drive, and the hotfix path for correct values.

The following disksets belong to the package:
- A+W Infrastructure 6 Middleware
- A+W Infrastructure 6 Service Locator
- A+W Infrastructure 6 Services
- A+W Infrastructure 6 Collector Service
- A+W Infrastructure 6 Web
- A+W Infrastructure 6 Workflow Studio
- A+W LicenseClient
- SAP Crystal Reports runtime engine for .NET Framework
- Java 7

Additionally, the database client (SQLServer, INFORMIX or Oracle) is necessary. The appropriate must be selected.

Now the connection to the Service Locator must be configured. For the host, enter the name of the computer on which the Service Locator was installed. The port is always 12000.

*[Image: A+W SetupLauncher 'Infrastructure Configuration' dialog for Service Locator Settings, showing Host and Port (12000) fields.]*

On the next dialog, you can determine under which user the AWSOA services will run. With a click on the Browse... button, the Windows user selection is started in order to make entry easier. A Windows user is necessary, the infrastructure ProcessServer does not work with the local system account.

*[Image: A+W SetupLauncher 'AWSOA Service User' dialog for entering a user and password to run the services.]*

After completion of the installation, the configuration of the components begins. For this, create the database connection first. For AWSOA, it is recommended that you use an individual database, see chapter "Databases and Clients."

*[Image: A+W Infrastructure Config dialog for Database Configuration, showing Type (SQLSERVER), Server instance, User, Password, and Database/DSN fields.]*

On the next screen, you determine whether the required database update files are called up from the FTP or the ones brought out locally are used. With the test button, you can determine whether a connection can be established with the FTP server from this computer.

*[Image: A+W Infrastructure Config dialog for 'Service Configurations', with an option to 'Use FTP download for database update files'. A successful test shows 'The FTP server is reachable from this computer.']*

Thus the installation and configuration is complete and the application can be used.

### 1.5 Installation of client components

During the installation of the server components, all Infrastructure Services were installed on the server, including the Service Locator.

If further computers are equipped with A+W Software, the Collector Service has to be installed on them for the evaluation of the protocols. This has been selected by default as a dependency. The middleware installs itself automatically as a dependency.
- A+W Infrastructure 6 Middleware
- A+W Infrastructure 6 Collector Service

The connection to the Service Locator has to be adjusted here as well (host: name or IP of server on which the ServiceLocator is installed; port always 12000).

During the configuration of the AWSOA service users, a Windows user should also be used.

This completes the installation of the client components. The computer can be evaluated in central protocolling.

### 1.6 Call of the application

The application is installed in the A+W folder and is started with a double-click.

*[Image: Windows Explorer view of the A+W Start Menu folder, with the 'Config Tools' sub-folder highlighted.]*

The sub-folder `Config Tools` contains:
- A+W Infrastructure 6 Config Tool
- A+W Protocolling Configuration Tool
- Service Locator Administration

*[Image: Windows Explorer view of the 'Config Tools' sub-folder, with 'A+W Infrastructure 6 Config Tool', 'Service Locator Administration', and 'A+W Infrastructure 6 Workflow Designer' highlighted.]*

### 1.7 Setting up access to the Service Locator

The AWSOA services can be managed via the Service Locator Administrator, e.g. you can check whether the services were started or you can restart them manually. This tool can be started from any PC on the network and is a component of the A+W Infrastructure Middleware. You connect with the master registry **"AWRegistry"** (case sensitive!) on the server on which the Service Locator (A+W_Infrastructure ProcessServer) was installed.

The first time you enter the Service Locator Administrator, you must establish the connection.

1.  Select "Direct Connection".
2.  Select "Connection to a Master Registry."

    *[Image: IceGrid Admin 'New Connection' wizard showing options for Direct and Routed connections.]*

3.  If the appropriate entry is present in the list of "Discovered Endpoints," it can be selected. If not, continue with "Manual Endpoint" and "A hostname and a port number?"

4.  Access is via host (name or IP server where the Service Locator was installed) and port number (12000), protocol is TCP.

    *[Image: IceGrid Admin 'New Connection' wizard to input Hostname (localhost), Port number (12000), and Protocol (TCP).]*

5.  Now specify a freely-selectable name and password for the connection. For the connection there is no user or password, however you must enter some user name in order to be able to save the connection. If you enter some password, later you will not be asked to enter a password when connecting.

After connecting, the ICE services are depicted in the Service Locator; they can be started and stopped here. However, under normal circumstances this is not necessary, for they start automatically if needed.

*[Image: IceGrid Admin main window showing the runtime components (services) in a tree view. Right-clicking a service shows options to Start, Stop, etc.]*

### 1.8 Incompatibilities

No incompatibilities are known.

### 1.9 Directory structure

The application installs itself completely under `C:\Program Files\A+W\Sandpiper1`

### 1.10 A+W Infrastructure Workflow Designer

Some A+W services use internal workflows. The infrastructure offers management with which you can specify which workflow should be used by which service (endpoint).

If it is necessary to adjust a workflow, the A+W Infrastructure Workflow Designer will also be installed. After the installation, the tool can be started under "Config Tools" on the start menu with a link.

*[Image: Start Menu 'Config Tools' folder with 'A+W Infrastructure 6 Workflow Designer' highlighted.]*

### 1.11 Infrastructure.Web – Workflow Management Dialog

The Workflow Management dialog of the Infrastructure.Web was reworked so that a client (multisite) and token assignment is possible. For a better overview, the dialog now loads all existing workflow assignments from the table: `Core_WFActivityAssignments`.

*[Image: Screenshot of the 'Workflow Management' dialog in the Infrastructure web interface, showing a table of Extension Points, Workflows, and assigned Clients.]*

In addition to the expansion of the overview table, the functions "Add" and "Delete" were included. The dialog starts with both buttons deactivated since you must always mark a row for use.

If you would like to add a workflow, select any extension point and click "Add". The selected row is copied to the first place in the table and can now be changed. After the change, you must click the "Save" button. If saving is successful, a message appears.

If there is an error when saving, because there is an attempt to save a doubled record, for example, a general error message appears and the window has to be reloaded. So make sure you pay attention to what you're configuring.

You can only delete rows that have a client and/or a token since the workflows without client assignment are basic workflows for the services.

**Best-practice multi-client capability:**

If a service should be multi-client capable and load the workflows accordingly, such as A+W iQuote, then you can create the workflows as follows:

| Extension Point | Workflow | Workflow Type | Clients | Token |
| :--- | :--- | :--- | :--- | :--- |
| 0000 - A+W iQuote | iQuote Enterprise | WebConfigurator | | |
| 0000 - A+W iQuote | iQuote Enterprise.test | WebConfigurator | Testmandant | |
| 0000 - A+W iQuote | iQuote Enterprise Groups Extended | WebConfigurator | Hauptmandant (140) | |

We assume that we have 4 clients: main client (140), location East (1140), location West (5140), test client.

- The main client has its own more complex workflow.
- The test client has a test workflow for the test environment.
- Location East (1140) and location West (5140) have no assignment and thus access the basic workflow since both locations want to work the same.

## 2. Tips and tricks /FAQs

### 2.1 The service/node is not displayed in the Service Locator, is red, has yellow?

For this, you must check whether the service nodes are running in the Windows Services. Depending on the original installation, it can be that the A+W Infrastructure 6 service has the addition „Collector" (A+W Infrastructure 6 Collector).

*[Image: Composite screenshot showing the IceGrid Admin on the left with a service node, and the Windows Services panel on the right, highlighting the corresponding running A+W services.]*

### 2.2 Application no longer starts "No switches were loaded for client xxx."

If the first site was entered in the site management, this error occurs sporadically. Please reboot the server, then it will work again. The pages are cached on the IIS and so the newly-created site is not found. Up to now, there is no other solution.

### 2.3 Check of the accessibility of the standard ports (if necessary, from DMZ)

For a quick check of the availability of the AWSOA services, for example from a DMZ, you can start the tool `AWSOA.ServerTest.exe` from the `InfrastructureMiddleware` directory.

The appropriate settings for the establishment of the connection are read from the registry and after that, there is an attempt to connect with the standard port of the Service Locator and service. In addition, it is indicated if there is more than one IP address stored for the DNS name.

If no connection to the AWRegistry or the services is possible, then the port enable of any firewall or the setting of the Service Locator on this machine must be checked.

```
AWSOA.ServerTest
IceHost read from Registry: DIH-Dev13
IcePort read from Registry: 12000
Trying to resolve IceHost IP from DNS
Found 1 IceHost IP address(es): 194.39.66.96
1. resolved IP address for name: 194.39.66.96
Reached AWRegistry:12000 on IP: 194.39.66.96
ConnectionString for AWRegistry: AWRegistry/Locator:default -h 194.39.66.96 -p 12000

Trying to reach 12000-12005 on IceHost
Reached the port 12000 on IP: 194.39.66.96
Reached the port 12001 on IP: 194.39.66.96
Error reaching port 12002 on IP: 194.39.66.96 No connection could be made because the target machine actively refused it 194.39.66.96:12002
Error reaching port 12003 on IP: 194.39.66.96 No connection could be made because the target machine actively refused it 194.39.66.96:12003
Reached the port 12004 on IP: 194.39.66.96
Reached the port 12005 on IP: 194.39.66.96
...
Press any key to end
```

### 2.4 Service Locator Administration is not displayed

One reason can be that the display coordinates are in an area that is not visible (e.g. -32000). A suspicion is that this happens if the application was closed on a second screen. Simply deleting the value or entering sensible values eliminates the problem.

*[Image: Windows Registry Editor showing the key `HKEY_CURRENT_USER\Software\JavaSoft\Prefs/Ice/Grid/G/U/I/Window` with values for `x` and `y` coordinates.]*

### 2.5 CorelceStorm cannot be reached

It can happen that when starting BasicData, license or workflow or other services, an error occurs and the corresponding services cannot be started. The following error messages occur then:

```
An inner exception occurred:
Type: Ice.UnknownException
Message: Exception of type 'Ice.UnknownException' was thrown.
StackTrace:   at IceInternal.AsyncResultI.wait()
   at IceStorm.TopicPrxHelper.end_subscribeAndGetPublisher(...)
   at IceStorm.TopicPrxHelper.subscribeAndGetPublisher(...)
   at IceStorm.TopicPrxHelper.subscribeAndGetPublisher(...)
   at AWSOA.Core.Client.Communication.IceClient.SubscribeTopicSlice(...)
   at AWSOA.Core.Client.Communication.IceClient.CreateIceSubscriberSliceFor[](...)
   at AWSOA.Core.Client.Communication.IceClientProxyFactory.CreateSubscriberSliceFor[T,TDel](...)
```

If a restart of the entire system doesn't change anything about the error messages, the previous "cache" of the IceCoreStorm can be deleted. It recreates itself when starting the corresponding service and can then simply be used after that.

The corresponding files are under:
`%PROGRAMDATA%\A+W\Sandpiper1\InfrastructureServices\db\servers\CoreIceStorm\data`

For example, starting with ICE 3.7:
`%PROGRAMDATA%\A+W\Sandpiper1\InfrastructureServices\db\servers\CoreIceStorm\data_CoreIceStorm`

The files included in this directory can be deleted after stopping the IceCoreStorm service. After that, the error should disappear and a connection for the clients should be possible again.

## 3. Uninstalling

To uninstall the software (for example, for a reinstall if a server was renamed), use the Windows program management. Here, make sure to adhere to the sequence. The Service Locator must be uninstalled as the next-to-last and the middleware as the last program.

If in addition to the infrastructure other AWSOA services must be installed, these must be uninstalled before the Service Locator and middleware during a complete uninstallation.

-   Uninstallation of all SOA services and websites
-   Uninstallation of the ServiceLocator infrastructure
-   Uninstallation of the middleware infrastructure

After the uninstallation, delete the following directories in order to remove the application completely:

-   `C:\Program Files (x86)\A+W\Sandpiper1\`
-   `C:\ProgramData\A+W\Sandpiper1\`

Both registry keys must also be deleted completely:
-   `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Albat+Wirsam\Communication`
-   `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Albat+Wirsam\Database`

A reboot of the system after work done is never a bad idea!
