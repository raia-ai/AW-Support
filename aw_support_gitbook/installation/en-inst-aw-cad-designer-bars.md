---
title: "EN INST A+W CAD Designer Bars"
category: "installation"
product: "A+W CAD Designer Bars"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W CAD Designer Bars"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions          A+W CAD Designer (Bars)    Change history:      Date            Edited by              Comments                     Version      2012-01-08      Jens Schmidt           Original version             1.0      2014-07-08      Jens Schmidt           Release 5.4                  5.4      2017-01-18      Jens Schmidt           Release 6.2                  6.2     19.02.2021                          EN-INST-A+W CAD Designer Bars.docx    1 Content     Installat"
source_file: "EN-INST-A+W CAD Designer Bars.pdf"
---


# EN INST A+W CAD Designer Bars

        Installation Instructions

        A+W CAD Designer (Bars)
   Change history:
     Date            Edited by              Comments                     Version
     2012-01-08      Jens Schmidt           Original version             1.0
     2014-07-08      Jens Schmidt           Release 5.4                  5.4
     2017-01-18      Jens Schmidt           Release 6.2                  6.2




19.02.2021                          EN-INST-A+W CAD Designer Bars.docx    1
Content

   Installation Instructions .................................................................... 1

   A+W CAD Designer (Bars) ................................................................ 1

   1         Overview and Basics.............................................................. 3
   1.1       Prerequisites .............................................................................................3
   1.1.1     Hardware ...................................................................................................3
   1.1.2     Network .....................................................................................................3
   1.1.3     Software ....................................................................................................3
   1.1.4     Database ...................................................................................................3

   2         Installation .............................................................................. 4
   2.1       Directory Structure.....................................................................................8
   2.2       Settings .....................................................................................................8
   2.2.1     A+W CAD Designer (Bars) ConfigTool ......................................................8
   2.2.2     Parameters ................................................................................................8
   2.2.3     Registry .....................................................................................................8
   2.3       Installation Result ......................................................................................8
   2.4       Alternative Installations..............................................................................9
   2.5       Patches .....................................................................................................9
   2.6       Uninstalling ................................................................................................9




19.02.2021                               EN-INST-A+W CAD Designer Bars.docx                                               2
1 Overview and Basics
1.1     Prerequisites
1.1.1 Hardware
No special requirements.
1.1.2 Network
A+W CAD Designer (Bars) requires at least a 10 Mbit Ethernet (10Base2 / IEEE
802.3a, 10Base-T / IEEE 802.3i ) network; better: Fast Ethernet or Gigabit Ethernet.
1.1.3 Software
For A+W CAD Designer 6, Microsoft Windows 7 is the minimum requirement. If it is
to be run on a terminal server, Windows Server 2008 R2 or newer is required.
Please also remember to install all other available service packs for the framework
and the operating system. We recommend to always keep the server up to date with
the Microsoft Update Service.
The .NET Framework 4.5 is automatically installed by the A+W Setup Launcher.
This installation takes about 30 minutes! If possible, please install .NET Framework
in advance (or have it installed).
1.1.4 Database
No database required.




19.02.2021                   EN-INST-A+W CAD Designer Bars.docx                        3
2 Installation

Subsequently, please proceed in the following order during installation:
        1. Start the A+W Setup Launcher. Subsequently, the following splash screen opens:




        2. After you have confirmed the dialog by clicking "Next", the following new dialog opens for
           the selection of the diskset. Select "Create new diskset":




19.02.2021                         EN-INST-A+W CAD Designer Bars.docx                              4
        3. This is followed by a dialog in which the source and target directory can be entered:




        4. Setup-Launcher now lists all components installed so far:




19.02.2021                         EN-INST-A+W CAD Designer Bars.docx                              5
        5. I0n the next dialogue, select A+W CAD Designer (Bars) from the elements to be installed:




             For standalone-installations please deactivate the „A+W Infrastructure
             CollectorService“ and „A+W Infrastructure Middleware“, as well as Java 7 Update ..“ under
             “External Software”.

             These components make the central evaluation of protocol files possible. To use this
             feature, further components are required.

             In this case you can ignore this warning.




19.02.2021                          EN-INST-A+W CAD Designer Bars.docx                              6
        6. Now the software is being installed:




        7. The program has been successfully installed.




19.02.2021                         EN-INST-A+W CAD Designer Bars.docx   7
2.1 Directory Structure
    -   The A+W CAD Designer (Bars) is installed in directory
        „C:\\Programme\\A+W\\Techsoft\\AWDesign“ by default.
        The configuration file for the program is saved in this directory but can also be read by the
        ALCIM transfer directory (Trans\\AWDesign).

2.2 Settings
2.2.1 A+W CAD Designer (Bars) ConfigTool
The settings for the protocolling can be made in the A+W CAD Designer (Bars)
ConfigTool.




2.2.2 Parameters
2.2.3 Registry
No entries in the registry are required.

2.3 Installation Result
Select the A+W CAD Designer (Bars) link in the start menu in A+W and start the
program.




19.02.2021                          EN-INST-A+W CAD Designer Bars.docx                                  8
2.4     Alternative Installations
Unknown.


2.5 Patches
Designation         Description                        Prerequisite




2.6     Uninstalling
To uninstall the software, select menu „Software“ in system management. You can
now uninstall A+W CAD Designer (Bars) there.




19.02.2021                  EN-INST-A+W CAD Designer Bars.docx                    9

