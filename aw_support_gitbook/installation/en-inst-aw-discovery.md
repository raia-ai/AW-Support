---
title: "EN INST A+W Discovery"
category: "installation"
product: "A+W Discovery"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Discovery"]
version: "1.0"
last_updated: "2025-12-10"
description: "Description of the Config Tool                                                      A+W Discovery  Change history   Date             Edited by                 Remarks                                                                           Version  2013-08-16 MISC                            Initial version                                                                   1.0  2013-09-10 RI                              Addition"
source_file: "EN-INST-A+W Discovery.pdf"
---


# EN INST A+W Discovery

                                  Description of the Config Tool

                                                    A+W Discovery

Change history


Date             Edited by                 Remarks                                                                           Version

2013-08-16 MISC                            Initial version                                                                   1.0

2013-09-10 RI                              Addition                                                                          1.1




Content

1.     Description......................................................................................................................... 1
       1.1. Configuring A+W Discovery ................................................................................................... 1
       1.2. Available parameters ........................................................................................................... 15
2.     Error handling.................................................................................................................. 22
       2.1. Configuration of the SQL Server services ............................................................................ 22



1. Description

       The following chapter discusses the working method of the A+W Discovery config tool and it
       explains the individual steps for configuring A+W Discovery successfully. Here, A+W Discovery
       assumes that an appropriate Microsoft SQL Server is installed on the target computer.




1.1. Configuring A+W Discovery

       The A+W Discovery installation is handled by the A+W SetupLauncher. It ensures that all
       resources required by the config tool are installed on the target computer. After this has happened,
       the SetupLauncher starts the A+W Discovery config tool. The first interface that appears looks like
       this:




03.07.2014                             US-Installations und Konfigurationsanleitung.docx                                                 1/22
                                           Figure 1: Start dialog


     In the beginning, the user is asked to specify the instance of the local SQL Server. If only the
     standard instance (unnamed instance) of the SQL Server is on the computer, this field must remain
     empty. This is due to the fact that in the SQL Server, the standard instance is not addressed by its
     instance name. Note: Currently in the config tool there is no remote configuration supported, so
     that no host can be entered here. Furthermore, it must be noted that – if there are several SQL
     Server instances on the computer – the SQL Server browser must be started since otherwise no
     connection to an instance can be established.

     In the second step, the entry of a user with administrative rights is requested. This user must be in
     the local administrator group of the computer. Furthermore, this update task also writes to the
     event log of the computer, which is only possible with such rights.



     If you click "Next" on the following two pages, the config tool checks whether:




03.07.2014                   US-Installations und Konfigurationsanleitung.docx                          2/22
         •   The specified user and password are correct and it is possible to log on with these.
         •   The user is in the administrator group.
         •   The instance can be found and a connection is possible.

     All three points must be fulfilled so that you can move to the next page. Here, the following is
     displayed:




                                      Figure 2: Optional de-installation


     Now it is possible to remove an optional A+W Discovery installation. It must be mentioned that
     A+W Discovery is not a normal "installation" of a program; instead, it is more the case that only the
     services of the respective SQL Server must be configured appropriately. Since the set-up for this
     must recognize the instance of the SQL Server, it runs within the config tool.



     A deinstallation checks and removes the following:




03.07.2014                   US-Installations und Konfigurationsanleitung.docx                          3/22
             •   All SQL Server tasks that start the data import and all previously-required authorizations
                 (log-ins, proxy, etc.).
             •   The SQL Server databases (DWH and Import).
             •   The SSIS packages within the integration services.
             •   The cube within the analysis services.

     Finally, the SQL Server is reset to its original state before installation.

     Next you will see the installation dialog:




                                             Figure 3: Installation dialog


     As soon as this view appears, there is an automatic background check as to whether A+W
     Discovery is installed correctly or whether an update is required.



     The update performs the following steps:




03.07.2014                        US-Installations und Konfigurationsanleitung.docx                       4/22
         1. The existing SSIS packages for the data import are updated.
         2. The existing cube is deleted and replaced with the current, empty cube. Important: all data
             previously in the cube is lost and therefore the cube must be processed anew. A complete
             new import of the data is not necessary since the DWH database is not deleted during an
             update.



     In case of a first installation, the following steps are performed:

         1. The database login is generated (SQL user "AWDiscovery_USR_SQL" with the server
             roles public and bulkadmin).
         2. The DWH and import databases are generated and added to the SQL user.
         3. Generation of a credential and proxy with the administrative user specified on the first
             dialog window.
         4. Creation of the two SQLServerAgent tasks for the daily import of the data. The tasks are
             performed under the previously-created proxy.
         5. If necessary, deletion of an already-existing A+W Discovery cube.
         6. Generation of the cube.
         7. Initialization of the databases (with statistical data).
         8. Initialization of the SSIS packages.

     Both for an update as well as for an installation, there is always a check in advance whether a
     connection to all services is possible and furthermore, whether these are configured correctly (start
     mode). Furthermore, the "FILESTREAM" option within the SQL Server is also read out and
     checked. If it is not active, this is indicated to the user in the config tool. During the installation in
     Figure 3, for example, you can see that the SQL ServerAgent is not configured appropriately. Here,
     however, the correct installation is not influenced. However the SQL ServerAgent must be
     configured manually after the fact since otherwise the future daily update cannot be performed
     successfully within the ServerAgent.

     For the update task with the designation "AWDiscovery_Update" it must also be mentioned that by
     default, it is performed daily at 3:00 am. Here, the data import is started and then – if no errors
     occurred during the import – the cube is built up again with the updated data. At the beginning and
     during the individual steps, there is also writing to the event log. If, due to network problems or
     similar, the task must be shifted to another time, then this must be set manually in SQL Server
     Management Studio.




03.07.2014                     US-Installations und Konfigurationsanleitung.docx                              5/22
     Furthermore, a second task called "AWDiscovery_CleanLogAndUpdateDate" is created, which
     cleans the internal data and keeps it consistent. This task is performed once on the last Sunday of
     the month at 10:00 pm. Here too, the manual time change applies.

     After the installation of A+W Discovery has been performed successfully, on the following dialog
     window, the following must be edited:




                                          Figure 4: Global settings


     The parameters listed here are necessary in order to ensure the data flow in the import and DWH
     databases. However, most of these are already specified and cannot be edited. Both variables
     Start year and Days in advance serve the internal date creation. Here, it is necessary to ensure
     that the configured interval (Start year until today + Days in advance) always covers the time
     period that the connected sites manage. If, for example, a site should be added that contains older
     data than the Start year, the Start year must be set back. The year specification is sufficient here
     since the beginning is always 01/01 of the year. The variable Days in advance ensures that future




03.07.2014                   US-Installations und Konfigurationsanleitung.docx                          6/22
     data values are also present. This variable may not be less than 31. Recommended here is the
     value 365.

     The (DWH) password can also be changed here that the AWDiscovery_USR_SQL-user should
     use to log on. By default, a default password is assigned here. After a password entry, there is a
     check to be sure the new password is valid and it does not violate any active password guideline. If
     this is the case, then this is indicated to the user with a warning messages on the lower part of the
     config tool. The SQL login applies for the DWH and import database. Important: if the password is
     changed after the fact, then you must ensure that change is also applied for already-existing sites.

     After a valid password entry, it takes a little while until the config tool has made all necessary
     changes. Here, the following steps are performed:

         1. The SQL login is assigned the new password (continue only if successful).
         2. The new password is transferred internally to all SSIS packages.
         3. The new password is set in the cube.

     After that, click "Next" to define the groups for sites that are created in the next step. However, this
     group definition is optional. For example, sites to be created here can be divided into regional
     groups or industries.




03.07.2014                    US-Installations und Konfigurationsanleitung.docx                           7/22
                                   Figure 5: Optional creation of groups


     After this step has been performed comes the actual creation of the various sites.




03.07.2014                   US-Installations und Konfigurationsanleitung.docx            8/22
                                         Figure 6: Creation of sites


     Here, sites to be imported (Business, Enterprise, and Production) can be created with "Add."
     Editing, copying, and deletion is also possible. When copying it must be noted that all values – but
     for the ID – are taken over from the original site. The following dialog appears:




03.07.2014                   US-Installations und Konfigurationsanleitung.docx                        9/22
                                   Figure 7: Selection of the module type


     First you must select what the type of the new site to be created should be. After you have made a
     seletion here, the type-specific, configurable parameters are loaded automatically.




03.07.2014                   US-Installations und Konfigurationsanleitung.docx                    10/22
     There is a listing of these parameters in Chapter 2.1.2. Here, the point is to explain in brief which
     parameters must absolutely be set for a successful import. In the beginning, the user can set a
     different ID than the one automatically specified. This option makes sense if for a site with e.g. ID =
     3 and type Production there is an additional type Enterprise. In this case, an additional Enterprise
     site with the same ID must be created. But: for one ID, the same type cannot be created several
     times.




03.07.2014                    US-Installations und Konfigurationsanleitung.docx                        11/22
     Next comes the specification of the database parameters. Here there is a distinction among the
     various supported database types Informix, SQLBase, and SQLServer. Depending on the type
     specified, the corresponding fields are adjusted or set to non-editable. For Informix, it must also be
     mentioned that here, its internal configuration (by Informix's own program SetNet) is executed
     automatically. Thus the user does not have to perform any additional Informix configuration in
     advance. But: if the site to be created is a SQLBase database, then the SQLBase "Connectivity
     Administrator" must be called in advance and the database server defined. Attention: for
     SQLBase it must also be noted that all required databases must have different names since the
     databases are only addressed using these.

     The correct entry of the database parameters in the config tool is indicated to the user after each
     editing and addition in the lower area with a connection test to the corresponding site.

     Another mandatory entry is the selection of the import database. If the import should always be up
     to the current day, then for "End date" only OFF should be specified (by setting disable in the date
     field). Later on, this causes the import to always import up to the current day. The start date causes
     processes to be imported that were changed since start date. But not recorded earlier than first
     date. Generally the specification of the correct date format through the "Date format" variable must
     be heeded since especially with the Informix driver (under DBDate), a date format can be specified
     that is used in the end. The "Import interval" variable handles the import of larger quantities of data
     and can be used in such a case to set the number of days (value > 0) that should be imported in a
     run. If, for example, data should be imported over a period of 2 years data, the import can be
     divided up into intervals of 100 day-steps. For this, you must only enter the value 100 in the
     variable. Thus – starting from start date – the data is imported in 100-day steps.

     Important: should the data for a site be imported in several import intervals, you must ensure that
     for this site there is one master data site (RunLevel on 1)

     In the end, for the import of a site it should be mentioned that this is always attempted several
     times or three times e.g. in case of network problems. The number of failed attempts is always
     documented in the event log.

     Next comes the "General," section where a definition and so-called RunLevel are defined. The
     latter is significant if, for example, there is a master data site that contains only the global master
     data for all sites. Such a one must contain the RunLevel 1 so that it is imported first. After all sites
     have been imported completely with such a RunLevel, then the sites with RunLevel 2, 3, etc.




03.07.2014                    US-Installations und Konfigurationsanleitung.docx                          12/22
     follow. Here it is generally sufficient to leave all other sites at RunLevel 2. Here too, it should be
     mentioned again that only for sites with RunLevel 1 can an ImportInterval be set.

     The "Global" rubric includes all parameters that are unique for a site. If for a site (ID) there should
     be several modules, then these parameters are the same for all modules and they are unique per
     site. Among other things, it is possible to specify an optional group from the previous dialog
     window here (if created). Important here, however, is the name of the site since it is used to create
     a corresponding local group on the computer and in the cube. The name of this group follows the
     following convention: "AWDiscovery Site <ID> <Name of the site>." If this name changes in a
     module, then the name is also changed for any other existing modules (with the same ID). The
     consequence of this is that the roles in the cube and in the Windows group are also renamed. By
     default, the role in the cube receives the limitation that only data for the respective site ID are
     visible and the corresponding, previously-created Windows group is assigned to it. Thus
     appropriate administrators can add the users (or groups) to the created Windows groups. The
     config tool creates only the corresponding groups.

     The last category is the "Master data," which is of special significance for customers with a central
     master data site. If, for example, there is a master data site with an ID = 1, then for the creation of
     another local site (ID = 2) there must be a reference to the first one:




03.07.2014                    US-Installations und Konfigurationsanleitung.docx                            13/22
                                     Figure 8: Configuration of master data


     Here, it can be specified individually for individual master data (item, models, etc.) where their
     reference should be sought. In the figure above, you can see that all master data refers to the
     master sites since all of these are set to its ID 1. If all master data is set to another ID, then the
     "ImportMasterData" option can be set to false. The effect of this is that no master data is imported
     for the current site.



     The field "House no." serves the internal site capability of the individual modules. Thus, for
     example, Enterprise is in a position to manage several internal houses within a site. Such a
     constellation must be created within the config tool as follows:

         •   Each internal house is created as an individual site (each has its own ID), whereby each
             site has is own module-specific house no.
                 o   And: for the first site created, the "ImportMasterData" switch is set to true and for all
                     others to false. Furthermore, for the latter the reference of the individual master data
                     must be set to the ID of the first site created.




03.07.2014                    US-Installations und Konfigurationsanleitung.docx                           14/22
       After these steps have been performed, a new site is successfully created and the configuration
       is complete.



       Now end users can use Excel to access the cube and its contents. These A+W Discovery reports
       are in "...\A+W\A+W Discovery\Resources\Documents" and on first opening, the data connection
       must be adjusted to the cube, since here by default the correct connection character string is not
       defined.


1.2. Available parameters

       Below is a list of all the parameters, only some of which may be edited by the user.


                                                                                   Read    Extended
       Display name      Description     Category            Default value
                                                                                   only       property


                          Count of
       Max. Parallel    concurrently
                                          General                  1                 1           1
         Packages         running
                         packages

             Import    Opt. Appendix                        Persist Security
                                           Import
        Connection       for import                         Info=True;Auto           1           1
                                         Connection
         Appendix        connection                        Translate=False;

                       DB Provider for
         Import DB                         Import
                           Import                             Internal set           1           1
         Provider                        Connection
                        Connection

                          Name of
             Import                        Import
                        database for                     AWDiscovery_Import          1           0
         Database                        Connection
                           import

                           Server
       Import Server                       Import
                       (Host\Instance)                                               1           0
             Name                        Connection
                         for import




03.07.2014                   US-Installations und Konfigurationsanleitung.docx                           15/22
                                                                                 Read   Extended
       Display name     Description      Category            Default value
                                                                                 only   property


                       Username for
             Import                        Import
                           Import                     AWDiscovery_USR_SQL         1        0
        Username                         Connection
                        Connection

                        Password for
             Import                        Import
                           Import                            AWdiscovery!         1        0
         Password                        Connection
                        Connection

              DWH      Opt. Appendix                        Persist Security
                                           DWH
        Connection        for DWH                           Info=True;Auto        1        1
                                         Connection
         Appendix       Connection                         Translate=False;

                        Provider for
         DWH DB                            DWH
                           DWH                                Internal set        1        1
         Provider                        Connection
                        Connection

                          Name of
              DWH                          DWH
                        database for                         AWDiscovery          1        0
         Database                        Connection
                           DWH

                           Server
       DWH Server                          DWH
                       (Host\Instance)                                            1        0
             Name                        Connection
                          for DWH

                       Username for
              DWH                          DWH
                           DWH                        AWDiscovery_USR_SQL         1        0
        Username                         Connection
                        Connection

                        Password for
              DWH                          DWH
                           DWH                               AWdiscovery!         0        0
         Password                        Connection
                        Connection



         Installed     AWDiscovery        General                                 1        0
             Version    Version No.




03.07.2014                   US-Installations und Konfigurationsanleitung.docx                     16/22
                                                                                             Read        Extended
       Display name       Description       Category              Default value
                                                                                             only        property



       Language ID       Language ID         General                     4                    1             1



                         Start year for
         Start year       insert data        General                   2008                   0             0
                        stamp into db

                            Days in
             Days in     advance for
                                             General                    365                   0             0
          advance         insert data
                        stamp into db


              SSIS      AW Discovery
                                             General                                          1             1
         Package           Package



        SSIS Date       AW Discovery         General                                          1             1


                              Figure 9: Description of the available, global variables




       As well as a list of all available parameters for the creation of a site:

                                                                                               Read
         Display name        Description      Category        Module         Default value                  Extended
                                                                                                  only

                               Kind of
              Module                          Identifiers      E,B,P                                0           0
                               module

                                ID for
               SiteID                              “              “                                 0           0
                             subsidiary




03.07.2014                     US-Installations und Konfigurationsanleitung.docx                                    17/22
                                                                                       Read
         Display name      Description      Category       Module     Default value           Extended
                                                                                       only

                            Database
        Database Type                       Connection        “             null        0        0
                               Type

                             Name of
              Database                          “             “             null        0        0
                             database

                           Host@server
         Server Name                            “             “                         0        0
                           or db name

                             User for
             Username                           “             “          alcimdb        0        0
                             database

              Password      Password            “             “                         0        0

                               Opt.
             Connection
                           appendix for         “             “                         0        1
              Appendix
                            connection

                           Servicename
        Servicename \
                               \ Port           “             “                         0        0
                Port
                            (Informix)

         Client Locale     Client Locale        “             “        en_US.1252       0        0

                            Database
             DB Locale                          “             “      en_us.CP1252       0        0
                              Locale

             DB Provider     Provider           “             “         internal set    1        1

                            Format of       Date and
         Date Format                                          “        yyyy-MM-dd       0        0
                               date           Time

                           Start date for
              Start date                        “             “                         0        0
                              import

                           End date for
              End date                          “             “            OFF          0        0
                              import




03.07.2014                    US-Installations und Konfigurationsanleitung.docx                      18/22
                                                                                       Read
         Display name       Description       Category      Module     Default value          Extended
                                                                                       only

                            Import date
             First date     for changed           “            “                        0        0
                               orders

                               Import
        Import interval      interval ( in        “            “              0         0        0
                                days)

                            Only relevant
       End interval date     in case of           “            “                        1        1
                               failure

             Description    Description       General          “        Description     0        0

             RunLevel        RunLevel             “            “              2         0        0

               Group           Group           Global          “                        0        0

                            Unique name
         Name for site                            “            “         SiteName       0        0
                               for site

                             Symbol for                                  SiteName
        Symbol for site                           “            “                        0        0
                                 site                                       short

                            Locale ID for
             Locale ID                            “            “            Null        0        0
                                 site

                               Internal
             House No.                       Master data     E, B            -1         0        0
                              house no

                            Master data
                             import for
       ImportMasterData                           ”            E                        0        0
                                 site
                            (replication)

                               Site for
        Site for articles      master             ”           E,B                       0        1
                               articles




03.07.2014                     US-Installations und Konfigurationsanleitung.docx                     19/22
                                                                                       Read
         Display name        Description     Category       Module     Default value          Extended
                                                                                       only

                               Site for
         Site for claim
                             master claim        ”             ”                        0        1
                place
                                place

                               Site for
         Site for claim
                             master claim        ”             ”                        0        1
               reasons
                               reasons

                               Site for
       Site for claim type master claim          ”             E                        0        1
                                 type

                               Site for
             Site for cost
                             master cost         ”           E, B                       0        1
               centers
                               centers

                               Site for
       Site for customer       master            ”             ”                        0        1
                              customers

                               Site for
       Site for customer       master
                                                 ”             ”                        0        1
               delivery       customer
                               delivery

                               Site for
       Site for economic       master
                                                 ”             E                        0        1
                region        economic
                                region

                               Site for
        Site for kind of
                             master kind         ”             B                        0        1
                order
                               of order




03.07.2014                     US-Installations und Konfigurationsanleitung.docx                     20/22
                                                                                      Read
         Display name       Description     Category       Module     Default value          Extended
                                                                                      only

                              Site for
         Site for model       master            ”             ”                        0        1
                              model

                              Site for
         Site for object                        ”             B                        0        1
                           master object

                              Site for
        Site for product      master
                                                “           E, B                       0        1
             groups          product
                              groups

                              Site for
         Site for rebate      master
                                                ”             E                        0        1
             method           rebate
                             method

                              Site for
         Site for sales
                           master sales         ”           E, B                       0        1
        representatives
                               rep.

                              Site for
         Site for status                        ”             B                        0        1
                           master status

                              Site for
        Site for supply       master            ”             B                        0        1
                              supply

                              Site for
        Site for type of
                           master type          ”           E, B                       0        1
             dispatch
                             of disp.

                              Site for
        Site for type of
                           master type          ”             ”                        0        1
             package
                             of pack.




03.07.2014                    US-Installations und Konfigurationsanleitung.docx                     21/22
2. Error handling

     If an error should occur during data import or cube construction, these are always stored
     permanently under the following components:

         •       Table sysssislog (present both in AWDiscovery as well as in AWDiscovery_Import
                 database)

         •       Event log ("application") of the computer under "AWDiscovery"

       Errors within the config tool and the A+W Discovery set-up are logged as follows:

             •    On each start, the config tool writes to a log file with an appropriate date stamp. The log
                  file is usually written away under the LogDir registry entry (usually: "C:\Program
                  Files(x86)\A+W\Installation Log"). If this entry is not present, then it is in the installation
                  folder of A+W Discovery (usually: "C:\Program Files (x86)\A+W\A+W Discovery"). There,
                  under "\Resources\Log" there is also a log file of the set-up, which is written continuously.




2.1. Configuration of the SQL Server services

The following table shows all required services with their start mode and "log on as" status. To be
heeded is also that the start mode does not prevent a successful starting of a service.

                 Name                    Start Mode                              Log On As

      Integration Services                Automatic              NT AUTHORITY\NETWORKSERVICE

        Analysis Services                      “                              .\awsqlsvradmin

             SQL Server                        ““                              LocalSystem

       SQL Server Agent                        “                              .\awsqlsvradmin

      SQL Server Browser                       “                               LocalSystem



For the SQL Server service, it must also be mentioned that here too attention must be paid to the
respective instance (if there are several instances on the system).




03.07.2014                        US-Installations und Konfigurationsanleitung.docx                            22/22

