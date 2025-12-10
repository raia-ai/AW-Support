---
description: "EN INST A+W iQuote"
---



# EN INST A+W iQuote

Installation Instructions

          iQuote – for A+W Business
   Change history:
     Date            Edited by        Remarks
     2018-01-10      D.Langsdorf      Release version
     2018-07-16      D.Langsdorf      Firewall TCP 1.3.2, 1.6
     2019-05-06      D.Langsdorf      Further screenshots
     2020-06-18      D.Langsdorf      Breaking Changes
     2020-07-15      D.Langsdorf      Browser cache and content reload
     2020-11-04      D. Langsdorf     Addition for HTTPS/SSL 1.5
     2022-02-02      D. Langsdorf     Multisite installation Commercial Document Service 1.4
     2023-10-06      D. Langsdorf     Login page with user management and multisite access 4



     The installation instructions will assist the planner with the installation and
     configuration process for the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




11.10.2023                               EN-INST-A+W iQuote.docx                               1
Content

   Installation Instructions .................................................................... 1

   iQuote – for A+W Business .............................................................. 1

   1         New installation of version 6 ................................................. 4
   1.1       Overview and the basics ...........................................................................4
   1.2       Time requirement ......................................................................................4
   1.3       Requirements ............................................................................................4
   1.3.1     Hardware ...................................................................................................4
   1.3.2     Network .....................................................................................................4
   1.3.3     Installation account ....................................................................................5
   1.3.4     Software ....................................................................................................6
   1.4       Installation of server components ............................................................10
   1.5       HTTPS configuration of the IIS ................................................................17
   1.6       Configuration of the firewall for the DMZ .................................................21
   1.7       Variants of implementation ......................................................................22
   1.7.1     In-house Hosting .....................................................................................22
   1.7.2     Hoster with VPN In-house .......................................................................23
   1.8       Call of the application ..............................................................................24
   1.9       Setting up access to the Service Locator ................................................25
   1.10      Incompatibilities .......................................................................................28
   1.11      Directory structure ...................................................................................28
   1.12      Tips and tricks .........................................................................................29
   1.12.1    FAQs .......................................................................................................29
   1.12.2    Web front end does not get a connection to the services ........................29
   1.12.3    The document service cannot be started.................................................30
   1.12.4    Error analysis in the browser ...................................................................31
   1.12.5    Copying the SOA tables into a new or existing database ........................34
   1.12.6    Internet Explorer Trusted Sites ................................................................39
   1.13      Uninstalling ..............................................................................................40
   1.14      A+W Licenses .........................................................................................41

   2         System configuration ........................................................... 42
   2.1       Configuration of IIS ..................................................................................42
   2.2       Browser cache and content reload ..........................................................44



11.10.2023                                     EN-INST-A+W iQuote.docx                                                   2
   3         Breaking Changes ................................................................ 45
   3.1       2-phase commit when saving the orders 13.04.3924 ..............................45

   4         Login page installation ........................................................ 46
   4.1       Requirements ..........................................................................................46
   4.2       Architecture .............................................................................................47
   4.3       Installation ...............................................................................................48




11.10.2023                                     EN-INST-A+W iQuote.docx                                                   3
1 New installation of version 6
The following installation instructions assume that there is no previous version
installed.
For all modules of the SOA, only a Version 6 is provided; these are the basis for the
installation.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during
installation:
    -   Installation .Net Framework 4.5
    -   Installation Internet Information Service IIS >=7
    -   Installation of the database client software
    -   Creation of the database if no inventory database is used
    -   Installation of the software with the Setup Launcher
    -   Installation A+W Business 6 or 5.5
    -   Installation A+W Infrastructure 6
    -   Activation of A+W License iQuote Configurator / Info

1.2 Time requirement
The time requirement will be approx. 90 minutes for the creation of the prerequisites
and the actual installation. There is no conversion of data stocks

1.3 Requirements
1.3.1 Hardware
Computer with Windows Server operating system Windows Server 2008 or higher
are approved in emergency situations and workstation installations will support the
installation starting with Windows 7. The latest service packs and operating systems
from Microsoft must always be installed.


1.3.2 Network
The installation of the infrastructure services is a prerequisite, it must be entered as
a dependency.
ICE services communicate via the ports 12000-12005 TCP + 65230-65235 TCP,
which have to be opened in the network. The installation opens these in the
Windows firewall of its own accord. If other firewall programs are used, then the
ports must be opened manually there.
PLEAE NOTE: A connection has to be established to the A+W FTP Service (port
25). Without this, the download of the SQL scripts cannot occur and the database
update service cannot initialize and update the database. The connection is


11.10.2023                           EN-INST-A+W iQuote.docx                               4
configured in the auto update of the Setup Launcher. The installation with local
update scripts is possible, but it requires the constant manual updating of the scripts.


1.3.3 Installation account
For the installation, a user with administration rights must be used. If there is a
MUI/Language pack installation of the Windows system, for this user the installation
language of the system must be set as primary language since otherwise the
internal users will not be recognized correctly during the installation of the ICE
services
(Could not retrieve Security ID for NT-AUTORITHÄT\SYSTEM: No mapping
between account names and security IDs was carried out.).




11.10.2023                        EN-INST-A+W iQuote.docx                              5
1.3.4 Software
1.3.4.1 A+W Software
Prerequisite is a complete installation of
A+W Business 6 or 5 SP5
A+W Infrastructure 6 xxx
A+W CAD Designer (Shapes)
A+W CAD 6 Services
A+W Commercial Document 6 Services
A+W iQuote 6 Services
A+W iQuote 6 Web
These are entered as dependencies in the DiskSet.


1.3.4.2 .Net Framework 4.5
The framework is installed automatically by the Setup Launcher.


1.3.4.3 Internet Information Service
The IIS (Version 7 or higher) must be installed.
If the .Net Framework 4 was installed prior to the IIS, it may occur that the required
Asp.Net 4.0 AppPools cannot be created correctly.
Please check this in IIS management under the application pools. Normally, this is
not necessary.




11.10.2023                         EN-INST-A+W iQuote.docx                               6
If this is the case, and .NET Framework Version is not on v4.0.30319, an
administrative command line could be used to generate the respective App Pools.
C:\Windows\Microsoft.NET\Framework\v4.0.30319>
aspnet_regiis.exe –i
If a Windows Server OS is used, the Server Management Tool has to be used.
In the Windows features, the following marked functions must be activated for the
IIS.
The activation of the WebSocket protocol is optional. With activated WebSockets,
the communication between the browser (>= IE10) and ASP.net is executed at the
level of the modern and fast WebSocket. Otherwise, less effective methods are
reverted to.




11.10.2023                        EN-INST-A+W iQuote.docx                           7
Caution: Starting with Version v6 Update 4, the performance features must be installed.
Since we have also activated the compression for dynamic content.




11.10.2023                         EN-INST-A+W iQuote.docx                                8
1.3.4.4 Windows Server operating system
If the user directly requests the web interface on a Windows Server operating
system, the "Internet Explorer Advanced Security Configuration" has to be disabled.




1.3.4.5 Databases and clients
The following database clients are approved
    •   Microsoft SQL Server 2008 R2 Native Client or newer
    •   Oracle 11g R2 Client Win32
    •   IBM Informix Client-SDK (32-bit) 3.50
The 32-bit version is always used, A+W does not support any 64-bit database
drivers.
If the system is used as an extension for A+W Business on SQLBase for the
trace/log mechanism, the necessary databases cannot be integrated in just any
SQLBase database. In order to get the protocol evaluation, a SQLServer Express
2012 installation can be undertaken and the installation of the AWSO components
undertaken in this.
Preparation of SQLServer
Here, only the native client must be installed; there is no need for configuration of
the client software. Access can be tested with a file with the extension .uld; these
can be created on the desktop and access to the SQL Server tested.
Preparation of Informix
Informix does not support Guids. Since, however, in stock databases a GUID
column is also created in existing tables. A function makeguid must be installed in
Informix. For this, the following steps must be executed before the installation of the
infrastructure services:


11.10.2023                         EN-INST-A+W iQuote.docx                                9
    1. On the database server, copy the file "guid.bld" into the directory
       "%INFORMIXDIR%\extend\Guid" or "c:\Program Files\IBM Informix Software
       Bundle\extend\Guid". The subdirectory Guid has to be created
        The file is a component of the middleware infrastructure and is in the directory
         "%PROGRAMFILES%\A+W\Sandpiper1\InfrastructureMiddleware\Informix\x86", for 32-bit
        Informix, or
        "%PROGRAMFILES%\A+W\Sandpiper1\InfrastructureMiddleware\Informix\x64", for 64-bit
        Informix
    2. The file GUID.BLD must have set the write-protect attribute.
    3. Setup of the function with the Informix tool dbaccess The user must be a
       member of the "Informix administrators" group. The command is in the file
       guid.sql in addition to the guid.bld file
             CREATE FUNCTION makeguid()
             RETURNING lvarchar
             WITH(VARIANT, PARALLELIZABLE)
             EXTERNAL NAME "$INFORMIXDIR/extend/guid/guid.bld(makeguid)"
             LANGUAGE C;


    4. After the installation of the function, it should be tested once manually:

             EXECUTE FUNCTION makeguid();



        For a successful test, the call must return a GUID. If there is an error, it must
        be eliminated.


Do not execute, only for info: in order to delete the function again, the command

 DROP FUNCTION makeguid();


must be executed.
For database access to Informix, an ODBC system DSN must be created with the
Informix ODBC. For this, an existing connection from A+W Production can be used.


Preparation of Oracle
For Oracle, the Oracle client has to be installed as well as an ODBC system DSN.

1.4 Installation of server components
For the installation, please proceed in the following sequence:


11.10.2023                            EN-INST-A+W iQuote.docx                           10
Start the Setup Launcher and generate a new diskset or expand an existing one. An
autoupdate installation should be the standard installation method for the
infrastructure services. Please read the installation instructions for the Setup
Launcher. Check the diskset directory, the installation drive, and the hotfix path for
correct values.




1. Confirm configuration in the main dialog by pressing Next.
2. Now the installed components are shown; proceed to the Next button.
3. In the component selection view under A+W Common, now select the components
        •    A+W Infrastructure 6 Services
        •    A+W Infrastructure 6 Web
        •    A+W iQuote 6 Services
        •    A+W iQuote 6 Web
        •    A+W Commercial 6 Business Services
        •    A+W Business 6 Basis
    off. All further components are automatically selected as dependencies.
4. Now the connection to the Service Locator must be configured. For the host, enter
   the name of the computer on which the Service Locator was installed. The port is
   always12000.




11.10.2023                           EN-INST-A+W iQuote.docx                        11
5. On the next dialog, you can determine under which user the services will run. With
   a click on the Browse... button, the Windows user selection is started in order to
   make entry easier.




    Here the user should coordinate the services with the user of the A+W Business



11.10.2023                       EN-INST-A+W iQuote.docx                           12
6. You can now save the configuration and start the installation. To do this, click the
   Next button.
7. After completion of the installation, the configuration of the components begins.
   For this, create the database connection first.
    Basically, inventory databases should be used from ERP or PPS. Since there are
    currently only applications in production, the production database should be
    preferred. If it is an ERP standalone installation, the ERP database can be
    selected. In the case of an SQLBase, the SQL Server Express has to be installed
    and an empty database created there.




    Type: select between SQLServer, Oracle or Informix as database system
    Server Instance: enter the instance of the database server
    User: select the database user
    Password: enter the user password
    Database: specify the database name
    For the SQLServer, you can search for this information using the combo boxes.
    After entering the data, click the Next button and the configuration now checks the
    database connection.




11.10.2023                        EN-INST-A+W iQuote.docx                            13
8. Now we will show you the multisite configuration for the Commercial Service. With
   this, you can determine for which sites a service should be activated and how
   many workers per site should be active. The workers function as load distribution
   instances per site. The basis is that in several sites are entered in the
   infrastructure.




    The service for this site can be activated in the "Active" property.
    The number of workers for the load distribution must be specified in the "Worker"
    property. This must be at least 1 worker.
    Special feature: if no "Active" property is set, the service will nevertheless be
    installed for the site 1. The number of workers can also be determined here. This
    type of installation is always needed if A+W iQuote is not installed for multiple sites;
    it is the default.




9. The CAD designer must still be configured for use in services. To do this, start the
   configuration program of the CAD designer and specify the user of the commercial
   services as the service user.




11.10.2023                          EN-INST-A+W iQuote.docx                               14
    Start with Run as admin.




    Here, enter the user from Step 5, who starts the commercial service.


Thus the installation and configuration is complete and the application can be used.


11.10.2023                        EN-INST-A+W iQuote.docx                          15
11.10.2023   EN-INST-A+W iQuote.docx   16
1.5 HTTPS configuration of the IIS
For security reasons, the Web components should always be installed with SSL
encryption via HTTPS. This is not done through the setup. Here the IIS administrator
must perform the additional set-up.
The installation of the certificate is done for the default site and is thus not restricted
to just one webservice. It is retained even in case of an update. It must therefore be
done once manually before the expiration of the certificate.
An SSL certificate must be made available by the client. Temporarily, a local
certificate can be created; however this cannot be used from the outside in real
operation.
Start the IIS Manager and mark under (1) the server, now double-click the (2) server
certificates




In order to import a real certificate, go to Import.
To create a self-signed test certificate, go to Create a Self-Signed Certificate




11.10.2023                          EN-INST-A+W iQuote.docx                               17
Give the certificate a meaningful name and specify Web hosting as the storage location




Now mark the Default site (1) and select the Bindings (2)




11.10.2023                          EN-INST-A+W iQuote.docx                              18
Now the binding for HTTPS must be added. To do this, click the Add button and set the type
to HTTPS and the SSL certificate to the previously-created certificate.




The "Host name" has to match the certificate and the URL that is called. You can verify this
with the Button view.




11.10.2023                           EN-INST-A+W iQuote.docx                               19
Now all sites can be surfed with https. Please note that you must apply for the certificate
from an authorization office. A+W cannot include this in the delivery since it represents a
position of trust of the Website operator.




11.10.2023                           EN-INST-A+W iQuote.docx                                  20
1.6 Configuration of the firewall for the DMZ
If the iQuote is installed in a DMZ (addressable from the Internet), then only the
package "A+W Infrastructure 6 Middleware" and "A+W iQuote 6 Web" must be
installed on the server in the DMZ.
The ports 12000-12005 TCP and 65230-65235 TCP are opened by the installation
of the middleware in the Windows firewall.
Since this computer is in the DMZ, however, there is probably another hardware
firewall; the ports above must also be enabled there.
However, this enabling should be limited to the target address of the process
server and the source address of the DMZ server.
The firewall must be opened to the Internet for port 80, otherwise the IIS cannot be
reached.




                       :80                           :12000
                                                     -12005
                                                        +
                                                     :65230
                                                     -65235




All services must be installed on the process computer; here only the installation of
the "A+W Web 6 Web" can be omitted.




11.10.2023                        EN-INST-A+W iQuote.docx                               21
1.7 Variants of implementation
iQuote can currently be brought out in 2 ways. As a mere in-house solution or as an
ASP.Net application hosted by a provider with connection to the services via a VPN
connection between provider and customer system.
A mere provider-hosted solution is not available at present, this requires both a
master data and a document replication.
1.7.1 In-house Hosting
All components are in the company. The IIS must be located in the DMZ. The services are
behind a second firewall on a server in the network.
This variant requires a license for the Windows server in the DMZ and a Core license of the
database. Please make sure, that the IIS can be addressed via Internet with sufficient
bandwidth.




      Browser
      IE10++,                        IIS
       Safari,                     ASP.Net                         Services
      Firefox,                      MVC5
      Chrome




                                                                     ERP
                                                                     DB
                                  Win Server
                                                                 Process-/DB -
                                     DMZ                            Server

                                                      In-house




11.10.2023                          EN-INST-A+W iQuote.docx                               22
1.7.2 Hoster with VPN In-house
For this variant, the IIS is transferred to the hoster and the services are addressed via VPN
connection. In this case, the hoster is responsible for the Windows Server licenses. The
bandwidth of the hoster is decisive, but, the bandwidth of the VPN connection must be
sufficient, too.
Normally, only the SQLServer Core licenses are necessary.




       Browser
       IE10++,                           IIS
        Safari,                        ASP.Net                         Services
       Firefox,                         MVC5
       Chrome                                                  VPN




                                                                          ERP
                                                                          DB
                                                                       Process-/
                                      Root Server                     DB - Server

                                         Hoster                        In-house




11.10.2023                           EN-INST-A+W iQuote.docx                                23
1.8 Call of the application
The application has installed itself in the A+W directory.




It is started with a double-click.
The Infrastructure 6 Config Tool and also the Service Locator Administrator are in
the Config Tools subfolder.




11.10.2023                           EN-INST-A+W iQuote.docx                         24
1.9 Setting up access to the Service Locator
The first time you enter the Service Locator Administrator, you must establish the
connection.




To do so, please select the direct connection


11.10.2023                        EN-INST-A+W iQuote.docx                            25
Now specify the name of the instance. CAUTION: lower and upper-case letters must
be heeded.




Access is made via host and port number




Enter these values that were already entered in the configuration tool.




11.10.2023                        EN-INST-A+W iQuote.docx                     26
Now specify a name for the connection. The password can remain empty, for access
is not secured.
Then when requesting the Service Locator, always press the button on the left and
select the connection.




The ICE services are depicted in the Service Locator; they can be started and
stopped here. However, under normal circumstances this is not necessary, for they
start automatically if needed.




11.10.2023                       EN-INST-A+W iQuote.docx                            27
1.10 Incompatibilities
No incompatibilities are known.

1.11 Directory structure
The application installs itself completely under
C:\Program Files\A+W\Sandpiper1




11.10.2023                         EN-INST-A+W iQuote.docx   28
1.12 Tips and tricks
1.12.1 FAQs
My services are not displayed in the Service Locator.
For this, you must check whether the service nodes are running in the Windows
Services.




Application no longer starts "No switches were loaded for client xxx."
If the first site was entered in the site management, this error occurs sporadically.
Please reboot the server, then it will work again. The pages are cached on the IIS
and so the newly-created site is not found. Up to now, there is no other solution.


1.12.2 Web front end does not get a connection to the services
If the DNS name resolution does not work in the Service Locator, the address of
the Service Locator should be entered with the IP address and not as name.
With the Telnet (add Windows components), you can check whether the services
are accessible through the firewall.
To do this, call telnet <computername> <port>.
The port numbers are:
12000-12005 and 65230-65235




11.10.2023                        EN-INST-A+W iQuote.docx                               29
1.12.3 The document service cannot be started
If this occurs after the installation, an explicit user should be entered for the
Business COM object. This user is queried during the Business installation, but can
be changed after the fact.




The user of the Windows services for the commercial service node can be set to another
user. This can lead to the solution of the problem.




11.10.2023                         EN-INST-A+W iQuote.docx                               30
1.12.4 Error analysis in the browser
Internet Explorer
Checking for IE11/10
Please check on the About dialog whether you are really using IE11/10. iQuote will not run
with older browsers < IE10; we recommend that you use IE11.




Javascript active
iQuote needs JavaScript in order to display the HTML pages correctly.
On the settings dialog, go to Internet options and check whether Active scripting is
activated.




11.10.2023                           EN-INST-A+W iQuote.docx                                 31
Cookies
Please check whether the browser settings allow the saving of cookies. Adjust the general
settings to medium or use additional settings to control the individual settings of the cookie
properties.




Network protocol
If the problems still exist, then activate the network protocol.
Please start Internet Explorer and press F12




11.10.2023                             EN-INST-A+W iQuote.docx                                   32
Activate the Network tab and start the protocol by clicking the green arrow.

Now enter the URL for iQuote and confirm with Enter




Now you will see all queries to iQuote; please send these to A+W Service or analyze the
situation independently. The Result column provides information about any errors.




11.10.2023                           EN-INST-A+W iQuote.docx                              33
1.12.5 Copying the SOA tables into a new or existing database

    1. Create the scripts for all SOA tables on the source database




    2. Select all SOA tables, please make sure that all of them are really selected




    3. Select the query window as output




11.10.2023                           EN-INST-A+W iQuote.docx                          34
    4. Now change the target database in the script




    5. Mark all commands of the script for execution up to the first old table WITH
       FOREIGN KEY!!!




11.10.2023                           EN-INST-A+W iQuote.docx                          35
    6. Now the data is exported from the source database




    7. Select the source and target database with the Native Client 10/11




11.10.2023                          EN-INST-A+W iQuote.docx                 36
    8. Select all tables that were created anew previously and transfer the data




    9. The last step is the creation of the foreign keys in the target database




    10. Now the SOA tables are copied into the target database!!!




11.10.2023                           EN-INST-A+W iQuote.docx                       37
    11. Don't forget to change the SOA database with the infrastructure config tool!




11.10.2023                           EN-INST-A+W iQuote.docx                           38
1.12.6 Internet Explorer Trusted Sites
On Windows Server 2012 R2 and higher, the domain must be taken into the trusted sites or
defined as local side, alternatively Both are made in the Internet options of the Internet
Explorer.




If this is not made, e.g. the icons are not displayed or other errors occur when security-
relevant functions are executed.

Calling iQuote without domain specification handles the problem, but is not possible on all
systems.




11.10.2023                            EN-INST-A+W iQuote.docx                                 39
1.13 Uninstalling
To uninstall the software, user the Windows program management. Here, make sure
to adhere to the sequence. The Service Locator must be uninstalled as the next-to-
last and the middleware as the last program.




11.10.2023                      EN-INST-A+W iQuote.docx                         40
1.14 A+W Licenses
There are 2 license modules for iQuote. On the one hand, there is the iQuote
configurator; it allows the configuration and use of the info(history) module.
There is also just the iQuote info module. This allows only the use of the information
area, with no possibility for configuration.




11.10.2023                        EN-INST-A+W iQuote.docx                            41
2 System configuration
2.1 Configuration of IIS
In order to achieve optimal performance of the Web page, it is necessary to make
some settings in the IIS. These affect the performance until the start page is
displayed (JIT compiler) and whether the IIS puts the worker process to sleep.
In the AppPool "Web.WebAppPool," the start mode must be set to "AlwaysRunning."
The idle time-out must be set to 0.




On the site Web.Web, the Preload enabled option must be set to True in the
Advanced Settings.




11.10.2023                       EN-INST-A+W iQuote.docx                           42
CAUTION: It must be heeded that the "Preload enabled" setting is currently
lost with each update.




11.10.2023                    EN-INST-A+W iQuote.docx                        43
2.2 Browser cache and content reload
The iQuote installation changes the IIS settings of the iQuote website. The http
response header is set so that, for example, JPGs are reloaded after an hour and
not drawn from the browser cache. However, this is only the case when the browser
is restarted.




Thanks to this change, the customer can change images and these also reach the
user; otherwise the user would have to delete the browser cache by hand. These
settings are in the web.config of the default site.




11.10.2023                      EN-INST-A+W iQuote.docx                          44
3 Breaking Changes
It will be listed below with which versions there were breaking changes and which
updates have to be made together. For a complete update of all modules, this is not
relevant. Incompatibilities and re-configurations always only affect partial updates of
the software.

3.1 2-phase commit when saving the orders 13.04.3924
        With this version, it has been prevented that the orders are created twice.
        The following modules have to be updated:
        A+W Business 6 Basis                                 13.04.1039 ++
        A+W Commercial 6 Document Services                   13.04.3924 ++
        A+W iQuote 6 Services                                13.04.3924 ++
        A+W iQuote 6 Web                                     13.04.3924 ++




11.10.2023                         EN-INST-A+W iQuote.docx                            45
4 Login page installation
4.1 Requirements
The login page must be installed on an IIS that is in the DMZ. A SQLServer must
also be installed on this computer. A SQLServer Express is sufficient. Before the
installation, an empty database must be created on the SQLServer. This database
serves the login provider for saving the login data. The customer passwords are
saved only as hash in this database and cannot be decrypted; they are only known
to the customer.
The user of the IIS application pool must have access to the login database!
The port for the service access must be opened in an existing firewall; the service
has a fixed port number like all iQuote services.


    •   IIS in the DMZ
    •   Installation SQLServer (Express), mixed authentication recommended
    •   Create an empty database
    •   The user of the IIS application pool must have access or use SQLServer
        authentication
    •   Provide Installation Setup Launcher and diskset




    •   Open the port 65215 for access to the multisite service

According to these prerequisites, the installation with the Setup Launcher can begin on the
IIS server and the process server. The Setup Launcher must also be installed and the
diskset must be in the access. In the DMZ, this can mean that the diskset must be stored
locally!




11.10.2023                          EN-INST-A+W iQuote.docx                                   46
4.2 Architecture
The login page like all iQuote IIS must be accessible from the Internet and therefore
in the DMZ. The SQLServer for the login data must also be installed there; it may
only save the user's login data and it can be a free SQL Server Express.
The multisite service is installed on the process server, for it must have access to
the mailserver.
The main IIS can be one of the cluster IISes; an individual IIS is not necessary for
this.

                                    Cluster 1 IIS

                                   iQuote site I
         Main IIS
                                    iQuote site II



       Login page
                                    Cluster 2 IIS
                                                            Firewall




                                  iQuote site III

                                    iQuote site IV

      Admin page
     assignment to
      iQuote site                                                      Process Server



                                   Port 65215
                                                                          Multisite
                                                                          Service
      Login Provider
        Database




11.10.2023                        EN-INST-A+W iQuote.docx                               47
4.3 Installation
To simplify the installation, here all components are installed together; of course
this is not done in the productive environment.




The A+W iQuote 6 Multisite installation package is the login page and it must be
installed on the IIS in the DMZ.
The service must be installed on the process computer.




The user for the Multisite Service must be entered; the service node runs under
this user.


11.10.2023                        EN-INST-A+W iQuote.docx                             48
For installation of the web page, access to the login database must be configured.




After the installation, the login page must be called up via the icon on the A+W start
menu. The configuration process is described in detail in the A+W iQuote
configuration instructions.




11.10.2023                         EN-INST-A+W iQuote.docx                               49

