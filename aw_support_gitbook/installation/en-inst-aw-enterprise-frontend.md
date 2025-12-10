---
title: "EN INST A+W Enterprise Frontend"
category: "installation"
product: "A+W Enterprise Frontend"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Enterprise Frontend"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions            A+W Enterprise 6 Frontend    Change history:      Date           Edited by                Remarks                                    Version     16.04.18       MP                       Creation                                   1.0     16.05.31       MP                       SSH proxy                                  1.1     16.12.13       MP                       AutoUpdate                                 1.2     21.02.20       TSC"
source_file: "EN-INST-A+W Enterprise Frontend.pdf"
---


# EN INST A+W Enterprise Frontend

          Installation Instructions

          A+W Enterprise 6 Frontend
   Change history:

    Date           Edited by                Remarks                                    Version
    16.04.18       MP                       Creation                                   1.0
    16.05.31       MP                       SSH proxy                                  1.1
    16.12.13       MP                       AutoUpdate                                 1.2
    21.02.20       TSC                      Adjustments to WiX setup                   1.3




     The installation instructions will assist the planner with the installation and
     configuration of the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




17.12.2024                          EN-INST-A+W Enterprise Frontend.docx                 1
Content

   1         Installation of the A+W Enterprise 6 Frontend ..................... 3
   1.1       Overview and the basics ............................................................................ 3
   1.2       Time requirement ....................................................................................... 3
   1.2.1     Installation time for the software ................................................................. 3
   1.2.2     Conversion Time for Data Set .................................................................... 3
   1.3       Requirements ............................................................................................. 3
   1.3.1     Hardware .................................................................................................... 3
   1.3.2     Network ...................................................................................................... 4
   1.3.3     Software ..................................................................................................... 4
   1.4       Procedure ................................................................................................... 4
   1.4.1     Config Tools ............................................................................................. 10
   1.5       Incompatibilities ........................................................................................ 10
   1.6       Directory structure .................................................................................... 10
   1.7       Result of the installation ........................................................................... 10
   1.8       Configuration ............................................................................................ 10
   1.9       Use of the TOE – Installation of the license client .................................... 10
   1.10      Installation alternatives ............................................................................. 10
   1.10.1    "Silent Setup" or "Unattended Installation" (#322660) .............................. 10
   1.11      SSH proxy service .................................................................................... 12
   1.12      Documentation ......................................................................................... 13
   1.12.1    Manuals .................................................................................................... 13
   1.12.2    SSH proxy documentation ........................................................................ 13
   1.13      Tips and tricks .......................................................................................... 13
   1.13.1    Adding sites after the fact ......................................................................... 13
   1.13.2    Known errors and workarounds ................................................................ 13
   1.13.1    AutoUpdate .............................................................................................. 14
   1.14      Uninstalling ............................................................................................... 14




17.12.2024                              EN-INST-A+W Enterprise Frontend.docx                                               2
1 Installation of the A+W Enterprise 6 Frontend
The following installation instructions assume that there is no previous version installed.

An update of an earlier release version of the A+W Enterprise 6 Frontend is executed
precisely like a new installation.

An update of an earlier version of the Frontend, e.g. from ALCIB 2011 Frontend to A+W
Enterprise 6 Frontend is not possible. These versions can be operated in parallel on a
computer.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during installation:
    -   Creation of the necessary set-ups
           o A+W CAD Designer (Bars)
           o A+W CAD Designer (Shapes)
           o A+W Infrastructure 6 Collector Services
           o A+W Infrastructure 6 Middleware
           o A+W Enterprise 6 Frontend
           o A+W Setup Launcher
    -   Execute Setup Launcher and thus install the Frontend disk set.

1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data:

1.2.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times will
vary for different computers. The installation time specified was determined using a
reference device with the following characteristics:
    -   Processor: 3000 Mhz
    -   RAM: 4 GB
    -   Other: /
For an initial or new installation, an installation time of 15 minutes must be anticipated for
the reference device. For higher or lower-power hardware, shorter or longer installation
times must be anticipated.

1.2.2 Conversion Time for Data Set
No data is converted.

1.3 Requirements
1.3.1 Hardware
1200 MHz or higher processor.
512 MB or more main RAM.
250 MB or more hard disk.



17.12.2024                        EN-INST-A+W Enterprise Frontend.docx                           3
Network card.

1.3.2 Network
For installation itself, no connection to a network is required. For the operation of A+W
Enterprise 6 Frontend, however, a network connection to the A+W Enterprise Application
Server must be established.

If a firewall is installed, then the ports 5000 to 5050 and 512 must be opened.
It is recommended that you deactivate the Windows firewall. The Windows firewall can
cause problems with some server operating systems. If the server operating system is
LINUX, the firewall must be deactivated on the client PCs.

1.3.3 Software
Supported operating systems:

    •   Windows 7, 8, 8.1 32/64-bit
    •   Windows 2008 Server R2 32/64-bit
    •   Windows 2012 Server R2 32/64-bit

The desktop must be set to at least 16-bit color depth.

1.4 Procedure
For the installation, please proceed in the following sequence:

1. The user who would like to install the A+W Enterprise 6 Frontend must have
   administrator rights.

2. Installation of the A+W Enterprise 6 Frontend with the Setup Launcher
   On the Component Selection dialog on the A+W Enterprise node, select the "A+W
   Enterprise 6 Frontend" module. This automatically selects all dependent set-ups.

3. All running sessions of the A+W Enterprise 6 front end must be closed so that an
   installation or update is possible. If this is not the case, the error 1224 will occur during
   installation.




17.12.2024                       EN-INST-A+W Enterprise Frontend.docx                              4
4. After the successful installation of the programs, the A+W Enterprise 6 Frontend is
   configured with the Config Tool.




17.12.2024                     EN-INST-A+W Enterprise Frontend.docx                      5
        3.1 Common Settings




        3.1.1   Frontend Language
                The language of the Windows frontend is set here. This does not define the
                A+W Enterprise language, but only the labels on the login dialog and the
                menu titles of the frontend. Default: English.
        3.1.2   Font Weight
                With this switch, you can set whether the display of the letters in A+W
                Enterprise should be normal or boldface. Default: Normal.
        3.1.3   Currency Symbol
                Here the currency symbol can be set, which is used on some dialogs in A+W
                Enterprise. Default: EUR.
        3.1.4   Use SSH Connect
                If the access to the backend should be via a SSH connection, this switch
                must be activated. Default: No.




17.12.2024                      EN-INST-A+W Enterprise Frontend.docx                         6
                If the setting is on Yes, the SSH proxy service is installed and started
                automatically with default values. (see chapter 1.11)
        3.1.5   Save Password
                If the option is set to "Yes," a selection possibility appears on the login screen
                to save the password for this connection. If the password is saved, it will be
                shown again on the next start of the frontend and the login screen will not
                appear and the user will be logged directly into the "Main menu".
        3.1.6   Show Startup Menu
                Only active if "Save password" was set to "Yes". Setting this value to "Yes"
                means that the login screen is displayed even if the password was saved. If
                the option is not active, the user is logged directly into the frontend and the
                start screen will no longer appear.
        3.1.7   Protocol-Button
                The internal logic completes under the path specified here the directory
                <Hausnummer> and <Kundennummer>. This automatically selects all
                dependent set-ups. On the first tab, the trace categories for the frontend are
                configured; on the following tabs, the tracing of dependent modules and
                programs can be activated if necessary.
        3.2     Server and Site Settings




17.12.2024                        EN-INST-A+W Enterprise Frontend.docx                           7
              On the second dialog of the Config Tools, you enter the A+W Enterprise
              Backend server name and the associated sites for which the Frontend will be
              set up.
              If you do not have this data to hand, please consult your system department
              or A+W Service. An example for the A+W Enterprise Backend server name is
              "romulus"' (input without quotation marks). One example for the client
              number is "57" (enter without quotation marks). You can only click "Next" if
              you have stored at least one server/site combination.
              Generally, you can create and then change as many server/site combinations
              as you wish.
              If you want to configure a foreign-language frontend for a client, enter the
              corresponding language abbreviation before the client number. As example
              for an English frontend „GB57“ (enter without quotation marks). The backend
              must be prepared accordingly for this configuration variant. Please contact
              your system department or the A+W Service
        3.3   Configuration finished
              Only if you see this dialog is the configuration finished. You can now finish
              the configuration with the Finish button. If you exit the Config Tool earlier than
              this, the settings selected have no effect on the program!


17.12.2024                      EN-INST-A+W Enterprise Frontend.docx                           8
             Only at this time were all configuration settings taken over, the links created,
             and the SSH service installed.




17.12.2024                    EN-INST-A+W Enterprise Frontend.docx                              9
1.4.1 Config Tools
The following programs have their own Config Tools. Please see their installation
instructions for information about the correct configuration of these programs.

    •   A+W CAD Designer (Bars)

    •   A+W CAD Designer (Shapes)



1.5 Incompatibilities
Currently, no incompatibilities are known.

1.6 Directory structure
The default installation directory is <Programs>\A+W\A+W Enterprise 6.

1.7 Result of the installation
After successful installation, the application has been installed in the directory
<Programs>\A+W\A+W Enterprise 6.

<Programs> is a placeholder for the "Programs" directory on the PC. With an English
operating system, this is called "program files".

You can now start the application via Start  Programs  A+W  A+W Enterprise 6
Frontend.

1.8 Configuration
Configuration is done during set-up.

1.9 Use of the TOE – Installation of the license client
When calling the TOE, a SN license is required.
This license can be made available by the A+W License Server. The license is requested
when starting the TOE.
Therefore, the A+W License Client must be installed on the same machine as the front
end. For additional information about the License Client installation, see the installation
instructions for the License Client.

1.10 Installation alternatives
1.10.1 "Silent Setup" or "Unattended Installation" (#322660)
The A+W Enterprise Frontend set-up supports the possibilities of the SetupLauncher to
execute a so-called "silent installation." Here, only the part is described that is necessary in
order to install the frontend "silently," that is, without user input.




17.12.2024                       EN-INST-A+W Enterprise Frontend.docx                              10
For this purpose, a file named awefrontend.config must be created in the diskset directory
of the A+W Enterprise 6 Setup. It must have a particular, defined structure. For this purpose,
there are two template files in the disk set directory, which can serve as template for this file.
In these files, the content of the awefrontend.config file is also explained.

The file awefrontend.config.single.template contains the structure if precisely one server-
site configuration should be installed.

The file awefrontend.config.multi.template contains the structure if precisely several
server-site configurations should be installed. An example of 2 such configurations is stored
in the template. Using the example, more than 2 configurations can also be set.
Important is that in the ServerCount field, you enter the total number!

In order to use these files as configuration, they must be changed to the name
awefrontend.config.

In the area of the A+W Enterprise 6 Frontend, otherwise there is nothing else to do in order
to execute a silent installation.

This function can also be used for an update within Version 6. Here it must be heeded that
the file specified by the planner wins and that any deviating configurations are lost.
1.10.1.1       Example: one server-site assignment
<?xml version="1.0"?>
<configuration>
  <appSettings>
  <add key="FrontendLanguage" value="0"/>
  <add key="FontWeight" value="0"/>
  <add key="CurrencySymbol" value="1"/>
  <add key="UseSshConnect" value="0"/>
  <add key="ServerCount" value="1"/>
  <add key="ProgType" value="default"/>
  <add key="Server" value="asteraix"/>
  <add key="Site" value="121"/>
  </appSettings>
</configuration>




17.12.2024                       EN-INST-A+W Enterprise Frontend.docx                           11
1.10.1.2     Example: two server-site assignments
<?xml version="1.0"?>
<configuration>
  <appSettings>
  <add key="FrontendLanguage" value="0"/>
  <add key="FontWeight" value="0"/>
  <add key="CurrencySymbol" value="1"/>
  <add key="UseSshConnect" value="0"/>
  <add key="ServerCount" value="2"/>
  <add key="ProgType1" value="default"/>
  <add key="Server1" value="asteraix"/>
  <add key="Site1" value="121"/>
  <add key="ProgType2" value="default"/>
  <add key="Server2" value="asteraix"/>
  <add key="Site2" value="1121"/>
  </appSettings>
</configuration>



1.11 SSH proxy service
If the setting Use SSH Connect has the value Yes, the ConfigTool automatically
configures the SSH proxy service with the following default values.




If the SSH proxy service should be deleted and uninstalled, you must set the
setting Use SSH Connect to No in the ConfigTool and run through the Config
Tool to the end.




17.12.2024                  EN-INST-A+W Enterprise Frontend.docx                 12
The log file of the SSH proxy service is written to %ProgramData%\A+W\A+W
Enterprise 6 Frontend\FXSSHPROXY_AWE.log.

For additional information about the SSH proxy service, see the associated
documentation.

1.12 Documentation
1.12.1 Manuals
With the set-up, the existing manuals are provided in German and English. These
are in the directory <Programs>\A+W\A+W Enterprise 6 Frontend\Doc\Manuals.


1.12.2 SSH proxy documentation
This is under <Programs>\A+W\A+W Enterprise 6 Frontend\fxsshproxy\doc

1.13 Tips and tricks
1.13.1 Adding sites after the fact
A new site can also be added manually without new installation.
Use the Config Tool for this. In the 2nd dialog, you can enter as many
server/client combinations as you like. For this, after completion of the
configuration, the appropriate links are created on the Start menu in the A+W
folder.
1.13.2 Known errors and workarounds
Error message such as "rexec protokollfehler: timeout?" (precise formulation
depends on the operating system)
This message can appear if you try to connect over a firewall. For communication
with A+W Enterprise, some ports must be enabled in the firewall. These ports are
entered in the installation directory in the file alcib.ini. The ports in the span
between the entries "Firstport" and "Lastport" must be enabled. By default, these
are the ports 5000 - 5050.
In case of a network with IP masquerading, a log in on the server with the A+W
Enterprise Frontend is not possible. Should you have problems due to IP
masquerading, please contact your network administrator.




17.12.2024                   EN-INST-A+W Enterprise Frontend.docx                    13
1.13.1 AutoUpdate
In order to be able to install the program via AutoUpdate, the setup must have
been installed successfully at least once with the Setup Launcher and configured
with the ConfigTool.

1.14 Uninstalling
You can uninstall the program as usual via Control Panel  Programs and Functions.
    1. Select the entry A+W Enterprise 6 Frontend and click Uninstall.
    2. Confirm this dialog with "Yes".




    3. A+W Enterprise 6 Frontend was successfully removed from your PC.




17.12.2024                      EN-INST-A+W Enterprise Frontend.docx                 14

