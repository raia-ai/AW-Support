---
description: "EN INST A+W Realtime Optimizer"
---



# EN INST A+W Realtime Optimizer

         Installation instructions for test
         purposes


A+W Realtime Optimizer




                                                                          English




   A+W Software GmbH   EN-INSTALL Develop- A+W Realtime Optimizer.docx    1


                                                                  - INTERNAL -
Content


1.   Prerequisite                                                          3
2.   Provision of the test database                                        4
     2.1. Importing the test database                                      4
     2.2. Creating admin users for the database                            6
     2.3. Creating the ODBC connection                                     7
3.   Installation & configuration via the Setup Launcher                   10
     3.1. AWServices user for the services                                 10
     3.2. Preparing the Setup Launcher                                     10
     3.3. Installation with the Setup Launcher                             11
     3.4. Configuration via the Setup Launcher                             15
          3.4.1. License client configuration                              15
          3.4.2. CAD Designer (Shapes) Config Tool                         15
          3.4.3. Shaping&Nesting Picture Service config                    17
          3.4.4. CAD Designer (Bars) Interface Service config              18
          3.4.5. Production config                                         18
          3.4.6. Plan Editor config                                        18
          3.4.7. Production PPSWebService config                           19
          3.4.8. Infrastructure config                                     20
          3.4.9. Conclusion                                                20
4.   Configuration of the Realtime Optimizer                               22
     4.1. Provision of the test save files                                 22
     4.2. Set-up of the user directory                                     22
     4.3. Configuring XTV on half a screen                                 22




A+W Software GmbH        EN-INSTALL Develop- A+W Realtime Optimizer.docx        2
1. Prerequisite
The installation is done on a development environment that is approved by the R&D Department -
- Architecture & Core. The development environment must be at least the 2015 version or higher.
The SQL Server in the environment must be Version 13 or higher.
If another environment than the A+W development environment is used, it can happen that steps
in addition to the ones described here are necessary, because, for example, the AWSOA database
is not yet pre-installed of the user awservices is not yet set up.




A+W Software GmbH        EN-INSTALL Develop- A+W Realtime Optimizer.docx                     3
2. Provision of the test database
2.1. Importing the test database
To import the test database, take the following steps:
    •   Start the Microsoft SQL Server Management Studio
    •   Connect to the SQL Server
    •   Identify the storage location of the local databases with the following steps:
            o   Right-click on Database in the Management Studio Server, then on Attach...




                Figure 2-1 Importing database via the MS SQL Server Management Studio




A+W Software GmbH          EN-INSTALL Develop- A+W Realtime Optimizer.docx                   4
           o   so that the Attach Databases window opens. Click the [Add] button here




               Figure 2-2 Linking database to the server

           o   so that the Locate Database Files window opens. Copy the path for Database
               Data File location: to the clipboard.




               Figure 2-3 Identifying storage location for the databases and selecting the database to link it with
               the server

   •   Open this folder for preparation in the File Explorer.
   •   Go to a new window of the File Explorer.
       \\jupiter\TECHSOFT_Develop\RTO_Template\Database and copy the database RTO13.ZIP
       or RTO14.ZIP locally to the machine in the folder that was opened for preparation. If a
       SQL Server 13 is installed in the development environment, use RTO13.ZIP; with SQL
       Server 14, use RTO14.ZIP. Unfortunately, older versions are not supported here.




A+W Software GmbH          EN-INSTALL Develop- A+W Realtime Optimizer.docx                                            5
    •   Unpack the database in the folder and attach the test database to the server. See Figure
        2-1, Figure 2-2 and Figure 2-3; in the end, the unpacked database must be selected and
        confirmed with [OK].


2.2. Creating admin users for the database
To create a strong user, you must take the following steps:
    •   Im MS SQL Server Management Studio, go to Security > Login > New Login…




        Figure 2-4 Creating a new login

    •   Under General, create the new Login Name alcimdb with the same password Remove
        the checkmark next to Enforce password policy.




        Figure 2-5 Creating a new database user -- General tab




A+W Software GmbH            EN-INSTALL Develop- A+W Realtime Optimizer.docx                  6
   •   On the Server Roles tab, set the checkmark by sysadmin and leave the checkmark
       by public.




       Figure 2-5 Creating a new database user -- General tab

   •   Confirm with a click on [OK].


2.3. Creating the ODBC connection
   •   Open ODBC 32bit and go to the System DSN tab and click [Add…].




       Figure 2-7 Creating the new ODBC connection

   •   Select SQL Server Native Client 11.0 and click [Finish].




A+W Software GmbH           EN-INSTALL Develop- A+W Realtime Optimizer.docx             7
       Figure 2-8 Selection of the ODBC driver

   •   On the new window Name: enter the RTO and Description: RTO. For Server select the local
       server that you also see in the MS SQL Management Studio.




       Figure 2-9 Reading off the local server in MS SQL Management Studio




       Figure 2-10 Selecting the local server in the ODBC Data Source Administrator

   •   Click [Next >].
   •   Activate the SQL Server authentication and enter the previously created admin user
       alcimdb.




A+W Software GmbH            EN-INSTALL Develop- A+W Realtime Optimizer.docx                 8
       Figure 2-11 Entering login for the new ODBC connection

   •   Click [Next >].
   •   Set the checkmark by Change the default database to and select the RTO database.




       Figure 2-12 Defining the default database

   •   Click [Next >], then click [Test Datasource].
   •   Keep clicking on [Next >] and [Finish] until the setup is completed.




A+W Software GmbH           EN-INSTALL Develop- A+W Realtime Optimizer.docx               9
3. Installation & configuration via the Setup
   Launcher
3.1. AWServices user for the services
During the installation, the user awservices is required, which should be created on all
development environments. To check this, take the following steps:
    •    Open Computer Management
    •    Under Local Users and Groups > Users, check whether the user awservices already exists.




Figure 3-1 Checking the user via the Computer Management



3.2. Preparing the Setup Launcher
For the installation of the A+W Realtime Optimizer with the Setup Launcher, it must first be
installed and set up. The following steps are required for this:
    •    Go to \\jupiter\SW_Develop\v13.0\SetupLauncher and install the Setup Launcher with a
         double-click on setup.exe
    •    After the installation, an A+W folder is created on the desktop; it contains the Setup
         Launcher. Go to \\jupiter\TECHSOFT_Develop\RTO_Template\Install and           copy the
         special RTO-Ini      for the Setup     Launcher to
         %programdata%\A+W\SetupLauncher




Figure 3-2 Copying RTO diskset ini for the Setup Launcher




A+W Software GmbH              EN-INSTALL Develop- A+W Realtime Optimizer.docx                 10
3.3. Installation with the Setup Launcher
To install an A+W Realtime Optimizer in the development environment for test purposes, take the
following steps:
   •   Start the A+W Setup Launcher via the A+W folder on the desktop, select [Open Diskset...],
       and then click [Next].
   •   Select the RTOInstallation.diskset. Then select the desired installation folder on Jupiter,
       for example \\Jupiter\SW_Develop\vNext\Diskset




   •   Click [Next], then select the A+W Realtime Optimizer. Now, all other dependent setups
       (e.g. A+W Production Shared Folders, XStockMaster) are also selected automatically.
   •   Click [Next] and select the Trans drive or create it anew. To do this, click the folder symbol
       to the right next to Server Directory, select the C drive, and click [Make New Folder]. Call
       the folder TRANS. Then right-click on the new folder right away and check > Properties >
       Edit > Permissions for User Full control as shown in Figure 3-4. Confirm everything with
       [OK].




A+W Software GmbH        EN-INSTALL Develop- A+W Realtime Optimizer.docx                             11
Figure 3-3 Creating the Trans drive




Figure 3-4 Setting up full access rights for the Trans drive

     •    For Server, enter Volume P: so that the screen looks like this:




A+W Software GmbH                EN-INSTALL Develop- A+W Realtime Optimizer.docx   12
Figure 3-5 Setting up Production transfer directory in the Setup Launcher

    •    Click [Next]. Check the database connection displayed now and click [Next] again.
    •    Enter the local computer name for the infrastructure configuration. The checkbox by
         Activate Distributed Services must be checked.




A+W Software GmbH               EN-INSTALL Develop- A+W Realtime Optimizer.docx                13
Figure 3-6 Infrastructure configuration in the Setup Launcher

    •    Click [Next].
    •    As soon as there is a query for a service user in the Setup Launcher, enter the user you
         looked up in section 3.1.
    •    Select the Install Software bullet point and confirm with [OK].
    •    When all installations have been run through, the configuration starts. It can happen here
         that individual configuration screens open in the background and must be focused
         manually.




A+W Software GmbH              EN-INSTALL Develop- A+W Realtime Optimizer.docx                  14
3.4. Configuration via the Setup Launcher
During configuration in the Setup Launcher, depending on the condition of the development
environment, the following configurations may be required:


3.4.1. License client configuration
Enter the licenseserver in the free text field and click [Test] if you have access to the license server
in Pohlheim (see Figure 3-7). With a successful test, confirm with [OK] and click [Next]. Keep
clicking [Next] until this button is grayed out, then click [Finish].
Figure 3-7 Configuration of the license client




3.4.2. CAD Designer (Shapes) Config Tool
First click [Start from default values], then go to [Next]. Keep clicking [Next] until this button is
grayed out, then click [Finish].




A+W Software GmbH                EN-INSTALL Develop- A+W Realtime Optimizer.docx                        15
Figure 3-8 Configuration CAD Designer (Shapes)




A+W Software GmbH             EN-INSTALL Develop- A+W Realtime Optimizer.docx   16
3.4.3. Shaping&Nesting Picture Service config




Figure 3-9 Shaping&Nesting Picture Service config

    •    Take steps 1-4 from Figure 3-9; for step 3, select the local computer.
Figure 3-10 Selecting awservices user and checking the name




    •    Then enter awservices in the free text field and click [Check Names]. As soon as the user is
         recognized, confirm with [OK].



A+W Software GmbH              EN-INSTALL Develop- A+W Realtime Optimizer.docx                    17
    •    Enter the password for the user awservices (P0hlhe1m) and click [Next]. Then various
         settings are checked, the CAD Designer starts briefly, etc. Then click [Finish].


3.4.4. CAD Designer (Bars) Interface Service config
The configuration is taken over from the previously set up Shaping&Nesting Picture Service config.
So just click [Next] here and then click [Finish].


3.4.5. Production config
Here the database connection for the RTO must be entered, just as in this figure:
Figure 3-11 Production config




Then test the connection with a click on [Test Connection]. Keep clicking [Next] and finish with
[Finish].


3.4.6. Plan Editor config
Select a folder for the Block.pth files here. Normally, the folder is the SN folder on the Trans drive.
If the folder does not exist yet, it must be created. With a click on [...] you can select the folder or
create it anew right away. Click [Next]. Then simultaneously




A+W Software GmbH               EN-INSTALL Develop- A+W Realtime Optimizer.docx                      18
there is a check whether this folder exists and is accessible. After a successful check, the entry
Create file Block.pth | Set path of Block-File to xxxx | Success appears at the bottom. Then click




[Next].
Figure 3-12 Plan Editor config


3.4.7. Production PPSWebService config
Enter a point in the domain (see Figure 3-13), select the user as explained in detail in section
3.4.3. Keep clicking [Next] until this button is grayed out, then click [Finish].




A+W Software GmbH                EN-INSTALL Develop- A+W Realtime Optimizer.docx                     19
Figure 3-13 Configuration of the PPS WebService


3.4.8. Infrastructure config
Enter the database connection as in section 3.4.5 again. Test the connection to the FTP server
with a click on [Test]. Keep clicking [Next] until this button is grayed out. Then click [Finish].



3.4.9. Conclusion
When all configuration steps have been completed successfully and the Setup Launcher looks as
in Figure 3-14, click [End].




A+W Software GmbH             EN-INSTALL Develop- A+W Realtime Optimizer.docx                  20
Figure 3-14 Completing configuration with the Setup Launcher




A+W Software GmbH             EN-INSTALL Develop- A+W Realtime Optimizer.docx   21
4. System configuration for the Realtime
   Optimizer
The first start of the A+W Realtime Optimizer must absolutely be done with the A+W folder on the
desktop, since only then will important files be copied into the appropriate user directory.
If there is a query for the station ID, enter a 2-digit number.


4.1. Provision of the test save files
The previously created Trans drive P:\ is used for the zipped optimization files (so-called save
files), which are formed by the work preparation or a table optimization. In order to be able to use
special test save files, which also fit the previously attached database, take the following steps:
     •   Copy the content of \\jupiter\TECHSOFT_Develop\RTO_Template\LW_P\Release\Save to
         the local folder P:\Release\Save.
     •   Unpack all files directly in the Save folder. All save files must be directly in this folder and
         may not be in a subfolder.
     •   Keep the original Zip file so that after tests during which these save files are changed, you
         can reset the environment to its original condition.


4.2. Set-up of the user directory
In order to set up the user directory for test purposes, take the following steps:
    •    Copy the content of \\jupiter\TECHSOFT_Develop\RTO_Template\$USER$\Xopton to the
         local folder %AppData%\A+W\Techsoft\Xopton.
    •    Copy the content of \\jupiter\TECHSOFT_Develop\RTO_Template\$USER$\Panorama to
         the local folder %AppData%\A+W\Techsoft\Panorama.


4.3. Configuring XTV on half a screen
If you are working with a monitor on the test system, it is difficult if the XTV opens across the
whole screen and pushes itself into the foreground. For this case, it is possible to configure the
XTV such that it only opens on half the screen. The following steps are required for this:
    •    Open the registry.
    •    Navigate to HKEY_CURRENT_USER\Software\Albat+Wirsam\PlanEdit\Global.
    •    Set the parameter MultiMonitorSystem to 1.
    •    So that the parameter takes effect, the Realtime Optimizer must be restarted.




A+W Software GmbH          EN-INSTALL Develop- A+W Realtime Optimizer.docx                             22
Figure 4-1 Registry entry with which the XTV starts on only half the screen.



4.4. Creating environment variables
The environment variables AlcimOther and AlcimReg must be created. To check this and to create
the missing environment variables, the following steps are required:
     •    Open the command line.
     •    Enter Set a and confirm with <Enter>.
     •    If everything looks as in Figure 4-2, you don't have to do anything else.




Figure 4-2 Necessary environment variables for the Realtime Optimizer

If the environment variables are missing, the following steps are required:
     •    Open the Control Panel and navigate to System and Security > System.
     •    Click Advanced system settings.




A+W Software GmbH               EN-INSTALL Develop- A+W Realtime Optimizer.docx             23
Figure 4-3 Advanced System Settings on the Control Panel

    •    Take all steps as described in Figure 4-4. As variable value, enter the path
         \\jupiter\TECHSOFT_Develop\Alcim\AlcimOther.




Figure 4-4 Creating the environment variable AlcimOther

    •    Then create the environment variable AlcimReg with value noreg, as depicted in Figure 4-
         5.




Figure 4-5 Creating the environment variable AlcimReg

    •    Confirm everything with [OK].




A+W Software GmbH             EN-INSTALL Develop- A+W Realtime Optimizer.docx                  24
5. Building the source code
In order to build the sources of the A+W Realtime Optimizer for the first time and to be able to
debug the A+W Realtime Optimizer, the following steps are required:
    •    Start the Visual Studio as administrator
    •    In the Source Control Explorer, navigate to GlassSuite > Production > Dev > Alcim. The
         source code of the A+W Realtime Optimizer is in the folders ALCIM > XOPTON and
         ALCIM_SHARED, whereby the main folder here is ALCIM > XOPTON.
    •    Do a Get Latest Version on the folders ALCIM and ALCIM_SHARED.
    •    In the folder ALCIM > XOPTON, open the solution Xopton_AllProjects.sln, do not update it.




Figure 5-1 Opening the solution Xopton_AllProjects.sln




Figure 5-2 Do not update the RTO sources




A+W Software GmbH              EN-INSTALL Develop- A+W Realtime Optimizer.docx                     25
     •    In Visual Studio, select the menu Build > Batch Build..., set all checkmarks and click
          [Rebuild].




Figure 5-3 Executing batch build in the RTO

     •    If necessary, also click [Overwrite].
     •    If in the end you have built more than 30 projects, everything is fine




Figure 5-4 Result of the batch build in the RTO

     •    In the folder Dev > ALCIM > Xopton, execute the batch file GetRTO_VNextEnv.bat as
          administrator. This way, the appropriate DLLs are drawn from the Setup.




Figure 5-5 Executing GetRTO_VNextEnv.bat

     •    Start RTO debugging and enjoy


A+W Software GmbH               EN-INSTALL Develop- A+W Realtime Optimizer.docx                    26
5.1. Troubleshooting: RTO does not have a license
If the license server is accessible from the computer, but you see a message when starting the
RTO that there is no license, you can solve this problem with the following steps:
    •   Is the client service running? No: start manually.
    •   Does the service end directly after a manual start? Yes: reinstall the license client
    •   Trick 17: manually end all SOA services, then start the license client and then restart the
        SOA services. The SOA services include Infrastructure, Planning, and CIM.




A+W Software GmbH         EN-INSTALL Develop- A+W Realtime Optimizer.docx                        27

