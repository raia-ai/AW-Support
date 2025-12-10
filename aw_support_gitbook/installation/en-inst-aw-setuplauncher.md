---
title: "EN INST A+W SetupLauncher"
category: "installation"
product: "A+W SetupLauncher"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W SetupLauncher"]
version: "1.0"
last_updated: "2025-12-10"
description: "Operating instructions          A+W Setup Launcher         Change history:              Date       Edited by      Remarks                                    Version              2008-01-06 André Münch    Original version                           1.0.1000              2009-12-15 André Münch    Auto Update                                1.0.1001              2010-01-05 André Münch    Installation Directory                     1.0.1002              2010-05-28 André Münch    Prerequisites a"
source_file: "EN-INST-A+W SetupLauncher.pdf"
---


# EN INST A+W SetupLauncher

        Operating instructions

        A+W Setup Launcher
        Change history:
             Date       Edited by      Remarks                                    Version
             2008-01-06 André Münch    Original version                           1.0.1000
             2009-12-15 André Münch    Auto Update                                1.0.1001
             2010-01-05 André Münch    Installation Directory                     1.0.1002
             2010-05-28 André Münch    Prerequisites amended                      1.0.1003
             2011-07-21 André Münch    Client AutoUpdate (1.7) added              1.0.1004
             2013-07-22 André Münch    Inclusion of the 2012 server preparation   1.0.1005
             2013-10-08 Jens Schmidt   Unsupervised installation                  1.0.1006
             2017-01-24 Jens Schmidt   Version 6.2                                13.2
             2017-12-01 Jens Schmidt   RDSH role (3.1.1)                          13.5




2023-03-13                              EN-INST-A+W SetupLauncher.docx                       1
Content

        1    Neuinstallation.............................................................................................................................. 4
             1.1         Installationsverzeichnis .................................................................................................... 4
             1.2         Übersicht und Grundsätzliches ........................................................................................ 4
             1.3         Begriffsabgrenzung .......................................................................................................... 4
             1.4         Zeitbedarf ......................................................................................................................... 4
                         1.4.1    Installationszeit für die Software...................................................................... 4
                         1.4.2    Konvertierungszeit für Datenbestand .............................................................. 5
             1.5         Voraussetzungen.............................................................................................................. 6
                         1.5.1   Hardware .......................................................................................................... 6
                         1.5.2   Dongle............................................................................................................... 6
                         1.5.3   Netzwerk........................................................................................................... 6
                         1.5.4   Software ........................................................................................................... 6
                         1.5.5   Dienstbenutzer / Administratorrechte ............................................................. 6
             1.6         Vorgehensweise ............................................................................................................... 7
             1.7         AutoUpdate ...................................................................................................................... 14
                         1.7.1  Allgemeines ...................................................................................................... 14
                         1.7.2  Einrichtung........................................................................................................ 15
                         1.7.3  Freigabe ............................................................................................................ 18
             1.8         Inkompatibilitäten............................................................................................................ 18
             1.9         Verzeichnisstruktur des Diskset Verzeichnisses .............................................................. 18
             1.10        Manuelle Einstellungen ................................................................................................... 18
             1.11        Kommandozeilenoption und automatisierter Modus ..................................................... 19
                         1.11.1 Unbeaufsichtigte Erstinstallation ..................................................................... 19
             1.12        Ergebnis der Installation .................................................................................................. 20
             1.13        Installationsalternativen .................................................................................................. 20
             1.14        Patches ............................................................................................................................. 20
             1.15        Deinstallation ................................................................................................................... 21

        2    Update .......................................................................................................................................... 22
             2.1         Vorgehensweise ............................................................................................................... 22

        3    Vorbereitung eines Windows Server 2012 für A+W Software ..................................................... 23
             3.1         Achtung!!! ........................................................................................................................ 23
             3.2         Der Server Manager ......................................................................................................... 23
                         3.2.1    Rollen ................................................................................................................ 23
                         3.2.2    Rollendienste .................................................................................................... 23
2023-03-13                                                   EN-INST-A+W SetupLauncher.docx                                                                         2
                   3.2.3        Features ............................................................................................................ 23
                   3.2.4        Bedienung des Server Managers ...................................................................... 23
             3.3   Hinzufügen von Rollen und Features ............................................................................... 24
                   3.3.1    Serverrollen ...................................................................................................... 26
                   3.3.2    Features ............................................................................................................ 28
                   3.3.3    Rollen Dienste des Anwendungsservers (Application Server).......................... 29
                   3.3.4    Webserver Rollendienste ................................................................................. 29
                   3.3.5    Rollendienste für die Remote Desktop Services .............................................. 31
                   3.3.6    Abschluss der Konfiguration ............................................................................. 31
             3.4   Skriptgestützte Einrichtung der benötigten Windows Features...................................... 31




2023-03-13                                           EN-INST-A+W SetupLauncher.docx                                                                        3
1 New installation
The following installation instructions assume that there is no previous version installed.

1.1 Installation Directory
The following rules apply to the customer's installation directory:
    •   To create the installation directory, you can copy the entire release \\jupiter\SW_INSTALL\v6 for a
        complete installation, and save it on the customer's system in a directory called Software\A+W.
        The Software directory should be configured as a release, all users should have reading rights.
    •   If just A+W Production or A+W Business shall be installed, you can use the two scripts
        \\jupiter\SW_INSTALL\GetAWProduction6Complete.cmd or
        \\jupiter\SW_INSTALL\GetAWB6Complete.cmd to create a local copy of the installation directory,
        and copy it to the customer's system.
    •   To speed up the installation, the customer can be provided beforehand with a directory which
        includes .NET Framework 4.5 and Service Pack 1 plus Windows Installer 3.1. These can be
        installed by the customer on the system before the actual installation. This directory can be created
        by means of the script \\jupiter\SW_INSTALL\GetRequirements.cmd in order to be passed on to
        the customer.

1.2 Overview and the basics
The following list provides and overview of the work that must be done during installation:
   •    Check all requirements (for Windows 2012 Server please stick to chapter 3)
   •    Installation of the Setup Launcher:
   •    Run the Setup Launcher to install A+W software

1.3 Definition of Terms
Diskset: A diskset is the set of software packages to be installed, including their parameters.

1.4 Time Required
If all requirements are checked and fulfilled, the following times are required for the installation and the
conversion of the existing data:

1.4.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times will vary for different
computers. The installation time specified was determined using a reference device with the following
characteristics:
   •   Processor:    Intel Pentium 4, 2.7 GHz, 1 GByte RAM
   •   Storage space:         Approx.10 MB of hard disk space is required
   •   Miscellaneous
For an initial or new installation, an installation time of 2 minutes must be anticipated for the reference
device. For higher or lower-power hardware, shorter or longer installation times must be anticipated.


2023-03-13                                     EN-INST-A+W SetupLauncher.docx                                  4
1.4.2 Conversion Time for Data Set
None.




2023-03-13                      EN-INST-A+W SetupLauncher.docx   5
1.5 Requirements
1.5.1 Hardware
None.

1.5.2 Dongle
No dongle required.

1.5.3 Network
When the A+W setup packages are available in the network, the directory must be released and the user
of the Setup Launcher must be able to access it.

1.5.4 Software
    •   .Net Framework 4.5 (will be downloaded and installed if it has not been installed already, and if
        there is a connection with the Internet or a Windows Update Server).
    •   The use of the automatic update via FTP requires Internet connection and access to the FTP
        Server.

1.5.5 Service user/Administrator rights
Use of the Setup Launcher require local administrator rights.




2023-03-13                                    EN-INST-A+W SetupLauncher.docx                                6
1.6 Procedure
        1. Installing the Setup Launcher:

             Execute „SetupStarter.exe“ in the CD's main directory. After installation, the Setup Launcher
             will start automatically. Press "Next" to proceed.




2023-03-13                                     EN-INST-A+W SetupLauncher.docx                                7
        2. Selecting a diskset:

             A diskset file is a control file which provides all information on the setup. Every disk set file
             must show at least the path where the setup packages can be found. Prefabricated disk set
             files can also include values which are necessary for installing the setup.




             Some predefined disksets are available at the start.
             The shown sequence of packages should match the installation sequence. This means, if
             several packages are necessary on one server, the individual packages should be installed in
             the sequence displayed in the A+W Setup Launcher.
             New disk sets can be created if required. Choose the entry „Create new diskset…“ from the list
             and press „Next“. Save the file in the following dialog. We recommend to use the preset path
             „%COMMONAPPDATA\SetupLauncher“.




2023-03-13                                       EN-INST-A+W SetupLauncher.docx                                  8
        3. Selecting the installation directory


             All software installed via Setup Launcher will be installed in a fixed directory tree. During
             installation you can choose the hard disk or partition.
             Source Directory shows the path in which the individual setup packages are found (disk sets).
             You can change this path in this dialog; this will not affect the other information in the disk set
             file.
             This dialog also shows information on the operating system.
             The button „Configure Auto Update…“ serves to make the settings for automatically updating
             the installation. Use "FTP Download" to execute the FTP Download manually. More information
             on the Feature are available in chapter 1.7.




2023-03-13                                        EN-INST-A+W SetupLauncher.docx                                   9
        4. Installed packages:

             The next page shows a short list of the packages already installed. The system will show all
             software systems either supplied by A+W or available in the selected disk set (or both). For
             every package installed, the system shows the version installed and the version existing in the
             disk set. In front of the installed package, there may be icons showing the state of the package:

             No icon: Software is not included in the present diskset.
             Yellow sign: A new version is available for software already installed on the system.

             Green sign: Installed software and software from the diskset have the same status.

             Red sign: Installed software newer than the diskset version.




        5. Selection of elements:

             Next, select the elements to be installed. Elements are grouped in different categories. The
             icon in front of the category defines whether no, all, or only some elements of this category
             shall be installed. On the right there is a window providing information on the selected element.

             Elements may include dependencies. These will be automatically selected together with the
             element. If these are not to be installed, they have to be deselected separately.



2023-03-13                                      EN-INST-A+W SetupLauncher.docx                              10
             The the end of the dialog, the system checks if all dependences are met. You can of course
             continue with the setup at your own risk; the correct functioning of the software cannot be
             guaranteed in this case however.




        6. A+W SOA Settings:

2023-03-13                                     EN-INST-A+W SetupLauncher.docx                              11
             If an A+W SOA component is installed, this dialog appears. Here it is defined where the A+W
             Service Locator is installed or shall be installed.
             It is important that only one instance of the A+W Service Locator is installed at customer and
             that all installations use the same Service Locator (Highlander principle).




             The port is correctly preset and should only be changed in agreement with the development.


        7. Settings for the selected elements:

             Next, collect the information you need to install the selected elements. Please refer to the
             installation instructions for the individual setups if required.


             Saving the information and starting the installation:

             When all the necessary information has been entered and the setups can be started, the
             collected information can be saved in a disk set file. You can choose from three options:

             Install the software: Start the installation without saving the information in a file.

             Save the diskset file and install it: Save information in a diskset file and start the installation.
             Installation: Installation means, to stop all relevant services, to start and run the installation
             packages, to run all ´Hotfixes of the the diskset (incl. Rollback, if necessary), to start the
             relevant Config Tools, and to start the services. While starting the services the system makes
             sure whether the service was started before the installation (only running services will be
2023-03-13                                        EN-INST-A+W SetupLauncher.docx                                    12
             restarted unless the installation itself starts the service!) and the former start type (manually,
             automatically, etc.) of the service will be restored.

             Save only diskset file: Save information in a diskset file and quit program.


             Manage Hotfixes: Enables the import of Hotfixes per product. The user has full control. But, he
             is also responsible for stopping all processes (user sessions of prgrams, services,
             Webservices, etc.). Thus, importing of hotfixes during operation is possible.




        8. Installing the software packages:

             The following image shows the current installation process. Every element has got its
             installation and configuration step. First, all elements are installed in the sequence described
             after which they are configured in the same sequence. The system will issue a message to
             show that installation and configuration has been completed.




2023-03-13                                       EN-INST-A+W SetupLauncher.docx                                   13
1.7 AutoUpdate
AutoUpdate is a way of updating all the A+W programs installed at a customer's. AutoUpdate proceeds in
two steps:
    1. Updating the setup packages: The versions in the installation directory can be updated by
       synchronising with the A+W FTP server. This process should be handled by an automatic
       Windows task which can be defined in the Setup Launcher. If necessary the synchronization with
       the A+W FTP Server can be started manually via the FTP download button. (see 1.6 point 3)
    2. Running the setups: The new versions will be installed on the computer.
For installations with several clients, only one computer (server or test system) has to be synchronised
with the FTP server. The client installations should only update the individual elements. No automatic task
has to be defined for the clients for this purpose.

1.7.1 General Information
To configure AutoUpdate on a computer, you have to create a diskset file first in which all installation tasks
have been entered. We recommend to use the diskset file for the AutoUpdate which has also been used
for the first complete installation, and save it at the end of the installation. AutoUpdate should be
configured during the initial installation if possible. If individual elements are installed later, you should
always use the diskset used for the AutoUpdate and add the new elements.




2023-03-13                                    EN-INST-A+W SetupLauncher.docx                                14
1.7.2 Set-up
AutoUpdates can be installed via SetupLauncher. From the dialog for selecting the installation directory,
you can open a dialog for setting up the AutoUpdate. This dialog offers three tabs:
    1. Setting up the FTP connection




This tab is used to configure the access to the A+W FTP server. The data in this dialog are saved on the
local computer, in the registry. Access to the FTP server requires the following entries:
        •    Customer: Customer number from the main database/AWDesk
        •    Server: A+W FTP server address
        •    Directory: Basic directory on the FTP server which also holds the current installation. This can
             be checked via the Explorer. The directory on the FTP server has to be entered in this field:

             For version 2009: upload/2009
             For version 2011: upload/2011
             For version 2012: upload/2012
             For version v6: upload/v6

        •    User: User for registering with the A+W FTP server
        •    Password: Password for registering with the A+W FTP server
        •    Use Proxy: Enable this option if the FTP server is accessed via Proxy server
        •    User: User name for authentication at the Proxy server
        •    Password: Password for authentication with the Proxy server
2023-03-13                                      EN-INST-A+W SetupLauncher.docx                              15
Only if the option „Configure FTP access for automatic Update“ is active, the option for synchronising with
the FTP server will be enabled when the links are set up in tab 3!


    2. Setting up the email notification




By enabling the email notification, one or more persons will be informed of the software update. Email
notification is enabled by the following entries:
        •    Server: Name of the email server which shall send out the emails
        •    Sending address: Name to be listed as the email sender's. This name must include at least one
             „@“. Our recommendation: AutoUpdate@Firma.Land, the company being replaced by the
             company name (without symbols or blanks) and the country, by the country code)
        •    Receiving address: Email address(es) of the recipient(s) (separated by „;“ if there is more than
             one)
        •    Port: Mail server port (usually 25)
        •    Authentication: Tick this option if the mail server requires special authentication. Please ask the
             mail server administrator for the necessary settings.




2023-03-13                                         EN-INST-A+W SetupLauncher.docx                             16
    3. Defining the links




This tab is used for defining the links for the automatic update. The options for this are:
    •    Create Icon on Desktop: Creates a link on the user's desktop which can be used to start an
         automatic update.
    •    Create Icon in start menu: Creates a link in the user's start menu which can be used to start an
         automatic update.
    •    Create scheduled task: This option defines a Windows task which runs the automatic update
         every date at a given time. Once created, this task can be amended in Windows task planning. If
         the version shall be tested on a server or a test system before being passed on to all clients, this
         option should be enabled only on this system, not on the clients. The FTP server control the
         availability of updates. With the August 2011 patch, an automatic task can also be defined for the
         client if the diskset includes a file of this version. For details please see chapter 1.7.3.
    •    Create Release Version Icon: This option serves to create an icon on the desktop which can be
         used to raise the diskset version by 1 (see 1.7.3). This should be created only on the system on
         which the FTP download is made.
    •    Update only if version is proved by User: If you choose this option, the automatic task and the
         links will be defined so that before the update is run, the version on the server will be compared to
         the client version. The update will be made only if the server version is higher than the client
         version (see 1.7.3). If links and tasks have already been defined, the argument –client will appear
         in the call.
When you confirm your entries by OK, the entries will be saved and the selected links will be created.



2023-03-13                                     EN-INST-A+W SetupLauncher.docx                               17
1.7.3 ReleaseRelease
The automatic Windows task updates the installation on the server. After the installation has been
checked, it can be made available to all clients. This is done by executing the Release Version link. When
this has been executed, the version of the file Version.txt in the diskset directory will have been raised by
1. With every installation from this directory, this number will be updated on the local computer.
At present, only the ALFAK start program uses this information. If the version in the diskset does not
match the version installed on the client, the start program cannot be run.
Amendments in August 2011:
The file Version.txt can be used only to control the updating of clients:
    •   If the automatic update is started on a client with the option –client (option „Update only if version
        is proved by User“ created) and if the file Version.txt exists in the diskset directory (e.g.
        \\jupiter\SW_INSTALL\v6\Diskset\Version.txt), the program checks prior to dhe update whether the
        version number of the file is higher than during the last update (in the client registration
        HKEY_LOCAL_MACHINE\Software\Albat+Wirsam\SetupLauncher\AutoUpdate\ClientVersion). If
        this number is higher, the update will be run. If the number is equal or lower, no update will be
        made.
    •   After the update, the file number is saved in the client's registry. This means that no update can be
        run for the client until the number on the server is raised.
    •   If the file does not exist or if the update is loaded without the option –client, the update will be run
        without a release check.
    •   The number in the file can be raised by one by means of the link ReleaseVersion (can be created
        via SetupLauncher). This should be done only on the server.

1.8 IncompatibilitiesIncompatibilities
Correct operation of the Setup Launcher can be impeded by missing version information in the Windows
software control because the Setup Launcher will be assumed to try and install a – seemingly – new
version. This can be prevented by deselecting this element in the element dialogue.
At present there is a problem with element selection, i.e. elements cannot be deselected if a category is
completely disabled.

1.9 Diskset Directory Structure
The directory which contains the installation packages must also contain the elements in sub-directories.
For every element there has to be at least one file called „package.xml“. This file describes the setup.

1.10Manual settings
You can also define special installation packages. In this case you have to make sure that the Xml files
are correct. Existing packages can be used as examples.
The diskset file can also be created by hand.




2023-03-13                                      EN-INST-A+W SetupLauncher.docx                                     18
1.11Command line option and automatic mode
SetupLauncher can also be operated in automatic mode so that no action on the user’s part is necessary.
First, create a diskset file from which the settings for the setup can be loaded. Now start automatic
installation with the help of the command line.
The following command line parameters are available:

 -automode                                             Transfers the SetupLauncher to automatic mode
                                                       in which no parameters will be checked. Must be
                                                       entered together wit the option –xml

 -xml:<filename>                                       Transfer of a diskset file to the SetupLauncher for
                                                       automatic mode

 -log:<filename>                                       Recording in this file

 -result:<filename>                                    Save installation result in the defined file

 -skipconfig                                           Skips the configuration of the installation
                                                       packages. Is mainly required for installing updates,
                                                       especially if these are implemented as scheduled
                                                       tasks.

 -ftpsync                                              Synchronises the setup packages from the FTP
                                                       server. FTP access must be configured
                                                       beforehand.

 -autoupdate                                           Automatic mode for updating all elements
                                                       installed. Must be entered together wit the option –
                                                       xml Must be entered together wit the option –xml

 -versionupdate                                        Raises the version number in file Version.txt. If the
                                                       file does not exist yet, it will be created, showing
                                                       the number 1. Must be entered together with
                                                       option –xml. Must be entered together wit the
                                                       option –xml Must be entered together wit the
                                                       option –xml

 -client                                               Check the file Version.txt by means of local
                                                       registration to see whether the version has been
                                                       released



1.11.1         Unsupervised initial installation
A+W SetupLauncher will start right after it has been installed. To run unsupervised installations, the
Setuplauncher can be given the start parameters by means of a registry key. The required parameters are
written in the key.
[HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432NODE\Albat+Wirsam\Setuplauncher]
RestartCmdLine=-autoupdate -skipconfig "-xml:<DisksetPfad>\<DisketName> " (REG_SZ)


2023-03-13                                  EN-INST-A+W SetupLauncher.docx                                   19
An example CMD command is (please start a 32 Bit input command!):
reg add HKLM\Software\Albat+Wirsam\SetupLauncher /v RestartCmdLine /t REG_SZ /d "-autoupdate -
skipconfig \"-xml:c:\programdata\setuplauncher\autoupdate.diskset\" "




1.12Result of the installationResult of the installation


1.13 Installation alternatives
None known.

1.14Patches
Designation             BESCHREIBUNG                         Prerequisite




2023-03-13                               EN-INST-A+W SetupLauncher.docx                          20
1.15 Uninstalling
To uninstall the software, select menu „Software“ in system management. Now uninstall the Setup
Launcher.




2023-03-13                                 EN-INST-A+W SetupLauncher.docx                         21
2 Update
2.1 Procedure
To update the Setup Launcher, execute „setup.exe“ again. Setup Launcher will automatically start after
the update.




2023-03-13                                  EN-INST-A+W SetupLauncher.docx                               22
3 Preparing a Windows Server 2012 for A+W Software
        This document shall provide assistance as to which roles, role services, and features have to be
        selected to make sure that the A+W software can be installed and operated.
        This document assumes that the installation of the Windows server has been completed and that
        a user from the local groups of administrators (here: the "Administrator“) has logged in. After the
        login, the "Server Manager“ should have started automatically; otherwise, this has to be done by
        hand (pressing the Windows key will open the new "App menu“ where you can just enter: "Server
        Manager“ then select the icon "Server Manager“ by a left mouse click.

3.1 ATTENTION!!!
        This chapter describes the typical problems which will be encountered at the initial installation
        should you have ignored this document!

        •    Terminal server = Remote Desktop Session Host

        •    ASP.NET is now called ASP.NET3.5! As from Server 2012, ASP.NET is the name for the
             ASP.NET of .NET Framework 4.5. The tool needs .NET-Framework 3.5.

        •    If the file server role is missing (Storage Services), no shares can be defined. The dialogues
             in Windows exist however and will return no error report. Still, no share has been created!

3.2 The Server Manager
        Logical software packages can be selected from the server manager. These logical software
        packages are called roles, role services, and features.
3.2.1 Roles
        A role describes the server's main function (e.g. Web server, file server or application server). A
        server can have several roles.
3.2.2 Role services
        Some roles have just one single function (e.g. DNS server). This is why no role services are
        available for those. Other roles (e.g. remote desktop services) have several role services which
        can be installed depending on the requirements. A role can be understood as a group of
        connected role services.
3.2.3 Features
        Features are software programs which are not directly part of roles but which support or improve
        the functionality of the server in general, or the functionality of roles. Examples for this are e.g.:
        Telnet (improves the server's communication options) or the fail-over cluster support (improves
        all roles which provide a service capable of handling clusters).
3.2.4 Server manager operationServer manager operation
        The server manager as compared with Windows Server 2008 (R2) has been revised. Remote
        administration of other servers is possible now. This also means that the server to be administered
        has to be defined first. In most of the cases, this will be the computer on which one is registered
        anyway, i.e. the "localhost“.
2023-03-13                                      EN-INST-A+W SetupLauncher.docx                                   23
3.3 Adding Roles and Features
        In the server manager, select item "2 Add roles and features“:




2023-03-13                                    EN-INST-A+W SetupLauncher.docx   24
        The "Before you begin“ dialogue is optional; it requires no actions and can be skipped by pressing
        "Next >“.




        In dialogue "Server Selection“ you can choose the computer to be administered. The local server
        is pre-selected.




2023-03-13                                    EN-INST-A+W SetupLauncher.docx                                 25
3.3.1 Server roles
        Now select the server roles. Important ones are:

        •    Application
             Server

        •    Storage services (in file and storage services)

        •    Web server (IIS)
        To install a Terminal Server, please install the remote desktop services. Usually, this is not
        necessary for the process server. Further licenses of Microsoft are necessary for the remote
        desktop services
        Depending on whether you want to install a terminal server or a process server you also have to
        select the Remote Desktop Services.




2023-03-13                                      EN-INST-A+W SetupLauncher.docx                            26
        When you select, "Web Server (IIS)“, a dialogue appears:




        The displayed settings are correct and will be suggested by default.




2023-03-13                                    EN-INST-A+W SetupLauncher.docx   27
3.3.2 Features
        The next dialogue serves for selecting the features. It is essential to select the following here:

        •    .NET Framework 3.5 Features

                o   .NET Framework 3.5 (includes .NET 2.0 and 3.0)

                o   HTTP Activation (confirm the dialogue)




2023-03-13                                     EN-INST-A+W SetupLauncher.docx                                28
3.3.3 Role services of the application server (Application Server)
        •    .NET                                          Framework                4.5


        •    Web Server (IIS) support
             This also opens a dialogue which just needs to be confirmed




3.3.4 Web server role services
        Please check the screenshot. And especially make sure that

        •    Web
             Server

                o     Application Development

                            ASP.NET 3.5
        are ticked! Other items that have to be ticked are:

        •    Management Tools

                o     IIS Management Console

                o     IIS 6 Management Compatibility

                            Tick all sub-items!

                o     IIS Management Script and Tools

2023-03-13                                         EN-INST-A+W SetupLauncher.docx         29
2023-03-13   EN-INST-A+W SetupLauncher.docx   30
3.3.5 Role services for the remote desktop services
        If the server is to be set up as a terminal server, please select the item Remote Desktop Session
        Host and confirm the settings in the following dialogue.
        Windows has renamed the terminal server services!
        Terminal server = Remote Desktop Session HostTerminal server = Remote Desktop
        Session Host


3.3.6 Completing the configuration
        In the "Confirmation“ window you can see the settings made and can also start the configuration
        by pressing "Install“.
        The "Result“ window shows the progress of the installation. The window can be closed; the
        installation keeps running.
        Alternatively, you can use "Export configuration settings“ to save the settings that have been
        made; these settings can be easily loaded for a follow-up installation.




3.4 Script based installation of necessary Windows features
The necessary scripts to install the Windows features can be found in
\\jupiter\sw_install\Tools\InstallationsSkripts.


        •    For desktop operation systems please start the file „Install_WindowsClient.cmd“ with admin
             rights.
        •    For server operation systems please start the file „Install_WindowsServer.cmd“ with admin
             rights.


To run the scripts, the Powershell console must allow running of Powershell scripts. Therefore, execute in
an administrative Powershell console the command
Set-ExecutionPolicy Unrestricted

But, the scripts refer to this if the permission was not granted yet.




2023-03-13                                     EN-INST-A+W SetupLauncher.docx                               31

