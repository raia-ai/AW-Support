---
description: "EN INST A+W Enterprise iQuote"
---



# EN INST A+W Enterprise iQuote

          Installation Instructions

          A+W iQuote for A+W Enterprise
   Change history:
     Date            Edited by        Remarks
     2021-10-18      A. Weil          Transfer from A+W Business document
     2021-11-12      A. Weil          Continuation of the A+W Enterprise-relevant data




     The installation instructions will assist the planner with the installation and
     configuration process for the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




12.04.2022                           EN-INST-A+W Enterprise iQuote.docx                  1
Contents

   Installation Instructions .................................................................... 1

   A+W iQuote for A+W Enterprise ...................................................... 1

   1         New installation of version 6 ................................................. 4
   1.1       Overview and the basics ...........................................................................4
   1.2       Time requirement ......................................................................................4
   1.3       Requirements ............................................................................................4
   1.3.1     Hardware Frontend....................................................................................4
   1.3.2     Hardware Backend ....................................................................................4
   1.3.3     Network .....................................................................................................4
   1.3.4     Installation account ....................................................................................5
   1.3.5     Software ....................................................................................................7
   1.4       Installation of server components ............................................................12
   1.5       Installation of the Backend components ..................................................22
   1.6       HTTPS configuration of the IIS ................................................................25
   1.7       Configuration of the firewall for the DMZ .................................................29
   1.8       Variants of implementation ......................................................................30
   1.8.1     In-house Hosting .....................................................................................30
   1.8.2     Hoster with VPN In-house .......................................................................31
   1.9       Call of the application ..............................................................................32
   1.10      Setting up access to the Service Locator ................................................33
   1.11      Incompatibilities .......................................................................................36
   1.12      Directory structure ...................................................................................36
   1.13      Tips and tricks .........................................................................................37
   1.13.1    FAQs .......................................................................................................37
   1.13.2    Web front end does not get a connection to the services ........................37
   1.13.3    Error analysis in the browser ...................................................................37
   1.13.4    Copying the SOA tables into a new or existing database ........................41
   1.13.5    Internet Explorer Trusted Sites ................................................................46
   1.14      Uninstalling ..............................................................................................47
   1.15      A+W Licenses .........................................................................................48

   2         System configuration ........................................................... 49
   2.1       Configuration of IIS ..................................................................................49
   2.2       Browser cache and content reload ..........................................................51


12.04.2022                               EN-INST-A+W Enterprise iQuote.docx                                              2
12.04.2022   EN-INST-A+W Enterprise iQuote.docx   3
1 New installation of version 6
The following installation instructions assume that there is no previous version
installed.
For all modules of the SOA, only a Version 6 is provided; these are the basis for the
installation.
After installation, please consult the EN-Config-A+W Enterprise instructions for
further set-up instructions.

1.1 Overview and the basics
The following list provides an overview of the work that must be done during
installation:
    -   Installation .Net Framework 4.5 or 4.8 (status as of May 2021)
    -   Installation Internet Information Service IIS >=7
    -   Installation of the database client software
    -   Creation of the database if no inventory database is used
    -   Installation of the software with the Setup Launcher
    -   Installation of the A+W Enterprise 6 Web
    -   Installation of the A+W Infrastructure 6
    -   Activation of A+W License iQuote Configurator / Info
    -   Installation of the ICE environment on the Unix back end
    -   Installation of documentservice (back end)

1.2 Time requirement
The time requirement will be approx. 120 minutes for the creation of the
prerequisites and the actual installation. There is no conversion of data stocks

1.3 Requirements
1.3.1 Hardware Frontend
Computer with Windows Server operating system Windows Server 2008 or higher
are approved in emergency situations and workstation installations will support the
installation starting with Windows 7. The latest service packs and operating systems
from Microsoft must always be installed.
1.3.2 Hardware Backend
Under Linux, the version Redhat ES 7 is required. (File: /etc/redhat-release)
For AIX, the Version 7.2 is required.
1.3.3 Network
The installation of the A+W infrastructure services is a prerequisite.




12.04.2022                       EN-INST-A+W Enterprise iQuote.docx                     4
ICE services communicate via the ports 12000-12005 TCP + 65230-65235 TCP,
which have to be opened in the network. The installation opens these in the
Windows firewall of its own accord. If other firewall programs are used, then the
ports must be opened manually there.
PLEAE NOTE: A connection has to be established to the A+W FTP Service (port
25). Without this, the download of the SQL scripts cannot occur and the database
update service cannot initialize and update the database. The connection is
configured in the auto update of the Setup Launcher. The installation with local
update scripts is possible, but it requires the constant manual updating of the scripts.


1.3.4 Installation account
For the installation, a user with administration rights must be used. If there is a
MUI/Language pack installation of the Windows system, for this user the installation
language of the system must be set as primary language since otherwise the
internal users will not be recognized correctly during the installation of the ICE
services
(Could not retrieve Security ID for NT-AUTORITHÄT\SYSTEM: No mapping
between account names and security IDs was carried out.).




12.04.2022                     EN-INST-A+W Enterprise iQuote.docx                      5
12.04.2022   EN-INST-A+W Enterprise iQuote.docx   6
1.3.5 Software
1.3.5.1 A+W Software
Prerequisite is a complete installation of the following Windows components:
A+W Enterprise 6 Frontend
A+W Infrastructure 6
A+W CAD 6 Services
A+W CAD Designer (Shapes)
A+W CAD Designer (Bars)
A+W Commercial 6 Converter Services
A+W iQuote 6 Services
A+W iQuote 6 Web


Prerequisite is a complete installation of the following Unix components:
documentservice


1.3.5.2 Unix back end ICE – environment
Prerequisite and installation of the ICE environment
    •   Under Linux, the version Redhat ES 7 is required. (File: /etc/redhat-release)
    •   For AIX, the Version 7.2 is required.
    •   The ICE repositories must be installed:
        1. Check whether repository for ICE is present on the system (as root)

             yum provides ice-all-runtime

             In the version, the packages ice-all-runtime-3.7.3-1.el7.i686 and ice-all-runtime-3.7.3-
             1.el7.x86_64 should be present. If the packages are not present, they must be downloaded
             with the commands from 2.

        2. Supply if the packages are not present (log in again as root)

             cd /etc/yum.repos.d

             wget https://zeroc.com/download/Ice/3.7/el7/zeroc-ice3.7.repo

        3. ICE installation (as root)

                     a. Installation of the ICE binaries and the 64-bit libraries:

                         yum install ice-all-runtime-3.7.4-1.el7

                     b. Manual reinstallation of the ICE 32-bit libraries:



12.04.2022                           EN-INST-A+W Enterprise iQuote.docx                            7
                         yum install libice3.7-c++.i686

        4. If the installation reports problems, the missing packages must be installed after the fact.

             On systems without Redhad subscription, these can be obtained after the change in the
             directory /tmp with:

             wget http://mirror.centos.org/centos/7/os/x86_64/Packages/packagename

             and installed there with:

             yum update *.rpm.



    •   For Linux 8:
        1. Supply of the repository:

             cd /etc/yum.repos.d

             rpm -i https://zeroc.com/download/ice/3.7/el7/ice-repo-3.7.el7.noarch.rpm

        2. The packages then have to be installed individually:

             yum install icegrid-3.7.4-1.el7.x86_64 – if this doesn't work, please try „yum install ice-
             all-runtime-3.7.4-1.el7.x86_64“

             yum install libice3.7-c++-3.7.4-1.el7.i686



    •   For AIX 7.2:
        1. Supply of the repository:

             yum             install                 https://zeroc.com/download/ice/3.7/aix7.2/ice-repo-
             3.7.aix7.2.noarch.rpm

        2. Installation of the ICE binaries:

             yum install ice-all-runtime

Configuration instructions: 10. ICE environment


1.3.5.3 .Net Framework 4.5 or 4.8
The framework is installed automatically by the Setup Launcher.
The complete services were upgraded to Framework 4.8 in April 2021. If an
installation or an update should be done starting from this point, then all components
must be reinstalled so that there is no framework difference.


1.3.5.4 Internet Information Service
The IIS (Version 7 or higher) must be installed.


12.04.2022                               EN-INST-A+W Enterprise iQuote.docx                               8
If the .Net Framework 4 was installed prior to the IIS, it may occur that the required
Asp.Net 4.0 AppPools cannot be created correctly.
Please check this in IIS management under the application pools. Normally, this is
not necessary.




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




12.04.2022                     EN-INST-A+W Enterprise iQuote.docx                        9
Caution: Starting with Version v6 Update 4, the performance features must be installed.
Since we have also activated the compression for dynamic content.




12.04.2022                     EN-INST-A+W Enterprise iQuote.docx                         10
1.3.5.5 Windows Server operating system
If the user directly requests the web interface on a Windows Server operating
system, the "Internet Explorer Advanced Security Configuration" has to be disabled.




1.3.5.6 Databases and clients
The following database clients are approved for the SOA services
    •   Microsoft SQL Server 2008 R2 Native Client or newer
    •   Oracle 11g R2 Client Win32
    •   IBM Informix Client-SDK (32-bit) 3.50
The 32-bit version is always used, A+W does not support any 64-bit database
drivers.
The back end database must be installed according to the prerequisites of A+W
Enterprise.
Preparation of SQLServer
Here, only the native client must be installed; there is no need for configuration of
the client software. Access can be tested with a file with the extension .uld; these
can be created on the desktop and access to the SQL Server tested.
Preparation of Informix
Informix does not support Guids. Since, however, in stock databases a GUID
column is also created in existing tables. A function makeguid must be installed in
Informix. For this, the following steps must be executed before the installation of the
infrastructure services:
    1. On the database server, copy the file "guid.bld" into the directory
       "%INFORMIXDIR%\extend\Guid" or "c:\Program Files\IBM Informix Software
       Bundle\extend\Guid". The subdirectory Guid has to be created


12.04.2022                     EN-INST-A+W Enterprise iQuote.docx                       11
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
Start the Setup Launcher and generate a new diskset or expand an existing one. An
autoupdate installation should be the standard installation method for the
infrastructure services. Please read the installation instructions for the Setup


12.04.2022                         EN-INST-A+W Enterprise iQuote.docx                   12
Launcher. Check the diskset directory, the installation drive, and the hotfix path for
correct values.




1. Confirm configuration in the main dialog by pressing Next.
2. Now the installed components are shown; proceed to the Next button.
    In the component selection view under A+W Common, now select the components
        •    A+W CAD 6 Services
        •    A+W CAD Designer (Shapes)
        •    A+W CAD Designer (Bars)
        •    A+W Commercial 6 Converter Services
        •    A+W Infrastructure 6 Services
        •    A+W Infrastructure 6 Web
        •    A+W Infrastructure 6 Workflow Studio
        •    A+W iQuote 6 Services
        •    A+W iQuote 6 Web
    All further components are automatically selected as dependencies.


3. Now the connection to the Service Locator must be configured. For the host, enter
   the name of the computer on which the Service Locator was installed. The port is
   always12000.



12.04.2022                      EN-INST-A+W Enterprise iQuote.docx                  13
4. On the next dialog, you can determine under which user the services will run. With
   a click on the "Browse..." button, the Windows user selection is started in order to
   make entry easier.




12.04.2022                    EN-INST-A+W Enterprise iQuote.docx                     14
    Here the user should coordinate the services with the user of other A+W services.
5. Service number of the Web\Configurator is always 1.




12.04.2022                    EN-INST-A+W Enterprise iQuote.docx                   15
    (Old status: before 03/15/2022)


6. You can now save the configuration and start the installation. To do this, click the
   Next button.
7. After completion of the installation, the configuration of the components begins.
   For this, create the database connection first.
    Basically, inventory databases should be used from ERP or PPS. Since there are
    currently only applications in production, the production database should be
    preferred. If it is an ERP standalone installation, the ERP database can be
    selected.




12.04.2022                    EN-INST-A+W Enterprise iQuote.docx                     16
    Type: select between SQLServer, Oracle or Informix as database system
    Server Instance: enter the instance of the database server
    User: select the database user
    Password: enter the user password
    Database: specify the database name
    For the SQLServer, you can search for this information using the combo boxes.
    For Informix or Oracle, an ODBC connection must be created.
    After entering the data, click the Next button and the configuration now checks the
    database connection.




12.04.2022                     EN-INST-A+W Enterprise iQuote.docx                    17
8. The CAD designer must still be configured for use in services. To do this, start the
   configuration program of the CAD designer and specify the user of the commercial
   services as the service user.




12.04.2022                    EN-INST-A+W Enterprise iQuote.docx                     18
    Start with Run as admin.




12.04.2022                     EN-INST-A+W Enterprise iQuote.docx   19
    Here, enter the user from Step 4, who starts the commercial service.
9. A+W iQuote Services Config
    Here, the site are read from the Infrastructure.Web > Master Data and suggested
    as multi-site client.
    If you would like to set up a multisite, then set each Site active = true and set a
    number of workers (standard number = 1).
    The start port number indicates starting when the portrange will be started. In the
    example below 65235. This number is incremented for each site and worker.
    Startport is mandatory and it must also be approved in case of firewalls, etc.




12.04.2022                      EN-INST-A+W Enterprise iQuote.docx                        20
    If no multisite is desired, you set all sites to active = false.


10. A+W iQuote Web Config
    Here, you can select the shortcuts for the desktop variant if you have set up
    multiple sites. A shortcut is always generated without site number.




12.04.2022                       EN-INST-A+W Enterprise iQuote.docx                 21
Thus the installation and configuration for Windows is complete. To be able to use
the application, the documentservice must be installed.

1.5 Installation of the Backend components
A+W programs with ICE communication include client applications that have to
connect to the A+W Service Locator (Ice Grid Admin). The client application draws
the connection data from the A+W Service Locator in order to connect to other ICE



12.04.2022                   EN-INST-A+W Enterprise iQuote.docx                      22
servers. The A+W Service Locator starts the required server automatically if
necessary.
The A+W Service Locator is the name of the computer on which the (Windows)
service "A+W Infrastructure 6 Service Locator" is running.
A+W Enterprise components that run under Unix require the alenv environment
variables in order to reach the A+W services in Windows. These include, e.g. the
dispatch control, the A+W LogisticBackEndService or the A+W Documentservice.
These environment variables must be set up:
    •   AWSOA_ICEHOST  Name of the host on which the A+W Service Locator is
        running
    •   AWSOA_ICEPORT  Port on which the A+W Service Locator can be
        reached (default: 12000)
For better research, the following environment variables should be set:
    •   AWSOA_LOGLEVEL_DOCUMENTSERVICE  Log-Level (1-4)
             o Status as of 11/12/21: please set Level 4
    •   AWSOAFTEST  FTest Level for ll A+W SOA services (1-9)


The current A+W Documentservice should be stored in the familiar Bin directory.
To enter the A+W Documentservice in the A+W Service Locator, the script iceconfig
(cdcmd) must be used. For this, the package iceconfig-1.0.gz must exist in the
scripts directory ($ALCIBPRG/install/config/). The script generates under the
$ALDATPFAD/iceconfig a folder with the Unix computer names and under this
folder, the Service Config files are accommodated, the ones that are required for
communication with the target computer and the A+W Service Locator.
Under /etc/hosts, the IP address of the host computer must be entered.
Now execute the script iceconfig. It checks the existing settings
(AWOSA_ICEHOST, AWSOA_ICEPORT), queries all the information required for
configuration, and registers the applications, here the A+W Documentservice, in the
A+W Service Locator under Windows.




12.04.2022                      EN-INST-A+W Enterprise iQuote.docx                 23
Thus, the environment as well as for the A+W iQuote application can be configured.
Important for communication between the registry under Windows and the
clients and server under Unix is that the firewall does not hinder the
communication.
For the purpose of testing, the firewall can be deactivated with "systemctl
stop firewalld" and systemctl disable firewalld" as root under Linux.
Starting the registry node (icegridnode) for the Unix services is enabled via the script
"icenodestart" (cdcmd). A stop of the node can be forced with the script
"icenodestop."
Windows settings with regard to communication with Unix
The A+W services, such as the A+W Logistics Optimizer and A+W iQuote, run
under Microsoft Windows and draw the connection dat from the Microsoft registry.
With these settings, the connection to the A+W Service Locator Administrator is
established.
This setting data is entered in the course of A+W setup and can be checked in the
registry:
HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\Albat+Wirsam\Communicat
ion

-     IceHost              Name of the host on which the A+W Service Locator
Administrator is running



12.04.2022                     EN-INST-A+W Enterprise iQuote.docx                     24
-      IcePort            Port on which the A+W Service Locator Administrator can
be reached (default: 12000)

1.6 HTTPS configuration of the IIS
For security reasons, the Web components should always be installed with SSL
encryption via HTTPS. This is not done through the setup. Here the IIS administrator
must perform the additional set-up.
The installation of the certificate is done for the default site and is thus not restricted
to just one webservice. It is retained even in case of an update. It must therefore be
done once manually before the expiration of the certificate.
An SSL certificate must be made available by the client. Temporarily, a local
certificate can be created; however, it cannot be used from the outside in real
operation.
Start the IIS Manager and mark the server under (1), then double-click the (2) server
certificates




In order to import a real certificate, go to Import.
To create a self-signed test certificate, go to Create a Self-Signed Certificate




12.04.2022                      EN-INST-A+W Enterprise iQuote.docx                        25
Give the certificate a meaningful name and specify Web hosting as the storage location




Now mark the Default site (1) and select the Bindings (2)




12.04.2022                      EN-INST-A+W Enterprise iQuote.docx                       26
Now the binding for HTTPS must be added. To do this, click the Add button and set the type
to HTTPS and the SSL certificate to the previously-created certificate.




The "Host name" has to match the certificate and the URL that is called. You can verify this
with the Button view.




12.04.2022                      EN-INST-A+W Enterprise iQuote.docx                         27
Now all sites can be surfed with https. Please note that you must apply for the certificate
from an authorization office. A+W cannot include this in the delivery since it represents a
position of trust of the Website operator.




12.04.2022                       EN-INST-A+W Enterprise iQuote.docx                           28
1.7 Configuration of the firewall for the DMZ
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




                       :80                            :12000
                                                      -12005
                                                         +
                                                      :65230
                                                      -65235




All services must be installed on the process computer; here only the installation of
the "A+W Web 6 Web" can be omitted.




12.04.2022                    EN-INST-A+W Enterprise iQuote.docx                        29
1.8 Variants of implementation
A+W iQuote can currently be brought out in 2 ways. As a mere in-house solution or
as an ASP.Net application hosted by a provider with connection to the services via a
VPN connection between provider and customer system.
A mere provider-hosted solution is not available at present, this requires both a
master data and a document replication.
1.8.1 In-house Hosting
All components are in the company. The IIS must be located in the DMZ. The services are
behind a second firewall on a server in the network.
This variant requires a license for the Windows server in the DMZ and a Core license of the
database. Please make sure, that the IIS can be addressed via Internet with sufficient
bandwidth.




      Browser
      IE10++,                        IIS
       Safari,                     ASP.Net                             Services
      Firefox,                      MVC5
      Chrome




                                                                         ERP
                                                                         DB
                                  Win Server
                                                                     Process-/DB -
                                      DMZ                               Server

                                                        In-house




12.04.2022                      EN-INST-A+W Enterprise iQuote.docx                        30
1.8.2 Hoster with VPN In-house
For this variant, the IIS is transferred to the hoster and the services are addressed via VPN
connection. In this case, the hoster is responsible for the Windows Server licenses. The
bandwidth of the hoster is decisive, but, the bandwidth of the VPN connection must be
sufficient, too.
Normally, only the SQLServer Core licenses are necessary.




       Browser
       IE10++,                            IIS
        Safari,                         ASP.Net                        Services
       Firefox,                          MVC5
       Chrome                                                 VPN




                                                                          ERP
                                                                          DB
                                                                       Process-/
                                      Root Server                     DB - Server

                                          Hoster                       In-house




12.04.2022                       EN-INST-A+W Enterprise iQuote.docx                         31
1.9 Call of the application
The application has installed itself in the A+W directory.




It is started with a double-click.
The Infrastructure 6 Config Tool and also the Service Locator Administrator are in
the Config Tools subfolder.




12.04.2022                       EN-INST-A+W Enterprise iQuote.docx                  32
1.10 Setting up access to the Service Locator
The first time you enter the Service Locator Administrator, you must establish the
connection.




To do so, please select the direct connection


12.04.2022                    EN-INST-A+W Enterprise iQuote.docx                     33
Now specify the name of the instance. CAUTION: lower and upper-case letters must
be heeded.




Access is made via host and port number




Enter these values that were already entered in the configuration tool.




12.04.2022                    EN-INST-A+W Enterprise iQuote.docx              34
Now specify a name for the connection. The password can remain empty, for access
is not secured.
Then when requesting the Service Locator, always press the button on the left and
select the connection.




The ICE services are depicted in the Service Locator; they can be started and
stopped here. However, under normal circumstances this is not necessary, for they
start automatically if needed.




12.04.2022                   EN-INST-A+W Enterprise iQuote.docx                     35
1.11 Incompatibilities
No incompatibilities are known.

1.12 Directory structure
The application installs itself completely under
C:\Program Files\A+W\Sandpiper1




12.04.2022                     EN-INST-A+W Enterprise iQuote.docx   36
1.13 Tips and tricks
1.13.1 FAQs
My services are not displayed in the Service Locator.
For this, you must check whether the service nodes are running in the Windows
Services.




Application no longer starts "No switches were loaded for client xxx."
If the first site was entered in the site management, this error occurs sporadically.
Please reboot the server, then it will work again. The pages are cached on the IIS
and so the newly-created site is not found. Up to now, there is no other solution.


1.13.2 Web front end does not get a connection to the services
If the DNS name resolution does not work in the Service Locator, the address of
the Service Locator should be entered with the IP address and not as name.
With the Telnet (add Windows components), you can check whether the services
are accessible through the firewall.
To do this, call telnet <computername> <port>.
The port numbers are:
12000-12005 and 65230-65235


1.13.3 Error analysis in the browser
Internet Explorer




12.04.2022                     EN-INST-A+W Enterprise iQuote.docx                       37
Checking for IE11/10
Please check on the About dialog whether you are really using IE11/10. iQuote will not run
with older browsers < IE10; we recommend that you use IE11.




Javascript active
A+W iQuote needs JavaScript in order to display the HTML pages correctly.
On the settings dialog, go to Internet options and check whether "Active scripting" is
activated.




12.04.2022                       EN-INST-A+W Enterprise iQuote.docx                          38
Cookies
Please check whether the browser settings allow the saving of cookies. Adjust the general
settings to medium or use additional settings to control the individual settings of the cookie
properties.




Network protocol
If the problems still exist, then activate the network protocol.
Please start Internet Explorer and press F12




12.04.2022                        EN-INST-A+W Enterprise iQuote.docx                             39
Activate the Network tab and start the protocol by clicking the green arrow.

Now enter the URL for A+W iQuote and confirm with Enter




Now you will see all queries to iQuote; please send these to A+W Service or analyze the
situation independently. The Result column provides information about any errors.




12.04.2022                       EN-INST-A+W Enterprise iQuote.docx                       40
1.13.4 Copying the SOA tables into a new or existing database

    1. Create the scripts for all SOA tables on the source database
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




    2. Select all SOA tables, please make sure that all of them are really selected
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




    3. Select the query window as output




12.04.2022                                                                                                                                                                                                                           EN-INST-A+W Enterprise iQuote.docx   41
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




    4. Now change the target database in the script
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




    5. Mark all commands of the script for execution up to the first old table WITH
       FOREIGN KEY!!!
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




12.04.2022                                                                                                                                                                                                                           EN-INST-A+W Enterprise iQuote.docx   42
    6. Now the data is exported from the source database
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




    7. Select the source and target database with the Native Client 10/11
                                                                                                                                                                                                                                            Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.

         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




12.04.2022                                                                                                                                                                                                                           EN-INST-A+W Enterprise iQuote.docx                                                                                                                                                                                                 43
    8. Select all tables that were created anew previously and transfer the data
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.

                                                                                                                                                                                                                                                          Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




    9. The last step is the creation of the foreign keys in the target database
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




    10. Now the SOA tables are copied into the target database!!!




12.04.2022                                                                                                                                                                                                                           EN-INST-A+W Enterprise iQuote.docx                                                                                                                                                                                                               44
    11. Don't forget to change the SOA database with the infrastructure config tool!
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




12.04.2022                                                                                                                                                                                                                           EN-INST-A+W Enterprise iQuote.docx   45
1.13.5 Internet Explorer Trusted Sites
On Windows Server 2012 R2 and higher, the domain must be taken into the trusted sites or
defined as local side, alternatively Both are made in the Internet options of the Internet
Explorer.




If this is not made, e.g. the icons are not displayed or other errors occur when security-
relevant functions are executed.

Calling iQuote without domain specification handles the problem, but is not possible on all
systems.




12.04.2022                       EN-INST-A+W Enterprise iQuote.docx                           46
1.14 Uninstalling
To uninstall the software, user the Windows program management. Here, make sure
to adhere to the sequence. The Service Locator must be uninstalled as the next-to-
last and the middleware as the last program.




12.04.2022                  EN-INST-A+W Enterprise iQuote.docx                  47
1.15 A+W Licenses
There are 2 license modules for iQuote. On the one hand, there is the iQuote
configurator; it allows the configuration and use of the info(history) module.
There is also just the iQuote info module. This allows only the use of the information
area, with no possibility for configuration.




12.04.2022                    EN-INST-A+W Enterprise iQuote.docx                     48
2 System configuration
2.1 Configuration of IIS
In order to achieve optimal performance of the Web page, it is necessary to make
some settings in the IIS. These affect the performance until the start page is
displayed (JIT compiler) and whether the IIS puts the worker process to sleep.
In the AppPool "Web.WebAppPool," the start mode must be set to "AlwaysRunning."
The idle time-out must be set to 0.




On the site Web.Web, the Preload enabled option must be set to True in the
Advanced Settings.




12.04.2022                   EN-INST-A+W Enterprise iQuote.docx                    49
CAUTION: It must be heeded that the "Preload enabled" setting is currently
lost with each update.




12.04.2022                 EN-INST-A+W Enterprise iQuote.docx                50
2.2 Browser cache and content reload
The iQuote installation changes the IIS settings of the iQuote website. The http
response header is set so that, for example, JPGs are reloaded after an hour and
not drawn from the browser cache. However, this is only the case when the browser
is restarted.




Thanks to this change, the customer can change images and these also reach the
user; otherwise the user would have to delete the browser cache by hand. These
settings are in the web.config of the default site.




12.04.2022                  EN-INST-A+W Enterprise iQuote.docx                   51

