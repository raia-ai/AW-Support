---
title: "EN INST A+W Customizing Manager"
category: "installation"
product: "A+W Customizing Manager"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Customizing Manager"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation Instructions             A+W Customizing Manager    Change history:       Date              Edited by                  Remarks      2018-09           DLA                        First draft      2018-10           DLA                        Second draft     This document enables the competent reader to install the described software. You should generally stick to this procedure:       1.     Check the installation requirements.      2.     Compile the required data, additio"
source_file: "EN-INST-A+W Customizing Manager.pdf"
---


# EN INST A+W Customizing Manager

           Installation Instructions

           A+W Customizing Manager
   Change history:

     Date              Edited by                  Remarks
     2018-09           DLA                        First draft
     2018-10           DLA                        Second draft




This document enables the competent reader to install the described software.
You should generally stick to this procedure:


    1.     Check the installation requirements.

    2.     Compile the required data, additional programs, drivers, etc.

    3.     Note or determine the time required.




22-08-16                               EN-INST-A+W Customizing Manager.docx     1
Content




   Installation Instructions ............................................................................. 1

   A+W Customizing Manger .......................................................................... 1

   1         Introduction ................................................................................... 3

   2         Prerequisites .................................................................................. 4

   3         Installation ..................................................................................... 5
   3.1       First start ..............................................................................................................5
   3.2       Configuration ........................................................................................................6
   3.2.1     Restrictions ...........................................................................................................6
   3.3       Registries ..............................................................................................................7

   4         How it works .................................................................................. 8
   4.1       Configure Master Data .........................................................................................8
   4.2       Configure Objects ...............................................................................................11
   4.3       Publish Objects ...................................................................................................16

   5         DB2 and Informix .......................................................................... 19




22-08-16                                  EN-INST-A+W Customizing Manager.docx                                                        2
1 Introduction
The A+W CustomizingManager support the management of customizing, like Reports, scripts,
configuration files, for a customer. It will be helpful for a company who handle the management by
himself, e.g. a company who create their own reports. The size of the company doesn’t matter, but
A+W CustomizingManager support the handling of customizing in different sites.
The A+W CustomizingManager has to run once on a central place in the company. The tool is not
made for multi user work and has no right system. The user who is allowed to login at the A+W
CustomizingManager database has access to all functions and objects stored in the application.
The A+W CustomizingManager has his one database, actual only INFORMIX. The database user login
will be the user of this tool. This user is also used in the history protocol. So if you have different
user which works with the A+W CustomizingManager (not parallel!), use different database logins to
see in history who has done what.
The tool is running on Windows OS.




22-08-16                          EN-INST-A+W Customizing Manager.docx                               3
2 Prerequisites
Install the IBM.DB2 Driver Package on the system before starting the A+W Customizing Manager
setup. Currently we deliver the Version 11.1.3fp3 (v11.1.3fp3_nt32_dsdriver_ALL_LANG) as extra
package in the diskset.
If there is already an IBM.Data.Informix Driver installed on that system, you need to do some steps
manually. Only then the IBM.DB2 Driver will fully work.
    •      After the installation of the driver package, check (and add when missing) the Registry
           for the key

           HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\IBM\DB2\InstalledCopies
           -> "11.1.3030.DEF.4"="IBMDBCL1"

           The value of the key must match your “InstalledCopies” DB2 Name


    •      Check the GAC Folder C:\Windows\Microsoft.NET\assembly\GAC_32
           There should be two folders present (DLLs installed)
              o IBM.Data.DB2
              o IBM.Data.DB2.Entity
If there are not present, then you add them with an administrative Command Prompt and the
gacutil tool.


Normally it could be found in one of these folders:
    •      C:\Program Files (x86)\Microsoft SDKs\Windows\v7.0A\Bin
    •      C:\Program Files (x86)\Microsoft SDKs\Windows\v8.1A\bin\NETFX 4.5.1
           Tools
Or copy it from our Tools folder:
    •      \\jupiter\SW_install\Tools -> NETFX 4.7.2 Tools
gacutil /i "C:\Program Files (x86)\IBM\IBM DATA SERVER DRIVER\bin\netf40\IBM.Data.DB2.dll"
gacutil /i "C:\Program Files (x86)\IBM\IBM DATA SERVER
DRIVER\bin\netf40\IBM.Data.DB2.Entity.dll"
The commands should return “Assembly successfully added to the cache”




22-08-16                            EN-INST-A+W Customizing Manager.docx                              4
3 Installation
The A+W Customizing Manager is installed via the A+W Setup Launcher, under section Common.
Install the tool on a central server or PC.
This central Server or PC needs network access to the different server of the different sites where
files should be exchange. By this application. For further version a database access and
corresponding database driver to different environment also are need.
CREATE DATABASE {db name} IN {DBSPACE name} WITH BUFFERED LOG;
Don’t forget to put this database into the backup jobs!

3.1 First start
After start, the database login information must be entered.




If the database connection works, the application checks its database version and update
the table structure if needed. On this reason, the database user must have the right to
change the database structure.
If you want to work with different users (not at the same time, the tool isn’t made for multi
user access), you need different database logins. The last login will be stored for each
windows user.


22-08-16                          EN-INST-A+W Customizing Manager.docx                                5
The database owner represents the user that is responsible to create the structure of the
database. All the tables must be accessed using this user as schema.
The database owner is set as default with the user that logged in for the first time in the
application, but it can be modified manually after that from the configuration tab.

3.2 Configuration
Open the tab Configuration:




The settings for trace level, entity framework trace level and language are stored for each windows
user and PC/server. To apply the changes, the application must be restarted.
The trace level represents the application logs that are saved in the logging file.
The entity framework trace level represents the level on which the scripts executed by entity
framework will be logged by the logging mechanism.
The settings in the list on the right side are global parameter which are stored in the database:
If all requirements are checked and fulfilled, the following times are required for the installation and
the conversion of the existing data:

    •      Object Output path
           The base path which is suggested if an object should be exported into a file
3.2.1 Restrictions
When creating SQL objects (stored procedure, function or view) the object name needs to be the
same as SQL object in the database.
An object for stored procedure “cu_sealingtype” needs to be named “cu_sealingtype”.




22-08-16                           EN-INST-A+W Customizing Manager.docx                                6
The reason is the customizing manager uses this name when checking if the object exists in the
target database(s) already. It will also use this name when dropping a database object before
creating it.
If no owner is defined in the script, the owner defined in Master Data for the target database will be
used. If no owner is defined in Master Data for target database, the user logged into the A+W
Customizing Manager is used.

3.3 Registries
All A+W Customizing manager registries can be found in:
           HKEY_CURRENT_USER\Software\A+W\AUW\CustomizingManager
The registries are split in 4 sub directories: Database, DatabaseOwner, Language and Trace.
In Database folder you can find all the information needed to login into the application (login to the
Customizing manager database). The password is encrypted and can be decrypted only from the
same device on which it was stored in registry.
In Database Owner folder you can find the database owner set in the login screen, that represents
the schema on which all the tables are created. To access the information from these table you
need to know the schema. In Informix the schema corresponds with the user that created the
tables.
In Language folder you can find the value representing the default language in the application. It can
be changed in the Configuration tab.
In Trace folder you can find all the settings about the trace level set in the application. It contains a
trace level for the application, a trace level for ORM (the mechanism responsible to connect to the
database) and a trace level for view.




22-08-16                            EN-INST-A+W Customizing Manager.docx                                    7
4 How it works
This chapter describes how A+W Customizing Manager works by an example.

4.1 Configure Master Data
In Master Data you configure Sites and their Environments. An Environment is allocated one of our
A+W products: A+W Business, A+W Enterprise and A+W Production. For each environment the user
must define whether is a Live or Test Environment and a set of Parameter can be set. The Parameter
are paths to the different categories of files: Reports, Scripts and Configuration or database. The
path must be a UNC path where the Windows user has access. It is a base path, later during
configuration of objects you can defined sub folders where each file will be stored.
Open the Master Data Tab and enter a new Site A+W Germany with Site ID 1:




Add to this new Site a new A+W Production live Environment “Production Germany”:




Add to this new Environment a new Path Category Reports and define the UNC Path to the Report
Folder of this Environment. If need add Path also for other categories:




22-08-16                         EN-INST-A+W Customizing Manager.docx                             8
Now repeat these steps to add a Test Environment “Production Germany Test” and a second Site
A+W France with a Test and Live Environment:




22-08-16                        EN-INST-A+W Customizing Manager.docx                           9
For every environment you can add a database:




22-08-16                       EN-INST-A+W Customizing Manager.docx   10
For every database you have to enter the data for connection string to that specific database:




4.2 Configure Objects
In the object tab all objects will be managed which should be handled by the A+W Customizing
Manager. Actual an object is a file of one of the existing categories like Report, Configuration or
Script. In future also database objects, like Functions and Stored Procedures will be handled.
In our example we want add Report Objects for A+W Production, click on the button to add a new
object:




A file open dialog opens, navigate to the folder where the report is stored:




22-08-16                           EN-INST-A+W Customizing Manager.docx                               11
Now set the setting and save the object:
    1. Set Product to “A+W Production”.
    2. Set Category to “Report”.
    3. Filename is the name from selected file, change the name if the name at the environments
       is different to the loaded name.
    4. If the file is stored in a sub folder, enter the name of the sob folder.
    5. Add a description which describe the object. This is only to manage in the object in the A+W
       Customizing Manager.
    6. Add an information to the load file. It is preset with the filename and can be changed. This
       information is used only to manage the different files of an object in the A+W Customizing
       Manager.
    7. Assign the Sites where this object exists. In our example select both existing sites. It is
       assigned to all “A+W Production” environments in the assigned sites.




    The new object has one file which is marked as test file (file symbol with the gear) and if the
    object will be published, this file will be published into “A+W Production” test environments of
    the assigned sites.




22-08-16                          EN-INST-A+W Customizing Manager.docx                             12
    Now you want to use this file also for live environments, so release the test file. The test file will
    be copied (file symbol whit the green check mark):




    You have the possibility to delete a selected file of an object:




    …or edit the file information:




22-08-16                             EN-INST-A+W Customizing Manager.docx                               13
    …or export the content of the file into a new file into your file system:




    Now we add a draft of a new IG Production list report to this object. New files will always store
    as test file. An existing test file will be automatically moved as archived. The new test has its
    own information and version which can be changed:




22-08-16                           EN-INST-A+W Customizing Manager.docx                             14
    A selected archive or release file can be copied as Test file. If this happens the actual test file will
    be moved into archive.




    If you enter a new test file or release a test file and the selected and target file are similar, you
    get a message that this action will not be done.




    In the file list in the las column you see a file symbol. This symbol show if it file has a content or
    not. If an empty file was load, the symbol shows blank file.



22-08-16                            EN-INST-A+W Customizing Manager.docx                                    15
4.3 Publish Objects
If you have a new version of a test or live file, with the Publication tab it is possible to copy the files
to the sites.
In the first step you select the kind of environment (live or test) and the product (A+W Production,
A+W Business, A+W Enterprise) where you want to publish the new files.
In the second step you select the category type (Report, Configuration, Script) of the objects.
You get 2 lists, one with all possible Environments and one with all allocated objects. All records in
both lists are checked.




With a click on the checkbox in a list, the entry can be unchecked or checked. With the 2 buttons
below each list, all entries in the list can be unchecked or checked.
Objects which are marked in grey, aren’t allocated to all records in environment list. Objects marked
in black are allocated to all records in environment list. For this it doesn’t matter if the
environments are checked or not.
With the fields for Filename, Sub Folder and Description the object list can be filtered. This could be
helpful if a long object list exists and you want to publish only one object. The environments can be
filtered using the search site field.
If you select all environment and objects which should be published, click on Check:




22-08-16                            EN-INST-A+W Customizing Manager.docx                                  16
A+W CustomizingManager now simulates the publication and shows a list of the results that were
obtained after check:




If the list of results has no errors, you can execute the publication. For execution a description is
need:




If the publishing file is equal to the file which actual exists at the target environment, the A+W
Customizing Manager doesn’t overwrite the target file.
If the actual exiting target file doesn’t exist in the object in A+W Customizing Manager (not only the
release publishing file, also in the backup files), the target file will be backed-up as archive before it
will be overwritten.
If an object cannot be published due to the fact that the environment doesn’t have configured the
specified category, that object will be skipped. In this case the check row will have the Publish
Message “Skipped” and you will be informed in a confirmation popup how many rows were
skipped.
A message appears if the task is finished, showing how many files succeeded, failed or were
skipped:


22-08-16                            EN-INST-A+W Customizing Manager.docx                                17
The results can be exported using the Export to CSV button:




22-08-16                         EN-INST-A+W Customizing Manager.docx   18
5 DB2 and Informix
You, or the customer IT, need to define a listener for the DRDA protocol. This is done through
corresponding entries in following files:
           - $INFORMIXDIR/etc/$ONCONFIG:
DBSERVERALIASES [<other_aliases>,]<drda_ifxserver>
           - $INFORMIXSQLHOSTS:
<drda_ifxserver> drsoctcp *<server_hostname> <drda_service>
           - /etc/services:
<drda_service> <drda_portnum>/tcp
The database instance needs to be restarted to activate the newly configured listener.




22-08-16                          EN-INST-A+W Customizing Manager.docx                           19

