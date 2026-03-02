---
description: "EN INST A+W Enterprise Web"
---



# EN INST A+W Enterprise Web

          Installation Instructions

          A+W Enterprise 6 Web
   Change history:
    Date           Edited by                Remarks                                    Version
    16.04.22       MP                       Creation                                   1.0
    16.05.31       MP                       SSH proxy                                  1.1
    16.12.15       MP                       AutoUpdate                                 1.2




     The installation instructions will assist the planner with the installation and
     configuration of the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




19.04.2018                            EN-INST-A+W Enterprise Web.docx                    1
Content

   1         Installation of the A+W Enterprise 6 Web ............................. 3
   1.1       Overview and the basics ............................................................................ 3
   1.2       Time requirement ....................................................................................... 3
   1.2.1     Installation time for the software ................................................................. 3
   1.2.2     Conversion Time for Data Set .................................................................... 3
   1.3       Requirements ............................................................................................. 3
   1.3.1     Hardware .................................................................................................... 3
   1.3.2     Network ...................................................................................................... 4
   1.3.3     Software ..................................................................................................... 4
   1.4       Procedure ................................................................................................... 4
   1.4.1     Config Tools ............................................................................................. 11
   1.5       IncompatibilitiesIncompatibilities .............................................................. 11
   1.6       Directory structure .................................................................................... 11
   1.7       Settings .................................................................................................... 11
   1.7.1     Firewall ..................................................................................................... 11
   1.7.2     IIS ............................................................................................................. 11
   1.8       Result of the installationResult of the installation ..................................... 13
   1.9       Configuration ............................................................................................ 13
   1.10      SSH proxy service .................................................................................... 13
   1.11      Documentation ......................................................................................... 14
   1.11.1    Manuals .................................................................................................... 14
   1.11.2    SSH proxy documentation ........................................................................ 14
   1.12      Tips and tricks .......................................................................................... 14
   1.12.1    Adding sites after the fact ......................................................................... 14
   1.12.1    AutoUpdate .............................................................................................. 14
   1.13      Uninstalling ............................................................................................... 14




19.04.2018                                 EN-INST-A+W Enterprise Web.docx                                                     2
1 Installation of the A+W Enterprise 6 Web
The following installation instructions assume that there is no previous version installed.

An update of an earlier release version of the A+W Enterprise 6 Web is executed precisely
like a new installation.

An update of an earlier version of the Frontend, e.g. A+W Enterprise 5 Web to A+W
Enterprise 6 Web is not possible. These versions can be operated in parallel on a computer.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during installation:
    -   Creation of the necessary set-ups
           o A+W CAD Designer (Bars)
           o A+W CAD Designer (Shapes)
           o A+W Infrastructure 6 Collector Services
           o A+W Infrastructure 6 Middleware
           o A+W Enterprise 6 Web
           o A+W Setup Launcher
    -   Execute Setup Launcher and thus install the Web disk set.

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
For an initial or new installation, an installation time of 10 minutes must be anticipated for
the reference device. For higher or lower-power hardware, shorter or longer installation
times must be anticipated.

1.2.2 Conversion Time for Data Set
No data is converted.

1.3 Requirements
1.3.1 Hardware
1200 MHz or higher processor.
512 MB or more main RAM.
250 MB or more hard disk.
Network card.



19.04.2018                          EN-INST-A+W Enterprise Web.docx                              3
1.3.2 Network
For installation itself, no connection to a network is required. For the operation of A+W
Enterprise 6 Web, however, a network connection to the A+W Enterprise Application Server
must be established.

If a firewall is installed, then the ports 5000 to 5050 and 512 must be opened.
It is recommended that you deactivate the Windows firewall. The Windows firewall can
cause problems with some server operating systems. If the server operating system is
LINUX, the firewall must be deactivated on the client PCs.

1.3.3 Software
Supported operating systems:

    •   Windows 2008 Server R2 32/64-bit
    •   Windows 2012 Server R2 32/64-bit

1.4 Procedure
For the installation, please proceed in the following sequence:

1. The user who would like to install the A+W Enterprise 6 Web must have administrator
   rights.

2. Installation of the A+W Enterprise 6 Web with the Setup Launcher
   On the Component Selection dialog on the A+W Enterprise node, select the "A+W
   Enterprise 6 Web" module. This automatically selects all dependent set-ups.




19.04.2018                        EN-INST-A+W Enterprise Web.docx                           4
3. After the successful installation of the programs, the A+W Enterprise 6 Web is
   configured with the Config Tool.




19.04.2018                      EN-INST-A+W Enterprise Web.docx                     5
        3.1 Common Settings
        3.1.1.   Font Weight

                 With this switch, you can set whether the display of the letters in A+W Enterprise
                 should be normal or boldface. Default: Normal.

                 Info: This setting is currently not available.

        3.1.2.   Currency Symbol

                 Here the currency symbol can be set, which is used on some dialogs in A+W
                 Enterprise. Default: EUR.

        3.1.3.   Use SSH Connect

                 If the access to the backend should be via a SSH connection, this switch must be
                 activated. Default: No.

                 If the setting is on Yes, the SSH proxy service is installed and started automatically
                 with default values. (see Chapter 1.10)

        3.1.4.   SSH Configuration

                 If the option Use SSH Connect has the value Yes, this button becomes active
                 and you can use it to start the program fxsshproxyss.exe. (see Chapter 1.10)


19.04.2018                             EN-INST-A+W Enterprise Web.docx                                6
        3.1.5.   Protocol-Button

                 The internal logic completes under the path specified here the directory
                 <Hausnummer> and <Kundennummer>. This automatically selects all dependent
                 set-ups. On the first tab, the trace categories for the frontend are configured; on the
                 following tabs, the tracing of dependent modules and programs can be activated if
                 necessary.




             The following trace levels are distinguished:
             o Fatal
             o Error".
             o Warning
             o Info
             o Debug

             With the Protocol button, you can reach the Protocol Configuration dialog. If, for example,
             the Info level is active, trace messages of the type Error and Warning will also be written
             into the tracing file.




19.04.2018                            EN-INST-A+W Enterprise Web.docx                                      7
              The tracing file is always in the directory %ProgramData%\A+W\Log. The file name
              consits of the service name, the current date and the process number and ends with
              .awtrc.

              The A+W Enterprise Print Service currently uses no log protocol.



        3.2       Server and Language Settings




              3.2.1.   The server connections are stored on this dialog.

              At least one server connection must be specified; otherwise you cannot leave this page
              in the Config Tool. Without this information, you cannot establish a connection to the
              A+W Enterprise Backend.

                  o    With the "New" button, a new connection can be created.

                  o    With the "Delete" button, a new connection can be deleted.

                  o    With "Edit," an existing connection can be edited.

              Generally, you can create and then change as many server/site combinations as you
              wish.

        3.4. Application Pool Identity Configuration



19.04.2018                             EN-INST-A+W Enterprise Web.docx                                 8
        3.3. Configuration finished

             Only if you see this dialog is the configuration finished. You can now finish the
             configuration with the Finish button. If you exit the Config Tool earlier than this, the
             settings selected have no effect on the program!




19.04.2018                            EN-INST-A+W Enterprise Web.docx                                   9
19.04.2018   EN-INST-A+W Enterprise Web.docx   10
1.4.1 Config Tools
        The following programs have their own Config Tools. Please see their installation
        instructions for information about the correct configuration of these programs.

             •   A+W CAD Designer (Bars)

             •   A+W CAD Designer (Shapes)



1.5 Incompatibilities
Currently, no incompatibilities are known.

1.6 Directory structure
The default installation directory is <Programs>\A+W\A+W Enterprise 6 Web.

1.7 Settings
1.7.1 Firewall
Through the set-up, an entry is configured for the Windows firewall in order to
enable the IIS Worker Process (w3wp.exe). Among other things, this is
responsible for the communication between Windows Server and A+W Enterprise
Backend.
However, with the set-up, all ports are opened for this process, although only the
ports 5000-6000 are required. This can be limited manually if necessary.
If another firewall than the Windows firewall is used, the w3wp.exe process must
be enabled manually in the port area named.
1.7.2 IIS
The set-up creates a so-called CGI/ISAPI limitation for the FixWtIIS.dll.
Under Windows Server 2008 R2 this currently does not work correctly. In the
path specification, the "+" sign is replaced with empty spaces. So that the
installation can be executed successfully and you can test the result, the option
"Do not allow specified ISAPI module" is also enabled.
WARNING! You should manually create a new CGI/ISAPI limitation and
deactivate the "Do not allow specified ISAPI module" option again.
!! The CGI/ISAPI limitation installed by the set-up may not be changed since
otherwise there can be problems during updating. !!
    1. Deactivating CGI and ISAPI




19.04.2018                        EN-INST-A+W Enterprise Web.docx                       11
        -    In the IIS Manager, search for and select the Server node on the left
             panel
        -    Double-click the "ISAPI and CGI restrictions" icon
        -    On the right panel, select "Edit Feature Settings"
        -    Deactivate checkboxes for CGI and ISAPI and exit the dialog.




    2. Add a CGI/ISAPI restriction
        -    Click "Add..."
        -    Select the path FixWtIIS.dll file in the "ISAPI or CGI path" field.
        -    Store a description.
        -    Place the check mark next to "Allow execution of the extension path".
        -    Confirm the dialog with OK.




19.04.2018                          EN-INST-A+W Enterprise Web.docx                  12
1.8 Result of the installation
After successful installation, the application has been installed in the directory
<Programs>\A+W\A+W Enterprise 6 Web.

<Programs> is a placeholder for the "Programs" directory on the PC. With an English
operating system, this is called "program files".

You can now start the application via Start  Programs  A+W.

1.9 Configuration
Configuration is done during set-up.

1.10 SSH proxy service
        If the setting Use SSH Connect has the value Yes, the ConfigTool
        automatically configures the SSH proxy service with default values.
        With the SSH Configuration button, you can change this configuration after
        the fact.




        If the SSH proxy service should be deleted and uninstalled, you must set
        the setting Use SSH Connect to No in the ConfigTool and run through the
        Config Tool to the end.
        The log file of the SSH proxy service is written to %ProgramData%\A+W\A+W
        Enterprise 6 Web\FXSSHPROXY_AWE.log.

        For additional information about the SSH proxy service, see the associated
        documentation.




19.04.2018                         EN-INST-A+W Enterprise Web.docx                    13
1.11 Documentation
1.11.1 Manuals
        With the set-up, the existing manuals are provided in German and English.
        These are in the directory <Programs>\A+W\A+W Enterprise 6
        Web\Doc\Manuals.


1.11.2 SSH proxy documentation
        This is under <Programs>\A+W\A+W Enterprise 6 Web\fxsshproxy\doc

1.12 Tips and tricks
1.12.1 Adding sites after the fact
A new site can also be added manually without new installation.
Use the Config Tool for this. In the 2nd dialog, you can enter as many server/client
combinations as you like. For this, after completion of the configuration, the appropriate links
are created on the Start menu in the A+W folder.

1.12.1 AutoUpdate
The A+W Enterprise Web Frontend Setup is currently NOT AutoUpdate capable!

1.13 Uninstalling
You can uninstall the program as usual via Control Panel  Programs and Functions.
    1. Select the entry A+W Enterprise 6 Web and click Uninstall.
    2. Confirm this dialog with "Yes".




    3. A+W Enterprise 6 Web was successfully removed from your PC.




19.04.2018                        EN-INST-A+W Enterprise Web.docx                              14

