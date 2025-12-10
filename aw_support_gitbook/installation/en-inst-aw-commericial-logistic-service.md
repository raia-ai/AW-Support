---
title: "EN INST A+W Commericial Logistic Service"
category: "installation"
product: "A+W Commericial Logistic Service"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Commericial Logistic Service"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions            A+W Commercial Logistic Service    Change history:      Date            Edited by                Comments                                 Version      2016-03-16      Bastian Michel           Original Version                         1.0          The installation instructions guide the consultant through the installation and      the configuration process of the cited software. Please proceed in the      following order:        1.      Check the inst"
source_file: "EN-INST-A+W Commericial Logistic Service.pdf"
---


# EN INST A+W Commericial Logistic Service

          Installation Instructions

          A+W Commercial Logistic Service
   Change history:
     Date            Edited by                Comments                                 Version
     2016-03-16      Bastian Michel           Original Version                         1.0




     The installation instructions guide the consultant through the installation and
     the configuration process of the cited software. Please proceed in the
     following order:


     1.      Check the installation requirements.

     2.      Collect the necessary data, additional programs, drivers, etc.

     3.      Consider or calculate the time required.




08.05.2018                       EN-INST-A+W Commericial Logistic Service.docx          1
Content




   Installation Instructions ................................................................... 1

   A+W Commercial Logistic Service ................................................. 1

   1         New installation of version 6 ................................................ 3
   1.1       Overview and Basics .................................................................................3
   1.2       Prerequisites .............................................................................................3
   1.2.1     A+W Business ...........................................................................................3
   1.3       Dependencies ...........................................................................................3
   1.4       Procedure ..................................................................................................3
   1.5       Settings .....................................................................................................3
   1.6       Installation Result ......................................................................................8
   1.7       Uninstalling ................................................................................................9




08.05.2018                          EN-INST-A+W Commericial Logistic Service.docx                                         2
1 New installation of version 6
The following installation instructions assume that no previous version has been
installed. Setup and additional configuration options are described in the
configuration instructions.

1.1 Overview and Basics
Below you will find a list of the work to be carried out during the installation:
    -   Installation of the A+W Commercial Logistic Service


The A+W Commercial Logistic Service is used for the communication between A+W
products (currently A+W Business and A+W Cantor) and the A+W Logistics
Optimizer. It transports the required document data to the Logistics Optimizer and
calculates the route data back again.

1.2 Prerequisites
There are various requirements for installation depending on the respective A+W
program.
1.2.1 A+W Business
For the use of A+W business, such a system has to be installed on the same system
as the BusinessCom.exe is used in the Logistic Service. Plus the respective
language package has to be installed so that the messages are displayed in the
correct language.

1.3 Dependencies
In order for the service to function properly, the A+W infrastructure services must be
installed on the system.

1.4 Procedure
The A+W Commercial Logistic Service has to be installed with the setup launcher.

1.5 Settings
Once the installation has been performed, the user has to be set up under which the
service is to run.




08.05.2018                     EN-INST-A+W Commericial Logistic Service.docx         3
Following installation, the service has to be configured. The A+W Commercial Logistic
Service requires a connection to the databases of A+W Business and A+W Logistics
Optimizer. They are configured in the A+W Infrastructure Web.




08.05.2018                  EN-INST-A+W Commericial Logistic Service.docx               4
Ill. A+W Business database


Please note that the A+W Logistics Optimizer currently only supports SQL servers.




08.05.2018                   EN-INST-A+W Commericial Logistic Service.docx          5
Ill. A+W Logistics Optimizer database

Plus the logical user for A+W Business has to be entered here with which the COM objects
logs in.




08.05.2018                      EN-INST-A+W Commericial Logistic Service.docx              6
Ill. Logical user A+W Business


Plus the backend type also has to be set in A+W Business.




08.05.2018                       EN-INST-A+W Commericial Logistic Service.docx   7
Ill. Type of system used




1.6 Installation Result
If the service can be started via Service Locator Administration, it was correctly
installed.




08.05.2018                 EN-INST-A+W Commericial Logistic Service.docx             8
1.7 Uninstalling
The service can be uninstalled via the Programs and Functions dialog in Windows.




08.05.2018               EN-INST-A+W Commericial Logistic Service.docx             9
08.05.2018   EN-INST-A+W Commericial Logistic Service.docx   10

