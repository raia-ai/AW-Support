---
description: "EN INST A+W Clarity Experience"
---



# EN INST A+W Clarity Experience

          Installation Instructions

          A+W Clarity Experience

   Change history:

     Date            Edited by              Remarks                                    Version
     2019-02-01      André Münch            Original Version                           1.0
     2020-12-04      André Münch            Back end dependencies in Chapter 1.3       1.1




     The installation instructions will assist the planner with the installation and
     configuration of the software named. Please proceed in the following sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




19.02.2021                          EN-INST-A+W Clarity Experience.docx                 1
Content




   Installation Instructions ............................................................................. 1

   A+W Clarity Experience .............................................................................. 1

   1         New installation of version 6 .......................................................... 3
   1.1       Overview and the basics .......................................................................................3
   1.2       Requirements .......................................................................................................3
   1.3       Dependencies .......................................................................................................3
   1.3.1     A+W Clarity Suite dependencies under Linux/AIX ............................................................. 4
   1.4       Procedure .............................................................................................................4
   1.5       Settings .................................................................................................................4
   1.6       Result of the installation .......................................................................................4
   1.7       Uninstalling ...........................................................................................................4




19.02.2021                                  EN-INST-A+W Clarity Experience.docx                                                       2
1 New installation of version 6
The following installation instructions assume that there is no previous version installed. Setup and
additional configuration options are described in the configuration instructions.

1.1 Overview and the basics
The following list provides an overview of the work that must be done during installation:

    -   Installation of the A+W Clarity Suite
    -   Installation of the A+W Clarity Suite add-ins (Dispatch, Sales, etc.)


The A+W Clarity Suite is the new interface for A+W Enterprise. In the first step, the Dispatch
Control module will be made available. The Sales module is planned in the second step.

1.2 Requirements
So that the new interface can establish a connection to A+W Enterprise, the following components
have to be installed on the PC:

    •   A+W Infrastructure 6 Middleware

    •   A+W Infrastructure 6 Collector Service



1.2.1   Data from production

In order to be able to display data from production within the A+W Clarity Suite, the following
AWSOA services have to be installed and accessible:
    •   A+W CIM 6 Barcoding Services

    •   A+W Planning 6 Job Services



The installation instructions are available at Installation CIM.

However, these services are optional. The A+W Clarity Suite can also run without them. However, if
the services are installed and accessible, the production information is added to the data
automatically.

1.3 Dependencies
In order for the service to function properly, the A+W infrastructure services has to be installed on
the system.

The Service Locator has to be accessible.


19.02.2021                           EN-INST-A+W Clarity Experience.docx                                3
1.3.1 A+W Clarity Suite dependencies under Linux/AIX
For the set-up of the ICE environment, you have to pay attention to Chapter 8 of the A+W
Enterprise configuration instructions! Without this environment, none of the back end services
will run!

Essentially, before the set-up, you have to check the following files under Linux/AIX (these should
always be up-to-date if possible):

    •   $ALCIBPRG/install/config/iceconfig.1.0.gz (templates for set-up of the services)

    •   $ALCIBPRG/cmd/iceconfig (script for configuration of the services)

    •   $ALCIBPRG/cmd/icenodestart (script for set-up of the ICE node)
    •   $ALCIBPRG/cmd/icenodestartint (internal script for starting the ICE node)

    •   $ALCIBPRG/cmd/icenodestop (script for stopping the ICE node)

    •   $ALCIBPRG/cmd/icegridservers (script for querying the ICE node)
    •   $ALCIBPRG/al_bin/Linux/dispatchservice (binary with the dispatch functionalities)

For the use of the A+W Logistic Optimizer also:

    •   $ALCIBPRG/al_bin/Linux/logistickbackendservice (binary with the functionalities for
        route optimization)

1.4 Procedure
The A+W Clarity Suite has to be installed in the A+W SetupLauncher. The dependent components
should be selected automatically in the SetupLauncher.

The additional add-ins can then be installed on each computer.

1.5 Settings
None.

1.6 Result of the installation
After the installation, the program can be called from the A+W Start menu folder.

1.7 Uninstalling
The program can be uninstalled via the Programs and Functions dialog in Windows.




19.02.2021                          EN-INST-A+W Clarity Experience.docx                               4

