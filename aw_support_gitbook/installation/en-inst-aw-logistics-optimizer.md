---
description: "EN INST A+W Logistics Optimizer"
---



# EN INST A+W Logistics Optimizer

          Installation Instructions

          A+W Logistics Optimizer
   Change history:
     Date            Edited by               Remarks                                   Version
     2013-10-01      PK                      Original version                          1.0
     2014-01-10      DLA                     New Version                               1.1
     2014-09-02      JL                      New Functions                             1.1.1
     2015-02-05      JL                      New Version                               1.2
     2016-02-26      D.Langsdorf             Database directory                        13.0.0
     2016-04-06      B. Michel               Last change Version 6                     13.0.1
     2016-07-27      DLA                     DB update and adjustments                 13.1.0
     2017-12-15      DLA                     DBUpdate tool on DB server                13.4.0




     The installation instructions will assist the planner with the installation and
     configuration process for the software named. Please proceed in the following
     sequence:


     1.      Check the installation requirements.

     2.      Compile the required data, additional programs, drivers, etc.

     3.      Note or determine the time required.




19.02.2021                          EN-INST-A+W Logistics Optimizer.docx                1
Content



   Installation Instructions .................................................................... 1

   A+W Logistics Optimizer .................................................................. 1

   1         Installation .............................................................................. 3
   1.1       Database ...................................................................................................3
   1.1.1     Database Creation.....................................................................................3
   1.2       Create ODBC Source ................................................................................4
   1.3       SetupLauncher ..........................................................................................4
   1.3.1     Database Update ......................................................................................6

   2         Configuration .......................................................................... 8
   2.1       A+W Business 5 + Pro ..............................................................................8
   2.2       A+W Logistics Optimizer database connectin .........................................10
   2.3       ERP interface ..........................................................................................11
   2.4       Licensing the A+W Logistics Optimizer ...................................................12
   2.5       Internet Explorer ......................................................................................14
   2.5.1     Compatibility with Internet Explorer 10 ....................................................16




19.02.2021                              EN-INST-A+W Logistics Optimizer.docx                                            2
1 Installation
The following installation instructions assume that there is no previous version
installed. Setup and additional configuration options are described in the
Configuration Documentation.

1.1 Database
Before starting installation, a database has to be created for the Logistic Optimizer in
SQLServer.
1.1.1 Database Creation
The Restore function in the SQLServer Management Studio has to be used for
creating the database. The backup file OTR.BAK has to be restored.
This is located in the following folder.
…\Diskset\A+W Logistics Optimizer\DB\OTR.BAK




Another way to create the database is to do it manually and then to execute each of
the files in the [.\Scripts\SYSDAM.OTR_*.SQL] folder. These create the database.
The scripts are located at
…\Diskset\A+W Logistics Optimizer\DB\Scripts




19.02.2021                     EN-INST-A+W Logistics Optimizer.docx                    3
1.2 Create ODBC Source
A 32 bit system ODBC Source has to be created on the OTR database so that reports
can also be printed from the OTR. For this purpose, use the ODBC Administrator
under
"C:\Windows\SysWOW64\odbcad32.exe". The name of the ODBC connection has to
be "OTRcr".




1.3 SetupLauncher
A+W Logistics Optimizer is contained in the A+W Setup Launcher.




The following dialogs appear during the installation process


19.02.2021                   EN-INST-A+W Logistics Optimizer.docx               4
After installation, A+W Logistics Optimizer must be found under Programs and
Features.




19.02.2021                EN-INST-A+W Logistics Optimizer.docx             5
1.3.1 Database Update
After the installation or after an update the database must be brought up-to-date. The
OTR DB Updater is used for this purpose. This tool can be found in the installation
directory:                                                         Ort.DbInstaller.EXE




Warning: OTR DB Updater must run on a server on which a SQLServer or its
components are installed, since the tool uses these. Either install OTR
completely on a DB server or copy the OTR directory from ProzessServer to DB
Server.


Both the database connection to OTR database and the path to the database update
scripts must be selected. This is the sub-directory „Databases“.




19.02.2021                   EN-INST-A+W Logistics Optimizer.docx                    6
19.02.2021   EN-INST-A+W Logistics Optimizer.docx   7
2 Configuration
From A+W Business 6 on, the OTR is connected over the A+W Commercial Logistic
Service. Therefore, point 2.1 is not necessary any longer, since OTR is not directly
connected to the ERP database, anymore. You must read the service's Installation
Manual thoroughly, in order to completely commission the integration. The integration
in A+W Business 6 is not part of this Installation Manual.

2.1 A+W Business 5 + Pro
Using customizing, an additional button has to be integrated so that the OTR software
can be called from AWB5. To do this, you have to create 2 formulas. One formula
describes the button (BUTTON OTR) while the other one describes the function that
is assigned to the button (EXECUTE OTR).
To do this, you open "Masterdata/Company/Formulas" in AWB and insert the 2 new
formulas.




The formula content can be taken from the "Customizing_alfak.txt" file. The formula
numbers (here 20000 and 20001) should stay as these values. If existing formulas
have already been assigned these numbers, other values can be used. Here, it must
be ensured that the reference made in the first formula to the second formula,
(Execute OTR), is entered correctly.
Additionally, it must be ensured that the path to the OTR software that is included in
the 2nd formula, is also entered correctly.
Then the button has to be integrated in such a way that it appears when called by the
Number Manager. To do this, you open the Number Manager under
"Documents/Order/NM order":




19.02.2021                   EN-INST-A+W Logistics Optimizer.docx                    8
 By right-clicking on the upper window bar, you open a menu where you can assign
the button to the Number Manager:




19.02.2021                 EN-INST-A+W Logistics Optimizer.docx                9
Following a restart of A+W Business the new button should now be visible in the Menu
Bar        once          the      Number          Manager         is         opened:




2.2 A+W Logistics Optimizer database connectin
The OTR database and if necessary the OTR archive database have to be entered
the first time the A+W Logistics Optimizer is executed. From version 6, the tab "ERP
Connection" is no longer configured.
Please note: These settings have to be made for each Windows user.




19.02.2021                   EN-INST-A+W Logistics Optimizer.docx                 10
If A+W Business 5 is used, the connection to ERP database must be configured
additionally.




2.3 ERP interface
From A+W Business 6, the switch AW_ERP_INTERFACE must be set in A+W
Logistics Optimizer, so that OTR communicates with the A+W Commercial Logistic
Service. After that, the program must be restarted.




19.02.2021                 EN-INST-A+W Logistics Optimizer.docx             11
2.4 Licensing the A+W Logistics Optimizer




If you see the message "Invalid map service license" in the A+W Logistics Optimizer
status line, you have to click on the [Next] button.




19.02.2021                  EN-INST-A+W Logistics Optimizer.docx                 12
The following steps have to be carried out, in order to get a new licence:
The installed system has a license that is valid for 5 days.
Click on the Start TAB  About OTR




The following dialog appears when you click on [Temporal license] button:




19.02.2021                    EN-INST-A+W Logistics Optimizer.docx           13
Completing the information and clicking on the [OK] button creates a temporary
license that is valid for 5 days.




When the license has been issued, the About OTR dialog looks like:




If you have with a problem with the online license creation, please send an e-mail to
jordi.luque@a-w.com.

2.5 Internet Explorer
Internet Explorer 10 or higher must be installed to be able to work with the A+W
Logistics Optimizer. There are security issues with Internet Explorer in some
instances.
This is not shown after the installation of the map license:




19.02.2021                    EN-INST-A+W Logistics Optimizer.docx                 14
Enter the following URLs in the Internet Explorer Security Settings as Trusted Sites:
        https://otrservice.onerbox.com
        https://js.cit.api.here.com
        https://1.base.maps.api.here.com
        about:security_Ort.App.exe
 It is absolutely imperative that the URL "about:security_Ort.App.exe" is included and
that HTTPS:// is deactivated.




The following messages can appear when calling the maps through Nokia Maps:




19.02.2021                   EN-INST-A+W Logistics Optimizer.docx                   15
If you ignore them, everything should work as normal. The OTR APP has to be
designated as trustworthy if you want to switch the message off.
2.5.1 Compatibility with Internet Explorer 10
As was stated previously, the installation of Internet Explorer 10 is an absolute
minimum requirement. With newer versions of Internet Explorers, the compatibility to
IE10 has to be set up.
The following key has to be entered in the Registry, in order to be able to work with
IE 10 compatibility.
The Registry Key is automatically inserted during installation. If it has not been
created, it has to be inserted manually:
Windows 64 Bits
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Internet
Explorer\Main\FeatureControl\FEATURE_BROWSER_EMULATION
Ort.App.exe 2711 (DWORD)

Windows 32 Bits
HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Internet
Explorer\MAIN\FeatureControl\FEATURE_BROWSER_EMULATION
Ort.App.exe 2711 (DWORD)




19.02.2021                   EN-INST-A+W Logistics Optimizer.docx                  16

