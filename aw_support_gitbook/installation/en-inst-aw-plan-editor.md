---
description: "EN INST A+W Plan Editor"
---



# EN INST A+W Plan Editor

        Installation Instructions

        A+W Plan Editor
   Change history:
    Date         Edited by              Comments                   Version
    2014-07-23   Michael Hartmann       Release 5.4                5.4




19.02.2021                          EN-INST-A+W Plan Editor.docx     1
Contents

   Installation Instructions ..................................................................... 1

   A+W Plan Editor ................................................................................. 1

   1         Overview and Basics............................................................... 3
   1.1       Requirements ............................................................................................. 3
   1.1.1     Hardware .................................................................................................... 3
   1.1.2     Network ...................................................................................................... 3
   1.1.3     Software ..................................................................................................... 3
   1.1.4     Database .................................................................................................... 3

   2         Installation ............................................................................... 4
   2.1       Directory Structure...................................................................................... 7
   2.2       Settings ...................................................................................................... 7
   2.2.1     A+W Plan Editor ConfigTool ....................................................................... 7
   2.2.2     Parameters ................................................................................................. 9
   2.2.3     Registry ...................................................................................................... 9
   2.3       Installation Result ....................................................................................... 9
   2.4       Alternative Installations............................................................................... 9
   2.5       Patches ...................................................................................................... 9
   2.6       Uninstalling ............................................................................................... 10




19.02.2021                                   EN-INST-A+W Plan Editor.docx                                                   2
1 Overview and Basics
1.1     Requirements
1.1.1 Hardware
No special requirements.
1.1.2 Network
A+W Plan Editor does not require a network.
1.1.3 Software
For A+W Plan Editor, Microsoft Windows 7 is the minimum requirement. If it is to be
run on a terminal server, Windows Server 2008 R2 is required.

Please also remember to install all other available service packs for the framework
and the operating system. We recommend to always keep the server up to date with
the Microsoft Update Service.
The .NET Framework 3.5 SP1 is installed by A+W SetupLauncher. This installation
takes about 30 minutes! If possible, please install .NET Framework in advance (or
have it installed).
1.1.4 Database
If you want to manually create patterns with A+W Plan Editor, certain master data
(article and parameters) must be maintained in a database. The Microsoft Access 97
database that is required for this purpose is automatically installed by the setup.




19.02.2021                      EN-INST-A+W Plan Editor.docx                          3
2 Installation

Subsequently, please proceed in the following order during installation:
        1. Start the A+W Setup Launcher. Subsequently, the following splash screen opens:




        2. After you have confirmed the dialog by clicking "Next", the following new dialog opens for
           the selection of the diskset. Select "Create new diskset":




19.02.2021                            EN-INST-A+W Plan Editor.docx                                  4
        3. This is followed by a dialog in which the source and target directory can be entered:




        4. Setup-Launcher now lists all components installed so far:




19.02.2021                            EN-INST-A+W Plan Editor.docx                                 5
        5. In the next dialog, select A+W Plan Editor from the components to be installed:




        6. Now the software is being installed:




        7. The program has been successfully installed.




19.02.2021                            EN-INST-A+W Plan Editor.docx                           6
2.1 Directory Structure
    -   By default, A+W Plan Editor is installed in folder "C:\Programme\A+W\Techsoft\Planedit".

2.2 Settings
2.2.1 A+W Plan Editor ConfigTool
In A+W Plan Editor Config Tool you can set the settings for protocolling. For this
purpose, click on the Protocol button in the first dialog of the A+W Plan Editor Config
Tool. The following dialog opens where you can set the protocolling settings:




A+W Plan Editor only uses tracing, therefore the values in the "Trace Level" column
must be set correspondingly.
In addition, you can use A+W Plan Editor Config Tool to select the language that
should be used for the program interface:




19.02.2021                            EN-INST-A+W Plan Editor.docx                                 7
In the next dialog, which opens when you click "Next" in the first dialog of the A+W
Plan Editor Config Tool, you can configure the path for the BLOCK file (in which the
existing free shapes are saved). Usually, the correct path is already defined here
after the installation.




19.02.2021                      EN-INST-A+W Plan Editor.docx                           8
By clicking on the "Next" button, you will reach the last dialog of the A+W Plan Editor
Config Tool in which you can configure the shape catalog that should be used by the
program. Here, the correct value is also usually already define.




2.2.2 Parameters
2.2.3 Registry
All program settings are saved in the registry. In order to configure any of these
values, you must start the Settings Editor which has been installed by the setup in
the program directory of A+W Plan Editor.

2.3 Installation Result
In the start menu under A+W, select the A+W Plan Editor shortcut and start the
program.

2.4     Alternative Installations
Unknown.


2.5 Patches
Designation          Description                          Precondition




19.02.2021                       EN-INST-A+W Plan Editor.docx                             9
2.6 Uninstalling
To uninstall the software, select menu item "Software" in the Control Panel. Now
A+W Plan Editor can be uninstalled in here.




19.02.2021                      EN-INST-A+W Plan Editor.docx                       10

