---
description: "EN INST A+W License Client"
---



# EN INST A+W License Client

          Installation Instructions

          A+W License Client
   Change history:
    Date           Edited by               Remarks                                     Version
    2014-07-18     J. Makowka              Original version                            1.0
    2022-12-08     B. Hanewinkel           System requirements                         1.1




     The installation instructions will assist the planner with the installation and
     configuration of the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




14.03.2023                            EN-INST-A+W License Client.docx                    1
Content

   Installation Instructions ..................................................................... 1

   A+W License Client ............................................................................ 1

   1         New Installation of Version 5 SP4 .......................................... 3
   1.1       Overview and the basics ............................................................................ 3
   1.2       Time requirement ....................................................................................... 3
   1.2.1     Installation time for the software ................................................................. 3
   1.2.2     Conversion time for data stock ................................................................... 3
   1.3       Requirements ............................................................................................. 3
   1.3.1     Hardware .................................................................................................... 3
   1.3.2     Network ...................................................................................................... 3
   1.3.3     Software ..................................................................................................... 4
   1.4       Procedure ................................................................................................... 4
   1.5       Incompatibilities ........................................................................................ 17
   1.6       Directory structure .................................................................................... 17
   1.7       Settings .................................................................................................... 17
   1.7.1     Protocol Settings ...................................................................................... 18
   1.8       Result of the installation ........................................................................... 20
   1.9       Configuration ............................................................................................ 21
   1.10      Alternative Installations............................................................................. 21
   1.11      Uninstalling ............................................................................................... 21

   2         Update License Client ........................................................... 22

   3         Appendix ................................................................................ 23
   3.1       Configuration Settings for Experts and Special Users .............................. 23
   3.1.1     ConfigTool for Computer-Wide Settings (License Client Machine Settings
             Config Tool) .............................................................................................. 23
   3.1.2     User-Specific Configuration (License Client User Settings Config Tool) .. 31

   4         Table of Figures ..................................................................... 38




14.03.2023                                 EN-INST-A+W License Client.docx                                                 2
1 New Installation of Version 5 SP4
The following installation instructions assume that there is no previous version
installed.

1.1 Overview and the basics
For the installation of the license client you must have local administrator rights on
the machine on which the client shall be installed.
The following list provides and overview of the work that must be done during
installation:
    -   Installation of the license client with the Setup Launcher. Normally, you install the license
        client together with other A+W products.

1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data:
1.2.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times
will vary for different computers. The installation time specified was determined
using a reference device with the following characteristics:
    -   Processor: Intel Xeon E5520, 2.67 GHz
    -   RAM: 4 GB
For an initial or new installation, an installation time of 2 minutes must be anticipated
for the reference device. For higher or lower-power hardware, shorter or longer
installation times must be anticipated. When combined with the installation of other
A+W software, the time required for installing the clients' licence is negligible.
1.2.2 Conversion time for data stock
Data is not converted. Therefore no time is required for this purpose.

1.3 Requirements
1.3.1 Hardware
There are no additional hardware requirements.
1.3.2 Network
If the license server is located on a different machine, a stable network connection to
this machine must exist.




14.03.2023                            EN-INST-A+W License Client.docx                                   3
1.3.3 Software
An A+W license server must exist, run and be available in the network. This
condition is met even if an A+W license server is installed on the same machine on
which the license client is supposed to be installed or if the A+W license server is
installed on the machine during the course of the same SetupLauncher session.


For the license client, installation on Windows 10 or Windows 11 is recommended. If
it is to be run on a terminal server, Windows Server 2008 R2 or higher is required.
Reinstallation on older systems is not supported. Windows systems for which
Microsoft support has expired may have limited support.


1.4 Procedure
For the installation, please proceed in the following sequence:
        1. Start the installation of the SetupLauncher from your diskset. Usually, you will only do this
           once and then install all required A+W packages.




             Fig. 1: Start SetupLauncher installation




14.03.2023                             EN-INST-A+W License Client.docx                                 4
        2. Confirm the administrator rights for the installation




             Fig. 2: Confirm the administrator rights

        3. You may receive additional safety information and queries depending on the operating
           system of the machine and the configuration of the computer. Always confirm with
           "Continue", "OK", etc.

        4. Wait until SetupLauncher has been installed.




             Fig. 3: Example of an installation progress box




14.03.2023                             EN-INST-A+W License Client.docx                        5
        5. Click "Next" in the welcome dialog of SetupLauncher.




             Fig. : Welcome dialog of SetupLauncher4

        6. The license client is included in the standard disksets that SetupLauncher offers for the
           installation. Usually, you select one of these disksets, e.g. "A+W Business Pro." You can
           also select one of the other standard disksets or create your own diskset. The approach
           depends on the A+W product you intend to install.




             Fig. 5: Select diskset

        7. In the SetupLauncher, you can now set up the installation plate and hotfix source,
           execute an FTP download or configure the auto update. For this purpose, please read
           the documentation on the product you are installing. Unless the corresponding



14.03.2023                            EN-INST-A+W License Client.docx                              6
             documentation includes different instructions, you can leave the preset default values
             unchanged and exit the dialog by selecting "Next." You can also execute the auto update
             configuration later.




             Figure 6: SetupLauncher - System settings

        8. The next dialogue shows the installed A+W software. Since this is a new installation, only
           the SetupLauncher is listed. Exit the dialog using "Next."




             Figure 7: Installed A+W software

        9. In the following dialog, you can select the software that is to be installed. For standard
           disksets the license client modules are already preselected. The actual module is "A+W



14.03.2023                            EN-INST-A+W License Client.docx                               7
             License Client." The modules "A+W Infrastructure 5 Collector Services" and "A+W
             Infrastructure 5 Middleware" are additionally required so that the protocols of the license
             client can be provided centrally. These modules are also preselected. If you install the
             license client in a different context, you may need to make these selections yourself.
             After selecting, exit the dialog using "Next."




             Fig. 8: Modules of the license client




14.03.2023                              EN-INST-A+W License Client.docx                                8
        10. Depending on the product you are installing, you may now need to fill out one or several
            entry dialogs. Please look up these dialogs in the installation instructions for the product
            you are installing.

             Lastly, the entry dialog for the infrastructure configuration opens. Under "Host," enter the
             name of the server on which the network-wide service locator runs. Please read the
             installation instructions for the infrastructure services for further information.




             Figure 9: Infrastructure configuration




14.03.2023                             EN-INST-A+W License Client.docx                                  9
        11. The SetupLauncher has now collected all required data. Leave the preset selection
            "Install software and save setup configuration to an XML file" and click "Next."




             Figure 10: Start installation

        12. Now you have to enter a name under which the diskset is saved for later references.




             Fig. 11: Save diskset



14.03.2023                               EN-INST-A+W License Client.docx                          10
        13. Now the installation of the modules starts. During the installation, the Setup Launcher
            displays the installation progress. You may also see various progress displays and notes.
            Wait until the configuration part of the SetupLauncher session starts.




             Figure 12: Installation progress




14.03.2023                             EN-INST-A+W License Client.docx                             11
        14. The configuration tool for the license client is called up in the configuration section of the
            SetupLauncher session. On server systems, it is possible that the tool opens behind the
            SetupLauncher dialog. If this is the case, click on an area of the configuration tool that
            does not include any buttons, in order to get the tool to the front.




             Fig. 13: Activate config tool




14.03.2023                              EN-INST-A+W License Client.docx                                 12
        15. In the configuration tool, you must select the license server to which the license client
            should connect. If a license server is running on the machine on which you are installing
            the license client, the selection option "The license service is running on this machine" is
            available and preselected. Normally, this is not the case; then this selection option is not
            available and instead the option "The license server is running on another machine" is
            preselected. If this selection has been made, you must always enter the name or the IP
            address of the machine on which the license server is running into the field "Host name
            or IP address." You can have the connection to other machines checked by clicking on
            the "Test" button.

             Note: In order to successfully complete the configuration, it is required that the license
             client can communicate with the specified license server.

             Click "Next" to open the next dialog.




             Fig. 14: Select license server

        16. The configuration tool obtains data from the license server now. During this process you
            will see a message.




             Fig. 15: Obtaining data from the license server




14.03.2023                              EN-INST-A+W License Client.docx                               13
        17. Now you must confirm or enter the settings for the workstation. Usually, the top three
            selection options are deactivated since there are no selection options available in the
            license. If a selection option has been enabled, make sure you make the correct
            selection for the workstation. You can also change the selection later by selecting the
            "License Client Machine Settings Config Tool" from the A+W program selection. Click the
            "Next" button to show the results.




             Fig. 16: Workstation settings




14.03.2023                             EN-INST-A+W License Client.docx                           14
        18. You will see the configuration results in the bottom section. Click the "Next" button to
            complete the configuration.




             Fig. 17: Configuration results




14.03.2023                              EN-INST-A+W License Client.docx                           15
        19. Now the configuration of the license client within the scope of the SetupLauncher session
            is completed. Click on the "Finish" button to exit the configuration tool and continue with
            the configuration tools of other components, if applicable. Please look up the installation
            instructions for the remaining modules to be installed in order to obtain information about
            the processes and entries.




             Fig. 18: Completing the installation

        20. As soon as all required configurations have been set, you will see the completion
            notification of the installation. Please wait until you see this notification. SetupLauncher
            may still be running operations in the background even if it seems in the foreground as if
            the installation is finished.




             Fig. 19: Installation end




14.03.2023                               EN-INST-A+W License Client.docx                              16
        21. After installation has been completed, close the SetupLauncher using the "End" button.




             Figure 20: Terminate SetupLauncher


1.5 Incompatibilities
No incompatibilities are known.

1.6 Directory structure
The program does not use any data on the hard disk. The protocols are stored at the
usual location (%PROGRAMDATA%\A+W\Log).

1.7 Settings
All settings shall be made with one of the configuration tools for the license client.
There is the "License Client Machine Settings Config Tool" for machine-wide
settings and the "License Client User Settings Config Tool" for user-specific
settings. The latter is only important in exceptional cases and is usually not used.
In addition to the basic configuration that has been made during the installation,
only the protocolling configuration is of general interest. The configuration tools
additionally offer a number of advanced configuration settings. These settings are
described in the attachment.




14.03.2023                           EN-INST-A+W License Client.docx                                 17
1.7.1 Protocol Settings
There are two sections in the license client for which the protocol settings can be
set at different locations. On a client machine there is a license proxy service. The
protocol settings for this proxy service can be set with the "License Client
Machine Settings Config Tool."
Every program that is subject to license includes a component for communicating
with the license proxy. This component does not have its own protocol category. It
uses the category "AlbwirBasis" to write entries. You can set this category in the
"Basis" tab of the protocol configuration of the configuration tool for the program
in question.
1.7.1.1 Protocol settings of the license proxy service
The protocol settings for the license proxy service can be changed with the
"License Client Machine Settings Config Tool." You can start this tool from the
folder "Config Tools" in the A+W start window. You have to have administrator
rights to use this tool.




14.03.2023                      EN-INST-A+W License Client.docx                         18
The configuration tool differs from the variant that you see during the installation
with the SetupLauncher by the two buttons "Expert Settings" and "Protocol" on
the first page. The settings that can be made using the button "Expert Settings"
are described in the attachment. Click on the "Protocol" button to change the
protocol settings. Click on [Protocol] to change the protocol settings..




Fig. 21: License Client Machine Settings Config Tool

The settings on the "LicenseProxy" tab relate to the areas of the license proxy.




Fig. 22: License proxy settings



14.03.2023                            EN-INST-A+W License Client.docx                  19
AWCCacheLicensing            Entries that relate to licensing from the license cache on the
                             client side
AWCLicenseCache              Entries that relate to the operation of the license cache on the
                             client side (e.g. activation, deactivation, mode switching)
AWCLicenseClient             Entries that relate to the communication with connected clients
AWCLicenseProxy              Entries that relate to the operation of the license proxy (e.g.
                             communication errors with the license server, notifications from
                             the Windows service)
AWCLicenseWatcher            Entries of the Watcher service that monitors the license proxy
AWCLicensing                 Entries that relate to the communicated licensing (license server
                             or license cache)
On the "Basis" tab, you will see the protocol settings for the basis libraries.




Fig. 23: Settings for the basis libraries

AlbwirBasis        Entries resulting from functions of the Albwir.Basis and other basis libraries.
                   Many base functions, e.g. standardized database functions use this
                   protocol category to write entries.
[…]                Special protocol categories of certain functions. Please leave the settings
                   for these categories under Trace Level at "Error" until you are requested by
                   a developer to change them. Changes to these protocol categories can
                   result in log occurrences in the range of gigabytes within very short periods
                   of time.

After you have carried out the requested changes, click the "OK" button to save the
changes. Exit the configuration tool by clicking "Next" until you can exit the tool using
"Finish." This will trigger a restart of the license proxy so that the new settings take effect.
Please note that it is useless to enter user-specific settings for the protocol level. The
license proxy is a Windows service that runs under a separate service user. Therefore,
user-specific settings do not take effect.

1.8 Result of the installation
The installation has been carried out correctly if you see the text "Success" in the
two result lines of the dialog shown in Chapter 1.4, item 18.


14.03.2023                                  EN-INST-A+W License Client.docx                          20
1.9 Configuration
No further configurations are required.

1.10 Alternative Installations
Support is available for the communication procedure of older programs subject to
license. Read the attachment for details.

1.11 Uninstalling
You can uninstall the license client by using the Windows Control Panel. Uninstalling
is basically only necessary if the A+W software is to be deleted from a machine.




Fig. 24: Uninstall license client




14.03.2023                          EN-INST-A+W License Client.docx                 21
2 Update License Client
The update of the license client does not differ from a new installation. The
previously set values are preset in the configuration tool in the configuration section
of the SetupLauncher session and do not need to be reentered.




14.03.2023                      EN-INST-A+W License Client.docx                           22
3 Appendix


3.1 Configuration Settings for Experts and Special Users

3.1.1 ConfigTool for Computer-Wide Settings (License Client Machine
      Settings Config Tool)




             Fig. 25: License client configuration – basic configuration, computer-wide



Key                      Value                        Description
The license service is       •   Not selected         The license service runs on the same
running on this                  (workstations)       computer on which the license client is
machine.                                              running. The settings are then made by the
                             •   Selected             ConfigTool so that they are optimized for this
                                 (process             case.
                                 server)

The license service is       •   Selected             The license service and license client do not
running on another               (workstations)       run on the same computer. In this case, the



14.03.2023                          EN-INST-A+W License Client.docx                              23
Key                      Value                       Description
machine.                    •    Not selected        computer on which the license service runs
                                 (process            must be entered in the field "Host name or IP
                                 server)             address."

Host name or IP          Name of the computer        The name or the IP address of the computer
address                  with the license            on which the license service runs.
                         service
Test                                                 With this button you can check the connection
                                                     to the license service if the option "The license
                                                     service is running on another machine" has
                                                     been selected.
Caution: personal        Visible or hidden           If this note is visible, it means that there are
settings for this user                               user-specific settings that overwrite the
are overriding the                                   computer-wide settings for the logged-on user.
global machine                                       You can check and edit such user-specific
settings                                             settings with the "License Client User Settings
                                                     Config Tool" (see 3.1.2).
                                                     This note is a link which shows a detailed note
                                                     when you click on it (Abbildung 26).
Expert settings                                      Open the advanced dialogs for the expert
                                                     settings with this button (see Abbildung 28 et
                                                     seq.).
                                                     Please note that you can make any setting in
                                                     the expert dialogs – even settings that will
                                                     result in an inoperable system. Therefore, you
                                                     should normally avoid using the expert
                                                     dialogs. You should only use these dialogs if
                                                     you have been asked to do so by an employee
                                                     of A+W Service or a developer.




14.03.2023                         EN-INST-A+W License Client.docx                               24
             Fig. 26: License client configuration – note regarding user-specific settings

This dialog provides more details if the ConfigTool has recognized that there are user-
specific settings that overwrite the computer-wide settings for the logged-on user. It is just
for information purposes.




14.03.2023                           EN-INST-A+W License Client.docx                             25
                   Fig. 27: License client configuration – workstation settings

Key                    Value                         Description
Company group          STANDARD                      Company group under which the licenses will
                                                     be searched for. The company group is the
                                                     highest hierarchy level where licenses are
                                                     granted.
                                                     You can only change this field if more than
                                                     one company group has been configured in
                                                     the license file of the specified license service.
                                                     Default value: Standard
SITE                   STANDARD                      Client under which the licenses will be
                                                     searched for.
                                                     You can only change this field if more than
                                                     one client has been configured in the license
                                                     file of the specified license service.
                                                     Default value: Standard
Workstation (LS)       Name of the                   Workstation under which the licenses will be
                       workstation                   searched for. The workstation is the lowest
                                                     hierarchy level where licenses can be granted.
                                                     You can only change this field if the license file
                                                     of the specified license service includes at



14.03.2023                         EN-INST-A+W License Client.docx                                26
Key                      Value                        Description
                                                      least one named workstation. Then you can
                                                      select one of the named workstations in the
                                                      license file and the computer name. If you
                                                      select the computer name, the licenses will be
                                                      taken from the stock of the "floating licenses."
                                                      Default value: Name of computer




                 Fig. 28: License client configuration – expert settings, named pipe

Please only use this dialog if you are absolutely sure that you know what you are
doing!

There are different variations of this dialog for the different connection types ("Connection").
The other variations are shown and explained in the images below.

Key                      Value                        Description
Connection               WCF Connection to            Connection type for the connection to the
                         Service via PIPE             license server. The dialog always looks
                         (From Version 2009)          different for the different connection types. The
                                                      other variations are shown in the remaining
                                                      images of this section.
                                                      WCF Connection to Service via PIPE (from
                                                      Version 2009) means that the connection is
                                                      established via so-called "named pipes." This
                                                      connection type can only be reliably
                                                      established on a local computer by means of a
                                                      license service. Therefore, the computer
                                                      cannot be specified if you select this
                                                      connection type ("Host name/IP").

Allow modification       Not selected                 This checkbox allows you to edit the input field
                                                      in front of it. This way, settings that are usually



14.03.2023                          EN-INST-A+W License Client.docx                                 27
Key                      Value                        Description
                                                      not changed are protected against
                                                      unintentional changes.
                                                      Default value: not selected
Pipe name                Glaston/SW/License-          Name of the named pipe used for the
                         Pipe                         connection. This name must be the same as
                                                      the one that has been configured for the
                                                      license service.
                                                      Default value: Glaston/SW/LicensePipe
Provide legacy client    Selected                     Determines whether the connection method
interface                                             for applications that was valid until Version
                                                      2008 is supported.
                                                      Default value: selected
Port no.                 1571                         Port that is used for the connection method for
                                                      applications that was valid until Version 2008.
                                                      Default value: 1571
Copy global settings                                  You can only see this button if the settings in
                                                      the dialog do not match the settings that were
                                                      valid prior to the dialog being opened. If you
                                                      can see this button, you can use it to readopt
                                                      the settings in the dialog that were valid prior
                                                      to the dialog being opened. As a result,
                                                      changes that you have made in the dialog will
                                                      be lost.




                  Fig. 29: License client configuration – expert settings, WCF/TCP

Please only use this dialog if you are absolutely sure that you know what you are
doing!

There are different variations of this dialog for the different connection types ("Connection").
The other variations are shown and explained in the other images of this section.




14.03.2023                          EN-INST-A+W License Client.docx                              28
Key                      Value                        Description
Connection               WCF connection to            Connection type for the connection to the
                         service via TCP (from        license server. The dialog always looks
                         Version 2009)                different for the different connection types. The
                                                      other variations are shown in the remaining
                                                      images of this section.
                                                      WCF connection to service via TCP (from
                                                      Version 2009) means that the connection is
                                                      established via TCP/IP and WCF.
Allow modification       Not selected                 This checkbox allows you to edit the input field
                                                      in front of it. This way, settings that are usually
                                                      not changed are protected against
                                                      unintentional changes.
                                                      Default value: not selected
Host name/IP             Name of the computer         DNS name or IP address of the computer on
                         on which the license         which the license service is running.
                         service is running
Port no. (top section)   1572                         Port number via which the connection to the
                                                      license service is established. This port must
                                                      be open for the TCP protocol in the firewall of
                                                      the computer on which the license service is
                                                      running.
                                                      Default value: 1572
Service name             Glaston/SW/License           Name of the TCP service that is addressed via
                                                      the connection. This name must be the same
                                                      as the one that has been configured for the
                                                      license service.
                                                      Default value: Glaston/SW/License
Provide legacy client    Selected                     Determines whether the connection method
interface                                             for applications that was valid until Version
                                                      2008 is supported.
                                                      Default value: selected
Port no. (bottom         1571                         Port that is used for the connection method for
section)                                              applications that was valid until Version 2008.
                                                      Default value: 1571
Copy global settings                                  You can only see this button if the settings in
                                                      the dialog do not match the settings that were
                                                      valid prior to the dialog being opened. If you
                                                      can see this button, you can use it to readopt
                                                      the settings in the dialog that were valid prior
                                                      to the dialog being opened. As a result,
                                                      changes that you have made in the dialog will
                                                      be lost.




14.03.2023                          EN-INST-A+W License Client.docx                                29
                Fig. : License client configuration – expert settings, .net-Remoting30

Please only use this dialog if you are absolutely sure that you know what you are
doing!

There are different variations of this dialog for the different connection types ("Connection").
The other variations are shown and explained in the other images of this section.

Key                      Value                         Description
Connection               Legacy (Remoting)             Connection type for the connection to the
                         Connection to Service         license server. The dialog always looks
                         (Pre Version 2009)            different for the different connection types. The
                                                       other variations are shown in the remaining
                                                       images of this section.
                                                       Legacy (Remoting) Connection to Service (pre
                                                       version 2009) means that the connection is
                                                       established via TCP/IP and .net-Remoting.
                                                       This connection type must be set if the
                                                       addressed license service is a version before
                                                       2009.
Allow modification       Not selected                  This checkbox allows you to edit the input field
                                                       in front of it. This way, settings that are usually
                                                       not changed are protected against
                                                       unintentional changes.
                                                       Default value: not selected
Host name/IP             Name of the computer          DNS name or IP address of the computer on
                         on which the license          which the license service is running.
                         service is running
Port no. (top section)   1570                          Port number via which the connection to the
                                                       license service is established. This port must
                                                       be open for the TCP protocol in the firewall of
                                                       the computer on which the license service is
                                                       running.
                                                       Default value: 1570


14.03.2023                           EN-INST-A+W License Client.docx                                30
Key                      Value                        Description
Service name             AWLicenseSer-                Name of the TCP service that is addressed via
                         vices.rem                    the connection. This name must be the same
                                                      as the one that has been configured for the
                                                      license service.
                                                      Default value: AWLicenseServices.rem
Provide legacy client    Selected                     Determines whether the connection method
interface                                             for applications that was valid until Version
                                                      2008 is supported.
                                                      Default value: selected
Port no. (bottom         1571                         Port that is used for the connection method for
section)                                              applications that was valid until Version 2008.
                                                      Default value: 1571
Copy global settings                                  You can only see this button if the settings in
                                                      the dialog do not match the settings that were
                                                      valid prior to the dialog being opened. If you
                                                      can see this button, you can use it to readopt
                                                      the settings in the dialog that were valid prior
                                                      to the dialog being opened. As a result,
                                                      changes that you have made in the dialog will
                                                      be lost.




3.1.2 User-Specific Configuration (License Client User Settings Config Tool)

This ConfigTool is used to define and edit user-specific settings for the license client. User-
specific settings allow the logged-on user to use settings different from the computer-wide
settings. For example, this is required on a terminal server if a user should receive his
licenses from a separate license stock while the other users obtain them from the stock of
floating licenses.

If there are no settings available yet, you cannot directly change the fields Company group,
Site und Workstation (LS). First of all, you must create a copy of the computer-wide settings
for the logged-on user, using the button Copy global settings. Subsequently, you can
change the settings.




14.03.2023                          EN-INST-A+W License Client.docx                               31
                   Fig. 31: License client configuration – basic settings, user-specific

Key                        Value                         Description
Company group              STANDARD                      Company group under which the licenses will
                                                         be searched for. The company group is the
                                                         highest hierarchy level where licenses are
                                                         granted.
                                                         You can only change this field if more than
                                                         one company group has been configured in
                                                         the license file of the specified license service.
                                                         Default value: Standard
SITE                       STANDARD                      Client under which the licenses will be
                                                         searched for.
                                                         You can only change this field if more than
                                                         one client has been configured in the license
                                                         file of the specified license service.
                                                         Default value: Standard
Workstation (LS)           Name of the                   Workstation under which the licenses will be
                           workstation                   searched for. The workstation is the lowest
                                                         hierarchy level where licenses can be granted.
                                                         You can only change this field if the license file
                                                         of the specified license service includes at



14.03.2023                             EN-INST-A+W License Client.docx                                32
Key                        Value                        Description
                                                        least one named workstation. Then you can
                                                        select one of the named workstations in the
                                                        license file and the computer name. If you
                                                        select the computer name, the licenses will be
                                                        taken from the stock of the "floating licenses."
                                                        Default value: Name of computer
Copy global settings                                    Use this button to copy the computer-wide
                                                        settings into the user-specific settings. You
                                                        have to do this if no user-specific settings are
                                                        available yet and you want to define the user-
                                                        specific settings.
Remove settings                                         Use this button to remove all user-specific
                                                        settings. After the removal of the user-specific
                                                        settings, the computer-wide settings apply for
                                                        the logged-on user.
Expert settings                                         Use this button to open the dialog for the
                                                        expert settings (Abbildung 32 et seq.). This
                                                        dialog allows you to set advanced
                                                        configuration settings, including the connection
                                                        to a license service different from the license
                                                        service that has been set computer-wide.
                                                        Please note that the settings in this dialog may
                                                        result in the logged-on user not being able to
                                                        obtain any more licenses if the settings are
                                                        made incorrectly. Therefore, only use this
                                                        dialog if you are absolutely sure that you know
                                                        what you are doing.



There are different variations of the dialog below depending on the set connection type
(Connection). The variations are individually described in this section.




    Fig. 32: License client configuration – connection configuration, same as computer, user-specific

Please only use this dialog if you are absolutely sure that you know what you are
doing!

Key                        Value                        Description
Connection                 Use Machine                  The computer-wide settings for the connection
                           Connection Settings          to the license service are used.


14.03.2023                            EN-INST-A+W License Client.docx                                   33
Key                           Value                        Description
                                                           This setting represents the most frequent case
                                                           since usually only one deviating workstation is
                                                           specified per user.
                                                           If the same license service as the one that has
                                                           been set computer-wide is used, this setting
                                                           should be used in any case. This ensures that
                                                           the user does not encounter any connection
                                                           problems if the computer-wide connection
                                                           settings are changed.
Copy global settings                                       You can only see this button if the settings that
                                                           have been made in the dialog deviate from the
                                                           settings that were valid prior to the dialog
                                                           being opened.
                                                           Use this button to copy the previously valid
                                                           settings back into the dialog. The changes you
                                                           made in the dialog will be lost.




             Fig. 33: License client configuration – connection configuration, pipe, user-specific

Please only use this dialog if you are absolutely sure that you know what you are
doing!

Please avoid selecting settings in this dialog that are identical to the computer-wide
settings. Later changes to the computer-wide settings would then not have an effect
on the logged-on user. If you want to use the computer-wide settings for connecting
to the license service, please set Connection to "Use Machine Connection Settings."

Key                           Value                        Description
Connection                    WCF connection to            Connection type for the connection to the
                              service via TCP (from        license server. The dialog always looks
                              Version 2009)                different for the different connection types. The
                                                           other variations are shown in the remaining
                                                           images of this section.
                                                           WCF connection to service via TCP (from
                                                           Version 2009) means that the connection is
                                                           established via TCP/IP and WCF.
Allow modification            Not selected                 This checkbox allows you to edit the input field


14.03.2023                               EN-INST-A+W License Client.docx                               34
Key                        Value                        Description
                                                        in front of it. This way, settings that are usually
                                                        not changed are protected against
                                                        unintentional changes.
                                                        Default value: not selected
Pipe name                  Glaston/SW/License-          Name of the named pipe used for the
                           Pipe                         connection. This name must be the same as
                                                        the one that has been configured for the
                                                        license service.
                                                        Default value: Glaston/SW/LicensePipe
Copy global settings                                    You can only see this button if the settings that
                                                        have been made in the dialog deviate from the
                                                        settings that were valid prior to the dialog
                                                        being opened.
                                                        Use this button to copy the previously valid
                                                        settings back into the dialog. The changes you
                                                        made in the dialog will be lost.




         Fig. 34: License client configuration – connection settings, WCF via TCP, user-specific

Please only use this dialog if you are absolutely sure that you know what you are
doing!

Please avoid selecting settings in this dialog that are identical to the computer-wide
settings. Later changes to the computer-wide settings would then not have an effect
on the logged-on user. If you want to use the computer-wide settings for connecting
to the license service, please set Connection to "Use Machine Connection Settings."

Key                        Value                        Description
Connection                 WCF connection to            Connection type for the connection to the
                           service via TCP (from        license server. The dialog always looks
                           Version 2009)                different for the different connection types. The
                                                        other variations are shown in the remaining
                                                        images of this section.
                                                        WCF connection to service via TCP (from
                                                        Version 2009) means that the connection is



14.03.2023                            EN-INST-A+W License Client.docx                                35
Key                        Value                         Description
                                                         established via TCP/IP and WCF.
Allow modification         Not selected                  This checkbox allows you to edit the input field
                                                         in front of it. This way, settings that are usually
                                                         not changed are protected against
                                                         unintentional changes.
                                                         Default value: not selected
Host name/IP               Name of the computer          DNS name or IP address of the computer on
                           on which the license          which the license service is running.
                           service is running
Port no.                   1572                          Port number via which the connection to the
                                                         license service is established. This port must
                                                         be open for the TCP protocol in the firewall of
                                                         the computer on which the license service is
                                                         running.
                                                         Default value: 1572
Service name               Glaston/SW/License            Name of the TCP service that is addressed via
                                                         the connection. This name must be the same
                                                         as the one that has been configured for the
                                                         license service.
                                                         Default value: Glaston/SW/License




      Fig. 35: License client configuration – connection configuration, .net-Remoting, user-specific

Please only use this dialog if you are absolutely sure that you know what you are
doing!

Please avoid selecting settings in this dialog that are identical to the computer-wide
settings. Later changes to the computer-wide settings would then not have an effect
on the logged-on user. If you want to use the computer-wide settings for connecting
to the license service, please set Connection to "Use Machine Connection Settings."

Key                        Value                         Description
Connection                 Legacy (Remoting)             Connection type for the connection to the
                           Connection to Service         license server. The dialog always looks
                           (Pre Version 2009)            different for the different connection types. The


14.03.2023                             EN-INST-A+W License Client.docx                                 36
Key                  Value                      Description
                                                other variations are shown in the remaining
                                                images of this section.
                                                Legacy (Remoting) Connection to Service (pre
                                                version 2009) means that the connection is
                                                established via TCP/IP and .net-Remoting.
                                                This connection type must be set if the
                                                addressed license service is a version before
                                                2009.
Allow modification   Not selected               This checkbox allows you to edit the input field
                                                in front of it. This way, settings that are usually
                                                not changed are protected against
                                                unintentional changes.
                                                Default value: not selected
Host name/IP         Name of the computer       DNS name or IP address of the computer on
                     on which the license       which the license service is running.
                     service is running
Port no.             1570                       Port number via which the connection to the
                                                license service is established. This port must
                                                be open for the TCP protocol in the firewall of
                                                the computer on which the license service is
                                                running.
                                                Default value: 1570
Service name         AWLicenseServices.r        Name of the TCP service that is addressed via
                     em                         the connection. This name must be the same
                                                as the one that has been configured for the
                                                license service.
                                                Default value: AWLicenseServices.rem




14.03.2023                    EN-INST-A+W License Client.docx                                 37
4 Table of Figures
Fig. 1: Start SetupLauncher installation ................................................................................. 4
Fig. 2: Confirm the administrator rights .................................................................................. 5
Fig. 3: Example of an installation progress box ..................................................................... 5
Fig. : Welcome dialog of SetupLauncher4 ............................................................................. 6
Fig. 5: Select diskset .............................................................................................................. 6
Figure 6: SetupLauncher - System settings ........................................................................... 7
Figure 7: Installed A+W software ........................................................................................... 7
Fig. 8: Modules of the license client ....................................................................................... 8
Figure 9: Infrastructure configuration ..................................................................................... 9
Figure 10: Start installation .................................................................................................. 10
Fig. 11: Save diskset ............................................................................................................ 10
Figure 12: Installation progress ............................................................................................ 11
Fig. 13: Activate config tool .................................................................................................. 12
Fig. 14: Select license server ............................................................................................... 13
Fig. 15: Obtaining data from the license server ................................................................... 13
Fig. 16: Workstation settings ................................................................................................ 14
Fig. 17: Configuration results ............................................................................................... 15
Fig. 18: Completing the installation ...................................................................................... 16
Fig. 19: Installation end ........................................................................................................ 16
Figure 20: Terminate SetupLauncher .................................................................................. 17
Fig. 21: License Client Machine Settings Config Tool .......................................................... 19
Fig. 22: License proxy settings ............................................................................................. 19
Fig. 23: Settings for the basis libraries ................................................................................. 20
Fig. 24: Uninstall license client ............................................................................................. 21
Fig. 25: License client configuration – basic configuration, computer-wide ......................... 23
Fig. 26: License client configuration – note regarding user-specific settings ....................... 25
Fig. 27: License client configuration – workstation settings ................................................ 26
Fig. 28: License client configuration – expert settings, named pipe ..................................... 27
Fig. 29: License client configuration – expert settings, WCF/TCP ...................................... 28
Fig. : License client configuration – expert settings, .net-Remoting30 ................................ 30
Fig. 31: License client configuration – basic settings, user-specific ..................................... 32
Fig. 32: License client configuration – connection configuration, same as computer, user-
specific ................................................................................................................................. 33
Fig. 33: License client configuration – connection configuration, pipe, user-specific ........... 34
Fig. 34: License client configuration – connection settings, WCF via TCP, user-specific .... 35
Fig. 35: License client configuration – connection configuration, .net-Remoting, user-specific
............................................................................................................................................. 36




14.03.2023                                           EN-INST-A+W License Client.docx                                                          38

