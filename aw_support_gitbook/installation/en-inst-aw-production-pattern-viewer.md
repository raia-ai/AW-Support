---
title: "EN INST A+W Production Pattern Viewer"
category: "installation"
product: "A+W Production Pattern Viewer"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Production Pattern Viewer"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions   A+W Production Pattern Viewer    Change history:      Date            Edited by               Remarks                                   Version      2019-06-04      DLA                     Original version                          1.0          The installation instructions will assist the planner with the installation and      configuration process for the software named. Please proceed in the following      sequence:        1.      Check the installation requirement"
source_file: "EN-INST-A+W Production Pattern Viewer.pdf"
---


# EN INST A+W Production Pattern Viewer

 Installation Instructions

 A+W Production Pattern Viewer
   Change history:
     Date            Edited by               Remarks                                   Version
     2019-06-04      DLA                     Original version                          1.0




     The installation instructions will assist the planner with the installation and
     configuration process for the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




18.06.2019                       EN-INST-A+W Production Pattern Viewer.docx             1
Content

   Installation Instructions ................................................................... 1

   A+W Production Pattern Viewer...................................................... 1

   1         Installation ............................................................................. 3
   1.1       Requirements ............................................................................................3
   1.2       Installation location ....................................................................................3
   1.3       Procedure ..................................................................................................3

   2         Registration ........................................................................... 4
   2.1       Testing.......................................................................................................6

   3         Configuration ......................................................................... 8
   3.1       Connecting to the A+W Realtime Optimizer ..............................................8
   3.2       Breakage reasons .....................................................................................8




18.06.2019                           EN-INST-A+W Production Pattern Viewer.docx                                           2
1 Installation
1.1     Requirements
In addition to a run-capable A+W Realtime Optimizer, the A+W Pattern Viewer
requires an AWSOA environment with an A+W Planning Optimisation Service.

1.2     Installation location
The A+W Pattern Viewer is installed on the machines that output a cutting plan output
on a monitor. This can be an individual PC that output the cutting plan on a monitor
on the cutting table, however it can also be the PC or server on which the A+W
Realtime Optimizer is running and that output the cutting plan on a second monitor.

1.3     Procedure
On the machines in question, the A+W Production Pattern Viewer diskset is executed with
all dependent disksets (A+W Infrastructure Middleware).

After the first installation on a machine, the A+W Pattern Viewer must be restarted manually
and configured.

If the A+W Pattern Viewer is operated on a terminal server, the configuration must be done
once under each Windows user who would like to use this tool.

If this has happened, the A+W Pattern Viewer must be connected to the respective A+W
Realtime Optimizer.

There are more details in the Configuration chapter.




18.06.2019                   EN-INST-A+W Production Pattern Viewer.docx                      3
2 Registration
After the first start of the A+W Pattern Viewer on a machine under a Windows user,
it must be registered in AWSOA. To do this, open the [Register user] menu in the
settings.




First click the [Register application] button:




18.06.2019                     EN-INST-A+W Production Pattern Viewer.docx            4
Then install the [Tray application]:




Now a node of this A+W Pattern Viewer is registered for this machine and Windows user in
the AWSOA Service Locator. There are no services yet.




Now the A+W Pattern Viewer has a tray symbol under this user with which you can end the
node and re-start it.




 This tray symbol must be started when the Windows user logs in; the A+W Pattern Viewer
creates a planned task for this.




For this Windows user, it is now possible to add a service for each client required:




18.06.2019                     EN-INST-A+W Production Pattern Viewer.docx                  5
Selection of the client, the ID of the cutting table, and a sequential number:




Now register this service:




Using this configuration, the services can also be removed again.

Now you can exit A+W Pattern Viewer. In the AWSOA Service Locator, the service is now
created and it can be started. The service has the name consisting of client number, ID of
the cutting table, and the sequential number:




This name of the service is displayed in the A+W Pattern View title bar if it is started via the
Service Locator Administrator.

2.1 Testing
Under tools, the installation includes the A+W Production Pattern Viewer Test Tool, with
which it should be possible to start the A+W Pattern Viewer if it has been registered



18.06.2019                    EN-INST-A+W Production Pattern Viewer.docx                           6
correctly:




18.06.2019   EN-INST-A+W Production Pattern Viewer.docx   7
3 Configuration
3.1 Connecting to the A+W Realtime Optimizer
So that the A+W Pattern Viewer is connected to the A+W Realtime Optimizer, the name of
the AWSO service must be entered in the XOPTON.CFG. Here the key consisting of client
ID of the cutting table and sequential number is separated with a hashtag. In addition, the
path is set permanently to the keyword ICE:
        [XTV]
        ServerName=1#TB1#001
        Path=ICE


3.2 Breakage reasons
The breakage reasons can be configured in the settings that all A+W Pattern Viewers use.
For this, the default group must be selected and the reasons to be used added. For each
breakage reason, the number of the break from the A+W Production master data and a
name must be entered. You can also assign a picture to each reason.

If different A+W Pattern Viewers require different breakage reasons, additional groups can
be added.




18.06.2019                   EN-INST-A+W Production Pattern Viewer.docx                       8

