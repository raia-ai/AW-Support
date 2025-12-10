---
title: "EN INST A+W Infrastructure License Statistics Collector"
category: "installation"
product: "A+W Infrastructure License Statistics Collector"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Infrastructure License Statistics Collector"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions            A+W Infrastructure                                      License                 Statistics           Collector    Change history:      Date            Edited by                 Comments                                           Version      2018-09-25      Jürgen Makowka            Original Version                                   1.0          The installation instructions will assist the planner with the installation and      configuration of the"
source_file: "EN-INST-A+W Infrastructure License Statistics Collector.pdf"
---


# EN INST A+W Infrastructure License Statistics Collector

          Installation Instructions

          A+W Infrastructure                                      License                 Statistics
          Collector
   Change history:
     Date            Edited by                 Comments                                           Version
     2018-09-25      Jürgen Makowka            Original Version                                   1.0




     The installation instructions will assist the planner with the installation and
     configuration of the software named. Please proceed in the following se-
     quence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




19.02.2021                 EN-INST-A+W Infrastructure License Statistics Collector.docx            1
Contents

   Installation Instructions .................................................................... 1

   A+W Infrastructure License Statistics Collector ............................ 1

   1         New installation of version 6 ................................................. 3
   1.1       Overview and the basics ...........................................................................3
   1.2       Time requirement ......................................................................................3
   1.2.1     Installation time for the software ................................................................3
   1.3       Requirements ............................................................................................3
   1.3.1     General Information ...................................................................................3
   1.3.2     User ...........................................................................................................4
   1.3.3     Software ....................................................................................................4
   1.4       Procedure ..................................................................................................4
   1.5       Directory structure ...................................................................................13
   1.6       Result of the installation ..........................................................................14
   1.7       Configuration ...........................................................................................14
   1.8       Uninstalling ..............................................................................................15

   2         Update ................................................................................... 16
   2.1       Overview .................................................................................................16
   2.2       Time requirement ....................................................................................16
   2.2.1     Installation time for the software ..............................................................16
   2.3       Requirements ..........................................................................................16
   2.4       Procedure ................................................................................................16
   2.5       Directory structure ...................................................................................16
   2.6       Settings ...................................................................................................16
   2.7       Result of the installation ..........................................................................17
   2.8       Configuration ...........................................................................................17

   3         Appendix: Explanations for the Collector app .................. 18
   3.1       Task and data transmitted .......................................................................18
   3.2       Security ...................................................................................................18
   3.3       Mode of operation....................................................................................19




19.02.2021                    EN-INST-A+W Infrastructure License Statistics Collector.docx                                  2
1 New installation of version 6
The following installation instructions assume that there is no previous version in-
stalled. For updates, an already installed version must be uninstalled before installa-
tion of the new version (see 1.8).


1.1 Overview and the basics
The following list provides an overview of the work that must be done during installa-
tion:
    -   Installation of the Collector app
    -   Enabling of the first password exchange



1.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data:


1.2.1 Installation time for the software
Depending on the computer, storage space, and configuration, the installation times
will vary for different computers. The installation time specified was determined using
a reference device with the following characteristics:
    -   Processor: virtual machine on Intel Xeon, model E5520, 2 virtual processors, 2.27 GHz
    -   RAM: 3.5 GB
    -   Other: N/A
For an initial or new installation, an installation time of 15 minutes must be anticipated
for the reference device. For higher or lower-power hardware, shorter or longer instal-
lation times must be anticipated.


1.3 Requirements

1.3.1 General Information
The A+W Infrastructure License Statistics Collector (Collector app) regularly transmits
data to A+W. Please inform yourself before installation in the project tracing system
(AWDesk, Project Facts) about whether the customer has already signed an appro-
priate contract with A+W!
The Collector app communicates with the A+W Infrastructure Service. Install the 'A+W Infra-
structure License Statistics Collector' diskset on the system on which the 'A+W Infrastructure'




19.02.2021               EN-INST-A+W Infrastructure License Statistics Collector.docx           3
diskset is installed. The minimal version of the A+W Infrastructure Service that is required is
v6 Update 4.
The Collector app transmits your data to an A+W server on the Internet. The data is transmit-
ted encrypted. Make sure that the server 'callback01.com' can be reached via https. You can
test this by calling up the web page https://callback01.a-w.com/CollectorTool from the target
system. Please do not use the web app yet. This call is only to ensure that the web server
can be reached. After the successful call, close the browser!


1.3.2 User
The Collector app is executed in the background without a user having to be logged in. For
the execution, a user is required who has the rights listed below:
      •    Login as batch job
      •    Full access to C:\ProgramData\A+W
      •    Full access to C:\Program Files (x86)\A+W 1
      •    Complete access to the registry range
           HKLM\Software\Wow6432Node\Albat+Wirsam
You should foresee using a local administrator for this task. Local administrators can poten-
tially write to all directories. Using a local administrator therefore represents a security risk. If
on this computer you have already created an appropriate user, you can use it. Make sure in
this case that you know the correct password for the user.
The Config tool makes available a functionality with which you can create a suitable user. If
necessary, use this functionality to create a new user.


1.3.3 Software
The Collector app assumes that an A+W License Server in version V6 Update 4 or higher is
present and that the computer on which the app should be installed is connected to this li-
cense server.



1.4 Procedure
For the installation, please proceed in the following sequence:
           1. With the A+W SetupLauncher from the 'Common' area, install the 'A+W Infrastructure 6
              License Statistics Collector' diskset: The application thus installed will be called the 'Col-
              lector app' below.




1   This is the default installation directory for A+W-Software. However, the customer can have a different default
    installation directory (e.g. on drive D). If the customer has a different installation directory, the customer's direc-
    tory should be used analogously.



19.02.2021                       EN-INST-A+W Infrastructure License Statistics Collector.docx                            4
        2. Before the Config tool is started, you will see the following notice:




                                                                                     The notice asks you
             to check whether the customer has already signed a new software usage agreement. New
             contract include a clause with which the customer agrees to the use of the Collector app.
             The 'Project Facts' system, which sill be used instead of AWDesk in the future, receives a
             characteristic (checkbox) with which you can acknowledge this state. Starting in August
             2018, customers who have signed a new software usage agreement have generally al-
             ready agreed to the clause. If the customer has signed a new software usage agreement
             (according to specifications in the project facts or if you have been able to confirm this
             another way),click '"OK" to continue with configuration of the Collector app. Otherwise,
             click "Cancel." If you click "Cancel," configuration is aborted. The Config tool is not started.
             The Collector app remains installed but is never executed. The rest of the installation in-
             structions are only relevant if you click "OK."




19.02.2021                  EN-INST-A+W Infrastructure License Statistics Collector.docx                   5
          3. After the notice, the Config tool for the Collector app is displayed. The dongle number is
             already filled out here and the field cannot be edited. 2




               Select the time at which the Collector app should make contact with the A+W web
               server for the first time. To do this, in the 'Collector task time:' field, enter one of
               the following values
                    •   'As soon as possible‘ – contact is nearly immediate, in general within the next five
                        minutes.

                    •   'During day‘ – contact will be made during the day, around mid-day

                    •   'During night‘ – contact will be made at night, around midnight
              The setting that you make for 'Collector task time' is not used for the time of initial
              contact. Insofar as nothing else is specified by A+W, the Collector app continues

2   If the Config tool could not determine the dongle number, the 'Dongle No.' field can be edited. In this case, you
    enter the customer's dongle number here. Please note that the missing dongle number means that the configu-
    ration of the license client on the computer may not be correct. Therefore, after installation, check the settings
    in the license client for the connection to the license server!



19.02.2021                     EN-INST-A+W Infrastructure License Statistics Collector.docx                         6
              to connect in the specified period in order to transfer the usage data. A+W can
              overwrite this initial setting in order to straighten out the transfer of data.
              Please make sure that you select a time for the time of first contact at which the
              computer is switched on! It is recommended that you use the default setting 'As
              soon as possible'. 3
              In the 'Collector task user:' field and in the 'Collector task password' field, enter the
              user with whom the Collector app should be executed. This user must have the
              properties in chapter 1.3.2.
                   a) Since for a new installation the already existing user does not yet have the
                      rights for the newly created folder, the tool makes the 'Repair privileges'
                      button available. Use this button to grant the user the required rights!
                   b) If the user that you have entered is a local administrator, you will see a
                      corresponding warning notice:




                      You should use the 'No' button and create a new user with the required
                      rights. There is a button in the Config tool for this. If you nevertheless want
                      to use the administrator user, click the 'Yes' button. This overwrites the war-
                      ning.
                   c) You can use the 'Create new user' button to create a new user who has the
                      required rights. For this, the following dialog opens:




3   The activities of the Collector app do not represent a great load for the computer on which they are performed.
    In addition, the default interval for execution is one month. Therefore, nothing speaks against using the setting
    'As soon as possible.' However, if your customer insists that the transfer should take place outside of normal
    working hours, the two other options are helpful.



19.02.2021                     EN-INST-A+W Infrastructure License Statistics Collector.docx                        7
             In the 'User name‘ field, enter a suitable user name and in the 'Full name'
             and 'Description' fields, enter texts with which it is possible to see the mean-
             ing of the user. Make sure to use a user name that does not exist yet! Enter
             a secure password and confirm it in the 'Confirm password' field. Make sure
             that this password is only known to a small group of people. Then use the
             'Create' button to create the user.
             The Config tool confirms the successful creation with the following mes-
             sage:




             Click 'OK.' The data for the user created is taken over into the Config tool:




19.02.2021         EN-INST-A+W Infrastructure License Statistics Collector.docx             8
             If necessary, note the customer's dongle number. You will need it later to enable
             the initial password exchange.
             Confirm with the 'Next' button and confirm the settings for log and trace on the next
             dialog.
        4. Enable the initial password exchange for the customer. To do this, call up the 'A+W
           Statistics Collector Web Tool‘ at the address https://callback01.a-w.com/Collector-
           Tool and log in with your A+W access data. It is not necessary that you call up the
           tool on the computer on which you are installing the Collector app. You can do this
           just as well from another device with Internet access, insofar as the browser used




19.02.2021                EN-INST-A+W Infrastructure License Statistics Collector.docx           9
               supports JavaScript. The computer on which you have to install must be able to
               reach the web server callback01.a-w.com (via HTTPS).




               You need a login for the domain 'AWAGDOM' of the A+W network. Furthermore,
               you must have been granted certain rights by A+W so that you can use this tool.
               If you have no login or if you should not be authorized, the employees at F&A can
               help you with enabling the initial password exchange. Please contact dongle@a-
               w.com and specify the dongle number, the customer, and the location if necessary.
               The employees in dongle administration will then take care of the enabling for you. 4
               After login, please enter the customer's dongle number. If you have not noted the
               number, you can display it with the 'A+W License Monitor.' After entry, click 'Sel-
               ect.'




4   If you are a member of the A+W installation staff or you work for A+W Service and you still do not have the
    required rights, please contact your colleagues at ICT at a suitable time in order to have them grant you the
    rights. If necessary, enter a case via the ICT helpdesk on the A+W intranet.



19.02.2021                    EN-INST-A+W Infrastructure License Statistics Collector.docx                    10
             The tool now displays the associated customer number (Great Plains ID) and the
             customer information. Please check the customer information and make sure that
             this information matches the customer for which you are doing the installation! If
             the information does not match, please check whether you have specified the cor-
             rect dongle number. You can use the 'Change Dongle' button to change the dongle
             number. Please contact dongle@a-w.com if you determine that there is actually a
             discrepancy between your customer and the information displayed. Employees
             there will help you resolve the discrepancies.
             Normally the information will match the customer's information. In this case, click
             the 'Enable initial password exchange' button. This informs the web service that
             the Collector app will connect to it soon in order to negotiate the initial password




19.02.2021                EN-INST-A+W Infrastructure License Statistics Collector.docx         11
               for the exchange of data. The enabling is valid for one day from the time at which
               you have clicked the button. 5




5   If the initial password exchange is not done during this time, the web service will decline the requests until the
    password exchange has been enabled again via the License Collector Web Tool. Similarly, the initial password
    exchange is declined if it has already been completed successfully. In this case too, it can be enabled again with
    the web tool.



19.02.2021                     EN-INST-A+W Infrastructure License Statistics Collector.docx                        12
             After enabling of the initial password exchange, you will receive an appropriate
             message. Confirm the message with a click on the 'OK' button and close the
             browser window.




1.5 Directory structure
    -   The Collector app installs itself in the folder C:\Program Files (x86)\A+W\Sandpiper1\Licens-
        eStatisticsCollector1
    -   The Collector app creates a new folder under C:\ProgramData\A+W. The folder is called 'Sta-
        tisticsCollector' and includes a file 'LocalSettings.dat' or 'LocalSettings.bin.' This file contains
        the current settings for the Collector app. Since this also includes passwords, the file is enc-
        rypted.




19.02.2021                 EN-INST-A+W Infrastructure License Statistics Collector.docx                  13
1.6 Result of the installation
If the Collector app was installed correctly, there is a new planned task in the Windows
task planner.
With Windows systems with Windows Server 2012 or higher, you can start the task
planner directly from the 'Tools' menu of the server manager. The menu entry is called
'Task Scheduler.'




You can find the newly planned task in the 'A+W' folder. In the middle portion of the
display, you can also see when the next execution is planned.
If the planned task is not present after the installation, please execute the 'A+W Infra-
structure 6 License Statistics Collector Config Tool' from the 'Config Tools' folder of
the A+W Start menu. After you have run through the Config tool, the planned task is
present.


1.7 Configuration
You have no opportunity to make configuration settings for the Collector app. All con-
figuration settings are controlled centrally by A+W and transferred in the course of
regular data exchange with A+W to the Collector app at the customer's.



19.02.2021             EN-INST-A+W Infrastructure License Statistics Collector.docx    14
Insofar as the customer has objected to its participation in the license usage data
collection, the transfer of data by A+W via the same mechanism is switched off. The
Collector app then stops all communication with A+W. However, the planned task is
still there, but in this case the program always exits immediately after the start.
If you are commissioned to reactivate the Collector app at a customer who has ob-
jected to participation, please execute the 'A+W Infrastructure 6 License Statistics
Collector Config Tool' and then enable the initial password exchange as described in
chapter 1.4, point 4.


1.8 Uninstalling
The Collector app has a functionality that allows A+W to exchange the app itself. This
happens in the course of normal data exchange. 6 Therefore, it is possible that the
binary data on a customer's system is no longer the files that were originally installed.
If there should be an update of the Collector app, it is recommended that you first
uninstall it completely. 7
To uninstall, proceed as follows:
    1. Open the task planner (see 1.6) and delete the planned task for the Collector
       app
    2. From the System Control, open 'Programs' and uninstall the 'A+W Infrastruc-
       ture 6 License Statistics Collector.'
    3. Delete the folder C:\Program Files (x86)\A+W\Sandpiper1\LicenseStatis-
       ticsCollector and all of its contents, insofar as it has not been removed com-
       pletely by the uninstallation.1
    4. Delete the folder C:\ProgramData\A+W\StatisticsCollector and all of its con-
       tents.
After executing this step, the Collector app has been removed completely from your
computer.
Please note that in case of a new installation, even in the course of an update, that
you must enable the initial password exchange again (see 1.4, point 4).




6 The exchange is necessary in order to be able to react quickly to change in legal regulation or to legal provisions
  in countries that were previously not supplied.
7 Normally the Collector app is updated via the integrated update mechanism. Therefore, after the first published

  versions, no new versions will be published as set-ups in the foreseeable future. For an update of other A+W
  modules, you don't have to count on the fact that there is also an update for the Collector app. If there should
  be a new set-up for the Collector app, the Development department will inform you of this in a conspicuous
  manner.



19.02.2021                    EN-INST-A+W Infrastructure License Statistics Collector.docx                        15
2 Update
The following installation description only describes the points that differ from the full
installation described above and that must be heeded for an update.


2.1 Overview
Normally, A+W does not publish any new set-ups for the Collector app. The Collector app is
equipped with a mechanism with which it updates itself as necessary. An update of the Col-
lector app with a new set-up therefore seldom occurs. If you have to perform such an update
at all, it will be a rare occurrence.



2.2 Time requirement
If all requirements are checked and fulfilled, the following times are required for the
installation and the conversion of the existing data:


2.2.1 Installation time for the software
The update process takes about 25 minutes on the reference device due to the re-
quired uninstallation.


2.3 Requirements
New installation


2.4 Procedure
        1. Uninstall the program (see 1.8)

        2. Perform a complete new installation (see 1.4)



2.5 Directory structure
New installation


2.6 Settings
Due to the complete uninstallation, no settings are taken over. However, there are
also no settings that you have to make. You must only enable the initial password
exchange once again (see 1.4, point 4).


19.02.2021               EN-INST-A+W Infrastructure License Statistics Collector.docx    16
2.7 Result of the installation
See new installation.


2.8 Configuration
See new installation.




19.02.2021              EN-INST-A+W Infrastructure License Statistics Collector.docx   17
3 Appendix: Explanations for the Collector app

3.1 Task and data transmitted
The Collector app handles the transmission of data about the use of A+W products to
A+W headquarters in Pohlheim. The data transmitted is collected during operation by
the 'A+W Infrastructure License Protocol Service'; it is a component of the 'A+W In-
frastructure' diskset.
The data transmitted is acquired from the raw data of the detailed license usage by
totaling up over the course of one day. The data contains no user assignments, so
that it is guaranteed that no personal data is transmitted. The data that is transmitted
can also be displayed on the Infrastructure Web. For this, the 'A+W Infrastructure
Web' diskset must be installed on one of the customer's servers. The Infrastructure
Web app can then be opened at 'http://<serverurl>/Infrastructure.Web', whereby
<serverurl> is the URL of the computer on which the 'A+W Infrastructure Web' is in-
stalled.
In the Infrastructure Web app, that license usage information that is also transmitted
to A+W is displayed with the 'License' element.
There are two evaluations (total usage and parallel usage) that are displayed in the
Infrastructure Web on two separate pages. Both statistics are transmitted to A+W.


3.2 Security
All data transmission between the Collector app and A+W is done using encrypted connec-
tions. The web service is addressed via the 'HTTPS' protocol, so that the Secure Socket Layer
(SSL) is used. For the web service and the Statistics Collector Web Tool, Web hosting certif-
icates from Comodo Secure are used; it is an official certification office. Therefore, no instal-
lation of certificates on the customer system is required.
So that no falsified data can be transmitted to the customer's detriment, the Collector app
must use a password that only it knows before the web service accepts data or transmits
settings. Each installation has its own password, which is negotiated during the initial pass-
word exchange and is then exchanged at regular intervals. The password is known only to
the Collector app. The WebService can verify the password using the information saved at
A+W. However, the information does not allow determination of the password through reverse
engineering.
During the initial password exchange, the license server's security system is used for authen-
tication, so that the identity of the requesting customer can be guaranteed.
The usage data is received by the web service and - after a short pause - transmitted to a
database that is located within the secured boundaries of the A+W network. It does not remain
on the web server. The further processing of the data is done exclusively within the bounda-
ries of the secured A+W network.



19.02.2021               EN-INST-A+W Infrastructure License Statistics Collector.docx          18
All customer-side binary data that belongs to the Collector app is provided with valid Authen-
ticode signatures so that its authenticity can be checked.



3.3 Mode of operation
The Collector app connects to an A+W web service at regular intervals.
At times configured by A+W, the Collector app transmits the summarized usage data
to the web service. The data is then transported further into a database that is within
the closed A+W network.
The times at which a transmission occurs and the address of the web service with
which the Collector app communicates are queried from the web service by the Col-
lector app. The times and intervals are specified by A+W so that - even taking into
consideration how the customer works - as even a receipt of data as possible is
achieved. For the customer, the advantage is that the transfer takes place quickly and
any compromising of the customer's system is reduced to a minimum. The time and
interval can change dynamically.
The address of the web service with which the Collector app communicates can also
be changed for the transfer of configuration data. This way, A+W can react dynami-
cally to changing data quantities by setting up additional web servers to receive the
data.
In the end, in the course of transmitting settings, components of the Collector app
itself can also be exchanged. The point of this is to be able to make quick changes to
new legal situations and eliminate critical errors quickly. The authenticity of the com-
ponents exchanged will be guaranteed by their digital signatures (Authenticode).




19.02.2021              EN-INST-A+W Infrastructure License Statistics Collector.docx        19

