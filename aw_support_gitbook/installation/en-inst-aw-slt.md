---
description: "EN INST A+W SLT"
---



# EN INST A+W SLT

          Installation Instructions

          A+W SLT
   Change history:
    Date           Edited by               Remarks                                     Version
    13.11.07       MP                      Original version                            0.9
    15.06.17       MP                      Information regarding Windows environment   1.0
    16.04.25       MP                      Update                                      1.1




     The installation instructions will assist the planner with the installation and
     configuration of the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




19.02.2021                                 EN-INST-A+W SLT.docx                          1
Content

   Installation Instructions ..................................................................... 1

   A+W SLT ............................................................................................. 1

   1         New Installation of the Version .............................................. 3
   1.1       Overview and the basics ............................................................................ 3
   1.2       Time requirement ....................................................................................... 3
   1.2.1     Installation time for the software ................................................................. 3
   1.3       Requirements ............................................................................................. 4
   1.3.1     Hardware .................................................................................................... 4
   1.3.2     Network ...................................................................................................... 4
   1.3.3     Software ..................................................................................................... 4
   1.4       Procedure ................................................................................................... 4
   1.5       Settings ...................................................................................................... 9
   1.5.1     Licensing .................................................................................................... 9
   1.5.2     Creating a New User ................................................................................ 10
   1.5.3     Customer-specific configuration ............................................................... 12
   1.6       Result of the installation ........................................................................... 13
   1.7       Installation alternatives ............................................................................. 13
   1.7.1     Network Mode .......................................................................................... 13
   1.8       Uninstalling ............................................................................................... 15
   1.8.1     A+W SLT Uninstallation ........................................................................... 16
   1.8.2     Firebird Uninstallation ............................................................................... 18
   1.8.3     FBDriver Uninstallation ............................................................................. 18




19.02.2021                                       EN-INST-A+W SLT.docx                                                       2
1 New Installation of the Version
The following installation instructions assume that there is no previous version
installed.
The update of an earlier release version of the A+W SLT is performed exactly as a
new installation.
A+W SLT can be operated in two modes, single workstation and network mode.
These installation instructions describe both modes. For the network mode, the A+W
SLT Network Driver is required. The differences between network and single
workstation can be found in the chapter Installation alternatives (1.10.1).
A Firebird 2.1 database is installed with A+W SLT. Its setup is integrated in the A+W
SLT setup.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during
installation:
    -   Creation of the necessary set-ups
            o A+W SLT
            o If necessary, a A+W SLT network driver
    -   Installation with the Setup Launcher
    -   Licensing of the A+W SLT
    -   User set up in A+W SLT
    -   Release of program directory (network mode)

1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data:
1.2.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times
will vary for different computers. The installation time specified was determined
using a reference device with the following characteristics:
    -   Processor: 3000 Mhz
    -   RAM: 4 GB
    -   Other: /
For an initial or new installation, an installation time of 20 minutes must be
anticipated for the reference device. For higher or lower-power hardware, shorter or
longer installation times must be anticipated.




19.02.2021                            EN-INST-A+W SLT.docx                                3
1.3 Requirements
1.3.1 Hardware
Up-to-date Windows computer or server.
1.3.2 Network
For the installation itself, no network access is necessary.
To operate the A+W SLT in network mode, there has to be a connection to the A+W
SLT main installation and the company network.


IMPORTANT! The server on which A+W SLT is installed, must be in the same
Windows domain in which the A+W Enterprise Frontend is installed. The server must
be listed in the list of trusted computers.


1.3.3 Software
Supported operating systems:
    -   Windows XP
    -   Windows 7
    -   Windows 8
    -   Windows Server 2008 R2
    -   Windows Server 2012 R2

1.4 Procedure
For the installation, please proceed in the following sequence:
    1. Installation of A+W SLT with the Setup Launcher
        On the Component Selection dialog on the External Software node, select the
        A+W SLT module. Currently, there are no depending Setups.




19.02.2021                          EN-INST-A+W SLT.docx                              4
    2. Configuration of A+W SLT during setup




19.02.2021                       EN-INST-A+W SLT.docx   5
        To proceed with installation, enable checkbox "I read the license agreement
        and accept the conditions",




19.02.2021                         EN-INST-A+W SLT.docx                               6
        When selecting the A+W SLT Poweruser, a desktop icon is created on the
        desktop. This is not the case for A+W SLT Standardusers. After selecting an
        option, click "Weiter".
        Confirm the following dialogs with "Proceed" until installation starts. No other
        settings are required.
        Then, the installation of the Firebird database starts automatically.




19.02.2021                           EN-INST-A+W SLT.docx                                  7
        In dialog License agreement select "I accept the agreement". Confirm the
        following dialogs with "Proceed". No other configurations are required.




19.02.2021                         EN-INST-A+W SLT.docx                            8
        After a successful installation of A+W SLT the following dialog appears.



1.5 Settings
1.5.1 Licensing
Licensing is carried out under "Init Passwort". The license is ordered via the
Contract department of A+W Software GmbH from Sommer Informatik GmbH.




19.02.2021                          EN-INST-A+W SLT.docx                           9
1.5.2 Creating a New User
The employees who are going to use A+W SLT have to be set up in A+W SLT.
Start A+W SLT and click the menu option "Bearbeiter" . Confirm login with "OK". No
password is required.




19.02.2021                        EN-INST-A+W SLT.docx                               10
In the next dialog, you will see an overview of employees that have been previously
entered. On the right side, there are three icons to add new users and to edit or
delete existing ones.




19.02.2021                        EN-INST-A+W SLT.docx                                11
It is important that the A+W Enterprise login name is entered in the field, so that
A+W Enterprise and A+W SLT can communicate with one another.




1.5.3 Customer-specific configuration
You can find the instructions for customer-specific configuration in the release notes
for construction products regulations Part 2.




19.02.2021                          EN-INST-A+W SLT.docx                              12
1.6 Result of the installation
The program files were unpacked under C:\Program Files (x86)\Sommer Informatik
GmbH\A+W SLT.
An icon was stored on the desktop with which you can start A+W SLT.

1.7 Installation alternatives
1.7.1 Network Mode
To access the A+W SLT program (A+WSLT.exe) the program directory
C:\Program Files (x86)\Sommer Informatik GmbH\A+W SLT has to be released
on the server.
    1. Select the program directory, right click and select the item "Erweiterte
       Freigabe...".




19.02.2021                        EN-INST-A+W SLT.docx                             13
    2. In this dialog, click "Erweiterte Freigabe" again.




    3. Fill in the next dialog as follows. Pay attention to share names, remove any
       blanks! Click on "Berechtigungen".




19.02.2021                           EN-INST-A+W SLT.docx                             14
    4. In the authorizations ["Berechtigungen"] assign full access to the directory to
       the user "Jeder".




    5. The A+W SLT Network Driver (FBTreiber) has to be installed on all client PCs
       that are to have access to the central A+W SLT. For this, please refer to the
       respective installation instructions.


1.8 Uninstalling
To uninstall the software, go to the Control Panel under "Programs and Features",
select the entries "S+W SLT", "FBTreiber" and "Firebird" and execute the "Uninstall"
option for each.




19.02.2021                          EN-INST-A+W SLT.docx                                 15
1.8.1 A+W SLT Uninstallation




19.02.2021                     EN-INST-A+W SLT.docx   16
19.02.2021   EN-INST-A+W SLT.docx   17
1.8.2 Firebird Uninstallation




Here, select the option " Ja, für Alle".


1.8.3 FBDriver Uninstallation




19.02.2021                           EN-INST-A+W SLT.docx   18

