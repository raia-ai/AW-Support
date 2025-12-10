---
title: "EN INST A+W CAD Designer Shapes"
category: "installation"
product: "A+W CAD Designer Shapes"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W CAD Designer Shapes"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions  A+W CAD Designer 6 (Shapes)     Change history:      Date             Edited by             Remarks                                     Version     11/2012          Bernd Hanewinkel      Version 2012                                1.0     05/2014          Bernd Hanewinkel      CI adjustment                               1.1     07/2014          Bernd Hanewinkel      Screen adjustment                           1.2     09/2016          Bernd Hanewinkel      Adjustments V"
source_file: "EN-INST-A+W CAD Designer Shapes.pdf"
---


# EN INST A+W CAD Designer Shapes

Installation Instructions

A+W CAD Designer 6 (Shapes)

   Change history:

    Date             Edited by             Remarks                                     Version
    11/2012          Bernd Hanewinkel      Version 2012                                1.0
    05/2014          Bernd Hanewinkel      CI adjustment                               1.1
    07/2014          Bernd Hanewinkel      Screen adjustment                           1.2
    09/2016          Bernd Hanewinkel      Adjustments Version 6                       1.3
    12/2022          Bernd Hanewinkel      Adaptation system requirements              1.4




     The installation instructions will assist the planner with the installation and
     configuration of the software named. Please proceed in the following sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




14.03.2023                         EN-INST-A+W CAD Designer Shapes.docx                  1
Content

   Installation Instructions .............................................................................. 1

   A+W CAD Designer 6 (Shapes) ..................................................................... 1

   1         Overview and the basics .................................................................. 3
   1.1       Requirements ........................................................................................................ 3
   1.1.1     Hardware ............................................................................................................................. 3

   1.1.2     Network ............................................................................................................................... 3

   1.1.3     Software............................................................................................................................... 3

   1.1.4     Database .............................................................................................................................. 3

   2         Installation ...................................................................................... 4
   2.1       Configuration ......................................................................................................... 5
   2.1.1     SetUp settings ...................................................................................................................... 5

   2.1.2     Global settings ..................................................................................................................... 6

   2.1.3     User settings ........................................................................................................................ 8

   2.1.4     services ................................................................................................................................ 9

   2.1.5     Overview .............................................................................................................................. 9

   2.1.6     Update Files ....................................................................................................................... 11

   2.1.7     Finish .................................................................................................................................. 12




14.03.2023                                    EN-INST-A+W CAD Designer Shapes.docx                                                                     2
1 Overview and the basics
1.1     Requirements
1.1.1 Hardware
No special requirements.

1.1.2 Network
A+W CAD Designer 5 requires at least a 10 Mbit Ethernet (10Base2 / IEEE 802.3a, 10Base-T / IEEE
802.3i ) network, better Fast Ethernet or Gigabit Ethernet.

1.1.3 Software
For A+W CAD Designer (Shapes), installation on Windows 10 or Windows 11 is recommended. If it is
to be run on a terminal server, Windows Server 2008 R2 or higher is required.

Reinstallation on older systems is not supported. Windows systems for which Microsoft support has
expired may have limited support.

Please also remember to install all other available service packs for the framework and the
operating system. We recommend to always keep the server up to date with the Microsoft Update
Service.

1.1.4 Database
No database required.




14.03.2023                       EN-INST-A+W CAD Designer Shapes.docx                               3
2 Installation
The setup for A+W CAD Designer 6 is available from \\jupiter\SW_Install\v6.

In connection with A+W Production /A+W Business /A+W Enterprise, A+W CAD Designer (Shapes)
will be installed automatically. For details on these installations please refer to the corresponding
installation instructions. A+W CAD Designer is part of the program group A+W Common. The ticked
box in front of A+W Common means that elements from the A+W Common section will be installed
as well.




                            Fig.: 1             Setup-Launcher – Component selection




14.03.2023                            EN-INST-A+W CAD Designer Shapes.docx                              4
2.1 Configuration
After installation, the configuration tool for A+W CAD Designer is started.

2.1.1 SetUp settings




In the first dialog, the user has to decide if the configuration shall be based on default settings or on
the existing settings. For new installations, the standard configuration should be selected at any
rate. In case of an update, the existing settings should be adopted. If Start from default values is
selected, the existing configuration will be lost!

The system does not decide automatically here. This is due to the fact that configuration settings
will be kept even if the system is uninstalled then installed again. You can therefore keep settings
although the installation is officially a new one.

The standard settings will be determined based on the installed programs.

If you use Next to move through the following menus you will always get an executable system. This
is perfectly sufficient in the A+W Enterprise/Business environment.

Close aborts the configuration without further changes and is therefore the right choice for an
update. Next will bring you to further settings.




14.03.2023                         EN-INST-A+W CAD Designer Shapes.docx                                     5
2.1.2 Global settings




The following menu serves to select a couple of global settings. The screenshot shows the default
setting for the fields with A+W Production installed. SN is configured in the SN Server Directory, in
this case in the sub-directory SN of the Alcim Server Directory, i.e. in trans\SN. The user-specific
configuration is based on the ALCIM Station ID. The SN catalog for standard shapes is found in
\trans\SN\Catalog.

If A+W Production has not been installed, the directory %ProgramData%\A+W\Techsoft\SN is
chosen as the default location for the configuration, i.e. usually C:\ProgramData\A+W\Techsoft\SN.
This is not the installation directory (c:\Program Files (x86)\A+W\Techsoft\SN)! The installation
directory usually offers only limited access rights which make a change of configuration difficult and
quite error-prone.

The settings for the SN Server Directory is the main switch in the AW Enterprise/ AWBusiness
environment. A central configuration can be set up here by means of network release.

Via the protocol button, the trace and log level can be set.




14.03.2023                         EN-INST-A+W CAD Designer Shapes.docx                                  6
14.03.2023   EN-INST-A+W CAD Designer Shapes.docx   7
2.1.3 User settings




The next dialog shows the settings for the current user. During installation this is usually an
administrator, i.e. none of the future users so that his menu is just meant for information. If Use
ALCIM Station ID has been selected in the first menu, the field Station ID is grey and cannot be
changed. Otherwise, you can enter a (SN) Station ID for the current user. This way, a user-specific
CAD Designer configuration can be defined in A+W Business/A+W Enterprise.




14.03.2023                        EN-INST-A+W CAD Designer Shapes.docx                                8
2.1.4 services




The next dialog configures the users for which A+W CAD Designer runs as a service. The user for
scheduling should be entered here (if scheduling shall be started on this computer). A user should
be added by means of the button Add user. All necessary system settings will be made now so that
the processes can be run in the background.

When you proceed to the next menu, the settings will be saved in the Registry. Up to that point you
can use Close to abort the configuration; the system will remain unchanged.

2.1.5 Overview




14.03.2023                       EN-INST-A+W CAD Designer Shapes.docx                                 9
Menu Overview shows a list of settings. At the bottom, the entry in category Registry shows that the
switches have been set successfully.

Meaning of the paths:

    •   SN Installation Directory: Installation directory. This is where SN.exe is found.

    •   SN User Directory: This is the directory in which SN is executed. This is the standard path
        in which SN searches first for data without an absolute path. This is where (in the
        production environment) the files Block.PTH and opt2txt.dat should exist.

    •   SN.INI Path: The path for SN.INI

    •   User Data Directory: The specific user data are stored here. The configuration tool shows
        the path for the user who has started the configuration tool. For the SetUps this is the
        installing user. In connection with ALCIM, this path is created by the Station ID. This is
        where additional data can be stored which are copied to the user directory when SN.exe
        is started. Supplements for SN.ini can also be stored here which override the switches in
        the standard Sn.ini. Example: a SN.ini which only includes the lines
        [Customer]
        Machines = BZ1


14.03.2023                         EN-INST-A+W CAD Designer Shapes.docx                               10
        . The machine PC1 is enabled for this user; all other machines are disabled. Still, all
        machines can be listed in the central SN.ini to permit a central configuration.

    •   DefaultData: Data stored here will be copied to %APPDATA%\Techsoft\SN for all users.


    •   SN ServerDirectory: central configuration directory for SN.

    •   Last, there are two entries for BLOCK.PTH. The first defines the contents of the file
        BLOCK.PTH, i.e. the path for the block file. The second shows where the BLOCK.PTH can
        be found.

        The configuration tool can even be started without administrator rights. In this case, only
        this menu appears, showing a list of settings.

2.1.6 Update Files




Next, the configuration tool copies data from the installation section to the configuration section
(e.g. Sn.ini). In case of an update, there can be already data there. The tool offers a list of all files

14.03.2023                          EN-INST-A+W CAD Designer Shapes.docx                                    11
with conflicts in that case. This will be e.g. SN.ini if it does not match the standard SN.ini. These files
will not be overwritten automatically unless the user ticks them on the list.

2.1.7 Finish




The configuration of the service is now finished. The path for the LOG file appears.




14.03.2023                          EN-INST-A+W CAD Designer Shapes.docx                                  12

