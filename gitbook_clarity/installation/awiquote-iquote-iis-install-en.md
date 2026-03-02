---
description: "EN-INST-AW_iQuote"
---


# Installation Instructions: iQuote – for A+W Business

---
## Change history:

| Date | Edited by | Remarks |
| :--- | :--- | :--- |
| 2018-01-10 | D.Langsdorf | Release version |
| 2018-07-16 | D.Langsdorf | Firewall TCP 1.3.2, 1.6 |
| 2019-05-06 | D.Langsdorf | Further screenshots |
| 2020-06-18 | D.Langsdorf | Breaking Changes |
| 2020-07-15 | D.Langsdorf | Browser cache and content reload |
| 2020-11-04 | D. Langsdorf | Addition for HTTPS/SSL 1.5 |
| 2022-02-02 | D. Langsdorf | Multisite installation Commercial Document Service 1.4 |
| 2023-10-06 | D. Langsdorf | Login page with user management and multisite access 4 |

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

## Content

- **Installation Instructions**
- **iQuote - for A+W Business**

### 1 New installation of version 6
- 1.1 Overview and the basics
- 1.2 Time requirement
- 1.3 Requirements
  - 1.3.1 Hardware
  - 1.3.2 Network
  - 1.3.3 Installation account
  - 1.3.4 Software
- 1.4 Installation of server components
- 1.5 HTTPS configuration of the IIS
- 1.6 Configuration of the firewall for the DMZ
- 1.7 Variants of implementation
  - 1.7.1 In-house Hosting
  - 1.7.2 Hoster with VPN In-house
- 1.8 Call of the application
- 1.9 Setting up access to the Service Locator
- 1.10 Incompatibilities
- 1.11 Directory structure
- 1.12 Tips and tricks
  - 1.12.1 FAQs
  - 1.12.2 Web front end does not get a connection to the services
  - 1.12.3 The document service cannot be started
  - 1.12.4 Error analysis in the browser
  - 1.12.5 Copying the SOA tables into a new or existing database
  - 1.12.6 Internet Explorer Trusted Sites
- 1.13 Uninstalling
- 1.14 A+W Licenses

### 2 System configuration
- 2.1 Configuration of IIS
- 2.2 Browser cache and content reload

### 3 Breaking Changes
- 3.1 2-phase commit when saving the orders 13.04.3924

### 4 Login page installation
- 4.1 Requirements
- 4.2 Architecture
- 4.3 Installation

## 1 New installation of version 6

The following installation instructions assume that there is no previous version installed. For all modules of the SOA, only a Version 6 is provided; these are the basis for the installation.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:
- Installation .Net Framework 4.5
- Installation Internet Information Service IIS >=7
- Installation of the database client software
- Creation of the database if no inventory database is used
- Installation of the software with the Setup Launcher
- Installation A+W Business 6 or 5.5
- Installation A+W Infrastructure 6
- Activation of A+W License iQuote Configurator / Info

### 1.2 Time requirement

The time requirement will be approx. 90 minutes for the creation of the prerequisites and the actual installation. There is no conversion of data stocks.

### 1.3 Requirements

#### 1.3.1 Hardware

Computers with Windows Server operating system Windows Server 2008 or higher are approved. In emergency situations and workstation installations will support the installation starting with Windows 7. The latest service packs and operating systems from Microsoft must always be installed.

#### 1.3.2 Network

The installation of the infrastructure services is a prerequisite; it must be entered as a dependency.

ICE services communicate via the ports 12000-12005 TCP + 65230-65235 TCP, which have to be opened in the network. The installation opens these in the Windows firewall of its own accord. If other firewall programs are used, then the ports must be opened manually there.

> **PLEASE NOTE:** A connection has to be established to the A+W FTP Service (port 25). Without this, the download of the SQL scripts cannot occur and the database update service cannot initialize and update the database. The connection is configured in the auto update of the Setup Launcher. The installation with local update scripts is possible, but it requires the constant manual updating of the scripts.

#### 1.3.3 Installation account

For the installation, a user with administration rights must be used. If there is a MUI/Language pack installation of the Windows system, for this user the installation language of the system must be set as primary language since otherwise the internal users will not be recognized correctly during the installation of the ICE services.
(Error message: `Could not retrieve Security ID for NT-AUTORITHÄT\SYSTEM: No mapping between account names and security IDs was carried out.`).

In the Language options, ensure the Windows display language is set to the primary installation language of the operating system.

#### 1.3.4 Software

##### 1.3.4.1 A+W Software

Prerequisite is a complete installation of:
- A+W Business 6 or 5 SP5
- A+W Infrastructure 6 xxx
- A+W CAD Designer (Shapes)
- A+W CAD 6 Services
- A+W Commercial Document 6 Services
- A+W iQuote 6 Services
- A+W iQuote 6 Web

These are entered as dependencies in the DiskSet.

##### 1.3.4.2 .Net Framework 4.5

The framework is installed automatically by the Setup Launcher.

##### 1.3.4.3 Internet Information Service

The IIS (Version 7 or higher) must be installed.

If the .Net Framework 4 was installed prior to the IIS, it may occur that the required Asp.Net 4.0 AppPools cannot be created correctly. Please check this in IIS management under the application pools.

If an App Pool's .NET Framework Version is not v4.0.30319, an administrative command line can be used to generate the respective App Pools:
```
C:\Windows\Microsoft.NET\Framework\v4.0.30319>aspnet_regiis.exe -i
```
If a Windows Server OS is used, the Server Management Tool has to be used. In the Windows features, the following functions must be activated for the IIS.

**Required IIS Features:**
- **Web Server (IIS)**
  - **Common HTTP Features**
  - **Health and Diagnostics**
  - **Performance**
    > **Caution:** Starting with Version v6 Update 4, the performance features (including dynamic content compression) must be installed.
  - **Security**
    - Request Filtering
    - Basic Authentication
    - Centralized SSL Certificate Support
    - Client Certificate Mapping Authentication
    - Digest Authentication
    - IIS Client Certificate Mapping Authentication
    - IP and Domain Restrictions
    - URL Authorization
    - Windows Authentication
  - **Application Development**
    - .NET Extensibility 3.5
    - .NET Extensibility 4.5
    - ASP
    - ASP.NET 3.5
    - ASP.NET 4.5
    - ISAPI Extensions
    - ISAPI Filters
    - WebSocket Protocol (optional, for modern fast communication)
- **Management Tools**
  - **IIS 6 Management Compatibility**
    - IIS 6 Metabase Compatibility
    - IIS 6 Scripting Tools
    - IIS 6 WMI Compatibility

##### 1.3.4.4 Windows Server operating system

If the user directly requests the web interface on a Windows Server operating system, the "Internet Explorer Enhanced Security Configuration" (IE ESC) has to be disabled for both Administrators and Users. This can be configured in the Server Manager.

##### 1.3.4.5 Databases and clients

The following 32-bit database clients are approved (A+W does not support any 64-bit database drivers):

*   Microsoft SQL Server 2008 R2 Native Client or newer
*   Oracle 11g R2 Client Win32
*   IBM Informix Client-SDK (32-bit) 3.50

If the system is used as an extension for A+W Business on SQLBase for the trace/log mechanism, a SQLServer Express 2012 installation can be undertaken for protocol evaluation.

**Preparation of SQLServer**
Only the native client must be installed; no configuration of the client software is needed. Access can be tested with a `.uld` file.

**Preparation of Informix**
Informix does not support Guids natively. A function `makeguid` must be installed in Informix before the installation of the infrastructure services.

1.  On the database server, copy the file `guid.bld` into the directory `%INFORMIXDIR%\extend\Guid` or `c:\Program Files\IBM Informix Software Bundle\extend\Guid`. The `Guid` subdirectory must be created. The file is a component of the middleware infrastructure and is located in:
    *   `%PROGRAMFILES%\A+W\Sandpiper1\InfrastructureMiddleware\Informix\x86` (for 32-bit Informix)
    *   `%PROGRAMFILES%\A+W\Sandpiper1\InfrastructureMiddleware\Informix\x64` (for 64-bit Informix)

2.  The file `guid.bld` must have the write-protect attribute set.
3.  Set up the function with the Informix tool `dbaccess`. The user must be a member of the "Informix administrators" group. The command is in the `guid.sql` file.
    ```sql
    CREATE FUNCTION makeguid()
    RETURNING lvarchar
    WITH(VARIANT, PARALLELIZABLE)
    EXTERNAL NAME "$INFORMIXDIR/extend/guid/guid.bld(makeguid)"
    LANGUAGE C;
    ```
4.  After installation, test the function once manually:
    ```sql
    EXECUTE FUNCTION makeguid();
    ```
    A successful test must return a GUID. If there is an error, it must be eliminated.

> **For info only:** To delete the function, use: `DROP FUNCTION makeguid();`

For database access to Informix, an ODBC system DSN must be created with the Informix ODBC. An existing connection from A+W Production can be used.

**Preparation of Oracle**
For Oracle, the Oracle client has to be installed, and an ODBC system DSN must be created.

### 1.4 Installation of server components

For the installation, please proceed in the following sequence:

1.  Start the Setup Launcher and generate a new diskset or expand an existing one. An autoupdate installation is the standard method. Check the diskset directory, installation drive, and hotfix path for correct values.
2.  Confirm the configuration in the main dialog by pressing **Next**.
3.  The installed components are shown. Proceed to the **Next** button.
4.  In the component selection view under `A+W Common`, select the following components. All further components are automatically selected as dependencies.
    *   A+W Infrastructure 6 Services
    *   A+W Infrastructure 6 Web
    *   A+W iQuote 6 Services
    *   A+W iQuote 6 Web
    *   A+W Commercial 6 Business Services
    *   A+W Business 6 Basis
5.  Configure the connection to the Service Locator. For the host, enter the name of the computer where the Service Locator was installed. The port is always `12000`.
6.  In the next dialog, determine the user under which the services will run. Click the **Browse...** button to open the Windows user selection. This user should be coordinated with the user of the A+W Business.
7.  Save the configuration and start the installation by clicking **Next**.
8.  After the installation is complete, the configuration of the components begins. First, create the database connection. Inventory databases from ERP or PPS should be used. For an ERP standalone installation, the ERP database can be selected. In the case of SQLBase, SQL Server Express must be installed and an empty database created.
    *   **Type**: select between SQLServer, Oracle, or Informix.
    *   **Server Instance**: enter the instance of the database server.
    *   **User**: select the database user.
    *   **Password**: enter the user password.
    *   **Database**: specify the database name.
    After entering the data, click **Next** to check the database connection.
9.  Configure the multisite settings for the Commercial Service. This determines which sites a service should be activated for and how many workers per site should be active.
    *   **Active**: Set to `True` to activate the service for a site.
    *   **Worker**: Specify the number of workers for load distribution (at least 1).
    > **Special feature:** If no "Active" property is set, the service will still be installed for site 1 by default. This is the default behavior if A+W iQuote is not installed for multiple sites.
10. The CAD designer must be configured for use in services. Start the configuration program of the CAD designer (`SN Config Tool`) with "Run as admin" and specify the user of the commercial services (the same user from Step 6) as the service user.

The installation and configuration is now complete.

### 1.5 HTTPS configuration of the IIS

For security reasons, Web components should always be installed with SSL encryption via HTTPS. This is not done through the setup and must be performed by the IIS administrator. The certificate is installed for the default site and is retained during updates.

An SSL certificate must be provided by the client. A self-signed test certificate can be created locally for temporary use.

1.  Start the **IIS Manager**, select the server node, and double-click **Server Certificates**.
2.  To import a real certificate, click **Import**. To create a test certificate, click **Create a Self-Signed Certificate**.
3.  Give the certificate a meaningful name (e.g., `A+W WebConfigurator`) and specify **Web Hosting** as the storage location.
4.  In the IIS Manager, select the **Default Web Site** and click **Bindings...** in the Actions pane.
5.  Click **Add...** to add a new site binding.
    *   **Type**: `https`
    *   **IP address**: `All Unassigned`
    *   **Port**: `443`
    *   **Host name**: (Optional) This must match the certificate and the URL that is called.
    *   **SSL certificate**: Select the previously created certificate from the dropdown list.
6.  Click **OK**.

Now all sites can be accessed via HTTPS.

> **Note:** You must apply for the certificate from an authorization office. A+W cannot include this in the delivery as it represents a position of trust for the Website operator.

### 1.6 Configuration of the firewall for the DMZ

If iQuote is installed in a DMZ (addressable from the Internet), only the packages "A+W Infrastructure 6 Middleware" and "A+W iQuote 6 Web" must be installed on the server in the DMZ.

The installation opens ports **12000-12005 TCP** and **65230-65235 TCP** in the Windows firewall. If a hardware firewall is in place for the DMZ, these ports must also be enabled there.

> **Important:** This enabling should be limited to the target address of the process server and the source address of the DMZ server.

The firewall must also be opened to the Internet for port 80 (or 443 for HTTPS) so the IIS can be reached.

**Architecture Overview (DMZ):**
- **External User (Browser)** communicates with the **IIS Server** in the DMZ over port 80/443.
- The **IIS Server (DMZ)** communicates with the **Process/DB-Server (Inhouse)** over ports 12000-12005 and 65230-65235.

All services (except "A+W Web 6 Web") must be installed on the process computer.

### 1.7 Variants of implementation

iQuote can be deployed in two ways: as an in-house solution or as an ASP.Net application hosted by a provider with a VPN connection to the customer's services. A provider-hosted solution without data replication is not currently available.

#### 1.7.1 In-house Hosting

All components are within the company. The IIS server is located in the DMZ, and the services are behind a second firewall on a server in the internal network. This variant requires a Windows Server license for the DMZ server and a Core license for the database. Ensure the IIS has sufficient bandwidth to be addressed from the Internet.

**Architecture:**
- **Browser** -> **IIS (DMZ)** -> **Services (In-house)**

#### 1.7.2 Hoster with VPN In-house

The IIS is transferred to a hoster, and the services are addressed via a VPN connection. The hoster is responsible for the Windows Server licenses. The bandwidth of both the hoster and the VPN connection must be sufficient. Normally, only SQLServer Core licenses are necessary.

**Architecture:**
- **Browser** -> **IIS (Hoster)** -> **VPN** -> **Services (In-house)**

### 1.8 Call of the application

The application installs its shortcuts in the A+W directory in the Start Menu (`C:\ProgramData\Microsoft\Windows\Start Menu\Programs\A+W`). It is started with a double-click.

The **Infrastructure 6 Config Tool** and the **Service Locator Administrator** are in the `Config Tools` subfolder.

### 1.9 Setting up access to the Service Locator

The first time you open the Service Locator Administrator (**IceGrid Admin**), you must establish a connection.

1.  In the "New Connection" wizard, select **Direct Connection**.
2.  Specify the **Instance Name**. The default is `AWRegistry`. (Note: This is case-sensitive).
3.  Choose to provide addressing information as **A hostname and a port number**.
4.  Enter the **Hostname** (`localhost` if on the same machine) and **Port number** (`12000`). These are the values entered during the installation.
5.  Specify a name for the connection (e.g., `MyName`). A password is not required for unsecured access.
6.  Click **Finish**.
7.  To connect, select the newly created connection from the list and click **Connect**.

The ICE services are depicted in the Service Locator. They can be started and stopped here, but this is not normally necessary as they start automatically.

### 1.10 Incompatibilities

No incompatibilities are known.

### 1.11 Directory structure

The application installs itself completely under:
`C:\Program Files\A+W\Sandpiper1`

### 1.12 Tips and tricks

#### 1.12.1 FAQs

**My services are not displayed in the Service Locator.**
Check whether the service nodes are running in Windows Services. Specifically, check for `A+W Infrastructure 6 Services Node` and `A+W Infrastructure 6 ServiceLocator`.

**Application no longer starts with "No switches were loaded for client xxx."**
This error can occur sporadically if the first site was just entered in site management. The pages are cached on the IIS, and the newly-created site is not found. **Reboot the server** to resolve this.

#### 1.12.2 Web front end does not get a connection to the services

If DNS name resolution does not work, enter the IP address of the Service Locator instead of its name in the Service Locator configuration.

You can use Telnet to check if the services are accessible through the firewall:
```
telnet <computername> <port>
```
The port numbers are **12000-12005** and **65230-65235**.

#### 1.12.3 The document service cannot be started

If this occurs after installation, an explicit user should be entered for the Business COM object.

1.  Open **Component Services**.
2.  Navigate to `Computers > My Computer > DCOM Config`.
3.  Find the relevant A+W component (e.g., `{4A82C8C3-51D4-4B0F-87A6-3BF4C32FA660}`).
4.  Open its **Properties** and go to the **Identity** tab.
5.  Select **This user** and enter the credentials for a user account (e.g., the same one used for the services).

Alternatively, changing the user for the `A+W Commercial 6` Windows service can also solve the problem.

1.  Open **Services**.
2.  Find **A+W Commercial 6**, open its **Properties**.
3.  Go to the **Log On** tab, select **This account**, and enter the user credentials.

#### 1.12.4 Error analysis in the browser

**Internet Explorer**

*   **Checking for IE11/10**: Go to `About Internet Explorer` to verify your version. iQuote requires IE10 or higher; IE11 is recommended.
*   **Javascript active**: iQuote requires JavaScript. In `Internet Options > Security > Custom level...`, ensure **Active scripting** is set to **Enable**.
*   **Cookies**: Check if browser settings allow cookies. In `Internet Options > Privacy`, ensure settings are not too restrictive. You may need to go to `Advanced` and `Accept` both First-party and Third-party cookies, or at least prompt.
*   **Network protocol**: If problems persist, use the browser's developer tools (press F12).
    1.  Open Internet Explorer and press **F12**.
    2.  Go to the **Network** tab.
    3.  Click the green "Play" button to start capturing traffic.
    4.  Enter the URL for iQuote and press Enter.
    5.  All network queries will be listed. The **Result** column provides status codes (e.g., 200 for success, 404 for not found). This log can be sent to A+W Service for analysis.

#### 1.12.5 Copying the SOA tables into a new or existing database

1.  In SQL Server Management Studio, right-click the source database, go to `Tasks > Generate Scripts...`.
2.  In the "Choose Objects" step, select **Select specific database objects** and check all SOA tables (e.g., `Cockpit_*`, `Core_*`, `Web_*`).
3.  In "Set Scripting Options", set the output to **Save to new query window**.
4.  In the generated script, change the `USE [database_name]` command to point to the target database.
5.  Execute only the `CREATE TABLE` and `ALTER TABLE ... ADD DEFAULT` commands from the script, up to the first `ALTER TABLE ... WITH CHECK ADD CONSTRAINT ... FOREIGN KEY` command.
6.  Export the data from the source database. Right-click the source database, go to `Tasks > Export Data...`.
7.  Select the source and target databases. In the "Specify Table Copy or Query" step, select **Copy data from one or more tables or views**.
8.  Select all the tables that were created in step 5 and execute the data transfer.
9.  Return to the script from step 4. Execute the remaining part of the script, which creates the foreign keys.
10. The SOA tables are now copied into the target database.
11. Finally, use the **A+W Infrastructure Config Tool** to change the SOA database connection to point to the new target database.

#### 1.12.6 Internet Explorer Trusted Sites

On Windows Server 2012 R2 and higher, the application's domain must be added to the **Trusted Sites** zone in Internet Explorer's Internet Options.

1.  Go to `Internet Options > Security > Trusted sites > Sites`.
2.  Add the website URL (e.g., `http://awbawp60.tse.intra`) to the zone.
3.  Uncheck `Require server verification (https:)` if using HTTP.

If this is not done, icons may not display correctly, or other security-related errors may occur.

### 1.13 Uninstalling

To uninstall the software, use the Windows **Programs and Features**. Adhere to the following sequence:
1.  Uninstall all other A+W components.
2.  Uninstall the **A+W Infrastructure 6 Service Locator** as the next-to-last program.
3.  Uninstall the **A+W Infrastructure 6 Middleware** as the last program.

### 1.14 A+W Licenses

There are two license modules for iQuote, visible in the A+W License Monitor:

*   **iQuote Configuration**: Allows configuration and use of the info (history) module. (e.g., `Module: 1 iQuote Configuration [Mode=Session; Licenses=250]`)
*   **iQuote Info**: Allows only the use of the information area, with no possibility for configuration. (e.g., `Module: 2 iQuote Info [Mode=Session; Licenses=250]`)

## 2 System configuration

### 2.1 Configuration of IIS

To achieve optimal performance, make the following settings in IIS. These affect performance until the start page is displayed (JIT compiler) and prevent the IIS worker process from going to sleep.

1.  In IIS Manager, go to **Application Pools**.
2.  Select the `Web.WebAppPool`.
3.  Open its **Advanced Settings**.
4.  Set **Start Mode** to `AlwaysRunning`.
5.  Set **Idle Time-out (minutes)** to `0`.
6.  In IIS Manager, navigate to the site (`Default Web Site > Web.Web`).
7.  Open its **Advanced Settings**.
8.  Set **Preload Enabled** to `True`.

> **CAUTION:** The "Preload enabled" setting is currently lost with each update and must be reapplied.

### 2.2 Browser cache and content reload

The iQuote installation changes the IIS settings for the iQuote website by setting an HTTP response header. This forces content like JPG images to be reloaded after one hour instead of being drawn from the browser cache. This is useful for customers who change images and want users to see the updates without manually clearing their cache.

This is configured in `IIS Manager > [Site] > HTTP Response Headers > Set Common Headers...`, by setting content to expire after a specific duration. This setting is stored in the `web.config` of the site.

## 3 Breaking Changes

This section lists versions with breaking changes that require multiple modules to be updated together.

### 3.1 2-phase commit when saving the orders 13.04.3924

This version prevents orders from being created twice. The following modules must be updated together:

*   A+W Business 6 Basis: `13.04.1039 ++`
*   A+W Commercial 6 Document Services: `13.04.3924 ++`
*   A+W iQuote 6 Services: `13.04.3924 ++`
*   A+W iQuote 6 Web: `13.04.3924 ++`

## 4 Login page installation

### 4.1 Requirements

The login page must be installed on an IIS server in the DMZ.
*   IIS in the DMZ.
*   Installation of SQLServer (Express is sufficient), with mixed authentication recommended.
*   An empty database must be created on the SQLServer for login data. Customer passwords are saved as hashes and cannot be decrypted.
*   The user of the IIS application pool must have access to the login database.
*   The port for the service access (**port 65215**) must be opened in any existing firewall.
*   Provide the Installation Setup Launcher and diskset. The diskset may need to be stored locally in the DMZ.
    *   A+W iQuote 6 Multisite
    *   A+W iQuote 6 Multisite Service

### 4.2 Architecture

The login page, like all iQuote IIS components, must be accessible from the Internet and therefore reside in the DMZ. The SQLServer for login data must also be in the DMZ.

The multisite service is installed on the process server, as it needs access to the mail server. The main IIS for the login page can be one of the cluster IISes; a dedicated IIS is not necessary.

**Architecture Flow:**
1.  **Main IIS** (in DMZ) hosts the **Login page** and an **Admin page** for site assignment.
2.  The Main IIS has a connection to the **Login Provider Database** (in DMZ).
3.  The Main IIS communicates with the **Multisite Service** on the **Process Server** (in-house) over **Port 65215** through a firewall.
4.  The Main IIS also routes users to the various **iQuote sites** hosted on cluster IIS servers (e.g., Cluster 1 IIS, Cluster 2 IIS).

### 4.3 Installation

For simplicity, the example shows all components installed together, but in a productive environment, this would not be the case.

1.  Using the Setup Launcher, select the components to install:
    *   **A+W iQuote 6 Multisite**: This is the login page and must be installed on the IIS in the DMZ.
    *   **A+W iQuote 6 Multisite Service**: This service must be installed on the process computer.
2.  During the installation, you will be prompted to enter the user for the Multisite Service. The service node will run under this user.
3.  For the web page installation, access to the login database must be configured. In the `A+W iQuote Multisite Config` tool, specify the SQL Server instance and database name for the login data.
4.  After installation, the login page configuration is accessed via the icon in the A+W start menu. The detailed configuration process is described in the `A+W_iQuote configuration instructions`.
