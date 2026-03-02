---
description: "EN-INST-AW_ERP_Web_Service"
---


# Installation Instructions: A+W ERP Web Service

---
## Change history:

| Date | Edited by | Remarks |
| :--- | :--- | :--- |
| 2012-01-16 | André Münch | Original version |
| 2014-03-25 | Alexander Weil | CI adjustment |
| 2015-12-01 | André Münch | Version 6 |
| 2016-03-16 | Ralf Imhof | General adjustments Version 6 |
| 2017-01-27 | M. Pitz | maxRequestLength |
| 2020-11-04 | D. Langsdorf | HTTPS Installation of the IIS 1.5 |

This document enables the competent reader to install the described software. You should generally stick to this procedure:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

---

## Content

*   **1 New installation**
    *   1.1 Overview and the basics
    *   1.2 Time requirement
        *   1.2.1 Installation time for the software
        *   1.2.2 Conversion time for data stock
    *   1.3 Requirements
        *   1.3.1 Hardware
        *   1.3.2 Network
        *   1.3.3 Software
    *   1.4 Procedure
        *   1.4.1 Installation A+W ERP Web Service
        *   1.4.2 Configuration of A+W Business 6
        *   1.4.3 Configuration A+W Enterprise 6
    *   1.5 HTTPS configuration of the IIS
    *   1.6 Directory structure
    *   1.7 Settings
        *   1.7.1 Web.Config
        *   1.7.2 Parameters
        *   1.7.3 Customer-specific configuration
        *   1.7.4 Registry
    *   1.8 Result of the installation
    *   1.9 Alternative Installations
    *   1.10 Patches
    *   1.11 Tips and tricks
        *   1.11.1 FAQS
        *   1.11.2 Known errors and workarounds
    *   1.12 Uninstalling

---

## 1. New installation

The following installation instructions assume that there is no previous version installed. The set-up and configuration are described in the start-up documentation.

### 1.1 Overview and the basics

The following list provides an overview of the work that must be done during installation:
*   Installation of the web service for the ERP system (A+W Business 6, A+W Enterprise 6)
*   Configure the connection parameters with the ERP database

> **THIS VERSION IS COMPATIBLE WITH THE 6-series versions of the ERP systems A+W Enterprise and A+W Business.**

### 1.2 Time requirement

If all requirements are checked and fulfilled, the following times are required for the installation and the conversion of the existing data:

#### 1.2.1 Installation time for the software

Depending on the computer, storage space, and configuration, the installation times will vary for different computers. The installation time specified was determined using a reference device with the following characteristics:
*   Processor: 2.4 GHz Pentium and storage space: 40 GB

For an initial or new installation, an installation time of 5 minutes must be anticipated for the reference device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.

#### 1.2.2 Conversion time for data stock

No data is converted.

### 1.3 Requirements

#### 1.3.1 Hardware

Web server and installed Internet Information Server (IIS version >= 6 for short)

#### 1.3.2 Network

There has to be a connection between the web server and the ERP system's database.
If this web service is installed for A+W Enterprise and shall be used to communicate with A+W Production capacity planning, there has to be a connection with the A+W Enterprise application server as well.

#### 1.3.3 Software

*   ERP software (A+W Business 6 or A+W Enterprise 6)
*   To create OrderXML from A+W Business 6, the latest version of ItemsForALCIM and the latest Albwir.Edi.Order.Data have to be installed in A+W Production. If this is not the case, OrderXML documents cannot be imported into A+W Production.
*   Depending on the ERP system to be addressed by the web service, different database drivers need to installed beforehand:
    *   A+W Business → SqlBase Server Version 11.6 or
    *   A+W Business → SqlServer from Version 2012 or
    *   A+W Enterprise → Informix-Client Version 4.10.TC6x6
*   An IIS from Version 7 must be installed on the web server.
*   CommonBase (only in connection with ALCIM 2009 or lower)

### 1.4 Procedure

Please proceed in the following order during the installation process:

#### 1.4.1 Installation A+W ERP Web Service

Start the A+W Setup Launcher. Perform the general settings of the A+W Setup Launcher until you reach the dialog "Component selection" and select the item "A+W Web Service 6".

In the next step, you must decide whether the web service should be installed for A+W Enterprise 6 or A+W Business 6.

*   **A+W Business:** In case of an A+W Business installation, enter a Windows account on which the application pool of IIS is run. It is essential to choose an account that has at least the rights to create files (perhaps even network-wide) and COM objects. When you quit this dialogue the system checks if the defined Windows account exists and whether this Windows account has the right to register as a service. To grant a Windows account the right to register as a service, please add the Windows account in system control, in Administration > Local safety rules > Local rules > Allocation of user rights > Register as a service.
*   **A+W Enterprise:** For an A+W Enterprise installation, the application pool is kept in the predefined account, "NetworkService".

#### 1.4.2 Configuration of A+W Business 6

After the web service has been installed successfully, it has to be configured.

In the first tab, it can be determined whether the web service requires a connection to the CommonBase. If one of the listed products is used, a checkmark must be placed here. If none of the products are use, you can dispense with the configuration of the CommonBase. Pressing the Protocol button takes you to the tracing settings.

The first tab asks for the CommonBase connection data and the administrator login. When you confirm this dialogue by Next, the system checks whether CommonBase can be actually accessed by means of these parameters and whether the administrator can log in. If not, an error message appears at the bottom of the dialog.

Once the administrator has logged in, the CommonBase user and the password has to be specified. The switch of the ERP web service is exported and shown in the next dialog. This dialog serves to make the settings for tracing of the ERP web service. Here you can either make targeted settings of the individual areas of the ERP web service or set the trace level for the entire web service.

#### 1.4.3 Configuration A+W Enterprise 6

After the web service has been installed successfully, tracing can be configured.
Here you can either make targeted settings of the individual areas of the ERP web service or set the trace level for the entire web service.

### 1.5 HTTPS configuration of the IIS

For security reasons, the Web components should always be installed with SSL encryption via HTTPS. This is not done through the setup. Here the IIS administrator must perform the additional set-up.

The installation of the certificate is done for the default site and is thus not restricted to just one webservice. It is retained even in case of an update. It must therefore be done once manually before the expiration of the certificate.

An SSL certificate must be made available by the client. Temporarily, a local certificate can be created; however, it cannot be used from the outside in real operation.

1.  Start the IIS Manager and mark the server under (1), then double-click the (2) server certificates.
2.  In order to import a real certificate, go to **Import**.
3.  To create a self-signed test certificate, go to **Create a Self-Signed Certificate**.
4.  Give the certificate a meaningful name (e.g., A+W WebConfigurator) and specify **Web hosting** as the storage location.
5.  Now mark the **Default site** (1) and select the **Bindings** (2) in the Actions pane.
6.  Now the binding for HTTPS must be added. To do this, click the **Add** button.
7.  In the "Add Site Binding" dialog:
    *   Set the **Type** to **https**.
    *   The **Port** will default to **443**.
    *   The "Host name" has to match the certificate and the URL that is called.
    *   Select the previously-created SSL certificate from the dropdown list.
    *   You can verify this with the **View** button.

Now all sites can be surfed with https. Please note that you must apply for the certificate from an authorization office. A+W cannot include this in the delivery since it represents a sign of the Website operator's trust.

### 1.6 Directory structure

The web service does not require any existing directory structures, nor will it create directories.

### 1.7 Settings

The database connection parameters with the ERP system's database are managed in CommonBase. This specifically involves the following buttons:

**Enterprise ERP – Web service - Purchase Order**
1.  **Cost rewrite**
    *   PUR rewrite to ALFAK order
    *   default: (empty)
2.  **Prefix for importing DORMA article numbers**
    *   Prefix for DORMA articles
    *   default: D.

**Enterprise ERP – Web service – Database**
3.  **Database name ERP system**
    *   Name of the database of the ERP system
    *   default: (empty)
4.  **Database server ERP system**
    *   Name of the database server hosting the database of the ERP system
    *   default: (empty)
5.  **Database user ERP system**
    *   Database user
    *   default: (empty)
6.  **Password ERP system (Base64)**
    *   Password of the database user (Base64 encrypted)
    *   default: (empty)
7.  **Client locale**
    *   ALCIB: client locale
    *   default: (empty)
8.  **Database locale**
    *   ALCIB: database locale
    *   default: (empty)
9.  **Database type**
    *   Database type (1=Informix, 2=SqlBase, 3=SqlServer, 4=Oracle)
    *   default: (empty)

**Enterprise ERP – Web service – Configuration**
10. **ALFAK ini file**
    *   Path and name of the ALFAK configuration file
    *   default:
11. **ALFAK password (Base64)**
    *   **ATTENTION!!! - no longer used - the password of the ALFAK user is maintained in switch "Password ERP-System"**
    *   default:
12. **ALFAK user**
    *   **ATTENTION!!! - no longer used - the ALFAK user is kept in switch "Database user ERP-System"**
    *   default:
13. **Server name ERP system**
    *   Database server
    *   default:
14. **Socket port ERP system**
    *   default:
15. **Type ERP system**
    *   Type of the ERP system (1 = ALCIB, 2 = ALFAK)
    *   default: 1
16. **URL**
    *   Address at which the web service is addressed
    *   default: „http://localhost/Albwir.Erp.WebService/ErpData.asmx"
17. **Path OrderXML-File**
    *   ALCIB: Path for OrderXML transfer
    *   default:
18. **Path Pictures Dorma**
    *   Path for DORMA article images
    *   default:
19. **Path Pictures KLMegla**
    *   Path for KLMegla article images
    *   default:
20. **Path Pictures WSS**
    *   Path for WSS article images
    *   default:

**Enterprise ERP – Web service – AWCapacity**
21. **Purchase order deadline check**
    *   Delivery date check by AWCapacity
    *   default: 0
22. **Stock reservation**
    *   Stock reservation in ALFAK by AWCapacity
    *   default: 0
23. **Update Timecosts**
    *   Update of time costs in ALFAK by AWCapacity
    *   default: 0

#### 1.7.1 Web.Config

With #378450 the switch „maxRequestLength" in the web.config raised from 4MB to 16MB to report large orders from A+W Production to A+W Enterprise.

#### 1.7.2 Parameters

No further parameters apart from the database configuration.

#### 1.7.3 Customer-specific configuration

No customer-specific configuration provided for.

#### 1.7.4 Registry

No processing needs to be done in the registry.

### 1.8 Result of the installation

The success of the installation can be checked by starting the Internet Explorer and entering the URL "http://localhost/<virtualDir>/erpdata.asmx" in the address field.
`<virtualDir>` is the dummy for the virtual address selected in the setup dialog.
If the installation is run without errors, the WSDL page (Web Service Description Language) of the web service will appear.

### 1.9 Alternative Installations

None known.

### 1.10 Patches

| Designation | BESCHREIBUNG | Prerequisite |
| :--- | :--- | :--- |
| | | |
| | | |

### 1.11 Tips and tricks

#### 1.11.1 FAQS

More FAQs that are not yet included in this document, may be available in http://bladeentw/dotnetnuke/

1.  **When you load the ASP.NET page or the web service, only HTML tags will appear in the Internet Explorer.**
    May happen if the Internet Information Server IIS was installed after the Framework!
    *   Check whether Framework 3.5 is installed (System control --> Software --> Microsoft .NET Framework 3.5)
    *   Reregister ASP.NET 2.0 via console (`systemroot\Microsoft.NET\Framework\v2.0.50727\aspnet_regiis -i`)
    *   Restart the IIS Admin service and all downstream services (WWW-Publishing, SMTP, FTP)
    *   Restart the computer

2.  **When you call an ASP.NET page on a newly installed Windows 2003 server (IIS 5.2), error message 400 "Page not found" appears although the URL clearly points to the web application.**
    Possibly, the "Web service extension for ASP.NET applications" is not valid in IIS!
    *   Open the IIS management program and search for the entry "Web service extensions"
    *   Select "Accept ASP.NET"

3.  **No tracing file is created although tracing is activate in the web.config.**
    The ASP user has no write rights in the directory in which the tracing file is to be created.
    *   Load the properties of the trace directory and select the tab "Security"
    *   Check whether the user IUSR_computer name appears on the list of group and user names
    *   If necessary, allocate this user and grant write rights for this directory
    > **WARNING:** For reasons of safety, this account should be granted access to the tracing directory only while tracing is run!

4.  **How can I find out how the web application accesses the CommonBase?**
    The CommonBase configuration is saved in the web.config
    *   **Section "appSettings"**
        The connection type is entered here. Possible values of the key "Connectiontype" are REMOTING and DIRECT. Only REMOTING is used at present.
    *   **Section "system.runtime.remoting"**
        lists the individual Remote objects and their connection parameters. Important is the attribute "url", especially the first part of the address which shows the computer name and port in which the CommonBase is hosted.
        (Example 1: `url="http://bladeentw:8082/CommonBaseServer/RemotingComServer.rem"` /> means that the CommonBase service runs on the computer BLADEENTW and its remote object "RemotingComServer" can be accessed via port 8082.)
        (Example 2: `url="http://localhost:1530/CommonBaseServer/RemotingComServer.rem"` /> means that the CommonBase service runs on the same server as the web application and its remote object "RemotingComServer" is accessible via port 1530.)

5.  **How can I find out how my CommonBase is configured for remote access and which database is used?**
    The CommonBase configuration is saved in the config file "albwir.cb.commonbaseservice.exe.config"
    *   **Section "system.runtime.remoting"**
        Here the port is entered under
        ```xml
        <application>
          <channels>
            <channel ref="http" port="1530">
        ```

    *   **Section "appSettings"**
        This is where the information on the database is saved. (Example: SqlBase database CBLOC on SERVER1, access via user SYSADM and password SYSADM)
        *   **Database type (SqlBase, Informix, SqlServer)**
            `<add key="DB/DBTYPE" value="SqlBase" />`
        *   **Name of the database**
            `<add key="DB/DBNAME" value="cbloc" />`
        *   **Server name**
            `<add key="DB/DBSERVER" value="server1" />`
        *   **Database user**
            `<add key="DB/DBUSER" value="sysadm" />`
        *   **Base64 encrypted password of the user**
            `<add key="DB/DBPWD" value="c3lzYWRt" />`

#### 1.11.2 Known errors and workarounds

##### 1.11.2.1 Write rights missing for the trace directory

If the web service fails to work and does not even write a trace file it may be that the user code under which the web service is run, has no write rights for the defined trace path.

### 1.12 Uninstalling

To uninstall the web service, load the uninstall routine in the software section of system control.

**Uninstallation must be done PRIOR to the new installation; otherwise, the installer cannot be loaded.**
